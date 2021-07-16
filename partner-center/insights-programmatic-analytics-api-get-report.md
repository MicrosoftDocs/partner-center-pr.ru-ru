---
title: получение данных API отчета — Аналитика данные
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API, чтобы получить все доступные ИДЕНТИФИКАТОРы отчетов в центре партнеров Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376123"
---
# <a name="get-report-api"></a><span data-ttu-id="a7dcd-103">API получения отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-103">Get report API</span></span>

<span data-ttu-id="a7dcd-104">Этот API возвращает все запланированные отчеты.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="a7dcd-105">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-105">**Request syntax**</span></span>

|    <span data-ttu-id="a7dcd-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a7dcd-106">Method</span></span>    |    <span data-ttu-id="a7dcd-107">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="a7dcd-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a7dcd-108">GET</span><span class="sxs-lookup"><span data-stu-id="a7dcd-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="a7dcd-109">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-109">**Request header**</span></span>

|    <span data-ttu-id="a7dcd-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7dcd-110">Header</span></span>    |    <span data-ttu-id="a7dcd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a7dcd-111">Type</span></span>    |    <span data-ttu-id="a7dcd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dcd-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="a7dcd-113">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7dcd-113">Authorization</span></span>    |    <span data-ttu-id="a7dcd-114">строка</span><span class="sxs-lookup"><span data-stu-id="a7dcd-114">string</span></span>    |    <span data-ttu-id="a7dcd-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-115">Required.</span></span> <span data-ttu-id="a7dcd-116">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="a7dcd-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="a7dcd-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7dcd-117">Content-Type</span></span>    |    <span data-ttu-id="a7dcd-118">строка</span><span class="sxs-lookup"><span data-stu-id="a7dcd-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="a7dcd-119">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-119">**Path parameter**</span></span>

<span data-ttu-id="a7dcd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a7dcd-120">None</span></span>

<span data-ttu-id="a7dcd-121">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-121">**Query parameter**</span></span>

|    <span data-ttu-id="a7dcd-122">имени параметра</span><span class="sxs-lookup"><span data-stu-id="a7dcd-122">Parameter Name</span></span>    |    <span data-ttu-id="a7dcd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a7dcd-123">Type</span></span>    |    <span data-ttu-id="a7dcd-124">Обязательно</span><span class="sxs-lookup"><span data-stu-id="a7dcd-124">Required</span></span>    |    <span data-ttu-id="a7dcd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dcd-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a7dcd-126">reportId</span><span class="sxs-lookup"><span data-stu-id="a7dcd-126">reportId</span></span>     |    <span data-ttu-id="a7dcd-127">строка</span><span class="sxs-lookup"><span data-stu-id="a7dcd-127">string</span></span>    |    <span data-ttu-id="a7dcd-128">Нет</span><span class="sxs-lookup"><span data-stu-id="a7dcd-128">No</span></span>    |    <span data-ttu-id="a7dcd-129">Фильтр для получения сведений только об отчетах с идентификатор reportID, указанными в этом аргументе</span><span class="sxs-lookup"><span data-stu-id="a7dcd-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="a7dcd-130">reportName</span><span class="sxs-lookup"><span data-stu-id="a7dcd-130">reportName</span></span>     |    <span data-ttu-id="a7dcd-131">строка</span><span class="sxs-lookup"><span data-stu-id="a7dcd-131">string</span></span>    |    <span data-ttu-id="a7dcd-132">Нет</span><span class="sxs-lookup"><span data-stu-id="a7dcd-132">No</span></span>    |    <span data-ttu-id="a7dcd-133">Фильтр для получения сведений только об отчетах с reportName, указанными в этом аргументе</span><span class="sxs-lookup"><span data-stu-id="a7dcd-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="a7dcd-134">queryId</span><span class="sxs-lookup"><span data-stu-id="a7dcd-134">queryId</span></span>     |    <span data-ttu-id="a7dcd-135">строка</span><span class="sxs-lookup"><span data-stu-id="a7dcd-135">string</span></span>    |    <span data-ttu-id="a7dcd-136">Нет</span><span class="sxs-lookup"><span data-stu-id="a7dcd-136">No</span></span>    |    <span data-ttu-id="a7dcd-137">Фильтр для получения сведений только об отчетах с queryId, указанными в этом аргументе</span><span class="sxs-lookup"><span data-stu-id="a7dcd-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="a7dcd-138">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-138">**Request payload**</span></span>

<span data-ttu-id="a7dcd-139">Нет</span><span class="sxs-lookup"><span data-stu-id="a7dcd-139">None</span></span>

<span data-ttu-id="a7dcd-140">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-140">**Glossary**</span></span>

