---
title: Использование файлов выверки | Центр партнеров
ms.topic: article
ms.date: 03/15/2019
description: Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8e7b17cb39f266c404d7873dc17e471741d52b32
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132784"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="40590-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="40590-103">Use the reconciliation files</span></span>

<span data-ttu-id="40590-104">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="40590-104">**Applies to**</span></span>

-  <span data-ttu-id="40590-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="40590-105">Partner Center</span></span>
-  <span data-ttu-id="40590-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="40590-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="40590-107">Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="40590-108">Эти сведения включают оплаты за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="40590-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="40590-109">Особенности форматирования</span><span class="sxs-lookup"><span data-stu-id="40590-109">Formatting issues</span></span>

<span data-ttu-id="40590-110">Иногда проверка файла возможно, проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="40590-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="40590-111">(Это может произойти, например, если не используется языковой стандарт EN-US.) Выполните следующие действия, чтобы устранить эти проблемы.</span><span class="sxs-lookup"><span data-stu-id="40590-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="40590-112">Откройте CSV-файл в Excel и выберите первый столбец.</span><span class="sxs-lookup"><span data-stu-id="40590-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="40590-113">На ленте выберите <strong>данных</strong>, а затем выберите <strong>текст по столбцам</strong>.</span><span class="sxs-lookup"><span data-stu-id="40590-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="40590-114">В преобразовать в столбцы мастера выберите <strong>с разделителями тип файла</strong>, а затем выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="40590-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="40590-115">В поле разделителей групп разрядов выберите <strong>разделителями</strong>.</span><span class="sxs-lookup"><span data-stu-id="40590-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="40590-116">Если <strong>вкладке</strong> является еще выбран, можно оставить его.</span><span class="sxs-lookup"><span data-stu-id="40590-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="40590-117">Выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="40590-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="40590-118">В поле формата столбца данных, выберите <strong>даты: MDY (МДГ)</strong>, а затем выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="40590-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="40590-119">В поле формата столбца данных, выберите <strong>текст</strong> для всех сумма столбцов, а затем выберите <strong>Готово</strong>.</span><span class="sxs-lookup"><span data-stu-id="40590-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="40590-120">Детализировать партнером</span><span class="sxs-lookup"><span data-stu-id="40590-120">Itemize by partner</span></span>


<span data-ttu-id="40590-121">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="40590-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="40590-122">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="40590-122">MPN ID</span></span></th>
<th><span data-ttu-id="40590-123">Описание</span><span class="sxs-lookup"><span data-stu-id="40590-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="40590-124">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="40590-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="40590-125">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="40590-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-126">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="40590-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="40590-127">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="40590-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="40590-128">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40590-129">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="40590-130">Просмотр позитивную или обновление торгового посредника, в меню центра партнеров выберите <strong>клиентов</strong>, затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="40590-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="40590-131">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="40590-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="40590-132">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="40590-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="40590-133">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="40590-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="40590-134">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="40590-135">Если партнер CSP удаляет идентификатор торгового посредника, это значение будет равно -1.</span><span class="sxs-lookup"><span data-stu-id="40590-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="40590-136">Поля файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="40590-136">License-based file fields</span></span>


