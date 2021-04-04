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
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132627"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="f2d14-104">Перенос подписок Office 365 E4 на новые версии Office 365</span><span class="sxs-lookup"><span data-stu-id="f2d14-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="f2d14-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="f2d14-105">**Appropriate roles**</span></span>

- <span data-ttu-id="f2d14-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f2d14-106">Global admin</span></span>
- <span data-ttu-id="f2d14-107">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="f2d14-107">User management admin</span></span>
- <span data-ttu-id="f2d14-108">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="f2d14-108">Admin agent</span></span>
- <span data-ttu-id="f2d14-109">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="f2d14-109">Sales agent</span></span>

<span data-ttu-id="f2d14-110">План Office 365 корпоративный E4 устарел 7 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f2d14-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="f2d14-111">После этого дня нельзя приобрести новые подписки Office 365 E4, а существующие подписки E4 не будут автоматически обновляться после истечения их срока действия.</span><span class="sxs-lookup"><span data-stu-id="f2d14-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="f2d14-112">По истечении срока действия подписок E4 они будут отменены.</span><span class="sxs-lookup"><span data-stu-id="f2d14-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="f2d14-113">Чтобы обеспечить непрерывность для пользователей, следует перенести пользователей с подписками E4, для которых истекает срок действия, на один из поддерживаемых SKU, которые перечислены ниже.</span><span class="sxs-lookup"><span data-stu-id="f2d14-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="f2d14-114">Рекомендуется переместить клиентов в новые подписки до даты окончания срока действия подписки, чтобы избежать простоев службы для клиентов.</span><span class="sxs-lookup"><span data-stu-id="f2d14-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="f2d14-115">Выпуски продуктов Office 365 Enterprise E4 для коммерческих и правительственных учреждений.</span><span class="sxs-lookup"><span data-stu-id="f2d14-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="f2d14-116">На странице сведений подписки состояние подписки E4 изменено с "Дата автоматического возобновления: [дата]" на "Срок действия истекает: [дата]".</span><span class="sxs-lookup"><span data-stu-id="f2d14-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="f2d14-117">Если вы используете API (CREST или Центра партнеров), вы можете найти подписки с истекающим сроком действия по дате завершения подписки и свойству автоматического возобновления со значением "ложь".</span><span class="sxs-lookup"><span data-stu-id="f2d14-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="f2d14-118">Для подписок E4 значение "ложь" для свойства автоматического возобновления устанавливается 7 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f2d14-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="f2d14-119">Перевести клиентов на новый план можно в любое время.</span><span class="sxs-lookup"><span data-stu-id="f2d14-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="f2d14-120">Планы замены выпуска Office 365 корпоративный E4</span><span class="sxs-lookup"><span data-stu-id="f2d14-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="f2d14-121">Можно поддерживать такую же функциональность в E4 или включить для клиентов обновленные функции и возможности в Office 365 и Skype для бизнеса Online.</span><span class="sxs-lookup"><span data-stu-id="f2d14-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="f2d14-122">Сведения о ценах приведены в прайс-листе и матрице предложений в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="f2d14-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="f2d14-123">Secure Product Enterprise E3 и Secure Productive Enterprise E5 можно заменить в следующих предложениях для Office 365 корпоративный E3 или Office 365 корпоративный E5 соответственно.</span><span class="sxs-lookup"><span data-stu-id="f2d14-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="f2d14-124">Предложение 1: Office 365 корпоративный E5</span><span class="sxs-lookup"><span data-stu-id="f2d14-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="f2d14-125">Предложение 2: Office 365 корпоративный E3 + облачная УАТС Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="f2d14-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="f2d14-126">Предложение 3: Office 365 корпоративный E3 + Skype для бизнеса Plus CAL (цены и функции аналогичны E4)</span><span class="sxs-lookup"><span data-stu-id="f2d14-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="f2d14-127">Предложение 4: Office 365 корпоративный E3</span><span class="sxs-lookup"><span data-stu-id="f2d14-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="f2d14-128">Компонент</span><span class="sxs-lookup"><span data-stu-id="f2d14-128">Feature</span></span> | <span data-ttu-id="f2d14-129">Вариант 1</span><span class="sxs-lookup"><span data-stu-id="f2d14-129">Option 1</span></span> | <span data-ttu-id="f2d14-130">Вариант 2</span><span class="sxs-lookup"><span data-stu-id="f2d14-130">Option 2</span></span> | <span data-ttu-id="f2d14-131">Предложение 3</span><span class="sxs-lookup"><span data-stu-id="f2d14-131">Option 3</span></span> | <span data-ttu-id="f2d14-132">Предложение 4</span><span class="sxs-lookup"><span data-stu-id="f2d14-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="f2d14-133">Получить все возможности, включенные в Office 365 корпоративный E4?</span><span class="sxs-lookup"><span data-stu-id="f2d14-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="f2d14-134">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-134">Yes</span></span> | <span data-ttu-id="f2d14-135">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-135">Yes</span></span> | <span data-ttu-id="f2d14-136">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-136">Yes</span></span> | <span data-ttu-id="f2d14-137">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-137">No</span></span> |
| <span data-ttu-id="f2d14-138">Управление номерами телефона в Office 365?</span><span class="sxs-lookup"><span data-stu-id="f2d14-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="f2d14-139">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-139">Yes</span></span> | <span data-ttu-id="f2d14-140">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-140">Yes</span></span> | <span data-ttu-id="f2d14-141">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-141">No</span></span> | <span data-ttu-id="f2d14-142">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-142">No</span></span> |
| <span data-ttu-id="f2d14-143">Управление номерами телефона выполняется как локально, так и в Office 365 (гибридное развертывание)?</span><span class="sxs-lookup"><span data-stu-id="f2d14-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="f2d14-144">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-144">Yes</span></span> | <span data-ttu-id="f2d14-145">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-145">Yes</span></span> | <span data-ttu-id="f2d14-146">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-146">No</span></span> | <span data-ttu-id="f2d14-147">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-147">No</span></span> |
| <span data-ttu-id="f2d14-148">Возможность добавить план голосовой связи ТСОП?</span><span class="sxs-lookup"><span data-stu-id="f2d14-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="f2d14-149">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-149">Yes</span></span> | <span data-ttu-id="f2d14-150">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-150">Yes</span></span> | <span data-ttu-id="f2d14-151">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-151">No</span></span> | <span data-ttu-id="f2d14-152">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-152">No</span></span> |
| <span data-ttu-id="f2d14-153">Конференции ТСОП?</span><span class="sxs-lookup"><span data-stu-id="f2d14-153">PSTN Conferencing?</span></span> | <span data-ttu-id="f2d14-154">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-154">Yes</span></span> | <span data-ttu-id="f2d14-155">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-155">No</span></span> | <span data-ttu-id="f2d14-156">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-156">No</span></span> | <span data-ttu-id="f2d14-157">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-157">No</span></span> |
| <span data-ttu-id="f2d14-158">Дополнительные средства для совместной работы, аналитики и безопасности?</span><span class="sxs-lookup"><span data-stu-id="f2d14-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="f2d14-159">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-159">Yes</span></span> | <span data-ttu-id="f2d14-160">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-160">No</span></span> | <span data-ttu-id="f2d14-161">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-161">No</span></span> | <span data-ttu-id="f2d14-162">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-162">No</span></span> |
| <span data-ttu-id="f2d14-163">Интерактивные отчеты, панели мониторинга и визуализация данных?</span><span class="sxs-lookup"><span data-stu-id="f2d14-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="f2d14-164">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-164">Yes</span></span> | <span data-ttu-id="f2d14-165">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-165">No</span></span> | <span data-ttu-id="f2d14-166">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-166">No</span></span> | <span data-ttu-id="f2d14-167">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-167">No</span></span> | 
| <span data-ttu-id="f2d14-168">Больше контроля над безопасностью данных и соответствием требованиям за счет встроенных функций конфиденциальности, прозрачности и улучшенных пользовательских элементов управления?</span><span class="sxs-lookup"><span data-stu-id="f2d14-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="f2d14-169">Да</span><span class="sxs-lookup"><span data-stu-id="f2d14-169">Yes</span></span> | <span data-ttu-id="f2d14-170">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-170">No</span></span> | <span data-ttu-id="f2d14-171">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-171">No</span></span> | <span data-ttu-id="f2d14-172">нет</span><span class="sxs-lookup"><span data-stu-id="f2d14-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f2d14-173">Перевод клиентов на новые планы продуктов</span><span class="sxs-lookup"><span data-stu-id="f2d14-173">Transition customers to new product plans</span></span>

