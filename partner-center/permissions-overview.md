---
title: Назначение пользователям ролей и разрешений | Центр партнеров
ms.topic: article
ms.date: 3/5/19
description: Каждому сотруднику, которому нужен для работы в партнерском центре должна быть назначена роль.
author: LauraBrenner
ms.author: labrenne
keywords: роли, разрешения, администратор, агент
ms.localizationpriority: medium
ms.openlocfilehash: 65a2f7f373fc57f86cfffa73aafd3b7095fe2c04
ms.sourcegitcommit: be8086534ec73937f2be9bcc495c2627423c50f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "67396726"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="704bc-104">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="704bc-104">Assign users roles and permissions</span></span>


<span data-ttu-id="704bc-105">Вы настроили профиль партнера, включая юридическое название и адрес, сведения о поддержке, налог исключения файла, bank info и основного контактного лица для вашей компании.</span><span class="sxs-lookup"><span data-stu-id="704bc-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="704bc-106">Следующий шаг: настройка с паролями, а также роли, чтобы они могли начать работу в центре партнеров с вами пользователи.</span><span class="sxs-lookup"><span data-stu-id="704bc-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="704bc-107">Настройка сотрудников для работы в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="704bc-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="704bc-108">Вы определите типы доступа пользователей к центра партнеров, роли и разрешения, которые вы не предоставите им.</span><span class="sxs-lookup"><span data-stu-id="704bc-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="704bc-109">Роли, связаны с исполняемом формате, который вашего бизнеса участвует в.</span><span class="sxs-lookup"><span data-stu-id="704bc-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="704bc-110">Например, если вашего бизнеса — это поставщик облачных решений (CSP), вы не только будет standard Azure AD роли управления, такие как глобальный администратор клиента, но потребуется роли относятся к программе CSP.</span><span class="sxs-lookup"><span data-stu-id="704bc-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="704bc-111">Каждая программа имеет роли, относящиеся к ней.</span><span class="sxs-lookup"><span data-stu-id="704bc-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="704bc-112">Роли клиента Azure Active Directory (AAD) включают глобального администратора, администратора пользователей и ролей CSP.</span><span class="sxs-lookup"><span data-stu-id="704bc-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="704bc-113">Роли AAD не являются ролей, которые не управление клиентом и включают администратора MPN, бизнеса профиль администратора, администратора ссылок, стимулирования администратора и стимулирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="704bc-113">Non-AAD roles are those roles that do not manage the tenant and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="704bc-114">Управление коммерческих транзакций в центре партнеров (Azure AD и ролей CSP)</span><span class="sxs-lookup"><span data-stu-id="704bc-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="704bc-115">**Роли**</span><span class="sxs-lookup"><span data-stu-id="704bc-115">**Role**</span></span>|<span data-ttu-id="704bc-116">**Их возможности**</span><span class="sxs-lookup"><span data-stu-id="704bc-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="704bc-117">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="704bc-117">Global admin</span></span>|<span data-ttu-id="704bc-118">• Можно получить доступ к учетной записи или службы Майкрософт с административными полномочиями</span><span class="sxs-lookup"><span data-stu-id="704bc-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="704bc-119">• Создание запросов в службу поддержки для центра партнеров</span><span class="sxs-lookup"><span data-stu-id="704bc-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="704bc-120">• Представление соглашения, прайс-листы и предложения</span><span class="sxs-lookup"><span data-stu-id="704bc-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="704bc-121">• Просмотр, создание и управление пользователей партнера</span><span class="sxs-lookup"><span data-stu-id="704bc-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="704bc-122">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="704bc-122">User Admin</span></span>   | <span data-ttu-id="704bc-123">• Просмотр, создание и управление пользователями</span><span class="sxs-lookup"><span data-stu-id="704bc-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="704bc-124">• Просмотреть все профили партнеров</span><span class="sxs-lookup"><span data-stu-id="704bc-124">• View all partner profiles</span></span>
||<span data-ttu-id="704bc-125">• Просмотр, создание и управление пользователей партнера</span><span class="sxs-lookup"><span data-stu-id="704bc-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="704bc-126">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="704bc-126">Billing admin</span></span> | <span data-ttu-id="704bc-127">— Просмотр, создание и управление выставлением счетов, счета-фактуры и проверка файлов</span><span class="sxs-lookup"><span data-stu-id="704bc-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="704bc-128">Пользователь по умолчанию</span><span class="sxs-lookup"><span data-stu-id="704bc-128">Default user</span></span>|  <span data-ttu-id="704bc-129">Просмотреть мой профиль</span><span class="sxs-lookup"><span data-stu-id="704bc-129">View My profile</span></span>   |
|<span data-ttu-id="704bc-130">Агент администрирования</span><span class="sxs-lookup"><span data-stu-id="704bc-130">Admin agent</span></span> | <span data-ttu-id="704bc-131">• Управление клиентами</span><span class="sxs-lookup"><span data-stu-id="704bc-131">•    Customer management</span></span>
||<span data-ttu-id="704bc-132">• Добавьте список устройств для центра партнеров <</span><span class="sxs-lookup"><span data-stu-id="704bc-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="704bc-133">• Создание и применение профилей на устройствах</span><span class="sxs-lookup"><span data-stu-id="704bc-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="704bc-134">• Управление подпиской</span><span class="sxs-lookup"><span data-stu-id="704bc-134">• Subscription management</span></span>
||<span data-ttu-id="704bc-135">• Служба работоспособности запросы и службы для клиентов</span><span class="sxs-lookup"><span data-stu-id="704bc-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="704bc-136">• Запрос делегирования привилегий администратора</span><span class="sxs-lookup"><span data-stu-id="704bc-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="704bc-137">• Просмотреть цены и предложения</span><span class="sxs-lookup"><span data-stu-id="704bc-137">• View pricing and offers</span></span>
||<span data-ttu-id="704bc-138">• Выставления счетов</span><span class="sxs-lookup"><span data-stu-id="704bc-138">• Billing</span></span>
||<span data-ttu-id="704bc-139">• Администрирование от имени клиента</span><span class="sxs-lookup"><span data-stu-id="704bc-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="704bc-140">• Register значение добавлены торгового посредника</span><span class="sxs-lookup"><span data-stu-id="704bc-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="704bc-141">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="704bc-141">Sales agent</span></span> | <span data-ttu-id="704bc-142">• Управление клиентами</span><span class="sxs-lookup"><span data-stu-id="704bc-142">•    Customer management</span></span>
||<span data-ttu-id="704bc-143">• Добавьте список устройств для центра партнеров</span><span class="sxs-lookup"><span data-stu-id="704bc-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="704bc-144">• Управление подпиской</span><span class="sxs-lookup"><span data-stu-id="704bc-144">• Subscription management</span></span>
||<span data-ttu-id="704bc-145">• Цена представлении перечислены и предлагает</span><span class="sxs-lookup"><span data-stu-id="704bc-145">• View price lists and offers</span></span>
||<span data-ttu-id="704bc-146">• Запросы в службу поддержки представления</span><span class="sxs-lookup"><span data-stu-id="704bc-146">• View support tickets</span></span>
||<span data-ttu-id="704bc-147">• Запрос связь с клиентом</span><span class="sxs-lookup"><span data-stu-id="704bc-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="704bc-148">• Управление интересов</span><span class="sxs-lookup"><span data-stu-id="704bc-148">• Manage customer leads</span></span>
||<span data-ttu-id="704bc-149">Представления • соглашении клиента</span><span class="sxs-lookup"><span data-stu-id="704bc-149">• View the customer agreement</span></span>
||<span data-ttu-id="704bc-150">• Register системного интегратора</span><span class="sxs-lookup"><span data-stu-id="704bc-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="704bc-151">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="704bc-151">Helpdesk agent</span></span>| <span data-ttu-id="704bc-152">• Поиск и просмотр клиента</span><span class="sxs-lookup"><span data-stu-id="704bc-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="704bc-153">• Изменение клиента сведений</span><span class="sxs-lookup"><span data-stu-id="704bc-153">• Edit customer details</span></span>
||<span data-ttu-id="704bc-154">• Справка устранить проблемы клиентов с помощью управления выставления счета или подписки</span><span class="sxs-lookup"><span data-stu-id="704bc-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="704bc-155">• Поддержка запросов от имени клиентов (Примечание: Должен быть агент администратора для выполнения этой задачи для подписки на Office 365)</span><span class="sxs-lookup"><span data-stu-id="704bc-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="704bc-156">• Управление подписками и выставления счетов проблемы от имени клиентов (Примечание: Должен быть агент администратора для выполнения этой задачи для подписки на Office 365)</span><span class="sxs-lookup"><span data-stu-id="704bc-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="704bc-157">Поставщик панели управления (CPV).</span><span class="sxs-lookup"><span data-stu-id="704bc-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="704bc-158">(Роль CSP и роли не AAD)</span><span class="sxs-lookup"><span data-stu-id="704bc-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="704bc-159">CPVs разработка приложений для использования с партнеров поставщика облачных решений (CSP), чтобы включить их для интеграции своих систем с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="704bc-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="704bc-160">**Роли**</span><span class="sxs-lookup"><span data-stu-id="704bc-160">**Role**</span></span>   |<span data-ttu-id="704bc-161">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="704bc-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="704bc-162">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="704bc-162">Global admin</span></span>| <span data-ttu-id="704bc-163">Просмотр и Управление профилем CPV</span><span class="sxs-lookup"><span data-stu-id="704bc-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="704bc-164">Просматривать и управлять любыми пользователями, которым требуется доступ к возможностям CPV</span><span class="sxs-lookup"><span data-stu-id="704bc-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="704bc-165">Гостевой пользователь (необходимо добавить в клиент AAD)</span><span class="sxs-lookup"><span data-stu-id="704bc-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="704bc-166">**Гостевой пользователь**</span><span class="sxs-lookup"><span data-stu-id="704bc-166">**Guest user**</span></span>   | <span data-ttu-id="704bc-167">**Роли**</span><span class="sxs-lookup"><span data-stu-id="704bc-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="704bc-168">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="704bc-168">MPN partner admin</span></span>|
||<span data-ttu-id="704bc-169">Учетные записи администратора</span><span class="sxs-lookup"><span data-stu-id="704bc-169">Accounts admin</span></span>|
||<span data-ttu-id="704bc-170">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="704bc-170">Incentives admin</span></span>|
||<span data-ttu-id="704bc-171">Администратор бизнес-профиля</span><span class="sxs-lookup"><span data-stu-id="704bc-171">Business profile admin</span></span>|
||<span data-ttu-id="704bc-172">Администратор ссылок</span><span class="sxs-lookup"><span data-stu-id="704bc-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="704bc-173">Управлять членством в MPN и вашей компании (роли не AAD: эти роли для управления бизнес-деятельности компании, а не клиента)</span><span class="sxs-lookup"><span data-stu-id="704bc-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="704bc-174">**Роли**</span><span class="sxs-lookup"><span data-stu-id="704bc-174">**Role**</span></span> | <span data-ttu-id="704bc-175">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="704bc-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="704bc-176">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="704bc-176">MPN partner admin</span></span>|<span data-ttu-id="704bc-177">•CAN Добавление пользователей не клиентами</span><span class="sxs-lookup"><span data-stu-id="704bc-177">•Can add non-tenant users</span></span>
||<span data-ttu-id="704bc-178">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="704bc-178">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="704bc-179">• Представление юридические, организации, бизнеса и профили MPN</span><span class="sxs-lookup"><span data-stu-id="704bc-179">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="704bc-180">• Просмотр сведений о пользователях и навыки работы с ними данных</span><span class="sxs-lookup"><span data-stu-id="704bc-180">• View user details and their skills data</span></span>
||<span data-ttu-id="704bc-181">• Просмотр компетенций</span><span class="sxs-lookup"><span data-stu-id="704bc-181">• View competencies</span></span>
||<span data-ttu-id="704bc-182">• Просмотр и управление ими преимущества</span><span class="sxs-lookup"><span data-stu-id="704bc-182">• View and manage benefits</span></span>
||<span data-ttu-id="704bc-183">• Представление и покупку MPN предлагает</span><span class="sxs-lookup"><span data-stu-id="704bc-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="704bc-184">• Представление MPN предлагает историю заказов и счета-фактуры</span><span class="sxs-lookup"><span data-stu-id="704bc-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="704bc-185">• Просмотр партнера вклад данных</span><span class="sxs-lookup"><span data-stu-id="704bc-185">• View partner contribution data</span></span>
||<span data-ttu-id="704bc-186">• Можно работать в средстве проверки ваучер</span><span class="sxs-lookup"><span data-stu-id="704bc-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="704bc-187">— Просмотр данных аналитики клиента</span><span class="sxs-lookup"><span data-stu-id="704bc-187">- View customer data analytics</span></span>
|<span data-ttu-id="704bc-188">Администрирование учетных записей</span><span class="sxs-lookup"><span data-stu-id="704bc-188">Account admin</span></span>| <span data-ttu-id="704bc-189">• Можно добавить пользователей не клиентами</span><span class="sxs-lookup"><span data-stu-id="704bc-189">•   Can add non-tenant users</span></span>
||<span data-ttu-id="704bc-190">• Добавление или удаление расположений</span><span class="sxs-lookup"><span data-stu-id="704bc-190">• Add or delete locations</span></span>
||<span data-ttu-id="704bc-191">-Управление профилями, связанные с учетными записями, которые вы являетесь администратором для</span><span class="sxs-lookup"><span data-stu-id="704bc-191">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="704bc-192">• Назначение ролей для пользователей в клиенте для роли не AAD</span><span class="sxs-lookup"><span data-stu-id="704bc-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="704bc-193">• Расположений в программы регистрации</span><span class="sxs-lookup"><span data-stu-id="704bc-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="704bc-194">Управлять потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="704bc-194">Manage referrals</span></span> 

|<span data-ttu-id="704bc-195">**Роли**</span><span class="sxs-lookup"><span data-stu-id="704bc-195">**Role**</span></span>|<span data-ttu-id="704bc-196">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="704bc-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="704bc-197">Администратор ссылок</span><span class="sxs-lookup"><span data-stu-id="704bc-197">Referrals admin</span></span>       |<span data-ttu-id="704bc-198">• Просмотр, создание и управление бизнес-профили</span><span class="sxs-lookup"><span data-stu-id="704bc-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="704bc-199">• Получать и управлять потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="704bc-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="704bc-200">• Просмотр, создание и управление совместных ссылок</span><span class="sxs-lookup"><span data-stu-id="704bc-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="704bc-201">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="704bc-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="704bc-202">Администратор бизнес-профиля</span><span class="sxs-lookup"><span data-stu-id="704bc-202">Business profile admin</span></span>   |<span data-ttu-id="704bc-203">• Просмотр, создание и управление бизнес-профиль</span><span class="sxs-lookup"><span data-stu-id="704bc-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="704bc-204">• Представления, создание и управление запросами на обслуживание партнера</span><span class="sxs-lookup"><span data-stu-id="704bc-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="704bc-205">Управление поощрения</span><span class="sxs-lookup"><span data-stu-id="704bc-205">Manage incentives</span></span> 

|<span data-ttu-id="704bc-206">**Роли**</span><span class="sxs-lookup"><span data-stu-id="704bc-206">**Role**</span></span> | <span data-ttu-id="704bc-207">**Что делать**</span><span class="sxs-lookup"><span data-stu-id="704bc-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="704bc-208">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="704bc-208">Incentives admin</span></span>|<span data-ttu-id="704bc-209">• Инициирует и управляет поощрения</span><span class="sxs-lookup"><span data-stu-id="704bc-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="704bc-210">• Можно просматривать и изменять все аспекты поощрения для программы</span><span class="sxs-lookup"><span data-stu-id="704bc-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="704bc-211">• Можно просматривать и изменять банковские и налоговые сведения</span><span class="sxs-lookup"><span data-stu-id="704bc-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="704bc-212">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="704bc-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="704bc-213">• Поддержка доступа</span><span class="sxs-lookup"><span data-stu-id="704bc-213">• Access support</span></span>
||<span data-ttu-id="704bc-214">• Споров в отношении поощрения платежей</span><span class="sxs-lookup"><span data-stu-id="704bc-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="704bc-215">Пользователь программы поощрения</span><span class="sxs-lookup"><span data-stu-id="704bc-215">Incentives user</span></span>|<span data-ttu-id="704bc-216">• Можно просмотреть поощрения для программы</span><span class="sxs-lookup"><span data-stu-id="704bc-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="704bc-217">• Можно просматривать и инициировать поощрения утверждений</span><span class="sxs-lookup"><span data-stu-id="704bc-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="704bc-218">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="704bc-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="704bc-219">Представления • бонус и кооперативного прибыль</span><span class="sxs-lookup"><span data-stu-id="704bc-219">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="704bc-220">• Поддержка доступа</span><span class="sxs-lookup"><span data-stu-id="704bc-220">• Access support</span></span>












