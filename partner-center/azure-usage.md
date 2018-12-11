---
title: Размеры виртуальных Машин Microsoft Azure для максимального использования резервирования | Центр партнеров
ms.topic: article
ms.date: 10/29/2018
Description: When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.
author: v-petand
ms.author: v-petand
keywords: azure, резервирования, виртуальная машина, управление, использование, размеры
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 04a027bf50739434f9a6d155eb8a31f4074185a7
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917546"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="568d2-103">Размеры виртуальных машин Microsoft Azure для максимального использования резервирования</span><span class="sxs-lookup"><span data-stu-id="568d2-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="568d2-104">Область применения</span><span class="sxs-lookup"><span data-stu-id="568d2-104">Applies to</span></span>**

-  <span data-ttu-id="568d2-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="568d2-105">Partner Center</span></span>
-  <span data-ttu-id="568d2-106">Портал Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-106">Azure portal</span></span>
-  <span data-ttu-id="568d2-107">Партнеры по программе CSP</span><span class="sxs-lookup"><span data-stu-id="568d2-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="568d2-108">Определение размера виртуальных машин для резервирования Azure клиента</span><span class="sxs-lookup"><span data-stu-id="568d2-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="568d2-109">При приобретении резервирований Microsoft Azure для клиентов необходимо выбрать размер виртуальной машины (VM), соответствующий требованиям клиента к вычислительной мощности.</span><span class="sxs-lookup"><span data-stu-id="568d2-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="568d2-110">Эту информацию можно получить одним из следующих способов:</span><span class="sxs-lookup"><span data-stu-id="568d2-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="568d2-111">API использования Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-111">Azure utilization API</span></span>
-   <span data-ttu-id="568d2-112">Портал Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-112">The Azure portal</span></span>
-   <span data-ttu-id="568d2-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="568d2-113">Azure PowerShell</span></span>
-   <span data-ttu-id="568d2-114">API для Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="568d2-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="568d2-115">Ниже приведены инструкции по каждому из этих методов.</span><span class="sxs-lookup"><span data-stu-id="568d2-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="568d2-116">После приобретения резервирования скидка на резервирование автоматически применяется к виртуальным машинам, которые соответствуют атрибутам и количеству резервирования.</span><span class="sxs-lookup"><span data-stu-id="568d2-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="568d2-117">Назначать резервирование виртуальной машине не требуется.</span><span class="sxs-lookup"><span data-stu-id="568d2-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="568d2-118">Скидки на резервирование не распространяются на классические и рекламные виртуальные машины.</span><span class="sxs-lookup"><span data-stu-id="568d2-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="568d2-119">Чтобы правильно определить тип и размер виртуальной машины, приобретаемой от лица клиента, воспользуйтесь одним из указанных методов. Помните, что тип серии виртуальной машины неправильно отображается в файлах выверки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="568d2-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="568d2-120">Получение сведений о размере виртуальной машины с помощью API использования Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="568d2-121">Используйте значение атрибута ServiceType из additionalInfo в ответе API, чтобы определить нужный размер виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="568d2-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="568d2-122">Дополнительные сведения см. в разделе [Получение статистики использования Azure для клиента](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) в документе [API Центра партнеров](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="568d2-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="568d2-123">Получение сведений о размере виртуальной машины на портале Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="568d2-124">В центре партнеров перейдите к странице " **Клиенты** ".</span><span class="sxs-lookup"><span data-stu-id="568d2-124">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="568d2-125">Найдите клиента, желающего приобрести резервирования Azure, затем выберите стрелку вниз, чтобы посмотреть сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="568d2-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="568d2-126">Выберите **Портал управления Microsoft Azure**, чтобы открыть запись клиента на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="568d2-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="568d2-127">Выберите пункт **Виртуальные машины** в меню портала, затем выберите виртуальную машину, для которой требуется приобрести резервирование.</span><span class="sxs-lookup"><span data-stu-id="568d2-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="568d2-128">На странице сведений о виртуальной машине найдите информацию о размере и регионе (см. рисунок ниже) и используйте эту информацию для приобретения резервирования в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="568d2-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Сведения о размере и регионе на странице сведений о](images/usage1.png)

