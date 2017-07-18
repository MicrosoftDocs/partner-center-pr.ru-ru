---
title: "Установка расходного бюджета Azure для клиентов | Центр партнеров"
description: "В Центре партнеров вы можете устанавливать ежемесячный бюджет для каждого клиента, чтобы сумма ежемесячных счетов клиентов в Azure не оказалась чрезмерно высокой."
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.openlocfilehash: 873190885d83f70f6ff68e277f288d58cc74ca00
ms.sourcegitcommit: 0b00306bfb0b406e64ad857cb360de4533740e6a
ms.translationtype: HT
ms.contentlocale: ru-RU
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="b4726-103">Установка расходного бюджета Azure для клиентов</span><span class="sxs-lookup"><span data-stu-id="b4726-103">Set an Azure spending budget for your customers</span></span>

**<span data-ttu-id="b4726-104">Относится к:</span><span class="sxs-lookup"><span data-stu-id="b4726-104">Applies to</span></span>**

-  <span data-ttu-id="b4726-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="b4726-105">Partner Center</span></span>
-  <span data-ttu-id="b4726-106">Центр партнеров для Microsoft Cloud для правительства США</span><span class="sxs-lookup"><span data-stu-id="b4726-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="b4726-107">Центр партнеров Microsoft Cloud для Германии</span><span class="sxs-lookup"><span data-stu-id="b4726-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="b4726-108">Чтобы помочь пользователям управлять их расходами в Azure, вы можете задать ежемесячный бюджет, чтобы счет за использование Azure не превышал указанную сумму.</span><span class="sxs-lookup"><span data-stu-id="b4726-108">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="b4726-109">Установка бюджета расходов Azure позволяет вам сравнивать расходы пользователей на Azure с бюджетом в течение месяца.</span><span class="sxs-lookup"><span data-stu-id="b4726-109">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="b4726-110">Возможности этой функции</span><span class="sxs-lookup"><span data-stu-id="b4726-110">With this feature, you can:</span></span> 

-   <span data-ttu-id="b4726-111">Получайте уведомления по электронной почте, если расходы клиента приближаются к ограничению бюджета.</span><span class="sxs-lookup"><span data-stu-id="b4726-111">Be notified by email if a customer's spending is near the budget limit.</span></span>
-   <span data-ttu-id="b4726-112">Просматривайте приблизительные расходы своих клиентов на Azure в месяц.</span><span class="sxs-lookup"><span data-stu-id="b4726-112">Review your customers’ estimated Azure costs per month.</span></span>
-   <span data-ttu-id="b4726-113">Выявляйте неверно настроенные службы или необычные тренды использования, свидетельствующие о возможном мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="b4726-113">Spot a misconfigured service, or unusual usage trends that might suggest fraud.</span></span>
-   <span data-ttu-id="b4726-114">Взаимодействуйте с клиентом, чтобы определить проблему и контролировать расходы.</span><span class="sxs-lookup"><span data-stu-id="b4726-114">Work with the customer to identify the root issue and manage costs.</span></span>
-   <span data-ttu-id="b4726-115">Увеличьте бюджет, если это устраивает Вас и Ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="b4726-115">Change the budget to a higher amount if you and your customer are comfortable with it.</span></span>

<span data-ttu-id="b4726-116">Данные о расходах в Azure приблизительны и не отражают налоги, кредиты, поправки и другие возможные взносы, поэтому фактическая сумма при выставлении счетов может отличаться.</span><span class="sxs-lookup"><span data-stu-id="b4726-116">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="b4726-117">Данные о расходах обновляются раз в день.</span><span class="sxs-lookup"><span data-stu-id="b4726-117">Spending data is refreshed once per day.</span></span> <span data-ttu-id="b4726-118">Клиенты продолжат использовать службы и ресурсы Azure (и оплачивать их), если вы не измените параметры учетной записи на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b4726-118">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

