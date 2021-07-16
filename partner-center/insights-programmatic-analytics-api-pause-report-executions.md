---
title: приостановка API выполнения отчета — данные Аналитика
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API, чтобы приостановить выполнение любого отчета в центре партнеров Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376118"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="85580-103">API приостановки выполнения отчетов</span><span class="sxs-lookup"><span data-stu-id="85580-103">Pause report executions API</span></span>

<span data-ttu-id="85580-104">При выполнении этот API приостанавливает запланированное выполнение отчетов.</span><span class="sxs-lookup"><span data-stu-id="85580-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="85580-105">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="85580-105">**Request syntax**</span></span>

|    <span data-ttu-id="85580-106">Метод</span><span class="sxs-lookup"><span data-stu-id="85580-106">Method</span></span>    |    <span data-ttu-id="85580-107">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="85580-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="85580-108">PUT</span><span class="sxs-lookup"><span data-stu-id="85580-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="85580-109">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="85580-109">**Request header**</span></span>

|    <span data-ttu-id="85580-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85580-110">Header</span></span>    |    <span data-ttu-id="85580-111">Тип</span><span class="sxs-lookup"><span data-stu-id="85580-111">Type</span></span>    |    <span data-ttu-id="85580-112">Описание</span><span class="sxs-lookup"><span data-stu-id="85580-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="85580-113">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85580-113">Authorization</span></span>    |    <span data-ttu-id="85580-114">строка</span><span class="sxs-lookup"><span data-stu-id="85580-114">string</span></span>    |    <span data-ttu-id="85580-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85580-115">Required.</span></span> <span data-ttu-id="85580-116">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="85580-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="85580-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85580-117">Content-Type</span></span>    |    <span data-ttu-id="85580-118">строка</span><span class="sxs-lookup"><span data-stu-id="85580-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="85580-119">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="85580-119">**Path parameter**</span></span>

|    <span data-ttu-id="85580-120">имени параметра</span><span class="sxs-lookup"><span data-stu-id="85580-120">Parameter Name</span></span>    |    <span data-ttu-id="85580-121">Тип</span><span class="sxs-lookup"><span data-stu-id="85580-121">Type</span></span>    |    <span data-ttu-id="85580-122">Обязательно</span><span class="sxs-lookup"><span data-stu-id="85580-122">Required</span></span>    |    <span data-ttu-id="85580-123">Описание</span><span class="sxs-lookup"><span data-stu-id="85580-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="85580-124">reportId</span><span class="sxs-lookup"><span data-stu-id="85580-124">reportId</span></span>     |    <span data-ttu-id="85580-125">строка</span><span class="sxs-lookup"><span data-stu-id="85580-125">string</span></span>    |    <span data-ttu-id="85580-126">Нет</span><span class="sxs-lookup"><span data-stu-id="85580-126">No</span></span>    |    <span data-ttu-id="85580-127">Идентификатор изменяемого отчета</span><span class="sxs-lookup"><span data-stu-id="85580-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="85580-128">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="85580-128">**Query parameter**</span></span>

<span data-ttu-id="85580-129">Нет</span><span class="sxs-lookup"><span data-stu-id="85580-129">None</span></span>

<span data-ttu-id="85580-130">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="85580-130">**Request payload**</span></span>

<span data-ttu-id="85580-131">Нет</span><span class="sxs-lookup"><span data-stu-id="85580-131">None</span></span>

<span data-ttu-id="85580-132">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="85580-132">**Glossary**</span></span>

<span data-ttu-id="85580-133">Нет</span><span class="sxs-lookup"><span data-stu-id="85580-133">None</span></span>

<span data-ttu-id="85580-134">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="85580-134">**Response**</span></span>

<span data-ttu-id="85580-135">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="85580-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="85580-136">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="85580-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="85580-137">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="85580-137">Response payload example:</span></span>

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

<span data-ttu-id="85580-138">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="85580-138">**Glossary**</span></span>

