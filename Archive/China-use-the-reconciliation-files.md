---
title: Использовать сверочные файлы (под управлением 21vianet центра партнеров)
ms.topic: article
ms.date: 10/29/2018
description: Для просмотра подробных сведений строковых элементов каждой оплаты в расчетном цикле, загрузите файлы выверки с информационной панели в Центре партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584987"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="9a9c6-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="9a9c6-103">Use the reconciliation files</span></span>

<span data-ttu-id="9a9c6-104">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="9a9c6-104">**Applies to**</span></span>

-   <span data-ttu-id="9a9c6-105">Центр партнеров, предоставляемый 21Vianet</span><span class="sxs-lookup"><span data-stu-id="9a9c6-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="9a9c6-106">Для просмотра подробных сведений строковых элементов каждой оплаты в расчетном цикле, загрузите файлы выверки с информационной панели в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="9a9c6-107">Эти сведения включают оплаты за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="9a9c6-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="9a9c6-108">Детализировать партнером</span><span class="sxs-lookup"><span data-stu-id="9a9c6-108">Itemize by partner</span></span>


<span data-ttu-id="9a9c6-109">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="9a9c6-110">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="9a9c6-110">MPN ID</span></span></th>
<th><span data-ttu-id="9a9c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9a9c6-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="9a9c6-112">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="9a9c6-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="9a9c6-113">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="9a9c6-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-114">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="9a9c6-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="9a9c6-115">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="9a9c6-116">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="9a9c6-117">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="9a9c6-118">Чтобы просмотреть или обновить сведения о торговом посреднике, выберите раздел <strong>Клиенты</strong> в меню Центра партнеров, после чего выберите нужного клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="9a9c6-119">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="9a9c6-120">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="9a9c6-121">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="9a9c6-122">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="9a9c6-123">Если партнер CSP удаляет идентификатор торгового посредника, это значение будет равно -1.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="9a9c6-124">Поля файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="9a9c6-124">License-based file fields</span></span>


