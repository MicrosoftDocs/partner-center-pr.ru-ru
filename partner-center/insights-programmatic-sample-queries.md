---
title: Список примеров запросов
description: Используйте примеры запросов для программного доступа к данным аналитики Partner Insights.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375852"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Примеры запросов для отчета центра партнеров

в этой статье приведены примеры запросов для партнеров, Аналитика отчеты. Эти запросы можно использовать путем вызова конечной точки API Create Report Query. При необходимости можно изменить вызов [API создания запроса отчета](insights-programmatic-access-paradigm.md#create-report-query-api) , чтобы добавить дополнительные столбцы, настроить период вычисления и добавить условия фильтра.

Дополнительные сведения о именах, атрибутах и описаниях столбцов см. в разделе [определения данных](insights-data-definitions.md).

## <a name="customer-details"></a>данные о клиентах

Эти примеры запросов относятся к отчету "сведения о клиентах":

### <a name="by-geography"></a>По географическому

Список клиентов из определенной географии за прошлый месяц.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>По SKU и счету за выручку

Список клиентов, использующих конкретный номер SKU и счет выручки, превышает 20 000 за последние 6 месяцев

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>По доступным местам

10 лучших клиентов на основе доступных мест за прошлый месяц

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Профиль партнера

Эти примеры запросов применяются к отчету о профиле партнера:

### <a name="by-geography"></a>По географическому

Список партнеров из определенного географического объекта.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>По партнеру MPN

Список партнеров в пределах одного MPN-партнера в КОРПУСе

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Производительность торгового посредника

Эти примеры запросов применяются к отчету "производительность торгового посредника":

### <a name="by-geography"></a>По географическому

Список торговых посредников из определенной географии за прошлый месяц.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>По торговому посреднику

Число клиентов, число подписок, общее количество доступных мест, общее число назначенных мест, общий доход для конкретного торгового посредника.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Первые 10 по доходу

10 лучших торговых посредников на основе общего дохода за прошлый месяц.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Сведения о подписке

Эти примеры запросов относятся к отчету "сведения о подписке":

### <a name="by-renewal-eligibility"></a>По допустимости продления

Список подписок, которые не могут быть включены в автоматическое продление за прошлый месяц.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>По состоянию подписки

Список подписок, которые находятся в состоянии отключения за прошлый месяц.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Число за шесть месяцев

Число подписок, общее число проданных рабочих мест, количество клиентов для конкретного партнера за последние шесть месяцев.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Использование Azure

Эти примеры запросов относятся к отчету об использовании Azure:

### <a name="by-meter-category"></a>По категории счетчиков

Список подписок на использование Azure с единицами использования и записью контроля доступа для определенной категории счетчиков за последние шесть месяцев.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>По общему количеству записей контроля доступа

Список подписок на использование Azure, в которых общая запись контроля доступа превышает 20 000 за последние шесть месяцев

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Дальнейшие действия

- [Интерфейсы API для доступа к данным аналитики Partner Insights](insights-programmatic-analytics-available-api.md)