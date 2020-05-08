---
title: Продажа клиентов Microsoft Azure резервирования
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Как поставщик облачных решений вы можете покупать и продавать резервирования Azure для клиентов, а также управлять ими. Используйте центр партнеров, портал Azure или API центра партнеров.
author: LauraBrenner
ms.author: labrenne
keywords: azure, резервирования, управление, выставление счетов, приобретение, Azure RI, Azure Reserved Instances
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19c156f0b47ccb39bc678cdd2ae9cce9db5c5ebd
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908288"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="4eb0e-105">Продавайте Microsoft Azure резервирования клиентам с помощью центра партнеров, портал Azure или интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<!--Maggie, 12/7/18 - Added "Partner Center" to metadata title and H1 title as per Catherine Watson in bug #19868631-->

<span data-ttu-id="4eb0e-106">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="4eb0e-106">**Applies to**</span></span>

- <span data-ttu-id="4eb0e-107">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="4eb0e-107">Partner Center</span></span>
- <span data-ttu-id="4eb0e-108">Портал Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="4eb0e-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="4eb0e-109">Партнеры по программе CSP</span><span class="sxs-lookup"><span data-stu-id="4eb0e-109">Partners in CSP</span></span>

<span data-ttu-id="4eb0e-110">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="4eb0e-110">**Appropriate roles**</span></span>

- <span data-ttu-id="4eb0e-111">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="4eb0e-111">Admin agent</span></span>
- <span data-ttu-id="4eb0e-112">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4eb0e-112">Global admin</span></span>
- <span data-ttu-id="4eb0e-113">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="4eb0e-113">Helpdesk agent</span></span>
- <span data-ttu-id="4eb0e-114">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="4eb0e-114">Sales agent</span></span>
- <span data-ttu-id="4eb0e-115">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="4eb0e-115">User management admin</span></span>

<span data-ttu-id="4eb0e-116">Партнеры в программе поставщика облачных решений (CSP) могут предложить своим клиентам Microsoft Azure резервирования.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="4eb0e-117">Клиенты могут получить значительную экономию при предварительном резервировании.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="4eb0e-118">Резервирование Azure предоставляет клиентам простоту и гибкость следующим образом:</span><span class="sxs-lookup"><span data-stu-id="4eb0e-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="4eb0e-119">Резервирование на один год или три года</span><span class="sxs-lookup"><span data-stu-id="4eb0e-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="4eb0e-120">Легко приступить к работе; установка занимает считаные секунды</span><span class="sxs-lookup"><span data-stu-id="4eb0e-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="4eb0e-121">Возможность отменить резервирование или заменить зарезервированные экземпляры в любое время с корректировкой оплаты и возмещением средств</span><span class="sxs-lookup"><span data-stu-id="4eb0e-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="4eb0e-122">Управление использованием зарезервированных экземпляров на уровне организации или отдельного подразделения</span><span class="sxs-lookup"><span data-stu-id="4eb0e-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="4eb0e-123">Резервирование Azure может попривлекательно клиентам следующими способами:</span><span class="sxs-lookup"><span data-stu-id="4eb0e-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="4eb0e-124">Резервирования могут обеспечить значительную экономию по цене оплаты по мере использования (PAYG).</span><span class="sxs-lookup"><span data-stu-id="4eb0e-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="4eb0e-125">Более точное планирование и прогнозирование бюджета с предоплатой за год или три года</span><span class="sxs-lookup"><span data-stu-id="4eb0e-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="4eb0e-126">Приоритетное использование вычислительной мощности в регионе Azure, ближайшем к офисам организации</span><span class="sxs-lookup"><span data-stu-id="4eb0e-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="4eb0e-127">Резервирование Azure предоставляет основу для комплексных решений инфраструктуры в сочетании с программным обеспечением, например Microsoft Windows Server и базой данных SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="4eb0e-128">Вы можете покупать, продавать и управлять резервированием Azure в центре партнеров и портал Azure, а также с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="4eb0e-129">Вы также можете предоставить своим клиентам разрешение на приобретение собственных резервирований Azure из подписки Azure, которую вы приобрели для них.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="4eb0e-130">Чтобы узнать, как это сделать, перейдите по ссылкам ниже.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="4eb0e-131">Ресурсы о резервированиях Azure</span><span class="sxs-lookup"><span data-stu-id="4eb0e-131">Azure reservations resources</span></span>

|<span data-ttu-id="4eb0e-132">**Сведения о**</span><span class="sxs-lookup"><span data-stu-id="4eb0e-132">**For information about**</span></span>   |<span data-ttu-id="4eb0e-133">**Прочитайте это**</span><span class="sxs-lookup"><span data-stu-id="4eb0e-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="4eb0e-134">Документация по резервированию Azure для ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="4eb0e-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="4eb0e-135">Основные сведения о резервировании в Azure</span><span class="sxs-lookup"><span data-stu-id="4eb0e-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="4eb0e-136">Приобретение резервирований Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="4eb0e-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="4eb0e-137">Приобретение резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="4eb0e-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="4eb0e-138">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="4eb0e-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="4eb0e-139">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="4eb0e-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="4eb0e-140">Определение правильного размера виртуальной машины и проверка использования виртуальной машины клиента</span><span class="sxs-lookup"><span data-stu-id="4eb0e-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="4eb0e-141">Размеры виртуальных машин для максимального использования резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="4eb0e-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="4eb0e-142">Приобретение резервирований Azure с помощью API Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="4eb0e-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="4eb0e-143">[Приобретение услуги Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="4eb0e-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="4eb0e-144">Предоставление клиентам разрешения на приобретение собственных резервирований Azure из подписки CSP.</span><span class="sxs-lookup"><span data-stu-id="4eb0e-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="4eb0e-145">Предоставление клиентам разрешения на приобретение собственных резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="4eb0e-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
