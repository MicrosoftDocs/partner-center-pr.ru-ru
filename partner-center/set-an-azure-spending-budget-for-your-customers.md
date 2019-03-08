---
title: Установка расходного бюджета Azure для клиентов | Центр партнеров
ms.topic: article
ms.date: 10/29/2018
description: В Центре партнеров вы можете устанавливать ежемесячный бюджет для каждого клиента, чтобы сумма ежемесячных счетов клиентов в Azure не оказалась чрезмерно высокой.
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 3158679d8a435a8252ad7dfb60d5cccc5cfa2f1f
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587587"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="75b5a-103">Установка расходного бюджета Azure для клиентов</span><span class="sxs-lookup"><span data-stu-id="75b5a-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="75b5a-104">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="75b5a-104">**Applies to**</span></span>

-  <span data-ttu-id="75b5a-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="75b5a-105">Partner Center</span></span>
-  <span data-ttu-id="75b5a-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="75b5a-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="75b5a-107">Чтобы помочь пользователям управлять их расходами в Azure, вы можете задать ежемесячный бюджет, чтобы счет за использование Azure не превышал указанную сумму.</span><span class="sxs-lookup"><span data-stu-id="75b5a-107">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="75b5a-108">Установка бюджета расходов Azure позволяет вам сравнивать расходы пользователей на Azure с бюджетом в течение месяца.</span><span class="sxs-lookup"><span data-stu-id="75b5a-108">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="75b5a-109">Возможности этой функции</span><span class="sxs-lookup"><span data-stu-id="75b5a-109">With this feature, you can:</span></span> 

-   <span data-ttu-id="75b5a-110">Получайте уведомления по электронной почте, если расходы клиента приближаются к ограничению бюджета</span><span class="sxs-lookup"><span data-stu-id="75b5a-110">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="75b5a-111">Просматривайте приблизительные расходы своих клиентов на Azure в месяц</span><span class="sxs-lookup"><span data-stu-id="75b5a-111">Review your customers’ estimated Azure costs per month</span></span>
-   <span data-ttu-id="75b5a-112">Выявляйте неверно настроенные службы или необычные тренды использования, свидетельствующие о возможном мошенничестве</span><span class="sxs-lookup"><span data-stu-id="75b5a-112">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="75b5a-113">Взаимодействуйте с клиентом, чтобы определить проблему и контролировать расходы</span><span class="sxs-lookup"><span data-stu-id="75b5a-113">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="75b5a-114">Увеличьте бюджет, если это устраивает Вас и Ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="75b5a-114">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="75b5a-115">Данные о расходах в Azure приблизительны и не отражают налоги, кредиты, поправки и другие возможные взносы, поэтому фактическая сумма при выставлении счетов может отличаться.</span><span class="sxs-lookup"><span data-stu-id="75b5a-115">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="75b5a-116">Данные о расходах обновляются раз в день.</span><span class="sxs-lookup"><span data-stu-id="75b5a-116">Spending data is refreshed once per day.</span></span> <span data-ttu-id="75b5a-117">Клиенты продолжат использовать службы и ресурсы Azure (и оплачивать их), если вы не измените параметры учетной записи на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="75b5a-117">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="75b5a-118">Эта функция не доступна в «песочницу» или тестирования в рабочей среде (TIP) учетных записей.</span><span class="sxs-lookup"><span data-stu-id="75b5a-118">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="75b5a-119">**Включить уведомления по электронной почте**</span><span class="sxs-lookup"><span data-stu-id="75b5a-119">**Turn on email notifications**</span></span>
1.  <span data-ttu-id="75b5a-120">В меню центра партнеров выберите **издержки на Azure**.</span><span class="sxs-lookup"><span data-stu-id="75b5a-120">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="75b5a-121">Нажмите кнопку **Получать электронные письма**, чтобы получать уведомления, если клиенты используют 80 % своего бюджета и более.</span><span class="sxs-lookup"><span data-stu-id="75b5a-121">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="75b5a-122">Это поможет вам следить за своими счетами Azure.</span><span class="sxs-lookup"><span data-stu-id="75b5a-122">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="75b5a-123">Вы можете изменить адрес электронной почты по умолчанию для получения уведомлений на личный или любой другой адрес.</span><span class="sxs-lookup"><span data-stu-id="75b5a-123">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="75b5a-124">**Установка бюджета**</span><span class="sxs-lookup"><span data-stu-id="75b5a-124">**Set a budget**</span></span>
1.  <span data-ttu-id="75b5a-125">В меню центра партнеров выберите **издержки на Azure**.</span><span class="sxs-lookup"><span data-stu-id="75b5a-125">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="75b5a-126">Выберите клиентов, для которых требуется задать бюджет.</span><span class="sxs-lookup"><span data-stu-id="75b5a-126">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="75b5a-127">Введите значение в поле **Ежемесячный бюджет** и выберите **Применить**.</span><span class="sxs-lookup"><span data-stu-id="75b5a-127">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="75b5a-128">Чтобы проверить текущие расходы, вернитесь на эту страницу.</span><span class="sxs-lookup"><span data-stu-id="75b5a-128">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="75b5a-129">Также можно установить отдельный бюджет для каждого клиента в разделе **Подписки с учетом использования** на странице управления клиентом.</span><span class="sxs-lookup"><span data-stu-id="75b5a-129">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="75b5a-130">**Удаление бюджета**</span><span class="sxs-lookup"><span data-stu-id="75b5a-130">**Remove a budget**</span></span>
1.  <span data-ttu-id="75b5a-131">В меню центра партнеров выберите **издержки на Azure**.</span><span class="sxs-lookup"><span data-stu-id="75b5a-131">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="75b5a-132">Выберите клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="75b5a-132">Select customers from the list.</span></span>
3.  <span data-ttu-id="75b5a-133">Выберите **Удалить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="75b5a-133">Select **Remove budget**.</span></span>

<span data-ttu-id="75b5a-134">**Просмотр детализированных затрат**</span><span class="sxs-lookup"><span data-stu-id="75b5a-134">**See itemized costs**</span></span>
1.  <span data-ttu-id="75b5a-135">В меню центра партнеров выберите **клиентов**.</span><span class="sxs-lookup"><span data-stu-id="75b5a-135">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="75b5a-136">Выберите клиента в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="75b5a-136">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="75b5a-137">Выберите подписку на странице управления клиентом в разделе **Подписки с учетом использования**.</span><span class="sxs-lookup"><span data-stu-id="75b5a-137">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="75b5a-138">Просмотрите текущее оценочное использование клиента и список детализированных расходов по службам.</span><span class="sxs-lookup"><span data-stu-id="75b5a-138">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



