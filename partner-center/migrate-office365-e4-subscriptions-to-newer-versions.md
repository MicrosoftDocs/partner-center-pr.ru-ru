---
title: Перенос подписок Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 корпоративный E4 перестал действовать 7 апреля 2017 г. Узнайте, как перенести подписки клиентов на более новые версии Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949048"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="2aa01-104">Перенос подписок Office 365 E4 на новые версии Office 365</span><span class="sxs-lookup"><span data-stu-id="2aa01-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="2aa01-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="2aa01-105">**Applies to**</span></span>

-  <span data-ttu-id="2aa01-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="2aa01-106">Partner Center</span></span>

<span data-ttu-id="2aa01-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="2aa01-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="2aa01-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2aa01-108">Global admin</span></span>
-   <span data-ttu-id="2aa01-109">администратор пользователей.</span><span class="sxs-lookup"><span data-stu-id="2aa01-109">User admin</span></span>
-   <span data-ttu-id="2aa01-110">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="2aa01-110">Admin agent</span></span>
-   <span data-ttu-id="2aa01-111">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="2aa01-111">Sales agent</span></span>

<span data-ttu-id="2aa01-112">План Office 365 корпоративный E4 устарел 7 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2aa01-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="2aa01-113">После этого дня нельзя приобрести новые подписки Office 365 E4, а существующие подписки E4 не будут автоматически обновляться после истечения их срока действия.</span><span class="sxs-lookup"><span data-stu-id="2aa01-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="2aa01-114">По истечении срока действия подписок E4 они будут отменены.</span><span class="sxs-lookup"><span data-stu-id="2aa01-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="2aa01-115">Чтобы обеспечить непрерывность для пользователей, следует перенести пользователей с подписками E4, для которых истекает срок действия, на один из поддерживаемых SKU, которые перечислены ниже.</span><span class="sxs-lookup"><span data-stu-id="2aa01-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="2aa01-116">Рекомендуется переместить клиентов в новые подписки до даты окончания срока действия подписки, чтобы избежать простоев службы для клиентов.</span><span class="sxs-lookup"><span data-stu-id="2aa01-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="2aa01-117">Выпуски продуктов Office 365 Enterprise E4 для коммерческих и правительственных учреждений.</span><span class="sxs-lookup"><span data-stu-id="2aa01-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="2aa01-118">На странице сведений подписки состояние подписки E4 изменено с "Дата автоматического возобновления: [дата]" на "Срок действия истекает: [дата]".</span><span class="sxs-lookup"><span data-stu-id="2aa01-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="2aa01-119">Если вы используете API (CREST или Центра партнеров), вы можете найти подписки с истекающим сроком действия по дате завершения подписки и свойству автоматического возобновления со значением "ложь".</span><span class="sxs-lookup"><span data-stu-id="2aa01-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="2aa01-120">Для подписок E4 значение "ложь" для свойства автоматического возобновления устанавливается 7 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2aa01-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="2aa01-121">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="2aa01-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="2aa01-122">Планы замены выпуска Office 365 корпоративный E4</span><span class="sxs-lookup"><span data-stu-id="2aa01-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="2aa01-123">Можно поддерживать такую же функциональность в E4 или включить для клиентов обновленные функции и возможности в Office 365 и Skype для бизнеса Online.</span><span class="sxs-lookup"><span data-stu-id="2aa01-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="2aa01-124">Сведения о ценах приведены в прайс-листе и матрице предложений в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="2aa01-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="2aa01-125">Secure Product Enterprise E3 и Secure Productive Enterprise E5 можно заменить в следующих предложениях для Office 365 корпоративный E3 или Office 365 корпоративный E5 соответственно.</span><span class="sxs-lookup"><span data-stu-id="2aa01-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="2aa01-126">Предложение 1: Office 365 корпоративный E5</span><span class="sxs-lookup"><span data-stu-id="2aa01-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="2aa01-127">Предложение 2: Office 365 корпоративный E3 + облачная УАТС Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="2aa01-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="2aa01-128">Предложение 3: Office 365 корпоративный E3 + Skype для бизнеса Plus CAL (цены и функции аналогичны E4)</span><span class="sxs-lookup"><span data-stu-id="2aa01-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="2aa01-129">Предложение 4: Office 365 корпоративный E3</span><span class="sxs-lookup"><span data-stu-id="2aa01-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="2aa01-130">Функция</span><span class="sxs-lookup"><span data-stu-id="2aa01-130">Feature</span></span> | <span data-ttu-id="2aa01-131">Вариант 1</span><span class="sxs-lookup"><span data-stu-id="2aa01-131">Option 1</span></span> | <span data-ttu-id="2aa01-132">Вариант 2</span><span class="sxs-lookup"><span data-stu-id="2aa01-132">Option 2</span></span> | <span data-ttu-id="2aa01-133">Предложение 3</span><span class="sxs-lookup"><span data-stu-id="2aa01-133">Option 3</span></span> | <span data-ttu-id="2aa01-134">Предложение 4</span><span class="sxs-lookup"><span data-stu-id="2aa01-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="2aa01-135">Получить все возможности, включенные в Office 365 корпоративный E4?</span><span class="sxs-lookup"><span data-stu-id="2aa01-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="2aa01-136">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-136">Yes</span></span> | <span data-ttu-id="2aa01-137">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-137">Yes</span></span> | <span data-ttu-id="2aa01-138">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-138">Yes</span></span> | <span data-ttu-id="2aa01-139">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-139">No</span></span> |
| <span data-ttu-id="2aa01-140">Управление номерами телефона в Office 365?</span><span class="sxs-lookup"><span data-stu-id="2aa01-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="2aa01-141">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-141">Yes</span></span> | <span data-ttu-id="2aa01-142">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-142">Yes</span></span> | <span data-ttu-id="2aa01-143">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-143">No</span></span> | <span data-ttu-id="2aa01-144">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-144">No</span></span> |
| <span data-ttu-id="2aa01-145">Управление номерами телефона выполняется как локально, так и в Office 365 (гибридное развертывание)?</span><span class="sxs-lookup"><span data-stu-id="2aa01-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="2aa01-146">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-146">Yes</span></span> | <span data-ttu-id="2aa01-147">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-147">Yes</span></span> | <span data-ttu-id="2aa01-148">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-148">No</span></span> | <span data-ttu-id="2aa01-149">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-149">No</span></span> |
| <span data-ttu-id="2aa01-150">Возможность добавить план голосовой связи ТСОП?</span><span class="sxs-lookup"><span data-stu-id="2aa01-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="2aa01-151">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-151">Yes</span></span> | <span data-ttu-id="2aa01-152">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-152">Yes</span></span> | <span data-ttu-id="2aa01-153">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-153">No</span></span> | <span data-ttu-id="2aa01-154">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-154">No</span></span> |
| <span data-ttu-id="2aa01-155">Конференции ТСОП?</span><span class="sxs-lookup"><span data-stu-id="2aa01-155">PSTN Conferencing?</span></span> | <span data-ttu-id="2aa01-156">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-156">Yes</span></span> | <span data-ttu-id="2aa01-157">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-157">No</span></span> | <span data-ttu-id="2aa01-158">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-158">No</span></span> | <span data-ttu-id="2aa01-159">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-159">No</span></span> |
| <span data-ttu-id="2aa01-160">Дополнительные средства для совместной работы, аналитики и безопасности?</span><span class="sxs-lookup"><span data-stu-id="2aa01-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="2aa01-161">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-161">Yes</span></span> | <span data-ttu-id="2aa01-162">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-162">No</span></span> | <span data-ttu-id="2aa01-163">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-163">No</span></span> | <span data-ttu-id="2aa01-164">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-164">No</span></span> |
| <span data-ttu-id="2aa01-165">Интерактивные отчеты, панели мониторинга и визуализация данных?</span><span class="sxs-lookup"><span data-stu-id="2aa01-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="2aa01-166">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-166">Yes</span></span> | <span data-ttu-id="2aa01-167">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-167">No</span></span> | <span data-ttu-id="2aa01-168">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-168">No</span></span> | <span data-ttu-id="2aa01-169">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-169">No</span></span> | 
| <span data-ttu-id="2aa01-170">Больше контроля над безопасностью данных и соответствием требованиям за счет встроенных функций конфиденциальности, прозрачности и улучшенных пользовательских элементов управления?</span><span class="sxs-lookup"><span data-stu-id="2aa01-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="2aa01-171">Да</span><span class="sxs-lookup"><span data-stu-id="2aa01-171">Yes</span></span> | <span data-ttu-id="2aa01-172">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-172">No</span></span> | <span data-ttu-id="2aa01-173">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-173">No</span></span> | <span data-ttu-id="2aa01-174">Нет</span><span class="sxs-lookup"><span data-stu-id="2aa01-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2aa01-175">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="2aa01-175">Transition customers to new product plans</span></span>

