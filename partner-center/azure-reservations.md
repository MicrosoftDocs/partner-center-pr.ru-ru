---
title: Продажа клиентов Microsoft Azure резервирования
description: Как поставщик облачных решений вы можете покупать и продавать резервирования Azure для клиентов, а также управлять ими. Используйте центр партнеров, портал Azure или API центра партнеров.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534902"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="ad54f-104">Продавайте Microsoft Azure резервирования клиентам с помощью центра партнеров, портал Azure или интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="ad54f-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="ad54f-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="ad54f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ad54f-106">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="ad54f-106">Admin agent</span></span>
- <span data-ttu-id="ad54f-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ad54f-107">Global admin</span></span>
- <span data-ttu-id="ad54f-108">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="ad54f-108">Helpdesk agent</span></span>
- <span data-ttu-id="ad54f-109">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="ad54f-109">Sales agent</span></span>
- <span data-ttu-id="ad54f-110">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="ad54f-110">User management admin</span></span>

<span data-ttu-id="ad54f-111">В качестве партнера в программе поставщика облачных решений (CSP) вы можете приобрести, продать или управлять резервированием Azure для клиентов.</span><span class="sxs-lookup"><span data-stu-id="ad54f-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="ad54f-112">Используйте центр партнеров, портал Azure или API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ad54f-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="ad54f-113">Эта статья относится только к партнерам в CSP.</span><span class="sxs-lookup"><span data-stu-id="ad54f-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="ad54f-114">Вместо этого клиенты, использующие другие типы подписок (например, оплата по мере использования, индивидуальные соглашения с клиентами Майкрософт или подписки Соглашение Enterprise), должны читать [эту документацию по резервированию Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="ad54f-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="ad54f-115">Партнеры в программе CSP могут предложить своим клиентам Microsoft Azure резервирования.</span><span class="sxs-lookup"><span data-stu-id="ad54f-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="ad54f-116">Клиенты могут получить значительную экономию при предварительном резервировании.</span><span class="sxs-lookup"><span data-stu-id="ad54f-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="ad54f-117">Резервирование Azure предоставляет клиентам простоту и гибкость следующим образом:</span><span class="sxs-lookup"><span data-stu-id="ad54f-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="ad54f-118">Резервирование на один год или три года</span><span class="sxs-lookup"><span data-stu-id="ad54f-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="ad54f-119">Легко приступить к работе; установка занимает считаные секунды</span><span class="sxs-lookup"><span data-stu-id="ad54f-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="ad54f-120">Возможность отменить резервирование или заменить зарезервированные экземпляры в любое время с корректировкой оплаты и возмещением средств</span><span class="sxs-lookup"><span data-stu-id="ad54f-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="ad54f-121">Управление использованием зарезервированных экземпляров на уровне организации или отдельного подразделения</span><span class="sxs-lookup"><span data-stu-id="ad54f-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="ad54f-122">Резервирование Azure может попривлекательно клиентам следующими способами:</span><span class="sxs-lookup"><span data-stu-id="ad54f-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="ad54f-123">Резервирования могут обеспечить значительную экономию по цене оплаты по мере использования (PAYG).</span><span class="sxs-lookup"><span data-stu-id="ad54f-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="ad54f-124">Более точное планирование и прогнозирование бюджета с предоплатой за год или три года</span><span class="sxs-lookup"><span data-stu-id="ad54f-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="ad54f-125">Приоритетное использование вычислительной мощности в регионе Azure, ближайшем к офисам организации</span><span class="sxs-lookup"><span data-stu-id="ad54f-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="ad54f-126">Резервирование Azure предоставляет основу для комплексных решений инфраструктуры в сочетании с программным обеспечением, например Microsoft Windows Server и базой данных SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="ad54f-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="ad54f-127">Вы можете покупать, продавать и управлять резервированием Azure в центре партнеров и портал Azure, а также с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ad54f-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="ad54f-128">Вы также можете предоставить своим клиентам разрешение на приобретение собственных резервирований Azure из подписки Azure, которую вы приобрели для них.</span><span class="sxs-lookup"><span data-stu-id="ad54f-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="ad54f-129">Чтобы узнать, как это сделать, перейдите по ссылкам ниже.</span><span class="sxs-lookup"><span data-stu-id="ad54f-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="ad54f-130">Ресурсы о резервированиях Azure</span><span class="sxs-lookup"><span data-stu-id="ad54f-130">Azure reservations resources</span></span>

|<span data-ttu-id="ad54f-131">**Сведения о**</span><span class="sxs-lookup"><span data-stu-id="ad54f-131">**For information about**</span></span>   |<span data-ttu-id="ad54f-132">**Прочитайте это**</span><span class="sxs-lookup"><span data-stu-id="ad54f-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="ad54f-133">Документация по резервированию Azure для ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="ad54f-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="ad54f-134">Что такое резервирования Azure?</span><span class="sxs-lookup"><span data-stu-id="ad54f-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="ad54f-135">Приобретение резервирований Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ad54f-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="ad54f-136">Приобретение резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="ad54f-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="ad54f-137">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ad54f-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="ad54f-138">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ad54f-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="ad54f-139">Определение правильного размера виртуальной машины и проверка использования виртуальной машины клиента</span><span class="sxs-lookup"><span data-stu-id="ad54f-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="ad54f-140">Размеры виртуальных машин для максимального использования резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="ad54f-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="ad54f-141">Приобретение резервирований Azure с помощью API Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="ad54f-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="ad54f-142">[Приобретение услуги Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ad54f-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="ad54f-143">Предоставление клиентам разрешения на приобретение собственных резервирований Azure из подписки CSP.</span><span class="sxs-lookup"><span data-stu-id="ad54f-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="ad54f-144">Предоставление клиентам разрешения на приобретение собственных резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="ad54f-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |