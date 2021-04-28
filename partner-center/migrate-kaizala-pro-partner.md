---
title: Перенос подписок Kaizala Pro в Microsoft 365
description: Узнайте, как перенести подписки Kaizala Pro на Microsoft 365 или версии Office 365. Дополнительные сведения о переходе клиентов см. в этой статье.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172410"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="7c269-104">Миграция автономных подписок Kaizala Pro на Microsoft 365 или версии Office 365</span><span class="sxs-lookup"><span data-stu-id="7c269-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="7c269-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="7c269-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7c269-106">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="7c269-106">Sales agent</span></span>

<span data-ttu-id="7c269-107">Начиная с 1 июля 2020 г. Корпорация Майкрософт завершает продажи автономной службы Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="7c269-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="7c269-108">Клиенты больше не смогут покупать новые подписки Kaizala Pro после этой даты, а существующие подписки Kaizala Pro не будут обновляться автоматически по истечении срока их действия.</span><span class="sxs-lookup"><span data-stu-id="7c269-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="7c269-109">Чтобы обеспечить непрерывность работы клиентов, следует перейти на поддержку Kaizala Pro автономных подписок на поддерживаемый SKU, указанный ниже.</span><span class="sxs-lookup"><span data-stu-id="7c269-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="7c269-110">Рекомендуется переместить клиентов в новые подписки до даты окончания срока действия подписки, чтобы избежать простоев службы для клиентов.</span><span class="sxs-lookup"><span data-stu-id="7c269-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="7c269-111">Если вы используете API (CREST или центр партнеров), вы можете обнаружить подписки с истекшим сроком действия, оценивая дату окончания подписки, а свойство Auto продления — в значение false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="7c269-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="7c269-112">Для подписок E4 будет установлено значение `auto renew=False` 1 июля 2020.</span><span class="sxs-lookup"><span data-stu-id="7c269-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="7c269-113">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="7c269-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="7c269-114">Автономные планы замены Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="7c269-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="7c269-115">Благодаря новым планам ваши клиенты могут воспользоваться преимуществами новых функций и функций в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7c269-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="7c269-116">Сведения о ценах приведены в прайс-листе и матрице предложений в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="7c269-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="7c269-117">[**Microsoft 365 для бизнеса**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), включая:</span><span class="sxs-lookup"><span data-stu-id="7c269-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="7c269-118">Microsoft 365 бизнес базовый;</span><span class="sxs-lookup"><span data-stu-id="7c269-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="7c269-119">Microsoft 365 бизнес стандартный;</span><span class="sxs-lookup"><span data-stu-id="7c269-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="7c269-120">Microsoft 365 бизнес премиум.</span><span class="sxs-lookup"><span data-stu-id="7c269-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="7c269-121">[**Microsoft 365 для оказался**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), включая:</span><span class="sxs-lookup"><span data-stu-id="7c269-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="7c269-122">Microsoft 365 F3 (ранее — Microsoft 365 F1) и Office 365 F3.</span><span class="sxs-lookup"><span data-stu-id="7c269-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="7c269-123">[**Microsoft 365 для предприятий**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), включая:</span><span class="sxs-lookup"><span data-stu-id="7c269-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="7c269-124">Office 365 E1;</span><span class="sxs-lookup"><span data-stu-id="7c269-124">Office 365 E1</span></span>
   - <span data-ttu-id="7c269-125">Microsoft 365 E3 и Office 365 E3;</span><span class="sxs-lookup"><span data-stu-id="7c269-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="7c269-126">Microsoft 365 E5 и Office 365 E5.</span><span class="sxs-lookup"><span data-stu-id="7c269-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="7c269-127">[**Microsoft 365 для образовательных учреждений**](https://www.microsoft.com/education/buy-license/microsoft365), включая:</span><span class="sxs-lookup"><span data-stu-id="7c269-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="7c269-128">Microsoft 365 A1 и Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="7c269-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="7c269-129">Microsoft 365 A3 и Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="7c269-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="7c269-130">Microsoft 365 A5 и Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="7c269-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="7c269-131">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="7c269-131">Transition customers to new product plans</span></span>

<span data-ttu-id="7c269-132">Корпорация Майкрософт регулярно предоставляет новые продукты и услуги нашим партнерам.</span><span class="sxs-lookup"><span data-stu-id="7c269-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="7c269-133">В подобных случаях вам может потребоваться обновить клиентов до новых служб или перенести их подписки с SKU, которые в конечном итоге будут закрыты.</span><span class="sxs-lookup"><span data-stu-id="7c269-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="7c269-134">Для переноса клиентов с устаревших SKU на новые требуется последовательно сделать следующее:</span><span class="sxs-lookup"><span data-stu-id="7c269-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="7c269-135">A.</span><span class="sxs-lookup"><span data-stu-id="7c269-135">A.</span></span> <span data-ttu-id="7c269-136">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="7c269-136">Purchase the new subscription</span></span>

<span data-ttu-id="7c269-137">Б.</span><span class="sxs-lookup"><span data-stu-id="7c269-137">B.</span></span> <span data-ttu-id="7c269-138">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="7c269-138">Reassign current user licenses</span></span>

<span data-ttu-id="7c269-139">В.</span><span class="sxs-lookup"><span data-stu-id="7c269-139">C.</span></span> <span data-ttu-id="7c269-140">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="7c269-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="7c269-141">Перевод пользователей на новые планы</span><span class="sxs-lookup"><span data-stu-id="7c269-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="7c269-142">A.</span><span class="sxs-lookup"><span data-stu-id="7c269-142">A.</span></span> <span data-ttu-id="7c269-143">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="7c269-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="7c269-144">Чтобы приобрести новую подписку, в меню **центра партнеров** выберите **Клиенты**, выберите клиента, которого требуется переместить, а затем щелкните **Добавить подписки**.</span><span class="sxs-lookup"><span data-stu-id="7c269-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="7c269-145">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="7c269-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="7c269-146">Теперь у клиента должны быть как старые, так и новые подписки, старая автономная подписка Kaizala Pro и новая подписка "цель", например 1 — Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="7c269-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="7c269-147">Б.</span><span class="sxs-lookup"><span data-stu-id="7c269-147">B.</span></span> <span data-ttu-id="7c269-148">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="7c269-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="7c269-149">Чтобы переназначить лицензии пользователей клиента, в меню **центра партнеров** выберите **Клиенты**, выберите клиента, которого вы перемещаете, а затем выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="7c269-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="7c269-150">Откроется страница пользователи и лицензии клиента.</span><span class="sxs-lookup"><span data-stu-id="7c269-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="7c269-151">Чтобы переназначить лицензию пользователя, выберите пользователя, которого нужно переназначить, а затем выберите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="7c269-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="7c269-152">На странице **Управление лицензиями** снимите флажок автономная лицензия Kaizala Pro и выберите новый план обслуживания для подписки, в которую будет перемещен клиент.</span><span class="sxs-lookup"><span data-stu-id="7c269-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="7c269-153">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="7c269-153">Select **Submit**.</span></span> <span data-ttu-id="7c269-154">На странице подтверждения указаны новые назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="7c269-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="7c269-155">Продолжите выполнять эти же действия применительно к другим пользователям, которым требуется назначить лицензии.</span><span class="sxs-lookup"><span data-stu-id="7c269-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="7c269-156">В.</span><span class="sxs-lookup"><span data-stu-id="7c269-156">C.</span></span> <span data-ttu-id="7c269-157">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="7c269-157">Cancel old subscription</span></span>

<span data-ttu-id="7c269-158">После перемещения пользовательской лицензии в новую службу вы можете отменить устаревшую подписку на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="7c269-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="7c269-159">В меню **Центр партнеров** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="7c269-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="7c269-160">Выберите клиента, подписку которого требуется отменить.</span><span class="sxs-lookup"><span data-stu-id="7c269-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="7c269-161">На странице с подробными сведениями о подписке установите статус **Приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="7c269-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="7c269-162">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="7c269-162">Select **Submit**.</span></span>

<span data-ttu-id="7c269-163">Старая подписка приостанавливается, а новая — активируется.</span><span class="sxs-lookup"><span data-stu-id="7c269-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="7c269-164">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="7c269-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="7c269-165">Клиент не несет дополнительных затрат на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="7c269-165">The customer incurs no additional costs for the old subscription.</span></span>
