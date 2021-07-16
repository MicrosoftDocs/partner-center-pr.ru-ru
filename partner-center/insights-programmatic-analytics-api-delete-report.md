---
title: удалить API отчета — Аналитика данные
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API для удаления любого отчета в центре партнеров Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376139"
---
# <a name="delete-report-api"></a><span data-ttu-id="e27df-103">API удаления отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-103">Delete report API</span></span>

<span data-ttu-id="e27df-104">При запуске этот API удаляет все записи об отчетах и выполнении отчетов.</span><span class="sxs-lookup"><span data-stu-id="e27df-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="e27df-105">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="e27df-105">**Request syntax**</span></span>

|    <span data-ttu-id="e27df-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e27df-106">Method</span></span>    |    <span data-ttu-id="e27df-107">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="e27df-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="e27df-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="e27df-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="e27df-109">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="e27df-109">**Request header**</span></span>

|    <span data-ttu-id="e27df-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e27df-110">Header</span></span>    |    <span data-ttu-id="e27df-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e27df-111">Type</span></span>    |    <span data-ttu-id="e27df-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e27df-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="e27df-113">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e27df-113">Authorization</span></span>    |    <span data-ttu-id="e27df-114">строка</span><span class="sxs-lookup"><span data-stu-id="e27df-114">string</span></span>    |    <span data-ttu-id="e27df-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e27df-115">Required.</span></span> <span data-ttu-id="e27df-116">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="e27df-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="e27df-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e27df-117">Content-Type</span></span>    |    <span data-ttu-id="e27df-118">строка</span><span class="sxs-lookup"><span data-stu-id="e27df-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="e27df-119">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="e27df-119">**Path parameter**</span></span>

|    <span data-ttu-id="e27df-120">имени параметра</span><span class="sxs-lookup"><span data-stu-id="e27df-120">Parameter Name</span></span>    |    <span data-ttu-id="e27df-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e27df-121">Type</span></span>    |    <span data-ttu-id="e27df-122">Обязательно</span><span class="sxs-lookup"><span data-stu-id="e27df-122">Required</span></span>    |    <span data-ttu-id="e27df-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e27df-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="e27df-124">reportId</span><span class="sxs-lookup"><span data-stu-id="e27df-124">reportId</span></span>     |    <span data-ttu-id="e27df-125">строка</span><span class="sxs-lookup"><span data-stu-id="e27df-125">string</span></span>    |    <span data-ttu-id="e27df-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e27df-126">No</span></span>    |    <span data-ttu-id="e27df-127">Идентификатор удаляемого отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="e27df-128">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="e27df-128">**Query parameter**</span></span>

<span data-ttu-id="e27df-129">Нет</span><span class="sxs-lookup"><span data-stu-id="e27df-129">None</span></span>

<span data-ttu-id="e27df-130">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="e27df-130">**Request payload**</span></span>

<span data-ttu-id="e27df-131">Нет</span><span class="sxs-lookup"><span data-stu-id="e27df-131">None</span></span>

<span data-ttu-id="e27df-132">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="e27df-132">**Glossary**</span></span>

<span data-ttu-id="e27df-133">Нет</span><span class="sxs-lookup"><span data-stu-id="e27df-133">None</span></span>

<span data-ttu-id="e27df-134">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="e27df-134">**Response**</span></span>

<span data-ttu-id="e27df-135">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="e27df-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="e27df-136">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="e27df-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="e27df-137">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="e27df-137">Response payload example:</span></span>

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

<span data-ttu-id="e27df-138">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="e27df-138">**Glossary**</span></span>

