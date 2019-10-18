---
title: Использование файлов выверки | Центр партнеров
ms.topic: article
ms.date: 07/08/2019
description: Для получения подробного представления по каждому элементу в цикле выставления счетов Скачайте файлы сверки из центра партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: cbc982fa5bf6848cb77a2de2dcdaa7660c422888
ms.sourcegitcommit: 30f946b3c5c2c30a5ee3276037385ea97e644781
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/03/2019
ms.locfileid: "71931577"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="23b62-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="23b62-103">Use the reconciliation files</span></span>

<span data-ttu-id="23b62-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="23b62-104">**Applies to**</span></span>

-  <span data-ttu-id="23b62-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="23b62-105">Partner Center</span></span>
-  <span data-ttu-id="23b62-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="23b62-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="23b62-107">Для получения подробного представления по каждому элементу в цикле выставления счетов Скачайте файлы сверки из центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="23b62-108">Эти сведения включают плату за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="23b62-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="23b62-109">Проблемы форматирования</span><span class="sxs-lookup"><span data-stu-id="23b62-109">Formatting issues</span></span>

<span data-ttu-id="23b62-110">Иногда файл разведывательную может иметь проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="23b62-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="23b62-111">(Это может произойти, например, если языковой стандарт EN-US не используется.) Чтобы устранить эти проблемы, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="23b62-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="23b62-112">Откройте CSV-файл в Excel и выберите первый столбец.</span><span class="sxs-lookup"><span data-stu-id="23b62-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="23b62-113">На ленте выберите <strong>данные</strong>, а затем выберите <strong>текст в столбцах</strong>.</span><span class="sxs-lookup"><span data-stu-id="23b62-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="23b62-114">В мастере преобразования текста в столбцы выберите <strong>Тип файла с разделителями</strong>, а затем нажмите кнопку <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="23b62-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="23b62-115">В поле разделителями Выберите <strong>запятая</strong>.</span><span class="sxs-lookup"><span data-stu-id="23b62-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="23b62-116">Если <strong>вкладка</strong> уже выбрана, можно оставить ее.</span><span class="sxs-lookup"><span data-stu-id="23b62-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="23b62-117">Выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="23b62-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="23b62-118">В поле Формат данных столбца выберите <strong>Date: mdy</strong>, а затем нажмите кнопку <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="23b62-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="23b62-119">В поле Формат данных столбца выберите <strong>текст</strong> для всех столбцов суммы, а затем нажмите кнопку <strong>Готово</strong>.</span><span class="sxs-lookup"><span data-stu-id="23b62-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="23b62-120">Скачивание большого файла разведывательную</span><span class="sxs-lookup"><span data-stu-id="23b62-120">Downloading a large recon file</span></span>

<span data-ttu-id="23b62-121">Файлы разведывательную могут увеличиваться очень большими и иногда трудно загружать.</span><span class="sxs-lookup"><span data-stu-id="23b62-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="23b62-122">Сведения о загрузке больших файлов разведывательную в скрипте PowerShell см. в разделе [Получение элементов строки счета](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="23b62-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="23b62-123">Детализировать по партнеру</span><span class="sxs-lookup"><span data-stu-id="23b62-123">Itemize by partner</span></span>


<span data-ttu-id="23b62-124">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="23b62-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="23b62-125">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="23b62-125">MPN ID</span></span></th>
<th><span data-ttu-id="23b62-126">Описание</span><span class="sxs-lookup"><span data-stu-id="23b62-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="23b62-127">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="23b62-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="23b62-128">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="23b62-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-129">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="23b62-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="23b62-130">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="23b62-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="23b62-131">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="23b62-132">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="23b62-133">Ето просмотреть или обновить торгового посредника, в меню центра партнеров выберите <strong>Клиенты</strong>, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="23b62-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="23b62-134">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="23b62-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="23b62-135">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="23b62-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="23b62-136">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="23b62-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="23b62-137">Если у партнера CSP есть торговый партнер без идентификатора MPN, то это значение устанавливается для идентификатора MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="23b62-138">Если партнер CSP удалил идентификатор торгового посредника, значение в этом поле равно -1.</span><span class="sxs-lookup"><span data-stu-id="23b62-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="23b62-139">Поля файла на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="23b62-139">License-based file fields</span></span>


