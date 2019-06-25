---
title: Использование файлов выверки | Центр партнеров
ms.topic: article
ms.date: 03/15/2019
description: Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fca9897720412a77ac39c86ba31db411c58c2cb0
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343471"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="96104-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="96104-103">Use the reconciliation files</span></span>

<span data-ttu-id="96104-104">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="96104-104">**Applies to**</span></span>

-  <span data-ttu-id="96104-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="96104-105">Partner Center</span></span>
-  <span data-ttu-id="96104-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="96104-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="96104-107">Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="96104-108">Эти сведения включают оплаты за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="96104-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="96104-109">Особенности форматирования</span><span class="sxs-lookup"><span data-stu-id="96104-109">Formatting issues</span></span>

<span data-ttu-id="96104-110">Иногда проверка файла возможно, проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="96104-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="96104-111">(Это может произойти, например, если не используется языковой стандарт EN-US.) Выполните следующие действия, чтобы устранить эти проблемы.</span><span class="sxs-lookup"><span data-stu-id="96104-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="96104-112">Откройте CSV-файл в Excel и выберите первый столбец.</span><span class="sxs-lookup"><span data-stu-id="96104-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="96104-113">На ленте выберите <strong>данных</strong>, а затем выберите <strong>текст по столбцам</strong>.</span><span class="sxs-lookup"><span data-stu-id="96104-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="96104-114">В преобразовать в столбцы мастера выберите <strong>с разделителями тип файла</strong>, а затем выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="96104-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="96104-115">В поле разделителей групп разрядов выберите <strong>разделителями</strong>.</span><span class="sxs-lookup"><span data-stu-id="96104-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="96104-116">Если <strong>вкладке</strong> является еще выбран, можно оставить его.</span><span class="sxs-lookup"><span data-stu-id="96104-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="96104-117">Выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="96104-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="96104-118">В поле формата столбца данных, выберите <strong>даты: MDY (МДГ)</strong>, а затем выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="96104-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="96104-119">В поле формата столбца данных, выберите <strong>текст</strong> для всех сумма столбцов, а затем выберите <strong>Готово</strong>.</span><span class="sxs-lookup"><span data-stu-id="96104-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="96104-120">Загрузка больших файлов разведывательную</span><span class="sxs-lookup"><span data-stu-id="96104-120">Downloading a large recon file</span></span>

<span data-ttu-id="96104-121">Проверка файлов может стать очень большой и иногда трудно загрузки.</span><span class="sxs-lookup"><span data-stu-id="96104-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="96104-122">Сценарий PowerShell для загрузки больших файлов разведывательную, см. в разделе [позиций в строках счета Get](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="96104-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="96104-123">Детализировать партнером</span><span class="sxs-lookup"><span data-stu-id="96104-123">Itemize by partner</span></span>


<span data-ttu-id="96104-124">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="96104-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="96104-125">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="96104-125">MPN ID</span></span></th>
<th><span data-ttu-id="96104-126">Описание</span><span class="sxs-lookup"><span data-stu-id="96104-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="96104-127">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="96104-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="96104-128">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="96104-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-129">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="96104-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="96104-130">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="96104-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="96104-131">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="96104-132">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="96104-133">Просмотр позитивную или обновление торгового посредника, в меню центра партнеров выберите <strong>клиентов</strong>, затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="96104-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="96104-134">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="96104-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="96104-135">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="96104-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="96104-136">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="96104-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="96104-137">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="96104-138">Если партнер CSP удаляет идентификатор торгового посредника, это значение будет равно -1.</span><span class="sxs-lookup"><span data-stu-id="96104-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="96104-139">Поля файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="96104-139">License-based file fields</span></span>


