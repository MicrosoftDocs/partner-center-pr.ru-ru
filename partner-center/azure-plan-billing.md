---
title: Выставление счетов для плана Azure | Центр партнеров
ms.topic: article
ms.date: 10/04/2019
description: Описывает структуру файла выверки и счета-фактуры
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171303"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="55008-103">Новый интерфейс для коммерческих приложений в CSP. Выставление счетов в Azure</span><span class="sxs-lookup"><span data-stu-id="55008-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="55008-104">Выставление счетов в рамках плана Azure — это простой инструмент выставления счетов за счет использования согласованной даты выставления счетов и расчетного периода на основе календарного месяца.</span><span class="sxs-lookup"><span data-stu-id="55008-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="55008-105">Сведения о платформе выставления счетов см. в статье [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (Руководство по современной коммерции с помощью Центра партнеров).</span><span class="sxs-lookup"><span data-stu-id="55008-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="55008-106">Основные сведения о выставлении счетов</span><span class="sxs-lookup"><span data-stu-id="55008-106">Summary of billing essentials</span></span>

- <span data-ttu-id="55008-107">**Дата выставления счета-фактуры**. Счет-фактура и файл выверки будут доступны с помощью API или Панели мониторинга Центра партнеров в полночь по UTC.</span><span class="sxs-lookup"><span data-stu-id="55008-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="55008-108">**Период выставления счетов**. Период выставления счетов определяется как за календарный месяц, например 1.10–31.10 или 1.11–30.11.</span><span class="sxs-lookup"><span data-stu-id="55008-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="55008-109">**Периоды начисления оплаты**: Плата будет начисляться за календарный месяц.</span><span class="sxs-lookup"><span data-stu-id="55008-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="55008-110">Например, если партнер, выставляющий счета, добавляет службы Azure через план Azure 15.10, а клиент начинает использование служб Azure с 15.10, то партнер получит счет-фактуру или файл выверки 8.11 по использованию клиентом служб в течение периода обслуживания 15.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="55008-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="55008-111">Счет за следующий месяц, который будет создан на 8.12, содержит все расходы за период обслуживания 1.11–31.11.</span><span class="sxs-lookup"><span data-stu-id="55008-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="55008-112">**Срок оплаты счета-фактуры**. В течение 60 дней.</span><span class="sxs-lookup"><span data-stu-id="55008-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="55008-113">**Валюта счета**. Партнеры будут по-прежнему получать счета-фактуры в назначенной валюте страны клиента.</span><span class="sxs-lookup"><span data-stu-id="55008-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="55008-114">Например, если партнер в Ирландии выставляет счета клиентам в Великобритании, Норвегии и Германии, то партнер будет получать счет-фактуру или файл выверки в фунтах стерлингов (GBP), норвежских кронах (NOK) и евро (EUR).</span><span class="sxs-lookup"><span data-stu-id="55008-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="55008-115">**Поощрения для партнеров**. Оплачено 45 дней с конца месяца счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="55008-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="55008-116">Доступ к своим счетам-фактурам и файлам выверки</span><span class="sxs-lookup"><span data-stu-id="55008-116">Access your invoices and recon files</span></span>

<span data-ttu-id="55008-117">Глобальный администратор или администратор выставления счетов для вашей компании получат электронное сообщение, когда счет-фактура будет готов к просмотру.</span><span class="sxs-lookup"><span data-stu-id="55008-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="55008-118">**Доступ к файлу выверки и счету-фактуре**</span><span class="sxs-lookup"><span data-stu-id="55008-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="55008-119">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="55008-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="55008-120">В меню Центра партнеров выберите **Billing** (Выставление счетов).</span><span class="sxs-lookup"><span data-stu-id="55008-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="55008-121">Выберите вкладку для параметра **Calendar-based** (Календарный) и валют, которые вас интересуют.</span><span class="sxs-lookup"><span data-stu-id="55008-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![выставление счетов](images/azure/billing1.png)

4. <span data-ttu-id="55008-123">Выберите **Invoice and Recon file** (Счет-фактура и файл выверки).</span><span class="sxs-lookup"><span data-stu-id="55008-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="55008-124">Чтобы просмотреть предыдущие счета-фактуры и файлы выверки, разверните строку "История счетов" ниже.</span><span class="sxs-lookup"><span data-stu-id="55008-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="55008-125">Чтение счета-фактуры</span><span class="sxs-lookup"><span data-stu-id="55008-125">Read the invoice</span></span>

