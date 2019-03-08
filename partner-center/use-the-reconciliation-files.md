---
title: Использование файлов выверки | Центр партнеров
ms.topic: article
ms.date: 10/29/2018
description: Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 5ce9b7cd9ead08b7709c68a0e967d64e9f2a32bd
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57585137"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="35862-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="35862-103">Use the reconciliation files</span></span>

<span data-ttu-id="35862-104">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="35862-104">**Applies to**</span></span>

-  <span data-ttu-id="35862-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="35862-105">Partner Center</span></span>
-  <span data-ttu-id="35862-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="35862-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="35862-107">Для просмотра подробных строке каждой издержки в цикле выставления счетов скачайте сверочные файлы из центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="35862-108">Эти сведения включают оплаты за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="35862-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="35862-109">Детализировать партнером</span><span class="sxs-lookup"><span data-stu-id="35862-109">Itemize by partner</span></span>


<span data-ttu-id="35862-110">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="35862-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="35862-111">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="35862-111">MPN ID</span></span></th>
<th><span data-ttu-id="35862-112">Описание</span><span class="sxs-lookup"><span data-stu-id="35862-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="35862-113">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="35862-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="35862-114">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="35862-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-115">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="35862-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="35862-116">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="35862-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="35862-117">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="35862-118">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="35862-119">Просмотр позитивную или обновление торгового посредника, в меню центра партнеров выберите <strong>клиентов</strong>, затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="35862-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="35862-120">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="35862-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="35862-121">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="35862-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="35862-122">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="35862-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="35862-123">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="35862-124">Если партнер CSP удаляет идентификатор торгового посредника, это значение будет равно -1.</span><span class="sxs-lookup"><span data-stu-id="35862-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="35862-125">Поля файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="35862-125">License-based file fields</span></span>


