---
title: Предварительные требования для программного доступа к данным аналитики
description: Предварительные требования для программного доступа к данным аналитики
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375864"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="c7f97-103">Предварительные требования для программного доступа к данным аналитики</span><span class="sxs-lookup"><span data-stu-id="c7f97-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="c7f97-104">**Соответствующие роли:** Глобальный администратор | Администратор MPN</span><span class="sxs-lookup"><span data-stu-id="c7f97-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="c7f97-105">Прежде чем можно будет получить доступ к данным аналитики Partner Insights программным способом, необходимо выполнить следующие требования.</span><span class="sxs-lookup"><span data-stu-id="c7f97-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="c7f97-106">Регистрация программы MPN</span><span class="sxs-lookup"><span data-stu-id="c7f97-106">MPN Program enrollment</span></span>

<span data-ttu-id="c7f97-107">Чтобы получить доступ к данным аналитики Partner Insights программным способом, необходимо зарегистрироваться в программе MPN и получить учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7f97-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="c7f97-108">Дополнительные сведения см. в статье [Создание учетной записи MPN в центре партнеров](mpn-create-a-partner-center-account.md) .</span><span class="sxs-lookup"><span data-stu-id="c7f97-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="c7f97-109">создание приложения Azure Active Directory (AAD)</span><span class="sxs-lookup"><span data-stu-id="c7f97-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="c7f97-110">обычные учетные данные пользователя нельзя использовать для программного доступа к данным аналитики партнеров Аналитика.</span><span class="sxs-lookup"><span data-stu-id="c7f97-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="c7f97-111">для доступа к api программного доступа необходимо создать приложение Azure Active Directory (AAD) вместе с секретом (доступ приложения и пользователя).</span><span class="sxs-lookup"><span data-stu-id="c7f97-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="c7f97-112">сведения о создании приложения и секрета AAD см. в разделе [краткое руководство. регистрация приложения в платформа удостоверений Майкрософт.](/azure/active-directory/develop/quickstart-register-app)   Для доступа к Microsoft Partner API требуется разрешение.</span><span class="sxs-lookup"><span data-stu-id="c7f97-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="c7f97-113">Чтобы узнать, как добавить разрешение, ознакомьтесь со статьей [Проверка подлинности партнерского API-партнера](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="c7f97-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="c7f97-114">Назначить пользователю роль средства просмотра отчетов руководителя (ЕРВ)</span><span class="sxs-lookup"><span data-stu-id="c7f97-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="c7f97-115">Чтобы получить доступ к данным аналитики Partner Insights программным способом, необходимо иметь средство просмотра отчетов с руководителем (ЕРВ).</span><span class="sxs-lookup"><span data-stu-id="c7f97-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="c7f97-116">чтобы узнать, как назначить роль ерв для пользователя, см. статью [центр партнеров Аналитика доступ на основе ролей в центре партнеров](insights-roles.md) .</span><span class="sxs-lookup"><span data-stu-id="c7f97-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="c7f97-117">Создание токена AAD</span><span class="sxs-lookup"><span data-stu-id="c7f97-117">Generate an AAD token</span></span>

<span data-ttu-id="c7f97-118">Необходимо создать токен AAD с помощью идентификатора приложения (клиента), секрета клиента, идентификатора пользователя и пароля. См.   [инструкции по созданию](insights-programmatic-first-api-call.md#token-generation) токена AAD.</span><span class="sxs-lookup"><span data-stu-id="c7f97-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="c7f97-119">Каждый маркер действителен в течение одного часа.</span><span class="sxs-lookup"><span data-stu-id="c7f97-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c7f97-120">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="c7f97-120">Next steps</span></span>
[<span data-ttu-id="c7f97-121">Парадигма программного доступа</span><span class="sxs-lookup"><span data-stu-id="c7f97-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)