1. <span data-ttu-id="55008-126">Счет будет доступен не позднее 8 числа каждого месяца.</span><span class="sxs-lookup"><span data-stu-id="55008-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="55008-127">У партнеров есть 60 дней для предъявления платежа.</span><span class="sxs-lookup"><span data-stu-id="55008-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="55008-128">Расчетный период охватывает заданный календарный месяц, например 1.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="55008-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="55008-129">Плата взимается в процентах от корректировок (сумма — это доля от "Партнерского кредита на управляемые службы").</span><span class="sxs-lookup"><span data-stu-id="55008-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="55008-130">Чтобы получить дополнительные сведения о выставлении счетов, см. файл выверки счета-фактуры и файл ежедневного использования.</span><span class="sxs-lookup"><span data-stu-id="55008-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![счет-фактура](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="55008-132">Чтение файла выверки</span><span class="sxs-lookup"><span data-stu-id="55008-132">Read the recon file</span></span>

1. <span data-ttu-id="55008-133">Каждый счетчик подписки Azure может иметь до двух строк выставления счетов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="55008-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="55008-134">Если счетчик для любого типа скидки или кредита (например, для скидок уровня 1 или партнерского кредита для управляемых служб) действует на протяжении всего календарного месяца, то файл выверки будет содержать только одну строку выставления счета.</span><span class="sxs-lookup"><span data-stu-id="55008-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="55008-135">Столбец **PriceAdjusmentDescription**  будет содержать скидку или полученный кредит; эффективная цена за единицу будет считаться розничной ценой за вычетом партнерского кредита или любых других скидок.</span><span class="sxs-lookup"><span data-stu-id="55008-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="55008-136">Если в течение всего календарного месяца счетчик не был назначен для партнерского кредита для управляемых служб, то файл выверки будет содержать только одну строку выставления счета, а действительная цена за единицу будет розничной ценой (которая будет ценой за единицу).</span><span class="sxs-lookup"><span data-stu-id="55008-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="55008-137">Если счетчик назначен для **Партнерского кредита для управляемых служб** за часть месяца, файл выверки будет содержать две строки выставления счета.</span><span class="sxs-lookup"><span data-stu-id="55008-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="55008-138">Одна строка будет представлять дни, в которых счетчик действует, а вторая — дни, в которые счетчик не применяется.</span><span class="sxs-lookup"><span data-stu-id="55008-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="55008-139">Чтение файла ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="55008-139">Read the daily usage file</span></span>

- <span data-ttu-id="55008-140">Счетчики подписки в плане Azure оцениваются и распределяются ежедневно.</span><span class="sxs-lookup"><span data-stu-id="55008-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="55008-141">**Партнерский кредит для управляемых служб** определяется и применяется ежедневно.</span><span class="sxs-lookup"><span data-stu-id="55008-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="55008-142">Каждый счетчик подписки будет иметь строку для каждого дня месяца, когда служба использовалась.</span><span class="sxs-lookup"><span data-stu-id="55008-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="55008-143">См. пример ниже.</span><span class="sxs-lookup"><span data-stu-id="55008-143">In the example below:</span></span>

  - <span data-ttu-id="55008-144">Счетчик действует для **Партнерского кредита для управляемых служб** за период 1.07–3.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="55008-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="55008-145">Счетчик не действует для **Партнерского кредита для управляемых служб** за период 4.07–7.07 (обратите внимание, что цена за единицу является розничной ценой).</span><span class="sxs-lookup"><span data-stu-id="55008-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="55008-146">Счетчик действует для **Партнерского кредита для управляемых служб** за период 8.07–31.07 (обратите внимание, что цена за единицу является розничной ценой за вычетом партнерского кредита).</span><span class="sxs-lookup"><span data-stu-id="55008-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="55008-148">Счет-фактура в валюте клиента</span><span class="sxs-lookup"><span data-stu-id="55008-148">Invoice in customer currency</span></span> 

<span data-ttu-id="55008-149">Плата за службы Azure в плане Azure будет взиматься в долларах США (USD) и оплачиваться в валюте назначенной страны клиента.</span><span class="sxs-lookup"><span data-stu-id="55008-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="55008-150">Если счет выставляется не в долларах США (USD), то на последней странице счета будет указан используемый курс валют.</span><span class="sxs-lookup"><span data-stu-id="55008-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="55008-151">Курс валют определяется за месяц и применяется к следующему счету.</span><span class="sxs-lookup"><span data-stu-id="55008-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="55008-152">Полный список валют см. в [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V) (Таблица валют клиентов и доступности новых коммерческих предложений в разных странах).</span><span class="sxs-lookup"><span data-stu-id="55008-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="55008-153">Корпорация Майкрософт будет использовать данные [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) при определении курса валют, используемого для определения и конвертации валюты счета.</span><span class="sxs-lookup"><span data-stu-id="55008-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="55008-154">Курс валют будет обновляться и доступен за день до первого дня месяца, для которого он применяется.</span><span class="sxs-lookup"><span data-stu-id="55008-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="55008-155">**Пример**:  Плата за использование в период обслуживания с 1 августа до 31 августа будет взиматься по курсу валют, опубликованному 1 августа.</span><span class="sxs-lookup"><span data-stu-id="55008-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="55008-156">Эта плата отобразится в сентябрьском счете-фактуре, и курс валют будет указан на последней странице счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="55008-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="55008-157">Пользователи-арендаторы партнера будут по-прежнему видеть связанные с ролью сведения обо всех клиентах и заказах, независимо от валюты выставления счета.</span><span class="sxs-lookup"><span data-stu-id="55008-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="55008-158">Кроме того, такой пользователь сможет видеть все счета во всех валютах.</span><span class="sxs-lookup"><span data-stu-id="55008-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="55008-159">Резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="55008-159">Azure reservations</span></span> 

