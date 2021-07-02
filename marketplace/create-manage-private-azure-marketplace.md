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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Создание частного магазина Azure Marketplace и управление им в портал Azure

Частная среда Azure Marketplace позволяет администраторам определять, какие решения сторонних разработчиков могут использовать пользователи. Это позволяет пользователю развертывать только предложения, утвержденные администратором и соответствующие политикам предприятия. Благодаря частному Azure Marketplace пользователи могут искать в Интернет-магазине соответствующие предложения для приобретения и развертывания.

Как администратор Marketplace (назначенная роль), вы начнете с отключенного и пустого частного хранилища, в котором можно добавить утвержденные предложения и планы. В этой статье описывается назначение необходимой роли, создание частного хранилища, Управление элементами, утверждение запросов пользователей и включение частного магазина Azure Marketplace для пользователей.

> [!NOTE]
> - Частный сайт Azure Marketplace находится на уровне клиента, поэтому все пользователи в клиенте будут видеть один проверенный список.
> - Все решения Майкрософт (включая предустановленные [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros)) автоматически добавляются в частный магазин Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Назначение роли администратора Marketplace

Глобальный администратор клиента должен назначить роль **администратора Marketplace** частному администратору Azure Marketplace, который будет управлять частным хранилищем.

>[!IMPORTANT]
> Доступ к частному управлению Azure Marketplace доступен только ИТ-администраторам с назначенной ролью администратора Marketplace.

### <a name="prerequisites"></a>Предварительные требования

Эти предварительные требования необходимы, прежде чем можно будет назначить роль администратора Marketplace пользователю в области клиента:

- У вас есть доступ к пользователю **глобального администратора** .
- У клиента есть по крайней мере одна подписка (может иметь любой тип).
- Пользователю глобального администратора назначается роль **участника** или выше для выбранной подписки.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Назначение роли администратора Marketplace с помощью управления доступом (IAM)

