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
# <a name="available-apis-for-partner-insights-analytics"></a>Доступные API для аналитики Partner Insights

Ниже приведен список интерфейсов API для аналитики Partner Insights и связанных с ними функций.

## <a name="dataset-pull-apis"></a>API-интерфейсы извлечения набора данных

***Таблица 1. API-интерфейсы извлечения набора данных***

| **API** | **Функциональность** |
| --- | --- |
| [Получение всех наборов данных](insights-programmatic-analytics-api-get-dataset.md) | Возвращает все доступные наборы данных. Наборы данных содержат список таблиц, столбцов, метрик и диапазонов времени. |
|||

## <a name="query-management-apis"></a>API-интерфейсы управления запросами

***Таблица 2. API-интерфейсы управления запросами***

| **API** | **Функциональность** |
| --- | --- |
| [Создание запроса отчета](insights-programmatic-access-paradigm.md#create-report-query-api) | Позволяет создавать пользовательские запросы, определяющие набор данных, из которого необходимо экспортировать столбцы и метрики. |
| [ПОЛУЧЕНИЕ запроса отчета](insights-programmatic-analytics-api-get-report-queries.md) | Возвращает все запросы, доступные для использования в отчетах. Возвращает все системные и пользовательские запросы по умолчанию. |
| [УДАЛИТЬ запрос отчета](insights-programmatic-analytics-api-delete-report-queries.md) | Позволяет удалять определяемые пользователем запросы. |
|||

## <a name="report-management-apis"></a>API-интерфейсы управления отчетами

***Таблица 3. API-интерфейсы управления отчетами***

| **API** | **Функциональность** |
| --- | --- |
| [Создание отчета](insights-programmatic-access-paradigm.md#create-report-api) | Позволяет запланировать выполнение запроса через равные интервалы времени. |
| [Попробуйте запросить отчет](insights-programmatic-analytics-api-try-report-queries.md) | Выполняет инструкцию запроса отчета. Возвращает только 10 записей, которые партнер может использовать для проверки соответствия ожидаемым данных. |
| [Получить отчет](insights-programmatic-analytics-api-get-report.md) | Возвращает все запланированные отчеты. |
| [Обновление отчета](insights-programmatic-analytics-api-update-report.md) | Позволяет изменить параметр отчета. |
| [Удаление отчета](insights-programmatic-analytics-api-delete-report.md) | Позволяет удалять все записи отчета и выполнения отчета. |
| [Приостановка выполнения отчетов](insights-programmatic-analytics-api-pause-report-executions.md) | Позволяет приостановить запланированное выполнение отчетов. |
| [Возобновление выполнения отчетов](insights-programmatic-analytics-api-resume-report-executions.md) | Позволяет возобновить запланированное выполнение приостановленного отчета. |
|||

## <a name="report-execution-pull-apis"></a>API-интерфейсы извлечения сведений о выполнении отчета

***Таблица 4. API-интерфейсы извлечения сведений о выполнении отчета***

| **API** | **Функциональность** |
| --- | --- |
| [Получение сведений о выполнении отчета](insights-programmatic-access-paradigm.md#get-report-execution-api) | Получение сведений обо всех выполнениях, осуществленных для указанного отчета. |
|||

## <a name="next-steps"></a>Дальнейшие действия

- Вы можете поработать с API-интерфейсами с помощью [URL-адреса API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).