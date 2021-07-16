---
title: API обновления отчета
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API для обновления параметров отчета в центре партнеров Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376091"
---
# <a name="update-report-api"></a><span data-ttu-id="880f3-103">API обновления отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-103">Update report API</span></span>

<span data-ttu-id="880f3-104">Этот API помогает изменить параметр отчета.</span><span class="sxs-lookup"><span data-stu-id="880f3-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="880f3-105">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="880f3-105">**Request syntax**</span></span>

|    <span data-ttu-id="880f3-106">Метод</span><span class="sxs-lookup"><span data-stu-id="880f3-106">Method</span></span>    |    <span data-ttu-id="880f3-107">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="880f3-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="880f3-108">PUT</span><span class="sxs-lookup"><span data-stu-id="880f3-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="880f3-109">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="880f3-109">**Request header**</span></span>

|    <span data-ttu-id="880f3-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="880f3-110">Header</span></span>    |    <span data-ttu-id="880f3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="880f3-111">Type</span></span>    |    <span data-ttu-id="880f3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="880f3-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="880f3-113">Авторизация</span><span class="sxs-lookup"><span data-stu-id="880f3-113">Authorization</span></span>    |    <span data-ttu-id="880f3-114">строка</span><span class="sxs-lookup"><span data-stu-id="880f3-114">string</span></span>    |    <span data-ttu-id="880f3-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="880f3-115">Required.</span></span> <span data-ttu-id="880f3-116">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="880f3-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="880f3-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="880f3-117">Content-Type</span></span>    |    <span data-ttu-id="880f3-118">строка</span><span class="sxs-lookup"><span data-stu-id="880f3-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="880f3-119">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="880f3-119">**Path parameter**</span></span>

|    <span data-ttu-id="880f3-120">имени параметра</span><span class="sxs-lookup"><span data-stu-id="880f3-120">Parameter Name</span></span>    |    <span data-ttu-id="880f3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="880f3-121">Type</span></span>    |    <span data-ttu-id="880f3-122">Обязательно</span><span class="sxs-lookup"><span data-stu-id="880f3-122">Required</span></span>    |    <span data-ttu-id="880f3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="880f3-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="880f3-124">reportId</span><span class="sxs-lookup"><span data-stu-id="880f3-124">reportId</span></span>     |    <span data-ttu-id="880f3-125">строка</span><span class="sxs-lookup"><span data-stu-id="880f3-125">string</span></span>    |    <span data-ttu-id="880f3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-126">No</span></span>    |    <span data-ttu-id="880f3-127">Идентификатор изменяемого отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="880f3-128">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="880f3-128">**Query parameter**</span></span>

<span data-ttu-id="880f3-129">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-129">None</span></span>

<span data-ttu-id="880f3-130">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="880f3-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="880f3-131">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="880f3-131">**Glossary**</span></span>

<span data-ttu-id="880f3-132">В этой таблице приведены основные определения элементов в ответе.</span><span class="sxs-lookup"><span data-stu-id="880f3-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="880f3-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="880f3-133">Parameter</span></span>    |    <span data-ttu-id="880f3-134">Обязательно</span><span class="sxs-lookup"><span data-stu-id="880f3-134">Required</span></span>    |    <span data-ttu-id="880f3-135">Описание</span><span class="sxs-lookup"><span data-stu-id="880f3-135">Description</span></span>    |    <span data-ttu-id="880f3-136">Допустимые значения</span><span class="sxs-lookup"><span data-stu-id="880f3-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="880f3-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="880f3-137">ReportName</span></span>     |    <span data-ttu-id="880f3-138">Да</span><span class="sxs-lookup"><span data-stu-id="880f3-138">Yes</span></span>     |    <span data-ttu-id="880f3-139">Имя, назначаемое отчету</span><span class="sxs-lookup"><span data-stu-id="880f3-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="880f3-140">Строка</span><span class="sxs-lookup"><span data-stu-id="880f3-140">String</span></span>     |
|    <span data-ttu-id="880f3-141">Описание</span><span class="sxs-lookup"><span data-stu-id="880f3-141">Description</span></span>     |    <span data-ttu-id="880f3-142">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-142">No</span></span>     |    <span data-ttu-id="880f3-143">Описание созданного отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-143">Description of the created report</span></span>     |    <span data-ttu-id="880f3-144">Строка</span><span class="sxs-lookup"><span data-stu-id="880f3-144">String</span></span>     |
|    <span data-ttu-id="880f3-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="880f3-145">StartTime</span></span>     |    <span data-ttu-id="880f3-146">Да</span><span class="sxs-lookup"><span data-stu-id="880f3-146">Yes</span></span>    |    <span data-ttu-id="880f3-147">Метка времени, после которой начнется создание отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="880f3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="880f3-148">String</span></span>     |
|    <span data-ttu-id="880f3-149">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="880f3-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="880f3-150">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-150">No</span></span>     |    <span data-ttu-id="880f3-151">Периодичность создания отчета в часах.</span><span class="sxs-lookup"><span data-stu-id="880f3-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="880f3-152">Минимальное значение — 4</span><span class="sxs-lookup"><span data-stu-id="880f3-152">Minimum value is 4</span></span>     |    <span data-ttu-id="880f3-153">Целое число</span><span class="sxs-lookup"><span data-stu-id="880f3-153">Integer</span></span>     |
|    <span data-ttu-id="880f3-154">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="880f3-154">RecurrenceCount</span></span>     |    <span data-ttu-id="880f3-155">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-155">No</span></span>     |    <span data-ttu-id="880f3-156">Число создаваемых отчетов.</span><span class="sxs-lookup"><span data-stu-id="880f3-156">Numbers of report to be generated.</span></span> <span data-ttu-id="880f3-157">Значение по умолчанию — неопределенное.</span><span class="sxs-lookup"><span data-stu-id="880f3-157">Default is indefinite.</span></span>     |    <span data-ttu-id="880f3-158">Целое число</span><span class="sxs-lookup"><span data-stu-id="880f3-158">Integer</span></span>     |
|    <span data-ttu-id="880f3-159">Формат</span><span class="sxs-lookup"><span data-stu-id="880f3-159">Format</span></span>     |    <span data-ttu-id="880f3-160">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-160">No</span></span>    |    <span data-ttu-id="880f3-161">Формат экспортируемого файла.</span><span class="sxs-lookup"><span data-stu-id="880f3-161">File format of the exported file.</span></span> <span data-ttu-id="880f3-162">Значение по умолчанию — CSV</span><span class="sxs-lookup"><span data-stu-id="880f3-162">Default is CSV</span></span>     |    <span data-ttu-id="880f3-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="880f3-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="880f3-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="880f3-164">CallbackURL</span></span>     |    <span data-ttu-id="880f3-165">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-165">No</span></span>     |    <span data-ttu-id="880f3-166">URL-адрес обратного вызова HTTPS, вызываемый при создании отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="880f3-167">Строка</span><span class="sxs-lookup"><span data-stu-id="880f3-167">String</span></span>     |
|    <span data-ttu-id="880f3-168">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="880f3-168">CallbackMethod</span></span>    |    <span data-ttu-id="880f3-169">Нет</span><span class="sxs-lookup"><span data-stu-id="880f3-169">No</span></span>    |    <span data-ttu-id="880f3-170">Метод HTTP, используемый для обратного вызова</span><span class="sxs-lookup"><span data-stu-id="880f3-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="880f3-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="880f3-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="880f3-172">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="880f3-172">**Response**</span></span>

<span data-ttu-id="880f3-173">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="880f3-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="880f3-174">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="880f3-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="880f3-175">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="880f3-175">Response payload example:</span></span>

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

<span data-ttu-id="880f3-176">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="880f3-176">**Glossary**</span></span>