1. Войдите на [портал Azure](https://portal.azure.com/).

1. Выберите **все службы** , а затем **Marketplace**.

1. В меню слева выберите **частный Marketplace** .

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Отображение пункта меню &quot;частный Marketplace&quot; в левой части Marketplace.":::

1. Выберите **Управление доступом (IAM)** , чтобы назначить роль администратора Marketplace.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Отображает экран управления доступом к M.":::

1. Выберите **+ Добавить** > **Добавить назначение ролей**.

1. В разделе **роль** выберите **Администратор Marketplace**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Отображает меню назначения ролей.":::

1. Выберите из раскрывающегося списка требуемого пользователя, а затем нажмите кнопку **Готово**.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Назначение роли администратора Marketplace с помощью PowerShell

Используйте следующий сценарий PowerShell для назначения роли администратора Marketplace. для этого требуются следующие параметры:

- **ИД клиента:** Идентификатор клиента в области (роль администратора Marketplace назначается в области клиента).
- **SubscriptionId:** Подписка, которой глобальный администратор имеет роль **участника** или более высокий назначенный.
- **Глобаладминусернаме:** Имя пользователя глобального администратора.
- **Усернаметоассигнролефор:** Имя пользователя, которому будет назначена роль администратора Marketplace.

> [!NOTE]
> Для гостевых пользователей, приглашенных для клиента, может потребоваться до 48 часов, пока их учетная запись не будет доступна для назначения роли администратора Marketplace. дополнительные сведения см. [в разделе свойства пользователя службы совместной работы B2B Azure Active Directory](/azure/active-directory/b2b/user-properties).

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

дополнительные сведения о командлетах, содержащихся в модуле PowerShell Az. Portal, см. в разделе [Microsoft Azure PowerShell: командлеты панели мониторинга портала](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Создание частного решения Azure Marketplace

1. Войдите на [портал Azure](https://portal.azure.com/).
2. Выберите **все службы** , а затем **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Отображает портал Azure главное окно.":::

3. В меню слева выберите **частный Marketplace** .

4. выберите **Начало работы** , чтобы создать частный магазин Azure Marketplace (это необходимо сделать только один раз).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="показано, как выбрать Начало работы в главном окне портал Azure.":::

    Если для этого клиента уже существует частная служба Azure Marketplace, **Управление Marketplace** будет выбрано по умолчанию.

5. После завершения вы получите пустой и отключенный частный Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Отображает пустой частный экран Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Добавление элементов из коллекции

Элемент — это сочетание предложения и плана. Вы можете искать и добавлять элементы на странице Управление Marketplace.

1. Выберите **Добавить элементы**.

2. Просмотрите **коллекцию** или используйте поле поиска, чтобы найти нужный элемент.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Показывает, как просматривать коллекцию или использовать поле поиска.":::

3. По умолчанию при добавлении нового предложения все текущие планы будут добавлены в список утвержденных. Чтобы изменить выбор плана перед добавлением выбранных элементов, выберите раскрывающееся меню на плитке предложения и обновите необходимые планы.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Показывает, как обновить обязательные планы.":::

4. Нажмите кнопку **Готово** в нижнем левом углу после того, как сделали выбор.

>[!Note]
> **Добавление элементов** в Marketplace будет доступно только для предложений сторонних разработчиков. Решения Майкрософт (включая предустановленные [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros)) будут помечены как "утвержденные по умолчанию" и не могут управляться в частном Marketplace.

## <a name="edit-items-plans"></a>Изменить планы элемента

Планы элемента можно изменить на странице Управление Marketplace.

1. В столбце **планы** проверьте доступные планы из раскрывающегося меню для этого элемента.

2. Установите или снимите флажки, чтобы выбрать, какие планы следует сделать доступными для пользователей.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Показывает, как установить или снять флажок для требуемого элемента.":::

   > [!NOTE]
   > Для каждого предложения требуется по крайней мере один план, который должен быть выбран для обновления. Чтобы удалить все планы, связанные с предложением, удалите все предложения (см. следующий раздел).

## <a name="delete-offers"></a>Удаление предложений

На странице "Управление Marketplace" установите флажок рядом с именем предложения (см. предыдущий экран) и выберите **удалить элементы**.

## <a name="enabledisable-private-azure-marketplace"></a>Включение и отключение частного магазина Azure Marketplace

На странице "Управление Marketplace" вы увидите одно из этих баннеров, которое показывает текущее состояние частного магазина Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Показывает баннер &quot;отключить состояние&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Показывает баннер &quot;включить состояние&quot;.":::

При необходимости вы можете включить или отключить частный Azure Marketplace.

- Если параметр отключен, выберите **включить частный рынок** для включения.
- Если этот флажок установлен, выберите **Отключить частный Marketplace** для отключения.

## <a name="private-azure-marketplace-notification-center"></a>Частный центр уведомлений Azure Marketplace

Центр уведомлений состоит из трех типов уведомлений и позволяет администратору Marketplace выполнять действия на основе уведомления:

- Запросы на утверждение от пользователей для элементов, которые отсутствуют в списке утвержденных (см. статью [запрос на добавление предложений или планов](#request-to-add-offers-or-plans) ниже).
- Новые уведомления о планах для предложений, у которых уже есть один или несколько планов в списке утвержденных.
- Удалены уведомления о планах для элементов, которые находятся в списке утвержденных, но были удалены из глобального магазина Azure Marketplace.

Чтобы получить доступ к центру уведомлений, сделайте следующее:

1. Выберите **уведомления** в меню слева.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Отображает меню уведомления.":::

1. Выберите меню с многоточием для получения дополнительных действий.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Отображает результаты меню &quot;другие параметры&quot;.":::

1. Для запросов плана **Отображение запросов** открывает форму запроса на утверждение, где можно просмотреть все запросы пользователей для конкретного предложения.
1. Выберите **утвердить** или **отклонить**.

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Показывает параметры утверждения и отклонения.":::

1. В раскрывающемся меню выберите план для утверждения.
1. Добавьте комментарий и выберите **Отправить**.

## <a name="browsing-private-azure-marketplace"></a>Просмотр частного решения Azure Marketplace

Если частная служба Azure Marketplace включена, пользователи увидят планы, утвержденные администратором Marketplace.

- Зеленое **утвержденное** уведомление указывает на то, что предложение Partner (не Майкрософт) утверждено.
- Сообщение, **утвержденное** синим цветом, указывает на предложение Майкрософт (включая рекомендованные [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros)), которое утверждено.

Пользователи могут фильтровать предложения, которые являются и не утверждены:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Отображает параметр фильтрации.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Купить или развернуть в частном магазине Azure Marketplace

Хотя страница сведений о продукте похожа на глобальную среду Azure Marketplace, существуют три частных сценария Azure Marketplace.

- Когда пользователь выбирает утвержденный план, кнопка **создать** включена.

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Показывает баннер предложения, указывающее на возможность создания плана.":::

- Если выбор плана продукта не отображается на странице сведений о продукте, но администратор утвердил один или несколько планов, в баннер записываются утверждения о том, какие планы утверждены и включена кнопка **создать** :

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Показывает баннер предложения, указывающее, что можно создать план и Показать доступные планы.":::

- Когда пользователь выбирает Неутвержденный план, заголовок замещает план как не утвержденный и кнопка **создать** отключена. Пользователь по-прежнему может запросить Добавление плана в список утвержденных (см. следующий раздел).

## <a name="request-to-add-offers-or-plans"></a>Запрос на добавление предложений или планов

Вы можете запросить добавить открытое предложение или план, который сейчас не утвержден в частном магазине Azure Marketplace.

1. Выберите **запрос для добавления** в баннере, чтобы открыть **форму запроса на доступ**.

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Отображает баннер с ссылкой &quot;запрос на добавление&quot;.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Отображает форму запроса на доступ к предложениям или планам.":::

1. Выберите, какие планы следует добавить в запрос (**любой план** сообщает администратору Marketplace, что у вас нет предпочтений для плана в предложении).

1. Добавьте **обоснование** и **запрос** на выборку, чтобы отправить запрос.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Показывает форму запроса на доступ для предложений или планов с примерами записей.":::

1. Указание ожидающего запроса появится в форме запроса на доступ с возможностью **отказаться от запроса**.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Отображает список утвержденных или ожидающих планов с ссылкой на отзыв запроса.":::

> [!NOTE]
> После отправки в [Центр уведомлений](#private-azure-marketplace-notification-center) будет отправлена форма запроса на утверждение, чтобы администратор Marketplace просмотрел запрос и принять меры.

> [!CAUTION]
> Утверждение в частном Marketplace не означает закупку решения.

## <a name="frequently-asked-questions-faqs"></a>Часто задаваемые вопросы (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Я уже блокировал стороннее приложение Marketplace с помощью политики Azure. Как это отличается?

В настоящее время существует два способа ограничения сторонних служб в Marketplace:

1. На портале EA или портал Azure отключите сторонние службы или ограничьте их только номерами SKU "бесплатный" или "BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Показывает, как ограничить службы в портал Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Показывает, как ограничить службы на портале E A.":::

2. Создайте политику Azure, чтобы разрешить только определенные виртуальные машины. дополнительные сведения о применении политики к Windows виртуальным машинам см. в статье [применение политик для Windows виртуальных машин с Azure Resource Manager](/azure/virtual-machines/windows/policy).

Частная Azure Marketplace обеспечивает большую гибкость при предоставлении определенных предложений и планов. Он информирует пользователей о доступности для развертывания в коллекции Marketplace даже перед тем, как они пытаются развернуть сторонние службы. Чтобы разрешить развертывание сторонних служб, задайте для Azure Marketplace значение Вкл./включено на портале EA и в портал Azure.

- В частном магазине Azure Marketplace партнерские решения могут не ограничиваться виртуальными машинами.
- Частный магазин Azure Marketplace может быть проверен на уровне плана и также может установить "текущий и будущий план".
- В частном магазине Azure Marketplace можно сообщить конечным пользователям о том, что можно и что нельзя развернуть.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>В чем разница между частным предложением и частным магазином Azure Marketplace?

**Частное предложение** позволяет издателям создавать планы, которые видны только целевым клиентам. Это позволяет частным пользователям совместно использовать настраиваемые решения с согласованными ценами, частными условиями и специализированными конфигурациями. Дополнительные сведения см. [в разделе частные предложения в коммерческом магазине](/azure/marketplace/private-offers).

**Частная Azure Marketplace** в портал Azure позволяет администраторам заранее утверждать, какие сторонние решения могут развертывать пользователи. Благодаря частному Azure Marketplace пользователи могут воспользоваться преимуществами Azure Marketplace, выполнив поиск, приобретение и развертывание соответствующих предложений. Чтобы управлять частными предложениями на основе подписок в частном Marketplace, администратор Marketplace должен иметь минимальную роль "чтение" для конкретной подписки.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Я добавил Частное предложение в частный магазин Azure Marketplace, почему оно не отображается на вкладке Управление Marketplace?

Частные предложения на основе подписки видимы только для перечисленных подписок в параметрах частного предложения. Чтобы просмотреть Частное предложение, убедитесь, что в фильтре глобальной подписки отображаются все подписки.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Отображение частного фильтра Marketplace.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Можно ли включить пользовательские образы в частном магазине Azure Marketplace?

Нет. Частная служба Azure Marketplace позволяет любому ИТ-администратору управлять решениями сторонних разработчиков и администрировать их из глобального магазина Azure Marketplace. Поскольку пользовательские образы не находятся в глобальной службе Azure Marketplace, ИТ – администратор не может выбрать и выбрать собственные образы. Если вы хотите предоставить общий доступ к пользовательским образам, воспользуйтесь [коллекцией Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).

1. Пошаговое инструкции по созданию коллекции общих образов (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Создание определения образа в SIG. Клиент должен выбрать **обобщенный** для поля состояния ОС. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Перенесите управляемый образ в общую галерею образов ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. Образы виртуальных машин SIG будут находиться в одной подписке. Чтобы сделать его доступным для других подписок, используйте регистрацию приложения ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Почему я вижу некоторые предложения **, утвержденные по умолчанию** , несмотря на то, что издатель не является корпорацией Майкрософт?

Корпорация Майкрософт поддерживает Linux и технологию с открытым кодом в Azure. Рекомендуемые [дистрибутивы Linux](/azure/virtual-machines/linux/endorsed-distros) поддерживаются в Azure, а цена интегрирована в виртуальные машины. Так как агент Linux для Azure уже предварительно установлен в Azure Marketplace, он рассматривается как предложение Майкрософт. Так как предложения Майкрософт утверждены по умолчанию, Рекомендуемые дистрибутивы Linux не могут управляться в частном магазине Azure Marketplace и утверждены по умолчанию.

## <a name="contact-support"></a>Обращение в службу поддержки

- Для поддержки Azure Marketplace посетите веб [-сайт Microsoft Q&A](/answers/products/).