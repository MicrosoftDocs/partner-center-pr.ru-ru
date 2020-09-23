---
title: Создание учетных записей пользователей и назначение ролей
description: Каждому сотруднику необходимо назначить роль, прежде чем он сможет получить доступ к Центру партнеров. Узнайте, как создавать учетные записи пользователей, назначать роли и задавать разрешения.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 637e88205d9944f7220e227b5101220d94ed42db
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000438"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="ab634-104">Создание учетных записей пользователей и назначение ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="ab634-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="ab634-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="ab634-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ab634-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="ab634-106">Account admin</span></span>
- <span data-ttu-id="ab634-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ab634-107">Global admin</span></span>
- <span data-ttu-id="ab634-108">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="ab634-108">User management admin</span></span>

<span data-ttu-id="ab634-109">Создайте учетные записи пользователей для сотрудников, которым требуется доступ к Центру партнеров.</span><span class="sxs-lookup"><span data-stu-id="ab634-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="ab634-110">Эти задачи должны выполняться администратором управления пользователями, администратором учетных записей или глобальным администратором. Пользователю, выполняющему эти задачи, нужно назначить роль администратора или глобального администратора Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="ab634-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="ab634-111">См. сведения о [разрешениях ролей администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="ab634-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="ab634-112">Добавление нового пользователя</span><span class="sxs-lookup"><span data-stu-id="ab634-112">Add a new user</span></span>

1. <span data-ttu-id="ab634-113">Щелкните значок **Параметры** в правом верхнем углу Центра партнеров и выберите **Управление пользователями**.</span><span class="sxs-lookup"><span data-stu-id="ab634-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="ab634-114">Выберите **Добавить пользователя**.</span><span class="sxs-lookup"><span data-stu-id="ab634-114">Select **Add user**.</span></span>

3. <span data-ttu-id="ab634-115">Введите полное имя пользователя и уникальный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ab634-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="ab634-116">Выберите тип агента и (или) тип администратора, который требуется назначить пользователю.</span><span class="sxs-lookup"><span data-stu-id="ab634-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="ab634-117">Доступ в Центре партнеров зависит от ролей, поэтому можно назначить разрешения, чтобы настроить представление пользователя на отображение только функциональных возможностей, необходимых пользователю для выполнения определенных задач.</span><span class="sxs-lookup"><span data-stu-id="ab634-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="ab634-118">Если пользователь хочет, чтобы ему назначили роль, ему нужно найти глобального администратора, перейдя в раздел **Управление пользователями** и выполнив фильтрацию по этой роли.</span><span class="sxs-lookup"><span data-stu-id="ab634-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="ab634-119">Выберите **Добавить** для создания учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab634-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="ab634-120">Подтвердите сведения пользователя на следующей странице.</span><span class="sxs-lookup"><span data-stu-id="ab634-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="ab634-121">Запомните или запишите данные для входа нового пользователя, отображаемые на этой странице.</span><span class="sxs-lookup"><span data-stu-id="ab634-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="ab634-122">Не забудьте скопировать и отправить эти сведения для новых пользователей, так как вы не сможете получить к нему доступ позже.</span><span class="sxs-lookup"><span data-stu-id="ab634-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="ab634-123">Пользователь должен войти в Центр партнеров с помощью имени пользователя и временного пароля.</span><span class="sxs-lookup"><span data-stu-id="ab634-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="ab634-124">Когда пользователь входит в Центр партнеров в первый раз, будет предложено изменить свой пароль.</span><span class="sxs-lookup"><span data-stu-id="ab634-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

## <a name="find-the-role-youve-been-assigned"></a><span data-ttu-id="ab634-125">Поиск назначенной роли</span><span class="sxs-lookup"><span data-stu-id="ab634-125">Find the role you've been assigned</span></span>

<span data-ttu-id="ab634-126">Если ваш глобальный администратор не сообщил, какая роль вам назначена, вы можете узнать это в Центре партнеров. Для этого сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="ab634-126">If your global admin hasn't told you, you can find out what role you have in Partner Center by doing the following:</span></span>

1. <span data-ttu-id="ab634-127">Войдите на [панель мониторинга]https://partner.microsoft.com/dashboard/home) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ab634-127">Sign into Partner Center [dashboard]https://partner.microsoft.com/dashboard/home).</span></span>

1. <span data-ttu-id="ab634-128">Щелкните значок **Параметры учетной записи** и выберите **Мой профиль**.</span><span class="sxs-lookup"><span data-stu-id="ab634-128">Select the **Account settings** icon and then select **My profile**.</span></span>
 
1. <span data-ttu-id="ab634-129">Откройте вкладку **Роли и разрешения**. Вы увидите свои роли и разрешения.</span><span class="sxs-lookup"><span data-stu-id="ab634-129">Select the **Roles and permissions** tab. You will see your roles and permissions.</span></span>
 

>[!Note]
><span data-ttu-id="ab634-130">Если при входе вы не видите программу, обычно это означает, что у вас нет нужных разрешений для работы с этой программой.</span><span class="sxs-lookup"><span data-stu-id="ab634-130">If you don't see a program when you sign in, it usually means you don't have the correct permissions to work in that program.</span></span> <span data-ttu-id="ab634-131">Например, если при входе вы не видите страницу Incentives, у вас нет соответствующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="ab634-131">So, for example, if you don't see the Incentives page when you sign in, you don't have Incentives permissions.</span></span> <span data-ttu-id="ab634-132">Глобальный администратор может предоставить вам необходимые разрешения.</span><span class="sxs-lookup"><span data-stu-id="ab634-132">Your global admin can give you needed permissions.</span></span>


## <a name="find-your-global-admin"></a><span data-ttu-id="ab634-133">Поиск глобального администратора</span><span class="sxs-lookup"><span data-stu-id="ab634-133">Find your global admin</span></span>

<span data-ttu-id="ab634-134">Иногда может потребоваться изменить роль имеющего пользователя или назначить определенную роль новому пользователю.</span><span class="sxs-lookup"><span data-stu-id="ab634-134">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="ab634-135">Чтобы найти глобального администратора, который может вносить изменения в роли или назначать роли новому пользователю, щелкните значок **Параметры учетной записи** в правом верхнем углу Центра партнеров, выберите **Управление пользователями** и выполните фильтрацию по роли глобального администратора. Вы также можете щелкнуть **Мой профиль**, выбрать **Роли и разрешения** и просмотреть список разных администраторов, которые могут помочь вам повысить уровень разрешений.</span><span class="sxs-lookup"><span data-stu-id="ab634-135">To find a global admin who can make role changes or assign roles to a new user, from the **Account settings icon** at the top right of the Partner Center, select **User management** and filter on global admin, or you can go to **My profile**, select **Roles and permissions** and see a list of the different admins who can help you elevate your permissions.</span></span> 


## <a name="new-global-admin"></a><span data-ttu-id="ab634-136">Новый глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ab634-136">New global admin</span></span>

<span data-ttu-id="ab634-137">Если ваш глобальный администратор покидает организацию и кому-то нужно занять его место, вы можете отправить запрос в команду Azure или Office 365.</span><span class="sxs-lookup"><span data-stu-id="ab634-137">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="ab634-138">Чтобы узнать, как это сделать, выберите один из вариантов ниже:</span><span class="sxs-lookup"><span data-stu-id="ab634-138">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="ab634-139">Новый глобальный администратор Azure</span><span class="sxs-lookup"><span data-stu-id="ab634-139">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="ab634-140">Новый глобальный администратор Office 365</span><span class="sxs-lookup"><span data-stu-id="ab634-140">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="ab634-141">Назначение ролей пользователей</span><span class="sxs-lookup"><span data-stu-id="ab634-141">Assign user roles</span></span>

<span data-ttu-id="ab634-142">Чтобы пользователь мог работать в Центре партнеров, ему должна быть назначена роль.</span><span class="sxs-lookup"><span data-stu-id="ab634-142">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="ab634-143">В настоящее время роли включают в себя роли клиента Azure Active Directory, роли поставщика облачных решений (CSP) и роли компании, не связанные с AAD.</span><span class="sxs-lookup"><span data-stu-id="ab634-143">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="ab634-144">Отдельная компания может нуждаться во всех этих ролях.</span><span class="sxs-lookup"><span data-stu-id="ab634-144">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="ab634-145">Чтобы пользователи могли получить доступ к Центру партнеров, они должны быть указаны в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="ab634-145">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="ab634-146">Назначения ролей обеспечивают дополнительный доступ.</span><span class="sxs-lookup"><span data-stu-id="ab634-146">Role assignments provide additional access.</span></span>


<span data-ttu-id="ab634-147">**Роли клиента AAD**:</span><span class="sxs-lookup"><span data-stu-id="ab634-147">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="ab634-148">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ab634-148">Global admin</span></span>
- <span data-ttu-id="ab634-149">администратор пользователей.</span><span class="sxs-lookup"><span data-stu-id="ab634-149">User admin</span></span>

<span data-ttu-id="ab634-150">**Роли CSP**:</span><span class="sxs-lookup"><span data-stu-id="ab634-150">**CSP roles include**:</span></span>
- <span data-ttu-id="ab634-151">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="ab634-151">Admin agent</span></span>
- <span data-ttu-id="ab634-152">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="ab634-152">Billing admin</span></span>
- <span data-ttu-id="ab634-153">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="ab634-153">Sales agent</span></span>
- <span data-ttu-id="ab634-154">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="ab634-154">Helpdesk agent</span></span>

<span data-ttu-id="ab634-155">**Роли, управляющие членством в MPN и организацией (не связанные с AAD)** :</span><span class="sxs-lookup"><span data-stu-id="ab634-155">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="ab634-156">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="ab634-156">MPN partner admin</span></span>
- <span data-ttu-id="ab634-157">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="ab634-157">Account admin</span></span>
- <span data-ttu-id="ab634-158">администратор рекомендаций;</span><span class="sxs-lookup"><span data-stu-id="ab634-158">Referral admin</span></span>
- <span data-ttu-id="ab634-159">Администратор бизнес-профиля</span><span class="sxs-lookup"><span data-stu-id="ab634-159">Business profile admin</span></span>
- <span data-ttu-id="ab634-160">администратор поощрений и пользователь.</span><span class="sxs-lookup"><span data-stu-id="ab634-160">Incentives admin and user</span></span>

<span data-ttu-id="ab634-161">**Роль поставщика панели управления (это CSP и роль, не связанная с AAD)** :</span><span class="sxs-lookup"><span data-stu-id="ab634-161">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="ab634-162">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ab634-162">Global admin</span></span>

<span data-ttu-id="ab634-163">**Гостевой пользователь** должен быть частью клиента AAD и может иметь любые роли, не связанные с AAD.</span><span class="sxs-lookup"><span data-stu-id="ab634-163">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="ab634-164">Более подробные сведения о ролях и возможностях каждой из них см. в статье [Назначение пользователям ролей и разрешений](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="ab634-164">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="ab634-165">Связывание учетной записи пользователя Microsoft Learn с Центром партнеров</span><span class="sxs-lookup"><span data-stu-id="ab634-165">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="ab634-166">Чтобы увидеть пути обучения, которые ваши пользователи проходят для получения компетенций, им необходимо связать свой идентификатор MCP с учетной записью Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ab634-166">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="ab634-167">При добавлении новых пользователей вам, как глобальному администратору, нужно напомнить им о необходимости связать идентификатор MCP с их учетной записью.</span><span class="sxs-lookup"><span data-stu-id="ab634-167">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="ab634-168">Связывание идентификатора MCP с учетной записью Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="ab634-168">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="ab634-169">В правом углу Панели мониторинга Центра партнеров щелкните значок **Your account** (Ваша учетная запись), а затем выберите **My profile** (Мой профиль).</span><span class="sxs-lookup"><span data-stu-id="ab634-169">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="ab634-170">В разделе **Your learning** (Ваше обучение) вы сможете привязать свою учетную запись Microsoft Learning, а также подключить учетную запись Майкрософт к Partner University.</span><span class="sxs-lookup"><span data-stu-id="ab634-170">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ab634-171">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ab634-171">Next steps</span></span>

- [<span data-ttu-id="ab634-172">Назначение ролей и разрешений пользователям компании для работы в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ab634-172">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)