<span data-ttu-id="96104-140">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="96104-141"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="96104-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="96104-142"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="96104-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="96104-143"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="96104-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="96104-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="96104-145">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="96104-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="96104-146">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="96104-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="96104-147">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="96104-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="96104-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="96104-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="96104-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="96104-150">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="96104-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="96104-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="96104-152">OrderID</span></span></td>
<td><p><span data-ttu-id="96104-153">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="96104-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="96104-154">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="96104-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="96104-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="96104-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="96104-157">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="96104-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="96104-158">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="96104-159">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="96104-160">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="96104-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="96104-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="96104-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="96104-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="96104-163">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="96104-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="96104-164">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="96104-165">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="96104-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="96104-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="96104-167">OfferID</span></span></td>
<td><p><span data-ttu-id="96104-168">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="96104-168">Unique offer ID.</span></span> <span data-ttu-id="96104-169">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="96104-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="96104-170"><b>Примечание</b>. Это значение не соответствует Идентификатору предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="96104-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="96104-171">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="96104-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="96104-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="96104-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="96104-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="96104-174">Уникальный идентификатор длительного предложения как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="96104-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="96104-175"><b>Примечание</b>. Это значение совпадает с Идентификатором предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="96104-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="96104-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="96104-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="96104-177">OfferName</span></span></td>
<td><p><span data-ttu-id="96104-178">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="96104-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="96104-179">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="96104-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="96104-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="96104-181">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="96104-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="96104-182">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="96104-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="96104-183">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="96104-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="96104-184">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="96104-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="96104-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="96104-186">Дата окончания подписки: 12 месяцев + x дней после даты начала (чтобы соответствовать выставления счетов даты партнера) или 12 месяцев с даты продления.</span><span class="sxs-lookup"><span data-stu-id="96104-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="96104-187">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="96104-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="96104-188">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="96104-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="96104-189">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="96104-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="96104-190">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="96104-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="96104-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="96104-192">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="96104-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="96104-193">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="96104-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="96104-194">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="96104-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="96104-195">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="96104-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="96104-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="96104-197">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="96104-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="96104-198">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="96104-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="96104-199">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="96104-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="96104-200">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="96104-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="96104-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="96104-202">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="96104-202">The type of charge or adjustment.</span></span> <span data-ttu-id="96104-203">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="96104-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="96104-204">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="96104-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="96104-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="96104-206">Цена за рабочее место, опубликованное в прайс-листе во время покупки.</span><span class="sxs-lookup"><span data-stu-id="96104-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="96104-207">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="96104-208">6,82</span><span class="sxs-lookup"><span data-stu-id="96104-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-209">Количество</span><span class="sxs-lookup"><span data-stu-id="96104-209">Quantity</span></span></td>
<td><p><span data-ttu-id="96104-210">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="96104-210">Number of seats.</span></span> <span data-ttu-id="96104-211">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="96104-212">2</span><span class="sxs-lookup"><span data-stu-id="96104-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-213">Сумма</span><span class="sxs-lookup"><span data-stu-id="96104-213">Amount</span></span></td>
<td><p><span data-ttu-id="96104-214">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="96104-214">Total of price for quantity.</span></span> <span data-ttu-id="96104-215">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="96104-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="96104-216">13,32</span><span class="sxs-lookup"><span data-stu-id="96104-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="96104-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="96104-218">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="96104-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="96104-219">IUR или новые подписки, на которые распространяются вознаграждения, будут также содержать сумму скидки в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="96104-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="96104-220">2,32</span><span class="sxs-lookup"><span data-stu-id="96104-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-221">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="96104-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="96104-222">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="96104-222">Total before tax.</span></span> <span data-ttu-id="96104-223">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="96104-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="96104-224">11</span><span class="sxs-lookup"><span data-stu-id="96104-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-225">Налог</span><span class="sxs-lookup"><span data-stu-id="96104-225">Tax</span></span></td>
<td><p><span data-ttu-id="96104-226">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="96104-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="96104-227">0</span><span class="sxs-lookup"><span data-stu-id="96104-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="96104-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="96104-229">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="96104-229">Total after tax.</span></span> <span data-ttu-id="96104-230">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="96104-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="96104-231">11</span><span class="sxs-lookup"><span data-stu-id="96104-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-232">Валюта</span><span class="sxs-lookup"><span data-stu-id="96104-232">Currency</span></span></td>
<td><p><span data-ttu-id="96104-233">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="96104-233">Currency type.</span></span> <span data-ttu-id="96104-234">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="96104-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="96104-235">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="96104-236">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="96104-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="96104-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="96104-238">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="96104-239">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="96104-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="96104-240">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="96104-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="96104-241">MPNID</span></span></td>
<td><p><span data-ttu-id="96104-242">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="96104-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="96104-243">4390934</span><span class="sxs-lookup"><span data-stu-id="96104-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="96104-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="96104-245">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="96104-246">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="96104-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="96104-247">4390934</span><span class="sxs-lookup"><span data-stu-id="96104-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="96104-248">DomainName</span></span></td>
<td><p><span data-ttu-id="96104-249">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="96104-250">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="96104-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="96104-251">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="96104-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="96104-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="96104-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="96104-254">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-254">Subscription nickname.</span></span> <span data-ttu-id="96104-255">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="96104-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="96104-256">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="96104-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="96104-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="96104-258">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="96104-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="96104-259">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="96104-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="96104-260">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="96104-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="96104-261">Поля файла на основе использования</span><span class="sxs-lookup"><span data-stu-id="96104-261">Usage-based file fields</span></span>


