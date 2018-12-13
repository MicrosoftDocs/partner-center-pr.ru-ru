---
title: Перенос Dynamics 365 и Customer Engagement Plan из Basic (полное предложения) новые версии | Центр партнеров
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement Plan Basic (полное предлагает) подписок на могут больше не будут обновлены.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968274"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="05a90-103">Перенос Dynamics 365 и Customer Engagement Plan из Basic (полное предложения) новые версии</span><span class="sxs-lookup"><span data-stu-id="05a90-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="05a90-104">Область применения</span><span class="sxs-lookup"><span data-stu-id="05a90-104">Applies to</span></span>**

-  <span data-ttu-id="05a90-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="05a90-105">Partner Center</span></span>

<span data-ttu-id="05a90-106">Эффективные 1 января 2019 г клиентов Dynamics 365 for Sales / Customer Engagement Plan Basic (полное предлагает) подписок на больше не может обновить эти устаревшие предложений; существующие подписки не будут продлеваться автоматически, когда истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="05a90-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="05a90-107">На странице сведений подписки состояние подписки поменяется на «Срок действия [дата]» «Автоматического возобновления: [дата]».</span><span class="sxs-lookup"><span data-stu-id="05a90-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="05a90-108">Чтобы обеспечить непрерывность для пользователей, следует перенести пользователей с истекающим сроком действия подписки на поддерживаемый вариант, перечисленные ниже.</span><span class="sxs-lookup"><span data-stu-id="05a90-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="05a90-109">Мы рекомендуем переводить клиентов на новые подписки до ежегодной даты завершения подписки, чтобы не допускать перерывов в предоставлении службы клиентам.</span><span class="sxs-lookup"><span data-stu-id="05a90-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="05a90-110">Если вы используете API (CREST или центра партнеров), вы можете найти подписки с истекающим сроком действия по дате завершения подписки автоматически = False свойства.</span><span class="sxs-lookup"><span data-stu-id="05a90-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="05a90-111">Рассматриваемый подписок будет установлено значение auto renew = "false" 1 января 2019 года.</span><span class="sxs-lookup"><span data-stu-id="05a90-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="05a90-112">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="05a90-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="05a90-113">Dynamics 365 предлагает выполнится успешно.</span><span class="sxs-lookup"><span data-stu-id="05a90-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="05a90-114">Dynamics 365 для продажи Enterprise Edition CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-115">Dynamics 365 для продажи Enterprise Edition CRMOL Basic (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="05a90-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="05a90-116">Dynamics 365 для продажи Enterprise Edition CRMOL Basic (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="05a90-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="05a90-117">Dynamics 365 для продажи Enterprise Edition (цены США) CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-118">Dynamics 365 для продажи Enterprise Edition с SA для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-119">Dynamics 365 для продажи Enterprise Edition с SA для CRM Basic (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="05a90-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="05a90-120">Dynamics 365 для продажи Enterprise Edition с SA для CRM Basic (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="05a90-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="05a90-121">Dynamics 365 для продажи Enterprise Edition (цены США) из SA для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-122">Dynamics 365 для продажи Enterprise Edition надстройки для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-123">Dynamics 365 для продажи Enterprise Edition надстройки для CRM Basic (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="05a90-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="05a90-124">Dynamics 365 для продажи Enterprise Edition надстройки для CRM Basic (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="05a90-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="05a90-125">Dynamics 365 для продажи Enterprise Edition (цены США) надстройки для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-126">Dynamics 365 клиента интереса план Enterprise Edition Basic CRMOL (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-127">Dynamics 365 клиента интереса план Enterprise Edition (цены США) Basic CRMOL (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-128">Dynamics 365 клиента интереса план Enterprise Edition CRMOL Basic (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="05a90-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="05a90-129">Dynamics 365 клиента интереса план Enterprise Edition CRMOL Basic (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="05a90-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="05a90-130">Dynamics 365 клиента Engagement план Enterprise Edition с SA для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-131">Dynamics 365 клиента интереса план Enterprise Edition (цены США) из SA для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-132">Dynamics 365 клиента Engagement план Enterprise Edition с SA для CRM Basic (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="05a90-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="05a90-133">Dynamics 365 клиента Engagement план Enterprise Edition с SA для CRM Basic (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="05a90-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="05a90-134">Dynamics 365 клиента интереса план Enterprise Edition надстройки для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-135">Dynamics 365 клиента интереса план Enterprise Edition (цены США) надстройки для CRM Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-136">Dynamics 365 клиента интереса план Enterprise Edition надстройки для CRM Basic (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="05a90-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="05a90-137">Dynamics 365 клиента интереса план Enterprise Edition надстройки для CRM Basic (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="05a90-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="05a90-138">Dynamics 365 for Sales / Customer Engagement Plan из Basic (полное предлагает) замену планы</span><span class="sxs-lookup"><span data-stu-id="05a90-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="05a90-139">Устаревшую предложения</span><span class="sxs-lookup"><span data-stu-id="05a90-139">Retired offers</span></span>**   

- <span data-ttu-id="05a90-140">Dynamics 365 for Sales из CRM Basic или CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="05a90-141">План Dynamics 365 Customer Engagement из CRM Basic или CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="05a90-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="05a90-142">Варианты замены</span><span class="sxs-lookup"><span data-stu-id="05a90-142">Replacement options</span></span>**
- <span data-ttu-id="05a90-143">Dynamics 365 для продажи Профессиональная (НОВОЕ)</span><span class="sxs-lookup"><span data-stu-id="05a90-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="05a90-144">Dynamics 365 для продажи Профессиональная (НОВОЕ)</span><span class="sxs-lookup"><span data-stu-id="05a90-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="05a90-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="05a90-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="05a90-146">План Dynamics 365 Customer Engagement или</span><span class="sxs-lookup"><span data-stu-id="05a90-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="05a90-147">Dynamics 365 Team Members</span><span class="sxs-lookup"><span data-stu-id="05a90-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="05a90-148">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="05a90-148">Transition customers to new product plans</span></span>

<span data-ttu-id="05a90-149">Перенос клиентов из устаревшую SKU на новыми необходимо выполнить следующие действия в указанном порядке:</span><span class="sxs-lookup"><span data-stu-id="05a90-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="05a90-150">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="05a90-150">Purchase the new subscription</span></span>
- <span data-ttu-id="05a90-151">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="05a90-151">Reassign current user licenses</span></span>
- <span data-ttu-id="05a90-152">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="05a90-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="05a90-153">Приобрести новый план для клиента</span><span class="sxs-lookup"><span data-stu-id="05a90-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="05a90-154">Выберите **клиентов** из левого навигации, а затем выберите клиента, которого вы хотите перейти на новую подписку.</span><span class="sxs-lookup"><span data-stu-id="05a90-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="05a90-155">Выберите, **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="05a90-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="05a90-156">Выберите из каталога подписку, которую требуется приобрести (в данном случае— одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="05a90-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="05a90-157">Ваш клиент монет составит старую подписку и новым.</span><span class="sxs-lookup"><span data-stu-id="05a90-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="05a90-158">Следующим шагом является необходимо переназначить лицензии клиента.</span><span class="sxs-lookup"><span data-stu-id="05a90-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="05a90-159">Выберите **клиентов** из левого навигации, а затем выберите клиента, которого вы перемещаете.</span><span class="sxs-lookup"><span data-stu-id="05a90-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="05a90-160">Выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="05a90-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="05a90-161">Чтобы переназначить лицензии на пользователя, выберите пользователя, а затем выберите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="05a90-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="05a90-162">На странице " **Управление лицензиями** " Очистить Dynamics 365 for Sales / план привлечения клиентов из Basic (полное предлагать) установите флажок и выберите новый план обслуживания для подписки, которую пользователь перемещается на.</span><span class="sxs-lookup"><span data-stu-id="05a90-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="05a90-163">Выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="05a90-163">Select **Submit**.</span></span> <span data-ttu-id="05a90-164">Это выполняется для каждого пользователя, кто новую лицензию.</span><span class="sxs-lookup"><span data-stu-id="05a90-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="05a90-165">После того, как перейти лицензии на новую подписку можно отменить старую подписку.</span><span class="sxs-lookup"><span data-stu-id="05a90-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="05a90-166">Выберите **клиентов** из левого навигации, а затем выберите клиента, которого вы перемещаете.</span><span class="sxs-lookup"><span data-stu-id="05a90-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="05a90-167">На странице сведений подписки равным старой подписки **приостановлено** и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="05a90-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="05a90-168">Теперь старая подписка приостанавливается, а новая — активируется.</span><span class="sxs-lookup"><span data-stu-id="05a90-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="05a90-169">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="05a90-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="05a90-170">Ваш клиент будет несут не дополнительные затраты на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="05a90-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



