---
title: Перенос подходящих подписок Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как перейти от квалифицированных подписок Dynamics 365 к новой подписке до истечения срока действия подписок.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Версии Dynamics 365 предложения, продление предложений, новые номера SKU Dynamics 365
ms.openlocfilehash: 1fb7a58d3c777f39bdd3594d6d2bc0be04fbf573
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992099"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="884bc-104">Перенос Dynamics 365 и плана Customer Engagement с "Базового" уровня (соответствующие предложения) в более новые версии</span><span class="sxs-lookup"><span data-stu-id="884bc-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="884bc-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="884bc-105">**Applies to**</span></span>

-  <span data-ttu-id="884bc-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="884bc-106">Partner Center</span></span>

<span data-ttu-id="884bc-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="884bc-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="884bc-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="884bc-108">Global admin</span></span>
-   <span data-ttu-id="884bc-109">администратор пользователей.</span><span class="sxs-lookup"><span data-stu-id="884bc-109">User admin</span></span>
-   <span data-ttu-id="884bc-110">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="884bc-110">Admin agent</span></span>
-   <span data-ttu-id="884bc-111">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="884bc-111">Sales agent</span></span>

<span data-ttu-id="884bc-112">Начиная с 1 января 2019 г. клиенты с Dynamics 365 для плана участия в продаже или клиенте по плану "базовый" (квалифицированные предложения) больше не могут обновлять эти предложения прежних версий. существующие подписки не будут обновляться автоматически по истечении срока их действия.</span><span class="sxs-lookup"><span data-stu-id="884bc-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="884bc-113">На странице сведений о подписке состояние подписки изменится на "срок действия истекает через [Дата]" с "автоматическая рассылка [Дата]".</span><span class="sxs-lookup"><span data-stu-id="884bc-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="884bc-114">Чтобы обеспечить непрерывность работы для клиентов, необходимо перенести подписки с истекающим сроком действия на поддерживаемый вариант, приведенный ниже.</span><span class="sxs-lookup"><span data-stu-id="884bc-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="884bc-115">Рекомендуется переместить клиентов в новые подписки до даты окончания срока действия подписки, чтобы избежать простоев службы для клиентов.</span><span class="sxs-lookup"><span data-stu-id="884bc-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="884bc-116">Если вы используете API (CREST или центр партнеров), вы можете найти подписки с истекающим сроком действия, оценивая дату окончания подписки вместе со свойством автоматического продления = false.</span><span class="sxs-lookup"><span data-stu-id="884bc-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="884bc-117">Для подписок в вопросе будет задано автоматическое продление = false в 1 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="884bc-118">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="884bc-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="884bc-119">Предложения Dynamics 365 будут прекращены</span><span class="sxs-lookup"><span data-stu-id="884bc-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="884bc-120">Dynamics 365 для Sales Enterprise Edition КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-121">Dynamics 365 для Sales Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="884bc-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="884bc-122">Dynamics 365 для Sales Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="884bc-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="884bc-123">Dynamics 365 для продаж Enterprise Edition (правительственные цены) КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-124">Dynamics 365 для продажи Enterprise Edition из SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-125">Dynamics 365 для продажи Enterprise Edition от SA для CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="884bc-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="884bc-126">Dynamics 365 для продажи Enterprise Edition от SA для CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="884bc-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="884bc-127">Dynamics 365 для продаж Enterprise Edition (стоимость государственных организаций) от SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-128">Надстройка Dynamics 365 для Sales Enterprise Edition для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-129">Надстройка Dynamics 365 для Sales Enterprise Edition для CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="884bc-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="884bc-130">Надстройка Dynamics 365 для Sales Enterprise Edition для CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="884bc-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="884bc-131">Надстройка Dynamics 365 для продажи Enterprise Edition (правительственные цены) для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-132">Dynamics 365 клиент в плане участия Enterprise Edition КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-133">Dynamics 365 клиент в плане взаимодействия с Enterprise Edition (стоимость государственных организаций) КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-134">Dynamics 365 клиент в плане участия Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="884bc-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="884bc-135">Dynamics 365 клиент в плане участия Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="884bc-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="884bc-136">Dynamics 365 клиент в плане участия в корпоративном выпуске из SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-137">План взаимодействия клиента Dynamics 365 Enterprise Edition (стоимость государственных организаций) от SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-138">Dynamics 365 клиентское взаимодействие план Enterprise Edition от SA для CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="884bc-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="884bc-139">Dynamics 365 клиент в плане участия в корпоративном выпуске SA для CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="884bc-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="884bc-140">Надстройка Enterprise Edition с планом обслуживания клиентов Dynamics 365 для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-141">Надстройка клиента Dynamics 365 с планом выпуска Enterprise Edition (ценообразование для государственных организаций) для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-142">Надстройка Enterprise Edition с планом обслуживания клиентов Dynamics 365 для служб CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="884bc-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="884bc-143">Надстройка Enterprise Edition с планом обслуживания клиентов Dynamics 365 для выпуска CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="884bc-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="884bc-144">Dynamics 365 для плана участия в продажах и клиентах из базовых (квалифицированных предложений) планов замены</span><span class="sxs-lookup"><span data-stu-id="884bc-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="884bc-145">**Отмененные предложения**</span><span class="sxs-lookup"><span data-stu-id="884bc-145">**Retired offers**</span></span>   

