---
title: Продажа клиентов Microsoft Azure резервирования
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Как поставщик облачных решений вы можете покупать и продавать резервирования Azure для клиентов, а также управлять ими. Используйте центр партнеров, портал Azure или API центра партнеров.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4524d810a036953e45fb94a72241734e02a2798f
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435733"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="8a1b9-104">Продавайте Microsoft Azure резервирования клиентам с помощью центра партнеров, портал Azure или интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="8a1b9-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="8a1b9-105">**Applies to**</span></span>

- <span data-ttu-id="8a1b9-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="8a1b9-106">Partner Center</span></span>
- <span data-ttu-id="8a1b9-107">Портал Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="8a1b9-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="8a1b9-108">Партнеры по программе CSP</span><span class="sxs-lookup"><span data-stu-id="8a1b9-108">Partners in CSP</span></span>

<span data-ttu-id="8a1b9-109">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="8a1b9-109">**Appropriate roles**</span></span>

- <span data-ttu-id="8a1b9-110">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="8a1b9-110">Admin agent</span></span>
- <span data-ttu-id="8a1b9-111">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8a1b9-111">Global admin</span></span>
- <span data-ttu-id="8a1b9-112">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="8a1b9-112">Helpdesk agent</span></span>
- <span data-ttu-id="8a1b9-113">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="8a1b9-113">Sales agent</span></span>
- <span data-ttu-id="8a1b9-114">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="8a1b9-114">User management admin</span></span>

<span data-ttu-id="8a1b9-115">Партнеры в программе поставщика облачных решений (CSP) могут предложить своим клиентам Microsoft Azure резервирования.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-115">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="8a1b9-116">Клиенты могут получить значительную экономию при предварительном резервировании.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="8a1b9-117">Резервирование Azure предоставляет клиентам простоту и гибкость следующим образом:</span><span class="sxs-lookup"><span data-stu-id="8a1b9-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="8a1b9-118">Резервирование на один год или три года</span><span class="sxs-lookup"><span data-stu-id="8a1b9-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="8a1b9-119">Легко приступить к работе; установка занимает считаные секунды</span><span class="sxs-lookup"><span data-stu-id="8a1b9-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="8a1b9-120">Возможность отменить резервирование или заменить зарезервированные экземпляры в любое время с корректировкой оплаты и возмещением средств</span><span class="sxs-lookup"><span data-stu-id="8a1b9-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="8a1b9-121">Управление использованием зарезервированных экземпляров на уровне организации или отдельного подразделения</span><span class="sxs-lookup"><span data-stu-id="8a1b9-121">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="8a1b9-122">Резервирование Azure может попривлекательно клиентам следующими способами:</span><span class="sxs-lookup"><span data-stu-id="8a1b9-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="8a1b9-123">Резервирования могут обеспечить значительную экономию по цене оплаты по мере использования (PAYG).</span><span class="sxs-lookup"><span data-stu-id="8a1b9-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="8a1b9-124">Более точное планирование и прогнозирование бюджета с предоплатой за год или три года</span><span class="sxs-lookup"><span data-stu-id="8a1b9-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="8a1b9-125">Приоритетное использование вычислительной мощности в регионе Azure, ближайшем к офисам организации</span><span class="sxs-lookup"><span data-stu-id="8a1b9-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="8a1b9-126">Резервирование Azure предоставляет основу для комплексных решений инфраструктуры в сочетании с программным обеспечением, например Microsoft Windows Server и базой данных SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="8a1b9-127">Вы можете покупать, продавать и управлять резервированием Azure в центре партнеров и портал Azure, а также с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="8a1b9-128">Вы также можете предоставить своим клиентам разрешение на приобретение собственных резервирований Azure из подписки Azure, которую вы приобрели для них.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="8a1b9-129">Чтобы узнать, как это сделать, перейдите по ссылкам ниже.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="8a1b9-130">Ресурсы о резервированиях Azure</span><span class="sxs-lookup"><span data-stu-id="8a1b9-130">Azure reservations resources</span></span>

|<span data-ttu-id="8a1b9-131">**Сведения о**</span><span class="sxs-lookup"><span data-stu-id="8a1b9-131">**For information about**</span></span>   |<span data-ttu-id="8a1b9-132">**Прочитайте это**</span><span class="sxs-lookup"><span data-stu-id="8a1b9-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="8a1b9-133">Документация по резервированию Azure для ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="8a1b9-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="8a1b9-134">Что такое резервирования Azure?</span><span class="sxs-lookup"><span data-stu-id="8a1b9-134">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="8a1b9-135">Приобретение резервирований Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="8a1b9-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="8a1b9-136">Приобретение резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="8a1b9-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="8a1b9-137">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="8a1b9-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="8a1b9-138">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="8a1b9-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="8a1b9-139">Определение правильного размера виртуальной машины и проверка использования виртуальной машины клиента</span><span class="sxs-lookup"><span data-stu-id="8a1b9-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="8a1b9-140">Размеры виртуальных машин для максимального использования резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="8a1b9-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="8a1b9-141">Приобретение резервирований Azure с помощью API Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="8a1b9-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="8a1b9-142">[Приобретение услуги Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="8a1b9-142">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="8a1b9-143">Предоставление клиентам разрешения на приобретение собственных резервирований Azure из подписки CSP.</span><span class="sxs-lookup"><span data-stu-id="8a1b9-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="8a1b9-144">Предоставление клиентам разрешения на приобретение собственных резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="8a1b9-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
