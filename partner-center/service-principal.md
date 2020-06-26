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
ms.openlocfilehash: d37fe2134d02063819abeb89e2f1b6a63e0ba505
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679391"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="099ca-105">Добавление приложения Azure AD (субъекта-службы) в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="099ca-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="099ca-106">В рамках программы коммерческой платформы в Центре партнеров пользователи учетных записей Центра партнеров теперь могут добавлять приложения Azure AD (субъекты-службы).</span><span class="sxs-lookup"><span data-stu-id="099ca-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="099ca-107">(Ранее это можно было сделать в учетной записи Портала Cloud Partner (CPP).</span><span class="sxs-lookup"><span data-stu-id="099ca-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="099ca-108">Теперь, когда вы перешли в Центр партнеров, учетную запись CPP можно использовать только для чтения.)</span><span class="sxs-lookup"><span data-stu-id="099ca-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="099ca-109">Субъект-служба — это синоним приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="099ca-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="099ca-110">Добавление приложения Azure AD (субъекта-службы)</span><span class="sxs-lookup"><span data-stu-id="099ca-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="099ca-111">На панели мониторинга Центра партнеров щелкните **Параметры** и выберите **Параметры разработчика**.</span><span class="sxs-lookup"><span data-stu-id="099ca-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="099ca-112">Щелкните **Пользователи** и выберите **Добавить приложения Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="099ca-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="099ca-113">Выберите существующее приложение Azure AD или создайте новое.</span><span class="sxs-lookup"><span data-stu-id="099ca-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="099ca-114">Если вы создаете новое приложение Azure  AD, укажите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="099ca-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="099ca-115">**URL-адрес ответа.** URL-адрес, по которому пользователи смогут входить и использовать ваше приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="099ca-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="099ca-116">**Универсальный код ресурса (URI) идентификатора приложения.** Логический идентификатор приложения Azure AD, который предоставляется, когда оно отправляет запрос единого входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="099ca-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="099ca-117">**Роли безопасности.** Роли **Руководитель** и **Разработчик** (роли владельца и участника на портале CPP соответственно) доступны в рамках программы коммерческой платформы в Центре партнеров. Их можно связать с этим приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="099ca-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
