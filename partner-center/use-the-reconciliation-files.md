---
title: Использование файлов выверки | Центр партнеров
description: Для просмотра подробных сведений строковых элементов каждой оплаты в расчетном цикле, загрузите файлы выверки с информационной панели в Центре партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.localizationpriority: medium
ms.openlocfilehash: f4135bfeb4bf4245f7fc78a4d95946d094390a2a
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877554"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="143d6-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="143d6-103">Use the reconciliation files</span></span>

**<span data-ttu-id="143d6-104">Относится к:</span><span class="sxs-lookup"><span data-stu-id="143d6-104">Applies to</span></span>**

-  <span data-ttu-id="143d6-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="143d6-105">Partner Center</span></span>
-  <span data-ttu-id="143d6-106">Центр партнеров для Microsoft Cloud для правительства США</span><span class="sxs-lookup"><span data-stu-id="143d6-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="143d6-107">Центр партнеров Microsoft Cloud для Германии</span><span class="sxs-lookup"><span data-stu-id="143d6-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="143d6-108">Для просмотра подробных сведений строковых элементов каждой оплаты в расчетном цикле, загрузите файлы выверки с информационной панели в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="143d6-109">Эти сведения включают плату за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="143d6-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="143d6-110">Детализация по партнерам</span><span class="sxs-lookup"><span data-stu-id="143d6-110">Itemize by partner</span></span>


<span data-ttu-id="143d6-111">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="143d6-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="143d6-112">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="143d6-112">MPN ID</span></span></th>
<th><span data-ttu-id="143d6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="143d6-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="143d6-114">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="143d6-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="143d6-115">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="143d6-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-116">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="143d6-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="143d6-117">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="143d6-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="143d6-118">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="143d6-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="143d6-119">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="143d6-120">Чтобы просмотреть или обновить сведения о торговом посреднике, выберите раздел <strong>Клиенты</strong> в меню Центра партнеров, после чего выберите нужного клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="143d6-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="143d6-121">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="143d6-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="143d6-122">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="143d6-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="143d6-123">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="143d6-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="143d6-124">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="143d6-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="143d6-125">Если партнер CSP удаляет идентификатор торгового посредника, это значение будет равно -1.</span><span class="sxs-lookup"><span data-stu-id="143d6-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="143d6-126">Поля файла на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="143d6-126">License-based file fields</span></span>


