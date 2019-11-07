---
title: Установка расходного бюджета Azure для клиентов | Центр партнеров
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: В центре партнеров можно задать ежемесячный бюджет для каждого клиента, чтобы его счет Azure не выудивлен в конце месяца.
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 03901b4b17c744c0c91d732331842f6cb579bf88
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "73654068"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="894c4-103">Установка расходного бюджета Azure для клиентов</span><span class="sxs-lookup"><span data-stu-id="894c4-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="894c4-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="894c4-104">**Applies to**</span></span>

-  <span data-ttu-id="894c4-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="894c4-105">Partner Center</span></span>
-  <span data-ttu-id="894c4-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="894c4-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="894c4-107">Чтобы помочь клиентам управлять расходами на Azure, можно установить месячный бюджет расходов, чтобы счета Azure не превышали ожидаемых.</span><span class="sxs-lookup"><span data-stu-id="894c4-107">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn't higher than they anticipated.</span></span> <span data-ttu-id="894c4-108">Установка бюджета расходов Azure позволяет вам сравнивать расходы пользователей на Azure с бюджетом в течение месяца.</span><span class="sxs-lookup"><span data-stu-id="894c4-108">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="894c4-109">Возможности этой функции</span><span class="sxs-lookup"><span data-stu-id="894c4-109">With this feature, you can:</span></span> 

-   <span data-ttu-id="894c4-110">Получайте уведомления по электронной почте, если расходы клиента приближаются к ограничению бюджета</span><span class="sxs-lookup"><span data-stu-id="894c4-110">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="894c4-111">Ознакомьтесь с оценочными затратами Azure в месяц</span><span class="sxs-lookup"><span data-stu-id="894c4-111">Review your customers' estimated Azure costs per month</span></span>
-   <span data-ttu-id="894c4-112">Выявляйте неверно настроенные службы или необычные тренды использования, свидетельствующие о возможном мошенничестве</span><span class="sxs-lookup"><span data-stu-id="894c4-112">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="894c4-113">Взаимодействуйте с клиентом, чтобы определить проблему и контролировать расходы</span><span class="sxs-lookup"><span data-stu-id="894c4-113">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="894c4-114">Увеличьте бюджет, если это устраивает Вас и Ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="894c4-114">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="894c4-115">Данные о расходах в Azure приблизительны и не отражают налоги, кредиты, поправки и другие возможные взносы, поэтому фактическая сумма при выставлении счетов может отличаться.</span><span class="sxs-lookup"><span data-stu-id="894c4-115">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="894c4-116">Данные о расходах обновляются раз в день.</span><span class="sxs-lookup"><span data-stu-id="894c4-116">Spending data is refreshed once per day.</span></span> <span data-ttu-id="894c4-117">Клиенты продолжат использовать службы и ресурсы Azure (и оплачивать их), если вы не измените параметры учетной записи на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="894c4-117">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="894c4-118">Эта функция недоступна в "песочнице" или "тестирование" в рабочей учетной записи (TIP).</span><span class="sxs-lookup"><span data-stu-id="894c4-118">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="894c4-119">**Включить уведомления по электронной почте**</span><span class="sxs-lookup"><span data-stu-id="894c4-119">**Turn on email notifications**</span></span>
1.  <span data-ttu-id="894c4-120">В меню Центр партнеров выберите затраты на **Azure**.</span><span class="sxs-lookup"><span data-stu-id="894c4-120">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="894c4-121">Нажмите кнопку **Получать электронные письма**, чтобы получать уведомления, если клиенты используют 80 % своего бюджета и более.</span><span class="sxs-lookup"><span data-stu-id="894c4-121">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="894c4-122">Это поможет вам следить за своими счетами Azure.</span><span class="sxs-lookup"><span data-stu-id="894c4-122">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="894c4-123">Вы можете изменить адрес электронной почты по умолчанию для получения уведомлений на личный или любой другой адрес.</span><span class="sxs-lookup"><span data-stu-id="894c4-123">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="894c4-124">**Задание бюджета**</span><span class="sxs-lookup"><span data-stu-id="894c4-124">**Set a budget**</span></span>
1.  <span data-ttu-id="894c4-125">В меню Центр партнеров выберите затраты на **Azure**.</span><span class="sxs-lookup"><span data-stu-id="894c4-125">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="894c4-126">Выберите клиентов, для которых требуется задать бюджет.</span><span class="sxs-lookup"><span data-stu-id="894c4-126">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="894c4-127">Введите значение в поле **Ежемесячный бюджет** и выберите **Применить**.</span><span class="sxs-lookup"><span data-stu-id="894c4-127">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="894c4-128">Чтобы проверить текущие расходы, вернитесь на эту страницу.</span><span class="sxs-lookup"><span data-stu-id="894c4-128">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="894c4-129">Также можно установить отдельный бюджет для каждого клиента в разделе **Подписки с учетом использования** на странице управления клиентом.</span><span class="sxs-lookup"><span data-stu-id="894c4-129">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="894c4-130">**Удаление бюджета**</span><span class="sxs-lookup"><span data-stu-id="894c4-130">**Remove a budget**</span></span>
1.  <span data-ttu-id="894c4-131">В меню Центр партнеров выберите затраты на **Azure**.</span><span class="sxs-lookup"><span data-stu-id="894c4-131">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="894c4-132">Выберите клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="894c4-132">Select customers from the list.</span></span>
3.  <span data-ttu-id="894c4-133">Выберите **Удалить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="894c4-133">Select **Remove budget**.</span></span>

<span data-ttu-id="894c4-134">**Просмотр детализированных затрат**</span><span class="sxs-lookup"><span data-stu-id="894c4-134">**See itemized costs**</span></span>
1.  <span data-ttu-id="894c4-135">В меню Центр партнеров выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="894c4-135">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="894c4-136">Выберите клиента в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="894c4-136">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="894c4-137">Выберите подписку на странице управления клиентом в разделе **Подписки с учетом использования**.</span><span class="sxs-lookup"><span data-stu-id="894c4-137">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="894c4-138">Просмотрите текущее оценочное использование клиента и список детализированных расходов по службам.</span><span class="sxs-lookup"><span data-stu-id="894c4-138">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



