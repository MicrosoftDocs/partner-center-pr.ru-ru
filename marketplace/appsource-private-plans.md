---
title: Частные планы в Microsoft AppSource
description: Настройка частных планов в Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008550"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="90df9-103">Частные планы в Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="90df9-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="90df9-104">Частные планы — это то, как издатели предоставляют пользовательские планы конкретным клиентам.</span><span class="sxs-lookup"><span data-stu-id="90df9-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="90df9-105">Этот параметр теперь доступен в Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="90df9-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="90df9-106">Частные планы могут продаваться на AppSource для программного обеспечения как услуга (SaaS) с предложением **получить** действие.</span><span class="sxs-lookup"><span data-stu-id="90df9-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="90df9-107">Спросите у своего поставщика программного обеспечения о закрытом плане</span><span class="sxs-lookup"><span data-stu-id="90df9-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="90df9-108">Чтобы частный план был доступен вам в AppSource, необходимо обратиться непосредственно к независимому поставщику программного обеспечения и согласовать пользовательскую цену и технические спецификации.</span><span class="sxs-lookup"><span data-stu-id="90df9-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="90df9-109">После согласования условий частного плана независимый поставщик программного обеспечения создаст план и присвоит его ИДЕНТИФИКАТОРу клиента вашей организации, который вам потребуется предоставить.</span><span class="sxs-lookup"><span data-stu-id="90df9-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="90df9-110">Поиск идентификатора клиента</span><span class="sxs-lookup"><span data-stu-id="90df9-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="90df9-111">В AppSource в правом верхнем углу щелкните значок профиля учетной записи и **Просмотрите клиент**.</span><span class="sxs-lookup"><span data-stu-id="90df9-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="90df9-112">Скопируйте идентификатор клиента и предоставьте его поставщику программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="90df9-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Показывает, как найти идентификатор клиента.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="90df9-114">Поиск частного плана в AppSource</span><span class="sxs-lookup"><span data-stu-id="90df9-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="90df9-115">После того, как поставщик программного обеспечения опубликует новый частный план, он может пройти до 48 часов, прежде чем увидеть его в AppSource.</span><span class="sxs-lookup"><span data-stu-id="90df9-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="90df9-116">Чтобы найти частные планы, связанные с ИДЕНТИФИКАТОРом клиента, выберите **частные планы** (значок замка) в правом верхнем углу AppSource.</span><span class="sxs-lookup"><span data-stu-id="90df9-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Отображение значка замка на верхней панели инструментов.":::

<span data-ttu-id="90df9-118">Если вы не вошли в системе, появится сообщение с запросом.</span><span class="sxs-lookup"><span data-stu-id="90df9-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="90df9-119">Затем можно приобрести частные планы, связанные с ИДЕНТИФИКАТОРом клиента, на вкладке **планы + цены** .</span><span class="sxs-lookup"><span data-stu-id="90df9-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Отображение частных предложений на вкладке план и цены.":::

<span data-ttu-id="90df9-121">Если частные планы недоступны для вашего клиента, в сообщении будет задано, что у вас нет частных планов или предложений.</span><span class="sxs-lookup"><span data-stu-id="90df9-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="90df9-122">Приобретите частный план</span><span class="sxs-lookup"><span data-stu-id="90df9-122">Purchase a private plan</span></span>

<span data-ttu-id="90df9-123">В рамках предложения независимый поставщик программного обеспечения может включать в себя один или несколько частных планов.</span><span class="sxs-lookup"><span data-stu-id="90df9-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="90df9-124">Каждое предложение может иметь как общедоступные, так и частные планы, но частные планы отображаются на отдельной странице со списком предложений, доступ к которой осуществляется из значка закрытых предложений (замка) в правом верхнем углу страницы.</span><span class="sxs-lookup"><span data-stu-id="90df9-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="90df9-125">Доступные частные планы отображаются на вкладке **планы + цены** . Частные планы имеют специальный синий значок.</span><span class="sxs-lookup"><span data-stu-id="90df9-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Отображается синий эмблема частного предложения рядом с частными предложениями.":::

<span data-ttu-id="90df9-127">Чтобы приобрести выбранный план, выберите **получить его сейчас** и следуйте приведенным шагам.</span><span class="sxs-lookup"><span data-stu-id="90df9-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="90df9-128">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="90df9-128">Next steps</span></span>

- [<span data-ttu-id="90df9-129">Что такое Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="90df9-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