- <span data-ttu-id="884bc-146">Dynamics 365 для продаж из CRM Basic или КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="884bc-147">План взаимодействия с клиентами Dynamics 365 из CRM Basic или КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="884bc-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="884bc-148">**Параметры замены**</span><span class="sxs-lookup"><span data-stu-id="884bc-148">**Replacement options**</span></span>
- <span data-ttu-id="884bc-149">Dynamics 365 для специалистов по продажам (впервые)</span><span class="sxs-lookup"><span data-stu-id="884bc-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="884bc-150">Dynamics 365 для специалистов по продажам (впервые)</span><span class="sxs-lookup"><span data-stu-id="884bc-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="884bc-151">Dynamics 365 for Customer Service;</span><span class="sxs-lookup"><span data-stu-id="884bc-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="884bc-152">План участия клиента Dynamics 365 или</span><span class="sxs-lookup"><span data-stu-id="884bc-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="884bc-153">Члены команды Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="884bc-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="884bc-154">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="884bc-154">Transition customers to new product plans</span></span>

<span data-ttu-id="884bc-155">Чтобы переместить клиентов из выпущенных номеров SKU в более новые, необходимо выполнить следующие действия в следующем порядке:</span><span class="sxs-lookup"><span data-stu-id="884bc-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="884bc-156">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="884bc-156">Purchase the new subscription</span></span>
- <span data-ttu-id="884bc-157">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="884bc-157">Reassign current user licenses</span></span>
- <span data-ttu-id="884bc-158">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="884bc-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="884bc-159">Приобретите новый план для клиента</span><span class="sxs-lookup"><span data-stu-id="884bc-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="884bc-160">В левой панели навигации выберите **Клиенты** , а затем выберите клиента, которого нужно переместить в новую подписку.</span><span class="sxs-lookup"><span data-stu-id="884bc-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="884bc-161">Выберите **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="884bc-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="884bc-162">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="884bc-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="884bc-163">Теперь у вашего клиента есть старая подписка и новая.</span><span class="sxs-lookup"><span data-stu-id="884bc-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="884bc-164">Следующий шаг — переназначить лицензии пользователям клиента.</span><span class="sxs-lookup"><span data-stu-id="884bc-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="884bc-165">В левой панели навигации выберите **Клиенты** , а затем выберите перемещаемый клиент.</span><span class="sxs-lookup"><span data-stu-id="884bc-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="884bc-166">Выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="884bc-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="884bc-167">Чтобы переназначить лицензию пользователю, выберите пользователя и нажмите кнопку **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="884bc-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="884bc-168">На странице **Управление лицензиями** снимите флажок Dynamics 365 для плана участия в продаже/клиенте в соответствии с базовым (квалифицированным предложением) лицензией и выберите новый план обслуживания для подписки, в которую будет перемещен клиент.</span><span class="sxs-lookup"><span data-stu-id="884bc-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="884bc-169">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="884bc-169">Select **Submit**.</span></span> <span data-ttu-id="884bc-170">Это будет сделано для каждого пользователя, которому требуется новая лицензия.</span><span class="sxs-lookup"><span data-stu-id="884bc-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="884bc-171">После переноса лицензий на новую подписку можно отменить старую подписку.</span><span class="sxs-lookup"><span data-stu-id="884bc-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="884bc-172">В левой панели навигации выберите **Клиенты** , а затем выберите перемещаемый клиент.</span><span class="sxs-lookup"><span data-stu-id="884bc-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="884bc-173">На странице сведения о подписке установите для старой подписки значение **приостановлено** и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="884bc-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="884bc-174">Старая подписка теперь приостановлена, и Новая Подписка активна.</span><span class="sxs-lookup"><span data-stu-id="884bc-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="884bc-175">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="884bc-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="884bc-176">Ваш клиент не потребует дополнительных затрат на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="884bc-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



