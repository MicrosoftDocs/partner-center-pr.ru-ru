---
title: Миграция подписок Kaizala Pro на Microsoft365
description: Узнайте, как перенести подписки Kaizala Pro на версии Microsoft365 или Office 365. Дополнительные сведения о переходе клиентов см. в этой статье.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175170"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="0fbc6-104">Миграция автономных подписок Kaizala Pro на Microsoft365 или версии Office 365</span><span class="sxs-lookup"><span data-stu-id="0fbc6-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="0fbc6-105">Начиная с 1 июля 2020 г. Корпорация Майкрософт завершает продажи автономной службы Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-105">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="0fbc6-106">Клиенты больше не смогут покупать новые подписки Kaizala Pro после этой даты, а существующие подписки Kaizala Pro не будут обновляться автоматически по истечении срока их действия.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-106">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="0fbc6-107">Чтобы обеспечить непрерывность работы клиентов, следует перейти на поддержку Kaizala Pro автономных подписок на поддерживаемый SKU, указанный ниже.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-107">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="0fbc6-108">Рекомендуется переместить клиентов в новые подписки до даты окончания срока действия подписки, чтобы избежать простоев службы для клиентов.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="0fbc6-109">Если вы используете API (CREST или центр партнеров), вы можете обнаружить подписки с истекшим сроком действия, оценивая дату окончания подписки, а свойство Auto продления — в значение false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="0fbc6-109">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="0fbc6-110">Для подписок E4 будет установлено значение `auto renew=False` 1 июля 2020.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-110">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="0fbc6-111">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-111">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="0fbc6-112">Автономные планы замены Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="0fbc6-112">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="0fbc6-113">Благодаря новым планам ваши клиенты могут воспользоваться преимуществами новых функций и функций в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-113">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="0fbc6-114">Сведения о ценах приведены в прайс-листе и матрице предложений в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-114">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="0fbc6-115">[**Microsoft 365 для бизнеса**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), включая:</span><span class="sxs-lookup"><span data-stu-id="0fbc6-115">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="0fbc6-116">Microsoft 365 бизнес базовый;</span><span class="sxs-lookup"><span data-stu-id="0fbc6-116">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="0fbc6-117">Microsoft 365 бизнес стандартный;</span><span class="sxs-lookup"><span data-stu-id="0fbc6-117">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="0fbc6-118">Microsoft 365 бизнес премиум.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-118">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="0fbc6-119">[**Microsoft 365 для оказался**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), включая:</span><span class="sxs-lookup"><span data-stu-id="0fbc6-119">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="0fbc6-120">Microsoft 365 F3 (ранее — Microsoft 365 F1) и Office 365 F3.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-120">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="0fbc6-121">[**Microsoft 365 для предприятий**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), включая:</span><span class="sxs-lookup"><span data-stu-id="0fbc6-121">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="0fbc6-122">Office 365 E1;</span><span class="sxs-lookup"><span data-stu-id="0fbc6-122">Office 365 E1</span></span>
   - <span data-ttu-id="0fbc6-123">Microsoft 365 E3 и Office 365 E3;</span><span class="sxs-lookup"><span data-stu-id="0fbc6-123">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="0fbc6-124">Microsoft 365 E5 и Office 365 E5.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-124">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="0fbc6-125">[**Microsoft 365 для образовательных учреждений**](https://www.microsoft.com/education/buy-license/microsoft365), включая:</span><span class="sxs-lookup"><span data-stu-id="0fbc6-125">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="0fbc6-126">Microsoft 365 A1 и Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="0fbc6-126">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="0fbc6-127">Microsoft 365 A3 и Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="0fbc6-127">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="0fbc6-128">Microsoft 365 A5 и Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="0fbc6-128">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="0fbc6-129">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="0fbc6-129">Transition customers to new product plans</span></span>

<span data-ttu-id="0fbc6-130">Корпорация Майкрософт регулярно предоставляет новые продукты и услуги нашим партнерам.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-130">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="0fbc6-131">В подобных случаях вам может потребоваться обновить клиентов до новых служб или перенести их подписки с SKU, которые в конечном итоге будут закрыты.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-131">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="0fbc6-132">Для переноса клиентов с устаревших SKU на новые требуется последовательно сделать следующее:</span><span class="sxs-lookup"><span data-stu-id="0fbc6-132">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="0fbc6-133">A.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-133">A.</span></span> <span data-ttu-id="0fbc6-134">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="0fbc6-134">Purchase the new subscription</span></span>

<span data-ttu-id="0fbc6-135">Б.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-135">B.</span></span> <span data-ttu-id="0fbc6-136">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="0fbc6-136">Reassign current user licenses</span></span>

<span data-ttu-id="0fbc6-137">В.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-137">C.</span></span> <span data-ttu-id="0fbc6-138">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="0fbc6-138">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="0fbc6-139">Перевод пользователей на новые планы</span><span class="sxs-lookup"><span data-stu-id="0fbc6-139">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="0fbc6-140">A.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-140">A.</span></span> <span data-ttu-id="0fbc6-141">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="0fbc6-141">Purchase the new subscription</span></span>

1. <span data-ttu-id="0fbc6-142">Чтобы приобрести новую подписку, в меню **центра партнеров** выберите **Клиенты**, выберите клиента, которого требуется переместить, а затем щелкните **Добавить подписки**.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-142">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="0fbc6-143">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-143">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="0fbc6-144">Теперь у клиента должны быть как старые, так и новые подписки, старая автономная подписка Kaizala Pro и новая подписка "цель", например 1 — Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-144">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="0fbc6-145">Б.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-145">B.</span></span> <span data-ttu-id="0fbc6-146">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="0fbc6-146">Reassign current user licenses</span></span>

1. <span data-ttu-id="0fbc6-147">Чтобы переназначить лицензии пользователей клиента, в меню **центра партнеров** выберите **Клиенты**, выберите клиента, которого вы перемещаете, а затем выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-147">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="0fbc6-148">Откроется страница пользователи и лицензии клиента.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-148">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="0fbc6-149">Чтобы переназначить лицензию пользователя, выберите пользователя, которого нужно переназначить, а затем выберите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-149">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="0fbc6-150">На странице **Управление лицензиями** снимите флажок автономная лицензия Kaizala Pro и выберите новый план обслуживания для подписки, в которую будет перемещен клиент.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-150">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="0fbc6-151">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="0fbc6-151">Select **Submit**.</span></span> <span data-ttu-id="0fbc6-152">На странице подтверждения указаны новые назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-152">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="0fbc6-153">Продолжите выполнять эти же действия применительно к другим пользователям, которым требуется назначить лицензии.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-153">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="0fbc6-154">В.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-154">C.</span></span> <span data-ttu-id="0fbc6-155">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="0fbc6-155">Cancel old subscription</span></span>

<span data-ttu-id="0fbc6-156">После перемещения пользовательской лицензии в новую службу вы можете отменить устаревшую подписку на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-156">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="0fbc6-157">В меню **Центр партнеров** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="0fbc6-157">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="0fbc6-158">Выберите клиента, подписку которого требуется отменить.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-158">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="0fbc6-159">На странице с подробными сведениями о подписке установите статус **Приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-159">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="0fbc6-160">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="0fbc6-160">Select **Submit**.</span></span>

<span data-ttu-id="0fbc6-161">Старая подписка приостанавливается, а новая — активируется.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-161">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="0fbc6-162">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-162">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="0fbc6-163">Клиент не несет дополнительных затрат на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="0fbc6-163">The customer incurs no additional costs for the old subscription.</span></span>