<span data-ttu-id="9a9c6-125">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="9a9c6-126"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="9a9c6-127"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="9a9c6-128"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-129">PartnerId</span><span class="sxs-lookup"><span data-stu-id="9a9c6-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="9a9c6-130">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="9a9c6-131">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="9a9c6-132">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="9a9c6-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="9a9c6-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="9a9c6-135">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="9a9c6-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="9a9c6-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-137">OrderID</span></span></td>
<td><p><span data-ttu-id="9a9c6-138">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="9a9c6-139">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="9a9c6-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="9a9c6-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="9a9c6-142">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="9a9c6-143">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="9a9c6-144">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="9a9c6-145">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="9a9c6-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="9a9c6-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-147">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="9a9c6-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="9a9c6-148">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="9a9c6-149">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="9a9c6-150">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="9a9c6-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="9a9c6-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-152">OfferID</span></span></td>
<td><p><span data-ttu-id="9a9c6-153">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-153">Unique offer ID.</span></span> <span data-ttu-id="9a9c6-154">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="9a9c6-155"><b>Примечание</b>. Это значение не соответствует Идентификатору предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="9a9c6-156">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="9a9c6-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="9a9c6-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="9a9c6-159">Уникальный идентификатор длительного предложения как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="9a9c6-160"><b>Примечание</b>. Это значение совпадает с Идентификатором предложения из прайс-лист.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="9a9c6-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="9a9c6-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-162">OfferName</span></span></td>
<td><p><span data-ttu-id="9a9c6-163">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="9a9c6-164">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="9a9c6-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="9a9c6-166">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="9a9c6-167">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="9a9c6-168">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="9a9c6-169">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="9a9c6-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="9a9c6-171">Дата окончания подписки: 12 месяцев + x дней после даты начала (чтобы соответствовать выставления счетов даты партнера) или 12 месяцев с даты продления.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="9a9c6-172">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="9a9c6-173">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="9a9c6-174">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="9a9c6-175">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="9a9c6-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="9a9c6-177">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="9a9c6-178">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="9a9c6-179">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="9a9c6-180">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="9a9c6-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="9a9c6-182">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="9a9c6-183">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="9a9c6-184">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="9a9c6-185">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="9a9c6-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="9a9c6-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="9a9c6-187">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-187">The type of charge or adjustment.</span></span> <span data-ttu-id="9a9c6-188">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="9a9c6-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="9a9c6-189">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="9a9c6-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="9a9c6-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="9a9c6-191">Цена за место.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-191">Price per seat.</span></span> <span data-ttu-id="9a9c6-192">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="9a9c6-193">6,82</span><span class="sxs-lookup"><span data-stu-id="9a9c6-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-194">Количество</span><span class="sxs-lookup"><span data-stu-id="9a9c6-194">Quantity</span></span></td>
<td><p><span data-ttu-id="9a9c6-195">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-195">Number of seats.</span></span> <span data-ttu-id="9a9c6-196">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="9a9c6-197">2</span><span class="sxs-lookup"><span data-stu-id="9a9c6-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-198">Сумма</span><span class="sxs-lookup"><span data-stu-id="9a9c6-198">Amount</span></span></td>
<td><p><span data-ttu-id="9a9c6-199">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-199">Total of price for quantity.</span></span> <span data-ttu-id="9a9c6-200">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="9a9c6-201">13,32</span><span class="sxs-lookup"><span data-stu-id="9a9c6-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="9a9c6-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="9a9c6-203">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="9a9c6-204">IUR или новые подписки, на которые распространяются вознаграждения, будут также содержать сумму скидки в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="9a9c6-205">2,32</span><span class="sxs-lookup"><span data-stu-id="9a9c6-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-206">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="9a9c6-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="9a9c6-207">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-207">Total before tax.</span></span> <span data-ttu-id="9a9c6-208">Указывает, что ваш промежуточный итог соответствует ожидаемой вами сумме в случае скидки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="9a9c6-209">11</span><span class="sxs-lookup"><span data-stu-id="9a9c6-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-210">Налог</span><span class="sxs-lookup"><span data-stu-id="9a9c6-210">Tax</span></span></td>
<td><p><span data-ttu-id="9a9c6-211">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="9a9c6-212">0</span><span class="sxs-lookup"><span data-stu-id="9a9c6-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="9a9c6-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="9a9c6-214">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-214">Total after tax.</span></span> <span data-ttu-id="9a9c6-215">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="9a9c6-216">11</span><span class="sxs-lookup"><span data-stu-id="9a9c6-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-217">Валюта</span><span class="sxs-lookup"><span data-stu-id="9a9c6-217">Currency</span></span></td>
<td><p><span data-ttu-id="9a9c6-218">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-218">Currency type.</span></span> <span data-ttu-id="9a9c6-219">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="9a9c6-220">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="9a9c6-221">CNY</span><span class="sxs-lookup"><span data-stu-id="9a9c6-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="9a9c6-223">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="9a9c6-224">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="9a9c6-225">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="9a9c6-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-226">MPNID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-226">MPNID</span></span></td>
<td><p><span data-ttu-id="9a9c6-227">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="9a9c6-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="9a9c6-228">4390934</span><span class="sxs-lookup"><span data-stu-id="9a9c6-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="9a9c6-230">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="9a9c6-231">См. раздел [Детализация по партнерам](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="9a9c6-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="9a9c6-232">4390934</span><span class="sxs-lookup"><span data-stu-id="9a9c6-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-233">DomainName</span></span></td>
<td><p><span data-ttu-id="9a9c6-234">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="9a9c6-235">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9a9c6-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="9a9c6-237">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-237">Subscription nickname.</span></span> <span data-ttu-id="9a9c6-238">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="9a9c6-239">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="9a9c6-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="9a9c6-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="9a9c6-241">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="9a9c6-242">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="9a9c6-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="9a9c6-243">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="9a9c6-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="9a9c6-244">Поля файла на основе использования</span><span class="sxs-lookup"><span data-stu-id="9a9c6-244">Usage-based file fields</span></span>


<span data-ttu-id="9a9c6-245">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="9a9c6-246">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="9a9c6-247"><strong>столбец</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="9a9c6-248"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="9a9c6-249"><strong>Образец значения</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="9a9c6-251">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="9a9c6-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="9a9c6-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="9a9c6-254">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="9a9c6-255">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="9a9c6-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="9a9c6-257">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="9a9c6-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="9a9c6-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="9a9c6-260">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="9a9c6-261">Это очень важно для выверки накладной с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="9a9c6-262">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="9a9c6-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-263">MPNID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-263">MPNID</span></span></td>
<td><p><span data-ttu-id="9a9c6-264">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="9a9c6-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="9a9c6-265">4390934</span><span class="sxs-lookup"><span data-stu-id="9a9c6-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="9a9c6-267">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="9a9c6-268">См. раздел [Детализация по партнерам](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="9a9c6-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="9a9c6-269">4390934</span><span class="sxs-lookup"><span data-stu-id="9a9c6-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="9a9c6-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="9a9c6-271">Номер накладной, содержащей указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="9a9c6-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="9a9c6-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="9a9c6-274">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="9a9c6-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="9a9c6-275">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="9a9c6-276">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="9a9c6-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="9a9c6-278">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="9a9c6-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="9a9c6-279">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="9a9c6-280">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="9a9c6-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="9a9c6-282">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="9a9c6-283">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="9a9c6-284">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="9a9c6-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="9a9c6-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="9a9c6-287">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="9a9c6-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="9a9c6-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="9a9c6-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="9a9c6-290">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="9a9c6-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="9a9c6-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="9a9c6-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-292">OrderID</span></span></td>
<td><p><span data-ttu-id="9a9c6-293">Уникальный идентификатор заказа в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="9a9c6-294">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="9a9c6-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="9a9c6-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="9a9c6-297">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="9a9c6-298">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="9a9c6-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="9a9c6-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="9a9c6-300">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="9a9c6-301">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="9a9c6-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="9a9c6-302">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="9a9c6-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="9a9c6-304">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="9a9c6-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="9a9c6-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-306">Resource Name</span><span class="sxs-lookup"><span data-stu-id="9a9c6-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="9a9c6-307">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="9a9c6-308">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="9a9c6-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="9a9c6-309">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="9a9c6-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-310">Region</span><span class="sxs-lookup"><span data-stu-id="9a9c6-310">Region</span></span></td>
<td><p><span data-ttu-id="9a9c6-311">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-311">The region the usage applies to.</span></span> <span data-ttu-id="9a9c6-312">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="9a9c6-313">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="9a9c6-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-314">SKU</span><span class="sxs-lookup"><span data-stu-id="9a9c6-314">SKU</span></span></td>
<td><p><span data-ttu-id="9a9c6-315">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="9a9c6-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="9a9c6-316">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="9a9c6-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="9a9c6-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="9a9c6-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="9a9c6-318">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="9a9c6-319">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним — другой.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="9a9c6-320">1</span><span class="sxs-lookup"><span data-stu-id="9a9c6-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="9a9c6-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="9a9c6-322">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="9a9c6-323">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="9a9c6-324">11</span><span class="sxs-lookup"><span data-stu-id="9a9c6-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="9a9c6-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="9a9c6-326">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-326">Units included as part of the offer.</span></span> <span data-ttu-id="9a9c6-327">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="9a9c6-328">0</span><span class="sxs-lookup"><span data-stu-id="9a9c6-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="9a9c6-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="9a9c6-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="9a9c6-330">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="9a9c6-331">Равняется разнице значений полей ConsumedQuantity и IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="9a9c6-332">11</span><span class="sxs-lookup"><span data-stu-id="9a9c6-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="9a9c6-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="9a9c6-334">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="9a9c6-335">0,0808 долл. США</span><span class="sxs-lookup"><span data-stu-id="9a9c6-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="9a9c6-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="9a9c6-337">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="9a9c6-338">0,085 долл. США</span><span class="sxs-lookup"><span data-stu-id="9a9c6-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="9a9c6-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="9a9c6-340">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="9a9c6-341">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="9a9c6-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="9a9c6-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="9a9c6-343">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="9a9c6-344">0,93 долл. США</span><span class="sxs-lookup"><span data-stu-id="9a9c6-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-345">Валюта</span><span class="sxs-lookup"><span data-stu-id="9a9c6-345">Currency</span></span></td>
<td><p><span data-ttu-id="9a9c6-346">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-346">Currency type.</span></span> <span data-ttu-id="9a9c6-347">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="9a9c6-348">Проверьте, соответствует ли тип валюты вашей первой накладной и каждой накладной после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="9a9c6-349">CNY</span><span class="sxs-lookup"><span data-stu-id="9a9c6-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="9a9c6-351">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-351">Pretax price per unit.</span></span> <span data-ttu-id="9a9c6-352">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="9a9c6-353">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="9a9c6-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="9a9c6-355">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-355">Post tax price per unit.</span></span> <span data-ttu-id="9a9c6-356">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="9a9c6-357">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="9a9c6-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="9a9c6-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="9a9c6-359">Тип взноса или корректировка.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-359">The type of charge or adjustment.</span></span> <span data-ttu-id="9a9c6-360">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="9a9c6-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="9a9c6-361">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="9a9c6-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="9a9c6-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="9a9c6-363">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="9a9c6-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="9a9c6-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="9a9c6-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="9a9c6-366">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="9a9c6-367">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="9a9c6-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="9a9c6-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="9a9c6-369">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="9a9c6-370">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="9a9c6-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-371">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="9a9c6-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="9a9c6-372">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="9a9c6-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="9a9c6-373">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="9a9c6-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="9a9c6-374">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="9a9c6-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="9a9c6-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="9a9c6-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="9a9c6-377">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="9a9c6-378">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="9a9c6-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-379">Проект</span><span class="sxs-lookup"><span data-stu-id="9a9c6-379">Project</span></span></td>
<td><p><span data-ttu-id="9a9c6-380">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="9a9c6-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="9a9c6-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="9a9c6-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="9a9c6-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="9a9c6-383">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="9a9c6-384">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="9a9c6-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="9a9c6-385">Если имеется 25 пакетов подключений служебной шины подготовлено, и вы использовалось 1 в течение этого дня, инструкцию ежедневное использование за этот день означает «25 подключений / 30 дней — использовано: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9a9c6-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="9a9c6-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="9a9c6-387">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="9a9c6-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="9a9c6-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9a9c6-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="9a9c6-389">DomainName</span></span></td>
<td><p><span data-ttu-id="9a9c6-390">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="9a9c6-391">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9a9c6-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="9a9c6-392">Сопоставление платежей в счете и сверочном файле</span><span class="sxs-lookup"><span data-stu-id="9a9c6-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="9a9c6-393">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="9a9c6-394">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="9a9c6-395">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="9a9c6-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="9a9c6-396"><strong>Описание платежа счета</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-397"><strong>Описание платежа сверочный файл (столбец ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-398"><strong>Что такое эта плата?</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-399"><strong>Как сопоставить эти счетом в счет?</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="9a9c6-400"><strong>Регулярные платежи</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-401">Отмена пропорционального распределения экземпляра</span><span class="sxs-lookup"><span data-stu-id="9a9c6-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-402">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="9a9c6-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="9a9c6-403">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="9a9c6-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-404">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="9a9c6-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-405">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="9a9c6-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-406">Пропорциональный перерасчет одного цикла</span><span class="sxs-lookup"><span data-stu-id="9a9c6-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-407">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="9a9c6-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-408">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="9a9c6-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-409">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="9a9c6-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-410">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="9a9c6-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-411">Пропорциональные сборы после покупки</span><span class="sxs-lookup"><span data-stu-id="9a9c6-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-412">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="9a9c6-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-413">Первоначальный взнос за подписку</span><span class="sxs-lookup"><span data-stu-id="9a9c6-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-414">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="9a9c6-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-415">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="9a9c6-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-416">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="9a9c6-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-417">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="9a9c6-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-418"><strong>Другие продукты и службы</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-419">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="9a9c6-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-420">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="9a9c6-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-421">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="9a9c6-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="9a9c6-422"><strong>Плата за использование</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-423">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="9a9c6-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-424">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="9a9c6-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="9a9c6-425">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="9a9c6-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-426">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="9a9c6-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-427">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="9a9c6-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-428"><strong>Деньги на счете &amp; корректировки</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-429">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="9a9c6-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-430">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="9a9c6-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-431">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="9a9c6-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="9a9c6-432">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="9a9c6-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="9a9c6-433"><strong>Другие скидки</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="9a9c6-434">
<em>(на основе использования)</em></span><span class="sxs-lookup"><span data-stu-id="9a9c6-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-435">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="9a9c6-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-436">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="9a9c6-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="9a9c6-437">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="9a9c6-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-438">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="9a9c6-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-439">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="9a9c6-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="9a9c6-440">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="9a9c6-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-441">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="9a9c6-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="9a9c6-442">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="9a9c6-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-443">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="9a9c6-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-444"><strong>Другие скидки</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="9a9c6-445">
<em>(на основе лицензий)</em></span><span class="sxs-lookup"><span data-stu-id="9a9c6-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-446"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="9a9c6-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="9a9c6-447">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="9a9c6-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="9a9c6-448"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="9a9c6-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-449"><em>Может применяться к нескольким типам платежей</em></span><span class="sxs-lookup"><span data-stu-id="9a9c6-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="9a9c6-450"><em>Исключение: «Позиции в строке» уже включает в себя налоги. См. в разделе кредиты &amp; корректировки выше.</em></span><span class="sxs-lookup"><span data-stu-id="9a9c6-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-451">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="9a9c6-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="9a9c6-452">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="9a9c6-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="9a9c6-453">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="9a9c6-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
