---
title: Краткое руководство. управление частными Azure Marketplace с помощью PowerShell
description: В этом кратком руководстве показано, как управлять предложениями в частном магазине Azure Marketplace с помощью Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412460"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="029b0-103">Краткое руководство. управление частными Azure Marketplace с помощью PowerShell</span><span class="sxs-lookup"><span data-stu-id="029b0-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="029b0-104">В этой статье описывается, как можно управлять предложениями в частном магазине Azure Marketplace с помощью модуля PowerShell [AZ. Marketplace](/powershell/module/az.marketplace) .</span><span class="sxs-lookup"><span data-stu-id="029b0-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="029b0-105">В настоящее время частная версия Azure Marketplace доступна в общедоступной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="029b0-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="029b0-106">Эта предварительная версия предоставляется без соглашения об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="029b0-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="029b0-107">Эта версия не рекомендуется для использования с рабочими нагрузками в производственной среде.</span><span class="sxs-lookup"><span data-stu-id="029b0-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="029b0-108">Некоторые функции могут не поддерживаться или иметь ограниченные возможности.</span><span class="sxs-lookup"><span data-stu-id="029b0-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="029b0-109">Дополнительные сведения см. в статье [Дополнительные условия использования предварительных выпусков Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="029b0-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="029b0-110">Требования</span><span class="sxs-lookup"><span data-stu-id="029b0-110">Requirements</span></span>

* <span data-ttu-id="029b0-111">Если у вас еще нет подписки Azure, создайте [бесплатную](https://azure.microsoft.com/free/) учетную запись Azure, прежде чем начинать работу.</span><span class="sxs-lookup"><span data-stu-id="029b0-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="029b0-112">Если вы используете Azure PowerShell локально:</span><span class="sxs-lookup"><span data-stu-id="029b0-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="029b0-113">[Установите модуль Az PowerShell.](/powershell/azure/install-az-ps)</span><span class="sxs-lookup"><span data-stu-id="029b0-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="029b0-114">Подключитесь к учетной записи Azure с помощью командлета [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="029b0-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="029b0-115">Если вы используете Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="029b0-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="029b0-116">Дополнительные сведения см. в статье [Общие сведения об Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="029b0-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="029b0-117">Пока модуль PowerShell **AZ. Marketplace** находится на этапе предварительной версии, его необходимо установить отдельно с помощью `Install-Module` командлета.</span><span class="sxs-lookup"><span data-stu-id="029b0-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="029b0-118">Как только этот модуль PowerShell станет общедоступным, он будет включен в один из будущих выпусков модуля Az PowerShell и по умолчанию встроен в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="029b0-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="029b0-119">Если вы используете несколько подписок Azure, выберите ту, за ресурсы в которой будут выставляться счета.</span><span class="sxs-lookup"><span data-stu-id="029b0-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="029b0-120">Выберите требуемую подписку с помощью командлета [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="029b0-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="029b0-121">Список частных магазинов</span><span class="sxs-lookup"><span data-stu-id="029b0-121">List private stores</span></span>

<span data-ttu-id="029b0-122">Чтобы получить список частных хранилищ, используйте командлет [Get-азмаркетплацеприватесторе](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="029b0-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="029b0-123">В следующем примере перечисляются частные хранилища, созданные в области клиента.</span><span class="sxs-lookup"><span data-stu-id="029b0-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="029b0-124">Добавление предложения в частный Marketplace</span><span class="sxs-lookup"><span data-stu-id="029b0-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="029b0-125">Чтобы добавить предложение в частное хранилище, используйте командлет [Set-азмаркетплацеприватестореоффер](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="029b0-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="029b0-126">В следующем примере указанное предложение добавляется в частный Marketplace для частного хранилища, созданного в области клиента.</span><span class="sxs-lookup"><span data-stu-id="029b0-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="029b0-127">Получение предложений частного магазина</span><span class="sxs-lookup"><span data-stu-id="029b0-127">Get private store offers</span></span>

<span data-ttu-id="029b0-128">Чтобы получить одно или несколько предложений частного хранилища, используйте командлет [Get-азмаркетплацеприватестореоффер](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="029b0-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="029b0-129">В следующем примере возвращаются предложения, связанные с указанным частным хранилищем, которые были добавлены в область клиента.</span><span class="sxs-lookup"><span data-stu-id="029b0-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="029b0-130">Удаление предложения</span><span class="sxs-lookup"><span data-stu-id="029b0-130">Remove an offer</span></span>

<span data-ttu-id="029b0-131">Чтобы удалить предложение из частного хранилища, используйте командлет [Remove-азмаркетплацеприватестореоффер](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="029b0-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="029b0-132">В следующем примере предложение удаляется из частного хранилища, созданного в области клиента.</span><span class="sxs-lookup"><span data-stu-id="029b0-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="029b0-133">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="029b0-133">Next steps</span></span>

<span data-ttu-id="029b0-134">[Создание частного магазина Azure Marketplace и управление им](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="029b0-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>