---
title: Влияние налоговых политик на Выдача для Azure Marketplace
description: Узнайте, как налоговые политики влияют на выплата в Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 32c5cda9558aaaeddaf194eb8258ba732e2ac698
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489974"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="d6497-103">Влияние налоговых политик на Выдача для Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d6497-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="d6497-104">**Соответствующие роли**: глобальный администратор | Администратор управления пользователями | Агент администратора</span><span class="sxs-lookup"><span data-stu-id="d6497-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="d6497-105">Введение</span><span class="sxs-lookup"><span data-stu-id="d6497-105">Introduction</span></span>

<span data-ttu-id="d6497-106">В коммерческом магазине Майкрософт есть глобальный доступ.</span><span class="sxs-lookup"><span data-stu-id="d6497-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="d6497-107">Транзакции происходят по границам, и в зависимости от того, где находятся независимые поставщики программного обеспечения и клиент, налоговые последствия могут различаться.</span><span class="sxs-lookup"><span data-stu-id="d6497-107">Transactions occur across borders and depending on where the independent software vendor (ISV) and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="d6497-108">Microsoft AppSource и Azure Marketplace используют сведения о профиле налогов центра партнеров для определения страны ISV.</span><span class="sxs-lookup"><span data-stu-id="d6497-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="d6497-109">Чтобы определить страну клиента, следует либо использовать сведения о выставлении счетов клиента, либо, если клиент входит в ЕС, мы используем два разных фрагмента информации.</span><span class="sxs-lookup"><span data-stu-id="d6497-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="d6497-110">Чтобы лучше разобраться в следующих сценариях, см. таблицу [сведения о налогах](tax-details-marketplace.md) , в которой показано, собирает ли корпорация Майкрософт налоги от имени издателя или если ответственность принадлежит к издателю.</span><span class="sxs-lookup"><span data-stu-id="d6497-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="d6497-111">Все примеры значений продаж и налоговых процентов в этом разделе предназначены только для наглядности, а не для точных иллюстраций.</span><span class="sxs-lookup"><span data-stu-id="d6497-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="d6497-112">Издатель взаимодействует в стране налога, управляемой корпорацией Майкрософт</span><span class="sxs-lookup"><span data-stu-id="d6497-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="d6497-113">**Сценарий A** — транзакции, которые выполняются между издателем и клиентом в [стране налога, управляемом корпорацией Майкрософт](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="d6497-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="d6497-114">Эти транзакции будут иметь применимый налог, добавленный во время продажи, и корпорация Майкрософт отправит этот налог в соответствующую страну.</span><span class="sxs-lookup"><span data-stu-id="d6497-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="d6497-115">Налоги не будут удержаны из расчета выплат, а Расчет выплат не является налоговым.</span><span class="sxs-lookup"><span data-stu-id="d6497-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="d6497-116">См. [сценарий г](#foreign-publisher-transacts-with-us-customer) для транзакций между издателем, ОТЛИЧНЫМ от США, и клиентом США.</span><span class="sxs-lookup"><span data-stu-id="d6497-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты а.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="d6497-118">Издатель взаимодействует в стране налога, управляемой корпорацией Майкрософт, где плата Marketplace является налогооблагаемой службой</span><span class="sxs-lookup"><span data-stu-id="d6497-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="d6497-119">**Сценарий б** . транзакции, выполняемые между издателем на основе США (как определено в сведениях о почтовом профиле центра партнеров) к клиенту в стране налога, управляемом корпорацией Майкрософт, в которой страна накладывает налог на плату Marketplace (налогооблагаемая служба).</span><span class="sxs-lookup"><span data-stu-id="d6497-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="d6497-120">В этом сценарии налог на услугу оплаты магазина вычитается из выплаты издателя.</span><span class="sxs-lookup"><span data-stu-id="d6497-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты б.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="d6497-122">Издатель взаимодействует в стране налога, управляемой издателем</span><span class="sxs-lookup"><span data-stu-id="d6497-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="d6497-123">**Сценарий C** — транзакции, которые выполняются между издателем и клиентом в налоговой стране, управляемой издателем, которая не накладывает на клиентов подоходный налог.</span><span class="sxs-lookup"><span data-stu-id="d6497-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="d6497-124">Клиенты платят без налогов на момент продажи, и это обязательства издателя по оплате всех применимых налогов.</span><span class="sxs-lookup"><span data-stu-id="d6497-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="d6497-125">Дополнительные сведения о ценах, относящихся к конкретной стране (например, для смещения предстоящего налогообложения), см. в статье [планы и цены на коммерческие предложения Marketplace](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="d6497-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="d6497-127">Внешний издатель взаимодействует с клиентами США</span><span class="sxs-lookup"><span data-stu-id="d6497-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="d6497-128">**Сценарий г** . все иностранные издатели (как определено в сведениях о почтовом профиле центра партнеров) в странах без соглашения США (см. [сценарий E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) принятие продажи клиенту на основе США (как определено в адресе учетной записи клиента).</span><span class="sxs-lookup"><span data-stu-id="d6497-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="d6497-129">Для государственных организаций США требуется, чтобы от имени издателя был удержан налог от корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d6497-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="d6497-130">Налог, удержанный от выплаты к издателю, вычисляется на основе цены предложения.</span><span class="sxs-lookup"><span data-stu-id="d6497-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты г.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="d6497-132">Внешний издатель с договором взаимодействует с клиентом США</span><span class="sxs-lookup"><span data-stu-id="d6497-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="d6497-133">**Сценарий E** . все иностранные издатели (как определено в сведениях о почтовом профиле центра партнеров) в странах с договором США о продажах клиенту на основе США (как определено по адресу учетной записи клиента).</span><span class="sxs-lookup"><span data-stu-id="d6497-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="d6497-134">Для государственных организаций США не требуется удержание налога от корпорации Майкрософт от имени издателя.</span><span class="sxs-lookup"><span data-stu-id="d6497-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="d6497-136">Иностранный издатель продает клиенту, зарегистрированному в ЕС, в стране, управляемой Майкрософт (за пределами Ирландии)</span><span class="sxs-lookup"><span data-stu-id="d6497-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="d6497-137">**Сценарий F** . все транзакции между внешними издателями и добавленными стоимостью налогов (НДС) — зарегистрированные клиенты (за пределами Ирландии) в стране Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="d6497-137">**Scenario F** – All transactions between foreign publishers and EU value-added tax (VAT)-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="d6497-138">Клиент не оплачивает налоги по продажам.</span><span class="sxs-lookup"><span data-stu-id="d6497-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="d6497-140">Иностранный издатель продает клиенту, зарегистрированному в ЕС, в стране, управляемой корпорацией Майкрософт (в Ирландии).</span><span class="sxs-lookup"><span data-stu-id="d6497-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="d6497-141">**Сценарий G** — все транзакции между внешними издателями и зарегистрированными клиентами ЕС (в Ирландии) в Microsoft-Managed стране.</span><span class="sxs-lookup"><span data-stu-id="d6497-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="d6497-142">Клиент оплачивает ирландский НДС, и корпорация Майкрософт оплачивает этот налог на правительство государственных организаций.</span><span class="sxs-lookup"><span data-stu-id="d6497-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты G.":::

## <a name="next-steps"></a><span data-ttu-id="d6497-144">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="d6497-144">Next steps</span></span>

- [<span data-ttu-id="d6497-145">Издатель: вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="d6497-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="d6497-146">Инструкции по созданию платежных и налоговых профилей</span><span class="sxs-lookup"><span data-stu-id="d6497-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)