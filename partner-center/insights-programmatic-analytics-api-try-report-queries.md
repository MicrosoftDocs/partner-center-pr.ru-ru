---
title: API пробного выполнения запросов отчетов
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API для проверки запроса и проверки результатов в центре партнеров Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376094"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="88c67-103">API пробного выполнения запросов отчетов</span><span class="sxs-lookup"><span data-stu-id="88c67-103">Try report queries API</span></span>

<span data-ttu-id="88c67-104">Этот API выполняет инструкцию запроса отчета.</span><span class="sxs-lookup"><span data-stu-id="88c67-104">This API executes a Report query statement.</span></span> <span data-ttu-id="88c67-105">API возвращает только 100 записей, которые вы в качестве партнера может использовать для проверки ожидаемых данных.</span><span class="sxs-lookup"><span data-stu-id="88c67-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="88c67-106">Время ожидания выполнения запроса для этого API составляет 100 секунд.</span><span class="sxs-lookup"><span data-stu-id="88c67-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="88c67-107">Если вы заметили, что API занимает более 100 секунд, очень вероятно, что запрос синтаксически верный, или же вы получили код ошибки, отличный от 200.</span><span class="sxs-lookup"><span data-stu-id="88c67-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="88c67-108">Фактическое создание отчета пройдет, если синтаксис запроса правильный.</span><span class="sxs-lookup"><span data-stu-id="88c67-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="88c67-109">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="88c67-109">**Request syntax**</span></span>

|    <span data-ttu-id="88c67-110">Метод</span><span class="sxs-lookup"><span data-stu-id="88c67-110">Method</span></span>    |    <span data-ttu-id="88c67-111">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="88c67-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="88c67-112">GET</span><span class="sxs-lookup"><span data-stu-id="88c67-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="88c67-113">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="88c67-113">**Request header**</span></span>

|    <span data-ttu-id="88c67-114">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88c67-114">Header</span></span>    |    <span data-ttu-id="88c67-115">Тип</span><span class="sxs-lookup"><span data-stu-id="88c67-115">Type</span></span>    |    <span data-ttu-id="88c67-116">Описание</span><span class="sxs-lookup"><span data-stu-id="88c67-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="88c67-117">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88c67-117">Authorization</span></span>    |    <span data-ttu-id="88c67-118">строка</span><span class="sxs-lookup"><span data-stu-id="88c67-118">string</span></span>    |    <span data-ttu-id="88c67-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88c67-119">Required.</span></span> <span data-ttu-id="88c67-120">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="88c67-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="88c67-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88c67-121">Content-Type</span></span>    |    <span data-ttu-id="88c67-122">строка</span><span class="sxs-lookup"><span data-stu-id="88c67-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="88c67-123">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="88c67-123">**Path parameter**</span></span>

<span data-ttu-id="88c67-124">Нет</span><span class="sxs-lookup"><span data-stu-id="88c67-124">None</span></span>

<span data-ttu-id="88c67-125">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="88c67-125">**Query parameter**</span></span>

