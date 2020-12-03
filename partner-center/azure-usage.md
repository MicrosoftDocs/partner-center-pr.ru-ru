---
title: Размеры виртуальных машин Azure для максимального использования резервирования
description: Узнайте, как масштабировать виртуальную машину с учетом потребностей клиентов при покупке Microsoft Azure резервирования для них.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 226ebd27b4ca4cdef56ce833a58a10bed89f8056
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534953"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="b2a69-103">Размеры виртуальных машин Microsoft Azure для максимального использования резервирования</span><span class="sxs-lookup"><span data-stu-id="b2a69-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="b2a69-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="b2a69-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b2a69-105">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="b2a69-105">Admin agent</span></span>
- <span data-ttu-id="b2a69-106">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="b2a69-106">Sales agent</span></span>

<span data-ttu-id="b2a69-107">В этой статье объясняется, как задать размер виртуальной машины (ВМ) для вычислительных потребностей клиентов при покупке Microsoft Azure резервирования для них.</span><span class="sxs-lookup"><span data-stu-id="b2a69-107">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="b2a69-108">Эта статья относится только к партнерам в программе поставщика облачных решений (CSP).</span><span class="sxs-lookup"><span data-stu-id="b2a69-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="b2a69-109">Вместо этого клиенты, использующие другие типы подписок (например, оплата по мере использования, индивидуальные соглашения с клиентами Майкрософт или подписки Соглашение Enterprise), должны читать [эту документацию по резервированию Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="b2a69-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="b2a69-110">Определение размера виртуальной машины для резервирования Azure клиента</span><span class="sxs-lookup"><span data-stu-id="b2a69-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="b2a69-111">При покупке Microsoft Azure резервирования от имени ваших клиентов необходимо выбрать размер виртуальной машины, чтобы удовлетворить потребности клиента.</span><span class="sxs-lookup"><span data-stu-id="b2a69-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="b2a69-112">Эту информацию можно получить одним из следующих способов:</span><span class="sxs-lookup"><span data-stu-id="b2a69-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="b2a69-113">API использования Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-113">Azure utilization API</span></span>
- <span data-ttu-id="b2a69-114">портал Azure;</span><span class="sxs-lookup"><span data-stu-id="b2a69-114">The Azure portal</span></span>
- <span data-ttu-id="b2a69-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b2a69-115">Azure PowerShell</span></span>
- <span data-ttu-id="b2a69-116">API для Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="b2a69-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="b2a69-117">Ниже приведены инструкции по каждому из этих методов.</span><span class="sxs-lookup"><span data-stu-id="b2a69-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="b2a69-118">После приобретения резервирования скидка на резервирование автоматически применяется к виртуальным машинам, которые соответствуют атрибутам и количеству резервирования.</span><span class="sxs-lookup"><span data-stu-id="b2a69-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="b2a69-119">Вам не нужно назначать резервирование виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="b2a69-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="b2a69-120">Скидки на резервирование не применяются к классическим или рекламным виртуальным машинам.</span><span class="sxs-lookup"><span data-stu-id="b2a69-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="b2a69-121">Чтобы правильно определить тип и размер виртуальной машины, приобретаемой от лица клиента, воспользуйтесь одним из указанных методов. Помните, что тип серии виртуальной машины неправильно отображается в файлах выверки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="b2a69-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="b2a69-122">Получение сведений о размере виртуальной машины с помощью API использования Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="b2a69-123">Используйте значение атрибута ServiceType из additionalInfo в ответе API, чтобы определить нужный размер виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="b2a69-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="b2a69-124">Дополнительные сведения см. в статье [получение записей об использовании клиента для Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) в [API центра партнеров](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="b2a69-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="b2a69-125">Получение сведений о размере виртуальной машины на портале Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="b2a69-126">В центре партнеров перейдите на страницу **Клиенты** .</span><span class="sxs-lookup"><span data-stu-id="b2a69-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="b2a69-127">Найдите клиента, желающего купить резервирования виртуальных машин Azure, а затем щелкните стрелку вниз, чтобы развернуть сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="b2a69-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="b2a69-128">Выберите **портал управления Microsoft Azure** , чтобы открыть запись клиента в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="b2a69-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="b2a69-129">Выберите пункт **Виртуальные машины** в меню портала, затем выберите виртуальную машину, для которой требуется приобрести резервирование.</span><span class="sxs-lookup"><span data-stu-id="b2a69-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="b2a69-130">На странице сведения о виртуальной машине найдите сведения о размере и регионе, как показано ниже, и используйте эти сведения для приобретения резервирования в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="b2a69-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Сведения о размере и регионе на странице сведений":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="b2a69-132">Получение сведений о размере виртуальной машины с помощью Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b2a69-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="b2a69-133">Чтобы определить местоположение и размер виртуальной машины, для которой нужно приобрести резервирование, используйте данные, показанные на рисунке ниже.</span><span class="sxs-lookup"><span data-stu-id="b2a69-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Расположение и размер виртуальной машины":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="b2a69-135">Получение сведений о размере виртуальной машины с помощью API для Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="b2a69-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="b2a69-136">С помощью ARMClient или API-интерфейсов ARM вызовите клиент ARM для виртуальной машины, для которой требуется приобрести резервирование.</span><span class="sxs-lookup"><span data-stu-id="b2a69-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="b2a69-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="b2a69-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="b2a69-138">Вызов возвращает значения для параметров **vmSize** и **location**, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="b2a69-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="значение vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="значение расположения":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="b2a69-141">Проверка использования виртуальной машины Azure и скидки на резервирование</span><span class="sxs-lookup"><span data-stu-id="b2a69-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="b2a69-142">После приобретения зарезервированного экземпляра виртуальной машины Azure от имени клиента автоматически применяется скидка за период оплаты для виртуальной машины, которая соответствует атрибутам и количеству резервирования клиента.</span><span class="sxs-lookup"><span data-stu-id="b2a69-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="b2a69-143">Вы можете проверить использование резервирования клиента и узнать, к каким виртуальным машинам применяются скидки на резервирование, одним из следующих способов:</span><span class="sxs-lookup"><span data-stu-id="b2a69-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="b2a69-144">портал Azure;</span><span class="sxs-lookup"><span data-stu-id="b2a69-144">The Azure portal</span></span>
- <span data-ttu-id="b2a69-145">API использования Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-145">Azure utilization API</span></span>

