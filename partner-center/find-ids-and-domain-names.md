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
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360077"
---
# <a name="locate-important-ids-for-a-user"></a>Поиск важных идентификаторов для пользователя

В этой статье описывается, как использовать [портал Azure](https://portal.azure.com/) для выявления следующих сведений для пользователя:

- Идентификатор клиента Microsoft Azure Active Directory (Azure AD) для организации или компании пользователя.

- Основное доменное имя организации или компании, связанной с клиентом Azure AD.

- Идентификатор объекта пользователя

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Поиск идентификатора клиента Microsoft Azure AD и основного доменного имени

Выполните следующие действия, чтобы указать идентификатор клиента Azure AD или имя основного домена в портал Azure. (Если вы хотите найти идентификатор клиента программно, см. раздел [Поиск идентификатора клиента с помощью PowerShell или интерфейса командной строки](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)

> [!NOTE]
> Идентификатор клиента может называться разными именами в разных приложениях или ресурсах. Например, идентификатор клиента может называться ИДЕНТИФИКАТОРом каталога, клиентом Azure Active Directory (Azure AD), ИДЕНТИФИКАТОРом Microsoft или для определенных отчетов, даже *тенантгуид*.

1. Войдите на [портал Azure](https://portal.azure.com/).

2. Выберите **Azure Active Directory** в меню.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Показывает портал Azure выборе параметра Azure Active Directory в меню.":::

3. Откроется страница **обзора** Azure Active Directory. Чтобы найти идентификатор клиента Azure AD или имя основного домена, найдите поле " **идентификатор клиента** " и поле " **основной домен** ". Эти поля отображаются в разделе сведения о клиенте.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Отображает страницу обзора с двумя выделенными полями, ИДЕНТИФИКАТОРом клиента и именем основного домена.":::

4. Идентификатор клиента можно найти в портал Azure несколькими другими способами. Выберите **Azure Active Directory** в меню. Затем в меню найдите раздел **Управление** и выберите пункт **свойства**.

   На странице свойств также отображается связанный с пользователем идентификатор клиента.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Отображает страницу свойств с выделенным полем &quot;идентификатор клиента&quot;.":::

## <a name="find-the-user-object-id"></a>Поиск идентификатора объекта пользователя

Просто найти доменное имя и идентификатор клиента может быть не всегда достаточно. Также может потребоваться указать идентификатор объекта, назначенный пользователю. Выполните следующие действия, чтобы найти идентификатор объекта пользователя в портал Azure:

1. Войдите на [портал Azure](https://portal.azure.com/).

2. Выберите **Azure Active Directory** в меню.

3. Найдите в меню раздел **Управление** , а затем выберите **Пользователи**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Отображает Azure Active Directory меню с выделенным, параметром пользователи.":::

4. На странице Пользователи введите имя пользователя в поле поиска.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Отображает страницу пользователей с полем поиска для поиска определенного пользователя.":::

5. Выберите имя пользователя, где он отображается в списке.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Показывает пользовательскую страницу, отображающую строку для искомого пользователя.":::

6. На странице профиля пользователя откройте раздел удостоверение. Поле "идентификатор объекта" отображается здесь с уникальным ИДЕНТИФИКАТОРом объекта пользователя.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Отображает страницу профиля пользователя с разделом Identity и одно выделенное поле для идентификатора объекта.":::

## <a name="next-steps"></a>Дальнейшие шаги

- [Программный поиск идентификатора клиента с помощью PowerShell или интерфейса командной строки](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Дополнительные сведения о профилях пользователей в Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Узнайте, как партнеры могут просматривать или экспортировать сведения о клиентах в центре партнеров](see-your-customer-list.md)