<span data-ttu-id="96104-262">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="96104-263">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="96104-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="96104-264"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="96104-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="96104-265"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="96104-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="96104-266"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="96104-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="96104-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="96104-268">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="96104-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="96104-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="96104-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="96104-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="96104-271">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="96104-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="96104-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="96104-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="96104-274">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="96104-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="96104-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="96104-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="96104-277">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="96104-278">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="96104-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="96104-279">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="96104-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="96104-280">MPNID</span></span></td>
<td><p><span data-ttu-id="96104-281">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="96104-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="96104-282">4390934</span><span class="sxs-lookup"><span data-stu-id="96104-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="96104-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="96104-284">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="96104-285">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="96104-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="96104-286">4390934</span><span class="sxs-lookup"><span data-stu-id="96104-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="96104-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="96104-288">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="96104-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="96104-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="96104-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="96104-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="96104-291">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="96104-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="96104-292">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="96104-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="96104-293">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="96104-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="96104-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="96104-295">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="96104-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="96104-296">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="96104-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="96104-297">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="96104-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="96104-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="96104-299">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="96104-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="96104-300">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="96104-301">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="96104-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="96104-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="96104-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="96104-304">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="96104-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="96104-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="96104-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="96104-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="96104-307">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="96104-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="96104-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="96104-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="96104-309">OrderID</span></span></td>
<td><p><span data-ttu-id="96104-310">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="96104-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="96104-311">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="96104-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="96104-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="96104-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="96104-314">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="96104-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="96104-315">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="96104-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="96104-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="96104-317">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="96104-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="96104-318">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="96104-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="96104-319">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="96104-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="96104-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="96104-321">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="96104-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="96104-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="96104-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-323">Resource Name</span><span class="sxs-lookup"><span data-stu-id="96104-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="96104-324">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="96104-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="96104-325">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="96104-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="96104-326">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="96104-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-327">Region</span><span class="sxs-lookup"><span data-stu-id="96104-327">Region</span></span></td>
<td><p><span data-ttu-id="96104-328">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="96104-328">The region the usage applies to.</span></span> <span data-ttu-id="96104-329">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="96104-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="96104-330">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="96104-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-331">номер SKU</span><span class="sxs-lookup"><span data-stu-id="96104-331">SKU</span></span></td>
<td><p><span data-ttu-id="96104-332">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="96104-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="96104-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="96104-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="96104-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="96104-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="96104-335">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="96104-336">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним — другой.</span><span class="sxs-lookup"><span data-stu-id="96104-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="96104-337">1</span><span class="sxs-lookup"><span data-stu-id="96104-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="96104-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="96104-339">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="96104-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="96104-340">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="96104-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="96104-341">11</span><span class="sxs-lookup"><span data-stu-id="96104-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="96104-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="96104-343">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="96104-343">Units included as part of the offer.</span></span> <span data-ttu-id="96104-344">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="96104-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="96104-345">0</span><span class="sxs-lookup"><span data-stu-id="96104-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="96104-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="96104-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="96104-347">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="96104-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="96104-348">Равняется разнице значений полей ConsumedQuantity и IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="96104-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="96104-349">11</span><span class="sxs-lookup"><span data-stu-id="96104-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="96104-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="96104-351">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="96104-352">0,0808 долл. США</span><span class="sxs-lookup"><span data-stu-id="96104-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="96104-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="96104-354">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="96104-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="96104-355">0,085 долл. США</span><span class="sxs-lookup"><span data-stu-id="96104-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="96104-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="96104-357">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="96104-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="96104-358">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="96104-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="96104-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="96104-360">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="96104-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="96104-361">0,93 долл. США</span><span class="sxs-lookup"><span data-stu-id="96104-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-362">Валюта</span><span class="sxs-lookup"><span data-stu-id="96104-362">Currency</span></span></td>
<td><p><span data-ttu-id="96104-363">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="96104-363">Currency type.</span></span> <span data-ttu-id="96104-364">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="96104-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="96104-365">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="96104-366">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="96104-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="96104-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="96104-368">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="96104-368">Pretax price per unit.</span></span> <span data-ttu-id="96104-369">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="96104-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="96104-370">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="96104-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="96104-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="96104-372">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="96104-372">Post tax price per unit.</span></span> <span data-ttu-id="96104-373">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="96104-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="96104-374">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="96104-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="96104-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="96104-376">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="96104-376">The type of charge or adjustment.</span></span> <span data-ttu-id="96104-377">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="96104-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="96104-378">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="96104-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="96104-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="96104-380">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="96104-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="96104-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="96104-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="96104-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="96104-383">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="96104-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="96104-384">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="96104-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="96104-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="96104-386">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="96104-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="96104-387">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="96104-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-388">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="96104-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="96104-389">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="96104-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="96104-390">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="96104-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="96104-391">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="96104-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="96104-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="96104-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="96104-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="96104-394">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="96104-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="96104-395">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="96104-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-396">Проект</span><span class="sxs-lookup"><span data-stu-id="96104-396">Project</span></span></td>
<td><p><span data-ttu-id="96104-397">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="96104-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="96104-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="96104-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="96104-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="96104-400">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="96104-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="96104-401">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="96104-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="96104-402">Если имеется 25 пакетов подключений служебной шины подготовлено, и вы использовалось 1 в течение этого дня, инструкцию ежедневное использование за этот день означает «25 подключений / 30 дней — использовано: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="96104-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="96104-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="96104-404">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="96104-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="96104-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="96104-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="96104-406">DomainName</span></span></td>
<td><p><span data-ttu-id="96104-407">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="96104-408">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="96104-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="96104-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="96104-410">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="96104-410">Unit</span></span></td>
<td><p><span data-ttu-id="96104-411">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="96104-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="96104-412">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="96104-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="96104-413">Файл одноразовые и повторяющиеся поля</span><span class="sxs-lookup"><span data-stu-id="96104-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="96104-414">Column</span><span class="sxs-lookup"><span data-stu-id="96104-414">Column</span></span></th>
<th><span data-ttu-id="96104-415">Описание</span><span class="sxs-lookup"><span data-stu-id="96104-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="96104-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="96104-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="96104-417">Уникальный идентификатор клиента Microsoft Azure Active Directory для конкретной сущности выставления счетов, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="96104-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="96104-418">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="96104-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="96104-419">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="96104-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-420">Идентификатор клиента</span><span class="sxs-lookup"><span data-stu-id="96104-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="96104-421">Уникальный Microsoft Azure Active Directory идентификатор клиента, в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-422">Customer Name (Имя клиента)</span><span class="sxs-lookup"><span data-stu-id="96104-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="96104-423">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="96104-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="96104-425">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="96104-426">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="96104-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="96104-427">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-428">Страна или регион клиента</span><span class="sxs-lookup"><span data-stu-id="96104-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="96104-429">Страна или регион, где находится клиент.</span><span class="sxs-lookup"><span data-stu-id="96104-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-430">Номер счета</span><span class="sxs-lookup"><span data-stu-id="96104-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="96104-431">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="96104-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="96104-432">MpnId</span></span></td>
<td><p><span data-ttu-id="96104-433">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="96104-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-434">MpnId торгового посредника</span><span class="sxs-lookup"><span data-stu-id="96104-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="96104-435">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-436">Идентификатор заказа</span><span class="sxs-lookup"><span data-stu-id="96104-436">Order ID</span></span></td>
<td><p><span data-ttu-id="96104-437">Уникальный идентификатор заказа на платформе Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="96104-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="96104-438">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-439">Дата заказа</span><span class="sxs-lookup"><span data-stu-id="96104-439">Order date</span></span></td>
<td><p><span data-ttu-id="96104-440">Дата размещения заказа.</span><span class="sxs-lookup"><span data-stu-id="96104-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-441">ProductID</span><span class="sxs-lookup"><span data-stu-id="96104-441">ProductId</span></span></td>
<td><p><span data-ttu-id="96104-442">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="96104-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="96104-443">SkuId</span></span></td>
<td><p><span data-ttu-id="96104-444">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="96104-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="96104-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="96104-446">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="96104-446">The ID for a particular Availability.</span></span> <span data-ttu-id="96104-447">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="96104-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-448">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="96104-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="96104-449">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="96104-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-450">название продукта;</span><span class="sxs-lookup"><span data-stu-id="96104-450">Product name</span></span></td>
<td><p><span data-ttu-id="96104-451">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="96104-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="96104-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="96104-453">Имя издателя продукта.</span><span class="sxs-lookup"><span data-stu-id="96104-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="96104-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="96104-455">Уникальный идентификатор для данного издателя.</span><span class="sxs-lookup"><span data-stu-id="96104-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-456">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="96104-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="96104-457">Понятное имя подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-458">Код подписки</span><span class="sxs-lookup"><span data-stu-id="96104-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="96104-459">Уникальный идентификатор для подписки на платформу Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="96104-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="96104-460">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="96104-461">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="96104-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="96104-463">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="96104-463">Start day of the charges.</span></span> <span data-ttu-id="96104-464">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="96104-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="96104-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="96104-466">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="96104-466">End day of the charges.</span></span> <span data-ttu-id="96104-467">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="96104-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-468">Термин и Billingcycle</span><span class="sxs-lookup"><span data-stu-id="96104-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="96104-469">Продолжительность срока и цикла выставления счетов за покупки.</span><span class="sxs-lookup"><span data-stu-id="96104-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="96104-470">Например «1 год, месяц.»</span><span class="sxs-lookup"><span data-stu-id="96104-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-471">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="96104-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="96104-472">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="96104-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-473">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="96104-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="96104-474">Цена, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="96104-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="96104-475">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-476">Эффективное модульное цена</span><span class="sxs-lookup"><span data-stu-id="96104-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="96104-477">Цена за единицу после изменения.</span><span class="sxs-lookup"><span data-stu-id="96104-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-478">Количество</span><span class="sxs-lookup"><span data-stu-id="96104-478">Quantity</span></span></td>
<td><p><span data-ttu-id="96104-479">Число единиц.</span><span class="sxs-lookup"><span data-stu-id="96104-479">Number of units.</span></span> <span data-ttu-id="96104-480">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-481">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="96104-481">Unit type</span></span></td>
<td><p><span data-ttu-id="96104-482">Тип приобретенная единица.</span><span class="sxs-lookup"><span data-stu-id="96104-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="96104-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="96104-484">Объяснение применяемой скидки.</span><span class="sxs-lookup"><span data-stu-id="96104-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-485">Итого</span><span class="sxs-lookup"><span data-stu-id="96104-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="96104-486">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="96104-486">Total before tax.</span></span> <span data-ttu-id="96104-487">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="96104-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-488">Общая сумма налога</span><span class="sxs-lookup"><span data-stu-id="96104-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="96104-489">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="96104-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-490">Total (Всего)</span><span class="sxs-lookup"><span data-stu-id="96104-490">Total</span></span></td>
<td><p><span data-ttu-id="96104-491">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="96104-491">Total after tax.</span></span> <span data-ttu-id="96104-492">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="96104-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-493">Валюта</span><span class="sxs-lookup"><span data-stu-id="96104-493">Currency</span></span></td>
<td><p><span data-ttu-id="96104-494">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="96104-494">Currency type.</span></span> <span data-ttu-id="96104-495">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="96104-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="96104-496">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-497">Альтернативного имени пользователя</span><span class="sxs-lookup"><span data-stu-id="96104-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="96104-498">Альтернативный идентификатор с идентификатором заказа.</span><span class="sxs-lookup"><span data-stu-id="96104-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="96104-499">Поля файла оценкой ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="96104-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="96104-500">Column</span><span class="sxs-lookup"><span data-stu-id="96104-500">Column</span></span></th>
<th><span data-ttu-id="96104-501">Описание</span><span class="sxs-lookup"><span data-stu-id="96104-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="96104-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="96104-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="96104-503">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="96104-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="96104-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="96104-505">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="96104-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="96104-507">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="96104-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="96104-509">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="96104-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="96104-510">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="96104-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="96104-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="96104-512">Имя домена клиента.</span><span class="sxs-lookup"><span data-stu-id="96104-512">The customer’s domain name.</span></span> <span data-ttu-id="96104-513">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="96104-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-514">Страна или регион клиента</span><span class="sxs-lookup"><span data-stu-id="96104-514">Customer country</span></span></td>
<td><p><span data-ttu-id="96104-515">Страна или регион, где находится клиент.</span><span class="sxs-lookup"><span data-stu-id="96104-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="96104-516">MPNID</span></span></td>
<td><p><span data-ttu-id="96104-517">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="96104-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-518">Торговый посредник MPNID</span><span class="sxs-lookup"><span data-stu-id="96104-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="96104-519">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="96104-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="96104-520">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="96104-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="96104-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="96104-522">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="96104-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="96104-523">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="96104-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-524">ProductID</span><span class="sxs-lookup"><span data-stu-id="96104-524">ProductId</span></span></td>
<td><p><span data-ttu-id="96104-525">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="96104-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="96104-526">SkuId</span></span></td>
<td><p><span data-ttu-id="96104-527">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="96104-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="96104-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="96104-529">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="96104-529">The ID for a particular Availability.</span></span> <span data-ttu-id="96104-530">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="96104-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-531">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="96104-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="96104-532">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="96104-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="96104-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="96104-534">Имя издателя.</span><span class="sxs-lookup"><span data-stu-id="96104-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="96104-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="96104-536">Идентификатор издателя, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="96104-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="96104-537">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="96104-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="96104-538">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="96104-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="96104-539">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="96104-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="96104-540">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="96104-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-541">Код подписки</span><span class="sxs-lookup"><span data-stu-id="96104-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="96104-542">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="96104-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="96104-543">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="96104-544">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="96104-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="96104-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="96104-546">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="96104-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="96104-547">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="96104-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="96104-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="96104-549">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="96104-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="96104-550">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="96104-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-551">Дата использования</span><span class="sxs-lookup"><span data-stu-id="96104-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="96104-552">Дата использования службы.</span><span class="sxs-lookup"><span data-stu-id="96104-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-553">Индикатор типа</span><span class="sxs-lookup"><span data-stu-id="96104-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="96104-554">Тип единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="96104-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-555">Категория счетчика</span><span class="sxs-lookup"><span data-stu-id="96104-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="96104-556">Служба верхнего уровня для использования.</span><span class="sxs-lookup"><span data-stu-id="96104-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-557">Идентификатор счетчика</span><span class="sxs-lookup"><span data-stu-id="96104-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="96104-558">Идентификатор для использования средства измерения.</span><span class="sxs-lookup"><span data-stu-id="96104-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-559">Подкатегория измерения</span><span class="sxs-lookup"><span data-stu-id="96104-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="96104-560">Тип службы Azure, которые могут повлиять на скорость.</span><span class="sxs-lookup"><span data-stu-id="96104-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-561">Имя единицы измерения</span><span class="sxs-lookup"><span data-stu-id="96104-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="96104-562">Единица измерения для использованного средства измерения.</span><span class="sxs-lookup"><span data-stu-id="96104-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-563">Регион счетчика</span><span class="sxs-lookup"><span data-stu-id="96104-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="96104-564">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="96104-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-565">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="96104-565">Unit</span></span></td>
<td><p><span data-ttu-id="96104-566">Единица имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="96104-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-567">Использованное количество</span><span class="sxs-lookup"><span data-stu-id="96104-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="96104-568">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="96104-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="96104-569">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="96104-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-570">Расположение ресурса</span><span class="sxs-lookup"><span data-stu-id="96104-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="96104-571">Центр обработки данных, где выполняется средства измерения.</span><span class="sxs-lookup"><span data-stu-id="96104-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-572">Используемой службы</span><span class="sxs-lookup"><span data-stu-id="96104-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="96104-573">Используемая служба платформы Azure.</span><span class="sxs-lookup"><span data-stu-id="96104-573">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-574">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="96104-574">Resource Group</span></span></td>
<td><p><span data-ttu-id="96104-575">Группа ресурсов, в которой выполняется развернутое средство измерения.</span><span class="sxs-lookup"><span data-stu-id="96104-575">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-576">URI ресурса</span><span class="sxs-lookup"><span data-stu-id="96104-576">Resource URI</span></span></td>
<td><p><span data-ttu-id="96104-577">URI ресурса, который используется.</span><span class="sxs-lookup"><span data-stu-id="96104-577">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-578">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="96104-578">Charge type</span></span></td>
<td><p><span data-ttu-id="96104-579">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="96104-579">The type of charge or adjustment.</span></span> <span data-ttu-id="96104-580">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="96104-580">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-581">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="96104-581">Unit price</span></span></td>
<td><p><span data-ttu-id="96104-582">Цена за лицензии, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="96104-582">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="96104-583">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-584">Количество</span><span class="sxs-lookup"><span data-stu-id="96104-584">Quantity</span></span></td>
<td><p><span data-ttu-id="96104-585">Количество лицензий.</span><span class="sxs-lookup"><span data-stu-id="96104-585">Number of licenses.</span></span> <span data-ttu-id="96104-586">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-586">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-587">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="96104-587">Unit type</span></span></td>
<td><p><span data-ttu-id="96104-588">Тип единицы измерения единицы измеряется объем использования.</span><span class="sxs-lookup"><span data-stu-id="96104-588">The type of unit the meter is charged in.</span></span> <span data-ttu-id="96104-589">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="96104-589">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-590">Налог pre выставления счетов</span><span class="sxs-lookup"><span data-stu-id="96104-590">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="96104-591">Общая сумма до налогов.</span><span class="sxs-lookup"><span data-stu-id="96104-591">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-592">Валюта для выставления счетов</span><span class="sxs-lookup"><span data-stu-id="96104-592">Billing currency</span></span></td>
<td><p><span data-ttu-id="96104-593">Валюта в географическом регионе клиента</span><span class="sxs-lookup"><span data-stu-id="96104-593">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-594">Цены до выплаты налогов всего</span><span class="sxs-lookup"><span data-stu-id="96104-594">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="96104-595">Цены до налогов.</span><span class="sxs-lookup"><span data-stu-id="96104-595">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-596">Цены на валюту</span><span class="sxs-lookup"><span data-stu-id="96104-596">Pricing currency</span></span></td>
<td><p><span data-ttu-id="96104-597">Валюта, в прайс-листа.</span><span class="sxs-lookup"><span data-stu-id="96104-597">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-598">Сведения о службе 1</span><span class="sxs-lookup"><span data-stu-id="96104-598">Service Info 1</span></span></td>
<td><p><span data-ttu-id="96104-599">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="96104-599">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-600">Сведения о службе 2</span><span class="sxs-lookup"><span data-stu-id="96104-600">Service Info 2</span></span></td>
<td><p><span data-ttu-id="96104-601">Устаревшее поле, в которое записываются необязательные метаданные службы.</span><span class="sxs-lookup"><span data-stu-id="96104-601">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="96104-602">Tags</span><span class="sxs-lookup"><span data-stu-id="96104-602">Tags</span></span></td>
<td><p><span data-ttu-id="96104-603">Теги, присваиваемый средству измерения в порядке для группировки записей выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="96104-603">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="96104-604">Например можно использовать теги для распределения затрат по отделу, который использует данное средство измерения.</span><span class="sxs-lookup"><span data-stu-id="96104-604">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="96104-605">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="96104-605">Additional Info</span></span></td>
<td><p><span data-ttu-id="96104-606">Любые дополнительные сведения, не включенные в другие столбцы.</span><span class="sxs-lookup"><span data-stu-id="96104-606">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="96104-607">Сопоставление платежей в счете и сверочном файле</span><span class="sxs-lookup"><span data-stu-id="96104-607">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="96104-608">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="96104-608">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="96104-609">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-609">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="96104-610">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="96104-610">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="96104-611">Одноразовые кредиты, скидки и возвраты денежных средств, которые отображаются в счете-фактуре как «Уточнения», не отображаются в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-611">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="96104-612">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="96104-612">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="96104-613"><strong>Описание платежа счета</strong></span><span class="sxs-lookup"><span data-stu-id="96104-613"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-614"><strong>Описание платежа сверочный файл (столбец ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="96104-614"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-615"><strong>Что такое эта плата?</strong></span><span class="sxs-lookup"><span data-stu-id="96104-615"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-616"><strong>Как сопоставить эти счетом в счет?</strong></span><span class="sxs-lookup"><span data-stu-id="96104-616"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="96104-617"><strong>Расходы на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="96104-617"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-618">Стоимость активации</span><span class="sxs-lookup"><span data-stu-id="96104-618">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-619">Сумма, взимаемая с клиента при использовании подписки после ее приобретения</span><span class="sxs-lookup"><span data-stu-id="96104-619">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="96104-620">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="96104-620">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-621">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="96104-621">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-622">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="96104-622">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-623">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="96104-623">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-624">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="96104-624">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-625">Пропорциональный перерасчет одного цикла</span><span class="sxs-lookup"><span data-stu-id="96104-625">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-626">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="96104-626">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-627">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="96104-627">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-628">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="96104-628">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-629">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="96104-629">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-630">Тип накладных расходов для подписки при использовании выставление счетов за год</span><span class="sxs-lookup"><span data-stu-id="96104-630">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-631">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="96104-631">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-632">Тип накладных расходов для подписки при использовании сумма ежемесячных счетов</span><span class="sxs-lookup"><span data-stu-id="96104-632">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-633">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="96104-633">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-634">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="96104-634">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="96104-635">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="96104-635">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-636">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="96104-636">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-637">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="96104-637">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-638">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="96104-638">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="96104-639"><strong>Одноразовый расходов</strong></span><span class="sxs-lookup"><span data-stu-id="96104-639"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="96104-640">Оператор new</span><span class="sxs-lookup"><span data-stu-id="96104-640">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-641">Используется при создании новой покупки</span><span class="sxs-lookup"><span data-stu-id="96104-641">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-642">addQuantity</span><span class="sxs-lookup"><span data-stu-id="96104-642">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-643">После увеличения использованы в возмещение первоначальной покупки и новое количество</span><span class="sxs-lookup"><span data-stu-id="96104-643">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="96104-644">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="96104-644">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-645">После уменьшения использованы в возмещение первоначальной покупки и новое количество</span><span class="sxs-lookup"><span data-stu-id="96104-645">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="96104-646">Отмена</span><span class="sxs-lookup"><span data-stu-id="96104-646">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-647">Используется при отмене подписки</span><span class="sxs-lookup"><span data-stu-id="96104-647">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="96104-648">Преобразование</span><span class="sxs-lookup"><span data-stu-id="96104-648">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-649">Используется, когда обновляется лицензию, но не изменяется число рабочих мест</span><span class="sxs-lookup"><span data-stu-id="96104-649">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="96104-650"><strong>Плата за использование</strong></span><span class="sxs-lookup"><span data-stu-id="96104-650"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-651">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="96104-651">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-652">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="96104-652">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="96104-653">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="96104-653">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-654">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="96104-654">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-655">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="96104-655">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="96104-656"><strong>Деньги на счете</strong></span><span class="sxs-lookup"><span data-stu-id="96104-656"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-657">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="96104-657">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-658">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="96104-658">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-659">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="96104-659">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="96104-660">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="96104-660">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="96104-661"><strong>Скидки на основе использования</strong></span><span class="sxs-lookup"><span data-stu-id="96104-661"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-662">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="96104-662">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-663">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="96104-663">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="96104-664">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="96104-664">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-665">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="96104-665">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-666">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="96104-666">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-667">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="96104-667">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-668">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="96104-668">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-669">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="96104-669">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-670">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="96104-670">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="96104-671"><strong>Скидки на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="96104-671"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-672"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="96104-672"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="96104-673">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="96104-673">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="96104-674"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="96104-674"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-675"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="96104-675"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="96104-676"><em>Исключение: &quot;Смещение элемента строки&quot; уже включает в себя налоги. Деньги на счете, см. выше.</em></span><span class="sxs-lookup"><span data-stu-id="96104-676"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-677">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="96104-677">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="96104-678">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="96104-678">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="96104-679">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="96104-679">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
