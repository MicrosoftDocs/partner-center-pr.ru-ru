---
title: Установка расходного бюджета Azure для клиентов | Центр партнеров
ms.topic: article
ms.date: 11/21/2019
description: Установите месячный бюджет для каждого клиента в центре партнеров.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 05212746e1ccbcc5081c68ca97ced6a99e20bb8c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384892"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="b0705-103">Установка расходного бюджета Azure для клиентов</span><span class="sxs-lookup"><span data-stu-id="b0705-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="b0705-104">Относится к:</span><span class="sxs-lookup"><span data-stu-id="b0705-104">Applies to:</span></span>

- <span data-ttu-id="b0705-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="b0705-105">Partner Center</span></span>
- <span data-ttu-id="b0705-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="b0705-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b0705-107">Вы можете [задать ежемесячный бюджет расходов на Azure для клиентов](#set-azure-spending-budget) в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0705-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="b0705-108">Это помогает Вашим клиентам управлять расходами на Azure.</span><span class="sxs-lookup"><span data-stu-id="b0705-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="b0705-109">Этот параметр позволяет сравнить расходы на Azure с бюджетом в течение месяца.</span><span class="sxs-lookup"><span data-stu-id="b0705-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="b0705-110">Это также помогает Вашим заказчикам оценить затраты на Azure, чтобы их месячный счет не превышал ожидаемый объем.</span><span class="sxs-lookup"><span data-stu-id="b0705-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>


> [!NOTE]  
> <span data-ttu-id="b0705-111">Эта функция недоступна в "песочнице" или "тестирование" в рабочей учетной записи (TIP).</span><span class="sxs-lookup"><span data-stu-id="b0705-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="b0705-112">После того как вы [настроили бюджет расходов Azure для ваших клиентов](#set-azure-spending-budget), вы также можете просматривать сведения об использовании клиентов следующими способами.</span><span class="sxs-lookup"><span data-stu-id="b0705-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="b0705-113">Эти параметры могут помочь вам выявить неправильно настроенные службы или необычные тенденции, которые могут предложить мошенничество.</span><span class="sxs-lookup"><span data-stu-id="b0705-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="b0705-114">Затем вы можете работать с клиентами для выяснения основной причины и управления затратами.</span><span class="sxs-lookup"><span data-stu-id="b0705-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="b0705-115">При необходимости можно также [изменить бюджет клиента](#set-azure-spending-budget) на более высокий.</span><span class="sxs-lookup"><span data-stu-id="b0705-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="b0705-116">Проверка текущих расходов Azure</span><span class="sxs-lookup"><span data-stu-id="b0705-116">Check current Azure spending</span></span>](#check-current-azure-spending)
- [<span data-ttu-id="b0705-117">Включить уведомления по электронной почте, когда расходы клиента приближается к лимиту бюджета</span><span class="sxs-lookup"><span data-stu-id="b0705-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)
- [<span data-ttu-id="b0705-118">Просмотр детализированных затрат по службе для подписок на основе использования</span><span class="sxs-lookup"><span data-stu-id="b0705-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="b0705-119">Вы также можете [Удалить бюджет расходов Azure](#remove-azure-spending-budget) для клиентов в любое время.</span><span class="sxs-lookup"><span data-stu-id="b0705-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="b0705-120">Данные о расходах Azure</span><span class="sxs-lookup"><span data-stu-id="b0705-120">Azure spending data</span></span>

<span data-ttu-id="b0705-121">Данные о расходах Azure — это *Оценка* , и *фактические суммы счетов могут отличаться*.</span><span class="sxs-lookup"><span data-stu-id="b0705-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="b0705-122">Значение данных *не отражает* налоги, кредиты, корректировки и другие расходы, которые могут быть применены.</span><span class="sxs-lookup"><span data-stu-id="b0705-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="b0705-123">Данные о расходах *обновляются раз в день*.</span><span class="sxs-lookup"><span data-stu-id="b0705-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="b0705-124">Ваши клиенты могут по-прежнему использовать и заставлять счета за использование служб и ресурсов Azure, если не изменить параметры учетной записи в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="b0705-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="b0705-125">Настройка бюджета расходов Azure</span><span class="sxs-lookup"><span data-stu-id="b0705-125">Set Azure spending budget</span></span>

<span data-ttu-id="b0705-126">Вы можете *задать ежемесячный бюджет расходов на Azure* для нескольких клиентов в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="b0705-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="b0705-127">Войдите на [панель мониторинга центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b0705-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="b0705-128">В меню слева в разделе **CSP**выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="b0705-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="b0705-129">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure**выберите клиентов, для которых требуется задать бюджет.</span><span class="sxs-lookup"><span data-stu-id="b0705-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>
4. <span data-ttu-id="b0705-130">Введите значение для **месячного бюджета**.</span><span class="sxs-lookup"><span data-stu-id="b0705-130">Enter a value for **Monthly budget**.</span></span>
5. <span data-ttu-id="b0705-131">Нажмите кнопку **Применить** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="b0705-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="b0705-132">Вы также можете *задать бюджет для отдельного клиента* в параметрах подписки:</span><span class="sxs-lookup"><span data-stu-id="b0705-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="b0705-133">Войдите на панель мониторинга центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0705-133">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="b0705-134">В меню слева в разделе **CSP**выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="b0705-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="b0705-135">На странице **Клиенты** выберите **название компании**клиента.</span><span class="sxs-lookup"><span data-stu-id="b0705-135">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="b0705-136">На странице **подписки** клиента в разделе **Подписка на основе использования**выберите **изменить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="b0705-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>
5. <span data-ttu-id="b0705-137">Введите значение для бюджета.</span><span class="sxs-lookup"><span data-stu-id="b0705-137">Enter a value for the budget.</span></span>
6. <span data-ttu-id="b0705-138">Нажмите кнопку **Применить** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="b0705-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="b0705-139">Удаление бюджета расходов Azure</span><span class="sxs-lookup"><span data-stu-id="b0705-139">Remove Azure spending budget</span></span>

<span data-ttu-id="b0705-140">Вы можете *Удалить месячный бюджет расходов на Azure* для ваших клиентов в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="b0705-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="b0705-141">Войдите на [панель мониторинга центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b0705-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="b0705-142">В меню слева в разделе **CSP**выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="b0705-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="b0705-143">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure**выберите клиентов, бюджет которых необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="b0705-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>
4. <span data-ttu-id="b0705-144">Выберите **Удалить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="b0705-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="b0705-145">Проверка текущих расходов Azure</span><span class="sxs-lookup"><span data-stu-id="b0705-145">Check current Azure spending</span></span>

<span data-ttu-id="b0705-146">Вы можете в любое время *отслеживанию текущих затрат Azure и ежемесячных бюджетов клиентов* :</span><span class="sxs-lookup"><span data-stu-id="b0705-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="b0705-147">Войдите на [панель мониторинга центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b0705-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="b0705-148">В меню слева в разделе **CSP**выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="b0705-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="b0705-149">На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure**вы можете просмотреть обзор месячных бюджетов клиентов, оценки текущих расходов и процент использования бюджета.</span><span class="sxs-lookup"><span data-stu-id="b0705-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="b0705-150">Уведомления об ограничениях бюджета</span><span class="sxs-lookup"><span data-stu-id="b0705-150">Notifications for budget limits</span></span>

<span data-ttu-id="b0705-151">Вы можете *включить уведомления по электронной почте* , когда месячные затраты клиента приближается к лимиту бюджета.</span><span class="sxs-lookup"><span data-stu-id="b0705-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="b0705-152">При включении этого параметра вы получите уведомления, когда клиенты будут использовать 80% или больше ежемесячного бюджета.</span><span class="sxs-lookup"><span data-stu-id="b0705-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="b0705-153">Этот параметр позволяет следить за счетом Azure.</span><span class="sxs-lookup"><span data-stu-id="b0705-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="b0705-154">Настройка уведомлений по электронной почте:</span><span class="sxs-lookup"><span data-stu-id="b0705-154">To configure email notifications:</span></span>

1. <span data-ttu-id="b0705-155">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0705-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="b0705-156">В меню слева в разделе **CSP**выберите **затраты на Azure**.</span><span class="sxs-lookup"><span data-stu-id="b0705-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="b0705-157">На странице " **расходы Azure** " в разделе **уведомления по электронной почте**установите переключатель **получить электронные сообщения** в положение **вкл**.</span><span class="sxs-lookup"><span data-stu-id="b0705-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>
4. <span data-ttu-id="b0705-158">Выберите **изменить адрес электронной почты** , чтобы просмотреть адрес электронной почты для уведомлений.</span><span class="sxs-lookup"><span data-stu-id="b0705-158">Choose **Change email address** to see the email address for notifications.</span></span>
5. <span data-ttu-id="b0705-159">Если адрес электронной почты *неправильный*, введите правильный адрес электронной почты и нажмите кнопку **Обновить**.</span><span class="sxs-lookup"><span data-stu-id="b0705-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="b0705-160">Если адрес электронной почты *указан правильно*, нажмите кнопку **Отмена**.</span><span class="sxs-lookup"><span data-stu-id="b0705-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="b0705-161">Детализированные затраты по службам</span><span class="sxs-lookup"><span data-stu-id="b0705-161">Itemized costs by service</span></span>

<span data-ttu-id="b0705-162">Можно *Просмотреть детализированные затраты (и предполагаемое использование) службой для подписок на основе использования*:</span><span class="sxs-lookup"><span data-stu-id="b0705-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="b0705-163">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0705-163">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="b0705-164">В меню слева в разделе **CSP**выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="b0705-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="b0705-165">На странице **Клиенты** выберите **название компании**клиента.</span><span class="sxs-lookup"><span data-stu-id="b0705-165">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="b0705-166">На странице **подписки** клиента в разделе **подписки на основе использования**выберите имя **подписки**.</span><span class="sxs-lookup"><span data-stu-id="b0705-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>
5. <span data-ttu-id="b0705-167">На странице подписки можно просматривать **детализированные затраты** по службам и **оценивать использование** за текущий месяц.</span><span class="sxs-lookup"><span data-stu-id="b0705-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
