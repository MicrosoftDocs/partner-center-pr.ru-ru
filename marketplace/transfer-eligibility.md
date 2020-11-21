---
title: Права на передачу — рекомендации по передаче подписки между учетными записями выставления счетов, Azure Marketplace
description: Рекомендации по коммерческой проверке перед передачей подписки между учетными записями выставления счетов в портал Azure.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007349"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="271ef-103">Права на перемещение для подписки между учетными записями выставления счетов</span><span class="sxs-lookup"><span data-stu-id="271ef-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="271ef-104">Подписку можно [переместить](/azure/cost-management-billing/understand/subscription-transfer) из одной учетной записи выставления счетов в другую в разделе выставления счетов портал Azure.</span><span class="sxs-lookup"><span data-stu-id="271ef-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="271ef-105">Перед переносом подписка проверяется на наличие продуктов сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="271ef-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="271ef-106">Перемещение разрешено только в том случае, если *все* продукты удалены для перемещения (см. [критерии](#criteria-for-transfer-approval-or-denial) ниже).</span><span class="sxs-lookup"><span data-stu-id="271ef-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="271ef-107">Система создаст соответствующие сообщения об ошибках для приложений, которые не удалось очистить, чтобы помочь вам определить дальнейшие действия.</span><span class="sxs-lookup"><span data-stu-id="271ef-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="271ef-108">Эта статья не относится к предложениям SaaS, так как ресурсы SaaS присоединены к клиенту, а не к подписке.</span><span class="sxs-lookup"><span data-stu-id="271ef-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="271ef-109">Ресурсы SaaS передаются из одной учетной записи выставления счетов в другую, но это делается для каждого ресурса, а служба поддержки Azure — как запрос на поддержку.</span><span class="sxs-lookup"><span data-stu-id="271ef-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="271ef-110">Критерии для утверждения или отказа в переносе</span><span class="sxs-lookup"><span data-stu-id="271ef-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="271ef-111">Нельзя переместить подписку, если любое из сторонних приложений соответствует одному из следующих критериев:</span><span class="sxs-lookup"><span data-stu-id="271ef-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="271ef-112">Целевая учетная запись является коммерческой, а приложение — для продажи через партнеров.</span><span class="sxs-lookup"><span data-stu-id="271ef-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="271ef-113">Приложение является явным согласием для выбранных участников, а Целевая учетная запись отсутствует в списке разрешений.</span><span class="sxs-lookup"><span data-stu-id="271ef-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="271ef-114">Предложение было предварительным предложением в прошлом для выбранных подписок или было частным предложением, а подписка больше не находится в списке разрешений.</span><span class="sxs-lookup"><span data-stu-id="271ef-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="271ef-115">Новая учетная запись выставления счетов находится в регионе, отличном от того, где было продано предложение, и предложение не будет продаваться в этом регионе.</span><span class="sxs-lookup"><span data-stu-id="271ef-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="271ef-116">Заблокированное перемещение действует до тех пор, пока ресурс не будет удален из подписки, после чего вы сможете повторить попытку перемещения.</span><span class="sxs-lookup"><span data-stu-id="271ef-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="271ef-117">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="271ef-117">Next steps</span></span>

[<span data-ttu-id="271ef-118">Получение поддержки для Microsoft AppSource и Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="271ef-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

