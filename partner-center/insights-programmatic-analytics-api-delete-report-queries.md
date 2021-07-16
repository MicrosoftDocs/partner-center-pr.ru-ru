---
title: удаление запросов отчета API — Аналитика данных
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API для удаления определяемого пользователем запроса в центре партнеров Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375885"
---
# <a name="delete-report-queries-api"></a>API удаления запросов отчетов

Этот API позволяет удалять определяемые пользователем запросы.

**Синтаксис запроса**

|    Метод    |    Универсальный код ресурса (URI) запроса    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**Заголовок запроса**

|    Заголовок    |    Тип    |    Описание    |
|    ----    |    ----    |    ----    |
|    Авторизация    |    строка    |    Обязательный. маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`    |
|    Content-Type    |    строка    |    `Application/JSON`    |
|        |        |        |

**Параметр пути**

|    имени параметра    |    Тип    |    Обязательно    |    Описание    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    строка     |    Нет    |    Фильтр для получения сведений только о запросах с идентификатором, заданным в аргументе     |
|        |        |        |        |

**Параметр запроса**

Нет

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
|    QueryId     |    Уникальный UUID удаленного запроса    |
|    Имя     |    Имя удаленного запроса    |
|    Описание     |    Описание удаленного запроса     |
|    Запрос     |    Строка запроса отчета для удаленного запроса    |
|    Тип     |    Задайте значение Пользователяопределенные для запросов, созданных пользователем.     |
|    Пользователь     |    Идентификатор пользователя, создавшего запрос     |
|    CreatedTime     |    Время создания запроса     |
|    TotalCount     |    Количество наборов данных в массиве Value     |
|    Сообщение     |    Сообщение о состоянии из выполнения API     |
|    StatusCode     |    Код результата. Возможные значения: 200, 400, 401, 403, 500     |
|        |        |
