---
title: Список API для доступа к данным Partner Insights
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Список API для доступа к данным Partner Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376078"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="48310-103">Доступные API для аналитики Partner Insights</span><span class="sxs-lookup"><span data-stu-id="48310-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="48310-104">Ниже приведен список интерфейсов API для аналитики Partner Insights и связанных с ними функций.</span><span class="sxs-lookup"><span data-stu-id="48310-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="48310-105">API-интерфейсы извлечения набора данных</span><span class="sxs-lookup"><span data-stu-id="48310-105">Dataset pull APIs</span></span>

<span data-ttu-id="48310-106">***Таблица 1. API-интерфейсы извлечения набора данных***</span><span class="sxs-lookup"><span data-stu-id="48310-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="48310-107">**API**</span><span class="sxs-lookup"><span data-stu-id="48310-107">**API**</span></span> | <span data-ttu-id="48310-108">**Функциональность**</span><span class="sxs-lookup"><span data-stu-id="48310-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="48310-109">Получение всех наборов данных</span><span class="sxs-lookup"><span data-stu-id="48310-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="48310-110">Возвращает все доступные наборы данных.</span><span class="sxs-lookup"><span data-stu-id="48310-110">Gets all the available datasets.</span></span> <span data-ttu-id="48310-111">Наборы данных содержат список таблиц, столбцов, метрик и диапазонов времени.</span><span class="sxs-lookup"><span data-stu-id="48310-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="48310-112">API-интерфейсы управления запросами</span><span class="sxs-lookup"><span data-stu-id="48310-112">Query management APIs</span></span>

<span data-ttu-id="48310-113">***Таблица 2. API-интерфейсы управления запросами***</span><span class="sxs-lookup"><span data-stu-id="48310-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="48310-114">**API**</span><span class="sxs-lookup"><span data-stu-id="48310-114">**API**</span></span> | <span data-ttu-id="48310-115">**Функциональность**</span><span class="sxs-lookup"><span data-stu-id="48310-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="48310-116">Создание запроса отчета</span><span class="sxs-lookup"><span data-stu-id="48310-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="48310-117">Позволяет создавать пользовательские запросы, определяющие набор данных, из которого необходимо экспортировать столбцы и метрики.</span><span class="sxs-lookup"><span data-stu-id="48310-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="48310-118">ПОЛУЧЕНИЕ запроса отчета</span><span class="sxs-lookup"><span data-stu-id="48310-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="48310-119">Возвращает все запросы, доступные для использования в отчетах.</span><span class="sxs-lookup"><span data-stu-id="48310-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="48310-120">Возвращает все системные и пользовательские запросы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="48310-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="48310-121">УДАЛИТЬ запрос отчета</span><span class="sxs-lookup"><span data-stu-id="48310-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="48310-122">Позволяет удалять определяемые пользователем запросы.</span><span class="sxs-lookup"><span data-stu-id="48310-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="48310-123">API-интерфейсы управления отчетами</span><span class="sxs-lookup"><span data-stu-id="48310-123">Report management APIs</span></span>

<span data-ttu-id="48310-124">***Таблица 3. API-интерфейсы управления отчетами***</span><span class="sxs-lookup"><span data-stu-id="48310-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="48310-125">**API**</span><span class="sxs-lookup"><span data-stu-id="48310-125">**API**</span></span> | <span data-ttu-id="48310-126">**Функциональность**</span><span class="sxs-lookup"><span data-stu-id="48310-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="48310-127">Создание отчета</span><span class="sxs-lookup"><span data-stu-id="48310-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="48310-128">Позволяет запланировать выполнение запроса через равные интервалы времени.</span><span class="sxs-lookup"><span data-stu-id="48310-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="48310-129">Попробуйте запросить отчет</span><span class="sxs-lookup"><span data-stu-id="48310-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="48310-130">Выполняет инструкцию запроса отчета.</span><span class="sxs-lookup"><span data-stu-id="48310-130">Executes a Report query statement.</span></span> <span data-ttu-id="48310-131">Возвращает только 10 записей, которые партнер может использовать для проверки соответствия ожидаемым данных.</span><span class="sxs-lookup"><span data-stu-id="48310-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="48310-132">Получить отчет</span><span class="sxs-lookup"><span data-stu-id="48310-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="48310-133">Возвращает все запланированные отчеты.</span><span class="sxs-lookup"><span data-stu-id="48310-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="48310-134">Обновление отчета</span><span class="sxs-lookup"><span data-stu-id="48310-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="48310-135">Позволяет изменить параметр отчета.</span><span class="sxs-lookup"><span data-stu-id="48310-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="48310-136">Удаление отчета</span><span class="sxs-lookup"><span data-stu-id="48310-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="48310-137">Позволяет удалять все записи отчета и выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="48310-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="48310-138">Приостановка выполнения отчетов</span><span class="sxs-lookup"><span data-stu-id="48310-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="48310-139">Позволяет приостановить запланированное выполнение отчетов.</span><span class="sxs-lookup"><span data-stu-id="48310-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="48310-140">Возобновление выполнения отчетов</span><span class="sxs-lookup"><span data-stu-id="48310-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="48310-141">Позволяет возобновить запланированное выполнение приостановленного отчета.</span><span class="sxs-lookup"><span data-stu-id="48310-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="48310-142">API-интерфейсы извлечения сведений о выполнении отчета</span><span class="sxs-lookup"><span data-stu-id="48310-142">Report execution pull APIs</span></span>

<span data-ttu-id="48310-143">***Таблица 4. API-интерфейсы извлечения сведений о выполнении отчета***</span><span class="sxs-lookup"><span data-stu-id="48310-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="48310-144">**API**</span><span class="sxs-lookup"><span data-stu-id="48310-144">**API**</span></span> | <span data-ttu-id="48310-145">**Функциональность**</span><span class="sxs-lookup"><span data-stu-id="48310-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="48310-146">Получение сведений о выполнении отчета</span><span class="sxs-lookup"><span data-stu-id="48310-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="48310-147">Получение сведений обо всех выполнениях, осуществленных для указанного отчета.</span><span class="sxs-lookup"><span data-stu-id="48310-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="48310-148">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="48310-148">Next steps</span></span>

- <span data-ttu-id="48310-149">Вы можете поработать с API-интерфейсами с помощью [URL-адреса API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span><span class="sxs-lookup"><span data-stu-id="48310-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>