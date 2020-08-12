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
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811244"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="37a59-104">Добавление приложения Azure AD (субъекта-службы) в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="37a59-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="37a59-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="37a59-105">**Applies to**</span></span>

- <span data-ttu-id="37a59-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="37a59-106">Partner Center</span></span>

<span data-ttu-id="37a59-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="37a59-107">**Appropriate roles**</span></span>

- <span data-ttu-id="37a59-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="37a59-108">Global admin</span></span>

<span data-ttu-id="37a59-109">В рамках программы коммерческой платформы в Центре партнеров пользователи учетных записей Центра партнеров теперь могут добавлять приложения Azure AD (субъекты-службы).</span><span class="sxs-lookup"><span data-stu-id="37a59-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="37a59-110">(Ранее это можно было сделать в учетной записи Портала Cloud Partner (CPP).</span><span class="sxs-lookup"><span data-stu-id="37a59-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="37a59-111">Теперь, когда вы перешли в Центр партнеров, учетную запись CPP можно использовать только для чтения.)</span><span class="sxs-lookup"><span data-stu-id="37a59-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="37a59-112">Субъект-служба — это синоним приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37a59-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="37a59-113">Добавление приложения Azure AD (субъекта-службы)</span><span class="sxs-lookup"><span data-stu-id="37a59-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="37a59-114">На панели мониторинга Центра партнеров щелкните **Параметры** и выберите **Параметры разработчика**.</span><span class="sxs-lookup"><span data-stu-id="37a59-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="37a59-115">Щелкните **Пользователи** и выберите **Добавить приложения Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="37a59-115">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="37a59-116">Выберите существующее приложение Azure AD или создайте новое.</span><span class="sxs-lookup"><span data-stu-id="37a59-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="37a59-117">Если вы создаете новое приложение Azure  AD, укажите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="37a59-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="37a59-118">**URL-адрес ответа.** URL-адрес, по которому пользователи смогут входить и использовать ваше приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37a59-118">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="37a59-119">**Универсальный код ресурса (URI) идентификатора приложения.** Логический идентификатор приложения Azure AD, который предоставляется, когда оно отправляет запрос единого входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37a59-119">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="37a59-120">**Роли безопасности.** Роли **Руководитель** и **Разработчик** (роли владельца и участника на портале CPP соответственно) доступны в рамках программы коммерческой платформы в Центре партнеров. Их можно связать с этим приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37a59-120">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="37a59-121">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="37a59-121">Next steps</span></span>

- [<span data-ttu-id="37a59-122">Общие сведения о коммерческой платформе в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="37a59-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)