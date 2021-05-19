---
title: Применение кредитного лимита
ms.topic: how-to
ms.date: 05/11/2021
description: Узнайте о лимите кредита и его расчете. Включает часто задаваемые вопросы.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148114"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="4ee87-104">Принудительное применение кредитного лимита (CLE)</span><span class="sxs-lookup"><span data-stu-id="4ee87-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="4ee87-105">**Соответствующие роли**: администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="4ee87-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="4ee87-106">Ваш кредитный лимит и принцип его работы</span><span class="sxs-lookup"><span data-stu-id="4ee87-106">Your credit limit and how it works</span></span>

<span data-ttu-id="4ee87-107">Лимит кредита — это максимальный объем (в долларах США), который вы как партнер может потратить на приобретение продуктов или подписок в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee87-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="4ee87-108">Если вы превысили лимит кредита, вы не сможете создавать новые покупки до тех пор, пока не будет выполнена достаточная оплата.</span><span class="sxs-lookup"><span data-stu-id="4ee87-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="4ee87-109">Существующие подписки будут продолжать работать.</span><span class="sxs-lookup"><span data-stu-id="4ee87-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="4ee87-110">Кредитные лимиты применяются к предложениям в плане Azure, резервировании Azure, программном обеспечении, Marketplace, Azure 145 P, Office и Dynamics.</span><span class="sxs-lookup"><span data-stu-id="4ee87-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="4ee87-111">Кредитные лимиты не применяются к продлению и текущему потреблению.</span><span class="sxs-lookup"><span data-stu-id="4ee87-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="4ee87-112">Мы присваиваем лимит кредита на уровне клиента в течение периода адаптации.</span><span class="sxs-lookup"><span data-stu-id="4ee87-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="4ee87-113">Это основано на прогнозируемом доходе, покупке провесс и журнале платежей.</span><span class="sxs-lookup"><span data-stu-id="4ee87-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="4ee87-114">Затем мы используем следующую формулу для вычисления доступного баланса:</span><span class="sxs-lookup"><span data-stu-id="4ee87-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="4ee87-115">**[Кредитный лимит — (входящий заказ на покупку + неоплаченные счета + неоплачиваемые расходы — переплата)]**</span><span class="sxs-lookup"><span data-stu-id="4ee87-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="4ee87-116">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="4ee87-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="4ee87-117">Установлен ли лимит кредита на уровне клиента или глобального уровня?</span><span class="sxs-lookup"><span data-stu-id="4ee87-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="4ee87-118">Уровень клиента.</span><span class="sxs-lookup"><span data-stu-id="4ee87-118">The tenant level.</span></span> <span data-ttu-id="4ee87-119">Например, предположим, что вы работали с США, Канады и Японии.</span><span class="sxs-lookup"><span data-stu-id="4ee87-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="4ee87-120">Если клиент Канады достигнет своего кредитного лимита, этот клиент получит уведомление при попытке выполнить покупку в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee87-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="4ee87-121">Другие клиенты не будут затронуты.</span><span class="sxs-lookup"><span data-stu-id="4ee87-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="4ee87-122">Если я превысить лимит кредита, можно ли продолжить обслуживание существующих клиентов и подписок с полным доступом?</span><span class="sxs-lookup"><span data-stu-id="4ee87-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="4ee87-123">Да.</span><span class="sxs-lookup"><span data-stu-id="4ee87-123">Yes.</span></span> <span data-ttu-id="4ee87-124">Существующие подписки клиентов будут продолжать работать без перерывов.</span><span class="sxs-lookup"><span data-stu-id="4ee87-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="4ee87-125">Однако вы не можете приобрести новые подписки для своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="4ee87-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="4ee87-126">Применяется ли CLE к прямым партнерам и косвенным поставщикам?</span><span class="sxs-lookup"><span data-stu-id="4ee87-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="4ee87-127">Да, это относится и к обоим.</span><span class="sxs-lookup"><span data-stu-id="4ee87-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="4ee87-128">Когда я отправит платеж, чтобы восстановить мою учетную запись, когда можно купить дополнительные подписки?</span><span class="sxs-lookup"><span data-stu-id="4ee87-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="4ee87-129">Вы сможете возобновить приобретение в течение 24 часов после оплаты, предполагая, что корпорация Майкрософт получила все требования для продолжения процесса проверки кредита.</span><span class="sxs-lookup"><span data-stu-id="4ee87-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="4ee87-130">Как можно проверить кредитный лимит?</span><span class="sxs-lookup"><span data-stu-id="4ee87-130">How can I check my credit limit?</span></span>

<span data-ttu-id="4ee87-131">Обратитесь [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) к, чтобы просмотреть кредитный лимит и получить сведения о последних покупках.</span><span class="sxs-lookup"><span data-stu-id="4ee87-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="4ee87-132">Учитываются ли счета с числом спорных вопросов по кредитному лимиту?</span><span class="sxs-lookup"><span data-stu-id="4ee87-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="4ee87-133">Да.</span><span class="sxs-lookup"><span data-stu-id="4ee87-133">Yes.</span></span> <span data-ttu-id="4ee87-134">Однако для решения этой проблемы можно обратиться в корпорацию Майкрософт по адресу [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) .</span><span class="sxs-lookup"><span data-stu-id="4ee87-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="4ee87-135">Как скоро будет слышен ответ, если я записал ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="4ee87-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="4ee87-136">Ответ должен быть менее 24 часов.</span><span class="sxs-lookup"><span data-stu-id="4ee87-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="4ee87-137">Какие критерии Корпорация Майкрософт использует для настройки кредитного лимита партнера?</span><span class="sxs-lookup"><span data-stu-id="4ee87-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="4ee87-138">Мы определяем лимит кредита на основе прогнозируемого дохода, покупки провесс и журнала платежей.</span><span class="sxs-lookup"><span data-stu-id="4ee87-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="4ee87-139">Используется ли лимит кредита в настоящее время для нового коммерческого интерфейса?</span><span class="sxs-lookup"><span data-stu-id="4ee87-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="4ee87-140">Да.</span><span class="sxs-lookup"><span data-stu-id="4ee87-140">Yes.</span></span> <span data-ttu-id="4ee87-141">Лимиты кредита применяются ко всем программам и продуктам CSP в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee87-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="4ee87-142">Кто будет принимать уведомление, когда моя организация приближается к кредитному лимиту?</span><span class="sxs-lookup"><span data-stu-id="4ee87-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="4ee87-143">Контактное лицо для расчета финансового счета в вашей организации должно получить уведомление.</span><span class="sxs-lookup"><span data-stu-id="4ee87-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4ee87-144">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="4ee87-144">Next steps</span></span>

[<span data-ttu-id="4ee87-145">Основы выставления счетов</span><span class="sxs-lookup"><span data-stu-id="4ee87-145">Billing basics</span></span>](./billing-basics.md)