<span data-ttu-id="a7dcd-141">Нет</span><span class="sxs-lookup"><span data-stu-id="a7dcd-141">None</span></span>

<span data-ttu-id="a7dcd-142">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-142">**Response**</span></span>

<span data-ttu-id="a7dcd-143">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="a7dcd-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="a7dcd-144">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="a7dcd-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="a7dcd-145">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="a7dcd-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="a7dcd-146">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="a7dcd-146">**Glossary**</span></span>

<span data-ttu-id="a7dcd-147">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="a7dcd-148">Параметр</span><span class="sxs-lookup"><span data-stu-id="a7dcd-148">Parameter</span></span>    |    <span data-ttu-id="a7dcd-149">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dcd-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a7dcd-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="a7dcd-150">ReportId</span></span>     |    <span data-ttu-id="a7dcd-151">Уникальный UUID созданного отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="a7dcd-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="a7dcd-152">ReportName</span></span>     |    <span data-ttu-id="a7dcd-153">Имя, присвоенное отчету в полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="a7dcd-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="a7dcd-154">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dcd-154">Description</span></span>     |    <span data-ttu-id="a7dcd-155">Описание, заданное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="a7dcd-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="a7dcd-156">QueryId</span></span>     |    <span data-ttu-id="a7dcd-157">Идентификатор запроса, переданный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="a7dcd-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7dcd-158">Query</span></span>     |    <span data-ttu-id="a7dcd-159">Текст запроса, который будет выполнен для этого отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="a7dcd-160">Пользователь</span><span class="sxs-lookup"><span data-stu-id="a7dcd-160">User</span></span>     |    <span data-ttu-id="a7dcd-161">Идентификатор пользователя, используемый для создания отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="a7dcd-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="a7dcd-162">CreatedTime</span></span>     |    <span data-ttu-id="a7dcd-163">Время создания отчета.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-163">Time the report was created.</span></span> <span data-ttu-id="a7dcd-164">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="a7dcd-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a7dcd-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a7dcd-165">ModifiedTime</span></span>     |    <span data-ttu-id="a7dcd-166">Время последнего изменения отчета.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-166">Time the report was last modified.</span></span> <span data-ttu-id="a7dcd-167">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="a7dcd-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a7dcd-168">ексекутенов</span><span class="sxs-lookup"><span data-stu-id="a7dcd-168">executeNow</span></span>     |    <span data-ttu-id="a7dcd-169">Флаг Ексекутенов, установленный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="a7dcd-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="a7dcd-170">StartTime</span></span>     |    <span data-ttu-id="a7dcd-171">Время начала выполнения.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-171">Time execution will begin.</span></span> <span data-ttu-id="a7dcd-172">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="a7dcd-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a7dcd-173">репортстатус</span><span class="sxs-lookup"><span data-stu-id="a7dcd-173">ReportStatus</span></span>     |    <span data-ttu-id="a7dcd-174">Состояние выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-174">Status of the report execution.</span></span> <span data-ttu-id="a7dcd-175">Возможные значения: Paused (Приостановлено), Active (Активно) и Inactive (Неактивно).</span><span class="sxs-lookup"><span data-stu-id="a7dcd-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="a7dcd-176">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="a7dcd-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="a7dcd-177">Интервал повторения, указанный при создании отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="a7dcd-178">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="a7dcd-178">RecurrenceCount</span></span>     |    <span data-ttu-id="a7dcd-179">Число повторений, указанное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="a7dcd-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a7dcd-180">CallbackUrl</span></span>     |    <span data-ttu-id="a7dcd-181">URL-адрес обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="a7dcd-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="a7dcd-182">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="a7dcd-182">CallbackMethod</span></span>    |    <span data-ttu-id="a7dcd-183">Метод обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="a7dcd-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="a7dcd-184">Формат</span><span class="sxs-lookup"><span data-stu-id="a7dcd-184">Format</span></span>     |    <span data-ttu-id="a7dcd-185">Формат файлов отчета</span><span class="sxs-lookup"><span data-stu-id="a7dcd-185">Format of the report files</span></span>     |
|    <span data-ttu-id="a7dcd-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a7dcd-186">TotalCount</span></span>     |    <span data-ttu-id="a7dcd-187">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="a7dcd-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="a7dcd-188">Сообщение</span><span class="sxs-lookup"><span data-stu-id="a7dcd-188">Message</span></span>     |    <span data-ttu-id="a7dcd-189">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="a7dcd-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="a7dcd-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="a7dcd-190">StatusCode</span></span>     |    <span data-ttu-id="a7dcd-191">Код результата.</span><span class="sxs-lookup"><span data-stu-id="a7dcd-191">Result Code.</span></span> <span data-ttu-id="a7dcd-192">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="a7dcd-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |