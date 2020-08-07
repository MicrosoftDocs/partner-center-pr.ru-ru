---
title: Продажа клиентов Microsoft Azure резервирования
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Как поставщик облачных решений вы можете покупать и продавать резервирования Azure для клиентов, а также управлять ими. Используйте центр партнеров, портал Azure или API центра партнеров.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3efe8ae6a955dee5cfe01d0571cd107f8ee50f5c
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900087"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="89516-104">Продавайте Microsoft Azure резервирования клиентам с помощью центра партнеров, портал Azure или интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="89516-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="89516-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="89516-105">**Applies to**</span></span>

- <span data-ttu-id="89516-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="89516-106">Partner Center</span></span>
- <span data-ttu-id="89516-107">Портал Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="89516-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="89516-108">Партнеры в программе CSP</span><span class="sxs-lookup"><span data-stu-id="89516-108">Partners in the CSP program</span></span>

<span data-ttu-id="89516-109">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="89516-109">**Appropriate roles**</span></span>

- <span data-ttu-id="89516-110">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="89516-110">Admin agent</span></span>
- <span data-ttu-id="89516-111">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="89516-111">Global admin</span></span>
- <span data-ttu-id="89516-112">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="89516-112">Helpdesk agent</span></span>
- <span data-ttu-id="89516-113">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="89516-113">Sales agent</span></span>
- <span data-ttu-id="89516-114">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="89516-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="89516-115">Эта статья относится только к партнерам в программе поставщика облачных решений (CSP).</span><span class="sxs-lookup"><span data-stu-id="89516-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="89516-116">Вместо этого клиенты, использующие другие типы подписок (например, оплата по мере использования, индивидуальные соглашения с клиентами Майкрософт или подписки Соглашение Enterprise), должны читать [эту документацию по резервированию Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="89516-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="89516-117">Партнеры в программе CSP могут предложить своим клиентам Microsoft Azure резервирования.</span><span class="sxs-lookup"><span data-stu-id="89516-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="89516-118">Клиенты могут получить значительную экономию при предварительном резервировании.</span><span class="sxs-lookup"><span data-stu-id="89516-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="89516-119">Резервирование Azure предоставляет клиентам простоту и гибкость следующим образом:</span><span class="sxs-lookup"><span data-stu-id="89516-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="89516-120">Резервирование на один год или три года</span><span class="sxs-lookup"><span data-stu-id="89516-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="89516-121">Легко приступить к работе; установка занимает считаные секунды</span><span class="sxs-lookup"><span data-stu-id="89516-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="89516-122">Возможность отменить резервирование или заменить зарезервированные экземпляры в любое время с корректировкой оплаты и возмещением средств</span><span class="sxs-lookup"><span data-stu-id="89516-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="89516-123">Управление использованием зарезервированных экземпляров на уровне организации или отдельного подразделения</span><span class="sxs-lookup"><span data-stu-id="89516-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="89516-124">Резервирование Azure может попривлекательно клиентам следующими способами:</span><span class="sxs-lookup"><span data-stu-id="89516-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="89516-125">Резервирования могут обеспечить значительную экономию по цене оплаты по мере использования (PAYG).</span><span class="sxs-lookup"><span data-stu-id="89516-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="89516-126">Более точное планирование и прогнозирование бюджета с предоплатой за год или три года</span><span class="sxs-lookup"><span data-stu-id="89516-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="89516-127">Приоритетное использование вычислительной мощности в регионе Azure, ближайшем к офисам организации</span><span class="sxs-lookup"><span data-stu-id="89516-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="89516-128">Резервирование Azure предоставляет основу для комплексных решений инфраструктуры в сочетании с программным обеспечением, например Microsoft Windows Server и базой данных SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="89516-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="89516-129">Вы можете покупать, продавать и управлять резервированием Azure в центре партнеров и портал Azure, а также с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="89516-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="89516-130">Вы также можете предоставить своим клиентам разрешение на приобретение собственных резервирований Azure из подписки Azure, которую вы приобрели для них.</span><span class="sxs-lookup"><span data-stu-id="89516-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="89516-131">Чтобы узнать, как это сделать, перейдите по ссылкам ниже.</span><span class="sxs-lookup"><span data-stu-id="89516-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="89516-132">Ресурсы о резервированиях Azure</span><span class="sxs-lookup"><span data-stu-id="89516-132">Azure reservations resources</span></span>

|<span data-ttu-id="89516-133">**Сведения о**</span><span class="sxs-lookup"><span data-stu-id="89516-133">**For information about**</span></span>   |<span data-ttu-id="89516-134">**Прочитайте это**</span><span class="sxs-lookup"><span data-stu-id="89516-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="89516-135">Документация по резервированию Azure для ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="89516-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="89516-136">Что такое резервирования Azure?</span><span class="sxs-lookup"><span data-stu-id="89516-136">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="89516-137">Приобретение резервирований Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="89516-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="89516-138">Приобретение резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="89516-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="89516-139">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="89516-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="89516-140">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="89516-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="89516-141">Определение правильного размера виртуальной машины и проверка использования виртуальной машины клиента</span><span class="sxs-lookup"><span data-stu-id="89516-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="89516-142">Размеры виртуальных машин для максимального использования резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="89516-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="89516-143">Приобретение резервирований Azure с помощью API Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="89516-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="89516-144">[Приобретение услуги Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="89516-144">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="89516-145">Предоставление клиентам разрешения на приобретение собственных резервирований Azure из подписки CSP.</span><span class="sxs-lookup"><span data-stu-id="89516-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="89516-146">Предоставление клиентам разрешения на приобретение собственных резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="89516-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
