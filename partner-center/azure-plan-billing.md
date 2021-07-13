---
title: Выставление счетов по планам Azure — счет и файлы выверки
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как получить доступ к структуре файлов счетов и сверки, связанной с выставлением счетов для плана Azure, и понять ее содержимое.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551526"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="5dff6-103">Новый интерфейс для коммерческих приложений в CSP. Выставление счетов в Azure</span><span class="sxs-lookup"><span data-stu-id="5dff6-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="5dff6-104">**Соответствующие роли**: агент по администрированию | глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5dff6-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="5dff6-105">В этой статье объясняется, как получить доступ к структуре файлов счетов и файлов выверки, связанной с выставлением счетов для плана Azure, и понять ее содержимое.</span><span class="sxs-lookup"><span data-stu-id="5dff6-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="5dff6-106">Выставление счетов в рамках плана Azure — это простой инструмент выставления счетов за счет использования согласованной даты выставления счетов и расчетного периода на основе календарного месяца.</span><span class="sxs-lookup"><span data-stu-id="5dff6-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="5dff6-107">Основные сведения о выставлении счетов</span><span class="sxs-lookup"><span data-stu-id="5dff6-107">Summary of billing essentials</span></span>

- <span data-ttu-id="5dff6-108">**Дата выставления счета-фактуры**. Счет-фактура и файл выверки будут доступны с помощью API или Панели мониторинга Центра партнеров в полночь по UTC.</span><span class="sxs-lookup"><span data-stu-id="5dff6-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="5dff6-109">**Период выставления счетов**. Период выставления счетов определяется как за календарный месяц, например 1.10–31.10 или 1.11–30.11.</span><span class="sxs-lookup"><span data-stu-id="5dff6-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="5dff6-110">**Периоды начисления оплаты**: Плата будет начисляться за календарный месяц.</span><span class="sxs-lookup"><span data-stu-id="5dff6-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="5dff6-111">Например, если партнер, выставляющий счета, добавляет службы Azure через план Azure 15.10, а клиент начинает использование служб Azure с 15.10, то партнер получит счет-фактуру или файл выверки 8.11 по использованию клиентом служб в течение периода обслуживания 15.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="5dff6-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="5dff6-112">Счет за следующий месяц, который будет создан на 8.12, содержит все расходы за период обслуживания 1.11–31.11.</span><span class="sxs-lookup"><span data-stu-id="5dff6-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="5dff6-113">**Срок оплаты счета-фактуры**. В течение 60 дней.</span><span class="sxs-lookup"><span data-stu-id="5dff6-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="5dff6-114">**Валюта счета**. Начиная с 28 января 2021 г. для партнеров в регионе ЕС/ЕАСТ и Соединенном Королевстве с новыми клиентами и существующими клиентами по программе CSP, впервые приобретающими коммерческие предложения, арендаторы которых были созданы до 11 мая 2020 г., выставление счетов по таким покупкам будет производиться в местной валюте партнера.</span><span class="sxs-lookup"><span data-stu-id="5dff6-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="5dff6-115">Партнеры, располагающиеся за пределами ЕС/ЕАСТ и Соединенного Королевства, будут и дальше получать счета в местной валюте партнера.</span><span class="sxs-lookup"><span data-stu-id="5dff6-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="5dff6-116">**Поощрения для партнеров**. Оплачено 45 дней с конца месяца счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="5dff6-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="5dff6-117">Доступ к своим счетам и файлам выверки</span><span class="sxs-lookup"><span data-stu-id="5dff6-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="5dff6-118">Глобальный администратор или администратор выставления счетов для вашей компании получат электронное сообщение, когда счет-фактура будет готов к просмотру.</span><span class="sxs-lookup"><span data-stu-id="5dff6-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="5dff6-119">Доступ к счету и файлу выверки</span><span class="sxs-lookup"><span data-stu-id="5dff6-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="5dff6-120">Выполните вход в [Панель мониторинга](https://partner.microsoft.com/dashboard/) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5dff6-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5dff6-121">В меню Центра партнеров выберите **Billing** (Выставление счетов).</span><span class="sxs-lookup"><span data-stu-id="5dff6-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="5dff6-122">Выберите вкладки **Повторяемый** и **Единоразовый**, затем выберите интересующую вас валюту.</span><span class="sxs-lookup"><span data-stu-id="5dff6-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="Выставление счетов":::.

4. <span data-ttu-id="5dff6-124">Выберите **счет** или **файл выверки**.</span><span class="sxs-lookup"><span data-stu-id="5dff6-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="5dff6-125">Чтобы просмотреть предыдущие счета-фактуры и файлы выверки, разверните строку "История счетов" ниже.</span><span class="sxs-lookup"><span data-stu-id="5dff6-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="5dff6-126">Основные сведения о данных об использовании</span><span class="sxs-lookup"><span data-stu-id="5dff6-126">Understanding usage data</span></span> 

1. <span data-ttu-id="5dff6-127">План Azure — это корень или контейнер верхнего уровня для данных об использовании.</span><span class="sxs-lookup"><span data-stu-id="5dff6-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="5dff6-128">Все данные об использовании привязываются к одному плану Azure.</span><span class="sxs-lookup"><span data-stu-id="5dff6-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="5dff6-129">В плане может быть одна или несколько подписок Azure.</span><span class="sxs-lookup"><span data-stu-id="5dff6-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="5dff6-130">Это контейнеры, используемые для управления ресурсами и развертывания.</span><span class="sxs-lookup"><span data-stu-id="5dff6-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="5dff6-131">В подписку добавляются группы ресурсов, чтобы группировать ресурсы.</span><span class="sxs-lookup"><span data-stu-id="5dff6-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="5dff6-132">Каждый ресурс развертывается в одной группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5dff6-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="5dff6-133">К примерам ресурсов относятся виртуальные машины и учетные записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5dff6-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="5dff6-134">Ресурсы выдают единицы измерения. Единицы измерения — это измерения потребления ресурса, и один ресурс может выдавать данные об использовании нескольких единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="5dff6-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="5dff6-135">Единицы измерения определяются идентификаторами ProductId, SKUId и AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="5dff6-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="5dff6-136">Иерархия групп ресурсов и контроля потребления ресурсов в подписке</span><span class="sxs-lookup"><span data-stu-id="5dff6-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="5dff6-137">**Учетная запись Azure (арендатор)**</span><span class="sxs-lookup"><span data-stu-id="5dff6-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="5dff6-138">Подписка А</span><span class="sxs-lookup"><span data-stu-id="5dff6-138">Subscription A</span></span>
    - <span data-ttu-id="5dff6-139">ГруппаРесурсов 1</span><span class="sxs-lookup"><span data-stu-id="5dff6-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="5dff6-140">Виртуальная машина (ресурс)</span><span class="sxs-lookup"><span data-stu-id="5dff6-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="5dff6-141">Единица измерения вычислений</span><span class="sxs-lookup"><span data-stu-id="5dff6-141">Compute meter</span></span>
        - <span data-ttu-id="5dff6-142">Виртуальная сеть (ресурс)</span><span class="sxs-lookup"><span data-stu-id="5dff6-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="5dff6-143">Без оплачиваемых единиц измерения</span><span class="sxs-lookup"><span data-stu-id="5dff6-143">No billing meter</span></span>

    - <span data-ttu-id="5dff6-144">ГруппаРесурсов 2</span><span class="sxs-lookup"><span data-stu-id="5dff6-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="5dff6-145">Виртуальная машина (ресурс)</span><span class="sxs-lookup"><span data-stu-id="5dff6-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="5dff6-146">Единица измерения компьютеров</span><span class="sxs-lookup"><span data-stu-id="5dff6-146">Computer meter</span></span>
        - <span data-ttu-id="5dff6-147">Управляемый диск SSD ценовой категории "Премиум" (ресурс)</span><span class="sxs-lookup"><span data-stu-id="5dff6-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="5dff6-148">Единица измерения емкости хранилища</span><span class="sxs-lookup"><span data-stu-id="5dff6-148">Storage capacity meter</span></span>
            - <span data-ttu-id="5dff6-149">Единица измерения операций хранилища</span><span class="sxs-lookup"><span data-stu-id="5dff6-149">Storage operations meter</span></span>

- <span data-ttu-id="5dff6-150">Подписка Б — ГруппаРесурсов1 — SQL Azure (ресурс) — Единица измерения DTU — VPN-шлюз (ресурс) — Единица измерения VPN-шлюзов</span><span class="sxs-lookup"><span data-stu-id="5dff6-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="5dff6-151">ГруппаРесурсов 2</span><span class="sxs-lookup"><span data-stu-id="5dff6-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="5dff6-152">Виртуальный сетевой интерфейс (ресурс)</span><span class="sxs-lookup"><span data-stu-id="5dff6-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="5dff6-153">Без оплачиваемых единиц измерения</span><span class="sxs-lookup"><span data-stu-id="5dff6-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="5dff6-154">Чтение счета-фактуры</span><span class="sxs-lookup"><span data-stu-id="5dff6-154">Read the invoice</span></span>

1. <span data-ttu-id="5dff6-155">Счет будет доступен не позднее восьмого числа каждого месяца.</span><span class="sxs-lookup"><span data-stu-id="5dff6-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="5dff6-156">У партнеров есть 60 дней для предъявления платежа.</span><span class="sxs-lookup"><span data-stu-id="5dff6-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="5dff6-157">Расчетный период охватывает заданный календарный месяц, например 1.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="5dff6-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="5dff6-158">Плата взимается в процентах от корректировок (сумма — это доля от "Партнерского кредита на управляемые службы").</span><span class="sxs-lookup"><span data-stu-id="5dff6-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="5dff6-159">Чтобы получить дополнительные сведения о выставлении счетов, см. файл выверки счета-фактуры и файл ежедневного использования.</span><span class="sxs-lookup"><span data-stu-id="5dff6-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Счет":::.

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="5dff6-161">Чтение файла выверки для счета</span><span class="sxs-lookup"><span data-stu-id="5dff6-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="5dff6-162">Для каждого плана Azure и единицы измерения файл выверки может содержать до двух строк выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="5dff6-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="5dff6-163">Если для единицы измерения действует какая-либо скидка или кредит (например, скидки на основе категории или партнерский кредит за управляемые службы) на протяжении всего календарного месяца, то файл выверки будет содержать только одну строку выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="5dff6-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="5dff6-164">Столбец **PriceAdjusmentDescription** будет учитывать скидку или полученный кредит.</span><span class="sxs-lookup"><span data-stu-id="5dff6-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="5dff6-165">Если для определенной единицы измерения нет ресурсов, для которых действует скидка или партнерский кредит, то файл выверки будет содержать только одну строку выставления счетов, а действительной ценой за единицу будет розничная цена (которая будет ценой за единицу).</span><span class="sxs-lookup"><span data-stu-id="5dff6-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="5dff6-166">Если для единицы измерения или выдающих ее ресурсов предоставлен **партнерский кредит за управляемые службы** за часть месяца, то файл выверки будет содержать две строки выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="5dff6-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="5dff6-167">Одна строка будет представлять дни, в которых счетчик действует, а вторая — дни, в которые счетчик не применяется.</span><span class="sxs-lookup"><span data-stu-id="5dff6-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

>[!NOTE]
><span data-ttu-id="5dff6-168">Вы можете согласовать свое использование Azure в файле выверки для однократной покупки.</span><span class="sxs-lookup"><span data-stu-id="5dff6-168">You can reconcile your Azure consumption in your one-time purchase recon file.</span></span> <span data-ttu-id="5dff6-169">Для этого перейдите в свой файл выверки с ежедневной оценкой использования и найдите свой идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="5dff6-169">To do this, go to your daily-rated usage recon file and search for your SubscriptionID.</span></span> <span data-ttu-id="5dff6-170">Это позволит просмотреть все затраты, связанные с вашим идентификатором плана Azure.</span><span class="sxs-lookup"><span data-stu-id="5dff6-170">This will display all costs associated with your Azure Plan ID.</span></span> <span data-ttu-id="5dff6-171">Идентификатор подписки Azure отображается как идентификатор права (EntitlementID).</span><span class="sxs-lookup"><span data-stu-id="5dff6-171">Your Azure SubscriptionID is shown as the EntitlementID.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="5dff6-172">Чтение файла ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="5dff6-172">Read the daily usage file</span></span>

- <span data-ttu-id="5dff6-173">Счетчики подписки в плане Azure оцениваются и распределяются ежедневно.</span><span class="sxs-lookup"><span data-stu-id="5dff6-173">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="5dff6-174">**Партнерский кредит для управляемых служб** определяется и применяется ежедневно.</span><span class="sxs-lookup"><span data-stu-id="5dff6-174">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="5dff6-175">Каждый счетчик подписки будет иметь строку для каждого дня месяца, когда служба использовалась.</span><span class="sxs-lookup"><span data-stu-id="5dff6-175">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="5dff6-176">См. пример ниже.</span><span class="sxs-lookup"><span data-stu-id="5dff6-176">In the example below:</span></span>

  - <span data-ttu-id="5dff6-177">Счетчик действует для **партнерского кредита за управляемые службы** за период с 01.07 по 03.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="5dff6-177">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="5dff6-178">Счетчик не действует для **партнерского кредита за управляемые службы** за период с 04.07 по 07.07 (обратите внимание, что цена за единицу является розничной ценой).</span><span class="sxs-lookup"><span data-stu-id="5dff6-178">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="5dff6-179">Счетчик действует для **партнерского кредита за управляемые службы** за период с 08.07 по 31.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="5dff6-179">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="Выверка 2":::.

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="5dff6-181">Счет-фактура в валюте клиента</span><span class="sxs-lookup"><span data-stu-id="5dff6-181">Invoice in customer currency</span></span>

<span data-ttu-id="5dff6-182">Плата за службы Azure в плане Azure будет взиматься в долларах США (USD) и оплачиваться в валюте назначенной страны клиента.</span><span class="sxs-lookup"><span data-stu-id="5dff6-182">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="5dff6-183">Если счет выставляется не в долларах США (USD), то на последней странице счета будет указан используемый курс валют.</span><span class="sxs-lookup"><span data-stu-id="5dff6-183">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="5dff6-184">Курс валют определяется за месяц и применяется к следующему счету.</span><span class="sxs-lookup"><span data-stu-id="5dff6-184">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="5dff6-185">См. полный список валют в [этом документе](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="5dff6-185">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="5dff6-186">Корпорация Майкрософт применяет предварительно определенный обменный курс к базовым ценам в долларах США для вычисления совокупных затрат на службы Azure, приобретенные или использованные в каждом календарном месяце.</span><span class="sxs-lookup"><span data-stu-id="5dff6-186">Microsoft applies a predetermined exchange rate to base USD prices to arrive at total charges incurred for Azure services purchased or consumed each calendar month.</span></span> <span data-ttu-id="5dff6-187">В качестве ежемесячного обменного курса используется средний обменный курс, публикуемый Thomson Reuters (обычно) за два рабочих дня до окончания предыдущего месяца в 16:00 (GMT).</span><span class="sxs-lookup"><span data-stu-id="5dff6-187">The monthly exchange rate is the mid-rate published by Thomson Reuters (typically) two business days prior to the preceding month-end at 4:00 pm GMT.</span></span> 

<span data-ttu-id="5dff6-188">**Например,** в качестве декабрьского обменного курса Майкрософт использовался бы средний обменный курс для заданной валюты, опубликованный 29 ноября.</span><span class="sxs-lookup"><span data-stu-id="5dff6-188">**For example,** Microsoft’s December exchange rate would be the Thomson Reuters mid-rate on or around November 29 for a given currency.</span></span> <span data-ttu-id="5dff6-189">Этот курс был бы применен ко всем покупкам в этой валюте, осуществленным в период с 1 по 31 декабря.</span><span class="sxs-lookup"><span data-stu-id="5dff6-189">That rate will be applied to all purchases in that currency from December 1 to December 31.</span></span> 

## <a name="azure-reservations"></a><span data-ttu-id="5dff6-190">Резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="5dff6-190">Azure reservations</span></span>


<span data-ttu-id="5dff6-191">При приобретении [резервирований Azure](azure-reservations.md) в рамках плана Azure вы можете выбрать однократное или ежемесячное выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="5dff6-191">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="5dff6-192">Расходы на Azure</span><span class="sxs-lookup"><span data-stu-id="5dff6-192">Azure spending</span></span>

<span data-ttu-id="5dff6-193">Существующие возможности Azure по контролю расходов обновлены для поддержки выставления счетов по новым планам Azure в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="5dff6-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="5dff6-194">Это дает партнерам следующие возможности:</span><span class="sxs-lookup"><span data-stu-id="5dff6-194">This enables partners to:</span></span>

- <span data-ttu-id="5dff6-195">просмотр, получение оповещений об установленном бюджете на уровне клиента и управление этими оповещениями;</span><span class="sxs-lookup"><span data-stu-id="5dff6-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="5dff6-196">просмотр общих прогнозируемых расходов на план Azure (с разбивкой на уровне ресурса и единицы измерения).</span><span class="sxs-lookup"><span data-stu-id="5dff6-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="5dff6-197">Так как модель выставления счетов для служб Azure в плане Azure — это использование служб после оплаты, чтобы избежать выставления счета, размер которого превышает ожидаемый, партнеры могут формировать месячный бюджет и следить за ростом использования служб.</span><span class="sxs-lookup"><span data-stu-id="5dff6-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="5dff6-198">Бюджет может быть применен к одному клиенту или нескольким клиентам одновременно.</span><span class="sxs-lookup"><span data-stu-id="5dff6-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Расходы на Azure":::.

## <a name="next-steps"></a><span data-ttu-id="5dff6-200">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5dff6-200">Next steps</span></span>

- <span data-ttu-id="5dff6-201">Узнайте, как вычисляется партнерский кредит.</span><span class="sxs-lookup"><span data-stu-id="5dff6-201">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="5dff6-202">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/) Центра партнеров и щелкните доступный прейскурант.</span><span class="sxs-lookup"><span data-stu-id="5dff6-202">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="5dff6-203">Подробнее о [приобретении плана Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="5dff6-203">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="5dff6-204">Просмотрите [прейскурант для новой коммерческой модели в CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="5dff6-204">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
