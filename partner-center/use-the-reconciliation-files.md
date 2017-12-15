---
title: "Использование файлов выверки | Центр партнеров"
description: "Для просмотра подробных сведений строковых элементов каждой оплаты в расчетном цикле, загрузите файлы выверки с информационной панели в Центре партнеров."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 892204ebcdfe1e1318985f2d50df8af2238bd4c1
ms.sourcegitcommit: 2436cb77fbefc41cc9cb3e62e8a616b6326c557f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2017
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="800a4-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="800a4-103">Use the reconciliation files</span></span>

**<span data-ttu-id="800a4-104">Относится к:</span><span class="sxs-lookup"><span data-stu-id="800a4-104">Applies to</span></span>**

-  <span data-ttu-id="800a4-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="800a4-105">Partner Center</span></span>
-  <span data-ttu-id="800a4-106">Центр партнеров для Microsoft Cloud для правительства США</span><span class="sxs-lookup"><span data-stu-id="800a4-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="800a4-107">Центр партнеров Microsoft Cloud для Германии</span><span class="sxs-lookup"><span data-stu-id="800a4-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="800a4-108">Для просмотра подробных сведений строковых элементов каждой оплаты в расчетном цикле, загрузите файлы выверки с информационной панели в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="800a4-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="800a4-109">Эти сведения включают плату за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="800a4-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="800a4-110">Детализация по партнерам</span><span class="sxs-lookup"><span data-stu-id="800a4-110">Itemize by partner</span></span>


<span data-ttu-id="800a4-111">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="800a4-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="800a4-112">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="800a4-112">MPN ID</span></span></th>
<th><span data-ttu-id="800a4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="800a4-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="800a4-114">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="800a4-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="800a4-115">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="800a4-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-116">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="800a4-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="800a4-117">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="800a4-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="800a4-118">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="800a4-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="800a4-119">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="800a4-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="800a4-120">Чтобы просмотреть или обновить сведения о торговом посреднике, выберите раздел <strong>Клиенты</strong> в меню Центра партнеров, после чего выберите нужного клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="800a4-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="800a4-121">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="800a4-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="800a4-122">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="800a4-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="800a4-123">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="800a4-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="800a4-124">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="800a4-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="800a4-125">Если партнер CSP удаляет идентификатор торгового посредника, это значение будет равно -1.</span><span class="sxs-lookup"><span data-stu-id="800a4-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="800a4-126">Поля файла на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="800a4-126">License-based file fields</span></span>


