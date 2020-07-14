---
title: Использование аналитики центра партнеров для Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как просматривать бизнес-данные с помощью приложения аналитики центра партнеров для Power BI (для прямых партнеров в CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302290"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="e71ca-103">Просматривайте бизнес-данные с помощью приложения "Аналитика Центра партнеров для Microsoft Power BI"</span><span class="sxs-lookup"><span data-stu-id="e71ca-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="e71ca-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="e71ca-104">**Applies to**</span></span>

- <span data-ttu-id="e71ca-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="e71ca-105">Partner Center</span></span>

<span data-ttu-id="e71ca-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="e71ca-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e71ca-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e71ca-107">Global admin</span></span>
- <span data-ttu-id="e71ca-108">администратор пользователей.</span><span class="sxs-lookup"><span data-stu-id="e71ca-108">User admin</span></span>
- <span data-ttu-id="e71ca-109">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="e71ca-109">Sales agent</span></span>
- <span data-ttu-id="e71ca-110">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="e71ca-110">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="e71ca-111">Просмотр бизнес-данных</span><span class="sxs-lookup"><span data-stu-id="e71ca-111">View your business data</span></span>

<span data-ttu-id="e71ca-112">Получите визуальное представление бизнес-данных с помощью приложения "Аналитика Центра партнеров для Power BI", в том числе:</span><span class="sxs-lookup"><span data-stu-id="e71ca-112">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="e71ca-113">роста числа клиентов, подписок и лицензий;</span><span class="sxs-lookup"><span data-stu-id="e71ca-113">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="e71ca-114">использования Office 365, Microsoft Dynamics и Microsoft Azure;</span><span class="sxs-lookup"><span data-stu-id="e71ca-114">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="e71ca-115">ежедневных единиц потребления измеряемых ресурсов для каждой подписки Azure за последние 60 дней;</span><span class="sxs-lookup"><span data-stu-id="e71ca-115">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="e71ca-116">определения стоимости на основе последней тарифной карты;</span><span class="sxs-lookup"><span data-stu-id="e71ca-116">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="e71ca-117">Возможность экспорта наборов данных и создания настраиваемых отчетов, в том числе для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="e71ca-117">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="e71ca-118">Сведения о предварительной версии приложения "Аналитика Центра партнеров"</span><span class="sxs-lookup"><span data-stu-id="e71ca-118">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="e71ca-119">Это приложение предназначено только для прямых партнеров в программе поставщиков облачных решений.</span><span class="sxs-lookup"><span data-stu-id="e71ca-119">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="e71ca-120">Другие партнеров в программе CSP (например, косвенные торговые посредники) не смогут выполнить вход в приложение.</span><span class="sxs-lookup"><span data-stu-id="e71ca-120">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="e71ca-121">Любые приблизительные расходы основаны на счетах до уплаты налогов и не обладают обязательным характером.</span><span class="sxs-lookup"><span data-stu-id="e71ca-121">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="e71ca-122">Приблизительные расходы предназначены только для оценки данных.</span><span class="sxs-lookup"><span data-stu-id="e71ca-122">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="e71ca-123">Сведения о клиентах основаны на подписках.</span><span class="sxs-lookup"><span data-stu-id="e71ca-123">Customer information is based on subscriptions.</span></span> <span data-ttu-id="e71ca-124">Любые клиенты, для которых вы недавно создали учетные записи, но у которых еще нет подписки, не включены в расчеты.</span><span class="sxs-lookup"><span data-stu-id="e71ca-124">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="e71ca-125">Приблизительные расходы основаны на последней тарифной карте, которая базируются на ценах CSP.</span><span class="sxs-lookup"><span data-stu-id="e71ca-125">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="e71ca-126">Дни являются календарными.</span><span class="sxs-lookup"><span data-stu-id="e71ca-126">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="e71ca-127">Отчет о бизнес-инсайтах</span><span class="sxs-lookup"><span data-stu-id="e71ca-127">Business Insights report</span></span>

- <span data-ttu-id="e71ca-128">**Клиенты заказчика**: количество различных клиентов Azure AD заказчиков, которые приобрели подписки</span><span class="sxs-lookup"><span data-stu-id="e71ca-128">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="e71ca-129">**Новые (за последние 30 дней)**: новые клиенты, которые приобрели по крайней мере одну подписку за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="e71ca-129">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="e71ca-130">**Обновление (за последние 30 дней)**: клиенты, не имеющие "активных", "льготных" или "отключенных" подписок</span><span class="sxs-lookup"><span data-stu-id="e71ca-130">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="e71ca-131">**Новые (за последние 24 часа)**: новые клиенты, которые приобрели по крайней мере одну подписку за последние 24 часа</span><span class="sxs-lookup"><span data-stu-id="e71ca-131">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="e71ca-132">**Приблизительные месячные затраты за последние 12 месяцев**: помесячная тенденция приблизительных расходов до уплаты налогов за последние 12 месяцев</span><span class="sxs-lookup"><span data-stu-id="e71ca-132">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e71ca-133">**Приблизительные затраты по продуктам за последние 12 месяцев**: проданные продукты, упорядоченные по сумме приблизительных расходов до уплаты налогов за последние 12 месяцев.</span><span class="sxs-lookup"><span data-stu-id="e71ca-133">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="e71ca-134">Это состояние указывает лучшие продукты, которые приносят большую прибыль.</span><span class="sxs-lookup"><span data-stu-id="e71ca-134">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="e71ca-135">**Клиенты за последние 12 месяцев**: помесячная тенденция новых клиентов и потерянных клиентов за последние 12 месяцев</span><span class="sxs-lookup"><span data-stu-id="e71ca-135">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e71ca-136">**Приблизительные затраты по клиентам за последние 12 месяцев**: клиенты, упорядоченные по сумме приблизительных расходов до уплаты налогов за последние 12 месяцев.</span><span class="sxs-lookup"><span data-stu-id="e71ca-136">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="e71ca-137">Это состояние указывает топ клиентов, которые приносят большую прибыль.</span><span class="sxs-lookup"><span data-stu-id="e71ca-137">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="e71ca-138">**Число клиентов по продуктам**: проданные продукты, упорядоченные по связанным клиентам.</span><span class="sxs-lookup"><span data-stu-id="e71ca-138">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="e71ca-139">Это состояние указывает лучшие продукты, продаваемые большинству клиентов.</span><span class="sxs-lookup"><span data-stu-id="e71ca-139">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="e71ca-140">Аналитический отчет о подписках</span><span class="sxs-lookup"><span data-stu-id="e71ca-140">Subscription Insights report</span></span>

- <span data-ttu-id="e71ca-141">**Состояние подписки**:</span><span class="sxs-lookup"><span data-stu-id="e71ca-141">**Subscription status**:</span></span>

- <span data-ttu-id="e71ca-142">Active: подписки, принадлежащие состоянию "активный" или "в льготном состоянии"</span><span class="sxs-lookup"><span data-stu-id="e71ca-142">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="e71ca-143">Приостановлено: подписки, принадлежащие состоянию "отключено"</span><span class="sxs-lookup"><span data-stu-id="e71ca-143">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="e71ca-144">Отмена подготовки: подписки, принадлежащие "отменено" или "истек срок действия"</span><span class="sxs-lookup"><span data-stu-id="e71ca-144">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="e71ca-145">**Состояние срока действия**:</span><span class="sxs-lookup"><span data-stu-id="e71ca-145">**Expiry status**:</span></span>

  - <span data-ttu-id="e71ca-146">Срок действия истек: подписки, срок действия которых истек (дата завершения действия подписки находится в прошлом)</span><span class="sxs-lookup"><span data-stu-id="e71ca-146">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="e71ca-147">Срок действия истекает после 30 дней: подписки, срок действия которых истекает после 30 дней (дата завершения действия подписки приходится на дату после следующих 30 дней)</span><span class="sxs-lookup"><span data-stu-id="e71ca-147">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="e71ca-148">Срок действия истекает через 30 дней: подписки, срок действия которых истекает через 30 дней (дата завершения действия подписки приходится на период между сегодняшней датой и следующими 30 днями)</span><span class="sxs-lookup"><span data-stu-id="e71ca-148">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="e71ca-149">**Всего подписок**: подписки в состоянии "активно", "по льготе" или "отключено"</span><span class="sxs-lookup"><span data-stu-id="e71ca-149">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="e71ca-150">**Новые (за последние 30 дней)**: новые подписки, которые клиенты приобрели за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="e71ca-150">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="e71ca-151">**Новые (за последние 24 часа)**: новые подписки, которые клиенты приобрели за последние 24 часа</span><span class="sxs-lookup"><span data-stu-id="e71ca-151">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="e71ca-152">**Срок действия истекает через 30 дней**: подписки, срок действия которых истекает в течение следующих 30 дней</span><span class="sxs-lookup"><span data-stu-id="e71ca-152">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="e71ca-153">**Отток (за последние 30 дней)**: подписки, которые были отменены или приостановлены (отключены) за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="e71ca-153">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="e71ca-154">**Распределение по типам подписок**:% распределения общих подписок по типам подписок на основе лицензий и использования</span><span class="sxs-lookup"><span data-stu-id="e71ca-154">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="e71ca-155">**Число активных подписок по продуктам**: проданные продукты, упорядоченные по количеству активных подписок</span><span class="sxs-lookup"><span data-stu-id="e71ca-155">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="e71ca-156">**Подписки за последние 12 месяцев**: помесячная тенденция новых подписок и потерянных подписок за последние 12 месяцев</span><span class="sxs-lookup"><span data-stu-id="e71ca-156">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e71ca-157">**Сведения о клиентской подписке**: подробное представление о клиентах, подписках и предложениях</span><span class="sxs-lookup"><span data-stu-id="e71ca-157">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="e71ca-158">Аналитический отчет по лицензиям:</span><span class="sxs-lookup"><span data-stu-id="e71ca-158">License Insights report:</span></span>

- <span data-ttu-id="e71ca-159">**Всего лицензий**: общее число лицензий, агрегированных по всем подпискам на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="e71ca-159">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="e71ca-160">**Новые (за последние 30 дней)**: лицензии, добавленные за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="e71ca-160">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="e71ca-161">**Отток (за последние 30 дней)**: лицензии, отмененные за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="e71ca-161">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="e71ca-162">**Новые (за последние 24 часа)**: лицензии, добавленные за последние 24 часа</span><span class="sxs-lookup"><span data-stu-id="e71ca-162">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="e71ca-163">**Лицензии за последние 90 дней**: помесячная тенденция добавления и удаления лицензий за последние 90 дней</span><span class="sxs-lookup"><span data-stu-id="e71ca-163">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="e71ca-164">**Число активных лицензий по продуктам**: проданные продукты, упорядоченные по количеству активных лицензий</span><span class="sxs-lookup"><span data-stu-id="e71ca-164">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="e71ca-165">**Число активных лицензий по клиентам**: количество клиентов, отсортированных по активному количеству лицензий</span><span class="sxs-lookup"><span data-stu-id="e71ca-165">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="e71ca-166">**Сведения о событиях клиентской лицензии за последние 90 дней**: подробное представление клиентов, подписок и событий подписки, включая дату события, имя события, количество и изменение количества.</span><span class="sxs-lookup"><span data-stu-id="e71ca-166">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="e71ca-167">Отчет об использовании лицензий:</span><span class="sxs-lookup"><span data-stu-id="e71ca-167">Licenses Usage report:</span></span>

- <span data-ttu-id="e71ca-168">**Назначенные лицензии по продуктам**: проданные продукты, упорядоченные по количеству назначений лицензий</span><span class="sxs-lookup"><span data-stu-id="e71ca-168">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="e71ca-169">**Используемые лицензии по продуктам**: проданные продукты, упорядоченные по количеству используемых лицензий</span><span class="sxs-lookup"><span data-stu-id="e71ca-169">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="e71ca-170">**Распределение назначенных лицензий у клиентов**: распределение общее количества клиентов по сегментам шириной 20 % по назначенным лицензиям</span><span class="sxs-lookup"><span data-stu-id="e71ca-170">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="e71ca-171">**Распределение используемых лицензий у клиентов**: распределение общее количества клиентов по сегментам шириной 20 % по используемым лицензиям</span><span class="sxs-lookup"><span data-stu-id="e71ca-171">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="e71ca-172">**Назначенные лицензии по клиентам**: подробное представление проданных и назначенных лицензий по клиентам и продуктам</span><span class="sxs-lookup"><span data-stu-id="e71ca-172">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="e71ca-173">**Используемые лицензии по клиентам**: подробное представление проданных и используемых лицензий по клиентам и продуктам</span><span class="sxs-lookup"><span data-stu-id="e71ca-173">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="e71ca-174">Аналитический отчет по Azure:</span><span class="sxs-lookup"><span data-stu-id="e71ca-174">Azure Insights report:</span></span>

- <span data-ttu-id="e71ca-175">**Клиенты на основе использования за последние 12 месяцев**: тенденция "месячный месяц" новых клиентов на основе использования и обработанных клиентов на основе использования, собранных ежемесячно за период за последние 12 месяцев.</span><span class="sxs-lookup"><span data-stu-id="e71ca-175">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e71ca-176">**Подписки на основе использования за последние 12 месяцев**: тенденция "месячный за месяц" новых подписок на основе использования и обработанных подписок на основе использования, агрегированных ежемесячно за период за последние 12 месяцев.</span><span class="sxs-lookup"><span data-stu-id="e71ca-176">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e71ca-177">**Оценочная стоимость использования клиентом за последние 60 дней**: клиенты на основе использования, отсортированные по предполагаемой сумме НДС с предварительной налоговой накладной за период за последние 60 дней.</span><span class="sxs-lookup"><span data-stu-id="e71ca-177">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="e71ca-178">Это состояние указывает, что клиенты на основе использования получают наибольший доход</span><span class="sxs-lookup"><span data-stu-id="e71ca-178">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="e71ca-179">**Оценочная стоимость использования по категориям за последние 60 дней**: категории счетчиков подписок на основе использования, отсортированные по предполагаемой сумме НДС с предварительной налоговой накладной за период за последние 60 дней.</span><span class="sxs-lookup"><span data-stu-id="e71ca-179">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="e71ca-180">**Оценочная стоимость использования по подписке за последние 60 дней**: подписки на основе использования путем оценки суммы в рублях по предварительным счетам, агрегированные за период за последние 60 дней.</span><span class="sxs-lookup"><span data-stu-id="e71ca-180">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="e71ca-181">**Предполагаемые расходы клиентов на использование по расходному бюджету**: клиенты, упорядоченные по проценту текущего использования расходного бюджета с превышением порога (100 %).</span><span class="sxs-lookup"><span data-stu-id="e71ca-181">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="e71ca-182">Отчет об использовании ресурсов Azure:</span><span class="sxs-lookup"><span data-stu-id="e71ca-182">Azure Resource Usage report:</span></span>

- <span data-ttu-id="e71ca-183">**Использование ресурсов Azure по дням за выбранный период**: ежедневные единицы потребления для каждого отслеживаемого ресурса в каждой подписке на основе использования для выбранного периода за последние 60 дней.</span><span class="sxs-lookup"><span data-stu-id="e71ca-183">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="e71ca-184">**Оценочная стоимость использования ресурсов Azure за выбранный период**: Оценочная стоимость на основе последней тарифной карты для каждого отслеживаемого ресурса в каждой подписке на основе использования в течение последних 60 дней.</span><span class="sxs-lookup"><span data-stu-id="e71ca-184">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e71ca-185">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="e71ca-185">Next steps</span></span>

- [<span data-ttu-id="e71ca-186">Обзор приложения "Аналитика Центра партнеров для Power BI"</span><span class="sxs-lookup"><span data-stu-id="e71ca-186">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="e71ca-187">Установка приложения "Аналитика Центра партнеров для Microsoft Power BI" и ознакомление с ним</span><span class="sxs-lookup"><span data-stu-id="e71ca-187">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
