---
title: Использование файлов сверки
ms.topic: article
ms.date: 03/26/2021
description: Сведения о выверке-файлах в центре партнеров и о том, как интерпретировать подробные представления строкового элемента для данного цикла выставления счетов.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730094"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="3a9ff-103">Узнайте, как читать элементы строк в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="3a9ff-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="3a9ff-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="3a9ff-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3a9ff-105">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="3a9ff-105">Billing admin</span></span>
- <span data-ttu-id="3a9ff-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3a9ff-106">Global admin</span></span>

<span data-ttu-id="3a9ff-107">Вы можете скачать файлы сверки из центра партнеров, чтобы получить подробное представление каждого из элементов в цикле выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="3a9ff-108">Сведения об элементе строки включают оплату за каждую из подписок клиента и подробные события (например, Добавление лицензий в подписку).</span><span class="sxs-lookup"><span data-stu-id="3a9ff-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="3a9ff-109">Сведения о том, как прочитать **счет**, см. в разделе [Чтение](read-your-bill.md)счета.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="3a9ff-110">Общие сведения о полях файла сверки</span><span class="sxs-lookup"><span data-stu-id="3a9ff-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="3a9ff-111">Поля сверочного файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="3a9ff-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="3a9ff-112">Поля сверочного файла на основе потребления</span><span class="sxs-lookup"><span data-stu-id="3a9ff-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="3a9ff-113">Поля сверочного файла потребления за сутки</span><span class="sxs-lookup"><span data-stu-id="3a9ff-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="3a9ff-114">Поля файла сверки CSP с одноразовой покупкой</span><span class="sxs-lookup"><span data-stu-id="3a9ff-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="3a9ff-115">Понимание типов оплаты в файлах выверки</span><span class="sxs-lookup"><span data-stu-id="3a9ff-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="3a9ff-116">Сведения о типах начислений в файлах выверки (столбец **чаржетипе** ) см. в разделе [типы оплаты за файл выверки](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ff-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="3a9ff-117">Устранение проблем форматирования</span><span class="sxs-lookup"><span data-stu-id="3a9ff-117">Fix formatting issues</span></span>

<span data-ttu-id="3a9ff-118">Иногда файл сверки может содержать проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="3a9ff-119">Например, эта проблема может возникать, если языковой стандарт EN-US не используется.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="3a9ff-120">Чтобы устранить проблемы форматирования в файлах сверки, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="3a9ff-121">Откройте файл сверки (в формате CSV) в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="3a9ff-122">Выберите первый столбец в файле.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="3a9ff-123">Откройте **Мастер преобразования текста в столбцы**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="3a9ff-124">На ленте выберите **данные**, а затем выберите **текст в столбцах**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="3a9ff-125">В мастере выберите **Тип файла с разделителями**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="3a9ff-126">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="3a9ff-127">В поле **разделители** выберите **запятая**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="3a9ff-128">(Если **вкладка** уже выбрана, можно оставить этот параметр установленным.) Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="3a9ff-129">В поле **Формат данных столбца** выберите **Date: mdy**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="3a9ff-130">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="3a9ff-131">В поле **Формат данных столбца** выберите **текст** для всех столбцов суммы.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="3a9ff-132">Нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="3a9ff-133">Программное скачивание файлов выверки</span><span class="sxs-lookup"><span data-stu-id="3a9ff-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="3a9ff-134">Файлы сверки могут быть очень большими и иногда трудно скачивать.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="3a9ff-135">Сведения об программной загрузке файлов выверки см. в разделе [Получение элементов строки счета](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="3a9ff-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="3a9ff-136">Если размер файла превышает ограничение по строкам в Excel</span><span class="sxs-lookup"><span data-stu-id="3a9ff-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="3a9ff-137">Если вы можете скачать файл сверки, но не открыть его в Microsoft Excel, вероятно, это означает, что файл содержит больше строк, чем позволяет Excel.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="3a9ff-138">В этом случае для открытия файла можно использовать любую из приведенных ниже процедур.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="3a9ff-139">Откройте файл разведывательную в Power BI</span><span class="sxs-lookup"><span data-stu-id="3a9ff-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="3a9ff-140">Загрузите файл сверки обычным образом.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="3a9ff-141">Скачайте, установите и откройте экземпляр Power BI.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="3a9ff-142">На вкладке Power BI **Главная** выберите **получить данные**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="3a9ff-143">В списке **общих источников данных** выберите **Text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="3a9ff-144">При появлении запроса откройте файл разведывательную.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="3a9ff-145">Открытие файла разведывательную в сводной таблице Excel</span><span class="sxs-lookup"><span data-stu-id="3a9ff-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="3a9ff-146">Загрузите файл сверки обычным образом.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="3a9ff-147">Откройте новый файл в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="3a9ff-148">На вкладке **данные** выберите **получить данные**, выберите **из файла**, а затем выберите **текстовый/CSV**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="3a9ff-149">При появлении запроса откройте файл разведывательную.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-149">When prompted, open your recon file.</span></span> <span data-ttu-id="3a9ff-150">Ваши данные будут отображаться.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-150">Your data will appear.</span></span>
5. <span data-ttu-id="3a9ff-151">В раскрывающемся меню **Загрузка** выберите пункт **загрузить в** и нажмите **кнопку ОК**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="3a9ff-152">В диалоговом окне **Импорт данных** выберите **отчет сводной таблицы** , чтобы открыть файл.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="3a9ff-153">Отображается отрицательная сумма</span><span class="sxs-lookup"><span data-stu-id="3a9ff-153">Negative amount displayed</span></span>

