---
title: Добавление дополнительных клиентов в учетную запись центра партнеров
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как добавить, консолидировать или управлять несколькими клиентами Azure AD в учетной записи центра партнеров. Дополнительные сведения о некоторых причинах, по которым может потребоваться сделать это.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175161"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="a505c-104">Добавление нескольких клиентов и управление ими в учетной записи центра партнеров</span><span class="sxs-lookup"><span data-stu-id="a505c-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="a505c-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="a505c-105">**Applies to**</span></span>

- <span data-ttu-id="a505c-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="a505c-106">Partner Center</span></span>

<span data-ttu-id="a505c-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="a505c-107">**Appropriate roles**</span></span>

- <span data-ttu-id="a505c-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a505c-108">Global admin</span></span>

<span data-ttu-id="a505c-109">Эта функция позволяет управлять несколькими арендаторами для вашей компании и объединить их в учетной записи Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="a505c-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="a505c-110">Существует множество причин, по которым вам может потребоваться управлять несколькими клиентами Azure AD в учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="a505c-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="a505c-111">Пример:</span><span class="sxs-lookup"><span data-stu-id="a505c-111">For example:</span></span>

- <span data-ttu-id="a505c-112">Компания может приобрести другую компанию и предоставить сотрудникам новой компании возможность использовать центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="a505c-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="a505c-113">Однако необходимо, чтобы две компании оставались отдельными.</span><span class="sxs-lookup"><span data-stu-id="a505c-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="a505c-114">В этом случае вы свяжете клиент Azure AD новой компании с глобальной учетной записью партнера (PGA).</span><span class="sxs-lookup"><span data-stu-id="a505c-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="a505c-115">Эта ассоциация позволит пользователям в обеих компаниях работать в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="a505c-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="a505c-116">При наличии нескольких клиентов для выполнения вашего бизнеса (например, contoso.com, contoso.uk, contoso.in) вы можете использовать мультитенантность, чтобы связать их с одной и той же учетной записью компьютера.</span><span class="sxs-lookup"><span data-stu-id="a505c-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="a505c-117">Для слияния и приобретения требуется работать с несколькими клиентами (например, если Contoso получает Fabrikam, вам потребуется иметь возможность использовать и Constoso.com, и Fabrikam.com соответствующих клиентов).</span><span class="sxs-lookup"><span data-stu-id="a505c-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="a505c-118">Пользователи из любого из клиентов должны иметь возможность:</span><span class="sxs-lookup"><span data-stu-id="a505c-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="a505c-119">Доступ к центру партнеров для обучения, цифровых Скачиваний, сопоставления MCP</span><span class="sxs-lookup"><span data-stu-id="a505c-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="a505c-120">Назначать роли центра партнеров, например администратора MPN, администратора поощрения и т. д.</span><span class="sxs-lookup"><span data-stu-id="a505c-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="a505c-121">Добавление другого клиента Azure AD в учетную запись</span><span class="sxs-lookup"><span data-stu-id="a505c-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="a505c-122">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard)центра партнеров в качестве глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="a505c-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="a505c-123">На значке **параметров** выберите **Параметры учетной записи** , а затем щелкните **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="a505c-123">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Связывание клиентов"::: 

3. <span data-ttu-id="a505c-125">Выберите **связать другой клиент AD** и укажите клиента, которого необходимо связать.</span><span class="sxs-lookup"><span data-stu-id="a505c-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="a505c-126">Войдите в клиент, который необходимо связать, и подтвердите связь с глобальным администратором.</span><span class="sxs-lookup"><span data-stu-id="a505c-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Связывание клиентов"::: 

5. <span data-ttu-id="a505c-128">После подтверждения вы увидите все уведомления о **наборе** .</span><span class="sxs-lookup"><span data-stu-id="a505c-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="a505c-129">Выберите **вернуться к управлению клиентами** , и вы увидите, что добавленный клиент указан в списке.</span><span class="sxs-lookup"><span data-stu-id="a505c-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="a505c-130">Вы не можете связать клиент с учетной записью, если он уже связан с другой учетной записью центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="a505c-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="a505c-131">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a505c-131">Next steps</span></span>

- [<span data-ttu-id="a505c-132">Добавление пользователей</span><span class="sxs-lookup"><span data-stu-id="a505c-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