<span data-ttu-id="85580-139">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="85580-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="85580-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="85580-140">Parameter</span></span>    |    <span data-ttu-id="85580-141">Описание</span><span class="sxs-lookup"><span data-stu-id="85580-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="85580-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="85580-142">ReportId</span></span>     |    <span data-ttu-id="85580-143">Универсальный уникальный идентификатор (UUID) приостановленного отчета</span><span class="sxs-lookup"><span data-stu-id="85580-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="85580-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="85580-144">ReportName</span></span>     |    <span data-ttu-id="85580-145">Имя, присвоенное отчету во время создания</span><span class="sxs-lookup"><span data-stu-id="85580-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="85580-146">Описание</span><span class="sxs-lookup"><span data-stu-id="85580-146">Description</span></span>     |    <span data-ttu-id="85580-147">Описание, заданное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="85580-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="85580-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="85580-148">QueryId</span></span>     |    <span data-ttu-id="85580-149">Идентификатор запроса, переданный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="85580-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="85580-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="85580-150">Query</span></span>     |    <span data-ttu-id="85580-151">Текст запроса, который будет выполнен для этого отчета</span><span class="sxs-lookup"><span data-stu-id="85580-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="85580-152">Пользователь</span><span class="sxs-lookup"><span data-stu-id="85580-152">User</span></span>     |    <span data-ttu-id="85580-153">Идентификатор пользователя, используемый для создания отчета</span><span class="sxs-lookup"><span data-stu-id="85580-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="85580-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="85580-154">CreatedTime</span></span>     |    <span data-ttu-id="85580-155">Время создания отчета.</span><span class="sxs-lookup"><span data-stu-id="85580-155">Time the report was created.</span></span> <span data-ttu-id="85580-156">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="85580-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="85580-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="85580-157">ModifiedTime</span></span>     |    <span data-ttu-id="85580-158">Время последнего изменения отчета.</span><span class="sxs-lookup"><span data-stu-id="85580-158">Time the report was last modified.</span></span> <span data-ttu-id="85580-159">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="85580-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="85580-160">ексекутенов</span><span class="sxs-lookup"><span data-stu-id="85580-160">ExecuteNow</span></span>     |    <span data-ttu-id="85580-161">Флаг Ексекутенов, установленный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="85580-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="85580-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="85580-162">StartTime</span></span>     |    <span data-ttu-id="85580-163">Время, когда начнется выполнение отчета.</span><span class="sxs-lookup"><span data-stu-id="85580-163">Time the report execution will begin.</span></span> <span data-ttu-id="85580-164">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="85580-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="85580-165">репортстатус</span><span class="sxs-lookup"><span data-stu-id="85580-165">ReportStatus</span></span>     |    <span data-ttu-id="85580-166">Состояние выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="85580-166">Status of the report execution.</span></span> <span data-ttu-id="85580-167">Возможные значения: Paused (Приостановлено), Active (Активно) и Inactive (Неактивно).</span><span class="sxs-lookup"><span data-stu-id="85580-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="85580-168">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="85580-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="85580-169">Интервал повторения, указанный при создании отчета</span><span class="sxs-lookup"><span data-stu-id="85580-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="85580-170">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="85580-170">RecurrenceCount</span></span>     |    <span data-ttu-id="85580-171">Число повторений, указанное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="85580-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="85580-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="85580-172">CallbackUrl</span></span>     |    <span data-ttu-id="85580-173">URL-адрес обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="85580-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="85580-174">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="85580-174">CallbackMethod</span></span>    |    <span data-ttu-id="85580-175">Метод обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="85580-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="85580-176">Формат</span><span class="sxs-lookup"><span data-stu-id="85580-176">Format</span></span>     |    <span data-ttu-id="85580-177">Формат файлов отчета</span><span class="sxs-lookup"><span data-stu-id="85580-177">Format of the report files</span></span>     |
|    <span data-ttu-id="85580-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="85580-178">TotalCount</span></span>     |    <span data-ttu-id="85580-179">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="85580-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="85580-180">Сообщение</span><span class="sxs-lookup"><span data-stu-id="85580-180">Message</span></span>     |    <span data-ttu-id="85580-181">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="85580-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="85580-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="85580-182">StatusCode</span></span>     |    <span data-ttu-id="85580-183">Код результата.</span><span class="sxs-lookup"><span data-stu-id="85580-183">Result Code.</span></span> <span data-ttu-id="85580-184">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="85580-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