<span data-ttu-id="23b62-140">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="23b62-141"><strong>Рубрик</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="23b62-142"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="23b62-143"><strong>Пример значения</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="23b62-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="23b62-145">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="23b62-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="23b62-146">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="23b62-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="23b62-147">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="23b62-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="23b62-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="23b62-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="23b62-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="23b62-150">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="23b62-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="23b62-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="23b62-152">OrderID</span></span></td>
<td><p><span data-ttu-id="23b62-153">Уникальный идентификатор заказа на платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="23b62-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="23b62-154">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="23b62-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="23b62-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="23b62-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="23b62-157">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="23b62-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="23b62-158">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="23b62-159">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="23b62-160">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="23b62-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="23b62-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="23b62-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="23b62-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="23b62-163">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="23b62-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="23b62-164">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="23b62-165">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="23b62-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="23b62-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="23b62-167">OfferID</span></span></td>
<td><p><span data-ttu-id="23b62-168">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="23b62-168">Unique offer ID.</span></span> <span data-ttu-id="23b62-169">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="23b62-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="23b62-170"><b>Примечание</b>: это значение не соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="23b62-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="23b62-171">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="23b62-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="23b62-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="23b62-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="23b62-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="23b62-174">Уникальный идентификатор длительного предложения, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="23b62-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="23b62-175"><b>Примечание</b>. Это значение соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="23b62-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="23b62-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="23b62-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="23b62-177">OfferName</span></span></td>
<td><p><span data-ttu-id="23b62-178">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="23b62-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="23b62-179">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="23b62-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="23b62-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="23b62-181">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="23b62-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="23b62-182">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="23b62-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="23b62-183">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="23b62-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="23b62-184">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="23b62-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="23b62-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="23b62-186">Дата завершения подписки — 12 месяцев + x дней после даты начала (чтобы совместить с датой выставления счетов партнера) или 12 месяцев от даты возобновления действия.</span><span class="sxs-lookup"><span data-stu-id="23b62-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="23b62-187">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="23b62-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="23b62-188">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="23b62-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="23b62-189">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="23b62-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="23b62-190">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="23b62-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="23b62-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="23b62-192">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="23b62-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="23b62-193">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="23b62-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="23b62-194">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="23b62-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="23b62-195">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="23b62-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="23b62-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="23b62-197">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="23b62-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="23b62-198">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="23b62-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="23b62-199">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="23b62-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="23b62-200">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="23b62-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="23b62-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="23b62-202">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="23b62-202">The type of charge or adjustment.</span></span> <span data-ttu-id="23b62-203">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="23b62-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="23b62-204">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="23b62-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="23b62-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="23b62-206">Цена за рабочее место, опубликованное в прайс-листе во время покупки.</span><span class="sxs-lookup"><span data-stu-id="23b62-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="23b62-207">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="23b62-208">6,82</span><span class="sxs-lookup"><span data-stu-id="23b62-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-209">Количество</span><span class="sxs-lookup"><span data-stu-id="23b62-209">Quantity</span></span></td>
<td><p><span data-ttu-id="23b62-210">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="23b62-210">Number of seats.</span></span> <span data-ttu-id="23b62-211">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="23b62-212">2</span><span class="sxs-lookup"><span data-stu-id="23b62-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-213">Сумма</span><span class="sxs-lookup"><span data-stu-id="23b62-213">Amount</span></span></td>
<td><p><span data-ttu-id="23b62-214">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="23b62-214">Total of price for quantity.</span></span> <span data-ttu-id="23b62-215">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="23b62-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="23b62-216">13,32</span><span class="sxs-lookup"><span data-stu-id="23b62-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="23b62-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="23b62-218">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="23b62-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="23b62-219">Лицензии на продукт, входящие в компетенцию или карты или новые подписки, подходящие для стимула, также будут содержать сумму скидки в этой статье.</span><span class="sxs-lookup"><span data-stu-id="23b62-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="23b62-220">2,32</span><span class="sxs-lookup"><span data-stu-id="23b62-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-221">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="23b62-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="23b62-222">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="23b62-222">Total before tax.</span></span> <span data-ttu-id="23b62-223">В случае применения скидки промежуточный итог должен соответствовать ожидаемой итоговой сумме.</span><span class="sxs-lookup"><span data-stu-id="23b62-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="23b62-224">11</span><span class="sxs-lookup"><span data-stu-id="23b62-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-225">Налог</span><span class="sxs-lookup"><span data-stu-id="23b62-225">Tax</span></span></td>
<td><p><span data-ttu-id="23b62-226">Сумма налога взимается на основе правил налогов на&#39;рынке и определенных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="23b62-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="23b62-227">0</span><span class="sxs-lookup"><span data-stu-id="23b62-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="23b62-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="23b62-229">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="23b62-229">Total after tax.</span></span> <span data-ttu-id="23b62-230">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="23b62-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="23b62-231">11</span><span class="sxs-lookup"><span data-stu-id="23b62-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-232">Валюта</span><span class="sxs-lookup"><span data-stu-id="23b62-232">Currency</span></span></td>
<td><p><span data-ttu-id="23b62-233">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="23b62-233">Currency type.</span></span> <span data-ttu-id="23b62-234">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="23b62-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="23b62-235">Проверьте, соответствует ли тип валюты вашему первому счету-фактуре. Повторяйте эту проверку после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="23b62-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="23b62-236">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="23b62-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="23b62-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="23b62-238">Имя&#39;организации клиента согласно сообщению в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="23b62-239">Очень важный элемент для сверки счета-фактуры с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="23b62-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="23b62-240">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="23b62-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="23b62-241">MPNID</span></span></td>
<td><p><span data-ttu-id="23b62-242">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="23b62-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="23b62-243">4390934</span><span class="sxs-lookup"><span data-stu-id="23b62-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="23b62-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="23b62-245">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="23b62-246">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="23b62-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="23b62-247">4390934</span><span class="sxs-lookup"><span data-stu-id="23b62-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="23b62-248">DomainName</span></span></td>
<td><p><span data-ttu-id="23b62-249">Имя&#39;домена клиента, используемое для поиска клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="23b62-250">Его не следует использовать для уникальной идентификации клиента, так как клиент или партнер может обновить домен именного/Default через портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="23b62-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="23b62-251">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="23b62-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="23b62-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="23b62-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="23b62-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="23b62-254">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-254">Subscription nickname.</span></span> <span data-ttu-id="23b62-255">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="23b62-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="23b62-256">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="23b62-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="23b62-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="23b62-258">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="23b62-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="23b62-259">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="23b62-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="23b62-260">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="23b62-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="23b62-261">Поля файла на основе использования</span><span class="sxs-lookup"><span data-stu-id="23b62-261">Usage-based file fields</span></span>


