---
title: Установка расходного бюджета Azure для клиентов
ms.topic: how-to
ms.date: 03/17/2021
description: Узнайте, как устанавливать или удалять месячные бюджеты расходов на Azure для клиентов, а также просматривать данные о расходах Azure и задавать уведомления, связанные с бюджетом.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712755"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="c254b-103">Установка, проверка и удаление ежемесячных бюджетных расходов Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="c254b-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="c254b-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="c254b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c254b-105">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="c254b-105">Admin agent</span></span>

<span data-ttu-id="c254b-106">Вы можете [задать ежемесячный бюджет расходов на Azure для клиентов](#set-azure-spending-budget) в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="c254b-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="c254b-107">Это помогает Вашим клиентам управлять расходами на Azure.</span><span class="sxs-lookup"><span data-stu-id="c254b-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="c254b-108">Этот параметр позволяет сравнить расходы на Azure с бюджетом в течение месяца.</span><span class="sxs-lookup"><span data-stu-id="c254b-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="c254b-109">Кроме того, он позволяет клиентам вычислять затраты на Azure, чтобы их месячный счет не превышал ожидаемый объем.</span><span class="sxs-lookup"><span data-stu-id="c254b-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="c254b-110">Эта функция недоступна в "песочнице" или "тестирование" в рабочей учетной записи (TIP).</span><span class="sxs-lookup"><span data-stu-id="c254b-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="c254b-111">После того как вы [настроили бюджет расходов Azure для ваших клиентов](#set-azure-spending-budget), вы также можете просматривать сведения об использовании клиентов следующими способами.</span><span class="sxs-lookup"><span data-stu-id="c254b-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="c254b-112">Эти параметры могут помочь вам выявить неправильно настроенные службы или необычные тенденции, которые могут предложить мошенничество.</span><span class="sxs-lookup"><span data-stu-id="c254b-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="c254b-113">Затем вы можете работать с клиентами для выяснения основной причины и управления затратами.</span><span class="sxs-lookup"><span data-stu-id="c254b-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="c254b-114">При необходимости можно также [изменить бюджет клиента](#set-azure-spending-budget) на более высокий.</span><span class="sxs-lookup"><span data-stu-id="c254b-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="c254b-115">Проверка текущих расходов Azure</span><span class="sxs-lookup"><span data-stu-id="c254b-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="c254b-116">Включить уведомления по электронной почте, когда расходы клиента приближается к лимиту бюджета</span><span class="sxs-lookup"><span data-stu-id="c254b-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="c254b-117">Просмотр детализированных затрат по службе для подписок на основе использования</span><span class="sxs-lookup"><span data-stu-id="c254b-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="c254b-118">Вы также можете [Удалить бюджет расходов Azure](#remove-azure-spending-budget) для клиентов в любое время.</span><span class="sxs-lookup"><span data-stu-id="c254b-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="c254b-119">Данные о расходах Azure</span><span class="sxs-lookup"><span data-stu-id="c254b-119">Azure spending data</span></span>

<span data-ttu-id="c254b-120">Данные о расходах Azure — это *Оценка* , и *фактические суммы счетов могут отличаться*.</span><span class="sxs-lookup"><span data-stu-id="c254b-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="c254b-121">Значение данных *не отражает* налоги, кредиты, корректировки и другие расходы, которые могут быть применены.</span><span class="sxs-lookup"><span data-stu-id="c254b-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="c254b-122">Данные о расходах *обновляются раз в день*.</span><span class="sxs-lookup"><span data-stu-id="c254b-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="c254b-123">Ваши клиенты могут по-прежнему использовать и заставлять счета за использование служб и ресурсов Azure, если не изменить параметры учетной записи в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="c254b-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="c254b-124">Настройка бюджета расходов Azure</span><span class="sxs-lookup"><span data-stu-id="c254b-124">Set Azure spending budget</span></span>

<span data-ttu-id="c254b-125">Вы можете *задать ежемесячный бюджет расходов на Azure* для нескольких клиентов в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="c254b-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="c254b-126">Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="c254b-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="c254b-127">В меню слева в разделе **CSP** выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="c254b-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="c254b-128">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** выберите клиентов, для которых требуется задать бюджет.</span><span class="sxs-lookup"><span data-stu-id="c254b-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="c254b-129">Введите значение для **месячного бюджета**.</span><span class="sxs-lookup"><span data-stu-id="c254b-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="c254b-130">Нажмите кнопку **Применить** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="c254b-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="c254b-131">Вы также можете *задать бюджет для отдельного клиента* в параметрах подписки:</span><span class="sxs-lookup"><span data-stu-id="c254b-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="c254b-132">Войдите на панель мониторинга Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c254b-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="c254b-133">В меню слева в разделе **CSP** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="c254b-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="c254b-134">На странице **Клиенты** выберите **название компании** клиента.</span><span class="sxs-lookup"><span data-stu-id="c254b-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="c254b-135">На странице **подписки** клиента в разделе **Подписка на основе использования** выберите **изменить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="c254b-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="c254b-136">Введите значение для бюджета.</span><span class="sxs-lookup"><span data-stu-id="c254b-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="c254b-137">Нажмите кнопку **Применить** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="c254b-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="c254b-138">Удаление бюджета расходов Azure</span><span class="sxs-lookup"><span data-stu-id="c254b-138">Remove Azure spending budget</span></span>

<span data-ttu-id="c254b-139">Вы можете *Удалить месячный бюджет расходов на Azure* для ваших клиентов в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="c254b-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="c254b-140">Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="c254b-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="c254b-141">В меню слева в разделе **CSP** выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="c254b-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="c254b-142">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** выберите клиентов, бюджет которых необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="c254b-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="c254b-143">Выберите **Удалить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="c254b-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="c254b-144">Проверка текущих расходов Azure</span><span class="sxs-lookup"><span data-stu-id="c254b-144">Check current Azure spending</span></span>

<span data-ttu-id="c254b-145">Вы можете в любое время *отслеживанию текущих затрат Azure и ежемесячных бюджетов клиентов* :</span><span class="sxs-lookup"><span data-stu-id="c254b-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="c254b-146">Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="c254b-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="c254b-147">В меню слева в разделе **CSP** выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="c254b-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="c254b-148">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** вы можете просмотреть обзор месячных бюджетов клиентов, оценки текущих расходов и процент использования бюджета.</span><span class="sxs-lookup"><span data-stu-id="c254b-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="c254b-149">Уведомления об ограничениях бюджета</span><span class="sxs-lookup"><span data-stu-id="c254b-149">Notifications for budget limits</span></span>

<span data-ttu-id="c254b-150">Вы можете *включить уведомления по электронной почте* , когда месячные затраты клиента приближается к лимиту бюджета.</span><span class="sxs-lookup"><span data-stu-id="c254b-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="c254b-151">При включении этого параметра вы получите уведомления, когда клиенты будут использовать 80% или больше ежемесячного бюджета.</span><span class="sxs-lookup"><span data-stu-id="c254b-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="c254b-152">Этот параметр позволяет следить за счетом Azure.</span><span class="sxs-lookup"><span data-stu-id="c254b-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="c254b-153">Настройка уведомлений по электронной почте:</span><span class="sxs-lookup"><span data-stu-id="c254b-153">To configure email notifications:</span></span>

1. <span data-ttu-id="c254b-154">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="c254b-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="c254b-155">Перейдите в меню **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="c254b-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="c254b-156">Выберите **Мои предпочтения**.</span><span class="sxs-lookup"><span data-stu-id="c254b-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="c254b-157">Если вы этого не сделали, настройте предпочтительный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c254b-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="c254b-158">Настройте предпочтительный язык для уведомления.</span><span class="sxs-lookup"><span data-stu-id="c254b-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="c254b-159">Выберите вкладку **CSP** в разделе **Параметры уведомления** .</span><span class="sxs-lookup"><span data-stu-id="c254b-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="c254b-160">Установите флажок Электронная почта для уведомления **Azure о расходах** и **Сохраните**.</span><span class="sxs-lookup"><span data-stu-id="c254b-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="c254b-161">Детализированные затраты по службам</span><span class="sxs-lookup"><span data-stu-id="c254b-161">Itemized costs by service</span></span>

<span data-ttu-id="c254b-162">Можно *Просмотреть детализированные затраты (и предполагаемое использование) службой для подписок на основе использования*:</span><span class="sxs-lookup"><span data-stu-id="c254b-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="c254b-163">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="c254b-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="c254b-164">В меню слева в разделе **CSP** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="c254b-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="c254b-165">На странице **Клиенты** выберите **название компании** клиента.</span><span class="sxs-lookup"><span data-stu-id="c254b-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="c254b-166">На странице **подписки** клиента в разделе **подписки на основе использования** выберите имя **подписки**.</span><span class="sxs-lookup"><span data-stu-id="c254b-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="c254b-167">На странице подписки можно просматривать **детализированные затраты** по службам и **оценивать использование** за текущий месяц.</span><span class="sxs-lookup"><span data-stu-id="c254b-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="c254b-168">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c254b-168">Next steps</span></span>

- [<span data-ttu-id="c254b-169">Новый интерфейс для коммерческих приложений в CSP. Выставление счетов в Azure</span><span class="sxs-lookup"><span data-stu-id="c254b-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
