---
title: Распространенные вопросы о программном доступе к партнерским аналитикам
description: Получите ответы на часто задаваемые вопросы о доступе к данным Partner Insights через API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376059"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a><span data-ttu-id="1f56d-103">Часто задаваемые вопросы о программном доступе к данным аналитики</span><span class="sxs-lookup"><span data-stu-id="1f56d-103">Programmatic access of analytics data common questions</span></span>

<span data-ttu-id="1f56d-104">В этой статье рассматриваются часто задаваемые вопросы о программном доступе к данным Partner Insights в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="1f56d-104">This article addresses commonly asked questions about how to programmatically access partner insights data in Partner Center.</span></span>

## <a name="api-responses"></a><span data-ttu-id="1f56d-105">Ответов API</span><span class="sxs-lookup"><span data-stu-id="1f56d-105">API responses</span></span>

<span data-ttu-id="1f56d-106">При каких сценариях можно получить ответ API, отличный от 200 (успешно)?</span><span class="sxs-lookup"><span data-stu-id="1f56d-106">What are the different scenarios under which I can receive an API response other than 200 (Success)?</span></span>

<span data-ttu-id="1f56d-107">В этой таблице описаны ответы API и действия, которые необходимо выполнить при их получении.</span><span class="sxs-lookup"><span data-stu-id="1f56d-107">This table describes the API responses and what to do if you receive them.</span></span>

