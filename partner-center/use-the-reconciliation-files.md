---
title: Использование файлов выверки | Центр партнеров
ms.topic: article
ms.date: 07/08/2019
description: Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 83be47cd9963d7e5f14b6c670cd57a8ab1d54011
ms.sourcegitcommit: 66afdaa662cfad217e29ba1f9e3a9ffd4349112f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2019
ms.locfileid: "67694927"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="ae00e-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="ae00e-103">Use the reconciliation files</span></span>

<span data-ttu-id="ae00e-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="ae00e-104">**Applies to**</span></span>

-  <span data-ttu-id="ae00e-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="ae00e-105">Partner Center</span></span>
-  <span data-ttu-id="ae00e-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="ae00e-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="ae00e-107">Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="ae00e-108">Эти сведения включают оплаты за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="ae00e-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="ae00e-109">Особенности форматирования</span><span class="sxs-lookup"><span data-stu-id="ae00e-109">Formatting issues</span></span>

<span data-ttu-id="ae00e-110">Иногда проверка файла возможно, проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="ae00e-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="ae00e-111">(Это может произойти, например, если не используется языковой стандарт EN-US.) Выполните следующие действия, чтобы устранить эти проблемы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="ae00e-112">Откройте CSV-файл в Excel и выберите первый столбец.</span><span class="sxs-lookup"><span data-stu-id="ae00e-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="ae00e-113">На ленте выберите <strong>данных</strong>, а затем выберите <strong>текст по столбцам</strong>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="ae00e-114">В преобразовать в столбцы мастера выберите <strong>с разделителями тип файла</strong>, а затем выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ae00e-115">В поле разделителей групп разрядов выберите <strong>разделителями</strong>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="ae00e-116">Если <strong>вкладке</strong> является еще выбран, можно оставить его.</span><span class="sxs-lookup"><span data-stu-id="ae00e-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="ae00e-117">Выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="ae00e-118">В поле формата столбца данных, выберите <strong>даты: MDY (МДГ)</strong>, а затем выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ae00e-119">В поле формата столбца данных, выберите <strong>текст</strong> для всех сумма столбцов, а затем выберите <strong>Готово</strong>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="ae00e-120">Загрузка больших файлов разведывательную</span><span class="sxs-lookup"><span data-stu-id="ae00e-120">Downloading a large recon file</span></span>

