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
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="04a10-103">Примеры запросов для отчета центра партнеров</span><span class="sxs-lookup"><span data-stu-id="04a10-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="04a10-104">в этой статье приведены примеры запросов для партнеров, Аналитика отчеты.</span><span class="sxs-lookup"><span data-stu-id="04a10-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="04a10-105">Эти запросы можно использовать путем вызова конечной точки API Create Report Query.</span><span class="sxs-lookup"><span data-stu-id="04a10-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="04a10-106">При необходимости можно изменить вызов [API создания запроса отчета](insights-programmatic-access-paradigm.md#create-report-query-api) , чтобы добавить дополнительные столбцы, настроить период вычисления и добавить условия фильтра.</span><span class="sxs-lookup"><span data-stu-id="04a10-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="04a10-107">Дополнительные сведения о именах, атрибутах и описаниях столбцов см. в разделе [определения данных](insights-data-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="04a10-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="04a10-108">данные о клиентах</span><span class="sxs-lookup"><span data-stu-id="04a10-108">Customer details</span></span>

<span data-ttu-id="04a10-109">Эти примеры запросов относятся к отчету "сведения о клиентах":</span><span class="sxs-lookup"><span data-stu-id="04a10-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="04a10-110">По географическому</span><span class="sxs-lookup"><span data-stu-id="04a10-110">By geography</span></span>

<span data-ttu-id="04a10-111">Список клиентов из определенной географии за прошлый месяц.</span><span class="sxs-lookup"><span data-stu-id="04a10-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="04a10-112">По SKU и счету за выручку</span><span class="sxs-lookup"><span data-stu-id="04a10-112">By SKU and billed revenue</span></span>

<span data-ttu-id="04a10-113">Список клиентов, использующих конкретный номер SKU и счет выручки, превышает 20 000 за последние 6 месяцев</span><span class="sxs-lookup"><span data-stu-id="04a10-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="04a10-114">По доступным местам</span><span class="sxs-lookup"><span data-stu-id="04a10-114">By available seats</span></span>

<span data-ttu-id="04a10-115">10 лучших клиентов на основе доступных мест за прошлый месяц</span><span class="sxs-lookup"><span data-stu-id="04a10-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="04a10-116">Профиль партнера</span><span class="sxs-lookup"><span data-stu-id="04a10-116">Partner Profile</span></span>

<span data-ttu-id="04a10-117">Эти примеры запросов применяются к отчету о профиле партнера:</span><span class="sxs-lookup"><span data-stu-id="04a10-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="04a10-118">По географическому</span><span class="sxs-lookup"><span data-stu-id="04a10-118">By geography</span></span>

<span data-ttu-id="04a10-119">Список партнеров из определенного географического объекта.</span><span class="sxs-lookup"><span data-stu-id="04a10-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="04a10-120">По партнеру MPN</span><span class="sxs-lookup"><span data-stu-id="04a10-120">By MPN partner</span></span>

<span data-ttu-id="04a10-121">Список партнеров в пределах одного MPN-партнера в КОРПУСе</span><span class="sxs-lookup"><span data-stu-id="04a10-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="04a10-122">Производительность торгового посредника</span><span class="sxs-lookup"><span data-stu-id="04a10-122">Reseller Performance</span></span>

<span data-ttu-id="04a10-123">Эти примеры запросов применяются к отчету "производительность торгового посредника":</span><span class="sxs-lookup"><span data-stu-id="04a10-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="04a10-124">По географическому</span><span class="sxs-lookup"><span data-stu-id="04a10-124">By geography</span></span>

<span data-ttu-id="04a10-125">Список торговых посредников из определенной географии за прошлый месяц.</span><span class="sxs-lookup"><span data-stu-id="04a10-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="04a10-126">По торговому посреднику</span><span class="sxs-lookup"><span data-stu-id="04a10-126">By reseller</span></span>

<span data-ttu-id="04a10-127">Число клиентов, число подписок, общее количество доступных мест, общее число назначенных мест, общий доход для конкретного торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="04a10-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="04a10-128">Первые 10 по доходу</span><span class="sxs-lookup"><span data-stu-id="04a10-128">Top 10 by revenue</span></span>

<span data-ttu-id="04a10-129">10 лучших торговых посредников на основе общего дохода за прошлый месяц.</span><span class="sxs-lookup"><span data-stu-id="04a10-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="04a10-130">Сведения о подписке</span><span class="sxs-lookup"><span data-stu-id="04a10-130">Subscription Details</span></span>

<span data-ttu-id="04a10-131">Эти примеры запросов относятся к отчету "сведения о подписке":</span><span class="sxs-lookup"><span data-stu-id="04a10-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="04a10-132">По допустимости продления</span><span class="sxs-lookup"><span data-stu-id="04a10-132">By renewal eligibility</span></span>

<span data-ttu-id="04a10-133">Список подписок, которые не могут быть включены в автоматическое продление за прошлый месяц.</span><span class="sxs-lookup"><span data-stu-id="04a10-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="04a10-134">По состоянию подписки</span><span class="sxs-lookup"><span data-stu-id="04a10-134">By subscription state</span></span>

<span data-ttu-id="04a10-135">Список подписок, которые находятся в состоянии отключения за прошлый месяц.</span><span class="sxs-lookup"><span data-stu-id="04a10-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="04a10-136">Число за шесть месяцев</span><span class="sxs-lookup"><span data-stu-id="04a10-136">Counts for six months</span></span>

<span data-ttu-id="04a10-137">Число подписок, общее число проданных рабочих мест, количество клиентов для конкретного партнера за последние шесть месяцев.</span><span class="sxs-lookup"><span data-stu-id="04a10-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="04a10-138">Использование Azure</span><span class="sxs-lookup"><span data-stu-id="04a10-138">Azure Usage</span></span>

<span data-ttu-id="04a10-139">Эти примеры запросов относятся к отчету об использовании Azure:</span><span class="sxs-lookup"><span data-stu-id="04a10-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="04a10-140">По категории счетчиков</span><span class="sxs-lookup"><span data-stu-id="04a10-140">By meter category</span></span>

<span data-ttu-id="04a10-141">Список подписок на использование Azure с единицами использования и записью контроля доступа для определенной категории счетчиков за последние шесть месяцев.</span><span class="sxs-lookup"><span data-stu-id="04a10-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="04a10-142">По общему количеству записей контроля доступа</span><span class="sxs-lookup"><span data-stu-id="04a10-142">By total ACR</span></span>

<span data-ttu-id="04a10-143">Список подписок на использование Azure, в которых общая запись контроля доступа превышает 20 000 за последние шесть месяцев</span><span class="sxs-lookup"><span data-stu-id="04a10-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="04a10-144">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="04a10-144">Next steps</span></span>

- [<span data-ttu-id="04a10-145">Интерфейсы API для доступа к данным аналитики Partner Insights</span><span class="sxs-lookup"><span data-stu-id="04a10-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)