<span data-ttu-id="40590-137">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="40590-138"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="40590-138"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="40590-139"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="40590-139"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="40590-140"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="40590-140"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="40590-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="40590-142">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="40590-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="40590-143">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="40590-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="40590-144">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="40590-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="40590-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="40590-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="40590-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="40590-147">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="40590-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="40590-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="40590-149">OrderID</span></span></td>
<td><p><span data-ttu-id="40590-150">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="40590-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="40590-151">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="40590-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="40590-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="40590-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="40590-154">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="40590-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="40590-155">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="40590-156">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="40590-157">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="40590-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="40590-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="40590-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="40590-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="40590-160">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="40590-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="40590-161">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="40590-162">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="40590-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="40590-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="40590-164">OfferID</span></span></td>
<td><p><span data-ttu-id="40590-165">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="40590-165">Unique offer ID.</span></span> <span data-ttu-id="40590-166">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="40590-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="40590-167"><b>Примечание</b>. Это значение не соответствует Идентификатору предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="40590-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="40590-168">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="40590-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="40590-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="40590-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="40590-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="40590-171">Уникальный идентификатор длительного предложения как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="40590-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="40590-172"><b>Примечание</b>. Это значение совпадает с Идентификатором предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="40590-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="40590-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="40590-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="40590-174">OfferName</span></span></td>
<td><p><span data-ttu-id="40590-175">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="40590-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="40590-176">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="40590-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="40590-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="40590-178">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="40590-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="40590-179">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="40590-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="40590-180">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="40590-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40590-181">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="40590-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="40590-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="40590-183">Дата окончания подписки: 12 месяцев + x дней после даты начала (чтобы соответствовать выставления счетов даты партнера) или 12 месяцев с даты продления.</span><span class="sxs-lookup"><span data-stu-id="40590-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="40590-184">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="40590-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="40590-185">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="40590-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="40590-186">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="40590-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40590-187">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="40590-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40590-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40590-189">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="40590-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="40590-190">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="40590-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="40590-191">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="40590-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40590-192">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="40590-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40590-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40590-194">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="40590-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="40590-195">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="40590-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="40590-196">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="40590-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="40590-197">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="40590-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="40590-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="40590-199">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="40590-199">The type of charge or adjustment.</span></span> <span data-ttu-id="40590-200">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="40590-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="40590-201">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="40590-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="40590-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="40590-203">Цена за рабочее место, опубликованное в прайс-листе во время покупки.</span><span class="sxs-lookup"><span data-stu-id="40590-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="40590-204">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="40590-205">6,82</span><span class="sxs-lookup"><span data-stu-id="40590-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-206">Количество</span><span class="sxs-lookup"><span data-stu-id="40590-206">Quantity</span></span></td>
<td><p><span data-ttu-id="40590-207">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="40590-207">Number of seats.</span></span> <span data-ttu-id="40590-208">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="40590-209">2</span><span class="sxs-lookup"><span data-stu-id="40590-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-210">Сумма</span><span class="sxs-lookup"><span data-stu-id="40590-210">Amount</span></span></td>
<td><p><span data-ttu-id="40590-211">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="40590-211">Total of price for quantity.</span></span> <span data-ttu-id="40590-212">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="40590-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="40590-213">13,32</span><span class="sxs-lookup"><span data-stu-id="40590-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="40590-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="40590-215">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="40590-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="40590-216">IUR или новые подписки, на которые распространяются вознаграждения, будут также содержать сумму скидки в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="40590-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="40590-217">2,32</span><span class="sxs-lookup"><span data-stu-id="40590-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-218">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="40590-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="40590-219">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="40590-219">Total before tax.</span></span> <span data-ttu-id="40590-220">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="40590-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="40590-221">11</span><span class="sxs-lookup"><span data-stu-id="40590-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-222">Налог</span><span class="sxs-lookup"><span data-stu-id="40590-222">Tax</span></span></td>
<td><p><span data-ttu-id="40590-223">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="40590-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="40590-224">0</span><span class="sxs-lookup"><span data-stu-id="40590-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="40590-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="40590-226">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="40590-226">Total after tax.</span></span> <span data-ttu-id="40590-227">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="40590-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="40590-228">11</span><span class="sxs-lookup"><span data-stu-id="40590-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-229">Валюта</span><span class="sxs-lookup"><span data-stu-id="40590-229">Currency</span></span></td>
<td><p><span data-ttu-id="40590-230">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="40590-230">Currency type.</span></span> <span data-ttu-id="40590-231">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="40590-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="40590-232">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="40590-233">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="40590-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="40590-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="40590-235">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="40590-236">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="40590-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="40590-237">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="40590-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="40590-238">MPNID</span></span></td>
<td><p><span data-ttu-id="40590-239">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="40590-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="40590-240">4390934</span><span class="sxs-lookup"><span data-stu-id="40590-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="40590-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="40590-242">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40590-243">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="40590-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="40590-244">4390934</span><span class="sxs-lookup"><span data-stu-id="40590-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="40590-245">DomainName</span></span></td>
<td><p><span data-ttu-id="40590-246">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="40590-247">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="40590-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="40590-248">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="40590-249">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="40590-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="40590-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="40590-251">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-251">Subscription nickname.</span></span> <span data-ttu-id="40590-252">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="40590-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="40590-253">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="40590-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="40590-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="40590-255">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="40590-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="40590-256">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="40590-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="40590-257">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="40590-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="40590-258">Поля файла на основе использования</span><span class="sxs-lookup"><span data-stu-id="40590-258">Usage-based file fields</span></span>


