---
title: Возобновление использования привилегий администратора для Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как помочь клиентам возобновить использование привилегий администратора партнера, чтобы партнер мог помочь им в управлении клиентскими подписками поставщика облачных решений (CSP) Azure.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510182"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Возобновление использования привилегий администратора для клиентских подписок Azure CSP  

**Соответствующие роли:** глобальный администратор | агент по администрированию

Клиенты часто ожидают, что будучи поставщиком облачных решений (CSP) вы будете управлять использованием ресурсов Azure клиентов и системами клиентов. У вас должны быть привилегии администратора для выполнения этих действий. Одни привилегии предоставляются при установлении отношений торгового посредничества между вами и клиентом. Другие привилегии предоставляются вашим клиентом.

## <a name="admin-privileges-for-azure-in-csp"></a>Привилегии администратора для Azure в CSP

Существуют два уровня привилегий администратора для Azure в CSP.

- **Привилегии администратора уровня арендатора (делегированные привилегии)** . Партнеры CSP получают эти привилегии при установлении отношений торгового посредника CSP с клиентами. Делегированные привилегии администратора предоставляют партнерам CSP доступ к арендаторам клиентов. Этот доступ позволяет им выполнять административные задачи, такие как добавление пользователей и управление ими, сброс паролей и управление лицензиями пользователей.
- **Привилегии администратора уровня подписки**. Партнеры CSP получают эти привилегии при создании подписок Azure в CSP для своих клиентов. Такие привилегии обеспечивают партнерам в рамках CSP полный доступ к данным подпискам, что позволяет им подготавливать ресурсы Azure и управлять ими.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Возобновление использования привилегий администратора для партнеров CSP

Клиент может повторно создать назначение роли CSP, если вы предоставите ему `object ID` группы AdminAgents. Чтобы повторно получить делегированные привилегии администратора, необходимо выполнить следующие действия совместно с клиентом.

1. Войдите на панель мониторинга Центра партнеров.

2. В меню Центра партнеров выберите **Клиенты**.

3. Выберите клиента, с которым вы работаете, и **запросите установление отношений, в которых вы выполняете роль торгового посредника**. В результате создается ссылка на клиента, у которого есть привилегии администратора арендатора.

4. Клиенту следует перейти по ссылке и подтвердить запрос на установление отношений, в которых вы выполняете роль торгового посредника.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Пример сообщения электронной почты о создании отношений торгового посредничества":::.

5. Чтобы получить идентификатор объекта группы AdminAgents, вам (как партнеру) необходимо подключиться к арендатору партнера.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Затем клиент должен выполнить следующие действия с помощью PowerShell или Azure CLI. У клиента должны быть:

- Роль **владельца** или **администратора доступа пользователей**. 
- Разрешения на создание назначений ролей на уровне подписки.

   a. Только для PowerShell: клиент должен обновить модуль `Az.Resources`.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Клиент подключается к арендатору, в котором размещается подписка CSP.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Клиент подключается к подписке. Это применимо *только* в том случае, если у пользователя есть разрешения на назначение роли для нескольких подписок в арендаторе.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Затем клиент создает назначение роли.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Вместо предоставления разрешений владельца в области действия подписки можно предоставить разрешения на уровне группы ресурсов или ресурса. 

- На уровне группы ресурсов

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- На уровне ресурса

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Если описанные выше действия не получается выполнить или при попытке их выполнения возникают ошибки, попробуйте выполнить следующую "универсальную" процедуру, чтобы восстановить права администратора для вашего клиента.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Устранение неполадок

Если клиенту не удается выполнить шаг 6 выше, попросите клиента выполнить следующую команду:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Передайте полученный файл `newRoleAssignment.log` в корпорацию Майкрософт для дальнейшего анализа.

Если при выполнении "универсальной" процедуры возникает ошибка во время `Import-Module`, выполните следующие действия:
- Если импорт завершается сбоем из-за того, что модуль используется, перезапустите сеанс PowerShell, закрыв и повторно открыв все окна.
- Проверьте версию `Az.Resources` с помощью `Get-Module Az.Resources -ListAvailable`.
- Если версия 4.1.1 не входит в список доступных, необходимо использовать `Update-Module Az.Resources -Force`.
- Если в сообщении об ошибке указано, что необходимо использовать конкретную версию `Az.Accounts`, также обновите этот модуль, заменив `Az.Resources` на `Az.Accounts`. После этого необходимо перезапустить сеанс PowerShell.


## <a name="next-steps"></a>Дальнейшие действия

- [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md)
