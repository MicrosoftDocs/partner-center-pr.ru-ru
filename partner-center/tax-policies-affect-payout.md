---
title: Влияние налоговых политик на Выдача для Azure Marketplace
description: Узнайте, как налоговые политики влияют на выплата в Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686319"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="b4d7d-103">Влияние налоговых политик на Выдача для Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="b4d7d-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="b4d7d-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="b4d7d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b4d7d-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b4d7d-105">Global admin</span></span>
- <span data-ttu-id="b4d7d-106">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="b4d7d-106">User management admin</span></span>
- <span data-ttu-id="b4d7d-107">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="b4d7d-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="b4d7d-108">Введение</span><span class="sxs-lookup"><span data-stu-id="b4d7d-108">Introduction</span></span>

<span data-ttu-id="b4d7d-109">В коммерческом магазине Майкрософт есть глобальный доступ.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="b4d7d-110">Транзакции происходят по границам, и в зависимости от того, где находятся независимые поставщики программного обеспечения и клиента, налоговые последствия могут различаться.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="b4d7d-111">Microsoft AppSource и Azure Marketplace используют сведения о профиле налогов центра партнеров для определения страны ISV.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="b4d7d-112">Чтобы определить страну клиента, следует либо использовать сведения о выставлении счетов клиента, либо, если клиент входит в ЕС, мы используем два разных фрагмента информации.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="b4d7d-113">Чтобы лучше разобраться в следующих сценариях, см. таблицу [сведения о налогах](tax-details-marketplace.md) , в которой показано, собирает ли корпорация Майкрософт налоги от имени издателя или если ответственность принадлежит к издателю.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="b4d7d-114">Все примеры значений продаж и налоговых процентов в этом разделе предназначены только для наглядности, а не для точных иллюстраций.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="b4d7d-115">Издатель взаимодействует в стране налога, управляемой корпорацией Майкрософт</span><span class="sxs-lookup"><span data-stu-id="b4d7d-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="b4d7d-116">**Сценарий A** — транзакции, которые выполняются между издателем и клиентом в [стране налога, управляемом корпорацией Майкрософт](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="b4d7d-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="b4d7d-117">Эти транзакции будут иметь применимый налог, добавленный во время продажи, и корпорация Майкрософт отправит этот налог в соответствующую страну.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="b4d7d-118">Налоги не будут удержаны из расчета выплат, а Расчет выплат не является налоговым.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="b4d7d-119">См. [сценарий г](#foreign-publisher-transacts-with-us-customer) для транзакций между издателем, ОТЛИЧНЫМ от США, и клиентом США.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты а.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="b4d7d-121">Издатель взаимодействует в стране налога, управляемой корпорацией Майкрософт, где плата Marketplace является налогооблагаемой службой</span><span class="sxs-lookup"><span data-stu-id="b4d7d-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="b4d7d-122">**Сценарий б** . транзакции, выполняемые между издателем на основе США (как определено в сведениях о почтовом профиле центра партнеров) к клиенту в стране налога, управляемом корпорацией Майкрософт, в которой страна накладывает налог на плату Marketplace (налогооблагаемая служба).</span><span class="sxs-lookup"><span data-stu-id="b4d7d-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="b4d7d-123">В этом сценарии налог на услугу оплаты магазина вычитается из выплаты издателя.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты б.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="b4d7d-125">Издатель взаимодействует в стране налога, управляемой издателем</span><span class="sxs-lookup"><span data-stu-id="b4d7d-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="b4d7d-126">**Сценарий C** — транзакции, которые выполняются между издателем и клиентом в налоговой стране, управляемой издателем, которая не накладывает на клиентов подоходный налог.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="b4d7d-127">Клиенты платят без налогов на момент продажи, и это обязательства издателя по оплате всех применимых налогов.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="b4d7d-128">Дополнительные сведения о ценах, относящихся к конкретной стране (например, для смещения предстоящего налогообложения), см. в статье [планы и цены на коммерческие предложения Marketplace](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="b4d7d-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="b4d7d-130">Внешний издатель взаимодействует с клиентами США</span><span class="sxs-lookup"><span data-stu-id="b4d7d-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="b4d7d-131">**Сценарий г** . все иностранные издатели (как определено в сведениях о почтовом профиле центра партнеров) в странах без соглашения США (см. [сценарий E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) принятие продажи клиенту на основе США (как определено в адресе учетной записи клиента).</span><span class="sxs-lookup"><span data-stu-id="b4d7d-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="b4d7d-132">Для государственных организаций США требуется, чтобы от имени издателя был удержан налог от корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="b4d7d-133">Налог, удержанный от выплаты к издателю, вычисляется на основе цены предложения.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты г.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="b4d7d-135">Внешний издатель с договором взаимодействует с клиентом США</span><span class="sxs-lookup"><span data-stu-id="b4d7d-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="b4d7d-136">**Сценарий E** . все иностранные издатели (как определено в сведениях о почтовом профиле центра партнеров) в странах с договором США о продажах клиенту на основе США (как определено по адресу учетной записи клиента).</span><span class="sxs-lookup"><span data-stu-id="b4d7d-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="b4d7d-137">Для государственных организаций США не требуется удержание налога от корпорации Майкрософт от имени издателя.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="b4d7d-139">Иностранный издатель продает клиенту, зарегистрированному в ЕС, в стране, управляемой Майкрософт (за пределами Ирландии)</span><span class="sxs-lookup"><span data-stu-id="b4d7d-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="b4d7d-140">**Сценарий F** — все транзакции между внешними издателями и зарегистрированными в ЕС клиентами (за пределами Ирландии) в стране Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="b4d7d-141">Клиент не оплачивает налоги по продажам.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="b4d7d-143">Иностранный издатель продает клиенту, зарегистрированному в ЕС, в стране, управляемой корпорацией Майкрософт (в Ирландии).</span><span class="sxs-lookup"><span data-stu-id="b4d7d-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="b4d7d-144">**Сценарий G** — все транзакции между внешними издателями и зарегистрированными клиентами ЕС (в Ирландии) в Microsoft-Managed стране.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="b4d7d-145">Клиент оплачивает ирландский НДС, и корпорация Майкрософт оплачивает этот налог на правительство государственных организаций.</span><span class="sxs-lookup"><span data-stu-id="b4d7d-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты G.":::

## <a name="next-steps"></a><span data-ttu-id="b4d7d-147">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b4d7d-147">Next steps</span></span>

- [<span data-ttu-id="b4d7d-148">Издатель: вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="b4d7d-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="b4d7d-149">Инструкции по созданию платежных и налоговых профилей</span><span class="sxs-lookup"><span data-stu-id="b4d7d-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)