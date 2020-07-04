---
title: Миграция Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как перенести квалифицированный выпуск Dynamics 365 Business Edition в более новые версии до истечения срока их действия.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Версии Dynamics 365 предложения, продление предложений, новые номера SKU Dynamics 365
ms.openlocfilehash: e32dc8f769e9ba6299a9f7d92c5c58d85940cd94
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949639"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="8b089-104">Перенос предложений с выпуском Dynamics 365 Business в более новые версии</span><span class="sxs-lookup"><span data-stu-id="8b089-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="8b089-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="8b089-105">**Applies to**</span></span>

- <span data-ttu-id="8b089-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="8b089-106">Partner Center</span></span>

<span data-ttu-id="8b089-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="8b089-107">**Appropriate roles**</span></span>
- <span data-ttu-id="8b089-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8b089-108">Global admin</span></span>
- <span data-ttu-id="8b089-109">администратор пользователей.</span><span class="sxs-lookup"><span data-stu-id="8b089-109">User admin</span></span>
- <span data-ttu-id="8b089-110">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="8b089-110">Admin agent</span></span>
- <span data-ttu-id="8b089-111">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="8b089-111">Sales agent</span></span>

<span data-ttu-id="8b089-112">Начиная с 1 января 2019 г. клиенты с подписками Dynamics 365 Business Edition больше не смогут продлить их до этих устаревших предложений. существующие подписки не будут обновляться автоматически по истечении срока их действия.</span><span class="sxs-lookup"><span data-stu-id="8b089-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="8b089-113">На странице сведений о подписке состояние подписки изменится на "срок действия истекает через [Дата]" с "автоматическая рассылка [Дата]".</span><span class="sxs-lookup"><span data-stu-id="8b089-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="8b089-114">Чтобы обеспечить непрерывность работы для клиентов, необходимо перенести подписки с истекающим сроком действия на поддерживаемый вариант, приведенный ниже.</span><span class="sxs-lookup"><span data-stu-id="8b089-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="8b089-115">Рекомендуется переместить клиентов в новые подписки до даты окончания срока действия подписки, чтобы избежать простоев службы для клиентов.</span><span class="sxs-lookup"><span data-stu-id="8b089-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="8b089-116">Если вы используете API (CREST или центр партнеров), вы можете найти подписки с истекающим сроком действия, оценивая дату окончания подписки вместе со свойством автоматического продления = false.</span><span class="sxs-lookup"><span data-stu-id="8b089-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="8b089-117">Для подписок в вопросе будет задано автоматическое продление = false в 1 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b089-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="8b089-118">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="8b089-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="8b089-119">Прекращение использования выпусков Dynamics 365 Business</span><span class="sxs-lookup"><span data-stu-id="8b089-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="8b089-120">Dynamics 365 for Finance and Operations (выпуск для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="8b089-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="8b089-121">Dynamics 365 for Team Members (выпуск для бизнеса).</span><span class="sxs-lookup"><span data-stu-id="8b089-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="8b089-122">Dynamics Business Central — новые предложения Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="8b089-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="8b089-123">Благодаря новым предложениям Dynamics Business Central клиенты могут подключаться к своим финансовым данным, продажам, службам и операциям для упрощения бизнес-процессов, улучшения взаимодействия с клиентами и принятия лучших решений.</span><span class="sxs-lookup"><span data-stu-id="8b089-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="8b089-124">Dynamics 365 Business Central — это облачная служба, доступная только по партнерам по программе поставщика облачных решений (CSP).</span><span class="sxs-lookup"><span data-stu-id="8b089-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="8b089-125">Клиенты Dynamics 365 Business Edition имеют право на получение цены на переход с скидкой на новые предложения для бизнеса до 30 июня 2020.</span><span class="sxs-lookup"><span data-stu-id="8b089-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8b089-126">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="8b089-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="8b089-127">Чтобы переместить клиентов из выпущенных номеров SKU в более новые, необходимо выполнить следующие действия в следующем порядке:</span><span class="sxs-lookup"><span data-stu-id="8b089-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="8b089-128">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="8b089-128">Purchase the new subscription</span></span>
- <span data-ttu-id="8b089-129">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="8b089-129">Reassign current user licenses</span></span>
- <span data-ttu-id="8b089-130">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="8b089-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="8b089-131">Приобретите новый план для клиента</span><span class="sxs-lookup"><span data-stu-id="8b089-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="8b089-132">В левой панели навигации выберите **Клиенты** , а затем выберите клиента, которого нужно переместить в новую подписку.</span><span class="sxs-lookup"><span data-stu-id="8b089-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="8b089-133">Выберите **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="8b089-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="8b089-134">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="8b089-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="8b089-135">Теперь у вашего клиента есть старая подписка и новая.</span><span class="sxs-lookup"><span data-stu-id="8b089-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="8b089-136">Следующий шаг — переназначить лицензии пользователям клиента.</span><span class="sxs-lookup"><span data-stu-id="8b089-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="8b089-137">В левой панели навигации выберите **Клиенты** , а затем выберите перемещаемый клиент.</span><span class="sxs-lookup"><span data-stu-id="8b089-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8b089-138">Выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="8b089-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="8b089-139">Чтобы переназначить лицензию пользователю, выберите пользователя и нажмите кнопку **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="8b089-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="8b089-140">На странице **Управление лицензиями** снимите флажок Dynamics 365 для плана участия в продаже/клиенте в соответствии с базовым (квалифицированным предложением) лицензией и выберите новый план обслуживания для подписки, в которую будет перемещен клиент.</span><span class="sxs-lookup"><span data-stu-id="8b089-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="8b089-141">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="8b089-141">Select **Submit**.</span></span> <span data-ttu-id="8b089-142">Это будет сделано для каждого пользователя, которому требуется новая лицензия.</span><span class="sxs-lookup"><span data-stu-id="8b089-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="8b089-143">После переноса лицензий на новую подписку можно отменить старую подписку.</span><span class="sxs-lookup"><span data-stu-id="8b089-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="8b089-144">В левой панели навигации выберите **Клиенты** , а затем выберите перемещаемый клиент.</span><span class="sxs-lookup"><span data-stu-id="8b089-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8b089-145">На странице сведения о подписке установите для старой подписки значение **приостановлено** и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="8b089-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="8b089-146">Старая подписка теперь приостановлена, и Новая Подписка активна.</span><span class="sxs-lookup"><span data-stu-id="8b089-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="8b089-147">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="8b089-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="8b089-148">Ваш клиент не потребует дополнительных затрат на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="8b089-148">Your customer will incur no additional costs for the old subscription.</span></span>
