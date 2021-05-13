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
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855358"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="d20dc-103">Установка, проверка и удаление ежемесячных бюджетных расходов Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="d20dc-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="d20dc-104">**Соответствующие роли**: Агент администрирования</span><span class="sxs-lookup"><span data-stu-id="d20dc-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="d20dc-105">Вы можете [задать ежемесячный бюджет расходов на Azure для клиентов](#set-azure-spending-budget) в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="d20dc-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="d20dc-106">Это помогает Вашим клиентам управлять расходами на Azure.</span><span class="sxs-lookup"><span data-stu-id="d20dc-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="d20dc-107">Этот параметр позволяет сравнить расходы на Azure с бюджетом в течение месяца.</span><span class="sxs-lookup"><span data-stu-id="d20dc-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="d20dc-108">Кроме того, он позволяет клиентам вычислять затраты на Azure, чтобы их месячный счет не превышал ожидаемый объем.</span><span class="sxs-lookup"><span data-stu-id="d20dc-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="d20dc-109">Эта функция недоступна в "песочнице" или "тестирование" в рабочей учетной записи (TIP).</span><span class="sxs-lookup"><span data-stu-id="d20dc-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="d20dc-110">После того как вы [настроили бюджет расходов Azure для ваших клиентов](#set-azure-spending-budget), вы также можете просматривать сведения об использовании клиентов следующими способами.</span><span class="sxs-lookup"><span data-stu-id="d20dc-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="d20dc-111">Эти параметры могут помочь вам выявить неправильно настроенные службы или необычные тенденции, которые могут предложить мошенничество.</span><span class="sxs-lookup"><span data-stu-id="d20dc-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="d20dc-112">Затем вы можете работать с клиентами для выяснения основной причины и управления затратами.</span><span class="sxs-lookup"><span data-stu-id="d20dc-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="d20dc-113">При необходимости можно также [изменить бюджет клиента](#set-azure-spending-budget) на более высокий.</span><span class="sxs-lookup"><span data-stu-id="d20dc-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="d20dc-114">Проверка текущих расходов Azure</span><span class="sxs-lookup"><span data-stu-id="d20dc-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="d20dc-115">Включить уведомления по электронной почте, когда расходы клиента приближается к лимиту бюджета</span><span class="sxs-lookup"><span data-stu-id="d20dc-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="d20dc-116">Просмотр детализированных затрат по службе для подписок на основе использования</span><span class="sxs-lookup"><span data-stu-id="d20dc-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="d20dc-117">Вы также можете [Удалить бюджет расходов Azure](#remove-azure-spending-budget) для клиентов в любое время.</span><span class="sxs-lookup"><span data-stu-id="d20dc-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="d20dc-118">Данные о расходах Azure</span><span class="sxs-lookup"><span data-stu-id="d20dc-118">Azure spending data</span></span>

<span data-ttu-id="d20dc-119">Данные о расходах Azure — это *Оценка* , и *фактические суммы счетов могут отличаться*.</span><span class="sxs-lookup"><span data-stu-id="d20dc-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="d20dc-120">Значение данных *не отражает* налоги, кредиты, корректировки и другие расходы, которые могут быть применены.</span><span class="sxs-lookup"><span data-stu-id="d20dc-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="d20dc-121">Данные о расходах *обновляются раз в день*.</span><span class="sxs-lookup"><span data-stu-id="d20dc-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="d20dc-122">Ваши клиенты могут по-прежнему использовать и заставлять счета за использование служб и ресурсов Azure, если не изменить параметры учетной записи в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="d20dc-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="d20dc-123">Настройка бюджета расходов Azure</span><span class="sxs-lookup"><span data-stu-id="d20dc-123">Set Azure spending budget</span></span>

<span data-ttu-id="d20dc-124">Вы можете *задать ежемесячный бюджет расходов на Azure* для нескольких клиентов в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="d20dc-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="d20dc-125">Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="d20dc-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="d20dc-126">В меню слева в разделе **CSP** выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="d20dc-127">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** выберите клиентов, для которых требуется задать бюджет.</span><span class="sxs-lookup"><span data-stu-id="d20dc-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="d20dc-128">Введите значение для **месячного бюджета**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="d20dc-129">Нажмите кнопку **Применить** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="d20dc-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="d20dc-130">Вы также можете *задать бюджет для отдельного клиента* в параметрах подписки:</span><span class="sxs-lookup"><span data-stu-id="d20dc-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="d20dc-131">Войдите на панель мониторинга Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d20dc-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="d20dc-132">В меню слева в разделе **CSP** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="d20dc-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="d20dc-133">На странице **Клиенты** выберите **название компании** клиента.</span><span class="sxs-lookup"><span data-stu-id="d20dc-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="d20dc-134">На странице **подписки** клиента в разделе **Подписка на основе использования** выберите **изменить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="d20dc-135">Введите значение для бюджета.</span><span class="sxs-lookup"><span data-stu-id="d20dc-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="d20dc-136">Нажмите кнопку **Применить** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="d20dc-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="d20dc-137">Удаление бюджета расходов Azure</span><span class="sxs-lookup"><span data-stu-id="d20dc-137">Remove Azure spending budget</span></span>

<span data-ttu-id="d20dc-138">Вы можете *Удалить месячный бюджет расходов на Azure* для ваших клиентов в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="d20dc-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="d20dc-139">Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="d20dc-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="d20dc-140">В меню слева в разделе **CSP** выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="d20dc-141">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** выберите клиентов, бюджет которых необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="d20dc-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="d20dc-142">Выберите **Удалить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="d20dc-143">Проверка текущих расходов Azure</span><span class="sxs-lookup"><span data-stu-id="d20dc-143">Check current Azure spending</span></span>

<span data-ttu-id="d20dc-144">Вы можете в любое время *отслеживанию текущих затрат Azure и ежемесячных бюджетов клиентов* :</span><span class="sxs-lookup"><span data-stu-id="d20dc-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="d20dc-145">Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="d20dc-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="d20dc-146">В меню слева в разделе **CSP** выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="d20dc-147">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** вы можете просмотреть обзор месячных бюджетов клиентов, оценки текущих расходов и процент использования бюджета.</span><span class="sxs-lookup"><span data-stu-id="d20dc-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="d20dc-148">Уведомления об ограничениях бюджета</span><span class="sxs-lookup"><span data-stu-id="d20dc-148">Notifications for budget limits</span></span>

<span data-ttu-id="d20dc-149">Вы можете *включить уведомления по электронной почте* , когда месячные затраты клиента приближается к лимиту бюджета.</span><span class="sxs-lookup"><span data-stu-id="d20dc-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="d20dc-150">При включении этого параметра вы получите уведомления, когда клиенты будут использовать 80% или больше ежемесячного бюджета.</span><span class="sxs-lookup"><span data-stu-id="d20dc-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="d20dc-151">Этот параметр позволяет следить за счетом Azure.</span><span class="sxs-lookup"><span data-stu-id="d20dc-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="d20dc-152">Настройка уведомлений по электронной почте:</span><span class="sxs-lookup"><span data-stu-id="d20dc-152">To configure email notifications:</span></span>

1. <span data-ttu-id="d20dc-153">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="d20dc-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="d20dc-154">Перейдите в меню **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="d20dc-155">Выберите **Мои предпочтения**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="d20dc-156">Если вы этого не сделали, настройте предпочтительный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d20dc-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="d20dc-157">Настройте предпочтительный язык для уведомления.</span><span class="sxs-lookup"><span data-stu-id="d20dc-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="d20dc-158">Выберите вкладку **CSP** в разделе **Параметры уведомления** .</span><span class="sxs-lookup"><span data-stu-id="d20dc-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="d20dc-159">Установите флажок Электронная почта для уведомления **Azure о расходах** и **Сохраните**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="d20dc-160">Детализированные затраты по службам</span><span class="sxs-lookup"><span data-stu-id="d20dc-160">Itemized costs by service</span></span>

<span data-ttu-id="d20dc-161">Можно *Просмотреть детализированные затраты (и предполагаемое использование) службой для подписок на основе использования*:</span><span class="sxs-lookup"><span data-stu-id="d20dc-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="d20dc-162">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="d20dc-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="d20dc-163">В меню слева в разделе **CSP** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="d20dc-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="d20dc-164">На странице **Клиенты** выберите **название компании** клиента.</span><span class="sxs-lookup"><span data-stu-id="d20dc-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="d20dc-165">На странице **подписки** клиента в разделе **подписки на основе использования** выберите имя **подписки**.</span><span class="sxs-lookup"><span data-stu-id="d20dc-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="d20dc-166">На странице подписки можно просматривать **детализированные затраты** по службам и **оценивать использование** за текущий месяц.</span><span class="sxs-lookup"><span data-stu-id="d20dc-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="d20dc-167">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d20dc-167">Next steps</span></span>

- [<span data-ttu-id="d20dc-168">Новый интерфейс для коммерческих приложений в CSP. Выставление счетов в Azure</span><span class="sxs-lookup"><span data-stu-id="d20dc-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