<span data-ttu-id="23b62-262">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="23b62-263">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="23b62-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="23b62-264"><strong>Рубрик</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="23b62-265"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="23b62-266"><strong>Пример значения</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="23b62-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="23b62-268">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="23b62-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="23b62-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="23b62-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="23b62-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="23b62-271">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="23b62-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="23b62-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="23b62-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="23b62-274">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="23b62-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="23b62-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="23b62-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="23b62-277">Имя&#39;организации клиента согласно сообщению в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="23b62-278">Очень важный элемент для сверки счета-фактуры с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="23b62-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="23b62-279">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="23b62-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="23b62-280">MPNID</span></span></td>
<td><p><span data-ttu-id="23b62-281">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="23b62-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="23b62-282">4390934</span><span class="sxs-lookup"><span data-stu-id="23b62-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="23b62-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="23b62-284">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="23b62-285">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="23b62-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="23b62-286">4390934</span><span class="sxs-lookup"><span data-stu-id="23b62-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="23b62-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="23b62-288">Номер счета-фактуры, содержащего указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="23b62-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="23b62-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="23b62-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="23b62-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="23b62-291">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="23b62-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="23b62-292">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="23b62-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="23b62-293">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="23b62-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="23b62-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="23b62-295">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="23b62-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="23b62-296">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="23b62-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="23b62-297">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="23b62-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="23b62-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="23b62-299">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="23b62-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="23b62-300">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="23b62-301">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="23b62-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="23b62-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="23b62-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="23b62-304">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="23b62-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="23b62-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="23b62-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="23b62-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="23b62-307">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="23b62-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="23b62-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="23b62-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="23b62-309">OrderID</span></span></td>
<td><p><span data-ttu-id="23b62-310">Уникальный идентификатор заказа на платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="23b62-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="23b62-311">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="23b62-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="23b62-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="23b62-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="23b62-314">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="23b62-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="23b62-315">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="23b62-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="23b62-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="23b62-317">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="23b62-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="23b62-318">Шина обслуживания — отдельная или пакет</span><span class="sxs-lookup"><span data-stu-id="23b62-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="23b62-319">База данных SQL Azure — для бизнеса или выпуск Web Edition</span><span class="sxs-lookup"><span data-stu-id="23b62-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="23b62-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="23b62-321">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="23b62-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="23b62-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="23b62-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-323">Resource Name</span><span class="sxs-lookup"><span data-stu-id="23b62-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="23b62-324">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="23b62-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="23b62-325">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="23b62-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="23b62-326">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="23b62-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-327">Region</span><span class="sxs-lookup"><span data-stu-id="23b62-327">Region</span></span></td>
<td><p><span data-ttu-id="23b62-328">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="23b62-328">The region the usage applies to.</span></span> <span data-ttu-id="23b62-329">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="23b62-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="23b62-330">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="23b62-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-331">SKU</span><span class="sxs-lookup"><span data-stu-id="23b62-331">SKU</span></span></td>
<td><p><span data-ttu-id="23b62-332">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="23b62-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="23b62-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="23b62-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="23b62-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="23b62-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="23b62-335">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="23b62-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="23b62-336">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним — другой.</span><span class="sxs-lookup"><span data-stu-id="23b62-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="23b62-337">1</span><span class="sxs-lookup"><span data-stu-id="23b62-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="23b62-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="23b62-339">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="23b62-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="23b62-340">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="23b62-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="23b62-341">11</span><span class="sxs-lookup"><span data-stu-id="23b62-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="23b62-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="23b62-343">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="23b62-343">Units included as part of the offer.</span></span> <span data-ttu-id="23b62-344">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="23b62-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="23b62-345">0</span><span class="sxs-lookup"><span data-stu-id="23b62-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="23b62-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="23b62-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="23b62-347">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="23b62-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="23b62-348">Равняется разнице значений полей ConsumedQuantity и IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="23b62-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="23b62-349">11</span><span class="sxs-lookup"><span data-stu-id="23b62-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="23b62-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="23b62-351">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="23b62-352">0,0808 долл. США</span><span class="sxs-lookup"><span data-stu-id="23b62-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="23b62-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="23b62-354">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="23b62-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="23b62-355">0,085 долл. США</span><span class="sxs-lookup"><span data-stu-id="23b62-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="23b62-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="23b62-357">Сумма налога взимается на основе правил налогов на&#39;рынке и определенных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="23b62-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="23b62-358">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="23b62-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="23b62-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="23b62-360">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="23b62-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="23b62-361">0,93 долл. США</span><span class="sxs-lookup"><span data-stu-id="23b62-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-362">Валюта</span><span class="sxs-lookup"><span data-stu-id="23b62-362">Currency</span></span></td>
<td><p><span data-ttu-id="23b62-363">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="23b62-363">Currency type.</span></span> <span data-ttu-id="23b62-364">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="23b62-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="23b62-365">Проверьте, соответствует ли тип валюты вашему первому счету-фактуре. Повторяйте эту проверку после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="23b62-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="23b62-366">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="23b62-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="23b62-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="23b62-368">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="23b62-368">Pretax price per unit.</span></span> <span data-ttu-id="23b62-369">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="23b62-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="23b62-370">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="23b62-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="23b62-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="23b62-372">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="23b62-372">Post tax price per unit.</span></span> <span data-ttu-id="23b62-373">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="23b62-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="23b62-374">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="23b62-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="23b62-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="23b62-376">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="23b62-376">The type of charge or adjustment.</span></span> <span data-ttu-id="23b62-377">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="23b62-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="23b62-378">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="23b62-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="23b62-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="23b62-380">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="23b62-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="23b62-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="23b62-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="23b62-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="23b62-383">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="23b62-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="23b62-384">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="23b62-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="23b62-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="23b62-386">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="23b62-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="23b62-387">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="23b62-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-388">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="23b62-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="23b62-389">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="23b62-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="23b62-390">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="23b62-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="23b62-391">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="23b62-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="23b62-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="23b62-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="23b62-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="23b62-394">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="23b62-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="23b62-395">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="23b62-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-396">Проект</span><span class="sxs-lookup"><span data-stu-id="23b62-396">Project</span></span></td>
<td><p><span data-ttu-id="23b62-397">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="23b62-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="23b62-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="23b62-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="23b62-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="23b62-400">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="23b62-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="23b62-401">Например: если у вас было отдельно подготовленное подключение в течение 30 дней, то параметр "Сведения_службы1" будет иметь следующий вид: "1,000000 подключений/30 дней".</span><span class="sxs-lookup"><span data-stu-id="23b62-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="23b62-402">Если у вас был пакет на 25 подготовленных подключений "Шина_обслуживания", и вы использовали 1 подключение в течение этого дня, отчет о дневном использовании для этого подключения будет указывать "25 подключений/30 дней — использовано: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="23b62-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="23b62-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="23b62-404">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="23b62-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="23b62-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="23b62-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="23b62-406">DomainName</span></span></td>
<td><p><span data-ttu-id="23b62-407">Имя&#39;домена клиента, используемое для поиска клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="23b62-408">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="23b62-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="23b62-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="23b62-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="23b62-410">Unit</span><span class="sxs-lookup"><span data-stu-id="23b62-410">Unit</span></span></td>
<td><p><span data-ttu-id="23b62-411">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="23b62-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="23b62-412">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="23b62-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="23b62-413">Поля однократного и повторяющегося файлов</span><span class="sxs-lookup"><span data-stu-id="23b62-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="23b62-414">Column</span><span class="sxs-lookup"><span data-stu-id="23b62-414">Column</span></span></th>
<th><span data-ttu-id="23b62-415">Описание</span><span class="sxs-lookup"><span data-stu-id="23b62-415">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="23b62-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="23b62-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="23b62-417">Уникальный идентификатор клиента Microsoft Azure Active Directory для определенной сущности выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="23b62-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="23b62-418">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="23b62-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="23b62-419">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="23b62-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-420">Идентификатор клиента</span><span class="sxs-lookup"><span data-stu-id="23b62-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="23b62-421">Уникальный идентификатор клиента Microsoft Azure Active Directory в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-422">Customer Name (Имя клиента)</span><span class="sxs-lookup"><span data-stu-id="23b62-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="23b62-423">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="23b62-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="23b62-425">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="23b62-426">Его не следует использовать для уникальной идентификации клиента, так как клиент или партнер может обновить домен именного/Default через портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="23b62-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="23b62-427">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="23b62-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-428">Страна клиента</span><span class="sxs-lookup"><span data-stu-id="23b62-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="23b62-429">Страна, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="23b62-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-430">Номер счета</span><span class="sxs-lookup"><span data-stu-id="23b62-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="23b62-431">Номер счета-фактуры, содержащего указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="23b62-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="23b62-432">MpnId</span></span></td>
<td><p><span data-ttu-id="23b62-433">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="23b62-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-434">MpnId торгового посредника</span><span class="sxs-lookup"><span data-stu-id="23b62-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="23b62-435">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-436">Идентификатор заказа</span><span class="sxs-lookup"><span data-stu-id="23b62-436">Order ID</span></span></td>
<td><p><span data-ttu-id="23b62-437">Уникальный идентификатор для заказа на платформе Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="23b62-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="23b62-438">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-439">Дата заказа</span><span class="sxs-lookup"><span data-stu-id="23b62-439">Order date</span></span></td>
<td><p><span data-ttu-id="23b62-440">Дата размещения заказа.</span><span class="sxs-lookup"><span data-stu-id="23b62-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-441">ProductID</span><span class="sxs-lookup"><span data-stu-id="23b62-441">ProductId</span></span></td>
<td><p><span data-ttu-id="23b62-442">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="23b62-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="23b62-443">SkuId</span></span></td>
<td><p><span data-ttu-id="23b62-444">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="23b62-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="23b62-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="23b62-446">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="23b62-446">The ID for a particular Availability.</span></span> <span data-ttu-id="23b62-447">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="23b62-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-448">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="23b62-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="23b62-449">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="23b62-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-450">название продукта;</span><span class="sxs-lookup"><span data-stu-id="23b62-450">Product name</span></span></td>
<td><p><span data-ttu-id="23b62-451">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="23b62-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="23b62-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="23b62-453">Имя издателя продукта.</span><span class="sxs-lookup"><span data-stu-id="23b62-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="23b62-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="23b62-455">Уникальный идентификатор для этого издателя.</span><span class="sxs-lookup"><span data-stu-id="23b62-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-456">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="23b62-457">Понятное имя подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-458">Код подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="23b62-459">Уникальный идентификатор подписки в платформе Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="23b62-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="23b62-460">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="23b62-461">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="23b62-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="23b62-463">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="23b62-463">Start day of the charges.</span></span> <span data-ttu-id="23b62-464">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="23b62-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="23b62-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="23b62-466">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="23b62-466">End day of the charges.</span></span> <span data-ttu-id="23b62-467">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="23b62-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-468">Term и Биллингцикле</span><span class="sxs-lookup"><span data-stu-id="23b62-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="23b62-469">Срок и цикл выставления счетов для покупки.</span><span class="sxs-lookup"><span data-stu-id="23b62-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="23b62-470">Например, "1 год, месяц".</span><span class="sxs-lookup"><span data-stu-id="23b62-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-471">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="23b62-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="23b62-472">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="23b62-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-473">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="23b62-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="23b62-474">Цена, опубликованная в PriceList во время покупки.</span><span class="sxs-lookup"><span data-stu-id="23b62-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="23b62-475">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-476">Эффективная цена за единицу</span><span class="sxs-lookup"><span data-stu-id="23b62-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="23b62-477">Цена за единицу после внесения корректировок.</span><span class="sxs-lookup"><span data-stu-id="23b62-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-478">Количество</span><span class="sxs-lookup"><span data-stu-id="23b62-478">Quantity</span></span></td>
<td><p><span data-ttu-id="23b62-479">Количество единиц.</span><span class="sxs-lookup"><span data-stu-id="23b62-479">Number of units.</span></span> <span data-ttu-id="23b62-480">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-481">Тип единицы</span><span class="sxs-lookup"><span data-stu-id="23b62-481">Unit type</span></span></td>
<td><p><span data-ttu-id="23b62-482">Тип приобретаемой единицы.</span><span class="sxs-lookup"><span data-stu-id="23b62-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="23b62-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="23b62-484">Описание применимой скидки.</span><span class="sxs-lookup"><span data-stu-id="23b62-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-485">Итого</span><span class="sxs-lookup"><span data-stu-id="23b62-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="23b62-486">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="23b62-486">Total before tax.</span></span> <span data-ttu-id="23b62-487">В случае применения скидки промежуточный итог должен соответствовать ожидаемой итоговой сумме.</span><span class="sxs-lookup"><span data-stu-id="23b62-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-488">Сумма налогов</span><span class="sxs-lookup"><span data-stu-id="23b62-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="23b62-489">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="23b62-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-490">Total (Всего)</span><span class="sxs-lookup"><span data-stu-id="23b62-490">Total</span></span></td>
<td><p><span data-ttu-id="23b62-491">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="23b62-491">Total after tax.</span></span> <span data-ttu-id="23b62-492">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="23b62-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-493">Валюта</span><span class="sxs-lookup"><span data-stu-id="23b62-493">Currency</span></span></td>
<td><p><span data-ttu-id="23b62-494">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="23b62-494">Currency type.</span></span> <span data-ttu-id="23b62-495">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="23b62-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="23b62-496">Проверьте, соответствует ли тип валюты вашему первому счету-фактуре. Повторяйте эту проверку после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="23b62-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-497">Альтернативного имени пользователя</span><span class="sxs-lookup"><span data-stu-id="23b62-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="23b62-498">Альтернативный идентификатор для идентификатора заказа.</span><span class="sxs-lookup"><span data-stu-id="23b62-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-499">биллингфрекуенци</span><span class="sxs-lookup"><span data-stu-id="23b62-499">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="23b62-500">Выводится ежемесячно, если включен ежемесячный счет.</span><span class="sxs-lookup"><span data-stu-id="23b62-500">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="23b62-501">В противном случае оставьте пустым.</span><span class="sxs-lookup"><span data-stu-id="23b62-501">Otherwise blank.</span></span> </p></td>
</tr>

