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
# <a name="custom-query-specification"></a><span data-ttu-id="d5a7d-103">Спецификация пользовательского запроса</span><span class="sxs-lookup"><span data-stu-id="d5a7d-103">Custom query specification</span></span>

<span data-ttu-id="d5a7d-104">Партнеры могут использовать эту спецификацию запроса, чтобы легко формировать пользовательские запросы на извлечение данных из таблиц аналитики.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="d5a7d-105">Запросы можно использовать для выбора только нужных столбцов и метрик, соответствующих определенному условию.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="d5a7d-106">В основе спецификации языка лежит определение набора данных, по которому можно написать пользовательский запрос.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="d5a7d-107">Наборы данных</span><span class="sxs-lookup"><span data-stu-id="d5a7d-107">Datasets</span></span>

<span data-ttu-id="d5a7d-108">Так же как некоторые запросы выполняются для базы данных, которая содержит таблицы и столбцы, пользовательский запрос работает с наборами, состоящими из столбцов и метрик.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="d5a7d-109">Полный список доступных наборов данных для составления запросов можно получить с помощью API наборов данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="d5a7d-110">Ниже приведен пример набора данных, показанного в виде JSON:</span><span class="sxs-lookup"><span data-stu-id="d5a7d-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="d5a7d-111">Части набора данных</span><span class="sxs-lookup"><span data-stu-id="d5a7d-111">Parts of a dataset</span></span>

- <span data-ttu-id="d5a7d-112">Имя набора данных похоже на имя таблицы в базе данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="d5a7d-113">Например, Оффицеусаже.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-113">For example, OfficeUsage.</span></span> <span data-ttu-id="d5a7d-114">Набор данных содержит список столбцов, которые можно выбрать, например Кустомертенантид.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="d5a7d-115">Набор данных также имеет метрики, которые подобны статистическим функциям в базе данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="d5a7d-116">Например, Тоталмонсляктивеусерс.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="d5a7d-117">Существуют фиксированные интервалы времени, в течение которых можно экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="d5a7d-118">Составление запроса по набору данных</span><span class="sxs-lookup"><span data-stu-id="d5a7d-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="d5a7d-119">Ниже приведены примеры запросов, извлекающих различные типы данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="d5a7d-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a7d-120">Query</span></span>|    <span data-ttu-id="d5a7d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d5a7d-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="d5a7d-122">**Выберите** Кустомертенантид **, паидаваилаблеунитс**</span><span class="sxs-lookup"><span data-stu-id="d5a7d-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="d5a7d-123">Оффицеусаже **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="d5a7d-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="d5a7d-124">Этот запрос получит все Кусотмертенантид и соответствующие Паидаваилаблеунитс за последний месяц.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="d5a7d-125">**Выберите** Кустомертенантид **, паидаваилаблеунитс**</span><span class="sxs-lookup"><span data-stu-id="d5a7d-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="d5a7d-126">Оффицеусаже **Order** by паидаваилаблеунитс **ограничение** 10</span><span class="sxs-lookup"><span data-stu-id="d5a7d-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="d5a7d-127">Этот запрос получает 10 лучших клиентов клиентов в порядке убывания количества платных доступных единиц.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="d5a7d-128">**Выберите** Кустомертенантид, Паидаваилаблеунитс, Монсляктивеусерс **из** Оффицеусаже, **где** МОНСЛЯКТИВЕУСЕРС > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="d5a7d-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="d5a7d-129">Этот запрос получит Паидаваилаблеунитс и Монсляктивеусерс всех клиентов, у которых Монсляктивеусерс больше 100 000.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="d5a7d-130">**Выберите** Кустомертенантид, месяц, Монсляктивеусерс **из**</span><span class="sxs-lookup"><span data-stu-id="d5a7d-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="d5a7d-131">Оффицеусаже, **где** кустомертпид in (' 2a31c234-1f4e-4c60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-b378-0242ac130002 ')</span><span class="sxs-lookup"><span data-stu-id="d5a7d-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="d5a7d-132">Этот запрос будет получать Кустомертенантид и ежемесячно активных пользователей за каждый месяц на два значения Кустомертпид: ' 2a31c234-1f4e-4c60-909e-76d234f93161 ' и ' 80780748-3f9a-11eb-b378-0242ac130002 '.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="d5a7d-133">Спецификация запроса</span><span class="sxs-lookup"><span data-stu-id="d5a7d-133">Query specification</span></span>

<span data-ttu-id="d5a7d-134">В этом разделе описывается определение и структура запроса.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="d5a7d-135">Справочник по грамматике</span><span class="sxs-lookup"><span data-stu-id="d5a7d-135">Grammar reference</span></span>

<span data-ttu-id="d5a7d-136">В этой таблице дано описание символов, используемых в запросах.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="d5a7d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a7d-137">Query</span></span>    |    <span data-ttu-id="d5a7d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d5a7d-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="d5a7d-139">Необязательно</span><span class="sxs-lookup"><span data-stu-id="d5a7d-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="d5a7d-140">Ноль или более</span><span class="sxs-lookup"><span data-stu-id="d5a7d-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="d5a7d-141">Один или более</span><span class="sxs-lookup"><span data-stu-id="d5a7d-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="d5a7d-142">Или один из списков</span><span class="sxs-lookup"><span data-stu-id="d5a7d-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="d5a7d-143">Определение запроса</span><span class="sxs-lookup"><span data-stu-id="d5a7d-143">Query definition</span></span>