<span data-ttu-id="2aa01-176">Корпорация Майкрософт регулярно предоставляет новые продукты и услуги нашим партнерам.</span><span class="sxs-lookup"><span data-stu-id="2aa01-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="2aa01-177">В подобных случаях вам может потребоваться обновить клиентов до новых служб или перенести их подписки с SKU, которые в конечном итоге будут закрыты.</span><span class="sxs-lookup"><span data-stu-id="2aa01-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="2aa01-178">Для переноса клиентов с устаревших SKU на новые требуется последовательно сделать следующее:</span><span class="sxs-lookup"><span data-stu-id="2aa01-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="2aa01-179">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="2aa01-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="2aa01-180">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="2aa01-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="2aa01-181">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="2aa01-181">Cancel the old subscription</span></span>

<span data-ttu-id="2aa01-182">Выполните эти действия, чтобы перенести подписку Office 365 корпоративный E4 клиента в одно из предложений, указанных в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="2aa01-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="2aa01-183">Шаг 1. Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="2aa01-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="2aa01-184">В меню **Центр партнеров** выберите **Клиенты**, выберите клиента, которого нужно переместить, а затем щелкните **Добавить подписки**.</span><span class="sxs-lookup"><span data-stu-id="2aa01-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="2aa01-185">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="2aa01-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="2aa01-186">Теперь у клиента должны быть как старые, так и новые подписки, старая подписка Office 365 Enterprise E4 и новая подписка на "целевой", например 1-Office 365 Enterprise.</span><span class="sxs-lookup"><span data-stu-id="2aa01-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="2aa01-187">Шаг 2. Переназначение пользовательских лицензий клиента</span><span class="sxs-lookup"><span data-stu-id="2aa01-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="2aa01-188">В меню **Центр партнеров** выберите **Клиенты**, выберите клиента, которого хотите переместить, а затем выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="2aa01-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="2aa01-189">Откроется страница пользователи и лицензии клиента.</span><span class="sxs-lookup"><span data-stu-id="2aa01-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="2aa01-190">Чтобы переназначить пользовательские лицензии, выберите пользователя, которого требуется переназначить, а затем нажмите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="2aa01-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="2aa01-191">На странице **Управление лицензиями** снимите флажок **Office 365 корпоративный E4** и выберите новый план обслуживания для подписки, на которую переходит клиент.</span><span class="sxs-lookup"><span data-stu-id="2aa01-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="2aa01-192">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="2aa01-192">Select **Submit**.</span></span> <span data-ttu-id="2aa01-193">На странице подтверждения указаны новые назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="2aa01-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="2aa01-194">Выполните эти же действия для всех остальных пользователей клиента, которым требуется переназначить лицензии.</span><span class="sxs-lookup"><span data-stu-id="2aa01-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="2aa01-195">После перемещения пользовательских лицензий в новую службу вы можете отменить устаревшую подписку на верхнем уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="2aa01-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="2aa01-196">Шаг 3. Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="2aa01-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="2aa01-197">В меню **Центр партнеров** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="2aa01-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2aa01-198">Выберите клиента, которого вы хотите перенести, и выберите подписку, которую нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="2aa01-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="2aa01-199">На странице сведения о подписке задайте для параметра состояние подписки значение **приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="2aa01-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="2aa01-200">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="2aa01-200">Select **Submit**.</span></span>

<span data-ttu-id="2aa01-201">Старая подписка приостанавливается, а новая активируется.</span><span class="sxs-lookup"><span data-stu-id="2aa01-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="2aa01-202">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="2aa01-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2aa01-203">Клиент не несет дополнительных затрат на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="2aa01-203">The customer incurs no additional costs for the old subscription.</span></span>



 