<span data-ttu-id="800a4-127">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="800a4-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="800a4-128">Столбец</span><span class="sxs-lookup"><span data-stu-id="800a4-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="800a4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="800a4-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="800a4-130">Пример значения</span><span class="sxs-lookup"><span data-stu-id="800a4-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="800a4-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="800a4-132">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="800a4-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="800a4-133">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="800a4-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="800a4-134">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="800a4-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="800a4-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="800a4-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="800a4-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="800a4-137">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="800a4-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="800a4-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="800a4-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="800a4-139">OrderID</span></span></td>
<td><p><span data-ttu-id="800a4-140">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="800a4-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="800a4-141">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="800a4-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="800a4-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="800a4-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="800a4-144">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="800a4-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="800a4-145">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="800a4-146">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="800a4-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="800a4-147">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="800a4-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="800a4-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="800a4-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="800a4-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="800a4-150">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="800a4-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="800a4-151">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="800a4-152">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="800a4-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="800a4-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="800a4-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="800a4-154">OfferID</span></span></td>
<td><p><span data-ttu-id="800a4-155">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="800a4-155">Unique offer ID.</span></span> <span data-ttu-id="800a4-156">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="800a4-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="800a4-157"><b>Примечание</b>: это значение не соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="800a4-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="800a4-158">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="800a4-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="800a4-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="800a4-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="800a4-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="800a4-161">Уникальный идентификатор длительного предложения, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="800a4-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="800a4-162"><b>Примечание</b>. Это значение соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="800a4-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="800a4-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="800a4-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="800a4-164">OfferName</span></span></td>
<td><p><span data-ttu-id="800a4-165">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="800a4-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="800a4-166">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="800a4-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="800a4-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="800a4-168">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="800a4-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="800a4-169">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="800a4-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="800a4-170">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="800a4-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="800a4-171">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="800a4-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="800a4-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="800a4-173">Дата завершения подписки — 12 месяцев + x дней после даты начала (чтобы совместить с датой выставления счетов партнера) или 12 месяцев от даты возобновления действия.</span><span class="sxs-lookup"><span data-stu-id="800a4-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="800a4-174">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="800a4-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="800a4-175">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="800a4-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="800a4-176">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="800a4-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="800a4-177">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="800a4-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="800a4-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="800a4-179">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="800a4-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="800a4-180">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="800a4-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="800a4-181">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="800a4-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="800a4-182">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="800a4-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="800a4-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="800a4-184">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="800a4-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="800a4-185">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="800a4-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="800a4-186">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="800a4-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="800a4-187">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="800a4-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="800a4-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="800a4-189">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="800a4-189">The type of charge or adjustment.</span></span> <span data-ttu-id="800a4-190">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="800a4-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="800a4-191">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="800a4-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="800a4-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="800a4-193">Цена за место.</span><span class="sxs-lookup"><span data-stu-id="800a4-193">Price per seat.</span></span> <span data-ttu-id="800a4-194">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="800a4-195">6,82</span><span class="sxs-lookup"><span data-stu-id="800a4-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="800a4-196">Quantity</span></span></td>
<td><p><span data-ttu-id="800a4-197">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="800a4-197">Number of seats.</span></span> <span data-ttu-id="800a4-198">Убедитесь, что оно соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="800a4-199">2</span><span class="sxs-lookup"><span data-stu-id="800a4-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-200">Amount</span><span class="sxs-lookup"><span data-stu-id="800a4-200">Amount</span></span></td>
<td><p><span data-ttu-id="800a4-201">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="800a4-201">Total of price for quantity.</span></span> <span data-ttu-id="800a4-202">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="800a4-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="800a4-203">13,32</span><span class="sxs-lookup"><span data-stu-id="800a4-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="800a4-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="800a4-205">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="800a4-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="800a4-206">IUR или новые подписки, на которые распространяются вознаграждения, будут также содержать сумму скидки в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="800a4-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="800a4-207">2,32</span><span class="sxs-lookup"><span data-stu-id="800a4-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="800a4-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="800a4-209">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="800a4-209">Total before tax.</span></span> <span data-ttu-id="800a4-210">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="800a4-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="800a4-211">11</span><span class="sxs-lookup"><span data-stu-id="800a4-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-212">Tax</span><span class="sxs-lookup"><span data-stu-id="800a4-212">Tax</span></span></td>
<td><p><span data-ttu-id="800a4-213">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="800a4-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="800a4-214">0</span><span class="sxs-lookup"><span data-stu-id="800a4-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="800a4-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="800a4-216">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="800a4-216">Total after tax.</span></span> <span data-ttu-id="800a4-217">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="800a4-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="800a4-218">11</span><span class="sxs-lookup"><span data-stu-id="800a4-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-219">Currency</span><span class="sxs-lookup"><span data-stu-id="800a4-219">Currency</span></span></td>
<td><p><span data-ttu-id="800a4-220">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="800a4-220">Currency type.</span></span> <span data-ttu-id="800a4-221">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="800a4-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="800a4-222">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="800a4-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="800a4-223">EUR</span><span class="sxs-lookup"><span data-stu-id="800a4-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="800a4-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="800a4-225">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="800a4-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="800a4-226">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="800a4-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="800a4-227">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="800a4-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="800a4-228">MPNID</span></span></td>
<td><p><span data-ttu-id="800a4-229">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="800a4-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="800a4-230">4390934</span><span class="sxs-lookup"><span data-stu-id="800a4-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="800a4-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="800a4-232">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="800a4-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="800a4-233">См. раздел [Детализация по партнерам](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="800a4-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="800a4-234">4390934</span><span class="sxs-lookup"><span data-stu-id="800a4-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="800a4-235">DomainName</span></span></td>
<td><p><span data-ttu-id="800a4-236">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="800a4-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="800a4-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="800a4-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="800a4-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="800a4-239">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="800a4-239">Subscription nickname.</span></span> <span data-ttu-id="800a4-240">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="800a4-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="800a4-241">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="800a4-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="800a4-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="800a4-243">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="800a4-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="800a4-244">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="800a4-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="800a4-245">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="800a4-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="800a4-246">Поля файла с учетом использования</span><span class="sxs-lookup"><span data-stu-id="800a4-246">Usage-based file fields</span></span>


<span data-ttu-id="800a4-247">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="800a4-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="800a4-248">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="800a4-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="800a4-249">Столбец</span><span class="sxs-lookup"><span data-stu-id="800a4-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="800a4-250">Описание</span><span class="sxs-lookup"><span data-stu-id="800a4-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="800a4-251">Пример значения</span><span class="sxs-lookup"><span data-stu-id="800a4-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="800a4-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="800a4-253">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="800a4-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="800a4-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="800a4-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="800a4-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="800a4-256">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="800a4-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="800a4-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="800a4-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="800a4-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="800a4-259">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="800a4-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="800a4-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="800a4-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="800a4-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="800a4-262">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="800a4-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="800a4-263">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="800a4-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="800a4-264">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="800a4-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="800a4-265">MPNID</span></span></td>
<td><p><span data-ttu-id="800a4-266">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="800a4-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="800a4-267">4390934</span><span class="sxs-lookup"><span data-stu-id="800a4-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="800a4-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="800a4-269">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="800a4-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="800a4-270">См. раздел [Детализация по партнерам](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="800a4-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="800a4-271">4390934</span><span class="sxs-lookup"><span data-stu-id="800a4-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="800a4-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="800a4-273">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="800a4-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="800a4-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="800a4-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="800a4-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="800a4-276">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="800a4-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="800a4-277">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="800a4-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="800a4-278">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="800a4-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="800a4-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="800a4-280">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="800a4-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="800a4-281">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="800a4-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="800a4-282">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="800a4-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="800a4-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="800a4-284">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="800a4-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="800a4-285">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="800a4-286">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="800a4-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="800a4-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="800a4-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="800a4-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="800a4-289">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="800a4-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="800a4-290">Платформа Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="800a4-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="800a4-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="800a4-292">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="800a4-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="800a4-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="800a4-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="800a4-294">OrderID</span></span></td>
<td><p><span data-ttu-id="800a4-295">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="800a4-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="800a4-296">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="800a4-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="800a4-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="800a4-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="800a4-299">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="800a4-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="800a4-300">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="800a4-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="800a4-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="800a4-302">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="800a4-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="800a4-303">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="800a4-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="800a4-304">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="800a4-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="800a4-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="800a4-306">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="800a4-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="800a4-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="800a4-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-308">Resource Name</span><span class="sxs-lookup"><span data-stu-id="800a4-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="800a4-309">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="800a4-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="800a4-310">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="800a4-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="800a4-311">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="800a4-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-312">Регион</span><span class="sxs-lookup"><span data-stu-id="800a4-312">Region</span></span></td>
<td><p><span data-ttu-id="800a4-313">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="800a4-313">The region the usage applies to.</span></span> <span data-ttu-id="800a4-314">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="800a4-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="800a4-315">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="800a4-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-316">SKU</span><span class="sxs-lookup"><span data-stu-id="800a4-316">SKU</span></span></td>
<td><p><span data-ttu-id="800a4-317">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="800a4-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="800a4-318">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="800a4-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="800a4-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="800a4-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="800a4-320">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="800a4-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="800a4-321">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним— другой.</span><span class="sxs-lookup"><span data-stu-id="800a4-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="800a4-322">1</span><span class="sxs-lookup"><span data-stu-id="800a4-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="800a4-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="800a4-324">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="800a4-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="800a4-325">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="800a4-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="800a4-326">11</span><span class="sxs-lookup"><span data-stu-id="800a4-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="800a4-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="800a4-328">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="800a4-328">Units included as part of the offer.</span></span> <span data-ttu-id="800a4-329">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="800a4-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="800a4-330">0</span><span class="sxs-lookup"><span data-stu-id="800a4-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="800a4-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="800a4-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="800a4-332">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="800a4-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="800a4-333">Равняется разнице значений полей ConsumedQuantityи IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="800a4-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="800a4-334">11</span><span class="sxs-lookup"><span data-stu-id="800a4-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="800a4-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="800a4-336">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="800a4-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="800a4-337">0,0808долл.США</span><span class="sxs-lookup"><span data-stu-id="800a4-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="800a4-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="800a4-339">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="800a4-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="800a4-340">0,085долл.США</span><span class="sxs-lookup"><span data-stu-id="800a4-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="800a4-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="800a4-342">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="800a4-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="800a4-343">0,08долл.США</span><span class="sxs-lookup"><span data-stu-id="800a4-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="800a4-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="800a4-345">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="800a4-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="800a4-346">0,93долл.США</span><span class="sxs-lookup"><span data-stu-id="800a4-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-347">Currency</span><span class="sxs-lookup"><span data-stu-id="800a4-347">Currency</span></span></td>
<td><p><span data-ttu-id="800a4-348">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="800a4-348">Currency type.</span></span> <span data-ttu-id="800a4-349">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="800a4-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="800a4-350">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="800a4-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="800a4-351">EUR</span><span class="sxs-lookup"><span data-stu-id="800a4-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="800a4-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="800a4-353">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="800a4-353">Pretax price per unit.</span></span> <span data-ttu-id="800a4-354">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="800a4-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="800a4-355">0,08долл.США</span><span class="sxs-lookup"><span data-stu-id="800a4-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="800a4-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="800a4-357">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="800a4-357">Post tax price per unit.</span></span> <span data-ttu-id="800a4-358">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="800a4-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="800a4-359">0,08долл.США</span><span class="sxs-lookup"><span data-stu-id="800a4-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="800a4-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="800a4-361">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="800a4-361">The type of charge or adjustment.</span></span> <span data-ttu-id="800a4-362">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="800a4-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="800a4-363">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="800a4-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="800a4-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="800a4-365">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="800a4-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="800a4-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="800a4-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="800a4-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="800a4-368">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="800a4-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="800a4-369">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="800a4-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="800a4-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="800a4-371">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="800a4-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="800a4-372">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="800a4-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-373">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="800a4-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="800a4-374">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="800a4-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="800a4-375">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="800a4-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="800a4-376">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="800a4-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="800a4-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="800a4-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="800a4-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="800a4-379">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="800a4-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="800a4-380">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="800a4-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-381">Проект</span><span class="sxs-lookup"><span data-stu-id="800a4-381">Project</span></span></td>
<td><p><span data-ttu-id="800a4-382">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="800a4-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="800a4-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="800a4-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="800a4-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="800a4-385">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="800a4-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="800a4-386">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="800a4-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="800a4-387">Если у вас был пакет на 25 подготовленных подключений "Шина_обслуживания", и вы использовали 1 подключение в течение этого дня, отчет о дневном использовании для этого подключения будет указывать "25 подключений/30 дней — использовано: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="800a4-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="800a4-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="800a4-389">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="800a4-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="800a4-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="800a4-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="800a4-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="800a4-391">DomainName</span></span></td>
<td><p><span data-ttu-id="800a4-392">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="800a4-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="800a4-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="800a4-393">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="800a4-394">Unit</span><span class="sxs-lookup"><span data-stu-id="800a4-394">Unit</span></span></td>
<td><p><span data-ttu-id="800a4-395">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="800a4-395">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="800a4-396">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="800a4-396">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="800a4-397">Сопоставление расходов в счете-фактуре и файле выверки</span><span class="sxs-lookup"><span data-stu-id="800a4-397">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="800a4-398">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="800a4-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="800a4-399">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="800a4-400">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="800a4-400">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="800a4-401">Одноразовые кредиты, скидки и возвраты денежных средств, которые отображаются в счете-фактуре как «Уточнения», не отображаются в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-401">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="800a4-402">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="800a4-402">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="800a4-403">Описание расходов по накладной</span><span class="sxs-lookup"><span data-stu-id="800a4-403">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="800a4-404">Описание расходов по файлу выверки (столбец ChargeType)</span><span class="sxs-lookup"><span data-stu-id="800a4-404">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="800a4-405">Что представляют собой данные расходы?</span><span class="sxs-lookup"><span data-stu-id="800a4-405">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="800a4-406">Как сопоставить эти типы расходов (ChargeTypes) со счетом-фактурой?</span><span class="sxs-lookup"><span data-stu-id="800a4-406">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="800a4-407">Повторяющиеся платежи</span><span class="sxs-lookup"><span data-stu-id="800a4-407">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="800a4-408">Отмена пропорционального распределения экземпляра</span><span class="sxs-lookup"><span data-stu-id="800a4-408">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-409">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="800a4-409">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="800a4-410">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="800a4-410">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-411">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="800a4-411">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-412">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="800a4-412">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-413">Пропорциональное распределение экземпляра цикла</span><span class="sxs-lookup"><span data-stu-id="800a4-413">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-414">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="800a4-414">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-415">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="800a4-415">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-416">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="800a4-416">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-417">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="800a4-417">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-418">Пропорциональные сборы после покупки</span><span class="sxs-lookup"><span data-stu-id="800a4-418">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-419">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="800a4-419">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-420">Первоначальный взнос за подписку</span><span class="sxs-lookup"><span data-stu-id="800a4-420">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-421">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="800a4-421">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-422">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="800a4-422">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-423">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="800a4-423">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-424">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="800a4-424">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="800a4-425">Прочие продукты и службы</span><span class="sxs-lookup"><span data-stu-id="800a4-425">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="800a4-426">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="800a4-426">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-427">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="800a4-427">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-428">Получите сумму значений столбца <strong>Сумма</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="800a4-428">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="800a4-429">Плата за использование</span><span class="sxs-lookup"><span data-stu-id="800a4-429">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="800a4-430">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="800a4-430">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-431">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="800a4-431">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="800a4-432">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="800a4-432">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-433">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="800a4-433">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-434">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="800a4-434">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="800a4-435">Кредиты и корректировки</span><span class="sxs-lookup"><span data-stu-id="800a4-435">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="800a4-436">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="800a4-436">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-437">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="800a4-437">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-438">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="800a4-438">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="800a4-439">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="800a4-439">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="800a4-440">Другие скидки</span><span class="sxs-lookup"><span data-stu-id="800a4-440">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="800a4-441">(по объему использования)</span><span class="sxs-lookup"><span data-stu-id="800a4-441">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="800a4-442">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="800a4-442">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-443">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="800a4-443">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="800a4-444">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="800a4-444">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-445">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="800a4-445">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-446">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="800a4-446">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="800a4-447">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="800a4-447">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-448">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="800a4-448">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="800a4-449">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="800a4-449">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-450">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="800a4-450">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="800a4-451">Другие скидки</span><span class="sxs-lookup"><span data-stu-id="800a4-451">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="800a4-452">(на основе лицензии)</span><span class="sxs-lookup"><span data-stu-id="800a4-452">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="800a4-453">Может применяться к различным типам платежей</span><span class="sxs-lookup"><span data-stu-id="800a4-453">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="800a4-454">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="800a4-454">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="800a4-455"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="800a4-455"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="800a4-456">Может применяться к различным типам платежей</span><span class="sxs-lookup"><span data-stu-id="800a4-456">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="800a4-457">Исключение: «Смещение позиции строки» уже включает налоги.</span><span class="sxs-lookup"><span data-stu-id="800a4-457">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="800a4-458">См. пункт «Кредиты и корректировки» выше.</span><span class="sxs-lookup"><span data-stu-id="800a4-458">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="800a4-459">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="800a4-459">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="800a4-460">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="800a4-460">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="800a4-461">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="800a4-461">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
