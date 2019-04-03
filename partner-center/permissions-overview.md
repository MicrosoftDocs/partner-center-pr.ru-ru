---
title: Назначение пользователям ролей и разрешений | Центр партнеров
ms.topic: article
ms.date: 3/5/19
description: Каждому сотруднику, которому нужен для работы в партнерском центре должна быть назначена роль.
author: LauraBrenner
ms.author: labrenne
keywords: роли, разрешения, администратор, агент
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682492"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="4c620-104">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="4c620-104">Assign users roles and permissions</span></span>


<span data-ttu-id="4c620-105">Вы настроили профиль партнера, включая юридическое название и адрес, сведения о поддержке, налог исключения файла, bank info и основного контактного лица для вашей компании.</span><span class="sxs-lookup"><span data-stu-id="4c620-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="4c620-106">Следующий шаг: настройка с паролями, а также роли, чтобы они могли начать работу в центре партнеров с вами пользователи.</span><span class="sxs-lookup"><span data-stu-id="4c620-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="4c620-107">Настройка сотрудников для работы в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="4c620-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="4c620-108">Вы определите типы доступа пользователей к центра партнеров, роли и разрешения, которые вы не предоставите им.</span><span class="sxs-lookup"><span data-stu-id="4c620-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="4c620-109">Роли, связаны с исполняемом формате, который вашего бизнеса участвует в.</span><span class="sxs-lookup"><span data-stu-id="4c620-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="4c620-110">Например, если вашего бизнеса — это поставщик облачных решений (CSP), вы не только будет standard Azure AD роли управления, такие как глобальный администратор клиента, но потребуется роли относятся к программе CSP.</span><span class="sxs-lookup"><span data-stu-id="4c620-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="4c620-111">Каждая программа имеет роли, относящиеся к ней.</span><span class="sxs-lookup"><span data-stu-id="4c620-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="4c620-112">Роли клиента Azure Active Directory (AAD) включают глобального администратора, администратора пользователей и ролей CSP.</span><span class="sxs-lookup"><span data-stu-id="4c620-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="4c620-113">Роли AAD не включать администратора MPN, бизнеса профиль администратора, администратора ссылок, стимулирования администратора и стимулирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="4c620-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="4c620-114">Управление коммерческих транзакций в центре партнеров (Azure AD и ролей CSP)</span><span class="sxs-lookup"><span data-stu-id="4c620-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="4c620-115">**Роли**</span><span class="sxs-lookup"><span data-stu-id="4c620-115">**Role**</span></span>|<span data-ttu-id="4c620-116">**Их возможности**</span><span class="sxs-lookup"><span data-stu-id="4c620-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="4c620-117">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4c620-117">Global admin</span></span>|<span data-ttu-id="4c620-118">• Можно получить доступ к учетной записи или службы Майкрософт с административными полномочиями</span><span class="sxs-lookup"><span data-stu-id="4c620-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="4c620-119">• Создание запросов в службу поддержки для центра партнеров</span><span class="sxs-lookup"><span data-stu-id="4c620-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4c620-120">• Представление соглашения, прайс-листы и предложения</span><span class="sxs-lookup"><span data-stu-id="4c620-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="4c620-121">• Просмотр, создание и управление пользователей партнера</span><span class="sxs-lookup"><span data-stu-id="4c620-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="4c620-122">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="4c620-122">User Admin</span></span>   | <span data-ttu-id="4c620-123">• Просмотр, создание и управление пользователями</span><span class="sxs-lookup"><span data-stu-id="4c620-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="4c620-124">• Просмотреть все профили партнеров</span><span class="sxs-lookup"><span data-stu-id="4c620-124">• View all partner profiles</span></span>
||<span data-ttu-id="4c620-125">• Просмотр, создание и управление пользователей партнера</span><span class="sxs-lookup"><span data-stu-id="4c620-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="4c620-126">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="4c620-126">Billing admin</span></span> | <span data-ttu-id="4c620-127">— Просмотр, создание и управление выставлением счетов, счета-фактуры и проверка файлов</span><span class="sxs-lookup"><span data-stu-id="4c620-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="4c620-128">Пользователь по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4c620-128">Default user</span></span>|  <span data-ttu-id="4c620-129">Просмотреть мой профиль</span><span class="sxs-lookup"><span data-stu-id="4c620-129">View My profile</span></span>   |
|<span data-ttu-id="4c620-130">Агент администрирования</span><span class="sxs-lookup"><span data-stu-id="4c620-130">Admin agent</span></span> | <span data-ttu-id="4c620-131">• Управление клиентами</span><span class="sxs-lookup"><span data-stu-id="4c620-131">•    Customer management</span></span>
||<span data-ttu-id="4c620-132">• Добавьте список устройств для центра партнеров <</span><span class="sxs-lookup"><span data-stu-id="4c620-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="4c620-133">• Создание и применение профилей на устройствах</span><span class="sxs-lookup"><span data-stu-id="4c620-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="4c620-134">• Управление подпиской</span><span class="sxs-lookup"><span data-stu-id="4c620-134">• Subscription management</span></span>
||<span data-ttu-id="4c620-135">• Служба работоспособности запросы и службы для клиентов</span><span class="sxs-lookup"><span data-stu-id="4c620-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="4c620-136">• Запрос делегирования привилегий администратора</span><span class="sxs-lookup"><span data-stu-id="4c620-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="4c620-137">• Просмотреть цены и предложения</span><span class="sxs-lookup"><span data-stu-id="4c620-137">• View pricing and offers</span></span>
||<span data-ttu-id="4c620-138">• Выставления счетов</span><span class="sxs-lookup"><span data-stu-id="4c620-138">• Billing</span></span>
||<span data-ttu-id="4c620-139">• Администрирование от имени клиента</span><span class="sxs-lookup"><span data-stu-id="4c620-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="4c620-140">• Register значение добавлены торгового посредника</span><span class="sxs-lookup"><span data-stu-id="4c620-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="4c620-141">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="4c620-141">Sales agent</span></span> | <span data-ttu-id="4c620-142">• Управление клиентами</span><span class="sxs-lookup"><span data-stu-id="4c620-142">•    Customer management</span></span>
||<span data-ttu-id="4c620-143">• Добавьте список устройств для центра партнеров</span><span class="sxs-lookup"><span data-stu-id="4c620-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="4c620-144">• Управление подпиской</span><span class="sxs-lookup"><span data-stu-id="4c620-144">• Subscription management</span></span>
||<span data-ttu-id="4c620-145">• Запросы в службу поддержки представления</span><span class="sxs-lookup"><span data-stu-id="4c620-145">• View support tickets</span></span>
||<span data-ttu-id="4c620-146">• Запрос связь с клиентом</span><span class="sxs-lookup"><span data-stu-id="4c620-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="4c620-147">• Управление интересов</span><span class="sxs-lookup"><span data-stu-id="4c620-147">• Manage customer leads</span></span>
||<span data-ttu-id="4c620-148">Представления • соглашении клиента</span><span class="sxs-lookup"><span data-stu-id="4c620-148">• View the customer agreement</span></span>
||<span data-ttu-id="4c620-149">• Register системного интегратора</span><span class="sxs-lookup"><span data-stu-id="4c620-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="4c620-150">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="4c620-150">Helpdesk agent</span></span>| <span data-ttu-id="4c620-151">• Поиск и просмотр клиента</span><span class="sxs-lookup"><span data-stu-id="4c620-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="4c620-152">• Изменение клиента сведений</span><span class="sxs-lookup"><span data-stu-id="4c620-152">• Edit customer details</span></span>
||<span data-ttu-id="4c620-153">• Справка устранить проблемы клиентов с помощью управления выставления счета или подписки</span><span class="sxs-lookup"><span data-stu-id="4c620-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="4c620-154">• Поддержка запросов от имени клиентов (Примечание: Должен быть агент администратора для выполнения этой задачи для подписки на Office 365)</span><span class="sxs-lookup"><span data-stu-id="4c620-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="4c620-155">• Управление подписками и выставления счетов проблемы от имени клиентов (Примечание: Должен быть агент администратора для выполнения этой задачи для подписки на Office 365)</span><span class="sxs-lookup"><span data-stu-id="4c620-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="4c620-156">Поставщик панели управления (CPV).</span><span class="sxs-lookup"><span data-stu-id="4c620-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="4c620-157">(Роль CSP и роли не AAD)</span><span class="sxs-lookup"><span data-stu-id="4c620-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="4c620-158">CPVs разработка приложений для использования с партнеров поставщика облачных решений (CSP), чтобы включить их для интеграции своих систем с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="4c620-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="4c620-159">**Роли**</span><span class="sxs-lookup"><span data-stu-id="4c620-159">**Role**</span></span>   |<span data-ttu-id="4c620-160">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="4c620-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="4c620-161">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4c620-161">Global admin</span></span>| <span data-ttu-id="4c620-162">Просмотр и Управление профилем CPV</span><span class="sxs-lookup"><span data-stu-id="4c620-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="4c620-163">Просматривать и управлять любыми пользователями, которым требуется доступ к возможностям CPV</span><span class="sxs-lookup"><span data-stu-id="4c620-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="4c620-164">Управлять членством в MPN и ваша компания (не AAD роли)</span><span class="sxs-lookup"><span data-stu-id="4c620-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="4c620-165">**Роли**</span><span class="sxs-lookup"><span data-stu-id="4c620-165">**Role**</span></span> | <span data-ttu-id="4c620-166">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="4c620-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="4c620-167">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="4c620-167">MPN partner admin</span></span>|<span data-ttu-id="4c620-168">•CAN Добавление пользователей не клиентами</span><span class="sxs-lookup"><span data-stu-id="4c620-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="4c620-169">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="4c620-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="4c620-170">• Представление юридические, организации, бизнеса и профили MPN</span><span class="sxs-lookup"><span data-stu-id="4c620-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="4c620-171">• Просмотр сведений о пользователях и навыки работы с ними данных</span><span class="sxs-lookup"><span data-stu-id="4c620-171">• View user details and their skills data</span></span>
||<span data-ttu-id="4c620-172">• Просмотр компетенций</span><span class="sxs-lookup"><span data-stu-id="4c620-172">• View competencies</span></span>
||<span data-ttu-id="4c620-173">• Просмотр и управление ими преимущества</span><span class="sxs-lookup"><span data-stu-id="4c620-173">• View and manage benefits</span></span>
||<span data-ttu-id="4c620-174">• Представление и покупку MPN предлагает</span><span class="sxs-lookup"><span data-stu-id="4c620-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="4c620-175">• Представление MPN предлагает историю заказов и счета-фактуры</span><span class="sxs-lookup"><span data-stu-id="4c620-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="4c620-176">• Просмотр партнера вклад данных</span><span class="sxs-lookup"><span data-stu-id="4c620-176">• View partner contribution data</span></span>
||<span data-ttu-id="4c620-177">• Можно работать в средстве проверки ваучер</span><span class="sxs-lookup"><span data-stu-id="4c620-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="4c620-178">— Просмотр данных аналитики клиента</span><span class="sxs-lookup"><span data-stu-id="4c620-178">- View customer data analytics</span></span>
|<span data-ttu-id="4c620-179">Администрирование учетных записей</span><span class="sxs-lookup"><span data-stu-id="4c620-179">Account admin</span></span>| <span data-ttu-id="4c620-180">• Можно добавить пользователей не клиентами</span><span class="sxs-lookup"><span data-stu-id="4c620-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="4c620-181">• Добавление или удаление расположений</span><span class="sxs-lookup"><span data-stu-id="4c620-181">• Add or delete locations</span></span>
||<span data-ttu-id="4c620-182">-Управление профилями, связанные с учетными записями, которые вы являетесь администратором для</span><span class="sxs-lookup"><span data-stu-id="4c620-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="4c620-183">• Назначение ролей для пользователей в клиенте для роли не AAD</span><span class="sxs-lookup"><span data-stu-id="4c620-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="4c620-184">• Расположений в программы регистрации</span><span class="sxs-lookup"><span data-stu-id="4c620-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="4c620-185">Гостевой пользователь (необходимо добавить в клиент AAD)</span><span class="sxs-lookup"><span data-stu-id="4c620-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="4c620-186">**Гостевой пользователь**</span><span class="sxs-lookup"><span data-stu-id="4c620-186">**Guest user**</span></span>   | <span data-ttu-id="4c620-187">**Роли**</span><span class="sxs-lookup"><span data-stu-id="4c620-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="4c620-188">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="4c620-188">MPN partner admin</span></span>|
||<span data-ttu-id="4c620-189">Учетные записи администратора</span><span class="sxs-lookup"><span data-stu-id="4c620-189">Accounts admin</span></span>|
||<span data-ttu-id="4c620-190">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="4c620-190">Incentives admin</span></span>|
||<span data-ttu-id="4c620-191">Администратор бизнес-профиля</span><span class="sxs-lookup"><span data-stu-id="4c620-191">Business profile admin</span></span>|
||<span data-ttu-id="4c620-192">Администратор ссылок</span><span class="sxs-lookup"><span data-stu-id="4c620-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="4c620-193">Управлять потенциальными клиентами (без AAD роли)</span><span class="sxs-lookup"><span data-stu-id="4c620-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="4c620-194">**Роли**</span><span class="sxs-lookup"><span data-stu-id="4c620-194">**Role**</span></span>|<span data-ttu-id="4c620-195">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="4c620-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="4c620-196">Администратор ссылок</span><span class="sxs-lookup"><span data-stu-id="4c620-196">Referrals admin</span></span>       |<span data-ttu-id="4c620-197">• Просмотр, создание и управление бизнес-профили</span><span class="sxs-lookup"><span data-stu-id="4c620-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="4c620-198">• Получать и управлять потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="4c620-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="4c620-199">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="4c620-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="4c620-200">Администратор бизнес-профиля</span><span class="sxs-lookup"><span data-stu-id="4c620-200">Business profile admin</span></span>   |<span data-ttu-id="4c620-201">•View, создавать и управлять бизнес-профиль</span><span class="sxs-lookup"><span data-stu-id="4c620-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="4c620-202">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="4c620-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="4c620-203">Управление поощрения (без AAD роли)</span><span class="sxs-lookup"><span data-stu-id="4c620-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="4c620-204">**Роли**</span><span class="sxs-lookup"><span data-stu-id="4c620-204">**Role**</span></span> | <span data-ttu-id="4c620-205">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="4c620-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="4c620-206">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="4c620-206">Incentives admin</span></span>|<span data-ttu-id="4c620-207">• Инициирует и управляет поощрения</span><span class="sxs-lookup"><span data-stu-id="4c620-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="4c620-208">• Можно просматривать и изменять все аспекты поощрения для программы</span><span class="sxs-lookup"><span data-stu-id="4c620-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="4c620-209">• Можно просматривать и изменять банковские и налоговые сведения</span><span class="sxs-lookup"><span data-stu-id="4c620-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="4c620-210">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="4c620-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4c620-211">• Поддержка доступа</span><span class="sxs-lookup"><span data-stu-id="4c620-211">• Access support</span></span>
||<span data-ttu-id="4c620-212">• Споров в отношении поощрения платежей</span><span class="sxs-lookup"><span data-stu-id="4c620-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="4c620-213">Пользователь программы поощрения</span><span class="sxs-lookup"><span data-stu-id="4c620-213">Incentives user</span></span>|<span data-ttu-id="4c620-214">• Можно просмотреть поощрения для программы</span><span class="sxs-lookup"><span data-stu-id="4c620-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="4c620-215">• Можно просматривать и инициировать поощрения утверждений</span><span class="sxs-lookup"><span data-stu-id="4c620-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="4c620-216">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="4c620-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4c620-217">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="4c620-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4c620-218">• Поддержка доступа</span><span class="sxs-lookup"><span data-stu-id="4c620-218">• Access support</span></span>