><span data-ttu-id="b4726-119">**Примечание.** Эта функция недоступна в «песочнице» или для учетных записей тестирования в рабочей среде (TIP).</span><span class="sxs-lookup"><span data-stu-id="b4726-119">**Note**   This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

**<span data-ttu-id="b4726-120">Включение уведомлений по электронной почте</span><span class="sxs-lookup"><span data-stu-id="b4726-120">Turn on email notifications</span></span>**

1.  <span data-ttu-id="b4726-121">В меню «Информационная панель» выберите **Расходы в Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="b4726-121">From the Dashboard menu, select **Microsoft Azure spending**.</span></span>
2.  <span data-ttu-id="b4726-122">Нажмите кнопку **Получать электронные письма**, чтобы получать уведомления, если клиенты используют 80% своего бюджета и более.</span><span class="sxs-lookup"><span data-stu-id="b4726-122">Click the **Get emails** button to be notified if your customers use 80% or more of their budget.</span></span> <span data-ttu-id="b4726-123">Это поможет вам следить за своими счетами Azure.</span><span class="sxs-lookup"><span data-stu-id="b4726-123">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="b4726-124">Вы можете изменить адрес электронной почты по умолчанию для получения уведомлений на личный или любой другой адрес.</span><span class="sxs-lookup"><span data-stu-id="b4726-124">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="b4726-125"><a href="" id="setabudget"></a>
**Установка бюджета**</span><span class="sxs-lookup"><span data-stu-id="b4726-125"><a href="" id="setabudget"></a>
**Set a budget**</span></span>

1.  <span data-ttu-id="b4726-126">В меню «Информационная панель» выберите **Расходы в Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="b4726-126">From the Dashboard menu, select **Microsoft Azure spending**.</span></span>
2.  <span data-ttu-id="b4726-127">Выберите клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="b4726-127">Select customers from the list.</span></span>
3.  <span data-ttu-id="b4726-128">Введите значение в поле **Ежемесячный бюджет** и выберите **Применить**.</span><span class="sxs-lookup"><span data-stu-id="b4726-128">Enter a value in the **Monthly budget** field and select **Apply**.</span></span>
4.  <span data-ttu-id="b4726-129">Чтобы проверить текущие расходы, вернитесь на эту страницу.</span><span class="sxs-lookup"><span data-stu-id="b4726-129">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="b4726-130">Также можно установить отдельный бюджет для каждого клиента в разделе **Подписки с учетом использования** на странице управления клиентом.</span><span class="sxs-lookup"><span data-stu-id="b4726-130">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="b4726-131"><a href="" id="removeabudget"></a>
**Удаление бюджета**</span><span class="sxs-lookup"><span data-stu-id="b4726-131"><a href="" id="removeabudget"></a>
**Remove a budget**</span></span>

1.  <span data-ttu-id="b4726-132">В меню «Информационная панель» выберите **Расходы в Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="b4726-132">From the Dashboard menu, select **Microsoft Azure spending**.</span></span>
2.  <span data-ttu-id="b4726-133">Выберите клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="b4726-133">Select customers from the list.</span></span>
3.  <span data-ttu-id="b4726-134">Выберите **Удалить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="b4726-134">Select **Remove budget**.</span></span>

<span data-ttu-id="b4726-135"><a href="" id="seeitemizedcosts"></a>
**Просмотр детализированных расходов**</span><span class="sxs-lookup"><span data-stu-id="b4726-135"><a href="" id="seeitemizedcosts"></a>
**See itemized costs**</span></span>

1.  <span data-ttu-id="b4726-136">В меню панели мониторинга выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="b4726-136">From the Dashboard menu, select **Customers**.</span></span>
2.  <span data-ttu-id="b4726-137">Выберите клиента в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="b4726-137">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="b4726-138">Выберите подписку на странице управления клиентом в разделе **Подписки с учетом использования**.</span><span class="sxs-lookup"><span data-stu-id="b4726-138">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="b4726-139">Просмотрите текущее оценочное использование клиента и список детализированных расходов по службам.</span><span class="sxs-lookup"><span data-stu-id="b4726-139">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



