---
title: Частные предложения в Azure Marketplace
description: Сведения о частных предложениях в Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 055151f0420d642d591554a829dc21b69df84ebd
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007388"
---
# <a name="private-offers-in-azure-marketplace"></a><span data-ttu-id="f7267-103">Частные предложения в Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f7267-103">Private offers in Azure Marketplace</span></span>

<span data-ttu-id="f7267-104">Частные предложения — это то, как издатели предоставляют пользовательские планы конкретным клиентам.</span><span class="sxs-lookup"><span data-stu-id="f7267-104">Private offers are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="f7267-105">Сейчас этот параметр поддерживается только в Azure Marketplace в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="f7267-105">This option is currently supported only in the Azure Marketplace experience in the Azure portal.</span></span> <span data-ttu-id="f7267-106">Частные предложения доступны только для платных предложений, которые можно приобрести и напрямую установить из портал Azure.</span><span class="sxs-lookup"><span data-stu-id="f7267-106">Private offers are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="f7267-107">Издатель не может создавать частные предложения для консультационных услуг, любой службы, имеющей **Контактное лицо** в качестве вызова действия или любой бесплатной службы, независимо от того, можно ли ее установить с портала.</span><span class="sxs-lookup"><span data-stu-id="f7267-107">Publisher cannot create private offers for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-offers-in-the-azure-portal"></a><span data-ttu-id="f7267-108">Поиск частных предложений в портал Azure</span><span class="sxs-lookup"><span data-stu-id="f7267-108">Find private offers in the Azure portal</span></span>

<span data-ttu-id="f7267-109">Когда партнер публикует Частное предложение, он отображается только для соответствующих пользователей в разделе **Marketplace** портал Azure.</span><span class="sxs-lookup"><span data-stu-id="f7267-109">When a partner publishes a private offer, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="f7267-110">Эти пользователи определяются по ИДЕНТИФИКАТОРу подписки или ИДЕНТИФИКАТОРу клиента в зависимости от типа предложения.</span><span class="sxs-lookup"><span data-stu-id="f7267-110">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="f7267-111">Если вы имеете право на закрытые предложения, существует два способа их поиска на портале.</span><span class="sxs-lookup"><span data-stu-id="f7267-111">If you are eligible for  private offers, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="f7267-112">Частные предложения сейчас недоступны для поиска или фильтрации (по категориям) в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="f7267-112">Private offers are currently not searchable or filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="f7267-113">В портал Azure выберите **+ создать ресурс** или выполните поиск по запросу "Marketplace", чтобы открыть страницу **Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="f7267-113">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="f7267-114">Если вы имеете право на частные предложения, вы увидите баннер с **личными предложениями** в верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="f7267-114">If you are eligible for private offers, you will see the **You have private offers available** banner on the top of the page.</span></span> <span data-ttu-id="f7267-115">Выберите **Просмотр частных предложений** , чтобы перейти на страницу закрытых предложений.</span><span class="sxs-lookup"><span data-stu-id="f7267-115">Select **View private offers** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Баннер, отображаемый при наличии доступных частных предложений.":::

<span data-ttu-id="f7267-117">Кроме того, если отображается баннер закрытые предложения, можно также перейти к нижней части страницы «коллекция продуктов», и вы увидите подмножество частных предложений.</span><span class="sxs-lookup"><span data-stu-id="f7267-117">Alternately, if you see the private offers banner, you can also scroll to the bottom of the product gallery page and you will see a subset of your private offers.</span></span> <span data-ttu-id="f7267-118">Щелкните ссылку, чтобы **Просмотреть дополнительные сведения** для перехода на вашу частную страницу предложений.</span><span class="sxs-lookup"><span data-stu-id="f7267-118">Select the link to **See More** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="Показывает частные предложения в нижней части экрана, а также ссылку Показать дополнительные.":::

## <a name="review-private-plans"></a><span data-ttu-id="f7267-120">Просмотр частных планов</span><span class="sxs-lookup"><span data-stu-id="f7267-120">Review private plans</span></span>

<span data-ttu-id="f7267-121">Частное предложение фактически является частным планом в рамках предложения.</span><span class="sxs-lookup"><span data-stu-id="f7267-121">A private offer is actually a private plan within an offer.</span></span> <span data-ttu-id="f7267-122">Каждое предложение может иметь несколько планов, как общедоступных, так и частных, но частные планы отображаются в отдельном списке из общедоступных планов.</span><span class="sxs-lookup"><span data-stu-id="f7267-122">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="f7267-123">Доступные частные планы можно просмотреть на вкладке **планы** , отмеченные особым **частным** значком:</span><span class="sxs-lookup"><span data-stu-id="f7267-123">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Страница планов, помеченная как частная.":::

<span data-ttu-id="f7267-125">Если у вас несколько подписок, вы увидите все частные предложения, доступные для всех ваших подписок.</span><span class="sxs-lookup"><span data-stu-id="f7267-125">If you have more than one subscription, you will see all private offers available for all your subscriptions.</span></span> <span data-ttu-id="f7267-126">При выборе **создать** вы направляетесь на страницу создания ресурсов, чтобы начать настройку ресурса.</span><span class="sxs-lookup"><span data-stu-id="f7267-126">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="f7267-127">Если вы выбрали **создать** и иметь несколько подписок, но не все из них добавлены в частный план, ваша подписка по умолчанию может быть не подписке, подходящей для этого частного предложения.</span><span class="sxs-lookup"><span data-stu-id="f7267-127">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private offer.</span></span> <span data-ttu-id="f7267-128">В этом случае выберите правильную подписку.</span><span class="sxs-lookup"><span data-stu-id="f7267-128">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Ссылка, указывающая на наличие более частных предложений, доступна.":::

## <a name="next-steps"></a><span data-ttu-id="f7267-130">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f7267-130">Next steps</span></span>

- [<span data-ttu-id="f7267-131">Что такое Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="f7267-131">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