<span data-ttu-id="e27df-139">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="e27df-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="e27df-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="e27df-140">Parameter</span></span>    |    <span data-ttu-id="e27df-141">Описание</span><span class="sxs-lookup"><span data-stu-id="e27df-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="e27df-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="e27df-142">ReportId</span></span>     |    <span data-ttu-id="e27df-143">Универсальный уникальный идентификатор (UUID) удаленного отчета.</span><span class="sxs-lookup"><span data-stu-id="e27df-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="e27df-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="e27df-144">ReportName</span></span>     |    <span data-ttu-id="e27df-145">Имя, присвоенное отчету во время создания</span><span class="sxs-lookup"><span data-stu-id="e27df-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="e27df-146">Описание</span><span class="sxs-lookup"><span data-stu-id="e27df-146">Description</span></span>     |    <span data-ttu-id="e27df-147">Описание, заданное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="e27df-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="e27df-148">QueryId</span></span>     |    <span data-ttu-id="e27df-149">Идентификатор запроса, переданный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="e27df-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="e27df-150">Query</span></span>     |    <span data-ttu-id="e27df-151">Текст запроса, который будет выполнен для этого отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="e27df-152">Пользователь</span><span class="sxs-lookup"><span data-stu-id="e27df-152">User</span></span>     |    <span data-ttu-id="e27df-153">Идентификатор пользователя, используемый для создания отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="e27df-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="e27df-154">CreatedTime</span></span>     |    <span data-ttu-id="e27df-155">Время создания отчета.</span><span class="sxs-lookup"><span data-stu-id="e27df-155">Time the report was created.</span></span> <span data-ttu-id="e27df-156">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="e27df-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e27df-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="e27df-157">ModifiedTime</span></span>     |    <span data-ttu-id="e27df-158">Время последнего изменения отчета.</span><span class="sxs-lookup"><span data-stu-id="e27df-158">Time the report was last modified.</span></span> <span data-ttu-id="e27df-159">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="e27df-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e27df-160">ексекутенов</span><span class="sxs-lookup"><span data-stu-id="e27df-160">ExecuteNow</span></span>     |    <span data-ttu-id="e27df-161">Флаг Ексекутенов, установленный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="e27df-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="e27df-162">StartTime</span></span>     |    <span data-ttu-id="e27df-163">Время, когда начнется выполнение отчета.</span><span class="sxs-lookup"><span data-stu-id="e27df-163">Time the report execution will begin.</span></span> <span data-ttu-id="e27df-164">Формат времени: гггг-ММ-ддTЧЧ:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="e27df-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e27df-165">репортстатус</span><span class="sxs-lookup"><span data-stu-id="e27df-165">ReportStatus</span></span>     |    <span data-ttu-id="e27df-166">Состояние выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="e27df-166">Status of the report execution.</span></span> <span data-ttu-id="e27df-167">Возможные значения: Paused (Приостановлено), Active (Активно) и Inactive (Неактивно).</span><span class="sxs-lookup"><span data-stu-id="e27df-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="e27df-168">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="e27df-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="e27df-169">Интервал повторения, указанный при создании отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="e27df-170">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="e27df-170">RecurrenceCount</span></span>     |    <span data-ttu-id="e27df-171">Число повторений, указанное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="e27df-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="e27df-172">CallbackUrl</span></span>     |    <span data-ttu-id="e27df-173">URL-адрес обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="e27df-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="e27df-174">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="e27df-174">CallbackMethod</span></span>    |    <span data-ttu-id="e27df-175">Метод обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="e27df-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="e27df-176">Формат</span><span class="sxs-lookup"><span data-stu-id="e27df-176">Format</span></span>     |    <span data-ttu-id="e27df-177">Формат файлов отчета</span><span class="sxs-lookup"><span data-stu-id="e27df-177">Format of the report files</span></span>     |
|    <span data-ttu-id="e27df-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="e27df-178">TotalCount</span></span>     |    <span data-ttu-id="e27df-179">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="e27df-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="e27df-180">Сообщение</span><span class="sxs-lookup"><span data-stu-id="e27df-180">Message</span></span>     |    <span data-ttu-id="e27df-181">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="e27df-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="e27df-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="e27df-182">StatusCode</span></span>     |    <span data-ttu-id="e27df-183">Код результата.</span><span class="sxs-lookup"><span data-stu-id="e27df-183">Result Code.</span></span> <span data-ttu-id="e27df-184">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="e27df-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
