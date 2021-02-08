---
title: Выставление счетов по планам Azure — счет и файлы выверки
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как получить доступ к структуре файлов счетов и сверки, связанной с выставлением счетов для плана Azure, и понять ее содержимое.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925004"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="071c9-103">Новый интерфейс для коммерческих приложений в CSP. Выставление счетов в Azure</span><span class="sxs-lookup"><span data-stu-id="071c9-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="071c9-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="071c9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="071c9-105">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="071c9-105">Admin agent</span></span>
- <span data-ttu-id="071c9-106">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="071c9-106">Billing admin</span></span>
- <span data-ttu-id="071c9-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="071c9-107">Global admin</span></span>

<span data-ttu-id="071c9-108">В этой статье объясняется, как получить доступ к структуре файлов счетов и файлов выверки, связанной с выставлением счетов для плана Azure, и понять ее содержимое.</span><span class="sxs-lookup"><span data-stu-id="071c9-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="071c9-109">Выставление счетов в рамках плана Azure — это простой инструмент выставления счетов за счет использования согласованной даты выставления счетов и расчетного периода на основе календарного месяца.</span><span class="sxs-lookup"><span data-stu-id="071c9-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="071c9-110">Основные сведения о выставлении счетов</span><span class="sxs-lookup"><span data-stu-id="071c9-110">Summary of billing essentials</span></span>

- <span data-ttu-id="071c9-111">**Дата выставления счета-фактуры**. Счет-фактура и файл выверки будут доступны с помощью API или Панели мониторинга Центра партнеров в полночь по UTC.</span><span class="sxs-lookup"><span data-stu-id="071c9-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="071c9-112">**Период выставления счетов**. Период выставления счетов определяется как за календарный месяц, например 1.10–31.10 или 1.11–30.11.</span><span class="sxs-lookup"><span data-stu-id="071c9-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="071c9-113">**Периоды начисления оплаты**: Плата будет начисляться за календарный месяц.</span><span class="sxs-lookup"><span data-stu-id="071c9-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="071c9-114">Например, если партнер, выставляющий счета, добавляет службы Azure через план Azure 15.10, а клиент начинает использование служб Azure с 15.10, то партнер получит счет-фактуру или файл выверки 8.11 по использованию клиентом служб в течение периода обслуживания 15.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="071c9-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="071c9-115">Счет за следующий месяц, который будет создан на 8.12, содержит все расходы за период обслуживания 1.11–31.11.</span><span class="sxs-lookup"><span data-stu-id="071c9-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="071c9-116">**Срок оплаты счета-фактуры**. В течение 60 дней.</span><span class="sxs-lookup"><span data-stu-id="071c9-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="071c9-117">**Валюта счета**. Начиная с 28 января 2021 г. для партнеров в регионе ЕС/ЕАСТ и Соединенном Королевстве с новыми клиентами и существующими клиентами по программе CSP, впервые приобретающими коммерческие предложения, арендаторы которых были созданы до 11 мая 2020 г., выставление счетов по таким покупкам будет производиться в местной валюте партнера.</span><span class="sxs-lookup"><span data-stu-id="071c9-117">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="071c9-118">Партнеры, располагающиеся за пределами ЕС/ЕАСТ и Соединенного Королевства, будут и дальше получать счета в местной валюте партнера.</span><span class="sxs-lookup"><span data-stu-id="071c9-118">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="071c9-119">**Поощрения для партнеров**. Оплачено 45 дней с конца месяца счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="071c9-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="071c9-120">Доступ к своим счетам и файлам выверки</span><span class="sxs-lookup"><span data-stu-id="071c9-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="071c9-121">Глобальный администратор или администратор выставления счетов для вашей компании получат электронное сообщение, когда счет-фактура будет готов к просмотру.</span><span class="sxs-lookup"><span data-stu-id="071c9-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="071c9-122">Доступ к счету и файлу выверки</span><span class="sxs-lookup"><span data-stu-id="071c9-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="071c9-123">Выполните вход в [Панель мониторинга](https://partner.microsoft.com/dashboard/) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="071c9-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="071c9-124">В меню Центра партнеров выберите **Billing** (Выставление счетов).</span><span class="sxs-lookup"><span data-stu-id="071c9-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="071c9-125">Выберите вкладки **Повторяемый** и **Единоразовый**, затем выберите интересующую вас валюту.</span><span class="sxs-lookup"><span data-stu-id="071c9-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="выставление счетов":::

4. <span data-ttu-id="071c9-127">Выберите **счет** или **файл выверки**.</span><span class="sxs-lookup"><span data-stu-id="071c9-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="071c9-128">Чтобы просмотреть предыдущие счета-фактуры и файлы выверки, разверните строку "История счетов" ниже.</span><span class="sxs-lookup"><span data-stu-id="071c9-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="071c9-129">Основные сведения о данных об использовании</span><span class="sxs-lookup"><span data-stu-id="071c9-129">Understanding usage data</span></span> 

1. <span data-ttu-id="071c9-130">План Azure — это корень или контейнер верхнего уровня для данных об использовании.</span><span class="sxs-lookup"><span data-stu-id="071c9-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="071c9-131">Все данные об использовании привязываются к одному плану Azure.</span><span class="sxs-lookup"><span data-stu-id="071c9-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="071c9-132">В плане может быть одна или несколько подписок Azure.</span><span class="sxs-lookup"><span data-stu-id="071c9-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="071c9-133">Это контейнеры, используемые для управления ресурсами и развертывания.</span><span class="sxs-lookup"><span data-stu-id="071c9-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="071c9-134">В подписку добавляются группы ресурсов, чтобы группировать ресурсы.</span><span class="sxs-lookup"><span data-stu-id="071c9-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="071c9-135">Каждый ресурс развертывается в одной группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="071c9-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="071c9-136">К примерам ресурсов относятся виртуальные машины и учетные записи хранения.</span><span class="sxs-lookup"><span data-stu-id="071c9-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="071c9-137">Ресурсы выдают единицы измерения. Единицы измерения — это измерения потребления ресурса, и один ресурс может выдавать данные об использовании нескольких единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="071c9-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="071c9-138">Единицы измерения определяются идентификаторами ProductId, SKUId и AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="071c9-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="071c9-139">Иерархия групп ресурсов и контроля потребления ресурсов в подписке</span><span class="sxs-lookup"><span data-stu-id="071c9-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="071c9-140">**Учетная запись Azure (арендатор)**</span><span class="sxs-lookup"><span data-stu-id="071c9-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="071c9-141">Подписка А</span><span class="sxs-lookup"><span data-stu-id="071c9-141">Subscription A</span></span>
    - <span data-ttu-id="071c9-142">ГруппаРесурсов 1</span><span class="sxs-lookup"><span data-stu-id="071c9-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="071c9-143">Виртуальная машина (ресурс)</span><span class="sxs-lookup"><span data-stu-id="071c9-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="071c9-144">Единица измерения вычислений</span><span class="sxs-lookup"><span data-stu-id="071c9-144">Compute meter</span></span>
        - <span data-ttu-id="071c9-145">Виртуальная сеть (ресурс)</span><span class="sxs-lookup"><span data-stu-id="071c9-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="071c9-146">Без оплачиваемых единиц измерения</span><span class="sxs-lookup"><span data-stu-id="071c9-146">No billing meter</span></span>

    - <span data-ttu-id="071c9-147">ГруппаРесурсов 2</span><span class="sxs-lookup"><span data-stu-id="071c9-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="071c9-148">Виртуальная машина (ресурс)</span><span class="sxs-lookup"><span data-stu-id="071c9-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="071c9-149">Единица измерения компьютеров</span><span class="sxs-lookup"><span data-stu-id="071c9-149">Computer meter</span></span>
        - <span data-ttu-id="071c9-150">Управляемый диск SSD ценовой категории "Премиум" (ресурс)</span><span class="sxs-lookup"><span data-stu-id="071c9-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="071c9-151">Единица измерения емкости хранилища</span><span class="sxs-lookup"><span data-stu-id="071c9-151">Storage capacity meter</span></span>
            - <span data-ttu-id="071c9-152">Единица измерения операций хранилища</span><span class="sxs-lookup"><span data-stu-id="071c9-152">Storage operations meter</span></span>

- <span data-ttu-id="071c9-153">Подписка Б — ГруппаРесурсов1 — SQL Azure (ресурс) — Единица измерения DTU — VPN-шлюз (ресурс) — Единица измерения VPN-шлюзов</span><span class="sxs-lookup"><span data-stu-id="071c9-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="071c9-154">ГруппаРесурсов 2</span><span class="sxs-lookup"><span data-stu-id="071c9-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="071c9-155">Виртуальный сетевой интерфейс (ресурс)</span><span class="sxs-lookup"><span data-stu-id="071c9-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="071c9-156">Без оплачиваемых единиц измерения</span><span class="sxs-lookup"><span data-stu-id="071c9-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="071c9-157">Чтение счета-фактуры</span><span class="sxs-lookup"><span data-stu-id="071c9-157">Read the invoice</span></span>

1. <span data-ttu-id="071c9-158">Счет будет доступен не позднее восьмого числа каждого месяца.</span><span class="sxs-lookup"><span data-stu-id="071c9-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="071c9-159">У партнеров есть 60 дней для предъявления платежа.</span><span class="sxs-lookup"><span data-stu-id="071c9-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="071c9-160">Расчетный период охватывает заданный календарный месяц, например 1.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="071c9-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="071c9-161">Плата взимается в процентах от корректировок (сумма — это доля от "Партнерского кредита на управляемые службы").</span><span class="sxs-lookup"><span data-stu-id="071c9-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="071c9-162">Чтобы получить дополнительные сведения о выставлении счетов, см. файл выверки счета-фактуры и файл ежедневного использования.</span><span class="sxs-lookup"><span data-stu-id="071c9-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="счет-фактура":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="071c9-164">Чтение файла выверки для счета</span><span class="sxs-lookup"><span data-stu-id="071c9-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="071c9-165">Для каждого плана Azure и единицы измерения файл выверки может содержать до двух строк выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="071c9-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="071c9-166">Если для единицы измерения действует какая-либо скидка или кредит (например, скидки на основе категории или партнерский кредит за управляемые службы) на протяжении всего календарного месяца, то файл выверки будет содержать только одну строку выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="071c9-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="071c9-167">Столбец **PriceAdjusmentDescription** будет учитывать скидку или полученный кредит.</span><span class="sxs-lookup"><span data-stu-id="071c9-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="071c9-168">Если для определенной единицы измерения нет ресурсов, для которых действует скидка или партнерский кредит, то файл выверки будет содержать только одну строку выставления счетов, а действительной ценой за единицу будет розничная цена (которая будет ценой за единицу).</span><span class="sxs-lookup"><span data-stu-id="071c9-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="071c9-169">Если для единицы измерения или выдающих ее ресурсов предоставлен **партнерский кредит за управляемые службы** за часть месяца, то файл выверки будет содержать две строки выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="071c9-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="071c9-170">Одна строка будет представлять дни, в которых счетчик действует, а вторая — дни, в которые счетчик не применяется.</span><span class="sxs-lookup"><span data-stu-id="071c9-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="071c9-171">Чтение файла ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="071c9-171">Read the daily usage file</span></span>

- <span data-ttu-id="071c9-172">Счетчики подписки в плане Azure оцениваются и распределяются ежедневно.</span><span class="sxs-lookup"><span data-stu-id="071c9-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="071c9-173">**Партнерский кредит для управляемых служб** определяется и применяется ежедневно.</span><span class="sxs-lookup"><span data-stu-id="071c9-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="071c9-174">Каждый счетчик подписки будет иметь строку для каждого дня месяца, когда служба использовалась.</span><span class="sxs-lookup"><span data-stu-id="071c9-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="071c9-175">См. пример ниже.</span><span class="sxs-lookup"><span data-stu-id="071c9-175">In the example below:</span></span>

  - <span data-ttu-id="071c9-176">Счетчик действует для **партнерского кредита за управляемые службы** за период с 01.07 по 03.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="071c9-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="071c9-177">Счетчик не действует для **партнерского кредита за управляемые службы** за период с 04.07 по 07.07 (обратите внимание, что цена за единицу является розничной ценой).</span><span class="sxs-lookup"><span data-stu-id="071c9-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="071c9-178">Счетчик действует для **партнерского кредита за управляемые службы** за период с 08.07 по 31.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="071c9-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="071c9-180">Счет-фактура в валюте клиента</span><span class="sxs-lookup"><span data-stu-id="071c9-180">Invoice in customer currency</span></span>

<span data-ttu-id="071c9-181">Плата за службы Azure в плане Azure будет взиматься в долларах США (USD) и оплачиваться в валюте назначенной страны клиента.</span><span class="sxs-lookup"><span data-stu-id="071c9-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="071c9-182">Если счет выставляется не в долларах США (USD), то на последней странице счета будет указан используемый курс валют.</span><span class="sxs-lookup"><span data-stu-id="071c9-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="071c9-183">Курс валют определяется за месяц и применяется к следующему счету.</span><span class="sxs-lookup"><span data-stu-id="071c9-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="071c9-184">См. полный список валют в [этом документе](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="071c9-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="071c9-185">Для конвертации корпорация Майкрософт руководствуется данными Лондонской фондовой биржи.</span><span class="sxs-lookup"><span data-stu-id="071c9-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="071c9-186">Мы используем обменный курс, зафиксированный на Лондонской фондовой бирже за последнюю секунду последнего рабочего дня месяца.</span><span class="sxs-lookup"><span data-stu-id="071c9-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="071c9-187">Курсы валют будут обновляться и доступны за день до первого дня месяца, для которого они применяются.</span><span class="sxs-lookup"><span data-stu-id="071c9-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="071c9-188">Резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="071c9-188">Azure reservations</span></span>


<span data-ttu-id="071c9-189">При приобретении [резервирований Azure](azure-reservations.md) в рамках плана Azure вы можете выбрать однократное или ежемесячное выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="071c9-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="071c9-190">Расходы на Azure</span><span class="sxs-lookup"><span data-stu-id="071c9-190">Azure spending</span></span>

<span data-ttu-id="071c9-191">Существующие возможности Azure по контролю расходов обновлены для поддержки выставления счетов по новым планам Azure в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="071c9-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="071c9-192">Это дает партнерам следующие возможности:</span><span class="sxs-lookup"><span data-stu-id="071c9-192">This enables partners to:</span></span>

- <span data-ttu-id="071c9-193">просмотр, получение оповещений об установленном бюджете на уровне клиента и управление этими оповещениями;</span><span class="sxs-lookup"><span data-stu-id="071c9-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="071c9-194">просмотр общих прогнозируемых расходов на план Azure (с разбивкой на уровне ресурса и единицы измерения).</span><span class="sxs-lookup"><span data-stu-id="071c9-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="071c9-195">Так как модель выставления счетов для служб Azure в плане Azure — это использование служб после оплаты, чтобы избежать выставления счета, размер которого превышает ожидаемый, партнеры могут формировать месячный бюджет и следить за ростом использования служб.</span><span class="sxs-lookup"><span data-stu-id="071c9-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="071c9-196">Бюджет может быть применен к одному клиенту или нескольким клиентам одновременно.</span><span class="sxs-lookup"><span data-stu-id="071c9-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Расходы на Azure":::

## <a name="next-steps"></a><span data-ttu-id="071c9-198">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="071c9-198">Next steps</span></span>

- <span data-ttu-id="071c9-199">Узнайте, как вычисляется партнерский кредит.</span><span class="sxs-lookup"><span data-stu-id="071c9-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="071c9-200">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/) Центра партнеров и щелкните доступный прейскурант.</span><span class="sxs-lookup"><span data-stu-id="071c9-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="071c9-201">Подробнее о [приобретении плана Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="071c9-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="071c9-202">Просмотрите [прейскурант для новой коммерческой модели в CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="071c9-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