|    <span data-ttu-id="1f56d-108">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="1f56d-108">Error description</span></span>     |    <span data-ttu-id="1f56d-109">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="1f56d-109">Error code</span></span>     |    <span data-ttu-id="1f56d-110">Диагностика</span><span class="sxs-lookup"><span data-stu-id="1f56d-110">Troubleshoot</span></span>     |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="1f56d-111">Не авторизовано</span><span class="sxs-lookup"><span data-stu-id="1f56d-111">Unauthorized</span></span>     |    <span data-ttu-id="1f56d-112">401</span><span class="sxs-lookup"><span data-stu-id="1f56d-112">401</span></span>     |    <span data-ttu-id="1f56d-113">Это исключение проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1f56d-113">This is an authentication exception.</span></span> <span data-ttu-id="1f56d-114">проверьте правильность маркера Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="1f56d-114">Check the correctness of the Azure Active Directory (AAD) token.</span></span> <span data-ttu-id="1f56d-115">Токен AAD действителен в течение 60 минут, после чего потребуется повторно создать токен AAD.</span><span class="sxs-lookup"><span data-stu-id="1f56d-115">The AAD token is valid for 60 minutes, after which time you would need to regenerate the AAD token.</span></span>     |
|    <span data-ttu-id="1f56d-116">Недопустимое имя таблицы</span><span class="sxs-lookup"><span data-stu-id="1f56d-116">Invalid table name</span></span>     |    <span data-ttu-id="1f56d-117">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-117">400</span></span>     |    <span data-ttu-id="1f56d-118">Введено неверное имя набора данных.</span><span class="sxs-lookup"><span data-stu-id="1f56d-118">The name of the dataset is wrong.</span></span> <span data-ttu-id="1f56d-119">Снова проверьте имя набора данных, вызвав API "получить все наборы данных".</span><span class="sxs-lookup"><span data-stu-id="1f56d-119">Recheck the dataset name by calling the "Get All Datasets" API.</span></span>     |
|    <span data-ttu-id="1f56d-120">Неправильное имя столбца</span><span class="sxs-lookup"><span data-stu-id="1f56d-120">Incorrect column name</span></span>     |    <span data-ttu-id="1f56d-121">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-121">400</span></span>     |    <span data-ttu-id="1f56d-122">В запросе указано неверное имя столбца.</span><span class="sxs-lookup"><span data-stu-id="1f56d-122">The name of the column in the query is incorrect.</span></span> <span data-ttu-id="1f56d-123">Проверьте имя столбца, вызвав API "получение всех наборов данных" или указав имена столбцов в определениях</span><span class="sxs-lookup"><span data-stu-id="1f56d-123">Recheck the column name by calling the "Get All Datasets" API or refer to the column names in the Data Definitions</span></span>    |
|    <span data-ttu-id="1f56d-124">Значение null или отсутствует</span><span class="sxs-lookup"><span data-stu-id="1f56d-124">Null or missing value</span></span>     |    <span data-ttu-id="1f56d-125">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-125">400</span></span>     |    <span data-ttu-id="1f56d-126">Возможно, отсутствуют обязательные параметры, являющиеся частью полезных данных запроса API.</span><span class="sxs-lookup"><span data-stu-id="1f56d-126">You may be missing mandatory parameters as part of the request payload of the API.</span></span>     |
|    <span data-ttu-id="1f56d-127">Недопустимые параметры отчета</span><span class="sxs-lookup"><span data-stu-id="1f56d-127">Invalid report parameters</span></span>     |    <span data-ttu-id="1f56d-128">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-128">400</span></span>     |    <span data-ttu-id="1f56d-129">Убедитесь, что параметры отчета верны.</span><span class="sxs-lookup"><span data-stu-id="1f56d-129">Make sure the report parameters are correct.</span></span> <span data-ttu-id="1f56d-130">Например, для параметра Рекурренцеинтервал может быть задано значение меньше 4.</span><span class="sxs-lookup"><span data-stu-id="1f56d-130">For example, you may be giving a value of less than 4 for RecurrenceInterval parameter.</span></span>     |
|    <span data-ttu-id="1f56d-131">Интервал повторения должен быть от 4 до 2160</span><span class="sxs-lookup"><span data-stu-id="1f56d-131">Recurrence Interval must be between 4 and 2160</span></span>     |    <span data-ttu-id="1f56d-132">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-132">400</span></span>     |    <span data-ttu-id="1f56d-133">Убедитесь, что значение параметра запроса Рекурренцеинтервал находится в диапазоне от 4 до 2160.</span><span class="sxs-lookup"><span data-stu-id="1f56d-133">Make sure the value of the RecurrenceInterval request parameter is between 4 and 2160.</span></span>     |
|    <span data-ttu-id="1f56d-134">Недопустимый QueryId</span><span class="sxs-lookup"><span data-stu-id="1f56d-134">Invalid QueryId</span></span>     |    <span data-ttu-id="1f56d-135">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-135">400</span></span>     |    <span data-ttu-id="1f56d-136">Проверьте созданный QueryId.</span><span class="sxs-lookup"><span data-stu-id="1f56d-136">Recheck the generated QueryId.</span></span>     |
|    <span data-ttu-id="1f56d-137">Недопустимые параметры отчета для времени начала создания отчета — не менее 4 часов от текущего времени в формате UTC</span><span class="sxs-lookup"><span data-stu-id="1f56d-137">Invalid report parameters for creation - Start time of report should at least be 4 hours from current UTC time</span></span>     |    <span data-ttu-id="1f56d-138">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-138">400</span></span>     |    <span data-ttu-id="1f56d-139">Параметр времени запуска как часть полезных данных запроса не должен быть в прошлом.</span><span class="sxs-lookup"><span data-stu-id="1f56d-139">Start Time parameter as part of request payload shouldn't be in the past.</span></span> <span data-ttu-id="1f56d-140">Время начала отчета должно составлять по крайней мере 4 часа от текущего времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1f56d-140">The start time of the report should be at least 4 hours from the current UTC time.</span></span>     |
|    <span data-ttu-id="1f56d-141">Запрошенное значение "строка" не найдено</span><span class="sxs-lookup"><span data-stu-id="1f56d-141">Requested value 'string' not found</span></span>     |    <span data-ttu-id="1f56d-142">400</span><span class="sxs-lookup"><span data-stu-id="1f56d-142">400</span></span>     |    <span data-ttu-id="1f56d-143">Проверьте, обновлены ли параметры `callbackurl` или формат запроса.</span><span class="sxs-lookup"><span data-stu-id="1f56d-143">Check whether you have updated the request parameters `callbackurl` or format.</span></span>     |
|    <span data-ttu-id="1f56d-144">Не удалось найти элемент с указанными фильтрами.</span><span class="sxs-lookup"><span data-stu-id="1f56d-144">No item found with given filters.</span></span>     |    <span data-ttu-id="1f56d-145">404</span><span class="sxs-lookup"><span data-stu-id="1f56d-145">404</span></span>     |    <span data-ttu-id="1f56d-146">Проверьте параметр идентификатор reportID, используемый в API получения отчетов о выполнении.</span><span class="sxs-lookup"><span data-stu-id="1f56d-146">Check the reportID parameter used in the Get Report Executions API.</span></span>     |
|    <span data-ttu-id="1f56d-147">Не найдено никаких выполнений для заданных условий фильтра.</span><span class="sxs-lookup"><span data-stu-id="1f56d-147">There are no executions that have occurred for the given filter conditions.</span></span> <span data-ttu-id="1f56d-148">Дважды проверьте идентификатор reportID или executionId и повторите попытку API после запланированного времени выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="1f56d-148">Double check the reportId or executionId and retry the API after the report's scheduled execution time</span></span>     |    <span data-ttu-id="1f56d-149">404</span><span class="sxs-lookup"><span data-stu-id="1f56d-149">404</span></span>     |    <span data-ttu-id="1f56d-150">Проверьте правильность идентификатор reportID.</span><span class="sxs-lookup"><span data-stu-id="1f56d-150">Make sure that the reportId is correct.</span></span> <span data-ttu-id="1f56d-151">Повторите попытку API после запланированного времени выполнения отчета, как указано в полезных данных запроса.</span><span class="sxs-lookup"><span data-stu-id="1f56d-151">Retry the API after the report's scheduled execution time as specified in the request payload.</span></span>     |
|    <span data-ttu-id="1f56d-152">Произошла внутренняя ошибка при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="1f56d-152">Internal error encountered while creating report.</span></span> <span data-ttu-id="1f56d-153">Идентификатор корреляции <></span><span class="sxs-lookup"><span data-stu-id="1f56d-153">Correlation ID <></span></span>     |    <span data-ttu-id="1f56d-154">500</span><span class="sxs-lookup"><span data-stu-id="1f56d-154">500</span></span>     |    <span data-ttu-id="1f56d-155">Убедитесь, что формат даты для полей *StartTime*, *куеристарттиме* и *куерендтиме* задан правильно.</span><span class="sxs-lookup"><span data-stu-id="1f56d-155">Make sure that the format of date for the fields *StartTime*, *QueryStartTime*, and *QueryEndTime* are correct.</span></span>     |
|    <span data-ttu-id="1f56d-156">Служба недоступна</span><span class="sxs-lookup"><span data-stu-id="1f56d-156">Service unavailable</span></span>    |    <span data-ttu-id="1f56d-157">500</span><span class="sxs-lookup"><span data-stu-id="1f56d-157">500</span></span>     |    <span data-ttu-id="1f56d-158">При постоянном получении недоступной службы (ошибка 5xx) отправьте запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="1f56d-158">If you continuously receive a service unavailable (5xx error), open a support ticket.</span></span>    |
|        |        |        |