<span data-ttu-id="143d6-127">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="143d6-128">Столбец</span><span class="sxs-lookup"><span data-stu-id="143d6-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="143d6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="143d6-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="143d6-130">Пример значения</span><span class="sxs-lookup"><span data-stu-id="143d6-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="143d6-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="143d6-132">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="143d6-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="143d6-133">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="143d6-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="143d6-134">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="143d6-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="143d6-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="143d6-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="143d6-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="143d6-137">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="143d6-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="143d6-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="143d6-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="143d6-139">OrderID</span></span></td>
<td><p><span data-ttu-id="143d6-140">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="143d6-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="143d6-141">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="143d6-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="143d6-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="143d6-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="143d6-144">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="143d6-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="143d6-145">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="143d6-146">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="143d6-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="143d6-147">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="143d6-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="143d6-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="143d6-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="143d6-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="143d6-150">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="143d6-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="143d6-151">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="143d6-152">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="143d6-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="143d6-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="143d6-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="143d6-154">OfferID</span></span></td>
<td><p><span data-ttu-id="143d6-155">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="143d6-155">Unique offer ID.</span></span> <span data-ttu-id="143d6-156">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="143d6-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="143d6-157"><b>Примечание</b>: это значение не соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="143d6-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="143d6-158">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="143d6-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="143d6-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="143d6-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="143d6-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="143d6-161">Уникальный идентификатор длительного предложения, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="143d6-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="143d6-162"><b>Примечание</b>. Это значение соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="143d6-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="143d6-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="143d6-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="143d6-164">OfferName</span></span></td>
<td><p><span data-ttu-id="143d6-165">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="143d6-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="143d6-166">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="143d6-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="143d6-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="143d6-168">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="143d6-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="143d6-169">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="143d6-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="143d6-170">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="143d6-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="143d6-171">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="143d6-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="143d6-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="143d6-173">Дата завершения подписки — 12 месяцев + x дней после даты начала (чтобы совместить с датой выставления счетов партнера) или 12 месяцев от даты возобновления действия.</span><span class="sxs-lookup"><span data-stu-id="143d6-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="143d6-174">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="143d6-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="143d6-175">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="143d6-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="143d6-176">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="143d6-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="143d6-177">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="143d6-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="143d6-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="143d6-179">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="143d6-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="143d6-180">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="143d6-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="143d6-181">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="143d6-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="143d6-182">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="143d6-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="143d6-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="143d6-184">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="143d6-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="143d6-185">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="143d6-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="143d6-186">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="143d6-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="143d6-187">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="143d6-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="143d6-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="143d6-189">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="143d6-189">The type of charge or adjustment.</span></span> <span data-ttu-id="143d6-190">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="143d6-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="143d6-191">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="143d6-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="143d6-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="143d6-193">Цена за рабочее место, опубликованное в прайс-листе во время покупки.</span><span class="sxs-lookup"><span data-stu-id="143d6-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="143d6-194">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="143d6-195">6,82</span><span class="sxs-lookup"><span data-stu-id="143d6-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="143d6-196">Quantity</span></span></td>
<td><p><span data-ttu-id="143d6-197">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="143d6-197">Number of seats.</span></span> <span data-ttu-id="143d6-198">Убедитесь, что оно соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="143d6-199">2</span><span class="sxs-lookup"><span data-stu-id="143d6-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-200">Amount</span><span class="sxs-lookup"><span data-stu-id="143d6-200">Amount</span></span></td>
<td><p><span data-ttu-id="143d6-201">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="143d6-201">Total of price for quantity.</span></span> <span data-ttu-id="143d6-202">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="143d6-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="143d6-203">13,32</span><span class="sxs-lookup"><span data-stu-id="143d6-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="143d6-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="143d6-205">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="143d6-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="143d6-206">IUR или новые подписки, на которые распространяются вознаграждения, будут также содержать сумму скидки в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="143d6-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="143d6-207">2,32</span><span class="sxs-lookup"><span data-stu-id="143d6-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="143d6-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="143d6-209">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="143d6-209">Total before tax.</span></span> <span data-ttu-id="143d6-210">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="143d6-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="143d6-211">11</span><span class="sxs-lookup"><span data-stu-id="143d6-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-212">Tax</span><span class="sxs-lookup"><span data-stu-id="143d6-212">Tax</span></span></td>
<td><p><span data-ttu-id="143d6-213">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="143d6-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="143d6-214">0</span><span class="sxs-lookup"><span data-stu-id="143d6-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="143d6-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="143d6-216">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="143d6-216">Total after tax.</span></span> <span data-ttu-id="143d6-217">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="143d6-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="143d6-218">11</span><span class="sxs-lookup"><span data-stu-id="143d6-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-219">Currency</span><span class="sxs-lookup"><span data-stu-id="143d6-219">Currency</span></span></td>
<td><p><span data-ttu-id="143d6-220">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="143d6-220">Currency type.</span></span> <span data-ttu-id="143d6-221">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="143d6-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="143d6-222">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="143d6-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="143d6-223">EUR</span><span class="sxs-lookup"><span data-stu-id="143d6-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="143d6-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="143d6-225">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="143d6-226">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="143d6-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="143d6-227">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="143d6-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="143d6-228">MPNID</span></span></td>
<td><p><span data-ttu-id="143d6-229">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="143d6-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="143d6-230">4390934</span><span class="sxs-lookup"><span data-stu-id="143d6-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="143d6-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="143d6-232">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="143d6-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="143d6-233">См. раздел [Детализация по партнерам](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="143d6-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="143d6-234">4390934</span><span class="sxs-lookup"><span data-stu-id="143d6-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="143d6-235">DomainName</span></span></td>
<td><p><span data-ttu-id="143d6-236">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="143d6-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="143d6-237">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="143d6-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="143d6-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="143d6-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="143d6-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="143d6-240">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="143d6-240">Subscription nickname.</span></span> <span data-ttu-id="143d6-241">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="143d6-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="143d6-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="143d6-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="143d6-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="143d6-244">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="143d6-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="143d6-245">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="143d6-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="143d6-246">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="143d6-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="143d6-247">Поля файла с учетом использования</span><span class="sxs-lookup"><span data-stu-id="143d6-247">Usage-based file fields</span></span>


<span data-ttu-id="143d6-248">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="143d6-249">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="143d6-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="143d6-250">Столбец</span><span class="sxs-lookup"><span data-stu-id="143d6-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="143d6-251">Описание</span><span class="sxs-lookup"><span data-stu-id="143d6-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="143d6-252">Пример значения</span><span class="sxs-lookup"><span data-stu-id="143d6-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="143d6-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="143d6-254">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="143d6-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="143d6-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="143d6-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="143d6-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="143d6-257">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="143d6-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="143d6-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="143d6-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="143d6-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="143d6-260">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="143d6-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="143d6-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="143d6-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="143d6-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="143d6-263">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="143d6-264">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="143d6-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="143d6-265">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="143d6-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="143d6-266">MPNID</span></span></td>
<td><p><span data-ttu-id="143d6-267">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="143d6-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="143d6-268">4390934</span><span class="sxs-lookup"><span data-stu-id="143d6-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="143d6-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="143d6-270">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="143d6-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="143d6-271">См. раздел [Детализация по партнерам](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="143d6-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="143d6-272">4390934</span><span class="sxs-lookup"><span data-stu-id="143d6-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="143d6-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="143d6-274">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="143d6-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="143d6-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="143d6-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="143d6-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="143d6-277">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="143d6-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="143d6-278">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="143d6-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="143d6-279">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="143d6-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="143d6-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="143d6-281">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="143d6-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="143d6-282">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="143d6-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="143d6-283">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="143d6-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="143d6-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="143d6-285">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="143d6-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="143d6-286">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="143d6-287">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="143d6-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="143d6-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="143d6-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="143d6-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="143d6-290">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="143d6-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="143d6-291">Платформа Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="143d6-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="143d6-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="143d6-293">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="143d6-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="143d6-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="143d6-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="143d6-295">OrderID</span></span></td>
<td><p><span data-ttu-id="143d6-296">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="143d6-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="143d6-297">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="143d6-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="143d6-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="143d6-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="143d6-300">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="143d6-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="143d6-301">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="143d6-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="143d6-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="143d6-303">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="143d6-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="143d6-304">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="143d6-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="143d6-305">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="143d6-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="143d6-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="143d6-307">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="143d6-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="143d6-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="143d6-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-309">Resource Name</span><span class="sxs-lookup"><span data-stu-id="143d6-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="143d6-310">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="143d6-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="143d6-311">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="143d6-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="143d6-312">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="143d6-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-313">Регион</span><span class="sxs-lookup"><span data-stu-id="143d6-313">Region</span></span></td>
<td><p><span data-ttu-id="143d6-314">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="143d6-314">The region the usage applies to.</span></span> <span data-ttu-id="143d6-315">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="143d6-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="143d6-316">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="143d6-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-317">SKU</span><span class="sxs-lookup"><span data-stu-id="143d6-317">SKU</span></span></td>
<td><p><span data-ttu-id="143d6-318">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="143d6-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="143d6-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="143d6-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="143d6-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="143d6-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="143d6-321">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="143d6-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="143d6-322">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним— другой.</span><span class="sxs-lookup"><span data-stu-id="143d6-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="143d6-323">1</span><span class="sxs-lookup"><span data-stu-id="143d6-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="143d6-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="143d6-325">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="143d6-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="143d6-326">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="143d6-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="143d6-327">11</span><span class="sxs-lookup"><span data-stu-id="143d6-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="143d6-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="143d6-329">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="143d6-329">Units included as part of the offer.</span></span> <span data-ttu-id="143d6-330">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="143d6-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="143d6-331">0</span><span class="sxs-lookup"><span data-stu-id="143d6-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="143d6-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="143d6-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="143d6-333">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="143d6-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="143d6-334">Равняется разнице значений полей ConsumedQuantityи IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="143d6-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="143d6-335">11</span><span class="sxs-lookup"><span data-stu-id="143d6-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="143d6-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="143d6-337">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="143d6-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="143d6-338">0,0808долл.США</span><span class="sxs-lookup"><span data-stu-id="143d6-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="143d6-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="143d6-340">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="143d6-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="143d6-341">0,085долл.США</span><span class="sxs-lookup"><span data-stu-id="143d6-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="143d6-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="143d6-343">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="143d6-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="143d6-344">0,08долл.США</span><span class="sxs-lookup"><span data-stu-id="143d6-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="143d6-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="143d6-346">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="143d6-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="143d6-347">0,93долл.США</span><span class="sxs-lookup"><span data-stu-id="143d6-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-348">Currency</span><span class="sxs-lookup"><span data-stu-id="143d6-348">Currency</span></span></td>
<td><p><span data-ttu-id="143d6-349">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="143d6-349">Currency type.</span></span> <span data-ttu-id="143d6-350">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="143d6-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="143d6-351">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="143d6-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="143d6-352">EUR</span><span class="sxs-lookup"><span data-stu-id="143d6-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="143d6-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="143d6-354">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="143d6-354">Pretax price per unit.</span></span> <span data-ttu-id="143d6-355">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="143d6-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="143d6-356">0,08долл.США</span><span class="sxs-lookup"><span data-stu-id="143d6-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="143d6-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="143d6-358">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="143d6-358">Post tax price per unit.</span></span> <span data-ttu-id="143d6-359">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="143d6-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="143d6-360">0,08долл.США</span><span class="sxs-lookup"><span data-stu-id="143d6-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="143d6-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="143d6-362">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="143d6-362">The type of charge or adjustment.</span></span> <span data-ttu-id="143d6-363">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="143d6-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="143d6-364">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="143d6-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="143d6-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="143d6-366">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="143d6-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="143d6-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="143d6-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="143d6-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="143d6-369">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="143d6-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="143d6-370">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="143d6-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="143d6-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="143d6-372">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="143d6-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="143d6-373">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="143d6-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-374">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="143d6-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="143d6-375">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="143d6-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="143d6-376">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="143d6-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="143d6-377">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="143d6-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="143d6-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="143d6-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="143d6-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="143d6-380">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="143d6-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="143d6-381">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="143d6-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-382">Проект</span><span class="sxs-lookup"><span data-stu-id="143d6-382">Project</span></span></td>
<td><p><span data-ttu-id="143d6-383">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="143d6-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="143d6-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="143d6-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="143d6-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="143d6-386">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="143d6-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="143d6-387">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="143d6-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="143d6-388">Если у вас был пакет на 25 подготовленных подключений "Шина_обслуживания", и вы использовали 1 подключение в течение этого дня, отчет о дневном использовании для этого подключения будет указывать "25 подключений/30 дней — использовано: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="143d6-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="143d6-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="143d6-390">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="143d6-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="143d6-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="143d6-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="143d6-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="143d6-392">DomainName</span></span></td>
<td><p><span data-ttu-id="143d6-393">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="143d6-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="143d6-394">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="143d6-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="143d6-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="143d6-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="143d6-396">Unit</span><span class="sxs-lookup"><span data-stu-id="143d6-396">Unit</span></span></td>
<td><p><span data-ttu-id="143d6-397">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="143d6-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="143d6-398">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="143d6-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="143d6-399">Поля файла единовременной покупки</span><span class="sxs-lookup"><span data-stu-id="143d6-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="143d6-400">Поле</span><span class="sxs-lookup"><span data-stu-id="143d6-400">Field</span></span>** |**<span data-ttu-id="143d6-401">Определение</span><span class="sxs-lookup"><span data-stu-id="143d6-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="143d6-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="143d6-402">PartnerId</span></span> |<span data-ttu-id="143d6-403">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="143d6-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="143d6-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="143d6-404">CustomerId</span></span> |<span data-ttu-id="143d6-405">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="143d6-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="143d6-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="143d6-406">CustomerName</span></span> |<span data-ttu-id="143d6-407">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="143d6-408">Очень важный элемент для сверки счета-фактуры с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="143d6-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="143d6-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="143d6-409">CustomerDomainName</span></span> |<span data-ttu-id="143d6-410">Имя домена клиента.</span><span class="sxs-lookup"><span data-stu-id="143d6-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="143d6-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="143d6-411">CustomerCountry</span></span> |<span data-ttu-id="143d6-412">Страна, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="143d6-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="143d6-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="143d6-413">InvoiceNumber</span></span> |<span data-ttu-id="143d6-414">Номер счета-фактуры, содержащего указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="143d6-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="143d6-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="143d6-415">MpnId</span></span> |<span data-ttu-id="143d6-416">Идентификатор MPN партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="143d6-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="143d6-417">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="143d6-417">Reseller MPN ID</span></span> |<span data-ttu-id="143d6-418">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="143d6-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="143d6-419">Идентификатор MPN зарегистрированного торгового посредника для резервирования.</span><span class="sxs-lookup"><span data-stu-id="143d6-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="143d6-420">Соответствует идентификатору торгового посредника, указанному для определенного резервирования в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="143d6-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="143d6-421">Если партнер CSP продал резервирование непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="143d6-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="143d6-422">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="143d6-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="143d6-423">Если партнер CSP удалил идентификатор торгового посредника, значение в этом поле равно -1.</span><span class="sxs-lookup"><span data-stu-id="143d6-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="143d6-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="143d6-424">OrderId</span></span> |<span data-ttu-id="143d6-425">Уникальный идентификатор заказа на платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="143d6-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="143d6-426">Может использоваться для идентификации резервирования Azure при обращении в службу технической поддержки, но не предназначен для выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="143d6-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="143d6-427">OrderDate</span></span> |<span data-ttu-id="143d6-428">Дата размещения заказа.</span><span class="sxs-lookup"><span data-stu-id="143d6-428">The date the order was placed.</span></span> |
|<span data-ttu-id="143d6-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="143d6-429">ProductId</span></span> |<span data-ttu-id="143d6-430">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="143d6-430">The ID for the product.</span></span> |
|<span data-ttu-id="143d6-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="143d6-431">SkuId</span></span>  |<span data-ttu-id="143d6-432">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="143d6-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="143d6-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="143d6-433">AvailabilityId</span></span> |<span data-ttu-id="143d6-434">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="143d6-434">The ID for a particular Availability.</span></span> <span data-ttu-id="143d6-435">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="143d6-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="143d6-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="143d6-436">SkuName</span></span>  |<span data-ttu-id="143d6-437">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="143d6-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="143d6-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="143d6-438">ProductName</span></span> |<span data-ttu-id="143d6-439">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="143d6-439">The name of the product.</span></span> |
|<span data-ttu-id="143d6-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="143d6-440">ChargeType</span></span> |<span data-ttu-id="143d6-441">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="143d6-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="143d6-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="143d6-442">UnitPrice</span></span> |<span data-ttu-id="143d6-443">Цена каждого заказанного продукта.</span><span class="sxs-lookup"><span data-stu-id="143d6-443">Price per product ordered.</span></span> |
|<span data-ttu-id="143d6-444">Количество</span><span class="sxs-lookup"><span data-stu-id="143d6-444">Quantity</span></span> |<span data-ttu-id="143d6-445">Количество заказанных продуктов.</span><span class="sxs-lookup"><span data-stu-id="143d6-445">Number of products ordered.</span></span> |
|<span data-ttu-id="143d6-446">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="143d6-446">Subtotal</span></span> |<span data-ttu-id="143d6-447">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="143d6-447">Total before tax.</span></span> <span data-ttu-id="143d6-448">В случае применения скидки промежуточный итог должен соответствовать ожидаемой итоговой сумме.</span><span class="sxs-lookup"><span data-stu-id="143d6-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="143d6-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="143d6-449">TaxTotal</span></span> |<span data-ttu-id="143d6-450">Общая сумма всех применимых налогов.</span><span class="sxs-lookup"><span data-stu-id="143d6-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="143d6-451">Итог</span><span class="sxs-lookup"><span data-stu-id="143d6-451">Total</span></span> |<span data-ttu-id="143d6-452">Общая сумма данной покупки.</span><span class="sxs-lookup"><span data-stu-id="143d6-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="143d6-453">Валюта</span><span class="sxs-lookup"><span data-stu-id="143d6-453">Currency</span></span> |<span data-ttu-id="143d6-454">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="143d6-454">Currency type.</span></span> <span data-ttu-id="143d6-455">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="143d6-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="143d6-456">Проверьте, соответствует ли тип валюты вашему первому счету-фактуре. Повторяйте эту проверку после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="143d6-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="143d6-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="143d6-457">DiscountDetails</span></span> |<span data-ttu-id="143d6-458">Подробный список всех соответствующих скидок.</span><span class="sxs-lookup"><span data-stu-id="143d6-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="143d6-459">Сопоставление расходов в счете-фактуре и файле выверки</span><span class="sxs-lookup"><span data-stu-id="143d6-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="143d6-460">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="143d6-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="143d6-461">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="143d6-462">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="143d6-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="143d6-463">Одноразовые кредиты, скидки и возвраты денежных средств, которые отображаются в счете-фактуре как «Уточнения», не отображаются в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="143d6-464">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="143d6-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="143d6-465">Описание расходов по накладной</span><span class="sxs-lookup"><span data-stu-id="143d6-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="143d6-466">Описание расходов по файлу выверки (столбец ChargeType)</span><span class="sxs-lookup"><span data-stu-id="143d6-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="143d6-467">Что представляют собой данные расходы?</span><span class="sxs-lookup"><span data-stu-id="143d6-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="143d6-468">Как сопоставить эти типы расходов (ChargeTypes) со счетом-фактурой?</span><span class="sxs-lookup"><span data-stu-id="143d6-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="143d6-469">Расходы на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="143d6-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="143d6-470">Стоимость активации</span><span class="sxs-lookup"><span data-stu-id="143d6-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-471">Сумма, взимаемая с клиента при использовании подписки после ее приобретения</span><span class="sxs-lookup"><span data-stu-id="143d6-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="143d6-472">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="143d6-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-473">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="143d6-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-474">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="143d6-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-475">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="143d6-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-476">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="143d6-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-477">Пропорциональное распределение экземпляра цикла</span><span class="sxs-lookup"><span data-stu-id="143d6-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-478">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="143d6-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-479">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="143d6-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-480">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="143d6-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-481">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="143d6-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-482">Пропорциональные сборы после покупки</span><span class="sxs-lookup"><span data-stu-id="143d6-482">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-483">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="143d6-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-484">Первоначальный взнос за подписку</span><span class="sxs-lookup"><span data-stu-id="143d6-484">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-485">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="143d6-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-486">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="143d6-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="143d6-487">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="143d6-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-488">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="143d6-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-489">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="143d6-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-490">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="143d6-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="143d6-491">Плата за использование</span><span class="sxs-lookup"><span data-stu-id="143d6-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="143d6-492">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="143d6-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-493">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="143d6-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="143d6-494">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="143d6-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-495">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="143d6-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-496">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="143d6-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="143d6-497">Кредиты</span><span class="sxs-lookup"><span data-stu-id="143d6-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="143d6-498">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="143d6-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-499">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="143d6-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-500">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="143d6-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="143d6-501">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="143d6-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="143d6-502">Скидки на основе использования</span><span class="sxs-lookup"><span data-stu-id="143d6-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="143d6-503">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="143d6-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-504">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="143d6-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="143d6-505">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="143d6-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-506">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="143d6-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-507">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="143d6-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-508">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="143d6-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-509">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="143d6-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-510">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="143d6-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-511">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="143d6-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="143d6-512">Скидки на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="143d6-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="143d6-513">Может применяться к различным типам платежей</span><span class="sxs-lookup"><span data-stu-id="143d6-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="143d6-514">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="143d6-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="143d6-515"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="143d6-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="143d6-516">Может применяться к различным типам платежей</span><span class="sxs-lookup"><span data-stu-id="143d6-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="143d6-517">Исключение: «Смещение позиции строки» уже включает налоги.</span><span class="sxs-lookup"><span data-stu-id="143d6-517">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="143d6-518">Кредиты, см. выше.</span><span class="sxs-lookup"><span data-stu-id="143d6-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="143d6-519">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="143d6-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="143d6-520">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="143d6-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="143d6-521">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="143d6-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