<span data-ttu-id="b2a69-146">Ниже приведены инструкции по каждому из этих методов.</span><span class="sxs-lookup"><span data-stu-id="b2a69-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="b2a69-147">Только API использования Azure показывает, к какой виртуальной машине применяется скидка.</span><span class="sxs-lookup"><span data-stu-id="b2a69-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="b2a69-148">Проверьте использование резервирования клиента в портал Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="b2a69-149">В центре партнеров перейдите на страницу **Клиенты** .</span><span class="sxs-lookup"><span data-stu-id="b2a69-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="b2a69-150">Найдите клиента, для которого требуется проверить скидку резервирования и использование, а затем щелкните стрелку вниз, чтобы развернуть сведения о клиенте.</span><span class="sxs-lookup"><span data-stu-id="b2a69-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="b2a69-151">Выберите **портал управления Microsoft Azure** , чтобы открыть запись клиента в портал Azure.</span><span class="sxs-lookup"><span data-stu-id="b2a69-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="b2a69-152">Выберите пункт **Резервирования** в меню портала, затем выберите резервирование, чтобы проверить его использование.</span><span class="sxs-lookup"><span data-stu-id="b2a69-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="b2a69-153">На странице **Обзор** проверьте график использования резервирования, который показывает, какая часть резервирования была применена к виртуальным машинам.</span><span class="sxs-lookup"><span data-stu-id="b2a69-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b2a69-154">Данные об использовании могут отображаться с задержкой до 8 часов.</span><span class="sxs-lookup"><span data-stu-id="b2a69-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="b2a69-155">а.</span><span class="sxs-lookup"><span data-stu-id="b2a69-155">a.</span></span> <span data-ttu-id="b2a69-156">Если использование резервирования составляет 100%, клиент получает все возможные сокращения, которые может предоставить Покупка резервирования.</span><span class="sxs-lookup"><span data-stu-id="b2a69-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="b2a69-157">b.</span><span class="sxs-lookup"><span data-stu-id="b2a69-157">b.</span></span> <span data-ttu-id="b2a69-158">Если использование резервирования составляет 0%, скидка не применяется ни к одной виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="b2a69-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="b2a69-159">c.</span><span class="sxs-lookup"><span data-stu-id="b2a69-159">c.</span></span> <span data-ttu-id="b2a69-160">Если использование резервирования составляет от 1% до 99%, то используются неиспользуемые преимущества.</span><span class="sxs-lookup"><span data-stu-id="b2a69-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="b2a69-161">Чтобы избежать такой ситуации, определите требуемый размер виртуальной машины, чтобы обеспечить поддержку вычислительных потребностей клиента перед покупкой.</span><span class="sxs-lookup"><span data-stu-id="b2a69-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="b2a69-162">Проверка использования резервирования клиентом с помощью API использования Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="b2a69-163">Только API использования Azure показывает, к какой виртуальной машине применяется скидка.</span><span class="sxs-lookup"><span data-stu-id="b2a69-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="b2a69-164">Вы можете получить данные об использовании резервирования с помощью API использования Azure. Так можно проверить, получает ли клиент скидку за резервирование, и посмотреть, к каким виртуальным машинам применяется эта скидка.</span><span class="sxs-lookup"><span data-stu-id="b2a69-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="b2a69-165">Сравните пример а с примером б, чтобы узнать, как проверить использование резервирования клиентом.</span><span class="sxs-lookup"><span data-stu-id="b2a69-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Примеры использования резервирования":::

- <span data-ttu-id="b2a69-167">Идентификатор reservationId определяет резервирование Azure, которое использовалось для применения скидки к виртуальной машине.</span><span class="sxs-lookup"><span data-stu-id="b2a69-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="b2a69-168">consumptionMeter — это MeterId для виртуальной машины, к которой применена скидка за резервирование.</span><span class="sxs-lookup"><span data-stu-id="b2a69-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="b2a69-169">ReservationMeter отображает стоимость $0, так как применена скидка за резервирование.</span><span class="sxs-lookup"><span data-stu-id="b2a69-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="b2a69-170">Дополнительные сведения см. в статье [получение записей об использовании клиента для Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) в [API центра партнеров](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="b2a69-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="b2a69-171">Стоимость программного обеспечения, например Microsoft Windows Server, в настоящее время не входит в цену резервирования виртуальных машин и отображается в отдельных строках заказа и счета.</span><span class="sxs-lookup"><span data-stu-id="b2a69-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="b2a69-172">Тем не менее, если у клиента есть преимущества гибридного использования Azure, стоимость программного обеспечения не учитывается.</span><span class="sxs-lookup"><span data-stu-id="b2a69-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="b2a69-173">Дополнительные сведения см. в разделе [Затраты на программное обеспечение Windows, не включенные в зарезервированные экземпляры](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="b2a69-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="b2a69-174">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b2a69-174">Next steps</span></span>

|<span data-ttu-id="b2a69-175">**Сведения о**</span><span class="sxs-lookup"><span data-stu-id="b2a69-175">**For information about**</span></span>   |<span data-ttu-id="b2a69-176">**Прочитайте это**</span><span class="sxs-lookup"><span data-stu-id="b2a69-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="b2a69-177">Обзор резервирований Azure в программе CSP</span><span class="sxs-lookup"><span data-stu-id="b2a69-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="b2a69-178">Продажа Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="b2a69-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="b2a69-179">Приобретение резервирований Azure для клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="b2a69-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="b2a69-180">Приобретение резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="b2a69-181">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="b2a69-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="b2a69-182">Управление резервированиями Azure в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="b2a69-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="b2a69-183">Приобретение резервирований Azure на портале Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="b2a69-184">[Предоплата за виртуальные машины с Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) в справке Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="b2a69-185">Управление резервированиями Azure на портале Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="b2a69-186">[Управление зарезервированными экземплярами виртуальных машин](/azure/billing/billing-manage-reserved-vm-instance) в справке Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="b2a69-187">Приобретение резервирований Azure с помощью API Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="b2a69-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="b2a69-188">[Приобретение услуги Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="b2a69-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="b2a69-189">Предоставление клиентам разрешения на приобретение собственных резервирований Azure из подписки, приобретенной для них.</span><span class="sxs-lookup"><span data-stu-id="b2a69-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="b2a69-190">Предоставление клиентам разрешения на приобретение собственных резервирований Azure</span><span class="sxs-lookup"><span data-stu-id="b2a69-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |