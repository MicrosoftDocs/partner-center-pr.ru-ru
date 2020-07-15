---
title: Создание учетных записей пользователей и назначение ролей
description: Каждому сотруднику необходимо назначить роль, прежде чем он сможет получить доступ к Центру партнеров. Узнайте, как создавать учетные записи пользователей, назначать роли и задавать разрешения.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
Keywords: роли, разрешения, добавление пользователя, назначение роли, администратор, агент,
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 9ec8e98f77d49e34b6747b0f580502e9df25a950
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265200"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="8e331-105">Создание учетных записей пользователей и назначение ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="8e331-105">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="8e331-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="8e331-106">**Appropriate roles**</span></span>

- <span data-ttu-id="8e331-107">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="8e331-107">Account admin</span></span>
- <span data-ttu-id="8e331-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8e331-108">Global admin</span></span>
- <span data-ttu-id="8e331-109">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="8e331-109">User management admin</span></span>

<span data-ttu-id="8e331-110">Создайте учетные записи пользователей для сотрудников, которым требуется доступ к Центру партнеров.</span><span class="sxs-lookup"><span data-stu-id="8e331-110">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="8e331-111">Эти задачи должны выполняться администратором управления пользователями, администратором учетных записей или глобальным администратором. Пользователю, выполняющему эти задачи, нужно назначить роль администратора или глобального администратора Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="8e331-111">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="8e331-112">См. сведения о [разрешениях ролей администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="8e331-112">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="8e331-113">Добавление нового пользователя</span><span class="sxs-lookup"><span data-stu-id="8e331-113">Add a new user</span></span>

1. <span data-ttu-id="8e331-114">Щелкните значок **Параметры** в правом верхнем углу Центра партнеров и выберите **Управление пользователями**.</span><span class="sxs-lookup"><span data-stu-id="8e331-114">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="8e331-115">Выберите **Добавить пользователя**.</span><span class="sxs-lookup"><span data-stu-id="8e331-115">Select **Add user**.</span></span>

3. <span data-ttu-id="8e331-116">Введите полное имя пользователя и уникальный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8e331-116">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="8e331-117">Выберите тип агента и (или) тип администратора, который требуется назначить пользователю.</span><span class="sxs-lookup"><span data-stu-id="8e331-117">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="8e331-118">Доступ в Центре партнеров зависит от ролей, поэтому можно назначить разрешения, чтобы настроить представление пользователя на отображение только функциональных возможностей, необходимых пользователю для выполнения определенных задач.</span><span class="sxs-lookup"><span data-stu-id="8e331-118">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="8e331-119">Если пользователь хочет, чтобы ему назначили роль, ему нужно найти глобального администратора, перейдя в раздел **Управление пользователями** и выполнив фильтрацию по этой роли.</span><span class="sxs-lookup"><span data-stu-id="8e331-119">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="8e331-120">Выберите **Добавить** для создания учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e331-120">Select **Add** to create the user account.</span></span> <span data-ttu-id="8e331-121">Подтвердите сведения пользователя на следующей странице.</span><span class="sxs-lookup"><span data-stu-id="8e331-121">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="8e331-122">Запомните или запишите данные для входа нового пользователя, отображаемые на этой странице.</span><span class="sxs-lookup"><span data-stu-id="8e331-122">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="8e331-123">Не забудьте скопировать и отправить эти сведения для новых пользователей, так как вы не сможете получить к нему доступ позже.</span><span class="sxs-lookup"><span data-stu-id="8e331-123">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="8e331-124">Пользователь должен войти в Центр партнеров с помощью имени пользователя и временного пароля.</span><span class="sxs-lookup"><span data-stu-id="8e331-124">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="8e331-125">Когда пользователь входит в Центр партнеров в первый раз, будет предложено изменить свой пароль.</span><span class="sxs-lookup"><span data-stu-id="8e331-125">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="8e331-126">Поиск глобального администратора</span><span class="sxs-lookup"><span data-stu-id="8e331-126">Find your global admin</span></span>

<span data-ttu-id="8e331-127">Иногда может потребоваться изменить роль имеющего пользователя или назначить определенную роль новому пользователю.</span><span class="sxs-lookup"><span data-stu-id="8e331-127">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="8e331-128">Чтобы найти глобального администратора, который может вносить изменения в роль или назначать роли новому пользователю, щелкните значок **Параметры** в правом верхнем углу Центра партнеров, выберите **Управление пользователями** и выполните фильтрацию по роли глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="8e331-128">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="8e331-129">Новый глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8e331-129">New global admin</span></span>

<span data-ttu-id="8e331-130">Если ваш глобальный администратор покидает организацию и кому-то нужно занять его место, вы можете отправить запрос в команду Azure или Office 365.</span><span class="sxs-lookup"><span data-stu-id="8e331-130">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="8e331-131">Чтобы узнать, как это сделать, выберите один из вариантов ниже:</span><span class="sxs-lookup"><span data-stu-id="8e331-131">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="8e331-132">Новый глобальный администратор Azure</span><span class="sxs-lookup"><span data-stu-id="8e331-132">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="8e331-133">Новый глобальный администратор Office 365</span><span class="sxs-lookup"><span data-stu-id="8e331-133">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="8e331-134">Назначение ролей пользователей</span><span class="sxs-lookup"><span data-stu-id="8e331-134">Assign user roles</span></span>

<span data-ttu-id="8e331-135">Чтобы пользователь мог работать в Центре партнеров, ему должна быть назначена роль.</span><span class="sxs-lookup"><span data-stu-id="8e331-135">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="8e331-136">В настоящее время роли включают в себя роли клиента Azure Active Directory, роли поставщика облачных решений (CSP) и роли компании, не связанные с AAD.</span><span class="sxs-lookup"><span data-stu-id="8e331-136">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="8e331-137">Отдельная компания может нуждаться во всех этих ролях.</span><span class="sxs-lookup"><span data-stu-id="8e331-137">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="8e331-138">Чтобы пользователи могли получить доступ к Центру партнеров, они должны быть указаны в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="8e331-138">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="8e331-139">Назначения ролей обеспечивают дополнительный доступ.</span><span class="sxs-lookup"><span data-stu-id="8e331-139">Role assignments provide additional access.</span></span>


<span data-ttu-id="8e331-140">**Роли клиента AAD**:</span><span class="sxs-lookup"><span data-stu-id="8e331-140">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="8e331-141">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8e331-141">Global admin</span></span>
- <span data-ttu-id="8e331-142">администратор пользователей.</span><span class="sxs-lookup"><span data-stu-id="8e331-142">User admin</span></span>

<span data-ttu-id="8e331-143">**Роли CSP**:</span><span class="sxs-lookup"><span data-stu-id="8e331-143">**CSP roles include**:</span></span>
- <span data-ttu-id="8e331-144">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="8e331-144">Admin agent</span></span>
- <span data-ttu-id="8e331-145">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="8e331-145">Billing admin</span></span>
- <span data-ttu-id="8e331-146">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="8e331-146">Sales agent</span></span>
- <span data-ttu-id="8e331-147">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="8e331-147">Helpdesk agent</span></span>

<span data-ttu-id="8e331-148">**Роли, управляющие членством в MPN и организацией (не связанные с AAD)** :</span><span class="sxs-lookup"><span data-stu-id="8e331-148">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="8e331-149">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="8e331-149">MPN partner admin</span></span>
- <span data-ttu-id="8e331-150">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="8e331-150">Account admin</span></span>
- <span data-ttu-id="8e331-151">администратор рекомендаций;</span><span class="sxs-lookup"><span data-stu-id="8e331-151">Referral admin</span></span>
- <span data-ttu-id="8e331-152">Администратор бизнес-профиля</span><span class="sxs-lookup"><span data-stu-id="8e331-152">Business profile admin</span></span>
- <span data-ttu-id="8e331-153">администратор поощрений и пользователь.</span><span class="sxs-lookup"><span data-stu-id="8e331-153">Incentives admin and user</span></span>

<span data-ttu-id="8e331-154">**Роль поставщика панели управления (это CSP и роль, не связанная с AAD)** :</span><span class="sxs-lookup"><span data-stu-id="8e331-154">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="8e331-155">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8e331-155">Global admin</span></span>

<span data-ttu-id="8e331-156">**Гостевой пользователь** должен быть частью клиента AAD и может иметь любые роли, не связанные с AAD.</span><span class="sxs-lookup"><span data-stu-id="8e331-156">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="8e331-157">Более подробные сведения о ролях и возможностях каждой из них см. в статье [Назначение пользователям ролей и разрешений](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8e331-157">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="8e331-158">Связывание учетной записи пользователя Microsoft Learn с Центром партнеров</span><span class="sxs-lookup"><span data-stu-id="8e331-158">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="8e331-159">Чтобы увидеть пути обучения, которые ваши пользователи проходят для получения компетенций, им необходимо связать свой идентификатор MCP с учетной записью Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="8e331-159">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="8e331-160">При добавлении новых пользователей вам, как глобальному администратору, нужно напомнить им о необходимости связать идентификатор MCP с их учетной записью.</span><span class="sxs-lookup"><span data-stu-id="8e331-160">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="8e331-161">Связывание идентификатора MCP с учетной записью Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="8e331-161">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="8e331-162">В правом углу Панели мониторинга Центра партнеров щелкните значок **Your account** (Ваша учетная запись), а затем выберите **My profile** (Мой профиль).</span><span class="sxs-lookup"><span data-stu-id="8e331-162">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="8e331-163">В разделе **Your learning** (Ваше обучение) вы сможете привязать свою учетную запись Microsoft Learning, а также подключить учетную запись Майкрософт к Partner University.</span><span class="sxs-lookup"><span data-stu-id="8e331-163">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>
