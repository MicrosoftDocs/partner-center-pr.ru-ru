---
title: Выставление счетов для плана Azure | Центр партнеров
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как получить доступ к структуре файлов счетов и сверки, связанной с выставлением счетов для плана Azure, и понять ее содержимое.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 7aade0443c6418c9044a58d37b2351a89f86266d
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722223"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="d0a57-103">Новый интерфейс для коммерческих приложений в CSP. Выставление счетов в Azure</span><span class="sxs-lookup"><span data-stu-id="d0a57-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="d0a57-104">**Соответствующие роли:**</span><span class="sxs-lookup"><span data-stu-id="d0a57-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="d0a57-105">Агент администрирования</span><span class="sxs-lookup"><span data-stu-id="d0a57-105">Admin agent</span></span>
- <span data-ttu-id="d0a57-106">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="d0a57-106">Billing admin</span></span>
- <span data-ttu-id="d0a57-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d0a57-107">Global admin</span></span>

<span data-ttu-id="d0a57-108">Выставление счетов в рамках плана Azure — это простой инструмент выставления счетов за счет использования согласованной даты выставления счетов и расчетного периода на основе календарного месяца.</span><span class="sxs-lookup"><span data-stu-id="d0a57-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="d0a57-109">Дополнительные сведения о платформе выставления счетов см. в статье [Общие сведения о выставлении счетов](billing-basics.md).</span><span class="sxs-lookup"><span data-stu-id="d0a57-109">For information on the billing platform, read [Billing overview](billing-basics.md).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="d0a57-110">Основные сведения о выставлении счетов</span><span class="sxs-lookup"><span data-stu-id="d0a57-110">Summary of billing essentials</span></span>

- <span data-ttu-id="d0a57-111">**Дата выставления счета-фактуры**. Счет-фактура и файл выверки будут доступны с помощью API или Панели мониторинга Центра партнеров в полночь по UTC.</span><span class="sxs-lookup"><span data-stu-id="d0a57-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="d0a57-112">**Период выставления счетов**. Период выставления счетов определяется как за календарный месяц, например 1.10–31.10 или 1.11–30.11.</span><span class="sxs-lookup"><span data-stu-id="d0a57-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="d0a57-113">**Периоды начисления оплаты**: Плата будет начисляться за календарный месяц.</span><span class="sxs-lookup"><span data-stu-id="d0a57-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="d0a57-114">Например, если партнер, выставляющий счета, добавляет службы Azure через план Azure 15.10, а клиент начинает использование служб Azure с 15.10, то партнер получит счет-фактуру или файл выверки 8.11 по использованию клиентом служб в течение периода обслуживания 15.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="d0a57-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="d0a57-115">Счет за следующий месяц, который будет создан на 8.12, содержит все расходы за период обслуживания 1.11–31.11.</span><span class="sxs-lookup"><span data-stu-id="d0a57-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="d0a57-116">**Срок оплаты счета-фактуры**. В течение 60 дней.</span><span class="sxs-lookup"><span data-stu-id="d0a57-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="d0a57-117">**Валюта счета**. Партнеры будут по-прежнему получать счета-фактуры в назначенной валюте страны клиента.</span><span class="sxs-lookup"><span data-stu-id="d0a57-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="d0a57-118">Например, если партнер в Ирландии выставляет счета клиентам в Великобритании, Норвегии и Германии, то партнер будет получать счет-фактуру или файл выверки в фунтах стерлингов (GBP), норвежских кронах (NOK) и евро (EUR).</span><span class="sxs-lookup"><span data-stu-id="d0a57-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="d0a57-119">**Поощрения для партнеров**. Оплачено 45 дней с конца месяца счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="d0a57-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="d0a57-120">Доступ к своим счетам и файлам выверки</span><span class="sxs-lookup"><span data-stu-id="d0a57-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="d0a57-121">Глобальный администратор или администратор выставления счетов для вашей компании получат электронное сообщение, когда счет-фактура будет готов к просмотру.</span><span class="sxs-lookup"><span data-stu-id="d0a57-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="d0a57-122">**Доступ к счету и файлу выверки**</span><span class="sxs-lookup"><span data-stu-id="d0a57-122">**To access the invoice and reconciliation file**</span></span>

1. <span data-ttu-id="d0a57-123">Выполните вход в [Панель мониторинга](https://partner.microsoft.com/en-us/dashboard/) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d0a57-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/).</span></span>

2. <span data-ttu-id="d0a57-124">В меню Центра партнеров выберите **Billing** (Выставление счетов).</span><span class="sxs-lookup"><span data-stu-id="d0a57-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="d0a57-125">Выберите вкладки **Повторяемый** и **Единоразовый**, затем выберите интересующую вас валюту.</span><span class="sxs-lookup"><span data-stu-id="d0a57-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

![выставление счетов](images/azure/billing1.png)

4. <span data-ttu-id="d0a57-127">Выберите **счет** или **файл выверки**.</span><span class="sxs-lookup"><span data-stu-id="d0a57-127">Select **Invoice** or **Reconciliation file**.</span></span>  

<span data-ttu-id="d0a57-128">Чтобы просмотреть предыдущие счета-фактуры и файлы выверки, разверните строку "История счетов" ниже.</span><span class="sxs-lookup"><span data-stu-id="d0a57-128">To view historical invoices and recon files expand the Billing history row below.</span></span>


## <a name="understanding-usage-data"></a><span data-ttu-id="d0a57-129">Основные сведения о данных об использовании</span><span class="sxs-lookup"><span data-stu-id="d0a57-129">Understanding usage data</span></span> 

1. <span data-ttu-id="d0a57-130">План Azure — это корень или контейнер верхнего уровня для данных об использовании.</span><span class="sxs-lookup"><span data-stu-id="d0a57-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="d0a57-131">Все данные об использовании привязываются к одному плану Azure.</span><span class="sxs-lookup"><span data-stu-id="d0a57-131">All usage is tied back to a single azure plan.</span></span> 

2. <span data-ttu-id="d0a57-132">В плане может быть одна или несколько подписок Azure.</span><span class="sxs-lookup"><span data-stu-id="d0a57-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="d0a57-133">Это контейнеры, используемые для управления ресурсами и развертывания.</span><span class="sxs-lookup"><span data-stu-id="d0a57-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="d0a57-134">В подписку добавляются группы ресурсов, чтобы группировать ресурсы.</span><span class="sxs-lookup"><span data-stu-id="d0a57-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="d0a57-135">Каждый ресурс развертывается в одной группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d0a57-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="d0a57-136">К примерам ресурсов относятся виртуальные машины и учетные записи хранения.</span><span class="sxs-lookup"><span data-stu-id="d0a57-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="d0a57-137">Ресурсы выдают единицы измерения. Единицы измерения — это измерения потребления ресурса, и один ресурс может выдавать данные об использовании нескольких единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="d0a57-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="d0a57-138">Единицы измерения определяются идентификаторами ProductId, SKUId и AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="d0a57-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="heirarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="d0a57-139">Иерархия групп ресурсов и контроля потребления ресурсов в подписке</span><span class="sxs-lookup"><span data-stu-id="d0a57-139">Heirarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="d0a57-140">**Учетная запись Azure (арендатор)**</span><span class="sxs-lookup"><span data-stu-id="d0a57-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="d0a57-141">Подписка А</span><span class="sxs-lookup"><span data-stu-id="d0a57-141">Subscription A</span></span>
    - <span data-ttu-id="d0a57-142">ГруппаРесурсов 1</span><span class="sxs-lookup"><span data-stu-id="d0a57-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="d0a57-143">Виртуальная машина (ресурс)</span><span class="sxs-lookup"><span data-stu-id="d0a57-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="d0a57-144">Единица измерения вычислений</span><span class="sxs-lookup"><span data-stu-id="d0a57-144">Compute meter</span></span>
        - <span data-ttu-id="d0a57-145">Виртуальная сеть (ресурс)</span><span class="sxs-lookup"><span data-stu-id="d0a57-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="d0a57-146">Без оплачиваемых единиц измерения</span><span class="sxs-lookup"><span data-stu-id="d0a57-146">No billing meter</span></span>

    - <span data-ttu-id="d0a57-147">ГруппаРесурсов 2</span><span class="sxs-lookup"><span data-stu-id="d0a57-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="d0a57-148">Виртуальная машина (ресурс)</span><span class="sxs-lookup"><span data-stu-id="d0a57-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="d0a57-149">Единица измерения компьютеров</span><span class="sxs-lookup"><span data-stu-id="d0a57-149">Computer meter</span></span>
        - <span data-ttu-id="d0a57-150">Управляемый диск SSD (цен. категория "Премиум") (ресурс)</span><span class="sxs-lookup"><span data-stu-id="d0a57-150">Premium SSD managed disk (resource)</span></span>
            - <span data-ttu-id="d0a57-151">Единица измерения емкости хранилища</span><span class="sxs-lookup"><span data-stu-id="d0a57-151">Storage capacity meter</span></span>
            - <span data-ttu-id="d0a57-152">Единица измерения операций хранилища</span><span class="sxs-lookup"><span data-stu-id="d0a57-152">Storage operations meter</span></span>

- <span data-ttu-id="d0a57-153">Подписка Б — ГруппаРесурсов1 — SQL Azure (ресурс) — Единица измерения DTU — VPN-шлюз (ресурс) — Единица измерения VPN-шлюзов</span><span class="sxs-lookup"><span data-stu-id="d0a57-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="d0a57-154">ГруппаРесурсов 2</span><span class="sxs-lookup"><span data-stu-id="d0a57-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="d0a57-155">Виртуальный сетевой интерфейс (ресурс)</span><span class="sxs-lookup"><span data-stu-id="d0a57-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="d0a57-156">Без оплачиваемых единиц измерения</span><span class="sxs-lookup"><span data-stu-id="d0a57-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="d0a57-157">Чтение счета-фактуры</span><span class="sxs-lookup"><span data-stu-id="d0a57-157">Read the invoice</span></span>

1. <span data-ttu-id="d0a57-158">Счет будет доступен не позднее 8 числа каждого месяца.</span><span class="sxs-lookup"><span data-stu-id="d0a57-158">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="d0a57-159">У партнеров есть 60 дней для предъявления платежа.</span><span class="sxs-lookup"><span data-stu-id="d0a57-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="d0a57-160">Расчетный период охватывает заданный календарный месяц, например 1.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="d0a57-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="d0a57-161">Плата взимается в процентах от корректировок (сумма — это доля от "Партнерского кредита на управляемые службы").</span><span class="sxs-lookup"><span data-stu-id="d0a57-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="d0a57-162">Чтобы получить дополнительные сведения о выставлении счетов, см. файл выверки счета-фактуры и файл ежедневного использования.</span><span class="sxs-lookup"><span data-stu-id="d0a57-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![счет-фактура](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="d0a57-164">Чтение файла выверки для счета</span><span class="sxs-lookup"><span data-stu-id="d0a57-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="d0a57-165">Для каждого плана Azure и единицы измерения файл выверки может содержать до двух строк выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d0a57-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="d0a57-166">Если для единицы измерения действует какая-либо скидка или кредит (например, скидки на основе категории или партнерский кредит за управляемые службы) на протяжении всего календарного месяца, то файл выверки будет содержать только одну строку выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d0a57-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="d0a57-167">Столбец **PriceAdjusmentDescription** будет учитывать скидку или полученный кредит.</span><span class="sxs-lookup"><span data-stu-id="d0a57-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="d0a57-168">Если для определенной единицы измерения нет ресурсов, для которых действует скидка или партнерский кредит, то файл выверки будет содержать только одну строку выставления счетов, а действительной ценой за единицу будет розничная цена (которая будет ценой за единицу).</span><span class="sxs-lookup"><span data-stu-id="d0a57-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="d0a57-169">Если для единицы измерения или выдающих ее ресурсов предоставлен **партнерский кредит за управляемые службы** за часть месяца, то файл выверки будет содержать две строки выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d0a57-169">If the meter, or any resources emitting that meter,qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="d0a57-170">Одна строка будет представлять дни, в которых счетчик действует, а вторая — дни, в которые счетчик не применяется.</span><span class="sxs-lookup"><span data-stu-id="d0a57-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="d0a57-171">Чтение файла ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="d0a57-171">Read the daily usage file</span></span>

- <span data-ttu-id="d0a57-172">Счетчики подписки в плане Azure оцениваются и распределяются ежедневно.</span><span class="sxs-lookup"><span data-stu-id="d0a57-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="d0a57-173">**Партнерский кредит для управляемых служб** определяется и применяется ежедневно.</span><span class="sxs-lookup"><span data-stu-id="d0a57-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="d0a57-174">Каждый счетчик подписки будет иметь строку для каждого дня месяца, когда служба использовалась.</span><span class="sxs-lookup"><span data-stu-id="d0a57-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="d0a57-175">См. пример ниже.</span><span class="sxs-lookup"><span data-stu-id="d0a57-175">In the example below:</span></span>

  - <span data-ttu-id="d0a57-176">Счетчик действует для **партнерского кредита за управляемые службы** за период с 01.07 по 03.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="d0a57-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="d0a57-177">Счетчик не действует для **партнерского кредита за управляемые службы** за период с 04.07 по 07.07 (обратите внимание, что цена за единицу является розничной ценой).</span><span class="sxs-lookup"><span data-stu-id="d0a57-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="d0a57-178">Счетчик действует для **партнерского кредита за управляемые службы** за период с 08.07 по 31.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="d0a57-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="d0a57-180">Счет-фактура в валюте клиента</span><span class="sxs-lookup"><span data-stu-id="d0a57-180">Invoice in customer currency</span></span> 

<span data-ttu-id="d0a57-181">Плата за службы Azure в плане Azure будет взиматься в долларах США (USD) и оплачиваться в валюте назначенной страны клиента.</span><span class="sxs-lookup"><span data-stu-id="d0a57-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="d0a57-182">Если счет выставляется не в долларах США (USD), то на последней странице счета будет указан используемый курс валют.</span><span class="sxs-lookup"><span data-stu-id="d0a57-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="d0a57-183">Курс валют определяется за месяц и применяется к следующему счету.</span><span class="sxs-lookup"><span data-stu-id="d0a57-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="d0a57-184">См. полный список валют в [этом документе](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="d0a57-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span> 

<span data-ttu-id="d0a57-185">Корпорация Майкрософт будет использовать данные [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) при определении курса валют, используемого для определения и конвертации валюты выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d0a57-185">Microsoft will use [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="d0a57-186">Курсы валют будут обновляться и доступны за день до первого дня месяца, для которого они применяются.</span><span class="sxs-lookup"><span data-stu-id="d0a57-186">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="d0a57-187">**Пример**:  Плата за использование в период обслуживания с 1 по 31 августа будет взиматься по курсу валют, опубликованному 31 июля.</span><span class="sxs-lookup"><span data-stu-id="d0a57-187">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="d0a57-188">Эта плата отобразится в сентябрьском счете-фактуре, и курс валют будет указан на последней странице счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="d0a57-188">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

 
## <a name="azure-reservations"></a><span data-ttu-id="d0a57-189">Резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="d0a57-189">Azure reservations</span></span> 

<span data-ttu-id="d0a57-190">В случае приобретения [резервирования Azure](https://docs.microsoft.com/partner-center/azure-reservations) с помощью плана Azure, сначала можно будет выбрать разовое выставление счета в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="d0a57-190">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="d0a57-191">Ежемесячное выставление счетов доступно на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d0a57-191">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="d0a57-192">Ежемесячное выставление счетов будет доступно в Центре партнеров позже.</span><span class="sxs-lookup"><span data-stu-id="d0a57-192">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-spending"></a><span data-ttu-id="d0a57-193">Расходы на Azure</span><span class="sxs-lookup"><span data-stu-id="d0a57-193">Azure spending</span></span> 

<span data-ttu-id="d0a57-194">Существующие возможности Azure по контролю расходов обновлены для поддержки выставления счетов по новым планам Azure в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="d0a57-194">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="d0a57-195">Это дает партнерам следующие возможности:</span><span class="sxs-lookup"><span data-stu-id="d0a57-195">This enables partners to:</span></span>

- <span data-ttu-id="d0a57-196">просмотр, получение оповещений об установленном бюджете на уровне клиента и управление этими оповещениями;</span><span class="sxs-lookup"><span data-stu-id="d0a57-196">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="d0a57-197">просмотр общих прогнозируемых расходов на план Azure (с разбивкой на уровне ресурса и единицы измерения).</span><span class="sxs-lookup"><span data-stu-id="d0a57-197">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="d0a57-198">Так как модель выставления счетов для служб Azure в плане Azure — это использование служб после оплаты, чтобы избежать выставления счета, размер которого превышает ожидаемый, партнеры могут формировать месячный бюджет и следить за ростом использования служб.</span><span class="sxs-lookup"><span data-stu-id="d0a57-198">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="d0a57-199">Бюджет может быть применен к одному клиенту или нескольким клиентам одновременно.</span><span class="sxs-lookup"><span data-stu-id="d0a57-199">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Расходы на Azure](images/azure/azurespend.png)

<span data-ttu-id="d0a57-201">**Дополнительные сведения**</span><span class="sxs-lookup"><span data-stu-id="d0a57-201">**For more information**</span></span>

-  <span data-ttu-id="d0a57-202">Схема расчета партнерского кредита указана в прейскуранте, доступном на [Панели мониторинга](https://partner.microsoft.com/en-us/dashboard/) Центра партнеров (требуется вход).</span><span class="sxs-lookup"><span data-stu-id="d0a57-202">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/) (sign in required).</span></span> 
   
-  [<span data-ttu-id="d0a57-203">Приобретение плана Azure</span><span class="sxs-lookup"><span data-stu-id="d0a57-203">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="d0a57-204">Прейскурант для новой коммерческой модели в CSP</span><span class="sxs-lookup"><span data-stu-id="d0a57-204">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
