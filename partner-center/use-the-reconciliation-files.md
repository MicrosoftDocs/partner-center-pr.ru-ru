---
title: Использование файлов выверки | Центр партнеров
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Для получения подробного представления по каждому элементу в цикле выставления счетов Скачайте файлы сверки из центра партнеров.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753850"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="7dd07-103">Использование файлов выверки</span><span class="sxs-lookup"><span data-stu-id="7dd07-103">Use the reconciliation files</span></span>

<span data-ttu-id="7dd07-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="7dd07-104">**Applies to**</span></span>

-  <span data-ttu-id="7dd07-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="7dd07-105">Partner Center</span></span>
-  <span data-ttu-id="7dd07-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="7dd07-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="7dd07-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="7dd07-107">**Appropriate roles**</span></span>

- <span data-ttu-id="7dd07-108">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="7dd07-108">Billing admin</span></span>
- <span data-ttu-id="7dd07-109">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7dd07-109">Global admin</span></span>

<span data-ttu-id="7dd07-110">Для получения подробного представления по каждому элементу в цикле выставления счетов Скачайте файлы сверки из центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="7dd07-111">Эти сведения включают плату за подписки каждого клиента и детализированные события (например, добавление количества мест к подписке в середине срока).</span><span class="sxs-lookup"><span data-stu-id="7dd07-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="7dd07-112">Проблемы форматирования</span><span class="sxs-lookup"><span data-stu-id="7dd07-112">Formatting issues</span></span>

<span data-ttu-id="7dd07-113">Иногда файл разведывательную может иметь проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="7dd07-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="7dd07-114">(Это может произойти, например, если языковой стандарт EN-US не используется.) Чтобы устранить эти проблемы, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="7dd07-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="7dd07-115">Откройте CSV-файл в Excel и выберите первый столбец.</span><span class="sxs-lookup"><span data-stu-id="7dd07-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="7dd07-116">На ленте выберите <strong>данные</strong>, а затем выберите <strong>текст в столбцах</strong>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="7dd07-117">В мастере преобразования текста в столбцы выберите <strong>Тип файла с разделителями</strong>, а затем нажмите кнопку <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="7dd07-118">В поле разделителями Выберите <strong>запятая</strong>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="7dd07-119">Если <strong>вкладка</strong> уже выбрана, можно оставить ее.</span><span class="sxs-lookup"><span data-stu-id="7dd07-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="7dd07-120">Выберите <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="7dd07-121">В поле Формат данных столбца выберите <strong>Date: mdy</strong>, а затем нажмите кнопку <strong>Далее</strong>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="7dd07-122">В поле Формат данных столбца выберите <strong>текст</strong> для всех столбцов суммы, а затем нажмите кнопку <strong>Готово</strong>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="7dd07-123">Скачивание большого файла разведывательную</span><span class="sxs-lookup"><span data-stu-id="7dd07-123">Downloading a large recon file</span></span>

<span data-ttu-id="7dd07-124">Файлы разведывательную могут увеличиваться очень большими и иногда трудно загружать.</span><span class="sxs-lookup"><span data-stu-id="7dd07-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="7dd07-125">Сведения о загрузке больших файлов разведывательную в скрипте PowerShell см. в разделе [Получение элементов строки счета](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="7dd07-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="7dd07-126">Детализировать по партнеру</span><span class="sxs-lookup"><span data-stu-id="7dd07-126">Itemize by partner</span></span>


