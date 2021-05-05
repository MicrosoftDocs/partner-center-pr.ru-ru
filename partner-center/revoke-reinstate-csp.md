---
title: Возобновление использования привилегий администратора для Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как помочь клиентам возобновить использования привилегий администратора партнера, чтобы партнер мог помочь в управлении клиентскими подписками Azure CSP.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018193"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Возобновление использования привилегий администратора для клиентских подписок Azure CSP  

**Соответствующие роли**

- Глобальный администратор
- Агент по администрированию

Клиенты часто ожидают, что так как вы являетесь партнером CSP, то вы будете управлять использованием ресурсов Azure и их системами. Для этого требуются привилегии администратора. Одни привилегии предоставляются при установлении отношений торгового посредничества между вами и клиентом. Другие привилегии предоставляются вашим клиентом.

## <a name="admin-privileges-for-azure-in-csp"></a>Привилегии администратора для Azure в CSP

Существуют два уровня привилегий администратора для Azure в CSP.

**Привилегии администратора уровня клиента** (**делегированные привилегии**). Партнеры CSP получают эти привилегии при установлении отношений торгового посредника CSP с клиентами. Делегированные привилегии администратора обеспечивают партнерам CSP доступ к арендаторам своих клиентов, что позволяет выполнять административные функции, такие как добавление пользователей и управление ими, а также сброс паролей и управление лицензиями пользователей.

**Привилегии администратора уровня подписки**. Партнеры CSP получают эти привилегии при создании подписок Azure в CSP для своих клиентов. Такие привилегии обеспечивают партнерам в рамках CSP полный доступ к данным подпискам, что позволяет им подготавливать ресурсы Azure и управлять ими.

## <a name="reinstate-csp-partners-admin-privileges"></a>Возобновление использования привилегий администратора для партнеров CSP

Клиент может повторно создать назначение роли CSP, если вы предоставите ему идентификатор объекта группы AdminAgents. Чтобы повторно получить делегированные привилегии администратора, необходимо обратиться к своему клиенту.

1. Войдите на Панель мониторинга Центра партнеров и в меню Центра партнеров выберите элемент **Клиенты**.

2. Выберите клиента, с которым вы работаете, и **запросите установление отношений, в которых вы выполняете роль торгового посредника**. В результате создается ссылка на клиента, у которого есть привилегии администратора арендатора.

3. Этому клиенту следует выбрать ссылку и утвердить запрос на установление отношений, в которых вы выполняете роль торгового посредника.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Пример сообщения электронной почты о создании отношений торгового посредничества":::

4. Чтобы получить идентификатор объекта группы AdminAgents, вам (как партнеру) необходимо подключиться к арендатору партнера.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Клиент с ролью **владельца или администратора доступа пользователей** и разрешением на создание назначения ролей на уровне подписки, выполняет следующие действия:


    1. Подключение к арендатору, где существует подписка CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Подключение к подписке (применимо, только если у пользователя есть разрешения на назначение роли для нескольких подписок в арендаторе).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "Идентификатор подписки CSP"`


    3. Создание назначения роли.
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Если нужно предоставить разрешение роли владельца на уровне группы ресурсов или ресурса, а не области подписки, можно использовать следующие команды:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Дальнейшие действия

- [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md)