<span data-ttu-id="35862-126">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="35862-127"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="35862-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="35862-128"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="35862-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="35862-129"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="35862-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="35862-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="35862-131">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="35862-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="35862-132">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="35862-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="35862-133">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="35862-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="35862-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="35862-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="35862-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="35862-136">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="35862-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="35862-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="35862-138">OrderID</span></span></td>
<td><p><span data-ttu-id="35862-139">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="35862-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="35862-140">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="35862-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="35862-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="35862-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="35862-143">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="35862-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="35862-144">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="35862-145">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="35862-146">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="35862-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="35862-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="35862-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="35862-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="35862-149">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="35862-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="35862-150">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="35862-151">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="35862-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="35862-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="35862-153">OfferID</span></span></td>
<td><p><span data-ttu-id="35862-154">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="35862-154">Unique offer ID.</span></span> <span data-ttu-id="35862-155">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="35862-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="35862-156"><b>Примечание</b>. Это значение не соответствует Идентификатору предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="35862-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="35862-157">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="35862-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="35862-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="35862-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="35862-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="35862-160">Уникальный идентификатор длительного предложения как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="35862-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="35862-161"><b>Примечание</b>. Это значение совпадает с Идентификатором предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="35862-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="35862-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="35862-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="35862-163">OfferName</span></span></td>
<td><p><span data-ttu-id="35862-164">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="35862-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="35862-165">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="35862-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="35862-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="35862-167">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="35862-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="35862-168">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="35862-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="35862-169">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="35862-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="35862-170">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="35862-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="35862-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="35862-172">Дата окончания подписки: 12 месяцев + x дней после даты начала (чтобы соответствовать выставления счетов даты партнера) или 12 месяцев с даты продления.</span><span class="sxs-lookup"><span data-stu-id="35862-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="35862-173">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="35862-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="35862-174">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="35862-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="35862-175">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="35862-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="35862-176">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="35862-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="35862-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="35862-178">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="35862-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="35862-179">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="35862-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="35862-180">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="35862-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="35862-181">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="35862-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="35862-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="35862-183">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="35862-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="35862-184">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="35862-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="35862-185">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="35862-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="35862-186">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="35862-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="35862-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="35862-188">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="35862-188">The type of charge or adjustment.</span></span> <span data-ttu-id="35862-189">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="35862-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="35862-190">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="35862-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="35862-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="35862-192">Цена за рабочее место, опубликованное в прайс-листе во время покупки.</span><span class="sxs-lookup"><span data-stu-id="35862-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="35862-193">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="35862-194">6,82</span><span class="sxs-lookup"><span data-stu-id="35862-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-195">Количество</span><span class="sxs-lookup"><span data-stu-id="35862-195">Quantity</span></span></td>
<td><p><span data-ttu-id="35862-196">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="35862-196">Number of seats.</span></span> <span data-ttu-id="35862-197">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="35862-198">2</span><span class="sxs-lookup"><span data-stu-id="35862-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-199">Сумма</span><span class="sxs-lookup"><span data-stu-id="35862-199">Amount</span></span></td>
<td><p><span data-ttu-id="35862-200">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="35862-200">Total of price for quantity.</span></span> <span data-ttu-id="35862-201">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="35862-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="35862-202">13,32</span><span class="sxs-lookup"><span data-stu-id="35862-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="35862-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="35862-204">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="35862-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="35862-205">IUR или новые подписки, на которые распространяются вознаграждения, будут также содержать сумму скидки в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="35862-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="35862-206">2,32</span><span class="sxs-lookup"><span data-stu-id="35862-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-207">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="35862-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="35862-208">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="35862-208">Total before tax.</span></span> <span data-ttu-id="35862-209">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="35862-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="35862-210">11</span><span class="sxs-lookup"><span data-stu-id="35862-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-211">Налог</span><span class="sxs-lookup"><span data-stu-id="35862-211">Tax</span></span></td>
<td><p><span data-ttu-id="35862-212">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="35862-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="35862-213">0</span><span class="sxs-lookup"><span data-stu-id="35862-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="35862-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="35862-215">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="35862-215">Total after tax.</span></span> <span data-ttu-id="35862-216">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="35862-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="35862-217">11</span><span class="sxs-lookup"><span data-stu-id="35862-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-218">Валюта</span><span class="sxs-lookup"><span data-stu-id="35862-218">Currency</span></span></td>
<td><p><span data-ttu-id="35862-219">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="35862-219">Currency type.</span></span> <span data-ttu-id="35862-220">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="35862-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="35862-221">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="35862-222">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="35862-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="35862-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="35862-224">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="35862-225">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="35862-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="35862-226">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="35862-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="35862-227">MPNID</span></span></td>
<td><p><span data-ttu-id="35862-228">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="35862-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="35862-229">4390934</span><span class="sxs-lookup"><span data-stu-id="35862-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="35862-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="35862-231">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="35862-232">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="35862-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="35862-233">4390934</span><span class="sxs-lookup"><span data-stu-id="35862-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="35862-234">DomainName</span></span></td>
<td><p><span data-ttu-id="35862-235">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="35862-236">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="35862-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="35862-237">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="35862-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="35862-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="35862-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="35862-240">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-240">Subscription nickname.</span></span> <span data-ttu-id="35862-241">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="35862-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="35862-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="35862-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="35862-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="35862-244">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="35862-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="35862-245">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="35862-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="35862-246">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="35862-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="35862-247">Поля файла на основе использования</span><span class="sxs-lookup"><span data-stu-id="35862-247">Usage-based file fields</span></span>


<span data-ttu-id="35862-248">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="35862-249">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="35862-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="35862-250"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="35862-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="35862-251"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="35862-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="35862-252"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="35862-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="35862-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="35862-254">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="35862-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="35862-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="35862-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="35862-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="35862-257">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="35862-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="35862-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="35862-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="35862-260">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="35862-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="35862-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="35862-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="35862-263">Клиент&#39;имя_организации s, указанное в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="35862-264">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="35862-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="35862-265">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="35862-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="35862-266">MPNID</span></span></td>
<td><p><span data-ttu-id="35862-267">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="35862-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="35862-268">4390934</span><span class="sxs-lookup"><span data-stu-id="35862-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="35862-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="35862-270">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="35862-271">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="35862-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="35862-272">4390934</span><span class="sxs-lookup"><span data-stu-id="35862-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="35862-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="35862-274">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="35862-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="35862-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="35862-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="35862-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="35862-277">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="35862-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="35862-278">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="35862-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="35862-279">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="35862-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="35862-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="35862-281">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="35862-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="35862-282">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="35862-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="35862-283">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="35862-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="35862-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="35862-285">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="35862-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="35862-286">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="35862-287">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="35862-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="35862-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="35862-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="35862-290">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="35862-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="35862-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="35862-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="35862-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="35862-293">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="35862-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="35862-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="35862-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="35862-295">OrderID</span></span></td>
<td><p><span data-ttu-id="35862-296">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="35862-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="35862-297">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="35862-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="35862-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="35862-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="35862-300">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="35862-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="35862-301">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="35862-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="35862-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="35862-303">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="35862-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="35862-304">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="35862-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="35862-305">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="35862-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="35862-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="35862-307">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="35862-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="35862-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="35862-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-309">Resource Name</span><span class="sxs-lookup"><span data-stu-id="35862-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="35862-310">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="35862-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="35862-311">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="35862-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="35862-312">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="35862-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-313">Region</span><span class="sxs-lookup"><span data-stu-id="35862-313">Region</span></span></td>
<td><p><span data-ttu-id="35862-314">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="35862-314">The region the usage applies to.</span></span> <span data-ttu-id="35862-315">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="35862-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="35862-316">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="35862-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-317">SKU</span><span class="sxs-lookup"><span data-stu-id="35862-317">SKU</span></span></td>
<td><p><span data-ttu-id="35862-318">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="35862-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="35862-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="35862-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="35862-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="35862-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="35862-321">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="35862-322">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним — другой.</span><span class="sxs-lookup"><span data-stu-id="35862-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="35862-323">1</span><span class="sxs-lookup"><span data-stu-id="35862-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="35862-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="35862-325">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="35862-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="35862-326">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="35862-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="35862-327">11</span><span class="sxs-lookup"><span data-stu-id="35862-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="35862-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="35862-329">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="35862-329">Units included as part of the offer.</span></span> <span data-ttu-id="35862-330">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="35862-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="35862-331">0</span><span class="sxs-lookup"><span data-stu-id="35862-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="35862-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="35862-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="35862-333">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="35862-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="35862-334">Равняется разнице значений полей ConsumedQuantity и IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="35862-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="35862-335">11</span><span class="sxs-lookup"><span data-stu-id="35862-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="35862-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="35862-337">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="35862-338">0,0808 долл. США</span><span class="sxs-lookup"><span data-stu-id="35862-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="35862-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="35862-340">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="35862-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="35862-341">0,085 долл. США</span><span class="sxs-lookup"><span data-stu-id="35862-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="35862-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="35862-343">Начисление суммы на вашем рынке основе&#39;s налога по налоговым правилам и определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="35862-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="35862-344">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="35862-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="35862-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="35862-346">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="35862-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="35862-347">0,93 долл. США</span><span class="sxs-lookup"><span data-stu-id="35862-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-348">Валюта</span><span class="sxs-lookup"><span data-stu-id="35862-348">Currency</span></span></td>
<td><p><span data-ttu-id="35862-349">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="35862-349">Currency type.</span></span> <span data-ttu-id="35862-350">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="35862-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="35862-351">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="35862-352">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="35862-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="35862-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="35862-354">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="35862-354">Pretax price per unit.</span></span> <span data-ttu-id="35862-355">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="35862-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="35862-356">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="35862-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="35862-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="35862-358">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="35862-358">Post tax price per unit.</span></span> <span data-ttu-id="35862-359">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="35862-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="35862-360">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="35862-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="35862-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="35862-362">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="35862-362">The type of charge or adjustment.</span></span> <span data-ttu-id="35862-363">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="35862-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="35862-364">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="35862-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="35862-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="35862-366">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="35862-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="35862-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="35862-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="35862-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="35862-369">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="35862-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="35862-370">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="35862-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="35862-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="35862-372">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="35862-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="35862-373">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="35862-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-374">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="35862-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="35862-375">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="35862-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="35862-376">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="35862-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="35862-377">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="35862-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="35862-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="35862-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="35862-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="35862-380">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="35862-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="35862-381">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="35862-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-382">Проект</span><span class="sxs-lookup"><span data-stu-id="35862-382">Project</span></span></td>
<td><p><span data-ttu-id="35862-383">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="35862-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="35862-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="35862-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="35862-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="35862-386">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="35862-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="35862-387">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="35862-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="35862-388">Если имеется 25 пакетов подключений служебной шины подготовлено, и вы использовалось 1 в течение этого дня, инструкцию ежедневное использование за этот день означает «25 подключений / 30 дней — использовано: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="35862-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="35862-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="35862-390">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="35862-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="35862-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="35862-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="35862-392">DomainName</span></span></td>
<td><p><span data-ttu-id="35862-393">Клиент&#39;s доменное имя, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="35862-394">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="35862-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="35862-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="35862-396">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="35862-396">Unit</span></span></td>
<td><p><span data-ttu-id="35862-397">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="35862-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="35862-398">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="35862-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="35862-399">Файл одноразовые и повторяющиеся поля</span><span class="sxs-lookup"><span data-stu-id="35862-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="35862-400">Column</span><span class="sxs-lookup"><span data-stu-id="35862-400">Column</span></span></th>
<th><span data-ttu-id="35862-401">Описание</span><span class="sxs-lookup"><span data-stu-id="35862-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="35862-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="35862-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="35862-403">Уникальный идентификатор клиента Microsoft Azure Active Directory для конкретной сущности выставления счетов, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="35862-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="35862-404">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="35862-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="35862-405">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="35862-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-406">Идентификатор клиента</span><span class="sxs-lookup"><span data-stu-id="35862-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="35862-407">Уникальный Microsoft Azure Active Directory идентификатор клиента, в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-408">Customer Name (Имя клиента)</span><span class="sxs-lookup"><span data-stu-id="35862-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="35862-409">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="35862-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="35862-411">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="35862-412">Это не должно использоваться для уникальной идентификации клиента, как клиент или партнер можно обновить домен именного/по умолчанию на портале Office 365.</span><span class="sxs-lookup"><span data-stu-id="35862-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="35862-413">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-414">Страна клиента</span><span class="sxs-lookup"><span data-stu-id="35862-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="35862-415">Страна, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="35862-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-416">Номер счета</span><span class="sxs-lookup"><span data-stu-id="35862-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="35862-417">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="35862-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="35862-418">MpnId</span></span></td>
<td><p><span data-ttu-id="35862-419">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="35862-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-420">MpnId торгового посредника</span><span class="sxs-lookup"><span data-stu-id="35862-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="35862-421">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-422">Идентификатор заказа</span><span class="sxs-lookup"><span data-stu-id="35862-422">Order ID</span></span></td>
<td><p><span data-ttu-id="35862-423">Уникальный идентификатор заказа на платформе Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="35862-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="35862-424">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-425">Дата заказа</span><span class="sxs-lookup"><span data-stu-id="35862-425">Order date</span></span></td>
<td><p><span data-ttu-id="35862-426">Дата размещения заказа.</span><span class="sxs-lookup"><span data-stu-id="35862-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-427">ProductID</span><span class="sxs-lookup"><span data-stu-id="35862-427">ProductId</span></span></td>
<td><p><span data-ttu-id="35862-428">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="35862-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="35862-429">SkuId</span></span></td>
<td><p><span data-ttu-id="35862-430">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="35862-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="35862-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="35862-432">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="35862-432">The ID for a particular Availability.</span></span> <span data-ttu-id="35862-433">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="35862-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-434">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="35862-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="35862-435">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="35862-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-436">название продукта;</span><span class="sxs-lookup"><span data-stu-id="35862-436">Product name</span></span></td>
<td><p><span data-ttu-id="35862-437">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="35862-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="35862-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="35862-439">Имя издателя продукта.</span><span class="sxs-lookup"><span data-stu-id="35862-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="35862-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="35862-441">Уникальный идентификатор для данного издателя.</span><span class="sxs-lookup"><span data-stu-id="35862-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-442">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="35862-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="35862-443">Понятное имя подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-444">Код подписки</span><span class="sxs-lookup"><span data-stu-id="35862-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="35862-445">Уникальный идентификатор для подписки на платформу Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="35862-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="35862-446">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="35862-447">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="35862-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="35862-449">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="35862-449">Start day of the charges.</span></span> <span data-ttu-id="35862-450">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="35862-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="35862-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="35862-452">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="35862-452">End day of the charges.</span></span> <span data-ttu-id="35862-453">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="35862-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-454">Термин и Billingcycle</span><span class="sxs-lookup"><span data-stu-id="35862-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="35862-455">Продолжительность срока и цикла выставления счетов за покупки.</span><span class="sxs-lookup"><span data-stu-id="35862-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="35862-456">Например «1 год, месяц.»</span><span class="sxs-lookup"><span data-stu-id="35862-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-457">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="35862-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="35862-458">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="35862-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-459">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="35862-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="35862-460">Цена, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="35862-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="35862-461">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-462">Эффективное модульное цена</span><span class="sxs-lookup"><span data-stu-id="35862-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="35862-463">Цена за единицу после изменения.</span><span class="sxs-lookup"><span data-stu-id="35862-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-464">Количество</span><span class="sxs-lookup"><span data-stu-id="35862-464">Quantity</span></span></td>
<td><p><span data-ttu-id="35862-465">Число единиц.</span><span class="sxs-lookup"><span data-stu-id="35862-465">Number of units.</span></span> <span data-ttu-id="35862-466">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-467">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="35862-467">Unit type</span></span></td>
<td><p><span data-ttu-id="35862-468">Тип приобретенная единица.</span><span class="sxs-lookup"><span data-stu-id="35862-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="35862-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="35862-470">Объяснение применяемой скидки.</span><span class="sxs-lookup"><span data-stu-id="35862-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-471">Итого</span><span class="sxs-lookup"><span data-stu-id="35862-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="35862-472">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="35862-472">Total before tax.</span></span> <span data-ttu-id="35862-473">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="35862-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-474">Общая сумма налога</span><span class="sxs-lookup"><span data-stu-id="35862-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="35862-475">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="35862-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-476">Total (Всего)</span><span class="sxs-lookup"><span data-stu-id="35862-476">Total</span></span></td>
<td><p><span data-ttu-id="35862-477">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="35862-477">Total after tax.</span></span> <span data-ttu-id="35862-478">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="35862-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-479">Валюта</span><span class="sxs-lookup"><span data-stu-id="35862-479">Currency</span></span></td>
<td><p><span data-ttu-id="35862-480">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="35862-480">Currency type.</span></span> <span data-ttu-id="35862-481">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="35862-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="35862-482">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-483">Альтернативного имени пользователя</span><span class="sxs-lookup"><span data-stu-id="35862-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="35862-484">Альтернативный идентификатор с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="35862-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="35862-485">Поля файла оценкой ежедневного использования</span><span class="sxs-lookup"><span data-stu-id="35862-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="35862-486">Column</span><span class="sxs-lookup"><span data-stu-id="35862-486">Column</span></span></th>
<th><span data-ttu-id="35862-487">Описание</span><span class="sxs-lookup"><span data-stu-id="35862-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="35862-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="35862-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="35862-489">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="35862-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="35862-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="35862-491">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="35862-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="35862-493">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="35862-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="35862-495">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="35862-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="35862-496">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="35862-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="35862-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="35862-498">Имя домена клиента.</span><span class="sxs-lookup"><span data-stu-id="35862-498">The customer’s domain name.</span></span> <span data-ttu-id="35862-499">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="35862-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-500">Страна клиента</span><span class="sxs-lookup"><span data-stu-id="35862-500">Customer country</span></span></td>
<td><p><span data-ttu-id="35862-501">Страна, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="35862-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="35862-502">MPNID</span></span></td>
<td><p><span data-ttu-id="35862-503">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="35862-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-504">Торговый посредник MPNID</span><span class="sxs-lookup"><span data-stu-id="35862-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="35862-505">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="35862-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="35862-506">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="35862-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="35862-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="35862-508">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="35862-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="35862-509">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="35862-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-510">ProductID</span><span class="sxs-lookup"><span data-stu-id="35862-510">ProductId</span></span></td>
<td><p><span data-ttu-id="35862-511">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="35862-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="35862-512">SkuId</span></span></td>
<td><p><span data-ttu-id="35862-513">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="35862-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="35862-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="35862-515">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="35862-515">The ID for a particular Availability.</span></span> <span data-ttu-id="35862-516">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="35862-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-517">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="35862-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="35862-518">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="35862-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="35862-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="35862-520">Имя издателя.</span><span class="sxs-lookup"><span data-stu-id="35862-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="35862-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="35862-522">Идентификатор издателя, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="35862-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="35862-523">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="35862-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="35862-524">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="35862-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="35862-525">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="35862-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="35862-526">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="35862-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-527">Код подписки</span><span class="sxs-lookup"><span data-stu-id="35862-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="35862-528">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="35862-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="35862-529">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="35862-530">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="35862-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="35862-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="35862-532">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="35862-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="35862-533">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="35862-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="35862-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="35862-535">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="35862-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="35862-536">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="35862-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-537">Дата использования</span><span class="sxs-lookup"><span data-stu-id="35862-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="35862-538">Дата использования службы.</span><span class="sxs-lookup"><span data-stu-id="35862-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-539">Индикатор типа</span><span class="sxs-lookup"><span data-stu-id="35862-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="35862-540">Тип единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="35862-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-541">Категория счетчика</span><span class="sxs-lookup"><span data-stu-id="35862-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="35862-542">Служба верхнего уровня для использования.</span><span class="sxs-lookup"><span data-stu-id="35862-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-543">Идентификатор счетчика</span><span class="sxs-lookup"><span data-stu-id="35862-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="35862-544">Идентификатор для использования средства измерения.</span><span class="sxs-lookup"><span data-stu-id="35862-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-545">Подкатегория измерения</span><span class="sxs-lookup"><span data-stu-id="35862-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="35862-546">Тип службы Azure, которые могут повлиять на скорость.</span><span class="sxs-lookup"><span data-stu-id="35862-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-547">Имя единицы измерения</span><span class="sxs-lookup"><span data-stu-id="35862-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="35862-548">Единица измерения для использованного средства измерения.</span><span class="sxs-lookup"><span data-stu-id="35862-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-549">Регион счетчика</span><span class="sxs-lookup"><span data-stu-id="35862-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="35862-550">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="35862-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-551">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="35862-551">Unit</span></span></td>
<td><p><span data-ttu-id="35862-552">Единица имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="35862-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-553">Использованное количество</span><span class="sxs-lookup"><span data-stu-id="35862-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="35862-554">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="35862-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="35862-555">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="35862-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-556">Расположение ресурса</span><span class="sxs-lookup"><span data-stu-id="35862-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="35862-557">Центр обработки данных, где выполняется средства измерения.</span><span class="sxs-lookup"><span data-stu-id="35862-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-558">Используемой службы</span><span class="sxs-lookup"><span data-stu-id="35862-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="35862-559">Используемая служба платформы Azure.</span><span class="sxs-lookup"><span data-stu-id="35862-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-560">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="35862-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="35862-561">Группа ресурсов, в которой выполняется развернутое средство измерения.</span><span class="sxs-lookup"><span data-stu-id="35862-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-562">URI ресурса</span><span class="sxs-lookup"><span data-stu-id="35862-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="35862-563">URI ресурса, который используется.</span><span class="sxs-lookup"><span data-stu-id="35862-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-564">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="35862-564">Charge type</span></span></td>
<td><p><span data-ttu-id="35862-565">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="35862-565">The type of charge or adjustment.</span></span> <span data-ttu-id="35862-566">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="35862-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-567">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="35862-567">Unit price</span></span></td>
<td><p><span data-ttu-id="35862-568">Цена за лицензии, опубликованной в прайс-лист во время покупки.</span><span class="sxs-lookup"><span data-stu-id="35862-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="35862-569">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-570">Количество</span><span class="sxs-lookup"><span data-stu-id="35862-570">Quantity</span></span></td>
<td><p><span data-ttu-id="35862-571">Количество лицензий.</span><span class="sxs-lookup"><span data-stu-id="35862-571">Number of licenses.</span></span> <span data-ttu-id="35862-572">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-573">Тип единицы измерения</span><span class="sxs-lookup"><span data-stu-id="35862-573">Unit type</span></span></td>
<td><p><span data-ttu-id="35862-574">Тип единицы измерения единицы измеряется объем использования.</span><span class="sxs-lookup"><span data-stu-id="35862-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="35862-575">Недоступно для текущего действия.</span><span class="sxs-lookup"><span data-stu-id="35862-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-576">Налог pre выставления счетов</span><span class="sxs-lookup"><span data-stu-id="35862-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="35862-577">Общая сумма до налогов.</span><span class="sxs-lookup"><span data-stu-id="35862-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-578">Валюта для выставления счетов</span><span class="sxs-lookup"><span data-stu-id="35862-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="35862-579">Валюта в географическом регионе клиента</span><span class="sxs-lookup"><span data-stu-id="35862-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-580">Цены до выплаты налогов всего</span><span class="sxs-lookup"><span data-stu-id="35862-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="35862-581">Цены до налогов.</span><span class="sxs-lookup"><span data-stu-id="35862-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-582">Цены на валюту</span><span class="sxs-lookup"><span data-stu-id="35862-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="35862-583">Валюта, в прайс-листа.</span><span class="sxs-lookup"><span data-stu-id="35862-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-584">Сведения о службе 1</span><span class="sxs-lookup"><span data-stu-id="35862-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="35862-585">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="35862-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-586">Сведения о службе 2</span><span class="sxs-lookup"><span data-stu-id="35862-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="35862-587">Устаревшее поле, в которое записываются необязательные метаданные службы.</span><span class="sxs-lookup"><span data-stu-id="35862-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="35862-588">Теги</span><span class="sxs-lookup"><span data-stu-id="35862-588">Tags</span></span></td>
<td><p><span data-ttu-id="35862-589">Теги, присваиваемый средству измерения в порядке для группировки записей выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="35862-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="35862-590">Например можно использовать теги для распределения затрат по отделу, который использует данное средство измерения.</span><span class="sxs-lookup"><span data-stu-id="35862-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="35862-591">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="35862-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="35862-592">Любые дополнительные сведения, не включенные в другие столбцы.</span><span class="sxs-lookup"><span data-stu-id="35862-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="35862-593">Сопоставление платежей в счете и сверочном файле</span><span class="sxs-lookup"><span data-stu-id="35862-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="35862-594">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="35862-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="35862-595">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="35862-596">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="35862-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="35862-597">Одноразовые кредиты, скидки и возвраты денежных средств, которые отображаются в счете-фактуре как «Уточнения», не отображаются в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="35862-598">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="35862-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="35862-599"><strong>Описание платежа счета</strong></span><span class="sxs-lookup"><span data-stu-id="35862-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-600"><strong>Описание платежа сверочный файл (столбец ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="35862-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-601"><strong>Что такое эта плата?</strong></span><span class="sxs-lookup"><span data-stu-id="35862-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-602"><strong>Как сопоставить эти счетом в счет?</strong></span><span class="sxs-lookup"><span data-stu-id="35862-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="35862-603"><strong>Расходы на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="35862-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-604">Стоимость активации</span><span class="sxs-lookup"><span data-stu-id="35862-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-605">Сумма, взимаемая с клиента при использовании подписки после ее приобретения</span><span class="sxs-lookup"><span data-stu-id="35862-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="35862-606">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="35862-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-607">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="35862-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-608">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="35862-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-609">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="35862-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-610">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="35862-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-611">Пропорциональный перерасчет одного цикла</span><span class="sxs-lookup"><span data-stu-id="35862-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-612">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="35862-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-613">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="35862-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-614">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="35862-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-615">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="35862-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-616">Тип накладных расходов для подписки при использовании выставление счетов за год</span><span class="sxs-lookup"><span data-stu-id="35862-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-617">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="35862-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-618">Тип накладных расходов для подписки при использовании сумма ежемесячных счетов</span><span class="sxs-lookup"><span data-stu-id="35862-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-619">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="35862-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-620">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="35862-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="35862-621">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="35862-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-622">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="35862-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-623">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="35862-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-624">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="35862-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="35862-625"><strong>Плата за использование</strong></span><span class="sxs-lookup"><span data-stu-id="35862-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-626">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="35862-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-627">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="35862-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="35862-628">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="35862-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-629">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="35862-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-630">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="35862-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-631"><strong>Деньги на счете</strong></span><span class="sxs-lookup"><span data-stu-id="35862-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-632">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="35862-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-633">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="35862-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-634">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="35862-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="35862-635">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="35862-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="35862-636"><strong>Скидки на основе использования</strong></span><span class="sxs-lookup"><span data-stu-id="35862-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-637">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="35862-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-638">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="35862-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="35862-639">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="35862-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-640">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="35862-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-641">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="35862-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-642">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="35862-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-643">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="35862-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-644">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="35862-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-645">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="35862-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="35862-646"><strong>Скидки на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="35862-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-647"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="35862-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="35862-648">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="35862-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="35862-649"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="35862-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-650"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="35862-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="35862-651"><em>Исключение: &quot;Смещение элемента строки&quot; уже включает в себя налоги. Деньги на счете, см. выше.</em></span><span class="sxs-lookup"><span data-stu-id="35862-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-652">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="35862-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="35862-653">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="35862-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="35862-654">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="35862-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
