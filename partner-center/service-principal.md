---
title: Субъект-служба Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как добавить субъект-службу в клиент Azure AD. Подразумевается добавление приложения Azure AD (субъекта-службы) в Центре партнеров.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, план Azure, субъект-служба, приложение Azure AD
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 76a65cd824c7c1af5242bea3af6069a466c9fa1c
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "84426003"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="9f0ee-105">Добавление приложения Azure AD (субъекта-службы) в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="9f0ee-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="9f0ee-106">В рамках программы коммерческой платформы в Центре партнеров пользователи учетных записей Центра партнеров теперь могут добавлять приложения Azure AD (субъекты-службы).</span><span class="sxs-lookup"><span data-stu-id="9f0ee-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="9f0ee-107">(Ранее это можно было сделать в учетной записи Портала Cloud Partner (CPP).</span><span class="sxs-lookup"><span data-stu-id="9f0ee-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="9f0ee-108">Теперь, когда вы перешли в Центр партнеров, учетную запись CPP можно использовать только для чтения.) Обратите внимание, что субъект-служба — это синоним приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9f0ee-108">Now that you have migrated to Partner Center, the CPP account is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="9f0ee-109">Добавление приложения Azure AD (субъекта-службы)</span><span class="sxs-lookup"><span data-stu-id="9f0ee-109">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="9f0ee-110">На панели мониторинга Центра партнеров щелкните **Параметры** и выберите **Параметры разработчика**.</span><span class="sxs-lookup"><span data-stu-id="9f0ee-110">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="9f0ee-111">Щелкните **Пользователи** и выберите **Добавить приложения Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="9f0ee-111">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="9f0ee-112">Выберите существующее приложение Azure AD или создайте новое.</span><span class="sxs-lookup"><span data-stu-id="9f0ee-112">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="9f0ee-113">Если вы создаете новое приложение Azure  AD, укажите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="9f0ee-113">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="9f0ee-114">**URL-адрес ответа.** URL-адрес, по которому пользователи смогут входить и использовать ваше приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9f0ee-114">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="9f0ee-115">**Универсальный код ресурса (URI) идентификатора приложения.** Логический идентификатор приложения Azure AD, который предоставляется, когда оно отправляет запрос единого входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9f0ee-115">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="9f0ee-116">**Роли безопасности.** Роли **Руководитель** и **Разработчик** (роли владельца и участника на портале CPP соответственно) доступны в рамках программы коммерческой платформы в Центре партнеров. Их можно связать с этим приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9f0ee-116">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
