---
title: Перенос данных о Dynamics 365 и план взаимодействия клиента с Basic (полное предложений) до более новых версий | Центр партнеров
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement план из подписок Basic (полное предлагает) могут не обновляться.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 предлагает, обновить предложения, новые номера SKU Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586947"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="ca846-104">Перенос Dynamics 365 и плана Customer Engagement с "Базового" уровня (соответствующие предложения) в более новые версии</span><span class="sxs-lookup"><span data-stu-id="ca846-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="ca846-105">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="ca846-105">**Applies to**</span></span>

-  <span data-ttu-id="ca846-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="ca846-106">Partner Center</span></span>

<span data-ttu-id="ca846-107">Действующие клиенты 1 января 2019 г., с помощью Dynamics 365 for Sales / Customer Engagement план из подписок Basic (полное предлагает) больше не можете продлить эти устаревшие предложения; существующие подписки не будут автоматически продлеваться истечении их срока действия.</span><span class="sxs-lookup"><span data-stu-id="ca846-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="ca846-108">На странице сведений о подписке состояние подписки изменится на «Истекает [дата]» из «Автоматически обновляет [дата]».</span><span class="sxs-lookup"><span data-stu-id="ca846-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="ca846-109">Чтобы обеспечить непрерывность для клиентов, должно перейти с истекающим сроком действия подписки на поддерживаемый параметр, перечисленных ниже.</span><span class="sxs-lookup"><span data-stu-id="ca846-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="ca846-110">Мы рекомендуем переводить клиентов на новые подписки до ежегодной даты завершения подписки, чтобы не допускать перерывов в предоставлении службы клиентам.</span><span class="sxs-lookup"><span data-stu-id="ca846-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ca846-111">Если вы используете API (CREST или центра партнеров), можно найти подписки, срок действия которых истекает, оценивая дату окончания подписки, а также автоматического обновления = False свойство.</span><span class="sxs-lookup"><span data-stu-id="ca846-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="ca846-112">Рассматриваемый подписки будет указано значение auto продлить = False на 1 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ca846-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="ca846-113">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="ca846-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="ca846-114">Dynamics 365 предлагает выводится из эксплуатации</span><span class="sxs-lookup"><span data-stu-id="ca846-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="ca846-115">Dynamics 365 для Sales Enterprise Edition CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-116">Dynamics 365 для Basic CRMOL Sales Enterprise Edition (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="ca846-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ca846-117">Dynamics 365 для Basic CRMOL Sales Enterprise Edition (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="ca846-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ca846-118">Dynamics 365 для Sales Enterprise Edition (для государственных организаций) CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-119">Dynamics 365 for Sales Enterprise Edition с SA для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-120">Dynamics 365 for Sales Enterprise Edition с SA для Basic CRM (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="ca846-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ca846-121">Dynamics 365 for Sales Enterprise Edition с SA для Basic CRM (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="ca846-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ca846-122">Dynamics 365 for Sales Enterprise Edition (для государственных организаций) из SA для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-123">Dynamics 365 для надстройки Sales Enterprise Edition для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-124">Dynamics 365 для надстройки Sales Enterprise Edition для Basic CRM (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="ca846-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ca846-125">Dynamics 365 для надстройки Sales Enterprise Edition для Basic CRM (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="ca846-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ca846-126">Dynamics 365 для Sales Enterprise Edition (для государственных организаций) надстройками для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-127">Dynamics 365 Customer Engagement плана Enterprise Edition Basic CRMOL (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-128">Dynamics 365 Customer Engagement плана Enterprise Edition (для государственных организаций) Basic CRMOL (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-129">Dynamics 365 Customer Engagement плана Enterprise Edition CRMOL Basic (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="ca846-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ca846-130">Dynamics 365 Customer Engagement плана Enterprise Edition CRMOL Basic (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="ca846-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ca846-131">Dynamics 365 Customer Engagement Plan Enterprise Edition с SA для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (для государственных организаций) из SA для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-133">Dynamics 365 Customer Engagement Plan Enterprise Edition с SA для Basic CRM (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="ca846-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ca846-134">Dynamics 365 Customer Engagement Plan Enterprise Edition с SA для Basic CRM (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="ca846-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ca846-135">Dynamics 365 Customer Engagement плана Enterprise Edition надстройку для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-136">Dynamics 365 Customer Engagement Enterprise Edition (для государственных организаций) надстройки плана для Basic CRM (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-137">Dynamics 365 Customer Engagement плана Enterprise Edition надстройку для Basic CRM (Полное предложение) для учащихся</span><span class="sxs-lookup"><span data-stu-id="ca846-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ca846-138">Dynamics 365 Customer Engagement плана Enterprise Edition надстройку для Basic CRM (Полное предложение) для преподавателей</span><span class="sxs-lookup"><span data-stu-id="ca846-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="ca846-139">Dynamics 365 for Sales / Customer Engagement плана Basic (полное предлагает) замены планы</span><span class="sxs-lookup"><span data-stu-id="ca846-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="ca846-140">**Устаревшие предложения**</span><span class="sxs-lookup"><span data-stu-id="ca846-140">**Retired offers**</span></span>   

- <span data-ttu-id="ca846-141">Dynamics 365 for Sales из CRM Basic или CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ca846-142">Плана Dynamics 365 Customer Engagement, из CRM Basic или CRMOL Basic (Полное предложение)</span><span class="sxs-lookup"><span data-stu-id="ca846-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="ca846-143">**Параметры замены**</span><span class="sxs-lookup"><span data-stu-id="ca846-143">**Replacement options**</span></span>
- <span data-ttu-id="ca846-144">Dynamics 365 for Sales Professional (НОВОЕ)</span><span class="sxs-lookup"><span data-stu-id="ca846-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ca846-145">Dynamics 365 for Sales Professional (НОВОЕ)</span><span class="sxs-lookup"><span data-stu-id="ca846-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ca846-146">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="ca846-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="ca846-147">Плана Dynamics 365 Customer Engagement или</span><span class="sxs-lookup"><span data-stu-id="ca846-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="ca846-148">Члены команды Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ca846-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ca846-149">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="ca846-149">Transition customers to new product plans</span></span>

<span data-ttu-id="ca846-150">Переход клиентов с удалено номера SKU на более новые необходимо выполнить следующие действия в указанном порядке:</span><span class="sxs-lookup"><span data-stu-id="ca846-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="ca846-151">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="ca846-151">Purchase the new subscription</span></span>
- <span data-ttu-id="ca846-152">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="ca846-152">Reassign current user licenses</span></span>
- <span data-ttu-id="ca846-153">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="ca846-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="ca846-154">Приобретите новый план для вашего клиента</span><span class="sxs-lookup"><span data-stu-id="ca846-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="ca846-155">Выберите **клиентов** (левая панель), а затем выберите клиента, которую требуется переместить в новую подписку.</span><span class="sxs-lookup"><span data-stu-id="ca846-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="ca846-156">Выберите **добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="ca846-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="ca846-157">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="ca846-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="ca846-158">Теперь у вашего клиента будут старой подписки и новое.</span><span class="sxs-lookup"><span data-stu-id="ca846-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="ca846-159">Следующий шаг — переназначать лицензии для пользователей клиента.</span><span class="sxs-lookup"><span data-stu-id="ca846-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="ca846-160">Выберите **клиентов** (левая панель), а затем выберите клиента вы переходите.</span><span class="sxs-lookup"><span data-stu-id="ca846-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ca846-161">Выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="ca846-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="ca846-162">Чтобы переназначить лицензию пользователю, выберите пользователя, а затем выберите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="ca846-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="ca846-163">На **Управление лицензиями** странице снимите Dynamics 365 for Sales / плана Customer Engagement из Basic (Полное предложение), лицензии "флажок" и выберите новый план службы для клиента на перенос подписки.</span><span class="sxs-lookup"><span data-stu-id="ca846-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="ca846-164">Выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="ca846-164">Select **Submit**.</span></span> <span data-ttu-id="ca846-165">Это будет сделать для каждого пользователя, которому требуется новая лицензия.</span><span class="sxs-lookup"><span data-stu-id="ca846-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="ca846-166">После перемещения лицензий в новую подписку можно отменить старой подписки.</span><span class="sxs-lookup"><span data-stu-id="ca846-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="ca846-167">Выберите **клиентов** (левая панель), а затем выберите клиента вы переходите.</span><span class="sxs-lookup"><span data-stu-id="ca846-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ca846-168">На странице сведений подписки присвоено старой подписки **Suspended** и выберите **отправить**.</span><span class="sxs-lookup"><span data-stu-id="ca846-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="ca846-169">Приостановлена старой подписки, а новая подписка активна.</span><span class="sxs-lookup"><span data-stu-id="ca846-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="ca846-170">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="ca846-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ca846-171">Клиент будет взиматься без дополнительных затрат для старой подписки.</span><span class="sxs-lookup"><span data-stu-id="ca846-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



