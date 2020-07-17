---
title: Размеры виртуальных машин Azure для максимального использования резервирования
ms.topic: article
ms.date: 07/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Узнайте, как масштабировать виртуальную машину с учетом потребностей клиентов при покупке Microsoft Azure резервирования для них.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 706021c39e136954d3791856da12c828cbdf6389
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435743"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="716ba-103">Размеры виртуальных машин Microsoft Azure для максимального использования резервирования</span><span class="sxs-lookup"><span data-stu-id="716ba-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="716ba-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="716ba-104">**Applies to**</span></span>

- <span data-ttu-id="716ba-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="716ba-105">Partner Center</span></span>
- <span data-ttu-id="716ba-106">Портал Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-106">Azure portal</span></span>
- <span data-ttu-id="716ba-107">Партнеры по программе CSP</span><span class="sxs-lookup"><span data-stu-id="716ba-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="716ba-108">Определение размера виртуальной машины для резервирования Azure клиента</span><span class="sxs-lookup"><span data-stu-id="716ba-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="716ba-109">При покупке Microsoft Azure резервирования от имени ваших клиентов необходимо выбрать размер виртуальной машины, чтобы удовлетворить потребности клиента.</span><span class="sxs-lookup"><span data-stu-id="716ba-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="716ba-110">Эту информацию можно получить одним из следующих способов:</span><span class="sxs-lookup"><span data-stu-id="716ba-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="716ba-111">API использования Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-111">Azure utilization API</span></span>
- <span data-ttu-id="716ba-112">Портал Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-112">The Azure portal</span></span>
- <span data-ttu-id="716ba-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="716ba-113">Azure PowerShell</span></span>
- <span data-ttu-id="716ba-114">API для Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="716ba-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="716ba-115">Ниже приведены инструкции по каждому из этих методов.</span><span class="sxs-lookup"><span data-stu-id="716ba-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="716ba-116">После приобретения резервирования скидка на резервирование автоматически применяется к виртуальным машинам, которые соответствуют атрибутам и количеству резервирования.</span><span class="sxs-lookup"><span data-stu-id="716ba-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="716ba-117">Вам не нужно назначать резервирование виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="716ba-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="716ba-118">Скидки на резервирование не применяются к классическим или рекламным виртуальным машинам.</span><span class="sxs-lookup"><span data-stu-id="716ba-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="716ba-119">Чтобы правильно определить тип и размер виртуальной машины, приобретаемой от лица клиента, воспользуйтесь одним из указанных методов. Помните, что тип серии виртуальной машины неправильно отображается в файлах выверки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="716ba-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="716ba-120">Получение сведений о размере виртуальной машины с помощью API использования Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="716ba-121">Используйте значение атрибута ServiceType из additionalInfo в ответе API, чтобы определить нужный размер виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="716ba-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="716ba-122">Дополнительные сведения см. в статье [получение записей об использовании клиента для Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) в [API центра партнеров](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="716ba-122">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="716ba-123">Получение сведений о размере виртуальной машины на портале Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="716ba-124">В центре партнеров перейдите на страницу **Клиенты** .</span><span class="sxs-lookup"><span data-stu-id="716ba-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="716ba-125">Найдите клиента, желающего купить резервирования виртуальных машин Azure, а затем щелкните стрелку вниз, чтобы развернуть сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="716ba-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="716ba-126">Выберите **портал управления Microsoft Azure** , чтобы открыть запись клиента в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="716ba-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="716ba-127">Выберите пункт **Виртуальные машины** в меню портала, затем выберите виртуальную машину, для которой требуется приобрести резервирование.</span><span class="sxs-lookup"><span data-stu-id="716ba-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="716ba-128">На странице сведения о виртуальной машине найдите сведения о размере и регионе, как показано ниже, и используйте эти сведения для приобретения резервирования в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="716ba-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Сведения о размере и регионе на странице сведений":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="716ba-130">Получение сведений о размере виртуальной машины с помощью Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="716ba-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="716ba-131">Чтобы определить местоположение и размер виртуальной машины, для которой нужно приобрести резервирование, используйте данные, показанные на рисунке ниже.</span><span class="sxs-lookup"><span data-stu-id="716ba-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Расположение и размер виртуальной машины":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="716ba-133">Получение сведений о размере виртуальной машины с помощью API для Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="716ba-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="716ba-134">С помощью ARMClient или API-интерфейсов ARM вызовите клиент ARM для виртуальной машины, для которой требуется приобрести резервирование.</span><span class="sxs-lookup"><span data-stu-id="716ba-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="716ba-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="716ba-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="716ba-136">Вызов возвращает значения для параметров **vmSize** и **location**, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="716ba-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="значение vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="значение расположения":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="716ba-139">Проверка использования виртуальной машины Azure и скидки на резервирование</span><span class="sxs-lookup"><span data-stu-id="716ba-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="716ba-140">После приобретения зарезервированного экземпляра виртуальной машины Azure от имени клиента автоматически применяется скидка за период оплаты для виртуальной машины, которая соответствует атрибутам и количеству резервирования клиента.</span><span class="sxs-lookup"><span data-stu-id="716ba-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="716ba-141">Вы можете проверить использование резервирования клиента и узнать, к каким виртуальным машинам применяются скидки на резервирование, одним из следующих способов:</span><span class="sxs-lookup"><span data-stu-id="716ba-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="716ba-142">Портал Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-142">The Azure portal</span></span>
- <span data-ttu-id="716ba-143">API использования Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-143">Azure utilization API</span></span>

