---
title: возобновление API выполнения отчета — Аналитика данных
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API, чтобы возобновить выполнение приостановленного отчета в центре партнеров Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376110"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="56d0e-103">API возобновления выполнения отчетов</span><span class="sxs-lookup"><span data-stu-id="56d0e-103">Resume report executions API</span></span>

<span data-ttu-id="56d0e-104">При выполнении этот API возобновляет запланированное выполнение приостановленного отчета.</span><span class="sxs-lookup"><span data-stu-id="56d0e-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="56d0e-105">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="56d0e-105">**Request syntax**</span></span>

|    <span data-ttu-id="56d0e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="56d0e-106">Method</span></span>    |    <span data-ttu-id="56d0e-107">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="56d0e-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="56d0e-108">PUT</span><span class="sxs-lookup"><span data-stu-id="56d0e-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="56d0e-109">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="56d0e-109">**Request header**</span></span>

|    <span data-ttu-id="56d0e-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56d0e-110">Header</span></span>    |    <span data-ttu-id="56d0e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="56d0e-111">Type</span></span>    |    <span data-ttu-id="56d0e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="56d0e-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="56d0e-113">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56d0e-113">Authorization</span></span>    |    <span data-ttu-id="56d0e-114">строка</span><span class="sxs-lookup"><span data-stu-id="56d0e-114">string</span></span>    |    <span data-ttu-id="56d0e-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56d0e-115">Required.</span></span> <span data-ttu-id="56d0e-116">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="56d0e-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="56d0e-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56d0e-117">Content-Type</span></span>    |    <span data-ttu-id="56d0e-118">строка</span><span class="sxs-lookup"><span data-stu-id="56d0e-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="56d0e-119">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="56d0e-119">**Path parameter**</span></span>

|    <span data-ttu-id="56d0e-120">имени параметра</span><span class="sxs-lookup"><span data-stu-id="56d0e-120">Parameter Name</span></span>    |    <span data-ttu-id="56d0e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="56d0e-121">Type</span></span>    |    <span data-ttu-id="56d0e-122">Обязательно</span><span class="sxs-lookup"><span data-stu-id="56d0e-122">Required</span></span>    |    <span data-ttu-id="56d0e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="56d0e-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="56d0e-124">reportId</span><span class="sxs-lookup"><span data-stu-id="56d0e-124">reportId</span></span>     |    <span data-ttu-id="56d0e-125">строка</span><span class="sxs-lookup"><span data-stu-id="56d0e-125">string</span></span>    |    <span data-ttu-id="56d0e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="56d0e-126">No</span></span>    |    <span data-ttu-id="56d0e-127">Идентификатор изменяемого отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="56d0e-128">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="56d0e-128">**Query parameter**</span></span>

<span data-ttu-id="56d0e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="56d0e-129">None</span></span>

<span data-ttu-id="56d0e-130">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="56d0e-130">**Request payload**</span></span>

<span data-ttu-id="56d0e-131">Нет</span><span class="sxs-lookup"><span data-stu-id="56d0e-131">None</span></span>

<span data-ttu-id="56d0e-132">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="56d0e-132">**Glossary**</span></span>

<span data-ttu-id="56d0e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="56d0e-133">None</span></span>

<span data-ttu-id="56d0e-134">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="56d0e-134">**Response**</span></span>

<span data-ttu-id="56d0e-135">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="56d0e-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="56d0e-136">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="56d0e-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="56d0e-137">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="56d0e-137">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="56d0e-138">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="56d0e-138">**Glossary**</span></span>

<span data-ttu-id="56d0e-139">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="56d0e-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="56d0e-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="56d0e-140">Parameter</span></span>    |    <span data-ttu-id="56d0e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="56d0e-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="56d0e-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="56d0e-142">ReportId</span></span>     |    <span data-ttu-id="56d0e-143">Универсальный уникальный идентификатор (UUID) возобновляемого отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="56d0e-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="56d0e-144">ReportName</span></span>     |    <span data-ttu-id="56d0e-145">Имя, присвоенное отчету во время создания</span><span class="sxs-lookup"><span data-stu-id="56d0e-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="56d0e-146">Описание</span><span class="sxs-lookup"><span data-stu-id="56d0e-146">Description</span></span>     |    <span data-ttu-id="56d0e-147">Описание, заданное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="56d0e-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="56d0e-148">QueryId</span></span>     |    <span data-ttu-id="56d0e-149">Идентификатор запроса, переданный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="56d0e-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="56d0e-150">Query</span></span>     |    <span data-ttu-id="56d0e-151">Текст запроса, который будет выполнен для этого отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="56d0e-152">Пользователь</span><span class="sxs-lookup"><span data-stu-id="56d0e-152">User</span></span>     |    <span data-ttu-id="56d0e-153">Идентификатор пользователя, используемый для создания отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="56d0e-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="56d0e-154">CreatedTime</span></span>     |    <span data-ttu-id="56d0e-155">Время создания отчета.</span><span class="sxs-lookup"><span data-stu-id="56d0e-155">Time the report was created.</span></span> <span data-ttu-id="56d0e-156">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="56d0e-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="56d0e-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="56d0e-157">ModifiedTime</span></span>     |    <span data-ttu-id="56d0e-158">Время последнего изменения отчета.</span><span class="sxs-lookup"><span data-stu-id="56d0e-158">Time the report was last modified.</span></span> <span data-ttu-id="56d0e-159">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="56d0e-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="56d0e-160">ексекутенов</span><span class="sxs-lookup"><span data-stu-id="56d0e-160">ExecuteNow</span></span>     |    <span data-ttu-id="56d0e-161">Флаг Ексекутенов, установленный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="56d0e-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="56d0e-162">StartTime</span></span>     |    <span data-ttu-id="56d0e-163">Время, когда начнется выполнение отчета.</span><span class="sxs-lookup"><span data-stu-id="56d0e-163">Time the report execution will begin.</span></span> <span data-ttu-id="56d0e-164">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="56d0e-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="56d0e-165">репортстатус</span><span class="sxs-lookup"><span data-stu-id="56d0e-165">ReportStatus</span></span>     |    <span data-ttu-id="56d0e-166">Состояние выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="56d0e-166">Status of the report execution.</span></span> <span data-ttu-id="56d0e-167">Возможные значения: Paused (Приостановлено), Active (Активно) и Inactive (Неактивно).</span><span class="sxs-lookup"><span data-stu-id="56d0e-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="56d0e-168">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="56d0e-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="56d0e-169">Интервал повторения, указанный при создании отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="56d0e-170">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="56d0e-170">RecurrenceCount</span></span>     |    <span data-ttu-id="56d0e-171">Число повторений, указанное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="56d0e-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="56d0e-172">CallbackUrl</span></span>     |    <span data-ttu-id="56d0e-173">URL-адрес обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="56d0e-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="56d0e-174">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="56d0e-174">CallbackMethod</span></span>    |    <span data-ttu-id="56d0e-175">Метод обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="56d0e-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="56d0e-176">Формат</span><span class="sxs-lookup"><span data-stu-id="56d0e-176">Format</span></span>     |    <span data-ttu-id="56d0e-177">Формат файлов отчета</span><span class="sxs-lookup"><span data-stu-id="56d0e-177">Format of the report files</span></span>     |
|    <span data-ttu-id="56d0e-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="56d0e-178">TotalCount</span></span>     |    <span data-ttu-id="56d0e-179">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="56d0e-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="56d0e-180">Сообщение</span><span class="sxs-lookup"><span data-stu-id="56d0e-180">Message</span></span>     |    <span data-ttu-id="56d0e-181">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="56d0e-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="56d0e-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="56d0e-182">StatusCode</span></span>     |    <span data-ttu-id="56d0e-183">Код результата.</span><span class="sxs-lookup"><span data-stu-id="56d0e-183">Result Code.</span></span> <span data-ttu-id="56d0e-184">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="56d0e-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
