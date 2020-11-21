---
title: Создание частного магазина Azure Marketplace и управление им в портал Azure
description: Узнайте, как создать частный сайт Azure Marketplace (Предварительная версия) и управлять им в портал Azure.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: f62c9aef13b51ba2db42b267d7620f506bbdc1ec
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006945"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="3000c-103">Создание и управление частными Azure Marketplace (Предварительная версия) в портал Azure</span><span class="sxs-lookup"><span data-stu-id="3000c-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="3000c-104">Частная среда Azure Marketplace (Предварительная версия) позволяет администраторам определять, какие сторонние решения могут использовать пользователи.</span><span class="sxs-lookup"><span data-stu-id="3000c-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="3000c-105">Это позволяет развертывать только те предложения, которые вы утверждаете и соответствует политикам предприятия.</span><span class="sxs-lookup"><span data-stu-id="3000c-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="3000c-106">Благодаря частному Azure Marketplace пользователи могут искать в Интернет-магазине соответствующие предложения для приобретения и развертывания.</span><span class="sxs-lookup"><span data-stu-id="3000c-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="3000c-107">Как администратор Marketplace (назначенная роль), вы начнете с отключенного и пустого частного хранилища, в котором можно добавить утвержденные предложения и планы.</span><span class="sxs-lookup"><span data-stu-id="3000c-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="3000c-108">В этой статье объясняется, как создавать частные Azure Marketplace для пользователей, управлять ими и включать их.</span><span class="sxs-lookup"><span data-stu-id="3000c-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="3000c-109">Примечания.</span><span class="sxs-lookup"><span data-stu-id="3000c-109">Notes:</span></span>

- <span data-ttu-id="3000c-110">Частный сайт Azure Marketplace находится на уровне клиента, поэтому все пользователи в клиенте будут видеть один проверенный список.</span><span class="sxs-lookup"><span data-stu-id="3000c-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="3000c-111">Все решения Майкрософт автоматически добавляются в частный магазин Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="3000c-112">Назначение роли администратора Marketplace</span><span class="sxs-lookup"><span data-stu-id="3000c-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="3000c-113">Глобальный администратор клиента должен назначить роль **администратора Marketplace** частному администратору Azure Marketplace, который будет управлять частным хранилищем.</span><span class="sxs-lookup"><span data-stu-id="3000c-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="3000c-114">Доступ к частному управлению Azure Marketplace доступен только ИТ-администраторам с назначенной ролью администратора Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="3000c-115">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3000c-115">Prerequisites</span></span>

