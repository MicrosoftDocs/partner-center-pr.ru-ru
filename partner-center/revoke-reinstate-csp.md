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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="85ccd-103">Возобновление использования привилегий администратора для клиентских подписок Azure CSP</span><span class="sxs-lookup"><span data-stu-id="85ccd-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="85ccd-104">**Соответствующие роли:** глобальный администратор | агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="85ccd-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="85ccd-105">Клиенты часто ожидают, что будучи поставщиком облачных решений (CSP) вы будете управлять использованием ресурсов Azure клиентов и системами клиентов.</span><span class="sxs-lookup"><span data-stu-id="85ccd-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="85ccd-106">У вас должны быть привилегии администратора для выполнения этих действий.</span><span class="sxs-lookup"><span data-stu-id="85ccd-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="85ccd-107">Одни привилегии предоставляются при установлении отношений торгового посредничества между вами и клиентом.</span><span class="sxs-lookup"><span data-stu-id="85ccd-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="85ccd-108">Другие привилегии предоставляются вашим клиентом.</span><span class="sxs-lookup"><span data-stu-id="85ccd-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="85ccd-109">Привилегии администратора для Azure в CSP</span><span class="sxs-lookup"><span data-stu-id="85ccd-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="85ccd-110">Существуют два уровня привилегий администратора для Azure в CSP.</span><span class="sxs-lookup"><span data-stu-id="85ccd-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="85ccd-111">**Привилегии администратора уровня арендатора (делегированные привилегии)** . Партнеры CSP получают эти привилегии при установлении отношений торгового посредника CSP с клиентами.</span><span class="sxs-lookup"><span data-stu-id="85ccd-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="85ccd-112">Делегированные привилегии администратора предоставляют партнерам CSP доступ к арендаторам клиентов.</span><span class="sxs-lookup"><span data-stu-id="85ccd-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="85ccd-113">Этот доступ позволяет им выполнять административные задачи, такие как добавление пользователей и управление ими, сброс паролей и управление лицензиями пользователей.</span><span class="sxs-lookup"><span data-stu-id="85ccd-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="85ccd-114">**Привилегии администратора уровня подписки**. Партнеры CSP получают эти привилегии при создании подписок Azure в CSP для своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="85ccd-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="85ccd-115">Такие привилегии обеспечивают партнерам в рамках CSP полный доступ к данным подпискам, что позволяет им подготавливать ресурсы Azure и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="85ccd-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="85ccd-116">Возобновление использования привилегий администратора для партнеров CSP</span><span class="sxs-lookup"><span data-stu-id="85ccd-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="85ccd-117">Клиент может повторно создать назначение роли CSP, если вы предоставите ему `object ID` группы AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="85ccd-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="85ccd-118">Чтобы повторно получить делегированные привилегии администратора, необходимо выполнить следующие действия совместно с клиентом.</span><span class="sxs-lookup"><span data-stu-id="85ccd-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="85ccd-119">Войдите на панель мониторинга Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="85ccd-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="85ccd-120">В меню Центра партнеров выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="85ccd-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="85ccd-121">Выберите клиента, с которым вы работаете, и **запросите установление отношений, в которых вы выполняете роль торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="85ccd-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="85ccd-122">В результате создается ссылка на клиента, у которого есть привилегии администратора арендатора.</span><span class="sxs-lookup"><span data-stu-id="85ccd-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="85ccd-123">Клиенту следует перейти по ссылке и подтвердить запрос на установление отношений, в которых вы выполняете роль торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="85ccd-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Пример сообщения электронной почты о создании отношений торгового посредничества":::.

5. <span data-ttu-id="85ccd-125">Чтобы получить идентификатор объекта группы AdminAgents, вам (как партнеру) необходимо подключиться к арендатору партнера.</span><span class="sxs-lookup"><span data-stu-id="85ccd-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="85ccd-126">Затем клиент должен выполнить следующие действия с помощью PowerShell или Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="85ccd-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="85ccd-127">У клиента должны быть:</span><span class="sxs-lookup"><span data-stu-id="85ccd-127">Your customer must have:</span></span>