<span data-ttu-id="3a9ff-154">В файле сверки может отобразиться отрицательная сумма.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-154">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="3a9ff-155">Возможно, это вызвано одной из следующих причин:</span><span class="sxs-lookup"><span data-stu-id="3a9ff-155">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="3a9ff-156">Вы недавно отменили или уменьшили число лицензий</span><span class="sxs-lookup"><span data-stu-id="3a9ff-156">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="3a9ff-157">Вы получили кредит для соглашения об уровне обслуживания (SLA) или для использования Azure</span><span class="sxs-lookup"><span data-stu-id="3a9ff-157">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="3a9ff-158">Чтобы получить дополнительные сведения об этой транзакции, проверьте атрибут типа оплаты в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-158">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="3a9ff-159">Сопоставьте налоги или НДС</span><span class="sxs-lookup"><span data-stu-id="3a9ff-159">Map taxes or VAT</span></span>

<span data-ttu-id="3a9ff-160">Чтобы сопоставлять налоги или налог на добавленные значения (VAT) к счету, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-160">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="3a9ff-161">Суммировать **налоговый** столбец из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-161">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="3a9ff-162">Вычислите сумму столбца **таксамаунт** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-162">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="3a9ff-163">Детализировать файлы сверки по партнерам</span><span class="sxs-lookup"><span data-stu-id="3a9ff-163">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="3a9ff-164">Партнеры в **косвенной модели** могут использовать эти дополнительные поля в файлах согласования на основе лицензий и на основе использования для перечисления файлов по торговому посреднику.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-164">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="3a9ff-165">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="3a9ff-165">MPN ID</span></span> | <span data-ttu-id="3a9ff-166">Описание</span><span class="sxs-lookup"><span data-stu-id="3a9ff-166">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="3a9ff-167">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="3a9ff-167">MPN ID</span></span> | <span data-ttu-id="3a9ff-168">Идентификатор Microsoft Partner Network (MPN) для партнера поставщика облачных решений (CSP) (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="3a9ff-168">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="3a9ff-169">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="3a9ff-169">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="3a9ff-170">[Идентификатор MPN торгового посредника записи для подписки](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="3a9ff-170">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="3a9ff-171">Это поле соответствует ИДЕНТИФИКАТОРу торгового посредника, указанному для конкретной подписки в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-171">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="3a9ff-172">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-172">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="3a9ff-173">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="3a9ff-173">Reseller MPN ID</span></span>

<span data-ttu-id="3a9ff-174">Если партнер CSP продавал подписку непосредственно клиенту, его **идентификатор MPN** указывается дважды, как **идентификатор MPN** и **Идентификатор торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-174">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="3a9ff-175">Если у партнера CSP есть посредника, у которого нет **идентификатора MPN**, вместо него задается **идентификатор MPN** партнера.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-175">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="3a9ff-176">Если партнер CSP удалит **MPN ID торгового посредника**, это значение будет равно *-1*.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-176">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="3a9ff-177">Чтобы просмотреть или изменить **идентификатор MPN торгового посредника**:</span><span class="sxs-lookup"><span data-stu-id="3a9ff-177">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="3a9ff-178">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-178">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="3a9ff-179">В меню Центра партнеров выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-179">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="3a9ff-180">Выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-180">Choose the customer from the list.</span></span>
4. <span data-ttu-id="3a9ff-181">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-181">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="3a9ff-182">Выберите подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-182">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="3a9ff-183">Выберите **обновить**, чтобы изменить пункт **Торговый посредник (идентификатор MPN)**.</span><span class="sxs-lookup"><span data-stu-id="3a9ff-183">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3a9ff-184">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3a9ff-184">Next steps</span></span>

- [<span data-ttu-id="3a9ff-185">Как прочитать файл счета & разведывательную</span><span class="sxs-lookup"><span data-stu-id="3a9ff-185">How to read your bill & recon file</span></span>](read-your-bill.md) 