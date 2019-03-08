---
title: Назначение пользователям ролей и разрешений | Центр партнеров
ms.topic: article
ms.date: 10/29/2018
description: Каждому сотруднику, которому нужен для работы в партнерском центре должна быть назначена роль.
author: LauraBrenner
ms.author: labrenne
keywords: роли, разрешения, администратор, агент
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587747"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="baa85-104">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="baa85-104">Assign users roles and permissions</span></span>


<span data-ttu-id="baa85-105">Вы настроили профиль партнера, включая юридическое название и адрес, сведения о поддержке, налог исключения файла, bank info и основного контактного лица для вашей компании.</span><span class="sxs-lookup"><span data-stu-id="baa85-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="baa85-106">Следующий шаг: настройка с паролями, а также роли, чтобы они могли начать работу в центре партнеров с вами пользователи.</span><span class="sxs-lookup"><span data-stu-id="baa85-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="baa85-107">Настройка сотрудников для работы в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="baa85-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="baa85-108">Вы определите типы доступа пользователей к центра партнеров, роли и разрешения, которые вы не предоставите им.</span><span class="sxs-lookup"><span data-stu-id="baa85-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="baa85-109">Роли, связаны с исполняемом формате, который вашего бизнеса участвует в.</span><span class="sxs-lookup"><span data-stu-id="baa85-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="baa85-110">Например, если вашего бизнеса — это поставщик облачных решений (CSP), вы не только будет standard Azure AD роли управления, такие как глобальный администратор клиента, но потребуется роли относятся к программе CSP.</span><span class="sxs-lookup"><span data-stu-id="baa85-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="baa85-111">Каждая программа имеет роли, относящиеся к ней.</span><span class="sxs-lookup"><span data-stu-id="baa85-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="baa85-112">Роли клиента Azure Active Directory (AAD) включают глобального администратора, администратора пользователей и ролей CSP.</span><span class="sxs-lookup"><span data-stu-id="baa85-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="baa85-113">Роли AAD не включать администратора MPN, бизнеса профиль администратора, администратора ссылок, стимулирования администратора и стимулирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="baa85-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="baa85-114">Управление коммерческих транзакций в центре партнеров (Azure AD и ролей CSP)</span><span class="sxs-lookup"><span data-stu-id="baa85-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="baa85-115">**Роли**</span><span class="sxs-lookup"><span data-stu-id="baa85-115">**Role**</span></span>|<span data-ttu-id="baa85-116">**Их возможности**</span><span class="sxs-lookup"><span data-stu-id="baa85-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="baa85-117">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="baa85-117">Global admin</span></span>|<span data-ttu-id="baa85-118">• Можно получить доступ к учетной записи или службы Майкрософт с административными полномочиями</span><span class="sxs-lookup"><span data-stu-id="baa85-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="baa85-119">• Создание запросов в службу поддержки для центра партнеров</span><span class="sxs-lookup"><span data-stu-id="baa85-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="baa85-120">• Представление соглашения, прайс-листы и предложения</span><span class="sxs-lookup"><span data-stu-id="baa85-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="baa85-121">• Просмотр, создание и управление пользователей партнера</span><span class="sxs-lookup"><span data-stu-id="baa85-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="baa85-122">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="baa85-122">User Admin</span></span>   | <span data-ttu-id="baa85-123">• Просмотр, создание и управление пользователями</span><span class="sxs-lookup"><span data-stu-id="baa85-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="baa85-124">• Просмотреть все профили партнеров</span><span class="sxs-lookup"><span data-stu-id="baa85-124">• View all partner profiles</span></span>
||<span data-ttu-id="baa85-125">• Просмотр, создание и управление пользователей партнера</span><span class="sxs-lookup"><span data-stu-id="baa85-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="baa85-126">Пользователь по умолчанию</span><span class="sxs-lookup"><span data-stu-id="baa85-126">Default user</span></span>|  <span data-ttu-id="baa85-127">Просмотреть мой профиль</span><span class="sxs-lookup"><span data-stu-id="baa85-127">View My profile</span></span>   |
|<span data-ttu-id="baa85-128">Агент администрирования</span><span class="sxs-lookup"><span data-stu-id="baa85-128">Admin agent</span></span> | <span data-ttu-id="baa85-129">• Управление клиентами</span><span class="sxs-lookup"><span data-stu-id="baa85-129">•    Customer management</span></span>
||<span data-ttu-id="baa85-130">• Добавьте список устройств для центра партнеров <</span><span class="sxs-lookup"><span data-stu-id="baa85-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="baa85-131">• Создание и применение профилей на устройствах</span><span class="sxs-lookup"><span data-stu-id="baa85-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="baa85-132">• Управление подпиской</span><span class="sxs-lookup"><span data-stu-id="baa85-132">• Subscription management</span></span>
||<span data-ttu-id="baa85-133">• Служба работоспособности запросы и службы для клиентов</span><span class="sxs-lookup"><span data-stu-id="baa85-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="baa85-134">• Запрос делегирования привилегий администратора</span><span class="sxs-lookup"><span data-stu-id="baa85-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="baa85-135">• Просмотреть цены и предложения</span><span class="sxs-lookup"><span data-stu-id="baa85-135">• View pricing and offers</span></span>
||<span data-ttu-id="baa85-136">• Выставления счетов</span><span class="sxs-lookup"><span data-stu-id="baa85-136">• Billing</span></span>
||<span data-ttu-id="baa85-137">• Администрирование от имени клиента</span><span class="sxs-lookup"><span data-stu-id="baa85-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="baa85-138">• Register значение добавлены торгового посредника</span><span class="sxs-lookup"><span data-stu-id="baa85-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="baa85-139">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="baa85-139">Sales agent</span></span> | <span data-ttu-id="baa85-140">• Управление клиентами</span><span class="sxs-lookup"><span data-stu-id="baa85-140">•    Customer management</span></span>
||<span data-ttu-id="baa85-141">• Добавьте список устройств для центра партнеров</span><span class="sxs-lookup"><span data-stu-id="baa85-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="baa85-142">• Управление подпиской</span><span class="sxs-lookup"><span data-stu-id="baa85-142">• Subscription management</span></span>
||<span data-ttu-id="baa85-143">• Запросы в службу поддержки представления</span><span class="sxs-lookup"><span data-stu-id="baa85-143">• View support tickets</span></span>
||<span data-ttu-id="baa85-144">• Запрос связь с клиентом</span><span class="sxs-lookup"><span data-stu-id="baa85-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="baa85-145">• Управление интересов</span><span class="sxs-lookup"><span data-stu-id="baa85-145">• Manage customer leads</span></span>
||<span data-ttu-id="baa85-146">Представления • соглашении клиента</span><span class="sxs-lookup"><span data-stu-id="baa85-146">• View the customer agreement</span></span>
||<span data-ttu-id="baa85-147">• Register системного интегратора</span><span class="sxs-lookup"><span data-stu-id="baa85-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="baa85-148">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="baa85-148">Helpdesk agent</span></span>| <span data-ttu-id="baa85-149">• Поиск и просмотр клиента</span><span class="sxs-lookup"><span data-stu-id="baa85-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="baa85-150">• Изменение клиента сведений</span><span class="sxs-lookup"><span data-stu-id="baa85-150">• Edit customer details</span></span>
||<span data-ttu-id="baa85-151">• Справка устранить проблемы клиентов с помощью управления выставления счета или подписки</span><span class="sxs-lookup"><span data-stu-id="baa85-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="baa85-152">• Поддержка запросов от имени клиентов (Примечание: Должен быть агент администратора для выполнения этой задачи для подписки на Office 365)</span><span class="sxs-lookup"><span data-stu-id="baa85-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="baa85-153">• Управление подписками и выставления счетов проблемы от имени клиентов (Примечание: Должен быть агент администратора для выполнения этой задачи для подписки на Office 365)</span><span class="sxs-lookup"><span data-stu-id="baa85-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="baa85-154">Поставщик панели управления (CPV).</span><span class="sxs-lookup"><span data-stu-id="baa85-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="baa85-155">(Роль CSP и роли не AAD)</span><span class="sxs-lookup"><span data-stu-id="baa85-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="baa85-156">CPVs разработка приложений для использования с партнеров поставщика облачных решений (CSP), чтобы включить их для интеграции своих систем с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="baa85-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="baa85-157">**Роли**</span><span class="sxs-lookup"><span data-stu-id="baa85-157">**Role**</span></span>   |<span data-ttu-id="baa85-158">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="baa85-158">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="baa85-159">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="baa85-159">Global admin</span></span>| <span data-ttu-id="baa85-160">Просмотр и Управление профилем CPV</span><span class="sxs-lookup"><span data-stu-id="baa85-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="baa85-161">Просматривать и управлять любыми пользователями, которым требуется доступ к возможностям CPV</span><span class="sxs-lookup"><span data-stu-id="baa85-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="baa85-162">Управлять членством в MPN и ваша компания (не AAD роли)</span><span class="sxs-lookup"><span data-stu-id="baa85-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="baa85-163">**Роли**</span><span class="sxs-lookup"><span data-stu-id="baa85-163">**Role**</span></span> | <span data-ttu-id="baa85-164">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="baa85-164">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="baa85-165">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="baa85-165">MPN partner admin</span></span>|<span data-ttu-id="baa85-166">•CAN Добавление пользователей не клиентами</span><span class="sxs-lookup"><span data-stu-id="baa85-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="baa85-167">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="baa85-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="baa85-168">• Представление юридические, организации, бизнеса и профили MPN</span><span class="sxs-lookup"><span data-stu-id="baa85-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="baa85-169">• Просмотр сведений о пользователях и навыки работы с ними данных</span><span class="sxs-lookup"><span data-stu-id="baa85-169">• View user details and their skills data</span></span>
||<span data-ttu-id="baa85-170">• Просмотр компетенций</span><span class="sxs-lookup"><span data-stu-id="baa85-170">• View competencies</span></span>
||<span data-ttu-id="baa85-171">• Просмотр и управление ими преимущества</span><span class="sxs-lookup"><span data-stu-id="baa85-171">• View and manage benefits</span></span>
||<span data-ttu-id="baa85-172">• Представление и покупку MPN предлагает</span><span class="sxs-lookup"><span data-stu-id="baa85-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="baa85-173">• Представление MPN предлагает историю заказов и счета-фактуры</span><span class="sxs-lookup"><span data-stu-id="baa85-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="baa85-174">• Просмотр партнера вклад данных</span><span class="sxs-lookup"><span data-stu-id="baa85-174">• View partner contribution data</span></span>
||<span data-ttu-id="baa85-175">• Можно работать в средстве проверки ваучер</span><span class="sxs-lookup"><span data-stu-id="baa85-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="baa85-176">— Просмотр данных аналитики клиента</span><span class="sxs-lookup"><span data-stu-id="baa85-176">- View customer data analytics</span></span>
|<span data-ttu-id="baa85-177">Администрирование учетных записей</span><span class="sxs-lookup"><span data-stu-id="baa85-177">Account admin</span></span>| <span data-ttu-id="baa85-178">• Можно добавить пользователей не клиентами</span><span class="sxs-lookup"><span data-stu-id="baa85-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="baa85-179">• Добавление или удаление расположений</span><span class="sxs-lookup"><span data-stu-id="baa85-179">• Add or delete locations</span></span>
||<span data-ttu-id="baa85-180">-Управление профилями, связанные с учетными записями, которые вы являетесь администратором для</span><span class="sxs-lookup"><span data-stu-id="baa85-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="baa85-181">• Назначение ролей для пользователей в клиенте для роли не AAD</span><span class="sxs-lookup"><span data-stu-id="baa85-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="baa85-182">• Расположений в программы регистрации</span><span class="sxs-lookup"><span data-stu-id="baa85-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="baa85-183">Управлять потенциальными клиентами (без AAD роли)</span><span class="sxs-lookup"><span data-stu-id="baa85-183">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="baa85-184">**Роли**</span><span class="sxs-lookup"><span data-stu-id="baa85-184">**Role**</span></span>|<span data-ttu-id="baa85-185">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="baa85-185">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="baa85-186">Администратор ссылок</span><span class="sxs-lookup"><span data-stu-id="baa85-186">Referrals admin</span></span>       |<span data-ttu-id="baa85-187">• Просмотр, создание и управление бизнес-профили</span><span class="sxs-lookup"><span data-stu-id="baa85-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="baa85-188">• Получать и управлять потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="baa85-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="baa85-189">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="baa85-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="baa85-190">Администратор бизнес-профиля</span><span class="sxs-lookup"><span data-stu-id="baa85-190">Business profile admin</span></span>   |<span data-ttu-id="baa85-191">•View, создавать и управлять бизнес-профиль</span><span class="sxs-lookup"><span data-stu-id="baa85-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="baa85-192">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="baa85-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="baa85-193">Управление поощрения (без AAD роли)</span><span class="sxs-lookup"><span data-stu-id="baa85-193">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="baa85-194">**Роли**</span><span class="sxs-lookup"><span data-stu-id="baa85-194">**Role**</span></span> | <span data-ttu-id="baa85-195">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="baa85-195">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="baa85-196">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="baa85-196">Incentives admin</span></span>|<span data-ttu-id="baa85-197">• Инициирует и управляет поощрения</span><span class="sxs-lookup"><span data-stu-id="baa85-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="baa85-198">• Можно просматривать и изменять все аспекты поощрения для программы</span><span class="sxs-lookup"><span data-stu-id="baa85-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="baa85-199">• Можно просматривать и изменять банковские и налоговые сведения</span><span class="sxs-lookup"><span data-stu-id="baa85-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="baa85-200">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="baa85-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="baa85-201">• Поддержка доступа</span><span class="sxs-lookup"><span data-stu-id="baa85-201">• Access support</span></span>
||<span data-ttu-id="baa85-202">• Споров в отношении поощрения платежей</span><span class="sxs-lookup"><span data-stu-id="baa85-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="baa85-203">Пользователь программы поощрения</span><span class="sxs-lookup"><span data-stu-id="baa85-203">Incentives user</span></span>|<span data-ttu-id="baa85-204">• Можно просмотреть поощрения для программы</span><span class="sxs-lookup"><span data-stu-id="baa85-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="baa85-205">• Можно просматривать и инициировать поощрения утверждений</span><span class="sxs-lookup"><span data-stu-id="baa85-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="baa85-206">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="baa85-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="baa85-207">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="baa85-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="baa85-208">• Поддержка доступа</span><span class="sxs-lookup"><span data-stu-id="baa85-208">• Access support</span></span>