<span data-ttu-id="40590-259">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="40590-260">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="40590-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="40590-261"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="40590-261"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="40590-262"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="40590-262"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="40590-263"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="40590-263"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="40590-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="40590-265">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="40590-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="40590-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="40590-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="40590-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="40590-268">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="40590-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="40590-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="40590-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="40590-271">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="40590-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="40590-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="40590-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="40590-274">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="40590-275">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="40590-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="40590-276">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="40590-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="40590-277">MPNID</span></span></td>
<td><p><span data-ttu-id="40590-278">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="40590-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="40590-279">4390934</span><span class="sxs-lookup"><span data-stu-id="40590-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="40590-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="40590-281">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40590-282">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="40590-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="40590-283">4390934</span><span class="sxs-lookup"><span data-stu-id="40590-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="40590-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="40590-285">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="40590-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="40590-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="40590-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40590-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40590-288">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="40590-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="40590-289">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="40590-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40590-290">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="40590-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40590-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40590-292">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="40590-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="40590-293">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="40590-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="40590-294">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="40590-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="40590-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="40590-296">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="40590-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="40590-297">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="40590-298">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="40590-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="40590-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="40590-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="40590-301">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="40590-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="40590-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="40590-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="40590-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="40590-304">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="40590-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="40590-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="40590-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="40590-306">OrderID</span></span></td>
<td><p><span data-ttu-id="40590-307">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="40590-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="40590-308">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="40590-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="40590-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="40590-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="40590-311">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="40590-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="40590-312">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="40590-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="40590-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="40590-314">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="40590-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="40590-315">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="40590-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="40590-316">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="40590-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="40590-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="40590-318">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="40590-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="40590-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="40590-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-320">Resource Name</span><span class="sxs-lookup"><span data-stu-id="40590-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="40590-321">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="40590-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="40590-322">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="40590-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="40590-323">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="40590-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-324">Region</span><span class="sxs-lookup"><span data-stu-id="40590-324">Region</span></span></td>
<td><p><span data-ttu-id="40590-325">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="40590-325">The region the usage applies to.</span></span> <span data-ttu-id="40590-326">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="40590-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="40590-327">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="40590-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-328">номер SKU</span><span class="sxs-lookup"><span data-stu-id="40590-328">SKU</span></span></td>
<td><p><span data-ttu-id="40590-329">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="40590-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="40590-330">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="40590-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="40590-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="40590-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="40590-332">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="40590-333">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним — другой.</span><span class="sxs-lookup"><span data-stu-id="40590-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="40590-334">1</span><span class="sxs-lookup"><span data-stu-id="40590-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="40590-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="40590-336">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="40590-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="40590-337">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="40590-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="40590-338">11</span><span class="sxs-lookup"><span data-stu-id="40590-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="40590-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="40590-340">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="40590-340">Units included as part of the offer.</span></span> <span data-ttu-id="40590-341">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="40590-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="40590-342">0</span><span class="sxs-lookup"><span data-stu-id="40590-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="40590-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="40590-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="40590-344">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="40590-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="40590-345">Равняется разнице значений полей ConsumedQuantity и IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="40590-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="40590-346">11</span><span class="sxs-lookup"><span data-stu-id="40590-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="40590-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="40590-348">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="40590-349">0,0808 долл. США</span><span class="sxs-lookup"><span data-stu-id="40590-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="40590-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="40590-351">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="40590-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="40590-352">0,085 долл. США</span><span class="sxs-lookup"><span data-stu-id="40590-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="40590-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="40590-354">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="40590-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="40590-355">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="40590-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="40590-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="40590-357">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="40590-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="40590-358">0,93 долл. США</span><span class="sxs-lookup"><span data-stu-id="40590-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-359">Валюта</span><span class="sxs-lookup"><span data-stu-id="40590-359">Currency</span></span></td>
<td><p><span data-ttu-id="40590-360">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="40590-360">Currency type.</span></span> <span data-ttu-id="40590-361">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="40590-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="40590-362">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="40590-363">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="40590-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="40590-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="40590-365">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="40590-365">Pretax price per unit.</span></span> <span data-ttu-id="40590-366">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="40590-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="40590-367">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="40590-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="40590-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="40590-369">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="40590-369">Post tax price per unit.</span></span> <span data-ttu-id="40590-370">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="40590-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="40590-371">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="40590-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="40590-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="40590-373">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="40590-373">The type of charge or adjustment.</span></span> <span data-ttu-id="40590-374">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="40590-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="40590-375">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="40590-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="40590-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="40590-377">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="40590-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="40590-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="40590-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="40590-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="40590-380">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="40590-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="40590-381">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="40590-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="40590-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="40590-383">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="40590-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="40590-384">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="40590-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-385">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="40590-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="40590-386">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="40590-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="40590-387">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="40590-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="40590-388">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="40590-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="40590-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="40590-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="40590-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="40590-391">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="40590-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="40590-392">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="40590-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-393">Проект</span><span class="sxs-lookup"><span data-stu-id="40590-393">Project</span></span></td>
<td><p><span data-ttu-id="40590-394">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="40590-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="40590-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="40590-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="40590-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="40590-397">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="40590-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="40590-398">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="40590-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="40590-399">Если имеется 25 пакетов подключений служебной шины подготовлено, и вы использовалось 1 в течение этого дня, инструкцию ежедневное использование за этот день означает «25 подключений / 30 дней — использовано: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="40590-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="40590-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="40590-401">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="40590-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="40590-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40590-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="40590-403">DomainName</span></span></td>
<td><p><span data-ttu-id="40590-404">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="40590-405">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="40590-406">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="40590-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="40590-407">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="40590-407">Unit</span></span></td>
<td><p><span data-ttu-id="40590-408">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="40590-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="40590-409">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="40590-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="40590-410">Файл одноразовые и повторяющиеся поля</span><span class="sxs-lookup"><span data-stu-id="40590-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="40590-411">Column</span><span class="sxs-lookup"><span data-stu-id="40590-411">Column</span></span></th>
<th><span data-ttu-id="40590-412">Описание</span><span class="sxs-lookup"><span data-stu-id="40590-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="40590-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="40590-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="40590-414">Уникальный идентификатор клиента Microsoft Azure Active Directory для конкретной сущности выставления счетов, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="40590-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="40590-415">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="40590-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="40590-416">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="40590-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-417">Идентификатор клиента</span><span class="sxs-lookup"><span data-stu-id="40590-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="40590-418">Уникальный Microsoft Azure Active Directory идентификатор клиента, в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-419">Customer Name (Имя клиента)</span><span class="sxs-lookup"><span data-stu-id="40590-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="40590-420">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="40590-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="40590-422">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="40590-423">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="40590-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="40590-424">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-425">Страна или регион клиента</span><span class="sxs-lookup"><span data-stu-id="40590-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="40590-426">Страна или регион, где находится клиент.</span><span class="sxs-lookup"><span data-stu-id="40590-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-427">Номер счета</span><span class="sxs-lookup"><span data-stu-id="40590-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="40590-428">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="40590-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="40590-429">MpnId</span></span></td>
<td><p><span data-ttu-id="40590-430">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="40590-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-431">MpnId торгового посредника</span><span class="sxs-lookup"><span data-stu-id="40590-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="40590-432">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-433">Идентификатор заказа</span><span class="sxs-lookup"><span data-stu-id="40590-433">Order ID</span></span></td>
<td><p><span data-ttu-id="40590-434">Уникальный идентификатор заказа на платформе Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="40590-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="40590-435">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-436">Дата заказа</span><span class="sxs-lookup"><span data-stu-id="40590-436">Order date</span></span></td>
<td><p><span data-ttu-id="40590-437">Дата размещения заказа.</span><span class="sxs-lookup"><span data-stu-id="40590-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-438">ProductID</span><span class="sxs-lookup"><span data-stu-id="40590-438">ProductId</span></span></td>
<td><p><span data-ttu-id="40590-439">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="40590-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="40590-440">SkuId</span></span></td>
<td><p><span data-ttu-id="40590-441">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="40590-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="40590-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="40590-443">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="40590-443">The ID for a particular Availability.</span></span> <span data-ttu-id="40590-444">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="40590-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-445">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="40590-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="40590-446">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="40590-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-447">название продукта;</span><span class="sxs-lookup"><span data-stu-id="40590-447">Product name</span></span></td>
<td><p><span data-ttu-id="40590-448">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="40590-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="40590-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="40590-450">Имя издателя продукта.</span><span class="sxs-lookup"><span data-stu-id="40590-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="40590-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="40590-452">Уникальный идентификатор для данного издателя.</span><span class="sxs-lookup"><span data-stu-id="40590-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-453">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="40590-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="40590-454">Понятное имя подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-455">Код подписки</span><span class="sxs-lookup"><span data-stu-id="40590-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="40590-456">Уникальный идентификатор для подписки на платформу Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="40590-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="40590-457">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="40590-458">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40590-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40590-460">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="40590-460">Start day of the charges.</span></span> <span data-ttu-id="40590-461">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="40590-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40590-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40590-463">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="40590-463">End day of the charges.</span></span> <span data-ttu-id="40590-464">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="40590-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-465">Термин и Billingcycle</span><span class="sxs-lookup"><span data-stu-id="40590-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="40590-466">Продолжительность срока и цикла выставления счетов за покупки.</span><span class="sxs-lookup"><span data-stu-id="40590-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="40590-467">Например «1 год, месяц.»</span><span class="sxs-lookup"><span data-stu-id="40590-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-468">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="40590-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="40590-469">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="40590-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-470">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="40590-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="40590-471">Цена, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="40590-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="40590-472">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-473">Эффективное модульное цена</span><span class="sxs-lookup"><span data-stu-id="40590-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="40590-474">Цена за единицу после изменения.</span><span class="sxs-lookup"><span data-stu-id="40590-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-475">Количество</span><span class="sxs-lookup"><span data-stu-id="40590-475">Quantity</span></span></td>
<td><p><span data-ttu-id="40590-476">Число единиц.</span><span class="sxs-lookup"><span data-stu-id="40590-476">Number of units.</span></span> <span data-ttu-id="40590-477">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-478">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="40590-478">Unit type</span></span></td>
<td><p><span data-ttu-id="40590-479">Тип приобретенная единица.</span><span class="sxs-lookup"><span data-stu-id="40590-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="40590-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="40590-481">Объяснение применяемой скидки.</span><span class="sxs-lookup"><span data-stu-id="40590-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-482">Итого</span><span class="sxs-lookup"><span data-stu-id="40590-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="40590-483">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="40590-483">Total before tax.</span></span> <span data-ttu-id="40590-484">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="40590-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-485">Общая сумма налога</span><span class="sxs-lookup"><span data-stu-id="40590-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="40590-486">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="40590-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-487">Total (Всего)</span><span class="sxs-lookup"><span data-stu-id="40590-487">Total</span></span></td>
<td><p><span data-ttu-id="40590-488">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="40590-488">Total after tax.</span></span> <span data-ttu-id="40590-489">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="40590-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-490">Валюта</span><span class="sxs-lookup"><span data-stu-id="40590-490">Currency</span></span></td>
<td><p><span data-ttu-id="40590-491">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="40590-491">Currency type.</span></span> <span data-ttu-id="40590-492">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="40590-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="40590-493">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-494">Альтернативного имени пользователя</span><span class="sxs-lookup"><span data-stu-id="40590-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="40590-495">Альтернативный идентификатор с идентификатором заказа.</span><span class="sxs-lookup"><span data-stu-id="40590-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="40590-496">Поля файла оценкой ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="40590-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="40590-497">Column</span><span class="sxs-lookup"><span data-stu-id="40590-497">Column</span></span></th>
<th><span data-ttu-id="40590-498">Описание</span><span class="sxs-lookup"><span data-stu-id="40590-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="40590-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="40590-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="40590-500">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="40590-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="40590-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="40590-502">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="40590-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="40590-504">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="40590-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="40590-506">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="40590-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="40590-507">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="40590-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="40590-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="40590-509">Имя домена клиента.</span><span class="sxs-lookup"><span data-stu-id="40590-509">The customer’s domain name.</span></span> <span data-ttu-id="40590-510">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="40590-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-511">Страна или регион клиента</span><span class="sxs-lookup"><span data-stu-id="40590-511">Customer country</span></span></td>
<td><p><span data-ttu-id="40590-512">Страна или регион, где находится клиент.</span><span class="sxs-lookup"><span data-stu-id="40590-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="40590-513">MPNID</span></span></td>
<td><p><span data-ttu-id="40590-514">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="40590-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-515">Торговый посредник MPNID</span><span class="sxs-lookup"><span data-stu-id="40590-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="40590-516">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="40590-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40590-517">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="40590-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="40590-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="40590-519">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="40590-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="40590-520">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="40590-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-521">ProductID</span><span class="sxs-lookup"><span data-stu-id="40590-521">ProductId</span></span></td>
<td><p><span data-ttu-id="40590-522">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="40590-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="40590-523">SkuId</span></span></td>
<td><p><span data-ttu-id="40590-524">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="40590-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="40590-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="40590-526">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="40590-526">The ID for a particular Availability.</span></span> <span data-ttu-id="40590-527">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="40590-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-528">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="40590-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="40590-529">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="40590-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="40590-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="40590-531">Имя издателя.</span><span class="sxs-lookup"><span data-stu-id="40590-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="40590-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="40590-533">Идентификатор издателя, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="40590-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="40590-534">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="40590-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="40590-535">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="40590-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="40590-536">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="40590-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="40590-537">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="40590-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-538">Код подписки</span><span class="sxs-lookup"><span data-stu-id="40590-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="40590-539">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="40590-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="40590-540">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="40590-541">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="40590-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40590-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40590-543">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="40590-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="40590-544">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="40590-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40590-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40590-546">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="40590-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="40590-547">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="40590-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-548">Дата использования</span><span class="sxs-lookup"><span data-stu-id="40590-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="40590-549">Дата использования службы.</span><span class="sxs-lookup"><span data-stu-id="40590-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-550">Индикатор типа</span><span class="sxs-lookup"><span data-stu-id="40590-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="40590-551">Тип единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="40590-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-552">Категория счетчика</span><span class="sxs-lookup"><span data-stu-id="40590-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="40590-553">Служба верхнего уровня для использования.</span><span class="sxs-lookup"><span data-stu-id="40590-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-554">Идентификатор счетчика</span><span class="sxs-lookup"><span data-stu-id="40590-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="40590-555">Идентификатор для использования средства измерения.</span><span class="sxs-lookup"><span data-stu-id="40590-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-556">Подкатегория измерения</span><span class="sxs-lookup"><span data-stu-id="40590-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="40590-557">Тип службы Azure, которые могут повлиять на скорость.</span><span class="sxs-lookup"><span data-stu-id="40590-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-558">Имя единицы измерения</span><span class="sxs-lookup"><span data-stu-id="40590-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="40590-559">Единица измерения для использованного средства измерения.</span><span class="sxs-lookup"><span data-stu-id="40590-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-560">Регион счетчика</span><span class="sxs-lookup"><span data-stu-id="40590-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="40590-561">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="40590-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-562">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="40590-562">Unit</span></span></td>
<td><p><span data-ttu-id="40590-563">Единица имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="40590-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-564">Использованное количество</span><span class="sxs-lookup"><span data-stu-id="40590-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="40590-565">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="40590-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="40590-566">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="40590-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-567">Расположение ресурса</span><span class="sxs-lookup"><span data-stu-id="40590-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="40590-568">Центр обработки данных, где выполняется средства измерения.</span><span class="sxs-lookup"><span data-stu-id="40590-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-569">Используемой службы</span><span class="sxs-lookup"><span data-stu-id="40590-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="40590-570">Используемая служба платформы Azure.</span><span class="sxs-lookup"><span data-stu-id="40590-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-571">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="40590-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="40590-572">Группа ресурсов, в которой выполняется развернутое средство измерения.</span><span class="sxs-lookup"><span data-stu-id="40590-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-573">URI ресурса</span><span class="sxs-lookup"><span data-stu-id="40590-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="40590-574">URI ресурса, который используется.</span><span class="sxs-lookup"><span data-stu-id="40590-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-575">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="40590-575">Charge type</span></span></td>
<td><p><span data-ttu-id="40590-576">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="40590-576">The type of charge or adjustment.</span></span> <span data-ttu-id="40590-577">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="40590-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-578">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="40590-578">Unit price</span></span></td>
<td><p><span data-ttu-id="40590-579">Цена за лицензии, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="40590-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="40590-580">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-581">Количество</span><span class="sxs-lookup"><span data-stu-id="40590-581">Quantity</span></span></td>
<td><p><span data-ttu-id="40590-582">Количество лицензий.</span><span class="sxs-lookup"><span data-stu-id="40590-582">Number of licenses.</span></span> <span data-ttu-id="40590-583">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-584">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="40590-584">Unit type</span></span></td>
<td><p><span data-ttu-id="40590-585">Тип единицы измерения единицы измеряется объем использования.</span><span class="sxs-lookup"><span data-stu-id="40590-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="40590-586">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="40590-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-587">Налог pre выставления счетов</span><span class="sxs-lookup"><span data-stu-id="40590-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="40590-588">Общая сумма до налогов.</span><span class="sxs-lookup"><span data-stu-id="40590-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-589">Валюта для выставления счетов</span><span class="sxs-lookup"><span data-stu-id="40590-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="40590-590">Валюта в географическом регионе клиента</span><span class="sxs-lookup"><span data-stu-id="40590-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-591">Цены до выплаты налогов всего</span><span class="sxs-lookup"><span data-stu-id="40590-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="40590-592">Цены до налогов.</span><span class="sxs-lookup"><span data-stu-id="40590-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-593">Цены на валюту</span><span class="sxs-lookup"><span data-stu-id="40590-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="40590-594">Валюта, в прайс-листа.</span><span class="sxs-lookup"><span data-stu-id="40590-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-595">Сведения о службе 1</span><span class="sxs-lookup"><span data-stu-id="40590-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="40590-596">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="40590-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-597">Сведения о службе 2</span><span class="sxs-lookup"><span data-stu-id="40590-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="40590-598">Устаревшее поле, в которое записываются необязательные метаданные службы.</span><span class="sxs-lookup"><span data-stu-id="40590-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40590-599">Теги</span><span class="sxs-lookup"><span data-stu-id="40590-599">Tags</span></span></td>
<td><p><span data-ttu-id="40590-600">Теги, присваиваемый средству измерения в порядке для группировки записей выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="40590-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="40590-601">Например можно использовать теги для распределения затрат по отделу, который использует данное средство измерения.</span><span class="sxs-lookup"><span data-stu-id="40590-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40590-602">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="40590-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="40590-603">Любые дополнительные сведения, не включенные в другие столбцы.</span><span class="sxs-lookup"><span data-stu-id="40590-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="40590-604">Сопоставление платежей в счете и сверочном файле</span><span class="sxs-lookup"><span data-stu-id="40590-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="40590-605">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="40590-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="40590-606">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="40590-607">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="40590-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="40590-608">Одноразовые кредиты, скидки и возвраты денежных средств, которые отображаются в счете-фактуре как «Уточнения», не отображаются в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="40590-609">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="40590-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="40590-610"><strong>Описание платежа счета</strong></span><span class="sxs-lookup"><span data-stu-id="40590-610"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-611"><strong>Описание платежа сверочный файл (столбец ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="40590-611"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-612"><strong>Что такое эта плата?</strong></span><span class="sxs-lookup"><span data-stu-id="40590-612"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-613"><strong>Как сопоставить эти счетом в счет?</strong></span><span class="sxs-lookup"><span data-stu-id="40590-613"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="40590-614"><strong>Расходы на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="40590-614"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-615">Стоимость активации</span><span class="sxs-lookup"><span data-stu-id="40590-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-616">Сумма, взимаемая с клиента при использовании подписки после ее приобретения</span><span class="sxs-lookup"><span data-stu-id="40590-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="40590-617">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="40590-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-618">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="40590-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-619">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="40590-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-620">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="40590-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-621">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="40590-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-622">Пропорциональный перерасчет одного цикла</span><span class="sxs-lookup"><span data-stu-id="40590-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-623">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="40590-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-624">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="40590-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-625">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="40590-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-626">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="40590-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-627">Тип накладных расходов для подписки при использовании выставление счетов за год</span><span class="sxs-lookup"><span data-stu-id="40590-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-628">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="40590-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-629">Тип накладных расходов для подписки при использовании сумма ежемесячных счетов</span><span class="sxs-lookup"><span data-stu-id="40590-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-630">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="40590-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-631">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="40590-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="40590-632">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="40590-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-633">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="40590-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-634">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="40590-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-635">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="40590-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="40590-636"><strong>Плата за использование</strong></span><span class="sxs-lookup"><span data-stu-id="40590-636"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-637">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="40590-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-638">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="40590-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="40590-639">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="40590-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-640">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="40590-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-641">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="40590-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-642"><strong>Деньги на счете</strong></span><span class="sxs-lookup"><span data-stu-id="40590-642"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-643">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="40590-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-644">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="40590-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-645">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="40590-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="40590-646">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="40590-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="40590-647"><strong>Скидки на основе использования</strong></span><span class="sxs-lookup"><span data-stu-id="40590-647"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-648">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="40590-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-649">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="40590-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="40590-650">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="40590-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-651">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="40590-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-652">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="40590-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-653">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="40590-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-654">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="40590-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-655">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="40590-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-656">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="40590-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="40590-657"><strong>Скидки на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="40590-657"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-658"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="40590-658"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="40590-659">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="40590-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40590-660"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="40590-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-661"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="40590-661"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="40590-662"><em>Исключение: &quot;Смещение элемента строки&quot; уже включает в себя налоги. Деньги на счете, см. выше.</em></span><span class="sxs-lookup"><span data-stu-id="40590-662"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-663">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="40590-663">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="40590-664">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="40590-664">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="40590-665">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="40590-665">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
