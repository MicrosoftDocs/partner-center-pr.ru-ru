---
title: Добавление клиентов в учетную запись центра партнеров
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как добавить, консолидировать или управлять несколькими клиентами Azure AD в учетной записи центра партнеров, а также узнать, почему это может потребоваться.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124811"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="4cb36-103">Добавление нескольких клиентов и управление ими в учетной записи центра партнеров</span><span class="sxs-lookup"><span data-stu-id="4cb36-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="4cb36-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="4cb36-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4cb36-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4cb36-105">Global admin</span></span>
- <span data-ttu-id="4cb36-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="4cb36-106">Account admin</span></span>

<span data-ttu-id="4cb36-107">В этой статье описывается Консолидация нескольких клиентов Azure Active Directory (Azure AD) для вашей компании, а затем их добавление в учетную запись центра партнеров и управление ими.</span><span class="sxs-lookup"><span data-stu-id="4cb36-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="4cb36-108">Это можно сделать несколькими причинами.</span><span class="sxs-lookup"><span data-stu-id="4cb36-108">There are many reasons to do so.</span></span> <span data-ttu-id="4cb36-109">Пример:</span><span class="sxs-lookup"><span data-stu-id="4cb36-109">For example:</span></span>

- <span data-ttu-id="4cb36-110">Предположим, что компания Contoso приобрела другую компанию Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="4cb36-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="4cb36-111">Вы хотите, чтобы эти две компании оставались отдельными, но вы хотите, чтобы новые сотрудники могли использовать центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="4cb36-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="4cb36-112">В этом случае вы связываете клиент Azure AD новой компании с глобальной учетной записью партнера (PGA).</span><span class="sxs-lookup"><span data-stu-id="4cb36-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="4cb36-113">Эта ассоциация позволяет пользователям в обеих компаниях работать в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="4cb36-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="4cb36-114">При запуске бизнеса с несколькими клиентами (например, *contoso.com*, *contoso.UK* и *contoso.in*) можно использовать мультитенантность для группировки их в одной учетной записи компьютера.</span><span class="sxs-lookup"><span data-stu-id="4cb36-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="4cb36-115">Если для слияния и получения рекомендаций требуется работа с клиентами обеих компаний, вы должны использовать как клиенты *constoso.com* , так и *Fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="4cb36-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="4cb36-116">Пользователи любого из клиентов должны иметь возможность:</span><span class="sxs-lookup"><span data-stu-id="4cb36-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="4cb36-117">Доступ к центру партнеров для обучения, цифровых скачиваний или связи Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="4cb36-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="4cb36-118">Назначать роли центра партнеров, такие как Microsoft Partner Network (MPN) администратора или администратора поощрения.</span><span class="sxs-lookup"><span data-stu-id="4cb36-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="4cb36-119">Добавление клиента Azure AD в учетную запись</span><span class="sxs-lookup"><span data-stu-id="4cb36-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="4cb36-120">Войдите в систему как глобальный администратор в [Центр партнеров Майкрософт](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4cb36-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="4cb36-121">В верхнем правом углу щелкните **Параметры**, выберите **Параметры учетной записи**, а затем — **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="4cb36-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Снимок экрана кнопки &quot;связать&quot; на панели профиля Azure AD."::: 

1. <span data-ttu-id="4cb36-123">Выберите **связать**, а затем укажите клиента, которого необходимо связать.</span><span class="sxs-lookup"><span data-stu-id="4cb36-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="4cb36-124">В командной строке Войдите в качестве глобального администратора клиента, которого необходимо связать, а затем нажмите кнопку **подтвердить**.</span><span class="sxs-lookup"><span data-stu-id="4cb36-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Снимок экрана с кнопкой &quot;подтвердить&quot; на панели &quot;подтверждение новой связи Azure AD&quot;."::: 

   <span data-ttu-id="4cb36-126">После подтверждения связи отображается сообщение **все установлено** .</span><span class="sxs-lookup"><span data-stu-id="4cb36-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="4cb36-127">Чтобы просмотреть добавленного клиента, выберите **вернуться к управлению клиентами**.</span><span class="sxs-lookup"><span data-stu-id="4cb36-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="4cb36-128">Вы не можете связать клиент с учетной записью, если он уже связан с другой учетной записью центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="4cb36-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="4cb36-129">Удаление клиента из учетной записи</span><span class="sxs-lookup"><span data-stu-id="4cb36-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="4cb36-130">Войдите в систему как глобальный администратор в [Центр партнеров Майкрософт](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4cb36-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="4cb36-131">В правом верхнем углу щелкните значок **Параметры** , а затем выберите **Параметры учетной записи**.</span><span class="sxs-lookup"><span data-stu-id="4cb36-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="4cb36-132">На левой панели выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="4cb36-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="4cb36-133">В разделе **Управление клиентами Azure AD** перейдите на вкладку **партнер** .</span><span class="sxs-lookup"><span data-stu-id="4cb36-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="4cb36-134">Выберите **Удалить** рядом с клиентом, связь которого нужно удалить.</span><span class="sxs-lookup"><span data-stu-id="4cb36-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Снимок экрана связей текущего клиента и их ссылок для удаления.":::

   <span data-ttu-id="4cb36-136">Как показано на предыдущем снимке экрана, ссылки для **удаления** включены для всех связанных клиентов, за исключением основного клиента и клиента, на который вы вошли в систему.</span><span class="sxs-lookup"><span data-stu-id="4cb36-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="4cb36-137">При удалении клиента у пользователей этого клиента больше нет доступа к учетной записи центра партнеров, и удаление может повлиять на компетенции.</span><span class="sxs-lookup"><span data-stu-id="4cb36-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="4cb36-138">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="4cb36-138">Next steps</span></span>

- [<span data-ttu-id="4cb36-139">Создание учетных записей пользователей</span><span class="sxs-lookup"><span data-stu-id="4cb36-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