<span data-ttu-id="716ba-144">Ниже приведены инструкции по каждому из этих методов.</span><span class="sxs-lookup"><span data-stu-id="716ba-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="716ba-145">Только API использования Azure показывает, к какой виртуальной машине применяется скидка.</span><span class="sxs-lookup"><span data-stu-id="716ba-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="716ba-146">Проверьте использование резервирования клиента в портал Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="716ba-147">В центре партнеров перейдите на страницу **Клиенты** .</span><span class="sxs-lookup"><span data-stu-id="716ba-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="716ba-148">Найдите клиента, для которого требуется проверить скидку резервирования и использование, а затем щелкните стрелку вниз, чтобы развернуть сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="716ba-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="716ba-149">Выберите **портал управления Microsoft Azure** , чтобы открыть запись клиента в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="716ba-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="716ba-150">Выберите пункт **Резервирования** в меню портала, затем выберите резервирование, чтобы проверить его использование.</span><span class="sxs-lookup"><span data-stu-id="716ba-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="716ba-151">На странице **Обзор** проверьте график использования резервирования, который показывает, какая часть резервирования была применена к виртуальным машинам.</span><span class="sxs-lookup"><span data-stu-id="716ba-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="716ba-152">Данные об использовании могут отображаться с задержкой до 8 часов.</span><span class="sxs-lookup"><span data-stu-id="716ba-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="716ba-153">a.</span><span class="sxs-lookup"><span data-stu-id="716ba-153">a.</span></span> <span data-ttu-id="716ba-154">Если использование резервирования составляет 100%, клиент получает все возможные сокращения, которые может предоставить Покупка резервирования.</span><span class="sxs-lookup"><span data-stu-id="716ba-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="716ba-155">b.</span><span class="sxs-lookup"><span data-stu-id="716ba-155">b.</span></span> <span data-ttu-id="716ba-156">Если использование резервирования составляет 0%, скидка не применяется ни к одной виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="716ba-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="716ba-157">c.</span><span class="sxs-lookup"><span data-stu-id="716ba-157">c.</span></span> <span data-ttu-id="716ba-158">Если использование резервирования составляет от 1% до 99%, то используются неиспользуемые преимущества.</span><span class="sxs-lookup"><span data-stu-id="716ba-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="716ba-159">Чтобы избежать такой ситуации, определите требуемый размер виртуальной машины, чтобы обеспечить поддержку вычислительных потребностей клиента перед покупкой.</span><span class="sxs-lookup"><span data-stu-id="716ba-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="716ba-160">Проверка использования резервирования клиентом с помощью API использования Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="716ba-161">Только API использования Azure показывает, к какой виртуальной машине применяется скидка.</span><span class="sxs-lookup"><span data-stu-id="716ba-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="716ba-162">Вы можете получить данные об использовании резервирования с помощью API использования Azure. Так можно проверить, получает ли клиент скидку за резервирование, и посмотреть, к каким виртуальным машинам применяется эта скидка.</span><span class="sxs-lookup"><span data-stu-id="716ba-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="716ba-163">Сравните пример а с примером б, чтобы узнать, как проверить использование резервирования клиентом.</span><span class="sxs-lookup"><span data-stu-id="716ba-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Примеры использования резервирования":::

- <span data-ttu-id="716ba-165">Идентификатор reservationId определяет резервирование Azure, которое использовалось для применения скидки к виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="716ba-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="716ba-166">consumptionMeter — это MeterId для виртуальной машины, к которой применена скидка за резервирование.</span><span class="sxs-lookup"><span data-stu-id="716ba-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="716ba-167">ReservationMeter отображает стоимость $0, так как применена скидка за резервирование.</span><span class="sxs-lookup"><span data-stu-id="716ba-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="716ba-168">Дополнительные сведения см. в статье [получение записей об использовании клиента для Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) в [API центра партнеров](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="716ba-168">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="716ba-169">Стоимость программного обеспечения, например Microsoft Windows Server, в настоящее время не входит в цену резервирования виртуальных машин и отображается в отдельных строках заказа и счета.</span><span class="sxs-lookup"><span data-stu-id="716ba-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="716ba-170">Тем не менее, если у клиента есть преимущества гибридного использования Azure, стоимость программного обеспечения не учитывается.</span><span class="sxs-lookup"><span data-stu-id="716ba-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="716ba-171">Дополнительные сведения см. в разделе [Затраты на программное обеспечение Windows, не включенные в зарезервированные экземпляры](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="716ba-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="716ba-172">Ресурсы о резервированиях Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-172">Azure reservations resources</span></span>

|<span data-ttu-id="716ba-173">**Сведения о**</span><span class="sxs-lookup"><span data-stu-id="716ba-173">**For information about**</span></span>   |<span data-ttu-id="716ba-174">**Прочитайте это**</span><span class="sxs-lookup"><span data-stu-id="716ba-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="716ba-175">Обзор резервирований Azure в программе CSP</span><span class="sxs-lookup"><span data-stu-id="716ba-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="716ba-176">Продажа Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="716ba-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="716ba-177">Приобретение резервирований Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="716ba-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="716ba-178">Приобретение резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="716ba-179">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="716ba-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="716ba-180">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="716ba-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="716ba-181">Приобретение резервирований Azure на портале Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="716ba-182">[Предоплата за виртуальные машины с Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) в справке Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="716ba-183">Управление резервированиями Azure на портале Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="716ba-184">[Управление зарезервированными экземплярами виртуальных машин](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) в справке Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="716ba-185">Приобретение резервирований Azure с помощью API Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="716ba-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="716ba-186">[Приобретение услуги Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="716ba-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="716ba-187">Предоставление клиентам разрешения на приобретение собственных резервирований Azure из подписки, приобретенной для них.</span><span class="sxs-lookup"><span data-stu-id="716ba-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="716ba-188">Предоставление клиентам разрешения на приобретение собственных резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="716ba-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
