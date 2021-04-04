---
title: Субъект-служба Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как добавить субъект-службу в клиент Azure AD. Подразумевается добавление приложения Azure AD (субъекта-службы) в Центре партнеров.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028474"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="e1f57-104">Добавление приложения Azure AD (субъекта-службы) в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="e1f57-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="e1f57-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="e1f57-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e1f57-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e1f57-106">Global admin</span></span>

<span data-ttu-id="e1f57-107">В рамках программы коммерческой платформы в Центре партнеров пользователи учетных записей Центра партнеров теперь могут добавлять приложения Azure AD (субъекты-службы).</span><span class="sxs-lookup"><span data-stu-id="e1f57-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="e1f57-108">(Ранее это можно было сделать в учетной записи Портала Cloud Partner (CPP).</span><span class="sxs-lookup"><span data-stu-id="e1f57-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="e1f57-109">Теперь, когда вы перешли в Центр партнеров, учетную запись CPP можно использовать только для чтения.)</span><span class="sxs-lookup"><span data-stu-id="e1f57-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="e1f57-110">Субъект-служба — это синоним приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e1f57-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="e1f57-111">Добавление приложения Azure AD (субъекта-службы)</span><span class="sxs-lookup"><span data-stu-id="e1f57-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="e1f57-112">На панели мониторинга Центра партнеров щелкните **Параметры** и выберите **Параметры разработчика**.</span><span class="sxs-lookup"><span data-stu-id="e1f57-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="e1f57-113">Щелкните **Пользователи** и выберите **Добавить приложения Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="e1f57-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="e1f57-114">Выберите существующее приложение Azure AD или создайте новое.</span><span class="sxs-lookup"><span data-stu-id="e1f57-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="e1f57-115">Если вы создаете новое приложение Azure  AD, укажите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="e1f57-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="e1f57-116">**URL-адрес ответа.** URL-адрес, по которому пользователи смогут входить и использовать ваше приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e1f57-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="e1f57-117">**Универсальный код ресурса (URI) идентификатора приложения.** Логический идентификатор приложения Azure AD, который предоставляется, когда оно отправляет запрос единого входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e1f57-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="e1f57-118">**Роли безопасности.** Роли **Руководитель** и **Разработчик** (роли владельца и участника на портале CPP соответственно) доступны в рамках программы коммерческой платформы в Центре партнеров. Их можно связать с этим приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e1f57-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="e1f57-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e1f57-119">Next steps</span></span>

- [<span data-ttu-id="e1f57-120">Общие сведения о коммерческой платформе в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="e1f57-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)