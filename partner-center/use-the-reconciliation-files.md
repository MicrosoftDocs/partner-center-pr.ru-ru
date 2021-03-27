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
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633902"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="feb5c-103">Узнайте, как читать элементы строк в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="feb5c-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="feb5c-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="feb5c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="feb5c-105">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="feb5c-105">Billing admin</span></span>
- <span data-ttu-id="feb5c-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="feb5c-106">Global admin</span></span>

<span data-ttu-id="feb5c-107">Вы можете скачать файлы сверки из центра партнеров, чтобы получить подробное представление каждого из элементов в цикле выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="feb5c-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="feb5c-108">Сведения об элементе строки включают оплату за каждую из подписок клиента и подробные события (например, Добавление лицензий в подписку).</span><span class="sxs-lookup"><span data-stu-id="feb5c-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="feb5c-109">Сведения о том, как прочитать **счет**, см. в разделе [Чтение](read-your-bill.md)счета.</span><span class="sxs-lookup"><span data-stu-id="feb5c-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="feb5c-110">Общие сведения о полях файла сверки</span><span class="sxs-lookup"><span data-stu-id="feb5c-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="feb5c-111">Поля сверочного файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="feb5c-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="feb5c-112">Поля сверочного файла на основе потребления</span><span class="sxs-lookup"><span data-stu-id="feb5c-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="feb5c-113">Поля сверочного файла потребления за сутки</span><span class="sxs-lookup"><span data-stu-id="feb5c-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="feb5c-114">Поля файла сверки CSP с одноразовой покупкой</span><span class="sxs-lookup"><span data-stu-id="feb5c-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="feb5c-115">Понимание типов оплаты в файлах выверки</span><span class="sxs-lookup"><span data-stu-id="feb5c-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="feb5c-116">Сведения о типах начислений в файлах выверки (столбец **чаржетипе** ) см. в разделе [типы оплаты за файл выверки](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="feb5c-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="feb5c-117">Устранение проблем форматирования</span><span class="sxs-lookup"><span data-stu-id="feb5c-117">Fix formatting issues</span></span>