- <span data-ttu-id="85ccd-128">Роль **владельца** или **администратора доступа пользователей**.</span><span class="sxs-lookup"><span data-stu-id="85ccd-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="85ccd-129">Разрешения на создание назначений ролей на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="85ccd-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="85ccd-130">a.</span><span class="sxs-lookup"><span data-stu-id="85ccd-130">a.</span></span> <span data-ttu-id="85ccd-131">Только для PowerShell: клиент должен обновить модуль `Az.Resources`.</span><span class="sxs-lookup"><span data-stu-id="85ccd-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="85ccd-132">b.</span><span class="sxs-lookup"><span data-stu-id="85ccd-132">b.</span></span> <span data-ttu-id="85ccd-133">Клиент подключается к арендатору, в котором размещается подписка CSP.</span><span class="sxs-lookup"><span data-stu-id="85ccd-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="85ccd-134">c.</span><span class="sxs-lookup"><span data-stu-id="85ccd-134">c.</span></span> <span data-ttu-id="85ccd-135">Клиент подключается к подписке.</span><span class="sxs-lookup"><span data-stu-id="85ccd-135">The customer connects to the subscription.</span></span> <span data-ttu-id="85ccd-136">Это применимо *только* в том случае, если у пользователя есть разрешения на назначение роли для нескольких подписок в арендаторе.</span><span class="sxs-lookup"><span data-stu-id="85ccd-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="85ccd-137">d.</span><span class="sxs-lookup"><span data-stu-id="85ccd-137">d.</span></span> <span data-ttu-id="85ccd-138">Затем клиент создает назначение роли.</span><span class="sxs-lookup"><span data-stu-id="85ccd-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="85ccd-139">Вместо предоставления разрешений владельца в области действия подписки можно предоставить разрешения на уровне группы ресурсов или ресурса.</span><span class="sxs-lookup"><span data-stu-id="85ccd-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="85ccd-140">На уровне группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="85ccd-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="85ccd-141">На уровне ресурса</span><span class="sxs-lookup"><span data-stu-id="85ccd-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="85ccd-142">Если описанные выше действия не получается выполнить или при попытке их выполнения возникают ошибки, попробуйте выполнить следующую "универсальную" процедуру, чтобы восстановить права администратора для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="85ccd-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="85ccd-143">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="85ccd-143">Troubleshooting</span></span>

<span data-ttu-id="85ccd-144">Если клиенту не удается выполнить шаг 6 выше, попросите клиента выполнить следующую команду:</span><span class="sxs-lookup"><span data-stu-id="85ccd-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="85ccd-145">Передайте полученный файл `newRoleAssignment.log` в корпорацию Майкрософт для дальнейшего анализа.</span><span class="sxs-lookup"><span data-stu-id="85ccd-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="85ccd-146">Если при выполнении "универсальной" процедуры возникает ошибка во время `Import-Module`, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="85ccd-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="85ccd-147">Если импорт завершается сбоем из-за того, что модуль используется, перезапустите сеанс PowerShell, закрыв и повторно открыв все окна.</span><span class="sxs-lookup"><span data-stu-id="85ccd-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="85ccd-148">Проверьте версию `Az.Resources` с помощью `Get-Module Az.Resources -ListAvailable`.</span><span class="sxs-lookup"><span data-stu-id="85ccd-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="85ccd-149">Если версия 4.1.1 не входит в список доступных, необходимо использовать `Update-Module Az.Resources -Force`.</span><span class="sxs-lookup"><span data-stu-id="85ccd-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="85ccd-150">Если в сообщении об ошибке указано, что необходимо использовать конкретную версию `Az.Accounts`, также обновите этот модуль, заменив `Az.Resources` на `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="85ccd-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="85ccd-151">После этого необходимо перезапустить сеанс PowerShell.</span><span class="sxs-lookup"><span data-stu-id="85ccd-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="85ccd-152">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="85ccd-152">Next steps</span></span>

- [<span data-ttu-id="85ccd-153">Управление подписками и ресурсами в плане Azure</span><span class="sxs-lookup"><span data-stu-id="85ccd-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