|    <span data-ttu-id="88c67-126">имени параметра</span><span class="sxs-lookup"><span data-stu-id="88c67-126">Parameter Name</span></span>    |    <span data-ttu-id="88c67-127">Тип</span><span class="sxs-lookup"><span data-stu-id="88c67-127">Type</span></span>    |    <span data-ttu-id="88c67-128">Обязательно</span><span class="sxs-lookup"><span data-stu-id="88c67-128">Required</span></span>    |    <span data-ttu-id="88c67-129">Описание</span><span class="sxs-lookup"><span data-stu-id="88c67-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="88c67-130">експорткуери</span><span class="sxs-lookup"><span data-stu-id="88c67-130">exportQuery</span></span>     |    <span data-ttu-id="88c67-131">строка</span><span class="sxs-lookup"><span data-stu-id="88c67-131">string</span></span>    |    <span data-ttu-id="88c67-132">Нет</span><span class="sxs-lookup"><span data-stu-id="88c67-132">No</span></span>    |    <span data-ttu-id="88c67-133">Строка запроса отчета, которую необходимо выполнить</span><span class="sxs-lookup"><span data-stu-id="88c67-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="88c67-134">queryId</span><span class="sxs-lookup"><span data-stu-id="88c67-134">queryId</span></span>     |    <span data-ttu-id="88c67-135">строка</span><span class="sxs-lookup"><span data-stu-id="88c67-135">string</span></span>    |    <span data-ttu-id="88c67-136">Нет</span><span class="sxs-lookup"><span data-stu-id="88c67-136">No</span></span>    |    <span data-ttu-id="88c67-137">Допустимый идентификатор существующего запроса.</span><span class="sxs-lookup"><span data-stu-id="88c67-137">A valid existing query ID.</span></span> <span data-ttu-id="88c67-138">Взаимоисключающая со строкой запроса, указанной в параметре Експорткуери</span><span class="sxs-lookup"><span data-stu-id="88c67-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="88c67-139">startTime</span><span class="sxs-lookup"><span data-stu-id="88c67-139">startTime</span></span>     |    <span data-ttu-id="88c67-140">строка</span><span class="sxs-lookup"><span data-stu-id="88c67-140">string</span></span>    |    <span data-ttu-id="88c67-141">Нет</span><span class="sxs-lookup"><span data-stu-id="88c67-141">No</span></span>    |    <span data-ttu-id="88c67-142">Время начала, с которого нам нужны данные.</span><span class="sxs-lookup"><span data-stu-id="88c67-142">Start time from which we want the data.</span></span> <span data-ttu-id="88c67-143">Он переопределяет TimeSpan, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="88c67-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="88c67-144">endTime</span><span class="sxs-lookup"><span data-stu-id="88c67-144">endTime</span></span>     |    <span data-ttu-id="88c67-145">строка</span><span class="sxs-lookup"><span data-stu-id="88c67-145">string</span></span>    |    <span data-ttu-id="88c67-146">Нет</span><span class="sxs-lookup"><span data-stu-id="88c67-146">No</span></span>    |    <span data-ttu-id="88c67-147">Время окончания, до которого мы хотим получить данные.</span><span class="sxs-lookup"><span data-stu-id="88c67-147">End time till which we want the data.</span></span> <span data-ttu-id="88c67-148">Он переопределяет TimeSpan, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="88c67-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="88c67-149">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="88c67-149">**Request payload**</span></span>

<span data-ttu-id="88c67-150">Нет</span><span class="sxs-lookup"><span data-stu-id="88c67-150">None</span></span>

<span data-ttu-id="88c67-151">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="88c67-151">**Glossary**</span></span>

<span data-ttu-id="88c67-152">Нет</span><span class="sxs-lookup"><span data-stu-id="88c67-152">None</span></span>

<span data-ttu-id="88c67-153">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="88c67-153">**Response**</span></span>

<span data-ttu-id="88c67-154">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="88c67-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="88c67-155">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="88c67-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="88c67-156">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="88c67-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="88c67-157">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="88c67-157">**Glossary**</span></span>

<span data-ttu-id="88c67-158">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="88c67-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="88c67-159">Параметр</span><span class="sxs-lookup"><span data-stu-id="88c67-159">Parameter</span></span>    |    <span data-ttu-id="88c67-160">Описание</span><span class="sxs-lookup"><span data-stu-id="88c67-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="88c67-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="88c67-161">TotalCount</span></span>     |    <span data-ttu-id="88c67-162">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="88c67-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="88c67-163">Сообщение</span><span class="sxs-lookup"><span data-stu-id="88c67-163">Message</span></span>     |    <span data-ttu-id="88c67-164">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="88c67-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="88c67-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="88c67-165">StatusCode</span></span>     |    <span data-ttu-id="88c67-166">Код результата.</span><span class="sxs-lookup"><span data-stu-id="88c67-166">Result Code.</span></span> <span data-ttu-id="88c67-167">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="88c67-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