<span data-ttu-id="7dd07-127">Партнеры в косвенной модели могут использовать эти дополнительные поля для детализации по торговым посредникам в файлах выверки как на основе лицензии, так и на основе использования.</span><span class="sxs-lookup"><span data-stu-id="7dd07-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="7dd07-128">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="7dd07-128">MPN ID</span></span></th>
<th><span data-ttu-id="7dd07-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd07-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="7dd07-130">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="7dd07-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="7dd07-131">Идентификатор сети Microsoft Partner Network (MPN) партнера CSP (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="7dd07-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-132">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="7dd07-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="7dd07-133">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="7dd07-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="7dd07-134">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="7dd07-135">Соответствует идентификатору торгового посредника, указанному для определенной подписки в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="7dd07-136">Ето просмотреть или обновить торгового посредника, в меню центра партнеров выберите <strong>Клиенты</strong>, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="7dd07-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="7dd07-137">В меню клиента выберите <strong>Подписки</strong>, а затем выберите нужную подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="7dd07-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="7dd07-138">Выберите <strong>обновить</strong>, чтобы изменить пункт <strong>Торговый посредник (идентификатор MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="7dd07-139">Если партнер CSP продал подписку непосредственно клиенту, то его идентификатор MPN указывается дважды, как идентификатор MPN и как идентификатор MPN торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="7dd07-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="7dd07-140">Если у партнера CSP есть посредника, у которого нет идентификатора MPN, вместо него задается идентификатор MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="7dd07-141">Если партнер CSP удалил идентификатор торгового посредника, значение в этом поле равно -1.</span><span class="sxs-lookup"><span data-stu-id="7dd07-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="7dd07-142">Поля файла на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="7dd07-142">License-based file fields</span></span>


<span data-ttu-id="7dd07-143">Чтобы согласовать ваши оплаты с заказами ваших клиентов, сравните свойство Syndication\_Partner\_Subscription\_Number из файла выверки с идентификационным кодом подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="7dd07-144"><strong>Рубрик</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="7dd07-145"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="7dd07-146"><strong>Пример значения</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="7dd07-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="7dd07-148">Уникальный идентификатор для конкретного объекта выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="7dd07-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="7dd07-149">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="7dd07-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="7dd07-150">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="7dd07-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="7dd07-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="7dd07-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="7dd07-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="7dd07-153">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="7dd07-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="7dd07-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="7dd07-155">OrderID</span></span></td>
<td><p><span data-ttu-id="7dd07-156">Уникальный идентификатор заказа на платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7dd07-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="7dd07-157">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="7dd07-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="7dd07-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="7dd07-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="7dd07-160">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7dd07-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="7dd07-161">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="7dd07-162">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="7dd07-163">См. поле Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="7dd07-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="7dd07-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="7dd07-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="7dd07-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="7dd07-166">Уникальный идентификатор для подписок.</span><span class="sxs-lookup"><span data-stu-id="7dd07-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="7dd07-167">Клиент может иметь несколько подписок для одного плана, поэтому этот параметр важен для анализа файла выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="7dd07-168">Это поле сопоставлено с идентификатором подписки в консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="7dd07-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="7dd07-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="7dd07-170">OfferID</span></span></td>
<td><p><span data-ttu-id="7dd07-171">Уникальный идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="7dd07-171">Unique offer ID.</span></span> <span data-ttu-id="7dd07-172">Идентификатор стандартного предложения в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="7dd07-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="7dd07-173"><b>Примечание</b>: это значение не соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="7dd07-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="7dd07-174">См. пункт «DurableOfferID» ниже.</span><span class="sxs-lookup"><span data-stu-id="7dd07-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="7dd07-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="7dd07-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="7dd07-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="7dd07-177">Уникальный идентификатор длительного предложения, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="7dd07-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="7dd07-178"><b>Примечание</b>. Это значение соответствует идентификатору предложения из прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="7dd07-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="7dd07-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="7dd07-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="7dd07-180">OfferName</span></span></td>
<td><p><span data-ttu-id="7dd07-181">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="7dd07-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="7dd07-182">Microsoft Office 365 (план E3)</span><span class="sxs-lookup"><span data-stu-id="7dd07-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="7dd07-184">Дата начала подписки — это день после отправки заказа.</span><span class="sxs-lookup"><span data-stu-id="7dd07-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="7dd07-185">Сопоставив даты начала и завершения подписки, вы можете определить, находится ли клиент на первом году подписки, или подписка возобновлена на следующий год.</span><span class="sxs-lookup"><span data-stu-id="7dd07-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="7dd07-186">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="7dd07-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7dd07-187">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="7dd07-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="7dd07-189">Дата завершения подписки — 12 месяцев + x дней после даты начала (чтобы совместить с датой выставления счетов партнера) или 12 месяцев от даты возобновления действия.</span><span class="sxs-lookup"><span data-stu-id="7dd07-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="7dd07-190">При возобновлении цены обновляются в соответствии с текущим прайс-листом.</span><span class="sxs-lookup"><span data-stu-id="7dd07-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="7dd07-191">При автоматическом возобновлении, возможно, необходимо будет заранее связаться с клиентом.</span><span class="sxs-lookup"><span data-stu-id="7dd07-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="7dd07-192">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="7dd07-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7dd07-193">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="7dd07-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="7dd07-195">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="7dd07-196">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="7dd07-197">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="7dd07-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7dd07-198">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="7dd07-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="7dd07-200">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="7dd07-201">Если пользователь изменяет количество мест, это количество используется для расчета ежедневной (пропорциональный расчет) оплаты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="7dd07-202">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="7dd07-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="7dd07-203">28.02.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="7dd07-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="7dd07-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="7dd07-205">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-205">The type of charge or adjustment.</span></span> <span data-ttu-id="7dd07-206">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="7dd07-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="7dd07-207">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="7dd07-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="7dd07-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="7dd07-209">Цена за рабочее место, опубликованное в прайс-листе во время покупки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="7dd07-210">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="7dd07-211">6,82</span><span class="sxs-lookup"><span data-stu-id="7dd07-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-212">Количество</span><span class="sxs-lookup"><span data-stu-id="7dd07-212">Quantity</span></span></td>
<td><p><span data-ttu-id="7dd07-213">Количество мест.</span><span class="sxs-lookup"><span data-stu-id="7dd07-213">Number of seats.</span></span> <span data-ttu-id="7dd07-214">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="7dd07-215">2</span><span class="sxs-lookup"><span data-stu-id="7dd07-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-216">Сумма</span><span class="sxs-lookup"><span data-stu-id="7dd07-216">Amount</span></span></td>
<td><p><span data-ttu-id="7dd07-217">Общая цена за количество.</span><span class="sxs-lookup"><span data-stu-id="7dd07-217">Total of price for quantity.</span></span> <span data-ttu-id="7dd07-218">Позволяет убедиться, что сумма расчета соответствует способу вычисления для клиентов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="7dd07-219">13,32</span><span class="sxs-lookup"><span data-stu-id="7dd07-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="7dd07-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="7dd07-221">Сумма скидки, примененная к этой оплате.</span><span class="sxs-lookup"><span data-stu-id="7dd07-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="7dd07-222">Лицензии на продукт, входящие в компетенцию или карты или новые подписки, подходящие для стимула, также будут содержать сумму скидки в этой статье.</span><span class="sxs-lookup"><span data-stu-id="7dd07-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="7dd07-223">2,32</span><span class="sxs-lookup"><span data-stu-id="7dd07-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-224">Промежуточный итог</span><span class="sxs-lookup"><span data-stu-id="7dd07-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="7dd07-225">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="7dd07-225">Total before tax.</span></span> <span data-ttu-id="7dd07-226">В случае применения скидки промежуточный итог должен соответствовать ожидаемой итоговой сумме.</span><span class="sxs-lookup"><span data-stu-id="7dd07-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="7dd07-227">11</span><span class="sxs-lookup"><span data-stu-id="7dd07-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-228">Налог</span><span class="sxs-lookup"><span data-stu-id="7dd07-228">Tax</span></span></td>
<td><p><span data-ttu-id="7dd07-229">Сумма налога взимается на основе правил налогов на&#39;рынке и определенных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="7dd07-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="7dd07-230">0</span><span class="sxs-lookup"><span data-stu-id="7dd07-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="7dd07-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="7dd07-232">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-232">Total after tax.</span></span> <span data-ttu-id="7dd07-233">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="7dd07-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="7dd07-234">11</span><span class="sxs-lookup"><span data-stu-id="7dd07-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-235">Валюта</span><span class="sxs-lookup"><span data-stu-id="7dd07-235">Currency</span></span></td>
<td><p><span data-ttu-id="7dd07-236">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-236">Currency type.</span></span> <span data-ttu-id="7dd07-237">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="7dd07-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="7dd07-238">Проверьте, соответствует ли тип валюты вашему первому счету-фактуре. Повторяйте эту проверку после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="7dd07-239">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="7dd07-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="7dd07-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="7dd07-241">Имя&#39;организации клиента согласно сообщению в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="7dd07-242">Очень важный элемент для сверки счета-фактуры с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="7dd07-243">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="7dd07-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="7dd07-244">MPNID</span></span></td>
<td><p><span data-ttu-id="7dd07-245">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="7dd07-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="7dd07-246">4390934</span><span class="sxs-lookup"><span data-stu-id="7dd07-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="7dd07-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="7dd07-248">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="7dd07-249">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="7dd07-250">4390934</span><span class="sxs-lookup"><span data-stu-id="7dd07-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="7dd07-251">DomainName</span></span></td>
<td><p><span data-ttu-id="7dd07-252">Имя&#39;домена клиента, используемое для поиска клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="7dd07-253">Его не следует использовать для уникальной идентификации клиента, так как клиент или партнер может обновить домен именного/Default через портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="7dd07-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="7dd07-254">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="7dd07-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7dd07-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="7dd07-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="7dd07-257">Псевдоним подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-257">Subscription nickname.</span></span> <span data-ttu-id="7dd07-258">Если псевдоним не указан, Центр партнеров использует значение OfferName.</span><span class="sxs-lookup"><span data-stu-id="7dd07-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="7dd07-259">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="7dd07-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="7dd07-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="7dd07-261">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="7dd07-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="7dd07-262">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="7dd07-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="7dd07-263">PROJECT ONLINE РАСШИРЕННЫЙ БЕЗ КЛИЕНТА PROJECT</span><span class="sxs-lookup"><span data-stu-id="7dd07-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="7dd07-264">Поля файла на основе использования</span><span class="sxs-lookup"><span data-stu-id="7dd07-264">Usage-based file fields</span></span>


<span data-ttu-id="7dd07-265">Чтобы выверить ваши взносы с использованием ваших клиентов, сравните поля ResellerID/ResellerName/ResellerBillableAccount из файла выверки, имя клиента и идентификатор подписки из Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="7dd07-266">В следующих полях объясняется, какие услуги были использованы и по какому тарифу.</span><span class="sxs-lookup"><span data-stu-id="7dd07-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="7dd07-267"><strong>Рубрик</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="7dd07-268"><strong>Описание</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="7dd07-269"><strong>Пример значения</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="7dd07-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="7dd07-271">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="7dd07-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="7dd07-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="7dd07-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="7dd07-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="7dd07-274">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="7dd07-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="7dd07-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="7dd07-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="7dd07-277">Идентификатор учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="7dd07-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="7dd07-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="7dd07-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="7dd07-280">Имя&#39;организации клиента согласно сообщению в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="7dd07-281">Очень важный элемент для сверки счета-фактуры с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="7dd07-282">Тестовый клиент A</span><span class="sxs-lookup"><span data-stu-id="7dd07-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="7dd07-283">MPNID</span></span></td>
<td><p><span data-ttu-id="7dd07-284">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="7dd07-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="7dd07-285">4390934</span><span class="sxs-lookup"><span data-stu-id="7dd07-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="7dd07-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="7dd07-287">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="7dd07-288">См. раздел <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Детализация по партнерам</a>.</span><span class="sxs-lookup"><span data-stu-id="7dd07-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="7dd07-289">4390934</span><span class="sxs-lookup"><span data-stu-id="7dd07-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="7dd07-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="7dd07-291">Номер счета-фактуры, содержащего указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="7dd07-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="7dd07-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="7dd07-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="7dd07-294">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="7dd07-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="7dd07-295">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="7dd07-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7dd07-296">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="7dd07-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="7dd07-298">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="7dd07-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="7dd07-299">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="7dd07-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="7dd07-300">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="7dd07-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="7dd07-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="7dd07-302">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7dd07-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="7dd07-303">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="7dd07-304">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="7dd07-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="7dd07-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="7dd07-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="7dd07-307">Псевдоним предложения службы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="7dd07-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="7dd07-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="7dd07-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="7dd07-310">Отрасль, к которой относится предложение службы</span><span class="sxs-lookup"><span data-stu-id="7dd07-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="7dd07-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="7dd07-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="7dd07-312">OrderID</span></span></td>
<td><p><span data-ttu-id="7dd07-313">Уникальный идентификатор заказа на платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7dd07-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="7dd07-314">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="7dd07-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="7dd07-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="7dd07-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="7dd07-317">Имя соответствующей службы Azure.</span><span class="sxs-lookup"><span data-stu-id="7dd07-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="7dd07-318">ВИРТУАЛЬНЫЕ МАШИНЫ</span><span class="sxs-lookup"><span data-stu-id="7dd07-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="7dd07-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="7dd07-320">Определенный тип службы Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="7dd07-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="7dd07-321">Служебная шина — индивидуальная или Pack</span><span class="sxs-lookup"><span data-stu-id="7dd07-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="7dd07-322">SQL Azure Database — Business или Web Edition</span><span class="sxs-lookup"><span data-stu-id="7dd07-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="7dd07-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="7dd07-324">Определенный уникальный идентификатор для всех данных и ценовой структуры службы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="7dd07-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="7dd07-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-326">Resource Name</span><span class="sxs-lookup"><span data-stu-id="7dd07-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="7dd07-327">Имя ресурса Azure.</span><span class="sxs-lookup"><span data-stu-id="7dd07-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="7dd07-328">Входящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="7dd07-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="7dd07-329">Исходящая передача данных (ГБ)</span><span class="sxs-lookup"><span data-stu-id="7dd07-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-330">Region</span><span class="sxs-lookup"><span data-stu-id="7dd07-330">Region</span></span></td>
<td><p><span data-ttu-id="7dd07-331">Регион, к которому применяется использование.</span><span class="sxs-lookup"><span data-stu-id="7dd07-331">The region the usage applies to.</span></span> <span data-ttu-id="7dd07-332">В основном используется для назначения тарифов за передачу данных, поскольку тарифы зависят от региона.</span><span class="sxs-lookup"><span data-stu-id="7dd07-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="7dd07-333">Азиатско-Тихоокеанский регион, Европа, Латинская Америка, Северная Америка</span><span class="sxs-lookup"><span data-stu-id="7dd07-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-334">SKU</span><span class="sxs-lookup"><span data-stu-id="7dd07-334">SKU</span></span></td>
<td><p><span data-ttu-id="7dd07-335">Уникальный идентификатор MSFT для предложения</span><span class="sxs-lookup"><span data-stu-id="7dd07-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="7dd07-336">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="7dd07-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="7dd07-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="7dd07-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="7dd07-338">Идентификатор и количество для детализации различных тарифов за услугу или ресурс за определенный период выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="7dd07-339">В многоуровневой системе тарифов Azure для определенного количества платных единиц может быть указан один тариф, а за ним — другой.</span><span class="sxs-lookup"><span data-stu-id="7dd07-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="7dd07-340">1</span><span class="sxs-lookup"><span data-stu-id="7dd07-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="7dd07-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="7dd07-342">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7dd07-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="7dd07-343">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="7dd07-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="7dd07-344">11</span><span class="sxs-lookup"><span data-stu-id="7dd07-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="7dd07-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="7dd07-346">Единицы в составе предложения.</span><span class="sxs-lookup"><span data-stu-id="7dd07-346">Units included as part of the offer.</span></span> <span data-ttu-id="7dd07-347">Обычно отсутствует в CSP.</span><span class="sxs-lookup"><span data-stu-id="7dd07-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="7dd07-348">0</span><span class="sxs-lookup"><span data-stu-id="7dd07-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="7dd07-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="7dd07-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="7dd07-350">Единицы, не включенные в предложение, которые должен оплатить партнер.</span><span class="sxs-lookup"><span data-stu-id="7dd07-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="7dd07-351">Равняется разнице значений полей ConsumedQuantity и IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="7dd07-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="7dd07-352">11</span><span class="sxs-lookup"><span data-stu-id="7dd07-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="7dd07-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="7dd07-354">Цена предложения на дату начала действия подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="7dd07-355">0,0808 долл. США</span><span class="sxs-lookup"><span data-stu-id="7dd07-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="7dd07-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="7dd07-357">Произведение значений полей ListPrist и OverageQuantity, округленное до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="7dd07-358">0,085 долл. США</span><span class="sxs-lookup"><span data-stu-id="7dd07-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="7dd07-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="7dd07-360">Сумма налога взимается на основе правил налогов на&#39;рынке и определенных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="7dd07-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="7dd07-361">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="7dd07-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="7dd07-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="7dd07-363">Итоговая сумма за вычетом налога, если таковой применим.</span><span class="sxs-lookup"><span data-stu-id="7dd07-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="7dd07-364">0,93 долл. США</span><span class="sxs-lookup"><span data-stu-id="7dd07-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-365">Валюта</span><span class="sxs-lookup"><span data-stu-id="7dd07-365">Currency</span></span></td>
<td><p><span data-ttu-id="7dd07-366">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-366">Currency type.</span></span> <span data-ttu-id="7dd07-367">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="7dd07-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="7dd07-368">Проверьте, соответствует ли тип валюты вашему первому счету-фактуре. Повторяйте эту проверку после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="7dd07-369">Евро (EUR)</span><span class="sxs-lookup"><span data-stu-id="7dd07-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="7dd07-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="7dd07-371">Цена за единицу до вычета налогов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-371">Pretax price per unit.</span></span> <span data-ttu-id="7dd07-372">Равняется отношению значения поля PretaxCharges к значению поля OverageQuantity, округленному до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="7dd07-373">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="7dd07-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="7dd07-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="7dd07-375">Цена за единицу после вычета налога.</span><span class="sxs-lookup"><span data-stu-id="7dd07-375">Post tax price per unit.</span></span> <span data-ttu-id="7dd07-376">Равняется отношению значения поля PostTaxTotal к значению поля OverageQuantity или сумме значения поля PretaxEffectiveRate и налоговой ставке за единицу, округленным до ближайшего цента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="7dd07-377">0,08 долл. США</span><span class="sxs-lookup"><span data-stu-id="7dd07-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="7dd07-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="7dd07-379">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-379">The type of charge or adjustment.</span></span> <span data-ttu-id="7dd07-380">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="7dd07-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="7dd07-381">См. раздел <a href="#charge_types">Сопоставление расходов в счете-фактуре и файле выверки</a></span><span class="sxs-lookup"><span data-stu-id="7dd07-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="7dd07-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="7dd07-383">Уникальный идентификатор учетной записи в платформе выставления счетов MSFT.</span><span class="sxs-lookup"><span data-stu-id="7dd07-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="7dd07-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="7dd07-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="7dd07-386">Дата развертывания службы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="7dd07-387">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="7dd07-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="7dd07-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="7dd07-389">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="7dd07-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="7dd07-390">Восточная Азия, Юго-Восточная Азия, Северная Европа, Западная Европа, Северо-Центральные штаты США, Южно-Центральные штаты США</span><span class="sxs-lookup"><span data-stu-id="7dd07-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-391">Измеренная_служба</span><span class="sxs-lookup"><span data-stu-id="7dd07-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="7dd07-392">Этот столбец используется для отслеживания отдельной службы Microsoft Azure, которую невозможно точно определить в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="7dd07-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="7dd07-393">Например, передача данных отражается как &quot;Microsoft Azure — все службы&quot; в столбце "Название службы".</span><span class="sxs-lookup"><span data-stu-id="7dd07-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="7dd07-394">Столбец "Измеренная_служба" будет указывать, к какой конкретной службе относится использование.</span><span class="sxs-lookup"><span data-stu-id="7dd07-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="7dd07-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="7dd07-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="7dd07-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="7dd07-397">Подзаголовок с уточняющими сведениями об отдельной службе Microsoft Azure за пределами уровня, указанного в поле MeteredService.</span><span class="sxs-lookup"><span data-stu-id="7dd07-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="7dd07-398">ВНЕШНЯЯ</span><span class="sxs-lookup"><span data-stu-id="7dd07-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-399">Проект</span><span class="sxs-lookup"><span data-stu-id="7dd07-399">Project</span></span></td>
<td><p><span data-ttu-id="7dd07-400">Указанное клиентом имя экземпляра службы</span><span class="sxs-lookup"><span data-stu-id="7dd07-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="7dd07-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="7dd07-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="7dd07-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="7dd07-403">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="7dd07-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="7dd07-404">Например, если в течение 30-дневного месяца было настроено отдельное подключение, в сведениях о службе 1 будет считано «1,000000 подключений/30 дней».</span><span class="sxs-lookup"><span data-stu-id="7dd07-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="7dd07-405">Если у вас есть 25 ServiceBus подключений и вы использовали 1 в течение этого дня, в течение этого дня инструкция ежедневного использования будет означать "25 соединений/30 дней-используется: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="7dd07-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="7dd07-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="7dd07-407">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="7dd07-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="7dd07-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="7dd07-409">DomainName</span></span></td>
<td><p><span data-ttu-id="7dd07-410">Имя&#39;домена клиента, используемое для поиска клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="7dd07-411">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="7dd07-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7dd07-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-413">Unit</span><span class="sxs-lookup"><span data-stu-id="7dd07-413">Unit</span></span></td>
<td><p><span data-ttu-id="7dd07-414">Единица измерения имени ресурса</span><span class="sxs-lookup"><span data-stu-id="7dd07-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="7dd07-415">ГБ или ЧАСЫ</span><span class="sxs-lookup"><span data-stu-id="7dd07-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="7dd07-416">Поля однократного и повторяющегося файлов</span><span class="sxs-lookup"><span data-stu-id="7dd07-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="7dd07-417">Column</span><span class="sxs-lookup"><span data-stu-id="7dd07-417">Column</span></span></th>
<th><span data-ttu-id="7dd07-418">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd07-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="7dd07-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="7dd07-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="7dd07-420">Уникальный идентификатор клиента Microsoft Azure Active Directory для определенной сущности выставления счетов в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="7dd07-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="7dd07-421">Не требуется для выверки, но при этом может содержать полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="7dd07-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="7dd07-422">Одинаково во всех строках.</span><span class="sxs-lookup"><span data-stu-id="7dd07-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-423">Идентификатор клиента</span><span class="sxs-lookup"><span data-stu-id="7dd07-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="7dd07-424">Уникальный идентификатор клиента Microsoft Azure Active Directory в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-425">Customer Name (Имя клиента)</span><span class="sxs-lookup"><span data-stu-id="7dd07-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="7dd07-426">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="7dd07-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="7dd07-428">Доменное имя клиента, используемое для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="7dd07-429">Его не следует использовать для уникальной идентификации клиента, так как клиент или партнер может обновить домен именного/Default через портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="7dd07-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="7dd07-430">Это поле может быть пустым до второго цикла выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-431">Страна клиента</span><span class="sxs-lookup"><span data-stu-id="7dd07-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="7dd07-432">Страна, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="7dd07-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-433">Номер счета</span><span class="sxs-lookup"><span data-stu-id="7dd07-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="7dd07-434">Номер счета-фактуры, содержащего указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="7dd07-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="7dd07-435">MpnId</span></span></td>
<td><p><span data-ttu-id="7dd07-436">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="7dd07-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-437">MpnId торгового посредника</span><span class="sxs-lookup"><span data-stu-id="7dd07-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="7dd07-438">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-439">Идентификатор заказа</span><span class="sxs-lookup"><span data-stu-id="7dd07-439">Order ID</span></span></td>
<td><p><span data-ttu-id="7dd07-440">Уникальный идентификатор для заказа на платформе Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="7dd07-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="7dd07-441">Может использоваться для определения заказа при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-442">Дата заказа</span><span class="sxs-lookup"><span data-stu-id="7dd07-442">Order date</span></span></td>
<td><p><span data-ttu-id="7dd07-443">Дата размещения заказа.</span><span class="sxs-lookup"><span data-stu-id="7dd07-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-444">ProductID</span><span class="sxs-lookup"><span data-stu-id="7dd07-444">ProductId</span></span></td>
<td><p><span data-ttu-id="7dd07-445">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="7dd07-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="7dd07-446">SkuId</span></span></td>
<td><p><span data-ttu-id="7dd07-447">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="7dd07-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="7dd07-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="7dd07-449">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-449">The ID for a particular Availability.</span></span> <span data-ttu-id="7dd07-450">"Доступность" означает, доступен ли конкретный номер SKU для покупки в указанной стране, валюте, отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="7dd07-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-451">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="7dd07-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="7dd07-452">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="7dd07-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-453">название продукта;</span><span class="sxs-lookup"><span data-stu-id="7dd07-453">Product name</span></span></td>
<td><p><span data-ttu-id="7dd07-454">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="7dd07-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="7dd07-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="7dd07-456">Имя издателя продукта.</span><span class="sxs-lookup"><span data-stu-id="7dd07-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="7dd07-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="7dd07-458">Уникальный идентификатор для этого издателя.</span><span class="sxs-lookup"><span data-stu-id="7dd07-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-459">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="7dd07-460">Понятное имя подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-461">Код подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="7dd07-462">Уникальный идентификатор подписки в платформе Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="7dd07-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="7dd07-463">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="7dd07-464">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="7dd07-466">Дата начала взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-466">Start day of the charges.</span></span> <span data-ttu-id="7dd07-467">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="7dd07-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="7dd07-469">День завершения взимания оплаты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-469">End day of the charges.</span></span> <span data-ttu-id="7dd07-470">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="7dd07-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-471">Term и Биллингцикле</span><span class="sxs-lookup"><span data-stu-id="7dd07-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="7dd07-472">Срок и цикл выставления счетов для покупки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="7dd07-473">Например, "1 год, месяц".</span><span class="sxs-lookup"><span data-stu-id="7dd07-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-474">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="7dd07-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="7dd07-475">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-476">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="7dd07-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="7dd07-477">Цена, опубликованная в PriceList во время покупки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="7dd07-478">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-479">Эффективная цена за единицу</span><span class="sxs-lookup"><span data-stu-id="7dd07-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="7dd07-480">Цена за единицу после внесения корректировок.</span><span class="sxs-lookup"><span data-stu-id="7dd07-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-481">Количество</span><span class="sxs-lookup"><span data-stu-id="7dd07-481">Quantity</span></span></td>
<td><p><span data-ttu-id="7dd07-482">Количество единиц.</span><span class="sxs-lookup"><span data-stu-id="7dd07-482">Number of units.</span></span> <span data-ttu-id="7dd07-483">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-484">Тип единицы</span><span class="sxs-lookup"><span data-stu-id="7dd07-484">Unit type</span></span></td>
<td><p><span data-ttu-id="7dd07-485">Тип приобретаемой единицы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-486">прицеаджустментдескриптион</span><span class="sxs-lookup"><span data-stu-id="7dd07-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="7dd07-487">Описание применимой скидки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-488">Итого</span><span class="sxs-lookup"><span data-stu-id="7dd07-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="7dd07-489">Сумма до налога.</span><span class="sxs-lookup"><span data-stu-id="7dd07-489">Total before tax.</span></span> <span data-ttu-id="7dd07-490">В случае применения скидки промежуточный итог должен соответствовать ожидаемой итоговой сумме.</span><span class="sxs-lookup"><span data-stu-id="7dd07-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-491">Сумма налогов</span><span class="sxs-lookup"><span data-stu-id="7dd07-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="7dd07-492">Сумма налоговых сборов на основании правил налогообложения вашего рынка и конкретных обстоятельств.</span><span class="sxs-lookup"><span data-stu-id="7dd07-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-493">Total (Всего)</span><span class="sxs-lookup"><span data-stu-id="7dd07-493">Total</span></span></td>
<td><p><span data-ttu-id="7dd07-494">Цена после налогов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-494">Total after tax.</span></span> <span data-ttu-id="7dd07-495">Проверьте, вычтены ли с вас налоги в накладной.</span><span class="sxs-lookup"><span data-stu-id="7dd07-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-496">Валюта</span><span class="sxs-lookup"><span data-stu-id="7dd07-496">Currency</span></span></td>
<td><p><span data-ttu-id="7dd07-497">Тип валюты.</span><span class="sxs-lookup"><span data-stu-id="7dd07-497">Currency type.</span></span> <span data-ttu-id="7dd07-498">Каждый объект выставления счетов имеет только одну валюту.</span><span class="sxs-lookup"><span data-stu-id="7dd07-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="7dd07-499">Проверьте, соответствует ли тип валюты вашему первому счету-фактуре. Повторяйте эту проверку после каждого крупного обновления платформы выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-500">Альтернативного имени пользователя</span><span class="sxs-lookup"><span data-stu-id="7dd07-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="7dd07-501">Альтернативный идентификатор для идентификатора заказа.</span><span class="sxs-lookup"><span data-stu-id="7dd07-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-502">биллингфрекуенци</span><span class="sxs-lookup"><span data-stu-id="7dd07-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="7dd07-503">Выводится ежемесячно, если включен ежемесячный счет.</span><span class="sxs-lookup"><span data-stu-id="7dd07-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="7dd07-504">В противном случае оставьте пустым.</span><span class="sxs-lookup"><span data-stu-id="7dd07-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-505">биллаблекуантити</span><span class="sxs-lookup"><span data-stu-id="7dd07-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="7dd07-506">Представляет общее количество приобретенных или израсходованных единиц.</span><span class="sxs-lookup"><span data-stu-id="7dd07-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-507">приЦингкурренци</span><span class="sxs-lookup"><span data-stu-id="7dd07-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="7dd07-508">Список цен на ресурс или предложение</span><span class="sxs-lookup"><span data-stu-id="7dd07-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-509">пктобцексчанжерате</span><span class="sxs-lookup"><span data-stu-id="7dd07-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="7dd07-510">Валютный курс, применяемый для валюты цены (Customers) в расчетной валюте</span><span class="sxs-lookup"><span data-stu-id="7dd07-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-511">пктобцексчанжератедате</span><span class="sxs-lookup"><span data-stu-id="7dd07-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="7dd07-512">Дата, с которой определяется Валюта валютного курса для валюты выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-513">метердескриптион</span><span class="sxs-lookup"><span data-stu-id="7dd07-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="7dd07-514">Описание счетчика для элемента строки потребления</span><span class="sxs-lookup"><span data-stu-id="7dd07-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="7dd07-515">Поля файла с ежедневной оценкой использования</span><span class="sxs-lookup"><span data-stu-id="7dd07-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="7dd07-516">Column</span><span class="sxs-lookup"><span data-stu-id="7dd07-516">Column</span></span></th>
<th><span data-ttu-id="7dd07-517">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd07-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="7dd07-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="7dd07-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="7dd07-519">Идентификатор партнера в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="7dd07-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="7dd07-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="7dd07-521">Имя партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="7dd07-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="7dd07-523">Уникальный идентификатор Майкрософт в формате GUID, используемый для идентификации клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-524">кустомеркомпанинаме</span><span class="sxs-lookup"><span data-stu-id="7dd07-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="7dd07-525">Имя организации клиента, указанное в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="7dd07-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="7dd07-526">Очень важный элемент для сверки счета-фактуры с данными вашей системы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="7dd07-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="7dd07-528">Доменное имя клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd07-528">The customer's domain name.</span></span> <span data-ttu-id="7dd07-529">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-530">Страна клиента</span><span class="sxs-lookup"><span data-stu-id="7dd07-530">Customer country</span></span></td>
<td><p><span data-ttu-id="7dd07-531">Страна, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="7dd07-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="7dd07-532">MPNID</span></span></td>
<td><p><span data-ttu-id="7dd07-533">Идентификатор MPN партнера CSP</span><span class="sxs-lookup"><span data-stu-id="7dd07-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-534">MPNID торгового посредника</span><span class="sxs-lookup"><span data-stu-id="7dd07-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="7dd07-535">Идентификатор MPN зарегистрированного торгового посредника для подписки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="7dd07-536">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="7dd07-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="7dd07-538">Номер счета-фактуры, содержащего указанную транзакцию.</span><span class="sxs-lookup"><span data-stu-id="7dd07-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="7dd07-539">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-540">ProductID</span><span class="sxs-lookup"><span data-stu-id="7dd07-540">ProductId</span></span></td>
<td><p><span data-ttu-id="7dd07-541">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="7dd07-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="7dd07-542">SkuId</span></span></td>
<td><p><span data-ttu-id="7dd07-543">Идентификатор определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="7dd07-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="7dd07-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="7dd07-545">Идентификатор определенного статуса доступности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-545">The ID for a particular Availability.</span></span> <span data-ttu-id="7dd07-546">"Доступность" означает, доступен ли конкретный номер SKU для покупки в указанной стране, валюте, отрасли и т. д.</span><span class="sxs-lookup"><span data-stu-id="7dd07-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-547">Имя SKU</span><span class="sxs-lookup"><span data-stu-id="7dd07-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="7dd07-548">Название для определенного номера SKU.</span><span class="sxs-lookup"><span data-stu-id="7dd07-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="7dd07-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="7dd07-550">Имя издателя.</span><span class="sxs-lookup"><span data-stu-id="7dd07-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="7dd07-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="7dd07-552">Идентификатор издателя в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="7dd07-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="7dd07-553">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-554">Описание подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="7dd07-555">Имя предложения службы, приобретенной клиентом, как указано в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="7dd07-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="7dd07-556">(Данное поле идентично полю «Название предложения»).</span><span class="sxs-lookup"><span data-stu-id="7dd07-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-557">Код подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="7dd07-558">Уникальный идентификатор подписки в платформе выставления счетов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7dd07-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="7dd07-559">Может быть полезным для определения подписки при обращении в службу поддержки, но не для выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="7dd07-560">Не совпадает с идентификатором подписки на консоли администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="7dd07-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="7dd07-562">Дата начала цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="7dd07-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="7dd07-563">Временем всегда является начало дня, 0:00.</span><span class="sxs-lookup"><span data-stu-id="7dd07-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="7dd07-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="7dd07-565">Дата окончания цикла выставления счетов за исключением представления дат ранее не оплаченных данных скрытого использования (из предыдущего цикла выставления счетов).</span><span class="sxs-lookup"><span data-stu-id="7dd07-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="7dd07-566">Временем всегда является конец дня, 23:59.</span><span class="sxs-lookup"><span data-stu-id="7dd07-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-567">Дата использования</span><span class="sxs-lookup"><span data-stu-id="7dd07-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="7dd07-568">Дата использования службы.</span><span class="sxs-lookup"><span data-stu-id="7dd07-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-569">Тип счетчика</span><span class="sxs-lookup"><span data-stu-id="7dd07-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="7dd07-570">Тип счетчика.</span><span class="sxs-lookup"><span data-stu-id="7dd07-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-571">Категория счетчиков</span><span class="sxs-lookup"><span data-stu-id="7dd07-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="7dd07-572">Служба верхнего уровня для использования.</span><span class="sxs-lookup"><span data-stu-id="7dd07-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-573">Идентификатор счетчика</span><span class="sxs-lookup"><span data-stu-id="7dd07-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="7dd07-574">Идентификатор используемого счетчика.</span><span class="sxs-lookup"><span data-stu-id="7dd07-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-575">Подкатегория счетчика</span><span class="sxs-lookup"><span data-stu-id="7dd07-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="7dd07-576">Тип службы Azure, которая может повлиять на скорость.</span><span class="sxs-lookup"><span data-stu-id="7dd07-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-577">Имя счетчика</span><span class="sxs-lookup"><span data-stu-id="7dd07-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="7dd07-578">Единица измерения для потребляемого измерения.</span><span class="sxs-lookup"><span data-stu-id="7dd07-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-579">Регион счетчика</span><span class="sxs-lookup"><span data-stu-id="7dd07-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="7dd07-580">Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется.</span><span class="sxs-lookup"><span data-stu-id="7dd07-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-581">Unit</span><span class="sxs-lookup"><span data-stu-id="7dd07-581">Unit</span></span></td>
<td><p><span data-ttu-id="7dd07-582">Единица имени ресурса.</span><span class="sxs-lookup"><span data-stu-id="7dd07-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-583">Потребленное количество</span><span class="sxs-lookup"><span data-stu-id="7dd07-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="7dd07-584">Потребленный объем службы (часы, ГБ и так далее) за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7dd07-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="7dd07-585">Также включает использованный объем за предыдущие отчетные периоды, по которому не выставлялся счет.</span><span class="sxs-lookup"><span data-stu-id="7dd07-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-586">Расположение ресурса</span><span class="sxs-lookup"><span data-stu-id="7dd07-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="7dd07-587">Центр обработки данных, в котором работает измерительный показатель.</span><span class="sxs-lookup"><span data-stu-id="7dd07-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-588">Потребленная служба</span><span class="sxs-lookup"><span data-stu-id="7dd07-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="7dd07-589">Используемая служба платформы Azure.</span><span class="sxs-lookup"><span data-stu-id="7dd07-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="7dd07-590">URI ресурса</span><span class="sxs-lookup"><span data-stu-id="7dd07-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="7dd07-591">URI используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="7dd07-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-592">Тип оплаты</span><span class="sxs-lookup"><span data-stu-id="7dd07-592">Charge type</span></span></td>
<td><p><span data-ttu-id="7dd07-593">Тип оплаты или корректировки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-593">The type of charge or adjustment.</span></span> <span data-ttu-id="7dd07-594">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-595">Цена за единицу</span><span class="sxs-lookup"><span data-stu-id="7dd07-595">Unit price</span></span></td>
<td><p><span data-ttu-id="7dd07-596">Цена за лицензию, опубликованная в PriceList на момент приобретения.</span><span class="sxs-lookup"><span data-stu-id="7dd07-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="7dd07-597">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-598">Количество</span><span class="sxs-lookup"><span data-stu-id="7dd07-598">Quantity</span></span></td>
<td><p><span data-ttu-id="7dd07-599">Число лицензий.</span><span class="sxs-lookup"><span data-stu-id="7dd07-599">Number of licenses.</span></span> <span data-ttu-id="7dd07-600">Убедитесь, что она соответствует информации, хранящейся в вашей биллинговой системе во время выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-601">Тип единицы</span><span class="sxs-lookup"><span data-stu-id="7dd07-601">Unit type</span></span></td>
<td><p><span data-ttu-id="7dd07-602">Тип единицы измерения, за которую наследуется данный счетчик.</span><span class="sxs-lookup"><span data-stu-id="7dd07-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="7dd07-603">Недоступно для текущей активности.</span><span class="sxs-lookup"><span data-stu-id="7dd07-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-604">Выставление счетов за предварительный налог</span><span class="sxs-lookup"><span data-stu-id="7dd07-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="7dd07-605">Общая сумма перед налогами.</span><span class="sxs-lookup"><span data-stu-id="7dd07-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-606">Валюта выставления счетов</span><span class="sxs-lookup"><span data-stu-id="7dd07-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="7dd07-607">Валюта в географическом регионе клиента</span><span class="sxs-lookup"><span data-stu-id="7dd07-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-608">Общие сведения о ценах цена</span><span class="sxs-lookup"><span data-stu-id="7dd07-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="7dd07-609">Цены перед добавлением налогов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-610">Валюта цены</span><span class="sxs-lookup"><span data-stu-id="7dd07-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="7dd07-611">Валюта в PriceList.</span><span class="sxs-lookup"><span data-stu-id="7dd07-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-612">Сведения о службе 1</span><span class="sxs-lookup"><span data-stu-id="7dd07-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="7dd07-613">Количество подключений ServiceBus, подготовленных к работе и использованных в определенный день.</span><span class="sxs-lookup"><span data-stu-id="7dd07-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="7dd07-614">Сведения о службе 2</span><span class="sxs-lookup"><span data-stu-id="7dd07-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="7dd07-615">Устаревшее поле, которое фиксирует необязательные метаданные, относящиеся к службе.</span><span class="sxs-lookup"><span data-stu-id="7dd07-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="7dd07-616">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="7dd07-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="7dd07-617">Дополнительные сведения, не охваченные другими столбцами.</span><span class="sxs-lookup"><span data-stu-id="7dd07-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-618">еффективеунитприце</span><span class="sxs-lookup"><span data-stu-id="7dd07-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="7dd07-619">Фактическое значение, оплачиваемое за единицу (включая скидки, полученные баллы и т. д.).</span><span class="sxs-lookup"><span data-stu-id="7dd07-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-620">пктобцексчанжерате</span><span class="sxs-lookup"><span data-stu-id="7dd07-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="7dd07-621">Валютный курс, применяемый для валюты счета (Customers).</span><span class="sxs-lookup"><span data-stu-id="7dd07-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-622">пктобцексчанжератедате</span><span class="sxs-lookup"><span data-stu-id="7dd07-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="7dd07-623">Дата, с которой определяется Валюта валютного курса для валюты выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7dd07-624">ентитлементид</span><span class="sxs-lookup"><span data-stu-id="7dd07-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="7dd07-625">Представляет Azure subscriptionID.</span><span class="sxs-lookup"><span data-stu-id="7dd07-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7dd07-626">ентитлементдескриптион</span><span class="sxs-lookup"><span data-stu-id="7dd07-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="7dd07-627">Представляет имя подписки Azure.</span><span class="sxs-lookup"><span data-stu-id="7dd07-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="7dd07-628">Сопоставление расходов между счетом и файлом сверки</span><span class="sxs-lookup"><span data-stu-id="7dd07-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="7dd07-629">Ваш счет-фактура содержит сводку по расходам, а файл выверки включает подробную постатейную разбивку операций с указанием типов расходов.</span><span class="sxs-lookup"><span data-stu-id="7dd07-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="7dd07-630">Для добавления перекрестных ссылок на суммы расходов между счетом-фактурой и файлом выверки можно с помощью параметров фильтрования Microsoft Excel отфильтровать расходы по типам в файле выверки, чтобы сопоставить расходы по накладной с набором разбивок расходов в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="7dd07-631">Файлы выверки, как на основе лицензий, так и на основе использования, отражают только транзакции и расходы, связанные с использованием (израсходованные единицы и связанные с ними платежи).</span><span class="sxs-lookup"><span data-stu-id="7dd07-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="7dd07-632">Один из кредитов, скидок или денег, которые отображаются в счете как "корректировки", не отображаются в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="7dd07-633">В таблице ниже показаны сопоставления между разделом счета-фактуры и связанными типами расходов, которые могут отображаться в файлах выверки.</span><span class="sxs-lookup"><span data-stu-id="7dd07-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="7dd07-634"><strong>Описание оплаты по счету</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-635"><strong>Описание оплаты файлов сверки (столбец Чаржетипе)</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-636"><strong>Что это за это?</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-637"><strong>Разделы справки сопоставлять эти Чаржетипес с накладной?</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="7dd07-638"><strong>Оплата на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-639">Сбор за активацию</span><span class="sxs-lookup"><span data-stu-id="7dd07-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-640">Сумма, взимаемая с клиента при использовании подписки после ее приобретения</span><span class="sxs-lookup"><span data-stu-id="7dd07-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="7dd07-641">Получите сумму значений столбца <strong>Сумма</strong> в файле на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="7dd07-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-642">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="7dd07-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-643">Пропорциональные взносы, возвращаемые клиенту при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="7dd07-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-644">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="7dd07-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-645">Периодические взносы за подписку</span><span class="sxs-lookup"><span data-stu-id="7dd07-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-646">Пропорциональное распределение экземпляра цикла</span><span class="sxs-lookup"><span data-stu-id="7dd07-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-647">Пропорциональные взносы, начисленные от клиента при изменении связанных мест</span><span class="sxs-lookup"><span data-stu-id="7dd07-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-648">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="7dd07-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-649">Пропорциональный возврат денег за неиспользованную часть услуги после отмены</span><span class="sxs-lookup"><span data-stu-id="7dd07-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-650">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="7dd07-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-651">Тип оплаты для подписки при использовании годового счета</span><span class="sxs-lookup"><span data-stu-id="7dd07-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-652">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="7dd07-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-653">Тип оплаты для подписки при ежемесячном выставлении счетов</span><span class="sxs-lookup"><span data-stu-id="7dd07-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-654">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="7dd07-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-655">Пропорциональные сборы после возобновления действия подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="7dd07-656">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="7dd07-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-657">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-658">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="7dd07-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-659">Пропорциональные сборы с момента активации до конца периода выставления счетов</span><span class="sxs-lookup"><span data-stu-id="7dd07-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="7dd07-660"><strong>Оплата за один раз</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="7dd07-661">Новый</span><span class="sxs-lookup"><span data-stu-id="7dd07-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-662">Используется при создании новой покупки</span><span class="sxs-lookup"><span data-stu-id="7dd07-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="7dd07-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-664">Используется как для возврата первоначальной покупки, так и для нового количества после увеличения.</span><span class="sxs-lookup"><span data-stu-id="7dd07-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="7dd07-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-666">Используется как для возврата первоначальной покупки, так и для нового количества после уменьшения</span><span class="sxs-lookup"><span data-stu-id="7dd07-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-667">"Отмена"</span><span class="sxs-lookup"><span data-stu-id="7dd07-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-668">Используется при отмене подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-669">Преобразование</span><span class="sxs-lookup"><span data-stu-id="7dd07-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-670">Используется при обновлении лицензии, но число рабочих мест остается неизменным</span><span class="sxs-lookup"><span data-stu-id="7dd07-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="7dd07-671"><strong>Плата за использование</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-672">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="7dd07-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-673">Сбор за использование Access после отмены за неоплаченное использование за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="7dd07-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="7dd07-674">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="7dd07-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-675">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="7dd07-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-676">Сбор за использование Access за текущий период выставления счетов</span><span class="sxs-lookup"><span data-stu-id="7dd07-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="7dd07-677"><strong>Автор</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-678">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="7dd07-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-679">Частичный или полный возврат денег по позиции строки, включая налоги</span><span class="sxs-lookup"><span data-stu-id="7dd07-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-680">Получите сумму значений столбца <strong>TotalForCustomer</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="7dd07-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="7dd07-681">Получите сумму значений столбца <strong>PostTaxTotal</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="7dd07-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="7dd07-682"><strong>Скидки на основе использования</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-683">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="7dd07-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-684">Скидка, применяемая при активации подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="7dd07-685">Получите сумму значений столбца <strong>PretaxCharges</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="7dd07-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-686">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="7dd07-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-687">Скидка, применяемая к периодическим платежам</span><span class="sxs-lookup"><span data-stu-id="7dd07-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-688">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="7dd07-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-689">Скидка, применяемая при возобновлении подписки</span><span class="sxs-lookup"><span data-stu-id="7dd07-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-690">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="7dd07-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-691">Плата при отмене скидок</span><span class="sxs-lookup"><span data-stu-id="7dd07-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="7dd07-692"><strong>Скидки на основе лицензий</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-693"><em>Может применяться к нескольким типам оплаты</em></span><span class="sxs-lookup"><span data-stu-id="7dd07-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="7dd07-694">Получите сумму значений столбца <strong>TotalOtherDiscount</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="7dd07-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7dd07-695"><strong>Налоги</strong>&nbsp;или&nbsp;<strong>НДС</strong></span><span class="sxs-lookup"><span data-stu-id="7dd07-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-696"><em>Может применяться к нескольким типам оплаты</em></span><span class="sxs-lookup"><span data-stu-id="7dd07-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="7dd07-697"><em>Исключение: &quot;Offset элемент строки &quot; уже включает налоги. См. кредиты выше.</em></span><span class="sxs-lookup"><span data-stu-id="7dd07-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-698">Налоги и налоги на добавленную стоимость (НДС)</span><span class="sxs-lookup"><span data-stu-id="7dd07-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="7dd07-699">Получите сумму значений столбца <strong>Налог</strong> в файле по продуктам, оплачиваемым на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="7dd07-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="7dd07-700">Получите сумму значений столбца <strong>TaxAmount</strong> в файле по продуктам, оплачиваемым по объему использования</span><span class="sxs-lookup"><span data-stu-id="7dd07-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
