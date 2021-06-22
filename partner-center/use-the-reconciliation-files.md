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
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431574"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="ba262-103">Узнайте, как читать элементы строк в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="ba262-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="ba262-104">**Соответствующие роли**: администратор выставления счетов | Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ba262-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="ba262-105">Вы можете скачать файлы сверки из центра партнеров, чтобы получить подробное представление каждого из элементов в цикле выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ba262-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="ba262-106">Сведения об элементе строки включают оплату за каждую из подписок клиента и подробные события (например, Добавление лицензий в подписку).</span><span class="sxs-lookup"><span data-stu-id="ba262-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="ba262-107">Сведения о том, как прочитать **счет**, см. в разделе [Чтение](read-your-bill.md)счета.</span><span class="sxs-lookup"><span data-stu-id="ba262-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="ba262-108">Общие сведения о полях файла сверки</span><span class="sxs-lookup"><span data-stu-id="ba262-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="ba262-109">Поля сверочного файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="ba262-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="ba262-110">Поля сверочного файла на основе потребления</span><span class="sxs-lookup"><span data-stu-id="ba262-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="ba262-111">Поля сверочного файла потребления за сутки</span><span class="sxs-lookup"><span data-stu-id="ba262-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="ba262-112">Поля файла сверки CSP с одноразовой покупкой</span><span class="sxs-lookup"><span data-stu-id="ba262-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="ba262-113">Понимание типов оплаты в файлах выверки</span><span class="sxs-lookup"><span data-stu-id="ba262-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="ba262-114">Сведения о типах начислений в файлах выверки (столбец **чаржетипе** ) см. в разделе [типы оплаты за файл выверки](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="ba262-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="ba262-115">Устранение проблем форматирования</span><span class="sxs-lookup"><span data-stu-id="ba262-115">Fix formatting issues</span></span>

<span data-ttu-id="ba262-116">Иногда файл сверки может содержать проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="ba262-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="ba262-117">Например, эта проблема может возникать, если языковой стандарт EN-US не используется.</span><span class="sxs-lookup"><span data-stu-id="ba262-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="ba262-118">Чтобы устранить проблемы форматирования в файлах сверки, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="ba262-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="ba262-119">Откройте файл сверки (в формате .csv) в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="ba262-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="ba262-120">Выберите первый столбец в файле.</span><span class="sxs-lookup"><span data-stu-id="ba262-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="ba262-121">Откройте **Мастер преобразования текста в столбцы**.</span><span class="sxs-lookup"><span data-stu-id="ba262-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="ba262-122">На ленте выберите **данные**, а затем выберите **текст в столбцах**.</span><span class="sxs-lookup"><span data-stu-id="ba262-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="ba262-123">В мастере выберите **Тип файла с разделителями**.</span><span class="sxs-lookup"><span data-stu-id="ba262-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="ba262-124">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="ba262-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="ba262-125">В поле **разделители** выберите **запятая**.</span><span class="sxs-lookup"><span data-stu-id="ba262-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="ba262-126">(Если **вкладка** уже выбрана, можно оставить этот параметр установленным.) Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="ba262-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="ba262-127">В поле **Формат данных столбца** выберите **Date: mdy**.</span><span class="sxs-lookup"><span data-stu-id="ba262-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="ba262-128">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="ba262-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="ba262-129">В поле **Формат данных столбца** выберите **текст** для всех столбцов суммы.</span><span class="sxs-lookup"><span data-stu-id="ba262-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="ba262-130">Нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="ba262-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="ba262-131">Программное скачивание файлов выверки</span><span class="sxs-lookup"><span data-stu-id="ba262-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="ba262-132">Файлы сверки могут быть очень большими и иногда трудно скачивать.</span><span class="sxs-lookup"><span data-stu-id="ba262-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="ba262-133">Сведения об программной загрузке файлов выверки см. в разделе [Получение элементов строки счета](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="ba262-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="ba262-134">Если размер файла превышает ограничение по строкам в Excel</span><span class="sxs-lookup"><span data-stu-id="ba262-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="ba262-135">Если вы можете скачать файл сверки, но не открыть его в Microsoft Excel, вероятно, это означает, что файл содержит больше строк, чем позволяет Excel.</span><span class="sxs-lookup"><span data-stu-id="ba262-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="ba262-136">В этом случае для открытия файла можно использовать любую из приведенных ниже процедур.</span><span class="sxs-lookup"><span data-stu-id="ba262-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="ba262-137">Откройте файл разведывательную в Power BI</span><span class="sxs-lookup"><span data-stu-id="ba262-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="ba262-138">Загрузите файл сверки обычным образом.</span><span class="sxs-lookup"><span data-stu-id="ba262-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="ba262-139">Скачайте, установите и откройте экземпляр Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="ba262-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="ba262-140">На вкладке Power BI **Главная** выберите **получить данные**.</span><span class="sxs-lookup"><span data-stu-id="ba262-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="ba262-141">В списке **общих источников данных** выберите **Text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="ba262-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="ba262-142">При появлении запроса откройте файл разведывательную.</span><span class="sxs-lookup"><span data-stu-id="ba262-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="ba262-143">Открытие файла разведывательную в сводной таблице Excel</span><span class="sxs-lookup"><span data-stu-id="ba262-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="ba262-144">Загрузите файл сверки обычным образом.</span><span class="sxs-lookup"><span data-stu-id="ba262-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="ba262-145">Откройте новый файл в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="ba262-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="ba262-146">На вкладке **данные** выберите **получить данные**, выберите **из файла**, а затем выберите **текстовый/CSV**.</span><span class="sxs-lookup"><span data-stu-id="ba262-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="ba262-147">При появлении запроса откройте файл разведывательную.</span><span class="sxs-lookup"><span data-stu-id="ba262-147">When prompted, open your recon file.</span></span> <span data-ttu-id="ba262-148">Ваши данные будут отображаться.</span><span class="sxs-lookup"><span data-stu-id="ba262-148">Your data will appear.</span></span>
5. <span data-ttu-id="ba262-149">В раскрывающемся меню **Загрузка** выберите пункт **загрузить в** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ba262-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="ba262-150">В диалоговом окне **Импорт данных** выберите **отчет сводной таблицы** , чтобы открыть файл.</span><span class="sxs-lookup"><span data-stu-id="ba262-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="ba262-151">Отображается отрицательная сумма</span><span class="sxs-lookup"><span data-stu-id="ba262-151">Negative amount displayed</span></span>

<span data-ttu-id="ba262-152">В файле сверки может отобразиться отрицательная сумма.</span><span class="sxs-lookup"><span data-stu-id="ba262-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="ba262-153">Возможно, эта проблема вызвана одной из следующих причин:</span><span class="sxs-lookup"><span data-stu-id="ba262-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="ba262-154">Вы недавно отменили или уменьшили число лицензий</span><span class="sxs-lookup"><span data-stu-id="ba262-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="ba262-155">Вы получили кредит для соглашения об уровне обслуживания (SLA) или для использования Azure</span><span class="sxs-lookup"><span data-stu-id="ba262-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="ba262-156">Чтобы получить дополнительные сведения об этой транзакции, проверьте атрибут типа оплаты в сверочном файле.</span><span class="sxs-lookup"><span data-stu-id="ba262-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="ba262-157">Сопоставьте налоги или НДС</span><span class="sxs-lookup"><span data-stu-id="ba262-157">Map taxes or VAT</span></span>

<span data-ttu-id="ba262-158">Чтобы сопоставлять налоги или налог на добавленные значения (VAT) к счету, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="ba262-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="ba262-159">Суммировать **налоговый** столбец из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="ba262-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="ba262-160">Вычислите сумму столбца **таксамаунт** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="ba262-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="ba262-161">Детализировать файлы сверки по партнерам</span><span class="sxs-lookup"><span data-stu-id="ba262-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="ba262-162">Партнеры в **косвенной модели** могут использовать эти дополнительные поля в файлах согласования на основе лицензий и на основе использования для перечисления файлов по торговому посреднику.</span><span class="sxs-lookup"><span data-stu-id="ba262-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="ba262-163">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="ba262-163">MPN ID</span></span> | <span data-ttu-id="ba262-164">Описание</span><span class="sxs-lookup"><span data-stu-id="ba262-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="ba262-165">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="ba262-165">MPN ID</span></span> | <span data-ttu-id="ba262-166">Идентификатор Microsoft Partner Network (MPN) для партнера поставщика облачных решений (CSP) (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="ba262-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="ba262-167">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="ba262-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="ba262-168">[Идентификатор MPN торгового посредника записи для подписки](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="ba262-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="ba262-169">Это поле соответствует ИДЕНТИФИКАТОРу торгового посредника, указанному для конкретной подписки в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ba262-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="ba262-170">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="ba262-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="ba262-171">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="ba262-171">Reseller MPN ID</span></span>

<span data-ttu-id="ba262-172">Если партнер CSP продавал подписку непосредственно клиенту, его **идентификатор MPN** указывается дважды, как **идентификатор MPN** и **Идентификатор торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="ba262-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="ba262-173">Если у партнера CSP есть посредника, у которого нет **идентификатора MPN**, вместо него задается **идентификатор MPN** партнера.</span><span class="sxs-lookup"><span data-stu-id="ba262-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="ba262-174">Если партнер CSP удалит **MPN ID торгового посредника**, это значение будет равно *-1*.</span><span class="sxs-lookup"><span data-stu-id="ba262-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="ba262-175">Чтобы просмотреть или изменить **идентификатор MPN торгового посредника**:</span><span class="sxs-lookup"><span data-stu-id="ba262-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="ba262-176">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="ba262-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="ba262-177">В меню Центра партнеров выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="ba262-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="ba262-178">Выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ba262-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="ba262-179">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="ba262-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="ba262-180">Выберите подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="ba262-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="ba262-181">Выберите **обновить**, чтобы изменить пункт **Торговый посредник (идентификатор MPN)**.</span><span class="sxs-lookup"><span data-stu-id="ba262-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba262-182">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="ba262-182">Next steps</span></span>

- [<span data-ttu-id="ba262-183">Как прочитать файл счета & разведывательную</span><span class="sxs-lookup"><span data-stu-id="ba262-183">How to read your bill & recon file</span></span>](read-your-bill.md) 