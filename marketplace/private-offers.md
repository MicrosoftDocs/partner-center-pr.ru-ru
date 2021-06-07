---
title: Частные предложения в Azure Marketplace
description: Сведения о частных предложениях в Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534174"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="1c360-103">Частные планы в Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="1c360-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="1c360-104">Частные планы — это то, как издатели предоставляют пользовательские планы конкретным клиентам.</span><span class="sxs-lookup"><span data-stu-id="1c360-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="1c360-105">Частные планы доступны только для платных предложений, которые можно приобрести и напрямую установить из портал Azure.</span><span class="sxs-lookup"><span data-stu-id="1c360-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="1c360-106">Издатели не могут создавать закрытые планы для консультационных услуг, любой службы, которая имеет **Контактное лицо** в качестве вызова действия или любой бесплатной службы, независимо от того, можно ли ее установить с портала.</span><span class="sxs-lookup"><span data-stu-id="1c360-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="1c360-107">Поиск частных планов в портал Azure</span><span class="sxs-lookup"><span data-stu-id="1c360-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="1c360-108">Когда партнер публикует частный план, он отображается только для соответствующих пользователей в разделе **Marketplace** портал Azure.</span><span class="sxs-lookup"><span data-stu-id="1c360-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="1c360-109">Эти пользователи определяются по ИДЕНТИФИКАТОРу подписки или ИДЕНТИФИКАТОРу клиента в зависимости от типа предложения.</span><span class="sxs-lookup"><span data-stu-id="1c360-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="1c360-110">Если вы имеете право на частные планы, то можете найти их на портале двумя способами.</span><span class="sxs-lookup"><span data-stu-id="1c360-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="1c360-111">Частные планы доступны для поиска, но не для фильтрации (по категориям) в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="1c360-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="1c360-112">В портал Azure выберите **+ создать ресурс** или выполните поиск по запросу "Marketplace", чтобы открыть страницу **Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="1c360-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="1c360-113">Если вы имеете право на частные планы, вы увидите баннер с **доступными частными планами** в верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="1c360-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="1c360-114">Выберите **Просмотреть частные предложения и планы** , чтобы перейти на страницу закрытых планов.</span><span class="sxs-lookup"><span data-stu-id="1c360-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Баннер, отображаемый при наличии доступных частных планов.":::

## <a name="review-private-plans"></a><span data-ttu-id="1c360-116">Просмотр частных планов</span><span class="sxs-lookup"><span data-stu-id="1c360-116">Review private plans</span></span>

<span data-ttu-id="1c360-117">Частный план является частью нескольких планов в предложении.</span><span class="sxs-lookup"><span data-stu-id="1c360-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="1c360-118">Каждое предложение может иметь несколько планов, как общедоступных, так и частных, но частные планы отображаются в отдельном списке из общедоступных планов.</span><span class="sxs-lookup"><span data-stu-id="1c360-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="1c360-119">Доступные частные планы можно просмотреть на вкладке **планы** , отмеченные особым **частным** значком:</span><span class="sxs-lookup"><span data-stu-id="1c360-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Страница планов, помеченная как частная.":::

<span data-ttu-id="1c360-121">Если у вас несколько подписок, вы увидите все частные планы, доступные для всех ваших подписок.</span><span class="sxs-lookup"><span data-stu-id="1c360-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="1c360-122">При выборе **создать** вы направляетесь на страницу создания ресурсов, чтобы начать настройку ресурса.</span><span class="sxs-lookup"><span data-stu-id="1c360-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="1c360-123">Если выбрать **создать** и иметь несколько подписок, но не все из них будут добавлены к частному плану, ваша подписка по умолчанию может быть не подписке, подходящей для этого частного плана.</span><span class="sxs-lookup"><span data-stu-id="1c360-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="1c360-124">В этом случае выберите правильную подписку.</span><span class="sxs-lookup"><span data-stu-id="1c360-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Ссылка, показывающая, доступны дополнительные частные планы.":::

## <a name="next-steps"></a><span data-ttu-id="1c360-126">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1c360-126">Next steps</span></span>

- [<span data-ttu-id="1c360-127">Что такое Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="1c360-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