<span data-ttu-id="3000c-116">Прежде чем назначать роль администратора Marketplace пользователю в области клиента, необходимо выполнить эти предварительные требования.</span><span class="sxs-lookup"><span data-stu-id="3000c-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="3000c-117">У вас есть доступ к пользователю **глобального администратора** .</span><span class="sxs-lookup"><span data-stu-id="3000c-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="3000c-118">У клиента есть по крайней мере одна подписка (может иметь любой тип).</span><span class="sxs-lookup"><span data-stu-id="3000c-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="3000c-119">Пользователю глобального администратора назначается роль **участника** или выше для выбранной подписки.</span><span class="sxs-lookup"><span data-stu-id="3000c-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>
- <span data-ttu-id="3000c-120">Уровень доступа пользователя глобального администратора имеет значение **Да** (см. раздел [повышение уровня доступа для управления всеми подписками Azure и группами управления](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="3000c-120">The Global administrator user has elevated access set to **Yes** (see [Elevate access to manage all Azure subscriptions and management groups](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="3000c-121">Назначение роли администратора Marketplace с помощью PowerShell</span><span class="sxs-lookup"><span data-stu-id="3000c-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="3000c-122">Используйте следующий сценарий PowerShell для назначения роли администратора Marketplace. для этого требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="3000c-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="3000c-123">**ИД клиента:** Идентификатор клиента в области (роль администратора Marketplace назначается в области клиента).</span><span class="sxs-lookup"><span data-stu-id="3000c-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="3000c-124">**SubscriptionId:** Подписка, которой глобальный администратор имеет роль **участника** или более высокий назначенный.</span><span class="sxs-lookup"><span data-stu-id="3000c-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="3000c-125">**Глобаладминусернаме:** Имя пользователя глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="3000c-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="3000c-126">**Усернаметоассигнролефор:** Имя пользователя, которому будет назначена роль администратора Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="3000c-127">Для гостевых пользователей, приглашенных для клиента, может потребоваться до 48 часов, пока их учетная запись не будет доступна для назначения роли администратора Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="3000c-128">Дополнительные сведения см. [в разделе Свойства пользователя службы совместной работы B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="3000c-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."
$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="3000c-129">Дополнительные сведения о командлетах, содержащихся в модуле PowerShell AZ. Portal, см. в разделе [Microsoft Azure PowerShell: командлеты панели мониторинга портала](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="3000c-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="3000c-130">Создание частного решения Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="3000c-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="3000c-131">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3000c-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="3000c-132">Выберите **все службы** , а затем **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="3000c-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Портал Azure главное окно.":::

3. <span data-ttu-id="3000c-134">Выберите **частный Marketplace** в параметрах слева.</span><span class="sxs-lookup"><span data-stu-id="3000c-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Выбор частного Marketplace в главном окне портал Azure.":::

4. <span data-ttu-id="3000c-136">Выберите **начать работу** , чтобы создать частный магазин Azure Marketplace (это необходимо сделать только один раз).</span><span class="sxs-lookup"><span data-stu-id="3000c-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Выберите начало работы в главном окне портал Azure.":::

    <span data-ttu-id="3000c-138">Если для этого клиента уже существует частная служба Azure Marketplace, **Управление Marketplace** будет выбрано по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3000c-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="3000c-139">После завершения вы получите пустой и отключенный частный Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Пустой частный экран Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="3000c-141">Добавление элементов из коллекции</span><span class="sxs-lookup"><span data-stu-id="3000c-141">Add items from gallery</span></span>

<span data-ttu-id="3000c-142">Элемент — это сочетание предложения и плана.</span><span class="sxs-lookup"><span data-stu-id="3000c-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="3000c-143">Вы можете найти и добавить элемент на странице Управление Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="3000c-144">Выберите **Добавить элементы**.</span><span class="sxs-lookup"><span data-stu-id="3000c-144">Select **Add items**.</span></span>

2. <span data-ttu-id="3000c-145">Просмотрите **коллекцию** или используйте поле поиска, чтобы найти нужный элемент.</span><span class="sxs-lookup"><span data-stu-id="3000c-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Просмотр коллекции или использование поля поиска.":::

3. <span data-ttu-id="3000c-147">По умолчанию при добавлении нового предложения все текущие планы будут добавлены в список разрешенных.</span><span class="sxs-lookup"><span data-stu-id="3000c-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="3000c-148">Чтобы изменить выбор плана перед добавлением выбранных элементов, выберите раскрывающееся меню на плитке предложения и обновите необходимые планы.</span><span class="sxs-lookup"><span data-stu-id="3000c-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Обновите обязательные планы.":::

4. <span data-ttu-id="3000c-150">Нажмите кнопку **Готово** в нижнем левом углу после того, как сделали выбор.</span><span class="sxs-lookup"><span data-stu-id="3000c-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="3000c-151">**Добавление элементов** в Marketplace будет доступно только для предложений сторонних разработчиков.</span><span class="sxs-lookup"><span data-stu-id="3000c-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="3000c-152">Предложения Майкрософт по умолчанию разрешены.</span><span class="sxs-lookup"><span data-stu-id="3000c-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="3000c-153">Изменение планов элементов</span><span class="sxs-lookup"><span data-stu-id="3000c-153">Edit item plans</span></span>

<span data-ttu-id="3000c-154">Планы элемента можно изменить на странице Управление Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="3000c-155">В столбце **планы** проверьте доступные планы из раскрывающегося меню для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="3000c-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="3000c-156">Установите или снимите флажки, чтобы выбрать, какие планы следует сделать доступными для пользователей.</span><span class="sxs-lookup"><span data-stu-id="3000c-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Установка или снятие флажка для требуемого элемента.":::

> [!NOTE]
> <span data-ttu-id="3000c-158">Для каждого предложения необходимо выбрать по крайней мере один план, чтобы обновление было выполнено.</span><span class="sxs-lookup"><span data-stu-id="3000c-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="3000c-159">Чтобы удалить все планы, связанные с предложением, удалите все предложения (см. следующий раздел).</span><span class="sxs-lookup"><span data-stu-id="3000c-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="3000c-160">Удаление предложений</span><span class="sxs-lookup"><span data-stu-id="3000c-160">Delete offers</span></span>

<span data-ttu-id="3000c-161">На странице "Управление Marketplace" установите флажок рядом с именем предложения (см. предыдущий экран) и выберите **удалить элементы**.</span><span class="sxs-lookup"><span data-stu-id="3000c-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="3000c-162">Включение и отключение частного магазина Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="3000c-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="3000c-163">На странице "Управление Marketplace" вы увидите одно из этих баннеров, которое показывает текущее состояние частного магазина Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="3000c-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Отключить баннер состояния":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Включить баннер состояния":::

<span data-ttu-id="3000c-166">При необходимости вы можете включить или отключить частный Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="3000c-167">Если параметр отключен, выберите **включить частный рынок** для включения.</span><span class="sxs-lookup"><span data-stu-id="3000c-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="3000c-168">Если этот флажок установлен, выберите **Отключить частный Marketplace** для отключения.</span><span class="sxs-lookup"><span data-stu-id="3000c-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="3000c-169">Просмотр частного решения Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="3000c-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="3000c-170">Если частная служба Azure Marketplace включена, пользователи увидят, какие планы разрешены администратором Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="3000c-171">Зеленое **разрешенное** уведомление указывает на то, что предложение Partner (не Майкрософт) разрешено.</span><span class="sxs-lookup"><span data-stu-id="3000c-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="3000c-172">Появление синего **разрешенного** уведомления означает, что предложение Microsoft разрешено.</span><span class="sxs-lookup"><span data-stu-id="3000c-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="3000c-173">Пользователи могут фильтровать предложения, которые являются и недопустимыми:</span><span class="sxs-lookup"><span data-stu-id="3000c-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Параметр фильтрации.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="3000c-175">Купить или развернуть в частном магазине Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="3000c-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="3000c-176">Хотя страница сведений о продукте похожа на общедоступную среду Azure Marketplace, существует три частных сценария Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3000c-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="3000c-177">Когда пользователь выбирает разрешенный план, кнопка **создать** включена.</span><span class="sxs-lookup"><span data-stu-id="3000c-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Баннер предложения с указанием на возможность создания плана.":::

- <span data-ttu-id="3000c-179">Когда пользователь выбирает неразрешенный план, баннер заметит, что этот план не разрешен и кнопка **создать** отключена.</span><span class="sxs-lookup"><span data-stu-id="3000c-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Баннер предложения, указывающее, что план не может быть создан.":::

- <span data-ttu-id="3000c-181">Если выбор плана продукта не отображается на странице сведений о продукте, но администратор утвердил один или несколько планов, в баннер записываются разрешенные планы и включена кнопка **создать** .</span><span class="sxs-lookup"><span data-stu-id="3000c-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Баннер предложения с уведомлением о том, что план можно создать и Показать доступные планы.":::

## <a name="contact-support"></a><span data-ttu-id="3000c-183">Обращение в службу поддержки</span><span class="sxs-lookup"><span data-stu-id="3000c-183">Contact support</span></span>

<span data-ttu-id="3000c-184">Для поддержки Azure Marketplace посетите веб [-сайт Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="3000c-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