</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="23b62-502">Поля файла с ежедневной оценкой использования</span><span class="sxs-lookup"><span data-stu-id="23b62-502">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="23b62-503">Column</span><span class="sxs-lookup"><span data-stu-id="23b62-503">Column</span></span></th>
<th><span data-ttu-id="23b62-504">Описание</span><span class="sxs-lookup"><span data-stu-id="23b62-504">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="23b62-505">PartnerId</span><span class="sxs-lookup"><span data-stu-id="23b62-505">PartnerId</span></span></td>
<td><p><span data-ttu-id="23b62-506">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="23b62-506">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-507">PartnerName</span><span class="sxs-lookup"><span data-stu-id="23b62-507">PartnerName</span></span></td>
<td><p><span data-ttu-id="23b62-508">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-508">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-509">CustomerId</span><span class="sxs-lookup"><span data-stu-id="23b62-509">CustomerId</span></span></td>
<td><p><span data-ttu-id="23b62-510">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-510">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-511">кустомеркомпанинаме</span><span class="sxs-lookup"><span data-stu-id="23b62-511">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="23b62-512">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="23b62-512">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="23b62-513">Очень важный элемент для сверки счета-фактуры с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="23b62-513">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-514">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="23b62-514">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="23b62-515">Имя домена клиента.</span><span class="sxs-lookup"><span data-stu-id="23b62-515">The customer’s domain name.</span></span> <span data-ttu-id="23b62-516">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="23b62-516">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-517">Страна клиента</span><span class="sxs-lookup"><span data-stu-id="23b62-517">Customer country</span></span></td>
<td><p><span data-ttu-id="23b62-518">Страна, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="23b62-518">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-519">MPNID</span><span class="sxs-lookup"><span data-stu-id="23b62-519">MPNID</span></span></td>
<td><p><span data-ttu-id="23b62-520">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="23b62-520">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-521">MPNID торгового посредника</span><span class="sxs-lookup"><span data-stu-id="23b62-521">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="23b62-522">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="23b62-522">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="23b62-523">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="23b62-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-524">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="23b62-524">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="23b62-525">Номер счета-фактуры, содержащего указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="23b62-525">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="23b62-526">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="23b62-526">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-527">ProductID</span><span class="sxs-lookup"><span data-stu-id="23b62-527">ProductId</span></span></td>
<td><p><span data-ttu-id="23b62-528">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="23b62-528">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-529">SkuId</span><span class="sxs-lookup"><span data-stu-id="23b62-529">SkuId</span></span></td>
<td><p><span data-ttu-id="23b62-530">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="23b62-530">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-531">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="23b62-531">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="23b62-532">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="23b62-532">The ID for a particular Availability.</span></span> <span data-ttu-id="23b62-533">Под доступностью подразумевается возможность приобрести продукт с определенным номером SKU в данной стране, валюте, сегменте отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="23b62-533">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-534">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="23b62-534">SKU Name</span></span></td>
<td><p><span data-ttu-id="23b62-535">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="23b62-535">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-536">PublisherName</span><span class="sxs-lookup"><span data-stu-id="23b62-536">PublisherName</span></span></td>
<td><p><span data-ttu-id="23b62-537">Имя издателя.</span><span class="sxs-lookup"><span data-stu-id="23b62-537">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-538">PublisherID</span><span class="sxs-lookup"><span data-stu-id="23b62-538">PublisherID</span></span></td>
<td><p><span data-ttu-id="23b62-539">Идентификатор издателя в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="23b62-539">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="23b62-540">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="23b62-540">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="23b62-541">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-541">Subscription Description</span></span></td>
<td><p><span data-ttu-id="23b62-542">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="23b62-542">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="23b62-543">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="23b62-543">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-544">Код подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-544">Subscription ID</span></span></td>
<td><p><span data-ttu-id="23b62-545">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="23b62-545">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="23b62-546">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-546">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="23b62-547">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="23b62-547">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-548">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="23b62-548">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="23b62-549">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="23b62-549">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="23b62-550">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="23b62-550">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-551">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="23b62-551">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="23b62-552">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="23b62-552">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="23b62-553">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="23b62-553">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-554">Дата использования</span><span class="sxs-lookup"><span data-stu-id="23b62-554">Usage Date</span></span></td>
<td><p><span data-ttu-id="23b62-555">Дата использования службы.</span><span class="sxs-lookup"><span data-stu-id="23b62-555">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-556">Тип счетчика</span><span class="sxs-lookup"><span data-stu-id="23b62-556">Meter Type</span></span></td>
<td><p><span data-ttu-id="23b62-557">Тип счетчика.</span><span class="sxs-lookup"><span data-stu-id="23b62-557">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-558">Категория счетчиков</span><span class="sxs-lookup"><span data-stu-id="23b62-558">Meter Category</span></span></td>
<td><p><span data-ttu-id="23b62-559">Служба верхнего уровня для использования.</span><span class="sxs-lookup"><span data-stu-id="23b62-559">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-560">Идентификатор счетчика</span><span class="sxs-lookup"><span data-stu-id="23b62-560">Meter Id</span></span></td>
<td><p><span data-ttu-id="23b62-561">Идентификатор используемого счетчика.</span><span class="sxs-lookup"><span data-stu-id="23b62-561">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-562">Подкатегория счетчика</span><span class="sxs-lookup"><span data-stu-id="23b62-562">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="23b62-563">Тип службы Azure, которая может повлиять на скорость.</span><span class="sxs-lookup"><span data-stu-id="23b62-563">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-564">Имя счетчика</span><span class="sxs-lookup"><span data-stu-id="23b62-564">Meter Name</span></span></td>
<td><p><span data-ttu-id="23b62-565">Единица измерения для потребляемого измерения.</span><span class="sxs-lookup"><span data-stu-id="23b62-565">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-566">Регион счетчика</span><span class="sxs-lookup"><span data-stu-id="23b62-566">Meter Region</span></span></td>
<td><p><span data-ttu-id="23b62-567">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="23b62-567">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-568">Unit</span><span class="sxs-lookup"><span data-stu-id="23b62-568">Unit</span></span></td>
<td><p><span data-ttu-id="23b62-569">Единица имени ресурса.</span><span class="sxs-lookup"><span data-stu-id="23b62-569">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-570">Потребленное количество</span><span class="sxs-lookup"><span data-stu-id="23b62-570">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="23b62-571">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="23b62-571">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="23b62-572">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="23b62-572">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-573">Расположение ресурса</span><span class="sxs-lookup"><span data-stu-id="23b62-573">Resource Location</span></span></td>
<td><p><span data-ttu-id="23b62-574">Центр обработки данных, в котором работает измерительный показатель.</span><span class="sxs-lookup"><span data-stu-id="23b62-574">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-575">Потребленная служба</span><span class="sxs-lookup"><span data-stu-id="23b62-575">Consumed Service</span></span></td>
<td><p><span data-ttu-id="23b62-576">Используемая служба платформы Azure.</span><span class="sxs-lookup"><span data-stu-id="23b62-576">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="23b62-577">URI ресурса</span><span class="sxs-lookup"><span data-stu-id="23b62-577">Resource URI</span></span></td>
<td><p><span data-ttu-id="23b62-578">URI используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="23b62-578">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-579">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="23b62-579">Charge type</span></span></td>
<td><p><span data-ttu-id="23b62-580">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="23b62-580">The type of charge or adjustment.</span></span> <span data-ttu-id="23b62-581">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="23b62-581">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-582">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="23b62-582">Unit price</span></span></td>
<td><p><span data-ttu-id="23b62-583">Цена за лицензию, опубликованная в PriceList на момент приобретения.</span><span class="sxs-lookup"><span data-stu-id="23b62-583">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="23b62-584">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-585">Количество</span><span class="sxs-lookup"><span data-stu-id="23b62-585">Quantity</span></span></td>
<td><p><span data-ttu-id="23b62-586">Число лицензий.</span><span class="sxs-lookup"><span data-stu-id="23b62-586">Number of licenses.</span></span> <span data-ttu-id="23b62-587">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-587">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-588">Тип единицы</span><span class="sxs-lookup"><span data-stu-id="23b62-588">Unit type</span></span></td>
<td><p><span data-ttu-id="23b62-589">Тип единицы измерения, за которую наследуется данный счетчик.</span><span class="sxs-lookup"><span data-stu-id="23b62-589">The type of unit the meter is charged in.</span></span> <span data-ttu-id="23b62-590">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="23b62-590">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-591">Выставление счетов за предварительный налог</span><span class="sxs-lookup"><span data-stu-id="23b62-591">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="23b62-592">Общая сумма перед налогами.</span><span class="sxs-lookup"><span data-stu-id="23b62-592">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-593">Валюта выставления счетов</span><span class="sxs-lookup"><span data-stu-id="23b62-593">Billing currency</span></span></td>
<td><p><span data-ttu-id="23b62-594">Валюта в географическом регионе клиента</span><span class="sxs-lookup"><span data-stu-id="23b62-594">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-595">Общие сведения о ценах цена</span><span class="sxs-lookup"><span data-stu-id="23b62-595">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="23b62-596">Цены перед добавлением налогов.</span><span class="sxs-lookup"><span data-stu-id="23b62-596">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-597">Валюта цены</span><span class="sxs-lookup"><span data-stu-id="23b62-597">Pricing currency</span></span></td>
<td><p><span data-ttu-id="23b62-598">Валюта в PriceList.</span><span class="sxs-lookup"><span data-stu-id="23b62-598">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="23b62-599">Сведения о службе 1</span><span class="sxs-lookup"><span data-stu-id="23b62-599">Service Info 1</span></span></td>
<td><p><span data-ttu-id="23b62-600">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="23b62-600">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-601">Сведения о службе 2</span><span class="sxs-lookup"><span data-stu-id="23b62-601">Service Info 2</span></span></td>
<td><p><span data-ttu-id="23b62-602">Устаревшее поле, которое фиксирует необязательные метаданные, относящиеся к службе.</span><span class="sxs-lookup"><span data-stu-id="23b62-602">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="23b62-603">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="23b62-603">Additional Info</span></span></td>
<td><p><span data-ttu-id="23b62-604">Дополнительные сведения, не охваченные другими столбцами.</span><span class="sxs-lookup"><span data-stu-id="23b62-604">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="23b62-605">Сопоставление расходов между счетом и файлом сверки</span><span class="sxs-lookup"><span data-stu-id="23b62-605">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="23b62-606">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="23b62-606">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="23b62-607">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-607">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="23b62-608">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="23b62-608">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="23b62-609">Одноразовые кредиты, скидки и возвраты денежных средств, которые отображаются в счете-фактуре как «Уточнения», не отображаются в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-609">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="23b62-610">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="23b62-610">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="23b62-611"><strong>Описание оплаты по счету</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-611"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-612"><strong>Описание оплаты файлов сверки (столбец Чаржетипе)</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-612"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-613"><strong>Что это за это?</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-613"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-614"><strong>Разделы справки сопоставлять эти Чаржетипес с накладной?</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-614"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="23b62-615"><strong>Оплата на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-615"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-616">Стоимость активации</span><span class="sxs-lookup"><span data-stu-id="23b62-616">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-617">Сумма, взимаемая с клиента при использовании подписки после ее приобретения</span><span class="sxs-lookup"><span data-stu-id="23b62-617">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="23b62-618">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="23b62-618">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-619">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="23b62-619">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-620">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="23b62-620">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-621">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="23b62-621">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-622">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="23b62-622">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-623">Пропорциональный перерасчет одного цикла</span><span class="sxs-lookup"><span data-stu-id="23b62-623">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-624">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="23b62-624">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-625">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="23b62-625">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-626">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="23b62-626">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-627">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="23b62-627">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-628">Тип оплаты для подписки при использовании годового счета</span><span class="sxs-lookup"><span data-stu-id="23b62-628">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-629">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="23b62-629">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-630">Тип оплаты для подписки при ежемесячном выставлении счетов</span><span class="sxs-lookup"><span data-stu-id="23b62-630">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-631">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="23b62-631">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-632">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-632">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="23b62-633">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="23b62-633">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-634">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-634">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-635">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="23b62-635">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-636">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="23b62-636">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="23b62-637"><strong>Оплата за один раз</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-637"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="23b62-638">Новый</span><span class="sxs-lookup"><span data-stu-id="23b62-638">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-639">Используется при создании новой покупки</span><span class="sxs-lookup"><span data-stu-id="23b62-639">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-640">addQuantity</span><span class="sxs-lookup"><span data-stu-id="23b62-640">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-641">Используется как для возврата первоначальной покупки, так и для нового количества после увеличения.</span><span class="sxs-lookup"><span data-stu-id="23b62-641">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-642">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="23b62-642">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-643">Используется как для возврата первоначальной покупки, так и для нового количества после уменьшения</span><span class="sxs-lookup"><span data-stu-id="23b62-643">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-644">"Отмена"</span><span class="sxs-lookup"><span data-stu-id="23b62-644">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-645">Используется при отмене подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-645">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-646">Преобразование</span><span class="sxs-lookup"><span data-stu-id="23b62-646">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-647">Используется при обновлении лицензии, но число рабочих мест остается неизменным</span><span class="sxs-lookup"><span data-stu-id="23b62-647">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="23b62-648"><strong>Плата за использование</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-648"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-649">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="23b62-649">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-650">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="23b62-650">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="23b62-651">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="23b62-651">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-652">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="23b62-652">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-653">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="23b62-653">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="23b62-654"><strong>Автор</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-654"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-655">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="23b62-655">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-656">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="23b62-656">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-657">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="23b62-657">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="23b62-658">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="23b62-658">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="23b62-659"><strong>Скидки на основе использования</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-659"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-660">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="23b62-660">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-661">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-661">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="23b62-662">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="23b62-662">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-663">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="23b62-663">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-664">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="23b62-664">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-665">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="23b62-665">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-666">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="23b62-666">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-667">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="23b62-667">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-668">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="23b62-668">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="23b62-669"><strong>Скидки на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-669"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-670"><em>Может применяться к нескольким типам оплаты</em></span><span class="sxs-lookup"><span data-stu-id="23b62-670"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="23b62-671">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="23b62-671">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="23b62-672"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="23b62-672"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-673"><em>Может применяться к нескольким типам оплаты</em></span><span class="sxs-lookup"><span data-stu-id="23b62-673"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="23b62-674"><em>Исключение: &quot;Offset элемент строки &quot; уже включает налоги. См. кредиты выше.</em></span><span class="sxs-lookup"><span data-stu-id="23b62-674"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-675">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="23b62-675">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="23b62-676">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="23b62-676">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="23b62-677">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="23b62-677">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
