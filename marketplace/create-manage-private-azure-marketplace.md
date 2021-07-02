---
title: Создание частного магазина Azure Marketplace и управление им в портал Azure
description: Узнайте, как создать частный сайт Azure Marketplace (Предварительная версия) и управлять им в портал Azure. Частная среда Azure Marketplace (Предварительная версия) позволяет администраторам определять, какие сторонние решения могут использовать пользователи.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173689"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="30c75-104">Создание частного магазина Azure Marketplace и управление им в портал Azure</span><span class="sxs-lookup"><span data-stu-id="30c75-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="30c75-105">Частная среда Azure Marketplace позволяет администраторам определять, какие решения сторонних разработчиков могут использовать пользователи.</span><span class="sxs-lookup"><span data-stu-id="30c75-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="30c75-106">Это позволяет пользователю развертывать только предложения, утвержденные администратором и соответствующие политикам предприятия.</span><span class="sxs-lookup"><span data-stu-id="30c75-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="30c75-107">Благодаря частному Azure Marketplace пользователи могут искать в Интернет-магазине соответствующие предложения для приобретения и развертывания.</span><span class="sxs-lookup"><span data-stu-id="30c75-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="30c75-108">Как администратор Marketplace (назначенная роль), вы начнете с отключенного и пустого частного хранилища, в котором можно добавить утвержденные предложения и планы.</span><span class="sxs-lookup"><span data-stu-id="30c75-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="30c75-109">В этой статье описывается назначение необходимой роли, создание частного хранилища, Управление элементами, утверждение запросов пользователей и включение частного магазина Azure Marketplace для пользователей.</span><span class="sxs-lookup"><span data-stu-id="30c75-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="30c75-110">Частный сайт Azure Marketplace находится на уровне клиента, поэтому все пользователи в клиенте будут видеть один проверенный список.</span><span class="sxs-lookup"><span data-stu-id="30c75-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="30c75-111">Все решения Майкрософт (включая предустановленные [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros)) автоматически добавляются в частный магазин Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="30c75-112">Назначение роли администратора Marketplace</span><span class="sxs-lookup"><span data-stu-id="30c75-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="30c75-113">Глобальный администратор клиента должен назначить роль **администратора Marketplace** частному администратору Azure Marketplace, который будет управлять частным хранилищем.</span><span class="sxs-lookup"><span data-stu-id="30c75-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="30c75-114">Доступ к частному управлению Azure Marketplace доступен только ИТ-администраторам с назначенной ролью администратора Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="30c75-115">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="30c75-115">Prerequisites</span></span>

<span data-ttu-id="30c75-116">Эти предварительные требования необходимы, прежде чем можно будет назначить роль администратора Marketplace пользователю в области клиента:</span><span class="sxs-lookup"><span data-stu-id="30c75-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="30c75-117">У вас есть доступ к пользователю **глобального администратора** .</span><span class="sxs-lookup"><span data-stu-id="30c75-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="30c75-118">У клиента есть по крайней мере одна подписка (может иметь любой тип).</span><span class="sxs-lookup"><span data-stu-id="30c75-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="30c75-119">Пользователю глобального администратора назначается роль **участника** или выше для выбранной подписки.</span><span class="sxs-lookup"><span data-stu-id="30c75-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="30c75-120">Назначение роли администратора Marketplace с помощью управления доступом (IAM)</span><span class="sxs-lookup"><span data-stu-id="30c75-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="30c75-121">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="30c75-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="30c75-122">Выберите **все службы** , а затем **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="30c75-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="30c75-123">В меню слева выберите **частный Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="30c75-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Отображение пункта меню &quot;частный Marketplace&quot; в левой части Marketplace.":::

1. <span data-ttu-id="30c75-125">Выберите **Управление доступом (IAM)** , чтобы назначить роль администратора Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Отображает экран управления доступом к M.":::

1. <span data-ttu-id="30c75-127">Выберите **+ Добавить** > **Добавить назначение ролей**.</span><span class="sxs-lookup"><span data-stu-id="30c75-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="30c75-128">В разделе **роль** выберите **Администратор Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="30c75-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Отображает меню назначения ролей.":::

1. <span data-ttu-id="30c75-130">Выберите из раскрывающегося списка требуемого пользователя, а затем нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="30c75-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="30c75-131">Назначение роли администратора Marketplace с помощью PowerShell</span><span class="sxs-lookup"><span data-stu-id="30c75-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="30c75-132">Используйте следующий сценарий PowerShell для назначения роли администратора Marketplace. для этого требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="30c75-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="30c75-133">**ИД клиента:** Идентификатор клиента в области (роль администратора Marketplace назначается в области клиента).</span><span class="sxs-lookup"><span data-stu-id="30c75-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="30c75-134">**SubscriptionId:** Подписка, которой глобальный администратор имеет роль **участника** или более высокий назначенный.</span><span class="sxs-lookup"><span data-stu-id="30c75-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="30c75-135">**Глобаладминусернаме:** Имя пользователя глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="30c75-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="30c75-136">**Усернаметоассигнролефор:** Имя пользователя, которому будет назначена роль администратора Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="30c75-137">Для гостевых пользователей, приглашенных для клиента, может потребоваться до 48 часов, пока их учетная запись не будет доступна для назначения роли администратора Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="30c75-138">дополнительные сведения см. [в разделе свойства пользователя службы совместной работы B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="30c75-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="30c75-139">дополнительные сведения о командлетах, содержащихся в модуле PowerShell Az. Portal, см. в разделе [Microsoft Azure PowerShell: командлеты панели мониторинга портала](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="30c75-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="30c75-140">Создание частного решения Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="30c75-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="30c75-141">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="30c75-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="30c75-142">Выберите **все службы** , а затем **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="30c75-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Отображает портал Azure главное окно.":::

3. <span data-ttu-id="30c75-144">В меню слева выберите **частный Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="30c75-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="30c75-145">выберите **Начало работы** , чтобы создать частный магазин Azure Marketplace (это необходимо сделать только один раз).</span><span class="sxs-lookup"><span data-stu-id="30c75-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="показано, как выбрать Начало работы в главном окне портал Azure.":::

    <span data-ttu-id="30c75-147">Если для этого клиента уже существует частная служба Azure Marketplace, **Управление Marketplace** будет выбрано по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="30c75-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="30c75-148">После завершения вы получите пустой и отключенный частный Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Отображает пустой частный экран Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="30c75-150">Добавление элементов из коллекции</span><span class="sxs-lookup"><span data-stu-id="30c75-150">Add items from gallery</span></span>

<span data-ttu-id="30c75-151">Элемент — это сочетание предложения и плана.</span><span class="sxs-lookup"><span data-stu-id="30c75-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="30c75-152">Вы можете искать и добавлять элементы на странице Управление Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="30c75-153">Выберите **Добавить элементы**.</span><span class="sxs-lookup"><span data-stu-id="30c75-153">Select **Add items**.</span></span>

2. <span data-ttu-id="30c75-154">Просмотрите **коллекцию** или используйте поле поиска, чтобы найти нужный элемент.</span><span class="sxs-lookup"><span data-stu-id="30c75-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Показывает, как просматривать коллекцию или использовать поле поиска.":::

3. <span data-ttu-id="30c75-156">По умолчанию при добавлении нового предложения все текущие планы будут добавлены в список утвержденных.</span><span class="sxs-lookup"><span data-stu-id="30c75-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="30c75-157">Чтобы изменить выбор плана перед добавлением выбранных элементов, выберите раскрывающееся меню на плитке предложения и обновите необходимые планы.</span><span class="sxs-lookup"><span data-stu-id="30c75-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Показывает, как обновить обязательные планы.":::

4. <span data-ttu-id="30c75-159">Нажмите кнопку **Готово** в нижнем левом углу после того, как сделали выбор.</span><span class="sxs-lookup"><span data-stu-id="30c75-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="30c75-160">**Добавление элементов** в Marketplace будет доступно только для предложений сторонних разработчиков.</span><span class="sxs-lookup"><span data-stu-id="30c75-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="30c75-161">Решения Майкрософт (включая предустановленные [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros)) будут помечены как "утвержденные по умолчанию" и не могут управляться в частном Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="30c75-162">Изменить планы элемента</span><span class="sxs-lookup"><span data-stu-id="30c75-162">Edit item's plans</span></span>

<span data-ttu-id="30c75-163">Планы элемента можно изменить на странице Управление Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="30c75-164">В столбце **планы** проверьте доступные планы из раскрывающегося меню для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="30c75-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="30c75-165">Установите или снимите флажки, чтобы выбрать, какие планы следует сделать доступными для пользователей.</span><span class="sxs-lookup"><span data-stu-id="30c75-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Показывает, как установить или снять флажок для требуемого элемента.":::

   > [!NOTE]
   > <span data-ttu-id="30c75-167">Для каждого предложения требуется по крайней мере один план, который должен быть выбран для обновления.</span><span class="sxs-lookup"><span data-stu-id="30c75-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="30c75-168">Чтобы удалить все планы, связанные с предложением, удалите все предложения (см. следующий раздел).</span><span class="sxs-lookup"><span data-stu-id="30c75-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="30c75-169">Удаление предложений</span><span class="sxs-lookup"><span data-stu-id="30c75-169">Delete offers</span></span>

<span data-ttu-id="30c75-170">На странице "Управление Marketplace" установите флажок рядом с именем предложения (см. предыдущий экран) и выберите **удалить элементы**.</span><span class="sxs-lookup"><span data-stu-id="30c75-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="30c75-171">Включение и отключение частного магазина Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="30c75-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="30c75-172">На странице "Управление Marketplace" вы увидите одно из этих баннеров, которое показывает текущее состояние частного магазина Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="30c75-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Показывает баннер &quot;отключить состояние&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Показывает баннер &quot;включить состояние&quot;.":::

<span data-ttu-id="30c75-175">При необходимости вы можете включить или отключить частный Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="30c75-176">Если параметр отключен, выберите **включить частный рынок** для включения.</span><span class="sxs-lookup"><span data-stu-id="30c75-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="30c75-177">Если этот флажок установлен, выберите **Отключить частный Marketplace** для отключения.</span><span class="sxs-lookup"><span data-stu-id="30c75-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="30c75-178">Частный центр уведомлений Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="30c75-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="30c75-179">Центр уведомлений состоит из трех типов уведомлений и позволяет администратору Marketplace выполнять действия на основе уведомления:</span><span class="sxs-lookup"><span data-stu-id="30c75-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="30c75-180">Запросы на утверждение от пользователей для элементов, которые отсутствуют в списке утвержденных (см. статью [запрос на добавление предложений или планов](#request-to-add-offers-or-plans) ниже).</span><span class="sxs-lookup"><span data-stu-id="30c75-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="30c75-181">Новые уведомления о планах для предложений, у которых уже есть один или несколько планов в списке утвержденных.</span><span class="sxs-lookup"><span data-stu-id="30c75-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="30c75-182">Удалены уведомления о планах для элементов, которые находятся в списке утвержденных, но были удалены из глобального магазина Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="30c75-183">Чтобы получить доступ к центру уведомлений, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="30c75-183">To access the notification center:</span></span>

1. <span data-ttu-id="30c75-184">Выберите **уведомления** в меню слева.</span><span class="sxs-lookup"><span data-stu-id="30c75-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Отображает меню уведомления.":::

1. <span data-ttu-id="30c75-186">Выберите меню с многоточием для получения дополнительных действий.</span><span class="sxs-lookup"><span data-stu-id="30c75-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Отображает результаты меню &quot;другие параметры&quot;.":::

1. <span data-ttu-id="30c75-188">Для запросов плана **Отображение запросов** открывает форму запроса на утверждение, где можно просмотреть все запросы пользователей для конкретного предложения.</span><span class="sxs-lookup"><span data-stu-id="30c75-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="30c75-189">Выберите **утвердить** или **отклонить**.</span><span class="sxs-lookup"><span data-stu-id="30c75-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Показывает параметры утверждения и отклонения.":::

1. <span data-ttu-id="30c75-191">В раскрывающемся меню выберите план для утверждения.</span><span class="sxs-lookup"><span data-stu-id="30c75-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="30c75-192">Добавьте комментарий и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="30c75-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="30c75-193">Просмотр частного решения Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="30c75-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="30c75-194">Если частная служба Azure Marketplace включена, пользователи увидят планы, утвержденные администратором Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="30c75-195">Зеленое **утвержденное** уведомление указывает на то, что предложение Partner (не Майкрософт) утверждено.</span><span class="sxs-lookup"><span data-stu-id="30c75-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="30c75-196">Сообщение, **утвержденное** синим цветом, указывает на предложение Майкрософт (включая рекомендованные [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros)), которое утверждено.</span><span class="sxs-lookup"><span data-stu-id="30c75-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="30c75-197">Пользователи могут фильтровать предложения, которые являются и не утверждены:</span><span class="sxs-lookup"><span data-stu-id="30c75-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Отображает параметр фильтрации.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="30c75-199">Купить или развернуть в частном магазине Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="30c75-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="30c75-200">Хотя страница сведений о продукте похожа на глобальную среду Azure Marketplace, существуют три частных сценария Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="30c75-201">Когда пользователь выбирает утвержденный план, кнопка **создать** включена.</span><span class="sxs-lookup"><span data-stu-id="30c75-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Показывает баннер предложения, указывающее на возможность создания плана.":::

- <span data-ttu-id="30c75-203">Если выбор плана продукта не отображается на странице сведений о продукте, но администратор утвердил один или несколько планов, в баннер записываются утверждения о том, какие планы утверждены и включена кнопка **создать** :</span><span class="sxs-lookup"><span data-stu-id="30c75-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Показывает баннер предложения, указывающее, что можно создать план и Показать доступные планы.":::

- <span data-ttu-id="30c75-205">Когда пользователь выбирает Неутвержденный план, заголовок замещает план как не утвержденный и кнопка **создать** отключена.</span><span class="sxs-lookup"><span data-stu-id="30c75-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="30c75-206">Пользователь по-прежнему может запросить Добавление плана в список утвержденных (см. следующий раздел).</span><span class="sxs-lookup"><span data-stu-id="30c75-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="30c75-207">Запрос на добавление предложений или планов</span><span class="sxs-lookup"><span data-stu-id="30c75-207">Request to add offers or plans</span></span>

<span data-ttu-id="30c75-208">Вы можете запросить добавить открытое предложение или план, который сейчас не утвержден в частном магазине Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="30c75-209">Выберите **запрос для добавления** в баннере, чтобы открыть **форму запроса на доступ**.</span><span class="sxs-lookup"><span data-stu-id="30c75-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Отображает баннер с ссылкой &quot;запрос на добавление&quot;.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Отображает форму запроса на доступ к предложениям или планам.":::

1. <span data-ttu-id="30c75-212">Выберите, какие планы следует добавить в запрос (**любой план** сообщает администратору Marketplace, что у вас нет предпочтений для плана в предложении).</span><span class="sxs-lookup"><span data-stu-id="30c75-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="30c75-213">Добавьте **обоснование** и **запрос** на выборку, чтобы отправить запрос.</span><span class="sxs-lookup"><span data-stu-id="30c75-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Показывает форму запроса на доступ для предложений или планов с примерами записей.":::

1. <span data-ttu-id="30c75-215">Указание ожидающего запроса появится в форме запроса на доступ с возможностью **отказаться от запроса**.</span><span class="sxs-lookup"><span data-stu-id="30c75-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Отображает список утвержденных или ожидающих планов с ссылкой на отзыв запроса.":::

> [!NOTE]
> <span data-ttu-id="30c75-217">После отправки в [Центр уведомлений](#private-azure-marketplace-notification-center) будет отправлена форма запроса на утверждение, чтобы администратор Marketplace просмотрел запрос и принять меры.</span><span class="sxs-lookup"><span data-stu-id="30c75-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="30c75-218">Утверждение в частном Marketplace не означает закупку решения.</span><span class="sxs-lookup"><span data-stu-id="30c75-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="30c75-219">Часто задаваемые вопросы (FAQ)</span><span class="sxs-lookup"><span data-stu-id="30c75-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="30c75-220">Я уже блокировал стороннее приложение Marketplace с помощью политики Azure.</span><span class="sxs-lookup"><span data-stu-id="30c75-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="30c75-221">Как это отличается?</span><span class="sxs-lookup"><span data-stu-id="30c75-221">How is this different?</span></span>

<span data-ttu-id="30c75-222">В настоящее время существует два способа ограничения сторонних служб в Marketplace:</span><span class="sxs-lookup"><span data-stu-id="30c75-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="30c75-223">На портале EA или портал Azure отключите сторонние службы или ограничьте их только номерами SKU "бесплатный" или "BYOL".</span><span class="sxs-lookup"><span data-stu-id="30c75-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Показывает, как ограничить службы в портал Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Показывает, как ограничить службы на портале E A.":::

2. <span data-ttu-id="30c75-226">Создайте политику Azure, чтобы разрешить только определенные виртуальные машины.</span><span class="sxs-lookup"><span data-stu-id="30c75-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="30c75-227">дополнительные сведения о применении политики к Windows виртуальным машинам см. в статье [применение политик для Windows виртуальных машин с Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="30c75-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="30c75-228">Частная Azure Marketplace обеспечивает большую гибкость при предоставлении определенных предложений и планов.</span><span class="sxs-lookup"><span data-stu-id="30c75-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="30c75-229">Он информирует пользователей о доступности для развертывания в коллекции Marketplace даже перед тем, как они пытаются развернуть сторонние службы.</span><span class="sxs-lookup"><span data-stu-id="30c75-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="30c75-230">Чтобы разрешить развертывание сторонних служб, задайте для Azure Marketplace значение Вкл./включено на портале EA и в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="30c75-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="30c75-231">В частном магазине Azure Marketplace партнерские решения могут не ограничиваться виртуальными машинами.</span><span class="sxs-lookup"><span data-stu-id="30c75-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="30c75-232">Частный магазин Azure Marketplace может быть проверен на уровне плана и также может установить "текущий и будущий план".</span><span class="sxs-lookup"><span data-stu-id="30c75-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="30c75-233">В частном магазине Azure Marketplace можно сообщить конечным пользователям о том, что можно и что нельзя развернуть.</span><span class="sxs-lookup"><span data-stu-id="30c75-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="30c75-234">В чем разница между частным предложением и частным магазином Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="30c75-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="30c75-235">**Частное предложение** позволяет издателям создавать планы, которые видны только целевым клиентам.</span><span class="sxs-lookup"><span data-stu-id="30c75-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="30c75-236">Это позволяет частным пользователям совместно использовать настраиваемые решения с согласованными ценами, частными условиями и специализированными конфигурациями.</span><span class="sxs-lookup"><span data-stu-id="30c75-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="30c75-237">Дополнительные сведения см. [в разделе частные предложения в коммерческом магазине](/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="30c75-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="30c75-238">**Частная Azure Marketplace** в портал Azure позволяет администраторам заранее утверждать, какие сторонние решения могут развертывать пользователи.</span><span class="sxs-lookup"><span data-stu-id="30c75-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="30c75-239">Благодаря частному Azure Marketplace пользователи могут воспользоваться преимуществами Azure Marketplace, выполнив поиск, приобретение и развертывание соответствующих предложений.</span><span class="sxs-lookup"><span data-stu-id="30c75-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="30c75-240">Чтобы управлять частными предложениями на основе подписок в частном Marketplace, администратор Marketplace должен иметь минимальную роль "чтение" для конкретной подписки.</span><span class="sxs-lookup"><span data-stu-id="30c75-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="30c75-241">Я добавил Частное предложение в частный магазин Azure Marketplace, почему оно не отображается на вкладке Управление Marketplace?</span><span class="sxs-lookup"><span data-stu-id="30c75-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="30c75-242">Частные предложения на основе подписки видимы только для перечисленных подписок в параметрах частного предложения.</span><span class="sxs-lookup"><span data-stu-id="30c75-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="30c75-243">Чтобы просмотреть Частное предложение, убедитесь, что в фильтре глобальной подписки отображаются все подписки.</span><span class="sxs-lookup"><span data-stu-id="30c75-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Отображение частного фильтра Marketplace.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="30c75-245">Можно ли включить пользовательские образы в частном магазине Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="30c75-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="30c75-246">Нет.</span><span class="sxs-lookup"><span data-stu-id="30c75-246">No.</span></span> <span data-ttu-id="30c75-247">Частная служба Azure Marketplace позволяет любому ИТ-администратору управлять решениями сторонних разработчиков и администрировать их из глобального магазина Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="30c75-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="30c75-248">Поскольку пользовательские образы не находятся в глобальной службе Azure Marketplace, ИТ – администратор не может выбрать и выбрать собственные образы.</span><span class="sxs-lookup"><span data-stu-id="30c75-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="30c75-249">Если вы хотите предоставить общий доступ к пользовательским образам, воспользуйтесь [коллекцией Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="30c75-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="30c75-250">Пошаговое инструкции по созданию коллекции общих образов (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="30c75-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="30c75-251">Создание определения образа в SIG.</span><span class="sxs-lookup"><span data-stu-id="30c75-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="30c75-252">Клиент должен выбрать **обобщенный** для поля состояния ОС.</span><span class="sxs-lookup"><span data-stu-id="30c75-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="30c75-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="30c75-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="30c75-254">Перенесите управляемый образ в общую галерею образов ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="30c75-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="30c75-255">Образы виртуальных машин SIG будут находиться в одной подписке.</span><span class="sxs-lookup"><span data-stu-id="30c75-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="30c75-256">Чтобы сделать его доступным для других подписок, используйте регистрацию приложения ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="30c75-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="30c75-257">Почему я вижу некоторые предложения **, утвержденные по умолчанию** , несмотря на то, что издатель не является корпорацией Майкрософт?</span><span class="sxs-lookup"><span data-stu-id="30c75-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="30c75-258">Корпорация Майкрософт поддерживает Linux и технологию с открытым кодом в Azure.</span><span class="sxs-lookup"><span data-stu-id="30c75-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="30c75-259">Рекомендуемые [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros) поддерживаются в Azure, а цена интегрирована в виртуальные машины.</span><span class="sxs-lookup"><span data-stu-id="30c75-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="30c75-260">Так как агент Linux для Azure уже предварительно установлен в Azure Marketplace, он рассматривается как предложение Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="30c75-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="30c75-261">Так как предложения Майкрософт утверждены по умолчанию, Рекомендуемые дистрибутивы Linux не могут управляться в частном магазине Azure Marketplace и утверждены по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="30c75-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="30c75-262">Обращение в службу поддержки</span><span class="sxs-lookup"><span data-stu-id="30c75-262">Contact support</span></span>

- <span data-ttu-id="30c75-263">Для поддержки Azure Marketplace посетите веб [-сайт Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="30c75-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>