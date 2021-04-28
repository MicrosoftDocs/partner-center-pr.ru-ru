---
title: Поиск идентификатора клиента, доменного имени, идентификатора объекта пользователя
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как найти идентификаторы в портал Azure — идентификатор клиента Azure AD в Организации, доменное имя или идентификатор конкретного объекта пользователя. Для некоторых задач требуются эти сведения.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172257"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="7724f-104">Поиск важных идентификаторов для пользователя</span><span class="sxs-lookup"><span data-stu-id="7724f-104">Locate important IDs for a user</span></span>

<span data-ttu-id="7724f-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="7724f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7724f-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7724f-106">Global admin</span></span>

<span data-ttu-id="7724f-107">В этой статье описывается, как использовать [портал Azure](https://portal.azure.com/) для выявления следующих сведений для пользователя:</span><span class="sxs-lookup"><span data-stu-id="7724f-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="7724f-108">Идентификатор клиента Microsoft Azure Active Directory (Azure AD) для организации или компании пользователя.</span><span class="sxs-lookup"><span data-stu-id="7724f-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="7724f-109">Основное доменное имя организации или компании, связанной с клиентом Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7724f-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="7724f-110">Идентификатор объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="7724f-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="7724f-111">Поиск идентификатора клиента Microsoft Azure AD и основного доменного имени</span><span class="sxs-lookup"><span data-stu-id="7724f-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="7724f-112">Выполните следующие действия, чтобы указать идентификатор клиента Azure AD или имя основного домена в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="7724f-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="7724f-113">(Если вы хотите найти идентификатор клиента программно, см. раздел [Поиск идентификатора клиента с помощью PowerShell или интерфейса командной строки](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="7724f-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="7724f-114">Идентификатор клиента может называться разными именами в разных приложениях или ресурсах.</span><span class="sxs-lookup"><span data-stu-id="7724f-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="7724f-115">Например, идентификатор клиента может называться ИДЕНТИФИКАТОРом каталога, клиентом Azure Active Directory (Azure AD), ИДЕНТИФИКАТОРом Microsoft или для определенных отчетов, даже *тенантгуид*.</span><span class="sxs-lookup"><span data-stu-id="7724f-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="7724f-116">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7724f-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7724f-117">Выберите **Azure Active Directory** в меню.</span><span class="sxs-lookup"><span data-stu-id="7724f-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Показывает портал Azure выборе параметра Azure Active Directory в меню.":::

3. <span data-ttu-id="7724f-119">Откроется страница **обзора** Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7724f-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="7724f-120">Чтобы найти идентификатор клиента Azure AD или имя основного домена, найдите поле " **идентификатор клиента** " и поле " **основной домен** ".</span><span class="sxs-lookup"><span data-stu-id="7724f-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="7724f-121">Эти поля отображаются в разделе сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="7724f-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Отображает страницу обзора с двумя выделенными полями, ИДЕНТИФИКАТОРом клиента и именем основного домена.":::

4. <span data-ttu-id="7724f-123">Идентификатор клиента можно найти в портал Azure несколькими другими способами.</span><span class="sxs-lookup"><span data-stu-id="7724f-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="7724f-124">Выберите **Azure Active Directory** в меню.</span><span class="sxs-lookup"><span data-stu-id="7724f-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="7724f-125">Затем в меню найдите раздел **Управление** и выберите пункт **свойства**.</span><span class="sxs-lookup"><span data-stu-id="7724f-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="7724f-126">На странице свойств также отображается связанный с пользователем идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="7724f-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Отображает страницу свойств с выделенным полем &quot;идентификатор клиента&quot;.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="7724f-128">Поиск идентификатора объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="7724f-128">Find the user object ID</span></span>

<span data-ttu-id="7724f-129">Просто найти доменное имя и идентификатор клиента может быть не всегда достаточно.</span><span class="sxs-lookup"><span data-stu-id="7724f-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="7724f-130">Также может потребоваться указать идентификатор объекта, назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="7724f-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="7724f-131">Выполните следующие действия, чтобы найти идентификатор объекта пользователя в портал Azure:</span><span class="sxs-lookup"><span data-stu-id="7724f-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="7724f-132">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7724f-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7724f-133">Выберите **Azure Active Directory** в меню.</span><span class="sxs-lookup"><span data-stu-id="7724f-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="7724f-134">Найдите в меню раздел **Управление** , а затем выберите **Пользователи**.</span><span class="sxs-lookup"><span data-stu-id="7724f-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Отображает Azure Active Directory меню с выделенным, параметром пользователи.":::

4. <span data-ttu-id="7724f-136">На странице Пользователи введите имя пользователя в поле поиска.</span><span class="sxs-lookup"><span data-stu-id="7724f-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Отображает страницу пользователей с полем поиска для поиска определенного пользователя.":::

5. <span data-ttu-id="7724f-138">Выберите имя пользователя, где он отображается в списке.</span><span class="sxs-lookup"><span data-stu-id="7724f-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Показывает пользовательскую страницу, отображающую строку для искомого пользователя.":::

6. <span data-ttu-id="7724f-140">На странице профиля пользователя откройте раздел удостоверение.</span><span class="sxs-lookup"><span data-stu-id="7724f-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="7724f-141">Поле "идентификатор объекта" отображается здесь с уникальным ИДЕНТИФИКАТОРом объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="7724f-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Отображает страницу профиля пользователя с разделом Identity и одно выделенное поле для идентификатора объекта.":::

## <a name="next-steps"></a><span data-ttu-id="7724f-143">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="7724f-143">Next steps</span></span>

- [<span data-ttu-id="7724f-144">Программный поиск идентификатора клиента с помощью PowerShell или интерфейса командной строки</span><span class="sxs-lookup"><span data-stu-id="7724f-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="7724f-145">Дополнительные сведения о профилях пользователей в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7724f-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="7724f-146">Узнайте, как партнеры могут просматривать или экспортировать сведения о клиентах в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="7724f-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