**<span data-ttu-id="568d2-130">Получение сведений о размере виртуальной машины с помощью Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="568d2-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="568d2-131">Чтобы определить местоположение и размер виртуальной машины, для которой нужно приобрести резервирование, используйте данные, показанные на рисунке ниже.</span><span class="sxs-lookup"><span data-stu-id="568d2-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![Виртуальная машина расположение и размер](images/usage2.png)

**<span data-ttu-id="568d2-133">Получение сведений о размере виртуальной машины с помощью API для Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="568d2-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="568d2-134">С помощью ARMClient или API-интерфейсов ARM вызовите клиент ARM для виртуальной машины, для которой требуется приобрести резервирование.</span><span class="sxs-lookup"><span data-stu-id="568d2-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="568d2-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="568d2-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="568d2-136">Вызов возвращает значения для параметров **vmSize** и **location**, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="568d2-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="568d2-137">![значение vmSize](images/usage3.png)
    ![значение расположения](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="568d2-137">![vmSize value](images/usage3.png)
![location value](images/usage4.png)</span></span>
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="568d2-138">Проверка использования виртуальной машины Azure и скидки на резервирование</span><span class="sxs-lookup"><span data-stu-id="568d2-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="568d2-139">После приобретения Azure Reserved VM Instance от имени клиента скидка на предоплату пространства на виртуальной машине автоматически применяется к виртуальным машинам, которые соответствуют атрибутам и количеству резервирования клиента.</span><span class="sxs-lookup"><span data-stu-id="568d2-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="568d2-140">Вы можете проверить использование резервирования клиента и посмотреть, к каким виртуальным машинам применены скидки на резервирование. Это можно сделать следующими способами:</span><span class="sxs-lookup"><span data-stu-id="568d2-140">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="568d2-141">Портал Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-141">The Azure portal</span></span>
-   <span data-ttu-id="568d2-142">API использования Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-142">Azure utilization API</span></span>

<span data-ttu-id="568d2-143">Ниже приведены инструкции по каждому из этих методов.</span><span class="sxs-lookup"><span data-stu-id="568d2-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="568d2-144">Только API использования Azure показывает, к какой виртуальной машине применяется скидка.</span><span class="sxs-lookup"><span data-stu-id="568d2-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="568d2-145">Проверка использования резервирования клиента на портале Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-145">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="568d2-146">В центре партнеров перейдите к странице " **Клиенты** ".</span><span class="sxs-lookup"><span data-stu-id="568d2-146">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="568d2-147">Найдите клиента, для которого необходимо проверить использование резервирования и скидку, затем выберите стрелку вниз, чтобы посмотреть сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="568d2-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="568d2-148">Выберите **Портал управления Microsoft Azure**, чтобы открыть запись клиента на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="568d2-148">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="568d2-149">Выберите пункт **Резервирования** в меню портала, затем выберите резервирование, чтобы проверить его использование.</span><span class="sxs-lookup"><span data-stu-id="568d2-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="568d2-150">На странице **Обзор** отображается график использования резервирования, который показывает, какой объем резервирования применен к виртуальным машинам.</span><span class="sxs-lookup"><span data-stu-id="568d2-150">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="568d2-151">Данные об использовании могут отображаться с задержкой до 8 часов.</span><span class="sxs-lookup"><span data-stu-id="568d2-151">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="568d2-152">а.</span><span class="sxs-lookup"><span data-stu-id="568d2-152">a.</span></span>  <span data-ttu-id="568d2-153">Если резервирование используется на 100%, клиент получает максимально возможную экономию, которую может обеспечить приобретенное резервирование.</span><span class="sxs-lookup"><span data-stu-id="568d2-153">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="568d2-154">б.</span><span class="sxs-lookup"><span data-stu-id="568d2-154">b.</span></span>  <span data-ttu-id="568d2-155">Если использование резервирования составляет 0%, скидка не применяется ни к одной виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="568d2-155">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="568d2-156">в.</span><span class="sxs-lookup"><span data-stu-id="568d2-156">c.</span></span>  <span data-ttu-id="568d2-157">Если использование резервирования составляет от 1% до 99%, у клиента есть неиспользуемые преимущества.</span><span class="sxs-lookup"><span data-stu-id="568d2-157">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="568d2-158">Во избежание подобных ситуаций перед покупкой необходимо правильно определить размер виртуальной машины в соответствии с требованиями клиента к вычислительной мощности.</span><span class="sxs-lookup"><span data-stu-id="568d2-158">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="568d2-159">Проверка использования резервирования клиента с помощью API использования Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-159">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="568d2-160">Только API использования Azure показывает, к какой виртуальной машине применяется скидка.</span><span class="sxs-lookup"><span data-stu-id="568d2-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="568d2-161">Вы можете получить данные об использовании резервирования с помощью API использования Azure. Так можно проверить, получает ли клиент скидку за резервирование, и посмотреть, к каким виртуальным машинам применяется эта скидка.</span><span class="sxs-lookup"><span data-stu-id="568d2-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="568d2-162">Сравните проверку использования резервирования в примерах А и Б.</span><span class="sxs-lookup"><span data-stu-id="568d2-162">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![Примеры использования резервирования](images\usage5.png)

-   <span data-ttu-id="568d2-164">Идентификатор reservationId определяет резервирование Azure, которое использовалось для применения скидки к виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="568d2-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="568d2-165">consumptionMeter — это MeterId для виртуальной машины, к которой применена скидка за резервирование.</span><span class="sxs-lookup"><span data-stu-id="568d2-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="568d2-166">ReservationMeter отображает стоимость $0, так как применена скидка за резервирование.</span><span class="sxs-lookup"><span data-stu-id="568d2-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="568d2-167">Дополнительные сведения см. в разделе [Получение статистики использования Azure для клиента](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) в документе [API Центра партнеров](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="568d2-167">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="568d2-168">Стоимость программного обеспечения, например Microsoft Windows Server, в настоящее время не входит в цену резервирования виртуальных машин и отображается в отдельных строках заказа и счета.</span><span class="sxs-lookup"><span data-stu-id="568d2-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="568d2-169">Тем не менее, если у клиента есть преимущества гибридного использования Azure, стоимость программного обеспечения не учитывается.</span><span class="sxs-lookup"><span data-stu-id="568d2-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="568d2-170">Дополнительные сведения см. в разделе [Затраты на программное обеспечение Windows, не включенные в зарезервированные экземпляры](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="568d2-170">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="568d2-171">Ресурсы о резервированиях Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-171">Azure reservations resources</span></span>
|**<span data-ttu-id="568d2-172">Для получения информации о</span><span class="sxs-lookup"><span data-stu-id="568d2-172">For information about</span></span>**   |**<span data-ttu-id="568d2-173">Прочтите этот документ</span><span class="sxs-lookup"><span data-stu-id="568d2-173">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="568d2-174">Обзор резервирований Azure в программе CSP</span><span class="sxs-lookup"><span data-stu-id="568d2-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="568d2-175">Продажа Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="568d2-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="568d2-176">Приобретение резервирований Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="568d2-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="568d2-177">Приобретение резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="568d2-178">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="568d2-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="568d2-179">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="568d2-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="568d2-180">Приобретение резервирований Azure на портале Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="568d2-181">[Предоплата за виртуальные машины с Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) в справке Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-181">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="568d2-182">Управление резервированиями Azure на портале Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-182">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="568d2-183">[Управление зарезервированными экземплярами виртуальных машин](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) в справке Azure</span><span class="sxs-lookup"><span data-stu-id="568d2-183">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="568d2-184">Приобретение резервирований Azure с помощью API Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="568d2-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="568d2-185">[Приобретение услуги Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="568d2-185">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



