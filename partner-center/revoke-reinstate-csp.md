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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="311b4-103">Возобновление использования привилегий администратора для клиентских подписок Azure CSP</span><span class="sxs-lookup"><span data-stu-id="311b4-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="311b4-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="311b4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="311b4-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="311b4-105">Global admin</span></span>
- <span data-ttu-id="311b4-106">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="311b4-106">Admin agent</span></span>

<span data-ttu-id="311b4-107">Клиенты часто ожидают, что так как вы являетесь партнером CSP, то вы будете управлять использованием ресурсов Azure и их системами.</span><span class="sxs-lookup"><span data-stu-id="311b4-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="311b4-108">Для этого требуются привилегии администратора.</span><span class="sxs-lookup"><span data-stu-id="311b4-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="311b4-109">Одни привилегии предоставляются при установлении отношений торгового посредничества между вами и клиентом.</span><span class="sxs-lookup"><span data-stu-id="311b4-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="311b4-110">Другие привилегии предоставляются вашим клиентом.</span><span class="sxs-lookup"><span data-stu-id="311b4-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="311b4-111">Привилегии администратора для Azure в CSP</span><span class="sxs-lookup"><span data-stu-id="311b4-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="311b4-112">Существуют два уровня привилегий администратора для Azure в CSP.</span><span class="sxs-lookup"><span data-stu-id="311b4-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="311b4-113">**Привилегии администратора уровня клиента** (**делегированные привилегии**). Партнеры CSP получают эти привилегии при установлении отношений торгового посредника CSP с клиентами.</span><span class="sxs-lookup"><span data-stu-id="311b4-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="311b4-114">Делегированные привилегии администратора обеспечивают партнерам CSP доступ к арендаторам своих клиентов, что позволяет выполнять административные функции, такие как добавление пользователей и управление ими, а также сброс паролей и управление лицензиями пользователей.</span><span class="sxs-lookup"><span data-stu-id="311b4-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="311b4-115">**Привилегии администратора уровня подписки**. Партнеры CSP получают эти привилегии при создании подписок Azure в CSP для своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="311b4-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="311b4-116">Такие привилегии обеспечивают партнерам в рамках CSP полный доступ к данным подпискам, что позволяет им подготавливать ресурсы Azure и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="311b4-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="311b4-117">Возобновление использования привилегий администратора для партнеров CSP</span><span class="sxs-lookup"><span data-stu-id="311b4-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="311b4-118">Клиент может повторно создать назначение роли CSP, если вы предоставите ему идентификатор объекта группы AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="311b4-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="311b4-119">Чтобы повторно получить делегированные привилегии администратора, необходимо обратиться к своему клиенту.</span><span class="sxs-lookup"><span data-stu-id="311b4-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="311b4-120">Войдите на Панель мониторинга Центра партнеров и в меню Центра партнеров выберите элемент **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="311b4-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="311b4-121">Выберите клиента, с которым вы работаете, и **запросите установление отношений, в которых вы выполняете роль торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="311b4-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="311b4-122">В результате создается ссылка на клиента, у которого есть привилегии администратора арендатора.</span><span class="sxs-lookup"><span data-stu-id="311b4-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="311b4-123">Этому клиенту следует выбрать ссылку и утвердить запрос на установление отношений, в которых вы выполняете роль торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="311b4-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Пример сообщения электронной почты о создании отношений торгового посредничества":::

4. <span data-ttu-id="311b4-125">Чтобы получить идентификатор объекта группы AdminAgents, вам (как партнеру) необходимо подключиться к арендатору партнера.</span><span class="sxs-lookup"><span data-stu-id="311b4-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="311b4-126">Клиент с ролью **владельца или администратора доступа пользователей** и разрешением на создание назначения ролей на уровне подписки, выполняет следующие действия:</span><span class="sxs-lookup"><span data-stu-id="311b4-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="311b4-127">Подключение к арендатору, где существует подписка CSP.</span><span class="sxs-lookup"><span data-stu-id="311b4-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="311b4-128">Подключение к подписке (применимо, только если у пользователя есть разрешения на назначение роли для нескольких подписок в арендаторе).</span><span class="sxs-lookup"><span data-stu-id="311b4-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="311b4-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "Идентификатор подписки CSP"\`</span><span class="sxs-lookup"><span data-stu-id="311b4-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="311b4-130">Создание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="311b4-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="311b4-131">Если нужно предоставить разрешение роли владельца на уровне группы ресурсов или ресурса, а не области подписки, можно использовать следующие команды:</span><span class="sxs-lookup"><span data-stu-id="311b4-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="311b4-132">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="311b4-132">Next steps</span></span>

- [<span data-ttu-id="311b4-133">Управление подписками и ресурсами в плане Azure</span><span class="sxs-lookup"><span data-stu-id="311b4-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
