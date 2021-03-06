---
title: получение Аналитика данных API запросов к отчетам
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Этот API используется для получения всех доступных запросов для использования в API отчетов.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376126"
---
# <a name="get-report-queries-api"></a>API получения запросов отчетов

API получения отчетов о запросах получает все запросы, доступные для использования в отчетах. Он получает все системные и пользовательские запросы по умолчанию.

**Синтаксис запроса**

|    Метод    |    Универсальный код ресурса (URI) запроса    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**Заголовок запроса**

|    Заголовок    |    Тип    |    Описание    |
|    ----    |    ----    |    ----    |
|    Авторизация    |    строка    |    Обязательный. маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`    |
|    Content-Type    |    строка    |    `Application/JSON`    |
|        |        |        |

**Параметр пути**

Нет

**Параметр запроса**

|    имени параметра    |    Тип    |    Обязательно    |    Описание    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    строка     |    Нет    |    Фильтр для получения сведений только о запросах с идентификатором, заданным в аргументе     |
|    queryName     |    строка     |    Нет    |    Фильтр для получения сведений только о запросах с именем, заданным в аргументе     |
|    инклудесистемкуериес     |    Логическое     |    Нет    |    Включить в ответ стандартные системные запросы     |
|    инклудеонлисистемкуериес     |    Логическое     |    Нет    |    Включить в ответ только системные запросы     |
|        |        |        |        |


**Полезные данные запроса**

Нет

**Словарь терминов**

Нет

**Ответ**

Полезные данные ответа имеют следующий формат:

Код отклика: 200, 400, 401, 403, 404, 500

Пример полезных данных ответа:

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

**Словарь терминов**

В следующей таблице описаны ключевые элементы ответа.

|    Параметр    |    Описание    |
|    ----    |    ----    |
|    QueryId     |    Уникальный UUID запроса     |
|    Имя     |    Имя, присвоенное запросу при создании запроса     |
|    Описание     |    Описание, заданное при создании запроса     |
|    Запрос     |    Строка запроса отчета     |
|    Тип     |    Задайте значение Пользователяопределенные для созданных пользователем запросов и системы для предопределенных системных запросов.     |
|    Пользователь     |    Идентификатор пользователя, создавшего запрос     |
|    CreatedTime     |    Время создания запроса     |
|    TotalCount     |    Количество наборов данных в массиве Value     |
|    Сообщение     |    Сообщение о состоянии из выполнения API     |
|    StatusCode     |    Код результата. Возможные значения: 200, 400, 401, 403, 500     |
|        |        |