<span data-ttu-id="f2d14-174">Корпорация Майкрософт регулярно предоставляет новые продукты и услуги нашим партнерам.</span><span class="sxs-lookup"><span data-stu-id="f2d14-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="f2d14-175">В подобных случаях вам может потребоваться обновить клиентов до новых служб или перенести их подписки с SKU, которые в конечном итоге будут закрыты.</span><span class="sxs-lookup"><span data-stu-id="f2d14-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="f2d14-176">Для переноса клиентов с устаревших SKU на новые требуется последовательно сделать следующее:</span><span class="sxs-lookup"><span data-stu-id="f2d14-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="f2d14-177">Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="f2d14-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="f2d14-178">Переназначение текущих пользовательских лицензий</span><span class="sxs-lookup"><span data-stu-id="f2d14-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="f2d14-179">Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="f2d14-179">Cancel the old subscription</span></span>

<span data-ttu-id="f2d14-180">Выполните эти действия, чтобы перенести подписку Office 365 корпоративный E4 клиента в одно из предложений, указанных в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="f2d14-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="f2d14-181">Шаг 1. Приобретение новой подписки</span><span class="sxs-lookup"><span data-stu-id="f2d14-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="f2d14-182">В меню **Центр партнеров** выберите **Клиенты**, выберите клиента, которого нужно переместить, а затем щелкните **Добавить подписки**.</span><span class="sxs-lookup"><span data-stu-id="f2d14-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="f2d14-183">Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="f2d14-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="f2d14-184">Теперь у клиента должны быть как старые, так и новые подписки, старая подписка Office 365 Enterprise E4 и новая подписка на "целевой", например 1-Office 365 Enterprise.</span><span class="sxs-lookup"><span data-stu-id="f2d14-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="f2d14-185">Шаг 2. Переназначение пользовательских лицензий клиента</span><span class="sxs-lookup"><span data-stu-id="f2d14-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="f2d14-186">В меню **Центр партнеров** выберите **Клиенты**, выберите клиента, которого хотите переместить, а затем выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="f2d14-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="f2d14-187">Откроется страница пользователи и лицензии клиента.</span><span class="sxs-lookup"><span data-stu-id="f2d14-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="f2d14-188">Чтобы переназначить пользовательские лицензии, выберите пользователя, которого нужно переназначить, а затем выберите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="f2d14-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="f2d14-189">На странице **Управление лицензиями** снимите флажок **Office 365 корпоративный E4** и выберите новый план обслуживания для подписки, на которую переходит клиент.</span><span class="sxs-lookup"><span data-stu-id="f2d14-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="f2d14-190">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="f2d14-190">Select **Submit**.</span></span> <span data-ttu-id="f2d14-191">На странице подтверждения указаны новые назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="f2d14-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="f2d14-192">Выполните эти же действия для всех остальных пользователей клиента, которым требуется переназначить лицензии.</span><span class="sxs-lookup"><span data-stu-id="f2d14-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="f2d14-193">После перемещения пользовательских лицензий в новую службу вы можете отменить устаревшую подписку на верхнем уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="f2d14-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="f2d14-194">Шаг 3. Отмена старой подписки</span><span class="sxs-lookup"><span data-stu-id="f2d14-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="f2d14-195">В меню **Центр партнеров** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="f2d14-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="f2d14-196">Выберите клиента, которого вы хотите перенести, и выберите подписку, которую нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="f2d14-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="f2d14-197">На странице сведения о подписке задайте для параметра состояние подписки значение **приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="f2d14-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="f2d14-198">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="f2d14-198">Select **Submit**.</span></span>

<span data-ttu-id="f2d14-199">Старая подписка приостанавливается, а новая активируется.</span><span class="sxs-lookup"><span data-stu-id="f2d14-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="f2d14-200">Приостановленная подписка будет автоматически отозвана через 120 дней.</span><span class="sxs-lookup"><span data-stu-id="f2d14-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f2d14-201">Клиент не несет дополнительных затрат на старую подписку.</span><span class="sxs-lookup"><span data-stu-id="f2d14-201">The customer incurs no additional costs for the old subscription.</span></span>



 



