---
title: Как рассчитывается полученный кредит от партнера | Центр партнеров
ms.topic: article
ms.date: 09/17/2019
description: Как рассчитывается процент полученного кредита плана Azure
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: eb0dd5ef22632a85ca0227cc9e988a88263e9ddf
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318769"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="0f5e0-103">Как вычисляется кредитоспособный кредит (PEC) партнера</span><span class="sxs-lookup"><span data-stu-id="0f5e0-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="0f5e0-104">Партнеры, владеющие Круглосуточная эксплуатацией ИТ или всей среды Azure своих клиентов в CSP, получают с помощью PEC.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="0f5e0-105">PEC предоставляется в качестве части счета партнеру, имеющему прямую связь с корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="0f5e0-106">Кредит вычисляется ежедневно и отражается в месячном счете.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="0f5e0-107">По умолчанию в CSP партнерам предоставляются необходимые права доступа к подписке клиента, позволяющие круглосуточно управлять ресурсами в подписке и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-107">By default, in CSP, partners are granted the necessary access rights to the customer’s subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="0f5e0-108">Дополнительные способы, с помощью которых клиент может подготавливать доступ для передействующего партнера, описаны в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="0f5e0-109">Важные требования к допустимости и вычислениям:</span><span class="sxs-lookup"><span data-stu-id="0f5e0-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="0f5e0-110">У партнера должно быть активное соглашение MPN и действующая роль с учетной записью C (RBAC) на основе правил для получения заработанного кредита для ресурсов Azure, которыми они управляют.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="0f5e0-111">Дополнительные сведения [допустимые роли RBAC]</span><span class="sxs-lookup"><span data-stu-id="0f5e0-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="0f5e0-112">Косвенный поставщик будет иметь право на PEC, если они или их непрямое торговые посредники, или оба имеют Круглосуточная оперативный контроль и управление ресурсами Azure клиента в CSP.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer’s Azure resources in CSP.</span></span>

- <span data-ttu-id="0f5e0-113">PEC связан с выставленным счетом за использование клиентской стороны Azure в CSP, управляемом партнером.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-113">PEC is associated to billed (chargeable) consumption of customer’s Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="0f5e0-114">PEC доступен только партнерам в CSP, за которые взимается плата Майкрософт (косвенный поставщик и прямой счет).</span><span class="sxs-lookup"><span data-stu-id="0f5e0-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="0f5e0-115">Подходящие службы: заработанный кредитный курс применяется ко всем ресурсам Azure 1PP Azure, указанным в прайс-списке.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="0f5e0-116">Существуют исключения, включая, но не ограниченные, 3PP и резервирование Azure.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="0f5e0-117">PEC вычисляется ежедневно и может быть просмотрен в ежедневном разведывательную файле.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="0f5e0-118">Партнер (поставщик или торговый посредник (через поставщика услуг) должен иметь доступ ко всему дню (круглосуточно), чтобы гарантировать получение PEC.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="0f5e0-119">PEC задается на уровне ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="0f5e0-120">Если у партнера есть допустимый доступ в подписке или на уровне группы ресурсов, каждый ресурс, который имеет роль до более высокой сущности, будет получать PEC.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="0f5e0-121">PEC будет включен в ежемесячный счет партнера.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="0f5e0-122">В счете указана чистая оплата.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-122">The invoice is net of charges.</span></span> <span data-ttu-id="0f5e0-123">Сведения отображаются в файле счета разведывательную.</span><span class="sxs-lookup"><span data-stu-id="0f5e0-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="0f5e0-124">Сведения о получении доступа к управлению подписками Azure и о том, как связать идентификатор MPN с ролями RBAC, см. в статье [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="0f5e0-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="0f5e0-125">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="0f5e0-125">For more information</span></span>

- [<span data-ttu-id="0f5e0-126">План Azure — выставление счетов</span><span class="sxs-lookup"><span data-stu-id="0f5e0-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="0f5e0-127">Прейскурант для нового коммерческого опыта в CSP</span><span class="sxs-lookup"><span data-stu-id="0f5e0-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)