<span data-ttu-id="ae00e-121">Проверка файлов может стать очень большой и иногда трудно загрузки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="ae00e-122">Сценарий PowerShell для загрузки больших файлов разведывательную, см. в разделе [позиций в строках счета Get](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="ae00e-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="ae00e-123">Детализировать партнером</span><span class="sxs-lookup"><span data-stu-id="ae00e-123">Itemize by partner</span></span>


<span data-ttu-id="ae00e-124">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="ae00e-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ae00e-125">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="ae00e-125">MPN ID</span></span></th>
<th><span data-ttu-id="ae00e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ae00e-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ae00e-127">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="ae00e-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="ae00e-128">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="ae00e-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-129">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="ae00e-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="ae00e-130">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="ae00e-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="ae00e-131">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ae00e-132">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="ae00e-133">Просмотр позитивную или обновление торгового посредника, в меню центра партнеров выберите <strong>клиентов</strong>, затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ae00e-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="ae00e-134">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="ae00e-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="ae00e-135">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="ae00e-136">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="ae00e-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="ae00e-137">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="ae00e-138">Если партнер CSP удаляет идентификатор торгового посредника, это значение будет равно -1.</span><span class="sxs-lookup"><span data-stu-id="ae00e-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="ae00e-139">Поля файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="ae00e-139">License-based file fields</span></span>


<span data-ttu-id="ae00e-140">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ae00e-141"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ae00e-142"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ae00e-143"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ae00e-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="ae00e-145">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="ae00e-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ae00e-146">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="ae00e-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ae00e-147">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="ae00e-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="ae00e-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="ae00e-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ae00e-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="ae00e-150">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ae00e-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="ae00e-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="ae00e-152">OrderID</span></span></td>
<td><p><span data-ttu-id="ae00e-153">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ae00e-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ae00e-154">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ae00e-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ae00e-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ae00e-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ae00e-157">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ae00e-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ae00e-158">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ae00e-159">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="ae00e-160">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="ae00e-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="ae00e-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ae00e-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="ae00e-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="ae00e-163">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="ae00e-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="ae00e-164">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="ae00e-165">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ae00e-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="ae00e-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="ae00e-167">OfferID</span></span></td>
<td><p><span data-ttu-id="ae00e-168">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="ae00e-168">Unique offer ID.</span></span> <span data-ttu-id="ae00e-169">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="ae00e-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="ae00e-170"><b>Примечание</b>. Это значение не соответствует Идентификатору предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="ae00e-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="ae00e-171">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="ae00e-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="ae00e-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="ae00e-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="ae00e-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="ae00e-174">Уникальный идентификатор длительного предложения как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="ae00e-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="ae00e-175"><b>Примечание</b>. Это значение совпадает с Идентификатором предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="ae00e-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="ae00e-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="ae00e-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="ae00e-177">OfferName</span></span></td>
<td><p><span data-ttu-id="ae00e-178">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="ae00e-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="ae00e-179">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="ae00e-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="ae00e-181">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="ae00e-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="ae00e-182">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="ae00e-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="ae00e-183">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ae00e-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ae00e-184">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ae00e-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="ae00e-186">Дата окончания подписки: 12 месяцев + x дней после даты начала (чтобы соответствовать выставления счетов даты партнера) или 12 месяцев с даты продления.</span><span class="sxs-lookup"><span data-stu-id="ae00e-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="ae00e-187">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="ae00e-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="ae00e-188">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="ae00e-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="ae00e-189">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ae00e-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ae00e-190">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ae00e-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ae00e-192">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="ae00e-193">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ae00e-194">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ae00e-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ae00e-195">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ae00e-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ae00e-197">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="ae00e-198">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ae00e-199">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ae00e-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ae00e-200">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="ae00e-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ae00e-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="ae00e-202">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="ae00e-202">The type of charge or adjustment.</span></span> <span data-ttu-id="ae00e-203">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="ae00e-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ae00e-204">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="ae00e-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="ae00e-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="ae00e-206">Цена за рабочее место, опубликованное в прайс-листе во время покупки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ae00e-207">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ae00e-208">6,82</span><span class="sxs-lookup"><span data-stu-id="ae00e-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-209">Количество</span><span class="sxs-lookup"><span data-stu-id="ae00e-209">Quantity</span></span></td>
<td><p><span data-ttu-id="ae00e-210">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="ae00e-210">Number of seats.</span></span> <span data-ttu-id="ae00e-211">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ae00e-212">2</span><span class="sxs-lookup"><span data-stu-id="ae00e-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-213">Сумма</span><span class="sxs-lookup"><span data-stu-id="ae00e-213">Amount</span></span></td>
<td><p><span data-ttu-id="ae00e-214">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="ae00e-214">Total of price for quantity.</span></span> <span data-ttu-id="ae00e-215">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="ae00e-216">13,32</span><span class="sxs-lookup"><span data-stu-id="ae00e-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="ae00e-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="ae00e-218">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="ae00e-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="ae00e-219">IUR или новые подписки, на которые распространяются вознаграждения, будут также содержать сумму скидки в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="ae00e-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="ae00e-220">2,32</span><span class="sxs-lookup"><span data-stu-id="ae00e-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-221">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="ae00e-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="ae00e-222">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="ae00e-222">Total before tax.</span></span> <span data-ttu-id="ae00e-223">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="ae00e-224">11</span><span class="sxs-lookup"><span data-stu-id="ae00e-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-225">Налог</span><span class="sxs-lookup"><span data-stu-id="ae00e-225">Tax</span></span></td>
<td><p><span data-ttu-id="ae00e-226">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="ae00e-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ae00e-227">0</span><span class="sxs-lookup"><span data-stu-id="ae00e-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="ae00e-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="ae00e-229">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-229">Total after tax.</span></span> <span data-ttu-id="ae00e-230">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="ae00e-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="ae00e-231">11</span><span class="sxs-lookup"><span data-stu-id="ae00e-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-232">Валюта</span><span class="sxs-lookup"><span data-stu-id="ae00e-232">Currency</span></span></td>
<td><p><span data-ttu-id="ae00e-233">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-233">Currency type.</span></span> <span data-ttu-id="ae00e-234">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="ae00e-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="ae00e-235">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ae00e-236">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="ae00e-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ae00e-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="ae00e-238">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ae00e-239">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ae00e-240">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="ae00e-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="ae00e-241">MPNID</span></span></td>
<td><p><span data-ttu-id="ae00e-242">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="ae00e-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="ae00e-243">4390934</span><span class="sxs-lookup"><span data-stu-id="ae00e-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ae00e-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ae00e-245">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ae00e-246">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ae00e-247">4390934</span><span class="sxs-lookup"><span data-stu-id="ae00e-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="ae00e-248">DomainName</span></span></td>
<td><p><span data-ttu-id="ae00e-249">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ae00e-250">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="ae00e-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ae00e-251">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ae00e-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ae00e-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ae00e-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ae00e-254">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-254">Subscription nickname.</span></span> <span data-ttu-id="ae00e-255">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="ae00e-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="ae00e-256">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="ae00e-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ae00e-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ae00e-258">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="ae00e-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ae00e-259">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="ae00e-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="ae00e-260">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="ae00e-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="ae00e-261">Поля файла на основе использования</span><span class="sxs-lookup"><span data-stu-id="ae00e-261">Usage-based file fields</span></span>


<span data-ttu-id="ae00e-262">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="ae00e-263">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="ae00e-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ae00e-264"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ae00e-265"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ae00e-266"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="ae00e-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="ae00e-268">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="ae00e-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="ae00e-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ae00e-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ae00e-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="ae00e-271">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="ae00e-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="ae00e-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="ae00e-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="ae00e-274">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="ae00e-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="ae00e-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ae00e-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="ae00e-277">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ae00e-278">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ae00e-279">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="ae00e-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="ae00e-280">MPNID</span></span></td>
<td><p><span data-ttu-id="ae00e-281">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="ae00e-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="ae00e-282">4390934</span><span class="sxs-lookup"><span data-stu-id="ae00e-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ae00e-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ae00e-284">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ae00e-285">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="ae00e-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ae00e-286">4390934</span><span class="sxs-lookup"><span data-stu-id="ae00e-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ae00e-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ae00e-288">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="ae00e-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="ae00e-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="ae00e-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ae00e-291">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="ae00e-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ae00e-292">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ae00e-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ae00e-293">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ae00e-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ae00e-295">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="ae00e-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ae00e-296">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ae00e-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ae00e-297">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="ae00e-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ae00e-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ae00e-299">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ae00e-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ae00e-300">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ae00e-301">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ae00e-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ae00e-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ae00e-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ae00e-304">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="ae00e-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ae00e-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ae00e-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ae00e-307">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="ae00e-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="ae00e-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ae00e-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="ae00e-309">OrderID</span></span></td>
<td><p><span data-ttu-id="ae00e-310">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ae00e-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ae00e-311">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ae00e-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ae00e-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="ae00e-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="ae00e-314">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="ae00e-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="ae00e-315">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="ae00e-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="ae00e-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="ae00e-317">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="ae00e-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ae00e-318">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="ae00e-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="ae00e-319">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="ae00e-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="ae00e-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="ae00e-321">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="ae00e-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ae00e-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-323">Resource Name</span><span class="sxs-lookup"><span data-stu-id="ae00e-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="ae00e-324">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="ae00e-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ae00e-325">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="ae00e-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="ae00e-326">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="ae00e-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-327">Region</span><span class="sxs-lookup"><span data-stu-id="ae00e-327">Region</span></span></td>
<td><p><span data-ttu-id="ae00e-328">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="ae00e-328">The region the usage applies to.</span></span> <span data-ttu-id="ae00e-329">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="ae00e-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="ae00e-330">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="ae00e-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-331">номер SKU</span><span class="sxs-lookup"><span data-stu-id="ae00e-331">SKU</span></span></td>
<td><p><span data-ttu-id="ae00e-332">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="ae00e-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="ae00e-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="ae00e-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="ae00e-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="ae00e-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="ae00e-335">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="ae00e-336">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним — другой.</span><span class="sxs-lookup"><span data-stu-id="ae00e-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="ae00e-337">1</span><span class="sxs-lookup"><span data-stu-id="ae00e-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="ae00e-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="ae00e-339">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ae00e-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="ae00e-340">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="ae00e-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="ae00e-341">11</span><span class="sxs-lookup"><span data-stu-id="ae00e-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="ae00e-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="ae00e-343">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="ae00e-343">Units included as part of the offer.</span></span> <span data-ttu-id="ae00e-344">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="ae00e-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="ae00e-345">0</span><span class="sxs-lookup"><span data-stu-id="ae00e-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="ae00e-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="ae00e-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="ae00e-347">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="ae00e-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="ae00e-348">Равняется разнице значений полей ConsumedQuantity и IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="ae00e-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="ae00e-349">11</span><span class="sxs-lookup"><span data-stu-id="ae00e-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="ae00e-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="ae00e-351">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="ae00e-352">0,0808 долл. США</span><span class="sxs-lookup"><span data-stu-id="ae00e-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="ae00e-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="ae00e-354">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ae00e-355">0,085 долл. США</span><span class="sxs-lookup"><span data-stu-id="ae00e-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="ae00e-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="ae00e-357">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="ae00e-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ae00e-358">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="ae00e-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="ae00e-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="ae00e-360">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="ae00e-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="ae00e-361">0,93 долл. США</span><span class="sxs-lookup"><span data-stu-id="ae00e-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-362">Валюта</span><span class="sxs-lookup"><span data-stu-id="ae00e-362">Currency</span></span></td>
<td><p><span data-ttu-id="ae00e-363">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-363">Currency type.</span></span> <span data-ttu-id="ae00e-364">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="ae00e-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="ae00e-365">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ae00e-366">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="ae00e-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ae00e-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ae00e-368">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-368">Pretax price per unit.</span></span> <span data-ttu-id="ae00e-369">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ae00e-370">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="ae00e-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ae00e-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ae00e-372">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="ae00e-372">Post tax price per unit.</span></span> <span data-ttu-id="ae00e-373">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ae00e-374">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="ae00e-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ae00e-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="ae00e-376">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="ae00e-376">The type of charge or adjustment.</span></span> <span data-ttu-id="ae00e-377">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="ae00e-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ae00e-378">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="ae00e-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="ae00e-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="ae00e-380">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="ae00e-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="ae00e-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="ae00e-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="ae00e-383">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="ae00e-384">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ae00e-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="ae00e-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="ae00e-386">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="ae00e-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="ae00e-387">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="ae00e-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-388">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="ae00e-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="ae00e-389">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="ae00e-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="ae00e-390">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="ae00e-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="ae00e-391">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="ae00e-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="ae00e-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="ae00e-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="ae00e-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="ae00e-394">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="ae00e-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="ae00e-395">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="ae00e-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-396">Проект</span><span class="sxs-lookup"><span data-stu-id="ae00e-396">Project</span></span></td>
<td><p><span data-ttu-id="ae00e-397">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="ae00e-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="ae00e-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ae00e-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="ae00e-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="ae00e-400">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="ae00e-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="ae00e-401">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="ae00e-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="ae00e-402">Если имеется 25 пакетов подключений служебной шины подготовлено, и вы использовалось 1 в течение этого дня, инструкцию ежедневное использование за этот день означает «25 подключений / 30 дней — использовано: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="ae00e-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ae00e-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="ae00e-404">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ae00e-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ae00e-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ae00e-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="ae00e-406">DomainName</span></span></td>
<td><p><span data-ttu-id="ae00e-407">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ae00e-408">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ae00e-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ae00e-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="ae00e-410">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="ae00e-410">Unit</span></span></td>
<td><p><span data-ttu-id="ae00e-411">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="ae00e-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="ae00e-412">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="ae00e-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="ae00e-413">Файл одноразовые и повторяющиеся поля</span><span class="sxs-lookup"><span data-stu-id="ae00e-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ae00e-414">Column</span><span class="sxs-lookup"><span data-stu-id="ae00e-414">Column</span></span></th>
<th><span data-ttu-id="ae00e-415">Описание</span><span class="sxs-lookup"><span data-stu-id="ae00e-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="ae00e-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ae00e-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="ae00e-417">Уникальный идентификатор клиента Microsoft Azure Active Directory для конкретной сущности выставления счетов, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="ae00e-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ae00e-418">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="ae00e-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ae00e-419">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="ae00e-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-420">Идентификатор клиента</span><span class="sxs-lookup"><span data-stu-id="ae00e-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="ae00e-421">Уникальный Microsoft Azure Active Directory идентификатор клиента, в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-422">Customer Name (Имя клиента)</span><span class="sxs-lookup"><span data-stu-id="ae00e-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="ae00e-423">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ae00e-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ae00e-425">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="ae00e-426">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="ae00e-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ae00e-427">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-428">Страна или регион клиента</span><span class="sxs-lookup"><span data-stu-id="ae00e-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="ae00e-429">Страна или регион, где находится клиент.</span><span class="sxs-lookup"><span data-stu-id="ae00e-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-430">Номер счета</span><span class="sxs-lookup"><span data-stu-id="ae00e-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="ae00e-431">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="ae00e-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="ae00e-432">MpnId</span></span></td>
<td><p><span data-ttu-id="ae00e-433">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="ae00e-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-434">MpnId торгового посредника</span><span class="sxs-lookup"><span data-stu-id="ae00e-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="ae00e-435">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-436">Идентификатор заказа</span><span class="sxs-lookup"><span data-stu-id="ae00e-436">Order ID</span></span></td>
<td><p><span data-ttu-id="ae00e-437">Уникальный идентификатор заказа на платформе Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="ae00e-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="ae00e-438">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-439">Дата заказа</span><span class="sxs-lookup"><span data-stu-id="ae00e-439">Order date</span></span></td>
<td><p><span data-ttu-id="ae00e-440">Дата размещения заказа.</span><span class="sxs-lookup"><span data-stu-id="ae00e-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-441">ProductID</span><span class="sxs-lookup"><span data-stu-id="ae00e-441">ProductId</span></span></td>
<td><p><span data-ttu-id="ae00e-442">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="ae00e-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="ae00e-443">SkuId</span></span></td>
<td><p><span data-ttu-id="ae00e-444">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="ae00e-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ae00e-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ae00e-446">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="ae00e-446">The ID for a particular Availability.</span></span> <span data-ttu-id="ae00e-447">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="ae00e-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-448">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="ae00e-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="ae00e-449">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="ae00e-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-450">название продукта;</span><span class="sxs-lookup"><span data-stu-id="ae00e-450">Product name</span></span></td>
<td><p><span data-ttu-id="ae00e-451">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="ae00e-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ae00e-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="ae00e-453">Имя издателя продукта.</span><span class="sxs-lookup"><span data-stu-id="ae00e-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ae00e-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="ae00e-455">Уникальный идентификатор для данного издателя.</span><span class="sxs-lookup"><span data-stu-id="ae00e-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-456">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ae00e-457">Понятное имя подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-458">Код подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ae00e-459">Уникальный идентификатор для подписки на платформу Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="ae00e-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="ae00e-460">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ae00e-461">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ae00e-463">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-463">Start day of the charges.</span></span> <span data-ttu-id="ae00e-464">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ae00e-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ae00e-466">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-466">End day of the charges.</span></span> <span data-ttu-id="ae00e-467">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ae00e-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-468">Термин и Billingcycle</span><span class="sxs-lookup"><span data-stu-id="ae00e-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="ae00e-469">Продолжительность срока и цикла выставления счетов за покупки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="ae00e-470">Например «1 год, месяц.»</span><span class="sxs-lookup"><span data-stu-id="ae00e-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-471">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="ae00e-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="ae00e-472">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="ae00e-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-473">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="ae00e-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="ae00e-474">Цена, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ae00e-475">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-476">Эффективное модульное цена</span><span class="sxs-lookup"><span data-stu-id="ae00e-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="ae00e-477">Цена за единицу после изменения.</span><span class="sxs-lookup"><span data-stu-id="ae00e-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-478">Количество</span><span class="sxs-lookup"><span data-stu-id="ae00e-478">Quantity</span></span></td>
<td><p><span data-ttu-id="ae00e-479">Число единиц.</span><span class="sxs-lookup"><span data-stu-id="ae00e-479">Number of units.</span></span> <span data-ttu-id="ae00e-480">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-481">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="ae00e-481">Unit type</span></span></td>
<td><p><span data-ttu-id="ae00e-482">Тип приобретенная единица.</span><span class="sxs-lookup"><span data-stu-id="ae00e-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="ae00e-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="ae00e-484">Объяснение применяемой скидки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-485">Итого</span><span class="sxs-lookup"><span data-stu-id="ae00e-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="ae00e-486">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="ae00e-486">Total before tax.</span></span> <span data-ttu-id="ae00e-487">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-488">Общая сумма налога</span><span class="sxs-lookup"><span data-stu-id="ae00e-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="ae00e-489">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="ae00e-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-490">Total (Всего)</span><span class="sxs-lookup"><span data-stu-id="ae00e-490">Total</span></span></td>
<td><p><span data-ttu-id="ae00e-491">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-491">Total after tax.</span></span> <span data-ttu-id="ae00e-492">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="ae00e-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-493">Валюта</span><span class="sxs-lookup"><span data-stu-id="ae00e-493">Currency</span></span></td>
<td><p><span data-ttu-id="ae00e-494">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="ae00e-494">Currency type.</span></span> <span data-ttu-id="ae00e-495">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="ae00e-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="ae00e-496">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-497">Альтернативного имени пользователя</span><span class="sxs-lookup"><span data-stu-id="ae00e-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="ae00e-498">Альтернативный идентификатор с идентификатором заказа.</span><span class="sxs-lookup"><span data-stu-id="ae00e-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="ae00e-499">Поля файла оценкой ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="ae00e-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ae00e-500">Column</span><span class="sxs-lookup"><span data-stu-id="ae00e-500">Column</span></span></th>
<th><span data-ttu-id="ae00e-501">Описание</span><span class="sxs-lookup"><span data-stu-id="ae00e-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="ae00e-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ae00e-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="ae00e-503">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="ae00e-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ae00e-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="ae00e-505">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="ae00e-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="ae00e-507">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="ae00e-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="ae00e-509">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ae00e-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ae00e-510">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ae00e-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ae00e-512">Имя домена клиента.</span><span class="sxs-lookup"><span data-stu-id="ae00e-512">The customer’s domain name.</span></span> <span data-ttu-id="ae00e-513">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="ae00e-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-514">Страна или регион клиента</span><span class="sxs-lookup"><span data-stu-id="ae00e-514">Customer country</span></span></td>
<td><p><span data-ttu-id="ae00e-515">Страна или регион, где находится клиент.</span><span class="sxs-lookup"><span data-stu-id="ae00e-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="ae00e-516">MPNID</span></span></td>
<td><p><span data-ttu-id="ae00e-517">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="ae00e-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-518">Торговый посредник MPNID</span><span class="sxs-lookup"><span data-stu-id="ae00e-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="ae00e-519">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ae00e-520">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="ae00e-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ae00e-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ae00e-522">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="ae00e-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="ae00e-523">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="ae00e-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-524">ProductID</span><span class="sxs-lookup"><span data-stu-id="ae00e-524">ProductId</span></span></td>
<td><p><span data-ttu-id="ae00e-525">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="ae00e-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="ae00e-526">SkuId</span></span></td>
<td><p><span data-ttu-id="ae00e-527">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="ae00e-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ae00e-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ae00e-529">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="ae00e-529">The ID for a particular Availability.</span></span> <span data-ttu-id="ae00e-530">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="ae00e-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-531">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="ae00e-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="ae00e-532">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="ae00e-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ae00e-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="ae00e-534">Имя издателя.</span><span class="sxs-lookup"><span data-stu-id="ae00e-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ae00e-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="ae00e-536">Идентификатор издателя, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="ae00e-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="ae00e-537">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="ae00e-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="ae00e-538">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ae00e-539">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="ae00e-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ae00e-540">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="ae00e-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-541">Код подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ae00e-542">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ae00e-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ae00e-543">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ae00e-544">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="ae00e-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ae00e-546">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="ae00e-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ae00e-547">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ae00e-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ae00e-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ae00e-549">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="ae00e-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ae00e-550">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ae00e-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-551">Дата использования</span><span class="sxs-lookup"><span data-stu-id="ae00e-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="ae00e-552">Дата использования службы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-553">Индикатор типа</span><span class="sxs-lookup"><span data-stu-id="ae00e-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="ae00e-554">Тип единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="ae00e-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-555">Категория счетчика</span><span class="sxs-lookup"><span data-stu-id="ae00e-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="ae00e-556">Служба верхнего уровня для использования.</span><span class="sxs-lookup"><span data-stu-id="ae00e-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-557">Идентификатор счетчика</span><span class="sxs-lookup"><span data-stu-id="ae00e-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="ae00e-558">Идентификатор для использования средства измерения.</span><span class="sxs-lookup"><span data-stu-id="ae00e-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-559">Подкатегория измерения</span><span class="sxs-lookup"><span data-stu-id="ae00e-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="ae00e-560">Тип службы Azure, которые могут повлиять на скорость.</span><span class="sxs-lookup"><span data-stu-id="ae00e-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-561">Имя единицы измерения</span><span class="sxs-lookup"><span data-stu-id="ae00e-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="ae00e-562">Единица измерения для использованного средства измерения.</span><span class="sxs-lookup"><span data-stu-id="ae00e-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-563">Регион счетчика</span><span class="sxs-lookup"><span data-stu-id="ae00e-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="ae00e-564">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="ae00e-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-565">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="ae00e-565">Unit</span></span></td>
<td><p><span data-ttu-id="ae00e-566">Единица имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="ae00e-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-567">Использованное количество</span><span class="sxs-lookup"><span data-stu-id="ae00e-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="ae00e-568">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ae00e-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="ae00e-569">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="ae00e-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-570">Расположение ресурса</span><span class="sxs-lookup"><span data-stu-id="ae00e-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="ae00e-571">Центр обработки данных, где выполняется средства измерения.</span><span class="sxs-lookup"><span data-stu-id="ae00e-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-572">Используемой службы</span><span class="sxs-lookup"><span data-stu-id="ae00e-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="ae00e-573">Используемая служба платформы Azure.</span><span class="sxs-lookup"><span data-stu-id="ae00e-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="ae00e-574">URI ресурса</span><span class="sxs-lookup"><span data-stu-id="ae00e-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="ae00e-575">URI ресурса, который используется.</span><span class="sxs-lookup"><span data-stu-id="ae00e-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-576">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="ae00e-576">Charge type</span></span></td>
<td><p><span data-ttu-id="ae00e-577">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="ae00e-577">The type of charge or adjustment.</span></span> <span data-ttu-id="ae00e-578">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="ae00e-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-579">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="ae00e-579">Unit price</span></span></td>
<td><p><span data-ttu-id="ae00e-580">Цена за лицензии, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ae00e-581">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-582">Количество</span><span class="sxs-lookup"><span data-stu-id="ae00e-582">Quantity</span></span></td>
<td><p><span data-ttu-id="ae00e-583">Количество лицензий.</span><span class="sxs-lookup"><span data-stu-id="ae00e-583">Number of licenses.</span></span> <span data-ttu-id="ae00e-584">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-585">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="ae00e-585">Unit type</span></span></td>
<td><p><span data-ttu-id="ae00e-586">Тип единицы измерения единицы измеряется объем использования.</span><span class="sxs-lookup"><span data-stu-id="ae00e-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="ae00e-587">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="ae00e-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-588">Налог pre выставления счетов</span><span class="sxs-lookup"><span data-stu-id="ae00e-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="ae00e-589">Общая сумма до налогов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-590">Валюта для выставления счетов</span><span class="sxs-lookup"><span data-stu-id="ae00e-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="ae00e-591">Валюта в географическом регионе клиента</span><span class="sxs-lookup"><span data-stu-id="ae00e-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-592">Цены до выплаты налогов всего</span><span class="sxs-lookup"><span data-stu-id="ae00e-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="ae00e-593">Цены до налогов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-594">Цены на валюту</span><span class="sxs-lookup"><span data-stu-id="ae00e-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="ae00e-595">Валюта, в прайс-листа.</span><span class="sxs-lookup"><span data-stu-id="ae00e-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ae00e-596">Сведения о службе 1</span><span class="sxs-lookup"><span data-stu-id="ae00e-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="ae00e-597">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="ae00e-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-598">Сведения о службе 2</span><span class="sxs-lookup"><span data-stu-id="ae00e-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="ae00e-599">Устаревшее поле, в которое записываются необязательные метаданные службы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ae00e-600">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="ae00e-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="ae00e-601">Любые дополнительные сведения, не включенные в другие столбцы.</span><span class="sxs-lookup"><span data-stu-id="ae00e-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="ae00e-602">Сопоставление платежей в счете и сверочном файле</span><span class="sxs-lookup"><span data-stu-id="ae00e-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="ae00e-603">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="ae00e-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="ae00e-604">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="ae00e-605">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="ae00e-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="ae00e-606">Одноразовые кредиты, скидки и возвраты денежных средств, которые отображаются в счете-фактуре как «Уточнения», не отображаются в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="ae00e-607">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="ae00e-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="ae00e-608"><strong>Описание платежа счета</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-609"><strong>Описание платежа сверочный файл (столбец ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-610"><strong>Что такое эта плата?</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-611"><strong>Как сопоставить эти счетом в счет?</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="ae00e-612"><strong>Расходы на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-613">Стоимость активации</span><span class="sxs-lookup"><span data-stu-id="ae00e-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-614">Сумма, взимаемая с клиента при использовании подписки после ее приобретения</span><span class="sxs-lookup"><span data-stu-id="ae00e-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="ae00e-615">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="ae00e-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-616">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="ae00e-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-617">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="ae00e-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-618">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="ae00e-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-619">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="ae00e-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-620">Пропорциональный перерасчет одного цикла</span><span class="sxs-lookup"><span data-stu-id="ae00e-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-621">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="ae00e-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-622">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="ae00e-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-623">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="ae00e-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-624">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="ae00e-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-625">Тип накладных расходов для подписки при использовании выставление счетов за год</span><span class="sxs-lookup"><span data-stu-id="ae00e-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-626">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="ae00e-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-627">Тип накладных расходов для подписки при использовании сумма ежемесячных счетов</span><span class="sxs-lookup"><span data-stu-id="ae00e-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-628">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="ae00e-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-629">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="ae00e-630">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="ae00e-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-631">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-632">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="ae00e-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-633">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="ae00e-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="ae00e-634"><strong>Одноразовый расходов</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="ae00e-635">Оператор new</span><span class="sxs-lookup"><span data-stu-id="ae00e-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-636">Используется при создании новой покупки</span><span class="sxs-lookup"><span data-stu-id="ae00e-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-637">addQuantity</span><span class="sxs-lookup"><span data-stu-id="ae00e-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-638">После увеличения использованы в возмещение первоначальной покупки и новое количество</span><span class="sxs-lookup"><span data-stu-id="ae00e-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-639">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="ae00e-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-640">После уменьшения использованы в возмещение первоначальной покупки и новое количество</span><span class="sxs-lookup"><span data-stu-id="ae00e-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-641">Отмена</span><span class="sxs-lookup"><span data-stu-id="ae00e-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-642">Используется при отмене подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-643">Преобразование</span><span class="sxs-lookup"><span data-stu-id="ae00e-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-644">Используется, когда обновляется лицензию, но не изменяется число рабочих мест</span><span class="sxs-lookup"><span data-stu-id="ae00e-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="ae00e-645"><strong>Плата за использование</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-646">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="ae00e-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-647">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="ae00e-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="ae00e-648">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="ae00e-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-649">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="ae00e-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-650">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="ae00e-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="ae00e-651"><strong>Деньги на счете</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-652">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="ae00e-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-653">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="ae00e-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-654">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="ae00e-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="ae00e-655">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="ae00e-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="ae00e-656"><strong>Скидки на основе использования</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-657">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="ae00e-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-658">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="ae00e-659">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="ae00e-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-660">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="ae00e-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-661">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="ae00e-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-662">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="ae00e-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-663">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="ae00e-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-664">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="ae00e-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-665">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="ae00e-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="ae00e-666"><strong>Скидки на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-667"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="ae00e-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="ae00e-668">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="ae00e-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ae00e-669"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="ae00e-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-670"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="ae00e-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="ae00e-671"><em>Исключение: &quot;Смещение элемента строки&quot; уже включает в себя налоги. Деньги на счете, см. выше.</em></span><span class="sxs-lookup"><span data-stu-id="ae00e-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-672">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="ae00e-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="ae00e-673">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="ae00e-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="ae00e-674">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="ae00e-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
