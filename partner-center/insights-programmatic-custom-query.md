---
title: Спецификация пользовательского запроса
description: Узнайте, как создавать пользовательские запросы для извлечения данных из таблиц аналитики.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376070"
---
# <a name="custom-query-specification"></a>Спецификация пользовательского запроса

Партнеры могут использовать эту спецификацию запроса, чтобы легко формировать пользовательские запросы на извлечение данных из таблиц аналитики. Запросы можно использовать для выбора только нужных столбцов и метрик, соответствующих определенному условию. В основе спецификации языка лежит определение набора данных, по которому можно написать пользовательский запрос.

## <a name="datasets"></a>Наборы данных

Так же как некоторые запросы выполняются для базы данных, которая содержит таблицы и столбцы, пользовательский запрос работает с наборами, состоящими из столбцов и метрик. Полный список доступных наборов данных для составления запросов можно получить с помощью API наборов данных.

Ниже приведен пример набора данных, показанного в виде JSON:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Части набора данных

- Имя набора данных похоже на имя таблицы в базе данных. Например, Оффицеусаже. Набор данных содержит список столбцов, которые можно выбрать, например Кустомертенантид.
- Набор данных также имеет метрики, которые подобны статистическим функциям в базе данных. Например, Тоталмонсляктивеусерс.
- Существуют фиксированные интервалы времени, в течение которых можно экспортировать данные.

## <a name="formulating-a-query-on-a-dataset"></a>Составление запроса по набору данных

Ниже приведены примеры запросов, извлекающих различные типы данных.

|Запрос|    Описание    |
|----|    ----    |
|**Выберите** Кустомертенантид **, паидаваилаблеунитс** <br>Оффицеусаже **TIMESPAN** LAST_MONTH|    Этот запрос получит все Кусотмертенантид и соответствующие Паидаваилаблеунитс за последний месяц.    |
|**Выберите** Кустомертенантид **, паидаваилаблеунитс** <br>Оффицеусаже **Order** by паидаваилаблеунитс **ограничение** 10|    Этот запрос получает 10 лучших клиентов клиентов в порядке убывания количества платных доступных единиц.     |
|**Выберите** Кустомертенантид, Паидаваилаблеунитс, Монсляктивеусерс **из** Оффицеусаже, **где** МОНСЛЯКТИВЕУСЕРС > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Этот запрос получит Паидаваилаблеунитс и Монсляктивеусерс всех клиентов, у которых Монсляктивеусерс больше 100 000.     |
|**Выберите** Кустомертенантид, месяц, Монсляктивеусерс **из** <br>Оффицеусаже, **где** кустомертпид in (' 2a31c234-1f4e-4c60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-b378-0242ac130002 ') |    Этот запрос будет получать Кустомертенантид и ежемесячно активных пользователей за каждый месяц на два значения Кустомертпид: ' 2a31c234-1f4e-4c60-909e-76d234f93161 ' и ' 80780748-3f9a-11eb-b378-0242ac130002 '.     |
|        |        |

## <a name="query-specification"></a>Спецификация запроса

В этом разделе описывается определение и структура запроса.

## <a name="grammar-reference"></a>Справочник по грамматике

В этой таблице дано описание символов, используемых в запросах.

|    Запрос    |    Описание    |
|    ----    |    ----    |
|    `?`    |    Необязательно    |
|    `*`    |    Ноль или более    |
|    `+`    |    Один или более    |
|    `\|`    |    Или один из списков    |
|        |        |

## <a name="query-definition"></a>Определение запроса

Инструкция запроса имеет следующие предложения: SelectClause, Фромклаусе, Вхереклаусе, Ордерклаусе, Лимитклаусе и TimeSpan.

- **SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName**: столбцы и метрики, которые определены в наборе данных
- **Фромклаусе**: `FROM DatasetName`
    - **DatasetName**: имя набора данных, которое определено в наборе данных
- **Вхереклаусе**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition**: ColumOrMetricName Operator Value
        - **Оператор**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Value**: Number | StringLiteral | MultiNumberList | MultiStringList
            - **Число**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **Стринглитерал**:  `' [a-zA-Z0-9_]*'`
            - **Мултинумберлист**: `(Number (,Number)*)`
            - **Мултистринглист**: `(StringLiteral (,StringLiteral)*)`
- **Ордерклаусе**: `ORDER BY OrderCondition (,OrderCondition)`
    - **Ордеркондитион**: `ColumOrMetricName (ASC | DESC)*`
- **Лимитклаусе**: `LIMIT [0-9]+`
- **Интервал** времени: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Структура запроса

Запрос отчета состоит из нескольких частей:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Каждая часть описана ниже.

### `SELECT`

В этой части запроса указываются столбцы, которые будут экспортированы. Столбцы, которые могут быть выбраны, — это поля, перечисленные в разделах *селектаблеколумнс* и *аваилаблеметрикс* набора данных.

При необходимости `DISTINCT` ключевое слово может быть указано после `SELECT` . Если `DISTINCT` указан параметр, то итоговые экспортированные строки всегда будут содержать отдельные значения выбранных столбцов. Метрики будут рассчитываться для каждого отдельного сочетания выбранных столбцов, поэтому `DISTINCT` ключевое слово не требуется, если столбец метрики включен в список Выбор столбцов.

**Пример**.

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Эта часть запроса определяет набор данных, из которого необходимо экспортировать данные. Имя набора данных, указанное здесь, должно быть допустимым именем набора данных, возвращаемым API наборов данных.

**Пример**.

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Эта часть запроса используется для указания условий фильтра для набора данных. В окончательном экспортированном файле будут присутствовать только строки, соответствующие условиям, указанным в этом предложении. Условие фильтра может находиться в любом из столбцов, перечисленных в *селектаблеколумнс* и *аваилаблеметрикс*. Значения, указанные в условии фильтра, могут представлять собой список чисел или список строк только в том случае, если оператор имеет значение `IN` или `NOT IN`. Значения всегда могут быть заданы в виде литеральной строки, и они будут преобразованы в собственные типы столбцов. Несколько условий фильтра должны быть разделены операцией и.

**Пример**.

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

В этой части запроса указываются критерии упорядочивания для экспортируемых строк. Столбцы, для которых может быть определен порядок сортировки, должны быть из *селектаблеколумнс* и *аваилаблеметрикс* набора данных. Если направление упорядочивания не указано, по умолчанию оно будет иметь значение DESC для столбца. Упорядочивание можно определить по нескольким столбцам, разделяя критерий запятой.

**Пример**.

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

В этой части запроса указывается количество строк, которые будут экспортированы. Указанное число должно быть положительным ненулевым целым числом.

### `TIMESPAN`

В этой части запроса указывается период времени, в течение которого необходимо экспортировать данные. Возможные значения должны быть из поля *аваилабледатеранжес* в определении набора данных.

### <a name="case-sensitivity-in-query-specification"></a>Чувствительность к регистру в спецификации запроса

Регистр символов в спецификации полностью игнорируется. Предопределенные ключевые слова, имена и значения столбцов можно указывать с помощью прописных и строчных символов.

## <a name="next-steps"></a>Дальнейшие действия

- [Список системных запросов](insights-programmatic-system-queries.md)
- [Список примеров запросов](insights-programmatic-sample-queries.md)