## <a name="no-records"></a><span data-ttu-id="1f56d-159">Записи отсутствуют</span><span class="sxs-lookup"><span data-stu-id="1f56d-159">No records</span></span>

<span data-ttu-id="1f56d-160">Я получаю ответ API 200 при скачивании отчета из безопасного расположения.</span><span class="sxs-lookup"><span data-stu-id="1f56d-160">I receive API response 200 when I download the report from the secure location.</span></span> <span data-ttu-id="1f56d-161">Почему в нем нет записей?</span><span class="sxs-lookup"><span data-stu-id="1f56d-161">Why am I getting no records?</span></span>
<span data-ttu-id="1f56d-162">Проверьте, имеет ли строка в запросе одно из допустимых значений для заголовка столбца.</span><span class="sxs-lookup"><span data-stu-id="1f56d-162">Check whether the string in the query has one of the allowable values for the column header.</span></span> <span data-ttu-id="1f56d-163">Например, этот запрос возвратит нулевые результаты:</span><span class="sxs-lookup"><span data-stu-id="1f56d-163">For example, this query will return zero results:</span></span>

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

<span data-ttu-id="1f56d-164">В этом примере допустимыми значениями для `IsDuplicateRowForPGA` являются 0 или 1.</span><span class="sxs-lookup"><span data-stu-id="1f56d-164">In this example, the allowable values for `IsDuplicateRowForPGA` are 0 or 1.</span></span> <span data-ttu-id="1f56d-165">См. [определения данных](insights-data-definitions.md) для всех возможных значений для различных столбцов.</span><span class="sxs-lookup"><span data-stu-id="1f56d-165">Refer to the [Data Definitions](insights-data-definitions.md) for all possible values for the various columns.</span></span>