---
title: Субъект-служба Azure AD | Центр партнеров
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Добавление субъекта-службы в клиент Azure AD
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, план Azure, субъект-служба, приложение Azure AD
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010385"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="ca873-104">Добавление приложения Azure AD (субъекта-службы) в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ca873-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="ca873-105">В рамках программы коммерческой платформы в Центре партнеров пользователи клиентов Azure AD теперь могут добавлять приложения Azure AD (субъекты-службы).</span><span class="sxs-lookup"><span data-stu-id="ca873-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Azure AD tenant.</span></span> <span data-ttu-id="ca873-106">(Раньше это можно было сделать с помощью учетной записи Портала Cloud Partner (CPP). После миграции в Центр партнеров эта учетная запись доступна только для чтения.) Обратите внимание, что субъект-служба — это синоним приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca873-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="ca873-107">Добавление приложения Azure AD (субъекта-службы)</span><span class="sxs-lookup"><span data-stu-id="ca873-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="ca873-108">На панели мониторинга Центра партнеров щелкните **Параметры** и выберите **Параметры разработчика**.</span><span class="sxs-lookup"><span data-stu-id="ca873-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="ca873-109">Щелкните **Пользователи** и выберите **Добавить приложения Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="ca873-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="ca873-110">Выберите существующее приложение Azure AD или создайте новое.</span><span class="sxs-lookup"><span data-stu-id="ca873-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="ca873-111">Если вы создаете новое приложение Azure  AD, укажите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="ca873-111">If you create a new Azure AD Application, include the following information:</span></span>  
<span data-ttu-id="ca873-112">  
\*\*Имя.\*\* Это поле соответствует полю для понятного имени на портале CPP.</span><span class="sxs-lookup"><span data-stu-id="ca873-112">  
\*\*Name\*\*: This is similar to the ‘friendly name’ field in the CPP portal.</span></span>

<span data-ttu-id="ca873-113">**URL-адрес ответа.** Это URL-адрес, по которому пользователи смогут входить и использовать ваше приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca873-113">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="ca873-114">**Универсальный код ресурса (URI) идентификатора приложения.** Это логический идентификатор приложения Azure AD, который предоставляется, когда оно отправляет запрос единого входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca873-114">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="ca873-115">**Роли безопасности.** Роли **Руководитель** и **Разработчик** (роли владельца и участника на портале CPP соответственно) доступны в рамках программы коммерческой платформы в Центре партнеров. Их можно связать с этим приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca873-115">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

<span data-ttu-id="ca873-116">Когда вы щелкнете **Создать**, чтобы создать приложение в Центре партнеров, сведения будут синхронизированы с данными в системе CPP.</span><span class="sxs-lookup"><span data-stu-id="ca873-116">When you select **Save**,  to create this in Partner Center, the information is also synced back to the CPP system.</span></span>  
