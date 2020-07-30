---
title: Добавление дополнительных клиентов в учетную запись центра партнеров
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Управление несколькими клиентами с помощью учетной записи центра партнеров
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389531"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="88d44-103">Добавление нескольких клиентов и управление ими в учетной записи центра партнеров</span><span class="sxs-lookup"><span data-stu-id="88d44-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="88d44-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="88d44-104">**Applies to**</span></span>

- <span data-ttu-id="88d44-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="88d44-105">Partner Center</span></span>

<span data-ttu-id="88d44-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="88d44-106">**Appropriate roles**</span></span>

- <span data-ttu-id="88d44-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="88d44-107">Global admin</span></span>

<span data-ttu-id="88d44-108">Существует множество причин, по которым вам может потребоваться управлять несколькими клиентами Azure AD в учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="88d44-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="88d44-109">Например, компания может приобрести другую компанию и предоставить сотрудникам новой компании возможность использовать центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="88d44-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="88d44-110">Однако необходимо, чтобы две компании оставались отдельными.</span><span class="sxs-lookup"><span data-stu-id="88d44-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="88d44-111">В этом случае вы свяжете клиент Azure AD новой компании с глобальной учетной записью партнера (PNG).</span><span class="sxs-lookup"><span data-stu-id="88d44-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="88d44-112">Эта ассоциация позволит пользователям в обеих компаниях работать в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="88d44-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="88d44-113">Добавление другого клиента Azure AD в учетную запись</span><span class="sxs-lookup"><span data-stu-id="88d44-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="88d44-114">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard)центра партнеров в качестве глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="88d44-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="88d44-115">На значке **параметров** выберите **Параметры учетной записи** , а затем щелкните **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="88d44-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="Связывание клиентов"::: 

3. <span data-ttu-id="88d44-117">Выберите **связать другой клиент AD** и укажите клиента, которого необходимо связать.</span><span class="sxs-lookup"><span data-stu-id="88d44-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="88d44-118">Войдите в клиент, который необходимо связать, и подтвердите связь с глобальным администратором.</span><span class="sxs-lookup"><span data-stu-id="88d44-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="подтверждение связывания клиентов"::: 

5. <span data-ttu-id="88d44-120">После подтверждения вы увидите все уведомления о **наборе** .</span><span class="sxs-lookup"><span data-stu-id="88d44-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="88d44-121">Выберите **вернуться к управлению клиентами** , и вы увидите, что добавленный клиент указан в списке.</span><span class="sxs-lookup"><span data-stu-id="88d44-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="88d44-122">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="88d44-122">Next steps</span></span>

- [<span data-ttu-id="88d44-123">Добавление пользователей</span><span class="sxs-lookup"><span data-stu-id="88d44-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