<span data-ttu-id="feb5c-118">Иногда файл сверки может содержать проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="feb5c-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="feb5c-119">Например, эта проблема может возникать, если языковой стандарт EN-US не используется.</span><span class="sxs-lookup"><span data-stu-id="feb5c-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="feb5c-120">Чтобы устранить проблемы форматирования в файлах сверки, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="feb5c-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="feb5c-121">Откройте файл сверки (в формате CSV) в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="feb5c-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="feb5c-122">Выберите первый столбец в файле.</span><span class="sxs-lookup"><span data-stu-id="feb5c-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="feb5c-123">Откройте **Мастер преобразования текста в столбцы**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="feb5c-124">На ленте выберите **данные**, а затем выберите **текст в столбцах**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="feb5c-125">В мастере выберите **Тип файла с разделителями**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="feb5c-126">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="feb5c-127">В поле **разделители** выберите **запятая**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="feb5c-128">(Если **вкладка** уже выбрана, можно оставить этот параметр установленным.) Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="feb5c-129">В поле **Формат данных столбца** выберите **Date: mdy**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="feb5c-130">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="feb5c-131">В поле **Формат данных столбца** выберите **текст** для всех столбцов суммы.</span><span class="sxs-lookup"><span data-stu-id="feb5c-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="feb5c-132">Нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="feb5c-133">Программное скачивание файлов выверки</span><span class="sxs-lookup"><span data-stu-id="feb5c-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="feb5c-134">Файлы сверки могут быть очень большими и иногда трудно скачивать.</span><span class="sxs-lookup"><span data-stu-id="feb5c-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="feb5c-135">Сведения об программной загрузке файлов выверки см. в разделе [Получение элементов строки счета](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="feb5c-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="feb5c-136">Если размер файла превышает ограничение по строкам в Excel</span><span class="sxs-lookup"><span data-stu-id="feb5c-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="feb5c-137">Если вы можете скачать файл сверки, но не открыть его в Microsoft Excel, вероятно, это означает, что файл содержит больше строк, чем позволяет Excel.</span><span class="sxs-lookup"><span data-stu-id="feb5c-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="feb5c-138">В этом случае для открытия файла можно использовать любую из приведенных ниже процедур.</span><span class="sxs-lookup"><span data-stu-id="feb5c-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="feb5c-139">Откройте файл разведывательную в Power BI</span><span class="sxs-lookup"><span data-stu-id="feb5c-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="feb5c-140">Загрузите файл сверки обычным образом.</span><span class="sxs-lookup"><span data-stu-id="feb5c-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="feb5c-141">Скачайте, установите и откройте экземпляр Power BI.</span><span class="sxs-lookup"><span data-stu-id="feb5c-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="feb5c-142">На вкладке Power BI **Главная** выберите **получить данные**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="feb5c-143">В списке **общих источников данных** выберите **Text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="feb5c-144">При появлении запроса откройте файл разведывательную.</span><span class="sxs-lookup"><span data-stu-id="feb5c-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="feb5c-145">Открытие файла разведывательную в сводной таблице Excel</span><span class="sxs-lookup"><span data-stu-id="feb5c-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="feb5c-146">Загрузите файл сверки обычным образом.</span><span class="sxs-lookup"><span data-stu-id="feb5c-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="feb5c-147">Откройте новый файл в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="feb5c-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="feb5c-148">На вкладке **данные** выберите **получить данные**, выберите **из файла**, а затем выберите **текстовый/CSV**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="feb5c-149">При появлении запроса откройте файл разведывательную.</span><span class="sxs-lookup"><span data-stu-id="feb5c-149">When prompted, open your recon file.</span></span> <span data-ttu-id="feb5c-150">Ваши данные будут отображаться.</span><span class="sxs-lookup"><span data-stu-id="feb5c-150">Your data will appear.</span></span>
5. <span data-ttu-id="feb5c-151">В раскрывающемся меню **Загрузка** выберите пункт **загрузить в** и нажмите **кнопку ОК**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="feb5c-152">В диалоговом окне **Импорт данных** выберите **отчет сводной таблицы** , чтобы открыть файл.</span><span class="sxs-lookup"><span data-stu-id="feb5c-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="feb5c-153">Сопоставьте налоги или НДС</span><span class="sxs-lookup"><span data-stu-id="feb5c-153">Map taxes or VAT</span></span>

<span data-ttu-id="feb5c-154">Чтобы сопоставлять налоги или налог на добавленные значения (VAT) к счету, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="feb5c-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="feb5c-155">Суммировать **налоговый** столбец из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="feb5c-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="feb5c-156">Вычислите сумму столбца **таксамаунт** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="feb5c-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="feb5c-157">Детализировать файлы сверки по партнерам</span><span class="sxs-lookup"><span data-stu-id="feb5c-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="feb5c-158">Партнеры в **косвенной модели** могут использовать эти дополнительные поля в файлах согласования на основе лицензий и на основе использования для перечисления файлов по торговому посреднику.</span><span class="sxs-lookup"><span data-stu-id="feb5c-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="feb5c-159">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="feb5c-159">MPN ID</span></span> | <span data-ttu-id="feb5c-160">Описание</span><span class="sxs-lookup"><span data-stu-id="feb5c-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="feb5c-161">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="feb5c-161">MPN ID</span></span> | <span data-ttu-id="feb5c-162">Идентификатор Microsoft Partner Network (MPN) для партнера поставщика облачных решений (CSP) (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="feb5c-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="feb5c-163">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="feb5c-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="feb5c-164">[Идентификатор MPN торгового посредника записи для подписки](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="feb5c-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="feb5c-165">Это поле соответствует ИДЕНТИФИКАТОРу торгового посредника, указанному для конкретной подписки в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="feb5c-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="feb5c-166">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="feb5c-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="feb5c-167">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="feb5c-167">Reseller MPN ID</span></span>

<span data-ttu-id="feb5c-168">Если партнер CSP продавал подписку непосредственно клиенту, его **идентификатор MPN** указывается дважды, как **идентификатор MPN** и **Идентификатор торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="feb5c-169">Если у партнера CSP есть посредника, у которого нет **идентификатора MPN**, вместо него задается **идентификатор MPN** партнера.</span><span class="sxs-lookup"><span data-stu-id="feb5c-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="feb5c-170">Если партнер CSP удалит **MPN ID торгового посредника**, это значение будет равно *-1*.</span><span class="sxs-lookup"><span data-stu-id="feb5c-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="feb5c-171">Чтобы просмотреть или изменить **идентификатор MPN торгового посредника**:</span><span class="sxs-lookup"><span data-stu-id="feb5c-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="feb5c-172">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="feb5c-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="feb5c-173">В меню Центра партнеров выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="feb5c-174">Выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="feb5c-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="feb5c-175">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="feb5c-176">Выберите подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="feb5c-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="feb5c-177">Выберите **обновить**, чтобы изменить пункт **Торговый посредник (идентификатор MPN)**.</span><span class="sxs-lookup"><span data-stu-id="feb5c-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="feb5c-178">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="feb5c-178">Next steps</span></span>

- [<span data-ttu-id="feb5c-179">Как прочитать файл счета & разведывательную</span><span class="sxs-lookup"><span data-stu-id="feb5c-179">How to read your bill & recon file</span></span>](read-your-bill.md) 