<span data-ttu-id="55008-160">В случае приобретения [резервирования Azure](https://docs.microsoft.com/partner-center/azure-reservations) с помощью плана Azure, сначала можно будет выбрать разовое выставление счета в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="55008-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="55008-161">Ежемесячное выставление счетов доступно на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="55008-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="55008-162">Ежемесячное выставление счетов будет доступно в Центре партнеров позже.</span><span class="sxs-lookup"><span data-stu-id="55008-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="55008-163">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="55008-163">Azure cost management</span></span> 

<span data-ttu-id="55008-164">Средства Azure Cost Management помогут организациям визуализировать и оптимизировать свои затраты в Microsoft Azure и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="55008-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="55008-165">Этот компонент будет доступен на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="55008-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="55008-166">У партнеров будет постоянно доступное решение с низкой задержкой, в котором предусмотрены следующие функции.</span><span class="sxs-lookup"><span data-stu-id="55008-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="55008-167">Расширенные средства анализа и оповещения о бюджете</span><span class="sxs-lookup"><span data-stu-id="55008-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="55008-168">Интерфейсы API и соединители Power BI</span><span class="sxs-lookup"><span data-stu-id="55008-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="55008-169">Представление с несколькими клиентами</span><span class="sxs-lookup"><span data-stu-id="55008-169">Multi-customer view</span></span> 
- <span data-ttu-id="55008-170">Бесплатное управление затратами на Azure</span><span class="sxs-lookup"><span data-stu-id="55008-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="55008-171">Расширение ролей и пользователей</span><span class="sxs-lookup"><span data-stu-id="55008-171">Expansion of roles/users</span></span> 

<span data-ttu-id="55008-172">Дополнительные сведения об этой функции, которая стала доступна для корпоративных соглашений в феврале 2019 г., см. в разделе [Azure Cost Management](https://azure.microsoft.com/services/cost-management).</span><span class="sxs-lookup"><span data-stu-id="55008-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="55008-173">Эта возможность доступна только в службах Azure, приобретенных в рамках этого нового коммерческого предложения Azure в CSP.</span><span class="sxs-lookup"><span data-stu-id="55008-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="55008-174">Расходы на Azure</span><span class="sxs-lookup"><span data-stu-id="55008-174">Azure spending</span></span> 

<span data-ttu-id="55008-175">Средство управления затратами Azure будет доступно в Центре партнеров для новых коммерческих предложений в CSP.</span><span class="sxs-lookup"><span data-stu-id="55008-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="55008-176">После применения эта возможность позволит партнерам видеть:</span><span class="sxs-lookup"><span data-stu-id="55008-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="55008-177">итоговый бюджет клиента;</span><span class="sxs-lookup"><span data-stu-id="55008-177">Total budget on a customer</span></span> 
- <span data-ttu-id="55008-178">общую оценку расходов на существующий план Azure;</span><span class="sxs-lookup"><span data-stu-id="55008-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="55008-179">процент использования служб клиентами за каждый расчетный период.</span><span class="sxs-lookup"><span data-stu-id="55008-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="55008-180">Так как модель выставления счетов для служб Azure в плане Azure — это использование служб после оплаты, чтобы избежать выставления счета, размер которого превышает ожидаемый, партнеры могут формировать месячный бюджет и следить за ростом использования служб.</span><span class="sxs-lookup"><span data-stu-id="55008-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="55008-181">Бюджет может быть применен к одному клиенту или нескольким клиентам одновременно.</span><span class="sxs-lookup"><span data-stu-id="55008-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Расходы на Azure](images/azure/azurespend.png)

<span data-ttu-id="55008-183">**Дополнительные сведения**</span><span class="sxs-lookup"><span data-stu-id="55008-183">**For more information**</span></span>

-  <span data-ttu-id="55008-184">Схема расчета партнерского кредита указана в прейскуранте, доступном на Панели мониторинга Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="55008-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="55008-185">Приобретение плана Azure</span><span class="sxs-lookup"><span data-stu-id="55008-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="55008-186">Прейскурант для новой коммерческой модели в CSP</span><span class="sxs-lookup"><span data-stu-id="55008-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
