---
title: Создание частного магазина Azure Marketplace и управление им в портал Azure
description: Узнайте, как создать частный сайт Azure Marketplace (Предварительная версия) и управлять им в портал Azure.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: c0a395a7c5bfe926cdc56d7386aaaebb0305fb68
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2020
ms.locfileid: "91429354"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Создание и управление частными Azure Marketplace (Предварительная версия) в портал Azure

Частная среда Azure Marketplace (Предварительная версия) позволяет администраторам определять, какие сторонние решения могут использовать пользователи. Это позволяет развертывать только те предложения, которые вы утверждаете и соответствует политикам предприятия. Благодаря частному Azure Marketplace пользователи могут искать в Интернет-магазине соответствующие предложения для приобретения и развертывания. 

Как администратор Marketplace (назначенная роль), вы начнете с отключенного и пустого частного хранилища, в котором можно добавить утвержденные предложения и планы. В этой статье объясняется, как создавать частные Azure Marketplace для пользователей, управлять ими и включать их.

Примечания.

- Частный сайт Azure Marketplace находится на уровне клиента, поэтому все пользователи в клиенте будут видеть один проверенный список.
- Все решения Майкрософт автоматически добавляются в частный магазин Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Назначение роли администратора Marketplace

Глобальный администратор клиента должен назначить роль **администратора Marketplace** частному администратору Azure Marketplace, который будет управлять частным хранилищем.

>[!IMPORTANT]
> Доступ к частному управлению Azure Marketplace доступен только ИТ-администраторам с назначенной ролью администратора Marketplace.

### <a name="prerequisites"></a>предварительные требования

Прежде чем назначать роль администратора Marketplace пользователю в области клиента, необходимо выполнить эти предварительные требования.

- У вас есть доступ к пользователю **глобального администратора** .
- У клиента есть по крайней мере одна подписка (может иметь любой тип).
- Пользователю глобального администратора назначается роль **участника** или выше для подписки, выбранной на шаге 2.
- Уровень доступа пользователя глобального администратора имеет значение **Да** (см. раздел [повышение прав-доступ-глобальный-администратор](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Назначение роли администратора Marketplace с помощью PowerShell

Используйте следующий сценарий PowerShell для назначения роли администратора Marketplace. для этого требуются следующие параметры:

- **ИД клиента:** Идентификатор клиента в области (роль администратора Marketplace назначается в области клиента).
- **SubscriptionId:** Подписка, которой глобальный администратор имеет роль **участника** или более высокий назначенный.
- **Глобаладминусернаме:** Имя пользователя глобального администратора.
- **Усернаметоассигнролефор:** Имя пользователя, которому будет назначена роль администратора Marketplace.

> [!NOTE]
> Для гостевых пользователей, приглашенных для клиента, может потребоваться до 48 часов, пока их учетная запись не будет доступна для назначения роли администратора Marketplace. Дополнительные сведения см. [в разделе Свойства пользователя службы совместной работы B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).

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

Дополнительные сведения о командлетах, содержащихся в модуле PowerShell AZ. Portal, см. в разделе [Microsoft Azure PowerShell: командлеты панели мониторинга портала](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Создание частного решения Azure Marketplace

1. Войдите на [портал Azure](https://portal.azure.com/).
2. Выберите **все службы** , а затем **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Портал Azure главное окно.":::

3. Выберите **частный Marketplace** в параметрах слева.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Портал Azure главное окно.":::

4. Выберите **начать работу** , чтобы создать частный магазин Azure Marketplace (это необходимо сделать только один раз).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Портал Azure главное окно.":::

    Если для этого клиента уже существует частная служба Azure Marketplace, **Управление Marketplace** будет выбрано по умолчанию.

5. После завершения вы получите пустой и отключенный частный Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Портал Azure главное окно.":::

## <a name="add-items-from-gallery"></a>Добавление элементов из коллекции

Элемент — это сочетание предложения и плана. Вы можете найти и добавить элемент на странице Управление Marketplace.

1. Выберите **Добавить элементы**.

2. Просмотрите **коллекцию** или используйте поле поиска, чтобы найти нужный элемент.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Портал Azure главное окно.":::

3. По умолчанию при добавлении нового предложения все текущие планы будут добавлены в список разрешенных. Чтобы изменить выбор плана перед добавлением выбранных элементов, выберите раскрывающееся меню на плитке предложения и обновите необходимые планы.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Портал Azure главное окно.":::

4. Нажмите кнопку **Готово** в нижнем левом углу после того, как сделали выбор.

>[!Note]
> **Добавление элементов** в Marketplace будет доступно только для предложений сторонних разработчиков. Предложения Майкрософт по умолчанию разрешены.

## <a name="edit-item-plans"></a>Изменение планов элементов

Планы элемента можно изменить на странице Управление Marketplace.

1. В столбце **планы** проверьте доступные планы из раскрывающегося меню для этого элемента.
2. Установите или снимите флажки, чтобы выбрать, какие планы следует сделать доступными для пользователей.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Портал Azure главное окно.":::

> [!NOTE]
> Для каждого предложения необходимо выбрать по крайней мере один план, чтобы обновление было выполнено. Чтобы удалить все планы, связанные с предложением, удалите все предложения (см. следующий раздел).

## <a name="delete-offers"></a>Удаление предложений

На странице "Управление Marketplace" установите флажок рядом с именем предложения (см. предыдущий экран) и выберите **удалить элементы**.

## <a name="enabledisable-private-azure-marketplace"></a>Включение и отключение частного магазина Azure Marketplace

На странице "Управление Marketplace" вы увидите одно из этих баннеров, которое показывает текущее состояние частного магазина Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Портал Azure главное окно.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Портал Azure главное окно.":::

При необходимости вы можете включить или отключить частный Azure Marketplace.

1. Если параметр отключен, выберите **включить частный рынок** для включения.
2. Если этот флажок установлен, выберите **Отключить частный Marketplace** для отключения.

## <a name="browsing-private-azure-marketplace"></a>Просмотр частного решения Azure Marketplace

Если частная служба Azure Marketplace включена, пользователи увидят, какие планы разрешены администратором Marketplace.

- Зеленое **разрешенное** уведомление указывает на то, что предложение Partner (не Майкрософт) разрешено.
- Появление синего **разрешенного** уведомления означает, что предложение Microsoft разрешено.

Пользователи могут фильтровать предложения, которые являются и недопустимыми:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Портал Azure главное окно.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Купить или развернуть в частном магазине Azure Marketplace

Хотя страница сведений о продукте похожа на общедоступную среду Azure Marketplace, существует три частных сценария Azure Marketplace.

- Когда пользователь выбирает разрешенный план, кнопка **создать** включена.

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Портал Azure главное окно.":::

- Когда пользователь выбирает неразрешенный план, баннер заметит, что этот план не разрешен и кнопка **создать** отключена.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Портал Azure главное окно.":::

- Если выбор плана продукта не отображается на странице сведений о продукте, но администратор утвердил один или несколько планов, в баннер записываются разрешенные планы и включена кнопка **создать** .

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Портал Azure главное окно.":::

## <a name="contact-support"></a>Обращение в службу поддержки

Для поддержки Azure Marketplace посетите веб [-сайт Microsoft Q&A](/answers/products/). 