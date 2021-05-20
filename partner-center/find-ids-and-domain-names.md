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
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150868"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="4ad4e-104">Поиск важных идентификаторов для пользователя</span><span class="sxs-lookup"><span data-stu-id="4ad4e-104">Locate important IDs for a user</span></span>

<span data-ttu-id="4ad4e-105">**Соответствующие роли** — глобальный администратор.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="4ad4e-106">В этой статье описывается, как использовать [портал Azure](https://portal.azure.com/) для выявления следующих сведений для пользователя:</span><span class="sxs-lookup"><span data-stu-id="4ad4e-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="4ad4e-107">Идентификатор клиента Microsoft Azure Active Directory (Azure AD) для организации или компании пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="4ad4e-108">Основное доменное имя организации или компании, связанной с клиентом Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="4ad4e-109">Идентификатор объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="4ad4e-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="4ad4e-110">Поиск идентификатора клиента Microsoft Azure AD и основного доменного имени</span><span class="sxs-lookup"><span data-stu-id="4ad4e-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="4ad4e-111">Выполните следующие действия, чтобы указать идентификатор клиента Azure AD или имя основного домена в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="4ad4e-112">(Если вы хотите найти идентификатор клиента программно, см. раздел [Поиск идентификатора клиента с помощью PowerShell или интерфейса командной строки](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="4ad4e-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="4ad4e-113">Идентификатор клиента может называться разными именами в разных приложениях или ресурсах.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="4ad4e-114">Например, идентификатор клиента может называться ИДЕНТИФИКАТОРом каталога, клиентом Azure Active Directory (Azure AD), ИДЕНТИФИКАТОРом Microsoft или для определенных отчетов, даже *тенантгуид*.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="4ad4e-115">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="4ad4e-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="4ad4e-116">Выберите **Azure Active Directory** в меню.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Показывает портал Azure выборе параметра Azure Active Directory в меню.":::

3. <span data-ttu-id="4ad4e-118">Откроется страница **обзора** Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="4ad4e-119">Чтобы найти идентификатор клиента Azure AD или имя основного домена, найдите поле " **идентификатор клиента** " и поле " **основной домен** ".</span><span class="sxs-lookup"><span data-stu-id="4ad4e-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="4ad4e-120">Эти поля отображаются в разделе сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Отображает страницу обзора с двумя выделенными полями, ИДЕНТИФИКАТОРом клиента и именем основного домена.":::

4. <span data-ttu-id="4ad4e-122">Идентификатор клиента можно найти в портал Azure несколькими другими способами.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="4ad4e-123">Выберите **Azure Active Directory** в меню.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="4ad4e-124">Затем в меню найдите раздел **Управление** и выберите пункт **свойства**.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="4ad4e-125">На странице свойств также отображается связанный с пользователем идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Отображает страницу свойств с выделенным полем &quot;идентификатор клиента&quot;.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="4ad4e-127">Поиск идентификатора объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="4ad4e-127">Find the user object ID</span></span>

<span data-ttu-id="4ad4e-128">Просто найти доменное имя и идентификатор клиента может быть не всегда достаточно.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="4ad4e-129">Также может потребоваться указать идентификатор объекта, назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="4ad4e-130">Выполните следующие действия, чтобы найти идентификатор объекта пользователя в портал Azure:</span><span class="sxs-lookup"><span data-stu-id="4ad4e-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="4ad4e-131">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="4ad4e-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="4ad4e-132">Выберите **Azure Active Directory** в меню.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="4ad4e-133">Найдите в меню раздел **Управление** , а затем выберите **Пользователи**.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Отображает Azure Active Directory меню с выделенным, параметром пользователи.":::

4. <span data-ttu-id="4ad4e-135">На странице Пользователи введите имя пользователя в поле поиска.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Отображает страницу пользователей с полем поиска для поиска определенного пользователя.":::

5. <span data-ttu-id="4ad4e-137">Выберите имя пользователя, где он отображается в списке.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Показывает пользовательскую страницу, отображающую строку для искомого пользователя.":::

6. <span data-ttu-id="4ad4e-139">На странице профиля пользователя откройте раздел удостоверение.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="4ad4e-140">Поле "идентификатор объекта" отображается здесь с уникальным ИДЕНТИФИКАТОРом объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ad4e-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Отображает страницу профиля пользователя с разделом Identity и одно выделенное поле для идентификатора объекта.":::

## <a name="next-steps"></a><span data-ttu-id="4ad4e-142">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="4ad4e-142">Next steps</span></span>

- [<span data-ttu-id="4ad4e-143">Программный поиск идентификатора клиента с помощью PowerShell или интерфейса командной строки</span><span class="sxs-lookup"><span data-stu-id="4ad4e-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="4ad4e-144">Дополнительные сведения о профилях пользователей в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4ad4e-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="4ad4e-145">Узнайте, как партнеры могут просматривать или экспортировать сведения о клиентах в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="4ad4e-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

