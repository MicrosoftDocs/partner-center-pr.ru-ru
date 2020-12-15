---
title: Создание учетных записей пользователей и назначение ролей
description: Каждому сотруднику необходимо назначить роль, прежде чем он сможет получить доступ к Центру партнеров. Узнайте, как создавать учетные записи пользователей, назначать роли и задавать разрешения.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492540"
---
# <a name="create-user-accounts"></a><span data-ttu-id="ca2cf-104">Создание учетных записей пользователей</span><span class="sxs-lookup"><span data-stu-id="ca2cf-104">Create user accounts</span></span>  

<span data-ttu-id="ca2cf-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="ca2cf-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ca2cf-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="ca2cf-106">Account admin</span></span>
- <span data-ttu-id="ca2cf-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ca2cf-107">Global admin</span></span>
- <span data-ttu-id="ca2cf-108">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="ca2cf-108">User management admin</span></span>

<span data-ttu-id="ca2cf-109">Создайте учетные записи пользователей для сотрудников, которым требуется доступ к Центру партнеров.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="ca2cf-110">Эти задачи должны выполняться администратором управления пользователями, администратором учетных записей или глобальным администратором. Пользователю, выполняющему эти задачи, нужно назначить роль администратора или глобального администратора Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="ca2cf-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="ca2cf-111">См. сведения о [разрешениях ролей администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="ca2cf-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="ca2cf-112">Добавление нового пользователя</span><span class="sxs-lookup"><span data-stu-id="ca2cf-112">Add a new user</span></span>

1. <span data-ttu-id="ca2cf-113">Щелкните значок **Параметры** в правом верхнем углу Центра партнеров, выберите **Параметры учетной записи**, а затем — **Управление пользователями**.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="ca2cf-114">Выберите **Добавить пользователя**.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-114">Select **Add user**.</span></span>

3. <span data-ttu-id="ca2cf-115">Введите полное имя пользователя и уникальный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="ca2cf-116">Выберите тип агента и (или) тип администратора, который требуется назначить пользователю.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="ca2cf-117">Доступ в Центре партнеров зависит от ролей, поэтому можно назначить разрешения, чтобы настроить представление пользователя на отображение только функциональных возможностей, необходимых пользователю для выполнения определенных задач.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="ca2cf-118">Если пользователь хочет, чтобы ему назначили роль, ему нужно найти глобального администратора, перейдя в раздел **Управление пользователями** и выполнив фильтрацию по этой роли.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="ca2cf-119">Выберите **Добавить** для создания учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="ca2cf-120">Подтвердите сведения пользователя на следующей странице.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="ca2cf-121">Запомните или запишите данные для входа нового пользователя, отображаемые на этой странице.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="ca2cf-122">Не забудьте скопировать и отправить эти сведения для новых пользователей, так как вы не сможете получить к нему доступ позже.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="ca2cf-123">Пользователь должен войти в Центр партнеров с помощью имени пользователя и временного пароля.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="ca2cf-124">Когда пользователь входит в Центр партнеров в первый раз, будет предложено изменить свой пароль.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="ca2cf-125">Назначение ролей пользователей</span><span class="sxs-lookup"><span data-stu-id="ca2cf-125">Assign user roles</span></span>

<span data-ttu-id="ca2cf-126">Чтобы пользователь мог работать в Центре партнеров, ему должна быть назначена роль.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="ca2cf-127">В настоящее время роли включают в себя роли клиента Azure Active Directory, роли поставщика облачных решений (CSP) и роли компании, не связанные с AAD.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="ca2cf-128">Отдельная компания может нуждаться во всех этих ролях.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="ca2cf-129">Чтобы пользователи могли получить доступ к Центру партнеров, они должны быть указаны в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="ca2cf-130">Назначения ролей обеспечивают дополнительный доступ.</span><span class="sxs-lookup"><span data-stu-id="ca2cf-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ca2cf-131">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ca2cf-131">Next steps</span></span>

- [<span data-ttu-id="ca2cf-132">Назначение пользовательских ролей и разрешений сотрудникам для работы в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ca2cf-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
