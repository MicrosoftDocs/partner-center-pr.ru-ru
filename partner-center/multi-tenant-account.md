---
title: Добавление дополнительных клиентов в учетную запись центра партнеров
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как добавить, консолидировать или управлять несколькими клиентами Azure AD в учетной записи центра партнеров. Дополнительные сведения о некоторых причинах, по которым может потребоваться сделать это.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182444"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="59405-104">Добавление нескольких клиентов и управление ими в учетной записи центра партнеров</span><span class="sxs-lookup"><span data-stu-id="59405-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="59405-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="59405-105">**Appropriate roles**</span></span>

- <span data-ttu-id="59405-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="59405-106">Global admin</span></span>
- <span data-ttu-id="59405-107">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="59405-107">Account admin</span></span>

<span data-ttu-id="59405-108">Эта функция позволяет управлять несколькими арендаторами для вашей компании и объединить их в учетной записи Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="59405-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="59405-109">Существует множество причин, по которым вам может потребоваться управлять несколькими клиентами Azure AD в учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="59405-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="59405-110">Пример:</span><span class="sxs-lookup"><span data-stu-id="59405-110">For example:</span></span>

- <span data-ttu-id="59405-111">Компания может приобрести другую компанию и предоставить сотрудникам новой компании возможность использовать центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="59405-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="59405-112">Однако необходимо, чтобы две компании оставались отдельными.</span><span class="sxs-lookup"><span data-stu-id="59405-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="59405-113">В этом случае вы свяжете клиент Azure AD новой компании с глобальной учетной записью партнера (PGA).</span><span class="sxs-lookup"><span data-stu-id="59405-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="59405-114">Эта ассоциация позволит пользователям в обеих компаниях работать в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="59405-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="59405-115">При наличии нескольких клиентов для выполнения вашего бизнеса (например, contoso.com, contoso.uk, contoso.in) вы можете использовать мультитенантность, чтобы связать их с одной и той же учетной записью компьютера.</span><span class="sxs-lookup"><span data-stu-id="59405-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="59405-116">Для слияния и приобретения требуется работать с несколькими клиентами (например, если Contoso получает Fabrikam, вам потребуется иметь возможность использовать и Constoso.com, и Fabrikam.com соответствующих клиентов).</span><span class="sxs-lookup"><span data-stu-id="59405-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="59405-117">Пользователи из любого из клиентов должны иметь возможность:</span><span class="sxs-lookup"><span data-stu-id="59405-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="59405-118">Доступ к центру партнеров для обучения, цифровых Скачиваний, сопоставления MCP</span><span class="sxs-lookup"><span data-stu-id="59405-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="59405-119">Назначать роли центра партнеров, например администратора MPN, администратора поощрения и т. д.</span><span class="sxs-lookup"><span data-stu-id="59405-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="59405-120">Добавление другого клиента Azure AD в учетную запись</span><span class="sxs-lookup"><span data-stu-id="59405-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="59405-121">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard)центра партнеров в качестве глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="59405-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="59405-122">На значке **параметров** выберите **Параметры учетной записи** , а затем щелкните **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="59405-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Связывание клиентов"::: 

3. <span data-ttu-id="59405-124">Выберите **связать другой клиент AD** и укажите клиента, которого необходимо связать.</span><span class="sxs-lookup"><span data-stu-id="59405-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="59405-125">Войдите в клиент, который необходимо связать, и подтвердите связь с глобальным администратором.</span><span class="sxs-lookup"><span data-stu-id="59405-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="подтверждение связывания клиентов"::: 

5. <span data-ttu-id="59405-127">После подтверждения вы увидите все уведомления о **наборе** .</span><span class="sxs-lookup"><span data-stu-id="59405-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="59405-128">Выберите **вернуться к управлению клиентами** , и вы увидите, что добавленный клиент указан в списке.</span><span class="sxs-lookup"><span data-stu-id="59405-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="59405-129">Вы не можете связать клиент с учетной записью, если он уже связан с другой учетной записью центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="59405-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="59405-130">Удаление клиента из учетной записи</span><span class="sxs-lookup"><span data-stu-id="59405-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="59405-131">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard)центра партнеров в качестве глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="59405-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="59405-132">На значке **параметров** выберите **Параметры учетной записи** — > клиенты и щелкните вкладку **Partner (партнер** ).</span><span class="sxs-lookup"><span data-stu-id="59405-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="59405-133">Нажмите кнопку **Удалить** для клиента, для которого требуется отменить связь.</span><span class="sxs-lookup"><span data-stu-id="59405-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="59405-134">Отмена связи с клиентом означает, что пользователи этого клиента больше не смогут получить доступ к учетной записи центра партнеров, и это может повлиять на компетенции.</span><span class="sxs-lookup"><span data-stu-id="59405-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="59405-135">Кнопка **Удалить** доступна для всех связанных клиентов, кроме первичного клиента и клиента, в который в данный момент выполнен вход.</span><span class="sxs-lookup"><span data-stu-id="59405-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="Клиенты с кнопкой &quot;Удалить&quot;":::
 

## <a name="next-steps"></a><span data-ttu-id="59405-137">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="59405-137">Next steps</span></span>

- [<span data-ttu-id="59405-138">Добавление пользователей</span><span class="sxs-lookup"><span data-stu-id="59405-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