<span data-ttu-id="d5a7d-144">Инструкция запроса имеет следующие предложения: SelectClause, Фромклаусе, Вхереклаусе, Ордерклаусе, Лимитклаусе и TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="d5a7d-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="d5a7d-146">**ColumOrMetricName**: столбцы и метрики, которые определены в наборе данных</span><span class="sxs-lookup"><span data-stu-id="d5a7d-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="d5a7d-147">**Фромклаусе**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="d5a7d-148">**DatasetName**: имя набора данных, которое определено в наборе данных</span><span class="sxs-lookup"><span data-stu-id="d5a7d-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="d5a7d-149">**Вхереклаусе**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="d5a7d-150">**FilterCondition**: ColumOrMetricName Operator Value</span><span class="sxs-lookup"><span data-stu-id="d5a7d-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="d5a7d-151">**Оператор**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="d5a7d-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="d5a7d-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="d5a7d-153">**Число**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="d5a7d-154">**Стринглитерал**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="d5a7d-155">**Мултинумберлист**: `(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="d5a7d-156">**Мултистринглист**: `(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="d5a7d-157">**Ордерклаусе**: `ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="d5a7d-158">**Ордеркондитион**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="d5a7d-159">**Лимитклаусе**: `LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="d5a7d-160">**Интервал** времени: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="d5a7d-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="d5a7d-161">Структура запроса</span><span class="sxs-lookup"><span data-stu-id="d5a7d-161">Query Structure</span></span>

<span data-ttu-id="d5a7d-162">Запрос отчета состоит из нескольких частей:</span><span class="sxs-lookup"><span data-stu-id="d5a7d-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="d5a7d-163">Каждая часть описана ниже.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="d5a7d-164">В этой части запроса указываются столбцы, которые будут экспортированы.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="d5a7d-165">Столбцы, которые могут быть выбраны, — это поля, перечисленные в разделах *селектаблеколумнс* и *аваилаблеметрикс* набора данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="d5a7d-166">При необходимости `DISTINCT` ключевое слово может быть указано после `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="d5a7d-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="d5a7d-167">Если `DISTINCT` указан параметр, то итоговые экспортированные строки всегда будут содержать отдельные значения выбранных столбцов.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="d5a7d-168">Метрики будут рассчитываться для каждого отдельного сочетания выбранных столбцов, поэтому `DISTINCT` ключевое слово не требуется, если столбец метрики включен в список Выбор столбцов.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="d5a7d-169">**Пример**.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="d5a7d-170">Эта часть запроса определяет набор данных, из которого необходимо экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="d5a7d-171">Имя набора данных, указанное здесь, должно быть допустимым именем набора данных, возвращаемым API наборов данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="d5a7d-172">**Пример**.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="d5a7d-173">Эта часть запроса используется для указания условий фильтра для набора данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="d5a7d-174">В окончательном экспортированном файле будут присутствовать только строки, соответствующие условиям, указанным в этом предложении.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="d5a7d-175">Условие фильтра может находиться в любом из столбцов, перечисленных в *селектаблеколумнс* и *аваилаблеметрикс*.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="d5a7d-176">Значения, указанные в условии фильтра, могут представлять собой список чисел или список строк только в том случае, если оператор имеет значение `IN` или `NOT IN`.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="d5a7d-177">Значения всегда могут быть заданы в виде литеральной строки, и они будут преобразованы в собственные типы столбцов.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="d5a7d-178">Несколько условий фильтра должны быть разделены операцией и.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="d5a7d-179">**Пример**.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="d5a7d-180">В этой части запроса указываются критерии упорядочивания для экспортируемых строк.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="d5a7d-181">Столбцы, для которых может быть определен порядок сортировки, должны быть из *селектаблеколумнс* и *аваилаблеметрикс* набора данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="d5a7d-182">Если направление упорядочивания не указано, по умолчанию оно будет иметь значение DESC для столбца.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="d5a7d-183">Упорядочивание можно определить по нескольким столбцам, разделяя критерий запятой.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="d5a7d-184">**Пример**.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="d5a7d-185">В этой части запроса указывается количество строк, которые будут экспортированы.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="d5a7d-186">Указанное число должно быть положительным ненулевым целым числом.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="d5a7d-187">В этой части запроса указывается период времени, в течение которого необходимо экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="d5a7d-188">Возможные значения должны быть из поля *аваилабледатеранжес* в определении набора данных.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="d5a7d-189">Чувствительность к регистру в спецификации запроса</span><span class="sxs-lookup"><span data-stu-id="d5a7d-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="d5a7d-190">Регистр символов в спецификации полностью игнорируется.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="d5a7d-191">Предопределенные ключевые слова, имена и значения столбцов можно указывать с помощью прописных и строчных символов.</span><span class="sxs-lookup"><span data-stu-id="d5a7d-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d5a7d-192">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d5a7d-192">Next steps</span></span>

- [<span data-ttu-id="d5a7d-193">Список системных запросов</span><span class="sxs-lookup"><span data-stu-id="d5a7d-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="d5a7d-194">Список примеров запросов</span><span class="sxs-lookup"><span data-stu-id="d5a7d-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)