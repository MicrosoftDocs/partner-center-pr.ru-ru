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
# <a name="delete-report-queries-api"></a><span data-ttu-id="86698-103">API удаления запросов отчетов</span><span class="sxs-lookup"><span data-stu-id="86698-103">Delete report queries API</span></span>

<span data-ttu-id="86698-104">Этот API позволяет удалять определяемые пользователем запросы.</span><span class="sxs-lookup"><span data-stu-id="86698-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="86698-105">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="86698-105">**Request syntax**</span></span>

|    <span data-ttu-id="86698-106">Метод</span><span class="sxs-lookup"><span data-stu-id="86698-106">Method</span></span>    |    <span data-ttu-id="86698-107">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="86698-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="86698-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="86698-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="86698-109">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="86698-109">**Request header**</span></span>

|    <span data-ttu-id="86698-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86698-110">Header</span></span>    |    <span data-ttu-id="86698-111">Тип</span><span class="sxs-lookup"><span data-stu-id="86698-111">Type</span></span>    |    <span data-ttu-id="86698-112">Описание</span><span class="sxs-lookup"><span data-stu-id="86698-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="86698-113">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86698-113">Authorization</span></span>    |    <span data-ttu-id="86698-114">строка</span><span class="sxs-lookup"><span data-stu-id="86698-114">string</span></span>    |    <span data-ttu-id="86698-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86698-115">Required.</span></span> <span data-ttu-id="86698-116">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="86698-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="86698-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86698-117">Content-Type</span></span>    |    <span data-ttu-id="86698-118">строка</span><span class="sxs-lookup"><span data-stu-id="86698-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="86698-119">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="86698-119">**Path parameter**</span></span>

|    <span data-ttu-id="86698-120">имени параметра</span><span class="sxs-lookup"><span data-stu-id="86698-120">Parameter Name</span></span>    |    <span data-ttu-id="86698-121">Тип</span><span class="sxs-lookup"><span data-stu-id="86698-121">Type</span></span>    |    <span data-ttu-id="86698-122">Обязательно</span><span class="sxs-lookup"><span data-stu-id="86698-122">Required</span></span>    |    <span data-ttu-id="86698-123">Описание</span><span class="sxs-lookup"><span data-stu-id="86698-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="86698-124">queryId</span><span class="sxs-lookup"><span data-stu-id="86698-124">queryId</span></span>     |    <span data-ttu-id="86698-125">строка</span><span class="sxs-lookup"><span data-stu-id="86698-125">string</span></span>     |    <span data-ttu-id="86698-126">Нет</span><span class="sxs-lookup"><span data-stu-id="86698-126">No</span></span>    |    <span data-ttu-id="86698-127">Фильтр для получения сведений только о запросах с идентификатором, заданным в аргументе</span><span class="sxs-lookup"><span data-stu-id="86698-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="86698-128">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="86698-128">**Query parameter**</span></span>

<span data-ttu-id="86698-129">Нет</span><span class="sxs-lookup"><span data-stu-id="86698-129">None</span></span>

<span data-ttu-id="86698-130">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="86698-130">**Request payload**</span></span>

<span data-ttu-id="86698-131">Нет</span><span class="sxs-lookup"><span data-stu-id="86698-131">None</span></span>

<span data-ttu-id="86698-132">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="86698-132">**Glossary**</span></span>

<span data-ttu-id="86698-133">Нет</span><span class="sxs-lookup"><span data-stu-id="86698-133">None</span></span>

<span data-ttu-id="86698-134">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="86698-134">**Response**</span></span>

<span data-ttu-id="86698-135">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="86698-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="86698-136">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="86698-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="86698-137">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="86698-137">Response payload example:</span></span>

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

<span data-ttu-id="86698-138">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="86698-138">**Glossary**</span></span>

<span data-ttu-id="86698-139">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="86698-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="86698-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="86698-140">Parameter</span></span>    |    <span data-ttu-id="86698-141">Описание</span><span class="sxs-lookup"><span data-stu-id="86698-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="86698-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="86698-142">QueryId</span></span>     |    <span data-ttu-id="86698-143">Уникальный UUID удаленного запроса</span><span class="sxs-lookup"><span data-stu-id="86698-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="86698-144">Имя</span><span class="sxs-lookup"><span data-stu-id="86698-144">Name</span></span>     |    <span data-ttu-id="86698-145">Имя удаленного запроса</span><span class="sxs-lookup"><span data-stu-id="86698-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="86698-146">Описание</span><span class="sxs-lookup"><span data-stu-id="86698-146">Description</span></span>     |    <span data-ttu-id="86698-147">Описание удаленного запроса</span><span class="sxs-lookup"><span data-stu-id="86698-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="86698-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="86698-148">Query</span></span>     |    <span data-ttu-id="86698-149">Строка запроса отчета для удаленного запроса</span><span class="sxs-lookup"><span data-stu-id="86698-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="86698-150">Тип</span><span class="sxs-lookup"><span data-stu-id="86698-150">Type</span></span>     |    <span data-ttu-id="86698-151">Задайте значение Пользователяопределенные для запросов, созданных пользователем.</span><span class="sxs-lookup"><span data-stu-id="86698-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="86698-152">Пользователь</span><span class="sxs-lookup"><span data-stu-id="86698-152">User</span></span>     |    <span data-ttu-id="86698-153">Идентификатор пользователя, создавшего запрос</span><span class="sxs-lookup"><span data-stu-id="86698-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="86698-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="86698-154">CreatedTime</span></span>     |    <span data-ttu-id="86698-155">Время создания запроса</span><span class="sxs-lookup"><span data-stu-id="86698-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="86698-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="86698-156">TotalCount</span></span>     |    <span data-ttu-id="86698-157">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="86698-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="86698-158">Сообщение</span><span class="sxs-lookup"><span data-stu-id="86698-158">Message</span></span>     |    <span data-ttu-id="86698-159">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="86698-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="86698-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="86698-160">StatusCode</span></span>     |    <span data-ttu-id="86698-161">Код результата.</span><span class="sxs-lookup"><span data-stu-id="86698-161">Result Code.</span></span> <span data-ttu-id="86698-162">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="86698-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
