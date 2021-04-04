---
title: Перенос подходящих подписок Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как перейти от квалифицированных подписок Dynamics 365 к новой подписке до истечения срока действия подписок.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132746"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="d4fa6-103">Перенос Dynamics 365 и плана Customer Engagement с "Базового" уровня (соответствующие предложения) в более новые версии</span><span class="sxs-lookup"><span data-stu-id="d4fa6-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="d4fa6-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="d4fa6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d4fa6-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d4fa6-105">Global admin</span></span>
- <span data-ttu-id="d4fa6-106">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="d4fa6-106">User management admin</span></span>
- <span data-ttu-id="d4fa6-107">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="d4fa6-107">Admin agent</span></span>
- <span data-ttu-id="d4fa6-108">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="d4fa6-108">Sales agent</span></span>

<span data-ttu-id="d4fa6-109">Начиная с 1 января 2019 г. клиенты с Dynamics 365 для плана участия в продаже или клиенте по плану "базовый" (квалифицированные предложения) больше не могут обновлять эти предложения прежних версий. существующие подписки не будут обновляться автоматически по истечении срока их действия.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="d4fa6-110">На странице сведений о подписке состояние подписки изменится на "срок действия истекает через [Дата]" с "автоматическая рассылка [Дата]".</span><span class="sxs-lookup"><span data-stu-id="d4fa6-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="d4fa6-111">Чтобы обеспечить непрерывность работы для клиентов, необходимо перенести подписки с истекающим сроком действия на поддерживаемый вариант, приведенный ниже.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="d4fa6-112">Рекомендуется переместить клиентов в новые подписки до даты окончания срока действия подписки, чтобы избежать простоев службы для клиентов.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="d4fa6-113">Если вы используете API (CREST или центр партнеров), вы можете найти подписки с истекающим сроком действия, оценивая дату окончания подписки вместе со свойством автоматического продления = false.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="d4fa6-114">Для подписок в вопросе будет задано автоматическое продление = false в 1 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="d4fa6-115">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="d4fa6-116">Предложения Dynamics 365 будут прекращены</span><span class="sxs-lookup"><span data-stu-id="d4fa6-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="d4fa6-117">Dynamics 365 для Sales Enterprise Edition КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-118">Dynamics 365 для Sales Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="d4fa6-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4fa6-119">Dynamics 365 для Sales Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="d4fa6-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4fa6-120">Dynamics 365 для продаж Enterprise Edition (правительственные цены) КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-121">Dynamics 365 для продажи Enterprise Edition из SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-122">Dynamics 365 для продажи Enterprise Edition от SA для CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="d4fa6-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4fa6-123">Dynamics 365 для продажи Enterprise Edition от SA для CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="d4fa6-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4fa6-124">Dynamics 365 для продаж Enterprise Edition (стоимость государственных организаций) от SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-125">Dynamics 365 для Sales Enterprise Edition Add-On для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-126">Dynamics 365 для Sales Enterprise Edition Add-On для CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="d4fa6-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4fa6-127">Dynamics 365 для Sales Enterprise Edition Add-On для CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="d4fa6-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4fa6-128">Dynamics 365 для продаж Enterprise Edition (стоимость государственных организаций) Add-On для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-129">Dynamics 365 клиент в плане участия Enterprise Edition КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-130">Dynamics 365 клиент в плане взаимодействия с Enterprise Edition (стоимость государственных организаций) КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-131">Dynamics 365 клиент в плане участия Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="d4fa6-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4fa6-132">Dynamics 365 клиент в плане участия Enterprise Edition КРМОЛ Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="d4fa6-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4fa6-133">Dynamics 365 клиент в плане участия в корпоративном выпуске из SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-134">План взаимодействия клиента Dynamics 365 Enterprise Edition (стоимость государственных организаций) от SA для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-135">Dynamics 365 клиентское взаимодействие план Enterprise Edition от SA для CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="d4fa6-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4fa6-136">Dynamics 365 клиент в плане участия в корпоративном выпуске SA для CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="d4fa6-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4fa6-137">Dynamics 365 клиент в плане участия в корпоративном выпуске Add-On для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-138">Корпоративный 365. план взаимодействия клиентов Enterprise Edition (ценообразование для государственных организаций) Add-On для CRM Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-139">Dynamics 365 клиент в плане участия Enterprise Edition Add-On для CRM Basic (квалифицированное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="d4fa6-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4fa6-140">Dynamics 365 клиент в плане участия в корпоративном выпуске Add-On для CRM Basic (квалифицированное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="d4fa6-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="d4fa6-141">Dynamics 365 для плана участия в продажах и клиентах из базовых (квалифицированных предложений) планов замены</span><span class="sxs-lookup"><span data-stu-id="d4fa6-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="d4fa6-142">**Отмененные предложения**</span><span class="sxs-lookup"><span data-stu-id="d4fa6-142">**Retired offers**</span></span>   

- <span data-ttu-id="d4fa6-143">Dynamics 365 для продаж из CRM Basic или КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4fa6-144">План взаимодействия с клиентами Dynamics 365 из CRM Basic или КРМОЛ Basic (квалифицированное предложение)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="d4fa6-145">**Параметры замены**</span><span class="sxs-lookup"><span data-stu-id="d4fa6-145">**Replacement options**</span></span>
- <span data-ttu-id="d4fa6-146">Dynamics 365 для специалистов по продажам (впервые)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d4fa6-147">Dynamics 365 для специалистов по продажам (впервые)</span><span class="sxs-lookup"><span data-stu-id="d4fa6-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d4fa6-148">Dynamics 365 for Customer Service;</span><span class="sxs-lookup"><span data-stu-id="d4fa6-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="d4fa6-149">План участия клиента Dynamics 365 или</span><span class="sxs-lookup"><span data-stu-id="d4fa6-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="d4fa6-150">Члены команды Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d4fa6-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="d4fa6-151">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="d4fa6-151">Transition customers to new product plans</span></span>

<span data-ttu-id="d4fa6-152">Чтобы переместить клиентов из выпущенных номеров SKU в более новые, необходимо выполнить следующие действия в следующем порядке:</span><span class="sxs-lookup"><span data-stu-id="d4fa6-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="d4fa6-153">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="d4fa6-153">Purchase the new subscription</span></span>
- <span data-ttu-id="d4fa6-154">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="d4fa6-154">Reassign current user licenses</span></span>
- <span data-ttu-id="d4fa6-155">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="d4fa6-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="d4fa6-156">Приобретите новый план для клиента</span><span class="sxs-lookup"><span data-stu-id="d4fa6-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="d4fa6-157">В левой панели навигации выберите **Клиенты** , а затем выберите клиента, которого нужно переместить в новую подписку.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="d4fa6-158">Выберите **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="d4fa6-159">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="d4fa6-160">Теперь у вашего клиента есть старая подписка и новая.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="d4fa6-161">Следующий шаг — переназначить лицензии пользователям клиента.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="d4fa6-162">В левой панели навигации выберите **Клиенты** , а затем выберите перемещаемый клиент.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d4fa6-163">Выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="d4fa6-164">Чтобы переназначить лицензию пользователю, выберите пользователя и нажмите кнопку **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="d4fa6-165">На странице **Управление лицензиями** снимите флажок Dynamics 365 для плана участия в продаже/клиенте в соответствии с базовым (квалифицированным предложением) лицензией и выберите новый план обслуживания для подписки, в которую будет перемещен клиент.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="d4fa6-166">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="d4fa6-166">Select **Submit**.</span></span> <span data-ttu-id="d4fa6-167">Это будет сделано для каждого пользователя, которому требуется новая лицензия.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="d4fa6-168">После переноса лицензий на новую подписку можно отменить старую подписку.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="d4fa6-169">В левой панели навигации выберите **Клиенты** , а затем выберите перемещаемый клиент.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d4fa6-170">На странице сведения о подписке установите для старой подписки значение **приостановлено** и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="d4fa6-171">Старая подписка теперь приостановлена, и Новая Подписка активна.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="d4fa6-172">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="d4fa6-173">Ваш клиент не потребует дополнительных затрат на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="d4fa6-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



