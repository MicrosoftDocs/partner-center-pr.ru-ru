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
# <a name="get-report-queries-api"></a><span data-ttu-id="3869e-103">API получения запросов отчетов</span><span class="sxs-lookup"><span data-stu-id="3869e-103">Get report queries API</span></span>

<span data-ttu-id="3869e-104">API получения отчетов о запросах получает все запросы, доступные для использования в отчетах.</span><span class="sxs-lookup"><span data-stu-id="3869e-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="3869e-105">Он получает все системные и пользовательские запросы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3869e-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="3869e-106">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="3869e-106">**Request syntax**</span></span>

|    <span data-ttu-id="3869e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3869e-107">Method</span></span>    |    <span data-ttu-id="3869e-108">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="3869e-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="3869e-109">GET</span><span class="sxs-lookup"><span data-stu-id="3869e-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="3869e-110">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="3869e-110">**Request header**</span></span>

|    <span data-ttu-id="3869e-111">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3869e-111">Header</span></span>    |    <span data-ttu-id="3869e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="3869e-112">Type</span></span>    |    <span data-ttu-id="3869e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3869e-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="3869e-114">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3869e-114">Authorization</span></span>    |    <span data-ttu-id="3869e-115">строка</span><span class="sxs-lookup"><span data-stu-id="3869e-115">string</span></span>    |    <span data-ttu-id="3869e-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3869e-116">Required.</span></span> <span data-ttu-id="3869e-117">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="3869e-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="3869e-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3869e-118">Content-Type</span></span>    |    <span data-ttu-id="3869e-119">строка</span><span class="sxs-lookup"><span data-stu-id="3869e-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="3869e-120">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="3869e-120">**Path parameter**</span></span>

<span data-ttu-id="3869e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3869e-121">None</span></span>

<span data-ttu-id="3869e-122">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="3869e-122">**Query parameter**</span></span>

|    <span data-ttu-id="3869e-123">имени параметра</span><span class="sxs-lookup"><span data-stu-id="3869e-123">Parameter Name</span></span>    |    <span data-ttu-id="3869e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3869e-124">Type</span></span>    |    <span data-ttu-id="3869e-125">Обязательно</span><span class="sxs-lookup"><span data-stu-id="3869e-125">Required</span></span>    |    <span data-ttu-id="3869e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3869e-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="3869e-127">queryId</span><span class="sxs-lookup"><span data-stu-id="3869e-127">queryId</span></span>     |    <span data-ttu-id="3869e-128">строка</span><span class="sxs-lookup"><span data-stu-id="3869e-128">string</span></span>     |    <span data-ttu-id="3869e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="3869e-129">No</span></span>    |    <span data-ttu-id="3869e-130">Фильтр для получения сведений только о запросах с идентификатором, заданным в аргументе</span><span class="sxs-lookup"><span data-stu-id="3869e-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="3869e-131">queryName</span><span class="sxs-lookup"><span data-stu-id="3869e-131">queryName</span></span>     |    <span data-ttu-id="3869e-132">строка</span><span class="sxs-lookup"><span data-stu-id="3869e-132">string</span></span>     |    <span data-ttu-id="3869e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="3869e-133">No</span></span>    |    <span data-ttu-id="3869e-134">Фильтр для получения сведений только о запросах с именем, заданным в аргументе</span><span class="sxs-lookup"><span data-stu-id="3869e-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="3869e-135">инклудесистемкуериес</span><span class="sxs-lookup"><span data-stu-id="3869e-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="3869e-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="3869e-136">boolean</span></span>     |    <span data-ttu-id="3869e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="3869e-137">No</span></span>    |    <span data-ttu-id="3869e-138">Включить в ответ стандартные системные запросы</span><span class="sxs-lookup"><span data-stu-id="3869e-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="3869e-139">инклудеонлисистемкуериес</span><span class="sxs-lookup"><span data-stu-id="3869e-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="3869e-140">Логическое</span><span class="sxs-lookup"><span data-stu-id="3869e-140">boolean</span></span>     |    <span data-ttu-id="3869e-141">Нет</span><span class="sxs-lookup"><span data-stu-id="3869e-141">No</span></span>    |    <span data-ttu-id="3869e-142">Включить в ответ только системные запросы</span><span class="sxs-lookup"><span data-stu-id="3869e-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="3869e-143">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="3869e-143">**Request payload**</span></span>