<span data-ttu-id="880f3-177">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="880f3-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="880f3-178">Параметр</span><span class="sxs-lookup"><span data-stu-id="880f3-178">Parameter</span></span>    |    <span data-ttu-id="880f3-179">Описание</span><span class="sxs-lookup"><span data-stu-id="880f3-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="880f3-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="880f3-180">ReportId</span></span>     |    <span data-ttu-id="880f3-181">Универсальный уникальный идентификатор (UUID) обновляемого отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="880f3-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="880f3-182">ReportName</span></span>     |    <span data-ttu-id="880f3-183">Имя, присвоенное отчету в полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="880f3-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="880f3-184">Описание</span><span class="sxs-lookup"><span data-stu-id="880f3-184">Description</span></span>     |    <span data-ttu-id="880f3-185">Описание, заданное для отчета в полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="880f3-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="880f3-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="880f3-186">QueryId</span></span>     |    <span data-ttu-id="880f3-187">Идентификатор запроса, переданный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="880f3-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="880f3-188">Query</span></span>     |    <span data-ttu-id="880f3-189">Текст запроса, который будет выполнен для этого отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="880f3-190">Пользователь</span><span class="sxs-lookup"><span data-stu-id="880f3-190">User</span></span>     |    <span data-ttu-id="880f3-191">Идентификатор пользователя, используемый для создания отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="880f3-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="880f3-192">CreatedTime</span></span>     |    <span data-ttu-id="880f3-193">Время создания отчета.</span><span class="sxs-lookup"><span data-stu-id="880f3-193">Time the report was created.</span></span> <span data-ttu-id="880f3-194">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="880f3-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="880f3-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="880f3-195">ModifiedTime</span></span>     |    <span data-ttu-id="880f3-196">Время последнего изменения отчета.</span><span class="sxs-lookup"><span data-stu-id="880f3-196">Time the report was last modified.</span></span> <span data-ttu-id="880f3-197">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="880f3-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="880f3-198">ексекутенов</span><span class="sxs-lookup"><span data-stu-id="880f3-198">ExecuteNow</span></span>     |    <span data-ttu-id="880f3-199">Флаг Ексекутенов, установленный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="880f3-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="880f3-200">StartTime</span></span>     |    <span data-ttu-id="880f3-201">Время, когда начнется выполнение отчета.</span><span class="sxs-lookup"><span data-stu-id="880f3-201">Time the report execution will begin.</span></span> <span data-ttu-id="880f3-202">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="880f3-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="880f3-203">репортстатус</span><span class="sxs-lookup"><span data-stu-id="880f3-203">ReportStatus</span></span>     |    <span data-ttu-id="880f3-204">Состояние выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="880f3-204">Status of the report execution.</span></span> <span data-ttu-id="880f3-205">Возможные значения: Paused (Приостановлено), Active (Активно) и Inactive (Неактивно).</span><span class="sxs-lookup"><span data-stu-id="880f3-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="880f3-206">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="880f3-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="880f3-207">Интервал повторения, указанный в полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="880f3-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="880f3-208">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="880f3-208">RecurrenceCount</span></span>     |    <span data-ttu-id="880f3-209">Число повторений, указанное в полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="880f3-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="880f3-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="880f3-210">CallbackUrl</span></span>     |    <span data-ttu-id="880f3-211">URL-адрес обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="880f3-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="880f3-212">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="880f3-212">CallbackMethod</span></span>    |    <span data-ttu-id="880f3-213">Метод обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="880f3-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="880f3-214">Формат</span><span class="sxs-lookup"><span data-stu-id="880f3-214">Format</span></span>     |    <span data-ttu-id="880f3-215">Формат файлов отчета</span><span class="sxs-lookup"><span data-stu-id="880f3-215">Format of the report files</span></span>     |
|    <span data-ttu-id="880f3-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="880f3-216">TotalCount</span></span>     |    <span data-ttu-id="880f3-217">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="880f3-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="880f3-218">Сообщение</span><span class="sxs-lookup"><span data-stu-id="880f3-218">Message</span></span>     |    <span data-ttu-id="880f3-219">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="880f3-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="880f3-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="880f3-220">StatusCode</span></span>     |    <span data-ttu-id="880f3-221">Код результата.</span><span class="sxs-lookup"><span data-stu-id="880f3-221">Result Code.</span></span> <span data-ttu-id="880f3-222">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="880f3-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |