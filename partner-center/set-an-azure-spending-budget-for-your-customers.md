---
title: Установка расходного бюджета Azure для клиентов | Центр партнеров
description: В Центре партнеров вы можете устанавливать ежемесячный бюджет для каждого клиента, чтобы сумма ежемесячных счетов клиентов в Azure не оказалась чрезмерно высокой.
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 6f6e0e733aed13174dcf4d318b522723bb425b30
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2018
ms.locfileid: "4488960"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="13d49-103">Установка расходного бюджета Azure для клиентов</span><span class="sxs-lookup"><span data-stu-id="13d49-103">Set an Azure spending budget for your customers</span></span>

**<span data-ttu-id="13d49-104">Относится к:</span><span class="sxs-lookup"><span data-stu-id="13d49-104">Applies to</span></span>**

-  <span data-ttu-id="13d49-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="13d49-105">Partner Center</span></span>
-  <span data-ttu-id="13d49-106">Центр партнеров для Microsoft Cloud для правительства США</span><span class="sxs-lookup"><span data-stu-id="13d49-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="13d49-107">Центр партнеров Microsoft Cloud для Германии</span><span class="sxs-lookup"><span data-stu-id="13d49-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="13d49-108">Чтобы помочь пользователям управлять их расходами в Azure, вы можете задать ежемесячный бюджет, чтобы счет за использование Azure не превышал указанную сумму.</span><span class="sxs-lookup"><span data-stu-id="13d49-108">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="13d49-109">Установка бюджета расходов Azure позволяет вам сравнивать расходы пользователей на Azure с бюджетом в течение месяца.</span><span class="sxs-lookup"><span data-stu-id="13d49-109">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="13d49-110">Возможности этой функции</span><span class="sxs-lookup"><span data-stu-id="13d49-110">With this feature, you can:</span></span> 

-   <span data-ttu-id="13d49-111">Получайте уведомления по электронной почте, если расходы клиента приближаются к ограничению бюджета</span><span class="sxs-lookup"><span data-stu-id="13d49-111">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="13d49-112">Просматривайте приблизительные расходы своих клиентов на Azure в месяц</span><span class="sxs-lookup"><span data-stu-id="13d49-112">Review your customers’ estimated Azure costs per month</span></span>
-   <span data-ttu-id="13d49-113">Выявляйте неверно настроенные службы или необычные тренды использования, свидетельствующие о возможном мошенничестве</span><span class="sxs-lookup"><span data-stu-id="13d49-113">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="13d49-114">Взаимодействуйте с клиентом, чтобы определить проблему и контролировать расходы</span><span class="sxs-lookup"><span data-stu-id="13d49-114">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="13d49-115">Увеличьте бюджет, если это устраивает Вас и Ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="13d49-115">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="13d49-116">Данные о расходах в Azure приблизительны и не отражают налоги, кредиты, поправки и другие возможные взносы, поэтому фактическая сумма при выставлении счетов может отличаться.</span><span class="sxs-lookup"><span data-stu-id="13d49-116">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="13d49-117">Данные о расходах обновляются раз в день.</span><span class="sxs-lookup"><span data-stu-id="13d49-117">Spending data is refreshed once per day.</span></span> <span data-ttu-id="13d49-118">Клиенты продолжат использовать службы и ресурсы Azure (и оплачивать их), если вы не измените параметры учетной записи на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="13d49-118">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="13d49-119">Эта функция недоступен в «песочнице» или тестирования в рабочей среде (TIP) учетных записей.</span><span class="sxs-lookup"><span data-stu-id="13d49-119">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

**<span data-ttu-id="13d49-120">Включение уведомлений по электронной почте</span><span class="sxs-lookup"><span data-stu-id="13d49-120">Turn on email notifications</span></span>**
1.  <span data-ttu-id="13d49-121">В меню центра партнеров выберите **расходы в Azure**.</span><span class="sxs-lookup"><span data-stu-id="13d49-121">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="13d49-122">Нажмите кнопку **Получать электронные письма**, чтобы получать уведомления, если клиенты используют 80% своего бюджета и более.</span><span class="sxs-lookup"><span data-stu-id="13d49-122">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="13d49-123">Это поможет вам следить за своими счетами Azure.</span><span class="sxs-lookup"><span data-stu-id="13d49-123">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="13d49-124">Вы можете изменить адрес электронной почты по умолчанию для получения уведомлений на личный или любой другой адрес.</span><span class="sxs-lookup"><span data-stu-id="13d49-124">You can change the default email address to a personal or any other email to receive notifications.</span></span>

**<span data-ttu-id="13d49-125">Установка бюджета</span><span class="sxs-lookup"><span data-stu-id="13d49-125">Set a budget</span></span>**
1.  <span data-ttu-id="13d49-126">В меню центра партнеров выберите **расходы в Azure**.</span><span class="sxs-lookup"><span data-stu-id="13d49-126">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="13d49-127">Выберите клиентов, для которых требуется задать бюджет.</span><span class="sxs-lookup"><span data-stu-id="13d49-127">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="13d49-128">Введите значение в поле **Ежемесячный бюджет** и выберите **Применить**.</span><span class="sxs-lookup"><span data-stu-id="13d49-128">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="13d49-129">Чтобы проверить текущие расходы, вернитесь на эту страницу.</span><span class="sxs-lookup"><span data-stu-id="13d49-129">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="13d49-130">Также можно установить отдельный бюджет для каждого клиента в разделе **Подписки с учетом использования** на странице управления клиентом.</span><span class="sxs-lookup"><span data-stu-id="13d49-130">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

**<span data-ttu-id="13d49-131">Удаление бюджета</span><span class="sxs-lookup"><span data-stu-id="13d49-131">Remove a budget</span></span>**
1.  <span data-ttu-id="13d49-132">В меню центра партнеров выберите **расходы в Azure**.</span><span class="sxs-lookup"><span data-stu-id="13d49-132">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="13d49-133">Выберите клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="13d49-133">Select customers from the list.</span></span>
3.  <span data-ttu-id="13d49-134">Выберите **Удалить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="13d49-134">Select **Remove budget**.</span></span>

**<span data-ttu-id="13d49-135">Просмотр детализированных расходов</span><span class="sxs-lookup"><span data-stu-id="13d49-135">See itemized costs</span></span>**
1.  <span data-ttu-id="13d49-136">В меню центра партнеров выберите **клиентов**.</span><span class="sxs-lookup"><span data-stu-id="13d49-136">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="13d49-137">Выберите клиента в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="13d49-137">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="13d49-138">Выберите подписку на странице управления клиентом в разделе **Подписки с учетом использования**.</span><span class="sxs-lookup"><span data-stu-id="13d49-138">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="13d49-139">Просмотрите текущее оценочное использование клиента и список детализированных расходов по службам.</span><span class="sxs-lookup"><span data-stu-id="13d49-139">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