<span data-ttu-id="3869e-144">Нет</span><span class="sxs-lookup"><span data-stu-id="3869e-144">None</span></span>

<span data-ttu-id="3869e-145">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="3869e-145">**Glossary**</span></span>

<span data-ttu-id="3869e-146">Нет</span><span class="sxs-lookup"><span data-stu-id="3869e-146">None</span></span>

<span data-ttu-id="3869e-147">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="3869e-147">**Response**</span></span>

<span data-ttu-id="3869e-148">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="3869e-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="3869e-149">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="3869e-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="3869e-150">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="3869e-150">Response payload example:</span></span>

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

<span data-ttu-id="3869e-151">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="3869e-151">**Glossary**</span></span>

<span data-ttu-id="3869e-152">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="3869e-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="3869e-153">Параметр</span><span class="sxs-lookup"><span data-stu-id="3869e-153">Parameter</span></span>    |    <span data-ttu-id="3869e-154">Описание</span><span class="sxs-lookup"><span data-stu-id="3869e-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="3869e-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="3869e-155">QueryId</span></span>     |    <span data-ttu-id="3869e-156">Уникальный UUID запроса</span><span class="sxs-lookup"><span data-stu-id="3869e-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="3869e-157">Имя</span><span class="sxs-lookup"><span data-stu-id="3869e-157">Name</span></span>     |    <span data-ttu-id="3869e-158">Имя, присвоенное запросу при создании запроса</span><span class="sxs-lookup"><span data-stu-id="3869e-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="3869e-159">Описание</span><span class="sxs-lookup"><span data-stu-id="3869e-159">Description</span></span>     |    <span data-ttu-id="3869e-160">Описание, заданное при создании запроса</span><span class="sxs-lookup"><span data-stu-id="3869e-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="3869e-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="3869e-161">Query</span></span>     |    <span data-ttu-id="3869e-162">Строка запроса отчета</span><span class="sxs-lookup"><span data-stu-id="3869e-162">Report query string</span></span>     |
|    <span data-ttu-id="3869e-163">Тип</span><span class="sxs-lookup"><span data-stu-id="3869e-163">Type</span></span>     |    <span data-ttu-id="3869e-164">Задайте значение Пользователяопределенные для созданных пользователем запросов и системы для предопределенных системных запросов.</span><span class="sxs-lookup"><span data-stu-id="3869e-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="3869e-165">Пользователь</span><span class="sxs-lookup"><span data-stu-id="3869e-165">User</span></span>     |    <span data-ttu-id="3869e-166">Идентификатор пользователя, создавшего запрос</span><span class="sxs-lookup"><span data-stu-id="3869e-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="3869e-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="3869e-167">CreatedTime</span></span>     |    <span data-ttu-id="3869e-168">Время создания запроса</span><span class="sxs-lookup"><span data-stu-id="3869e-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="3869e-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="3869e-169">TotalCount</span></span>     |    <span data-ttu-id="3869e-170">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="3869e-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="3869e-171">Сообщение</span><span class="sxs-lookup"><span data-stu-id="3869e-171">Message</span></span>     |    <span data-ttu-id="3869e-172">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="3869e-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="3869e-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="3869e-173">StatusCode</span></span>     |    <span data-ttu-id="3869e-174">Код результата.</span><span class="sxs-lookup"><span data-stu-id="3869e-174">Result Code.</span></span> <span data-ttu-id="3869e-175">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="3869e-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
