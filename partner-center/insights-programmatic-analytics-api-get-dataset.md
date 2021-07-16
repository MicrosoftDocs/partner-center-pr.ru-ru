---
title: получение всех Аналитика данных API-интерфейсов
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте этот API для получения сведений обо всех доступных наборах данных в центре партнеров.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375870"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="41c67-103">API получения всех наборов данных</span><span class="sxs-lookup"><span data-stu-id="41c67-103">Get all datasets API</span></span>

<span data-ttu-id="41c67-104">API получения всех наборов данных возвращает полный список доступных наборов данных.</span><span class="sxs-lookup"><span data-stu-id="41c67-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="41c67-105">Список наборов данных содержит таблицы, столбцы, метрики и диапазоны времени.</span><span class="sxs-lookup"><span data-stu-id="41c67-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="41c67-106">**Синтаксис запроса**</span><span class="sxs-lookup"><span data-stu-id="41c67-106">**Request syntax**</span></span>

|    <span data-ttu-id="41c67-107">Метод</span><span class="sxs-lookup"><span data-stu-id="41c67-107">Method</span></span>    |    <span data-ttu-id="41c67-108">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="41c67-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="41c67-109">GET</span><span class="sxs-lookup"><span data-stu-id="41c67-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="41c67-110">**Заголовок запроса**</span><span class="sxs-lookup"><span data-stu-id="41c67-110">**Request header**</span></span>

|    <span data-ttu-id="41c67-111">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41c67-111">Header</span></span>    |    <span data-ttu-id="41c67-112">Тип</span><span class="sxs-lookup"><span data-stu-id="41c67-112">Type</span></span>    |    <span data-ttu-id="41c67-113">Описание</span><span class="sxs-lookup"><span data-stu-id="41c67-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="41c67-114">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41c67-114">Authorization</span></span>    |    <span data-ttu-id="41c67-115">строка</span><span class="sxs-lookup"><span data-stu-id="41c67-115">string</span></span>    |    <span data-ttu-id="41c67-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41c67-116">Required.</span></span> <span data-ttu-id="41c67-117">маркер доступа Azure Active Directory (AAD) в форме`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="41c67-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="41c67-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41c67-118">Content-Type</span></span>    |    <span data-ttu-id="41c67-119">строка</span><span class="sxs-lookup"><span data-stu-id="41c67-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="41c67-120">**Параметр пути**</span><span class="sxs-lookup"><span data-stu-id="41c67-120">**Path parameter**</span></span>

<span data-ttu-id="41c67-121">Нет</span><span class="sxs-lookup"><span data-stu-id="41c67-121">None</span></span>

<span data-ttu-id="41c67-122">**Параметр запроса**</span><span class="sxs-lookup"><span data-stu-id="41c67-122">**Query parameter**</span></span>

|    <span data-ttu-id="41c67-123">имени параметра</span><span class="sxs-lookup"><span data-stu-id="41c67-123">Parameter Name</span></span>    |    <span data-ttu-id="41c67-124">Тип</span><span class="sxs-lookup"><span data-stu-id="41c67-124">Type</span></span>    |    <span data-ttu-id="41c67-125">Обязательно</span><span class="sxs-lookup"><span data-stu-id="41c67-125">Required</span></span>    |    <span data-ttu-id="41c67-126">Описание</span><span class="sxs-lookup"><span data-stu-id="41c67-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="41c67-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="41c67-127">datasetName</span></span>    |    <span data-ttu-id="41c67-128">строка</span><span class="sxs-lookup"><span data-stu-id="41c67-128">string</span></span>    |    <span data-ttu-id="41c67-129">Нет</span><span class="sxs-lookup"><span data-stu-id="41c67-129">No</span></span>    |    <span data-ttu-id="41c67-130">Фильтр для получения сведений только об одном наборе данных</span><span class="sxs-lookup"><span data-stu-id="41c67-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="41c67-131">**Полезные данные запроса**</span><span class="sxs-lookup"><span data-stu-id="41c67-131">**Request payload**</span></span>

<span data-ttu-id="41c67-132">Нет</span><span class="sxs-lookup"><span data-stu-id="41c67-132">None</span></span>

<span data-ttu-id="41c67-133">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="41c67-133">**Glossary**</span></span>

<span data-ttu-id="41c67-134">Нет</span><span class="sxs-lookup"><span data-stu-id="41c67-134">None</span></span>

<span data-ttu-id="41c67-135">**Ответ**</span><span class="sxs-lookup"><span data-stu-id="41c67-135">**Response**</span></span>

<span data-ttu-id="41c67-136">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="41c67-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="41c67-137">Код отклика: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="41c67-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="41c67-138">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="41c67-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="41c67-139">**Словарь терминов**</span><span class="sxs-lookup"><span data-stu-id="41c67-139">**Glossary**</span></span>

<span data-ttu-id="41c67-140">В следующей таблице описаны ключевые элементы ответа.</span><span class="sxs-lookup"><span data-stu-id="41c67-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="41c67-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="41c67-141">Parameter</span></span>    |    <span data-ttu-id="41c67-142">Описание</span><span class="sxs-lookup"><span data-stu-id="41c67-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="41c67-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="41c67-143">DatasetName</span></span>     |    <span data-ttu-id="41c67-144">Имя набора данных, определяемого этим объектом массива.</span><span class="sxs-lookup"><span data-stu-id="41c67-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="41c67-145">селектаблеколумнс</span><span class="sxs-lookup"><span data-stu-id="41c67-145">SelectableColumns</span></span>     |    <span data-ttu-id="41c67-146">Необработанные столбцы, которые можно указать в операции SELECT COLUMNS.</span><span class="sxs-lookup"><span data-stu-id="41c67-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="41c67-147">аваилаблеметрикс</span><span class="sxs-lookup"><span data-stu-id="41c67-147">AvailableMetrics</span></span>     |    <span data-ttu-id="41c67-148">Имена столбцов агрегирования и метрик, которые можно указать в операции SELECT COLUMNS.</span><span class="sxs-lookup"><span data-stu-id="41c67-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="41c67-149">аваилабледатеранжес</span><span class="sxs-lookup"><span data-stu-id="41c67-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="41c67-150">Диапазон дат, который можно использовать в запросах отчета для набора данных.</span><span class="sxs-lookup"><span data-stu-id="41c67-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="41c67-151">минимумрекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="41c67-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="41c67-152">Минимальное значение интервала повторения</span><span class="sxs-lookup"><span data-stu-id="41c67-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="41c67-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="41c67-153">TotalCount</span></span>     |    <span data-ttu-id="41c67-154">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="41c67-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="41c67-155">Сообщение</span><span class="sxs-lookup"><span data-stu-id="41c67-155">Message</span></span>     |    <span data-ttu-id="41c67-156">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="41c67-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="41c67-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="41c67-157">StatusCode</span></span>     |    <span data-ttu-id="41c67-158">Код результата.</span><span class="sxs-lookup"><span data-stu-id="41c67-158">Result Code.</span></span> <span data-ttu-id="41c67-159">Возможные значения: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="41c67-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
