---
title: Использование файлов сверки
ms.topic: article
ms.date: 03/10/2021
description: Сведения о выверке-файлах в центре партнеров и о том, как интерпретировать подробные представления строкового элемента для данного цикла выставления счетов.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022780"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="0b176-103">Узнайте, как читать элементы строк в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="0b176-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="0b176-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="0b176-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0b176-105">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="0b176-105">Billing admin</span></span>
- <span data-ttu-id="0b176-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0b176-106">Global admin</span></span>

<span data-ttu-id="0b176-107">Вы можете скачать файлы сверки из центра партнеров, чтобы получить подробное представление каждого из элементов в цикле выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="0b176-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="0b176-108">Сведения об элементе строки включают оплату за каждую из подписок клиента и подробные события (например, Добавление лицензий в подписку).</span><span class="sxs-lookup"><span data-stu-id="0b176-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="0b176-109">Сведения о том, как прочитать **счет**, см. в разделе [Чтение](read-your-bill.md)счета.</span><span class="sxs-lookup"><span data-stu-id="0b176-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="0b176-110">Общие сведения о полях файла сверки</span><span class="sxs-lookup"><span data-stu-id="0b176-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="0b176-111">Поля сверочного файла на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="0b176-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="0b176-112">Поля сверочного файла на основе потребления</span><span class="sxs-lookup"><span data-stu-id="0b176-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="0b176-113">Поля сверочного файла потребления за сутки</span><span class="sxs-lookup"><span data-stu-id="0b176-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="0b176-114">Поля файла сверки CSP с одноразовой покупкой</span><span class="sxs-lookup"><span data-stu-id="0b176-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="0b176-115">Понимание типов оплаты в файлах выверки</span><span class="sxs-lookup"><span data-stu-id="0b176-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="0b176-116">Сведения о типах начислений в файлах выверки (столбец **чаржетипе** ) см. в разделе [типы оплаты за файл выверки](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="0b176-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="0b176-117">Устранение проблем форматирования</span><span class="sxs-lookup"><span data-stu-id="0b176-117">Fix formatting issues</span></span>

<span data-ttu-id="0b176-118">Иногда файл сверки может содержать проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="0b176-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="0b176-119">Например, эта проблема может возникать, если языковой стандарт EN-US не используется.</span><span class="sxs-lookup"><span data-stu-id="0b176-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="0b176-120">Чтобы устранить проблемы форматирования в файлах сверки, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="0b176-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="0b176-121">Откройте файл сверки (в формате CSV) в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="0b176-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="0b176-122">Выберите первый столбец в файле.</span><span class="sxs-lookup"><span data-stu-id="0b176-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="0b176-123">Откройте **Мастер преобразования текста в столбцы**.</span><span class="sxs-lookup"><span data-stu-id="0b176-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="0b176-124">На ленте выберите **данные**, а затем выберите **текст в столбцах**.</span><span class="sxs-lookup"><span data-stu-id="0b176-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="0b176-125">В мастере выберите **Тип файла с разделителями**.</span><span class="sxs-lookup"><span data-stu-id="0b176-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="0b176-126">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="0b176-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="0b176-127">В поле **разделители** выберите **запятая**.</span><span class="sxs-lookup"><span data-stu-id="0b176-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="0b176-128">(Если **вкладка** уже выбрана, можно оставить этот параметр установленным.) Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="0b176-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="0b176-129">В поле **Формат данных столбца** выберите **Date: mdy**.</span><span class="sxs-lookup"><span data-stu-id="0b176-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="0b176-130">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="0b176-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="0b176-131">В поле **Формат данных столбца** выберите **текст** для всех столбцов суммы.</span><span class="sxs-lookup"><span data-stu-id="0b176-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="0b176-132">Нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="0b176-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="0b176-133">Программное скачивание файлов выверки</span><span class="sxs-lookup"><span data-stu-id="0b176-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="0b176-134">Файлы сверки могут быть очень большими и иногда трудно скачивать.</span><span class="sxs-lookup"><span data-stu-id="0b176-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="0b176-135">Сведения об программной загрузке файлов выверки см. в разделе [Получение элементов строки счета](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="0b176-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="0b176-136">Сопоставьте налоги или НДС</span><span class="sxs-lookup"><span data-stu-id="0b176-136">Map taxes or VAT</span></span>

<span data-ttu-id="0b176-137">Чтобы сопоставлять налоги или налог на добавленные значения (VAT) к счету, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="0b176-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="0b176-138">Суммировать **налоговый** столбец из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="0b176-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="0b176-139">Вычислите сумму столбца **таксамаунт** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="0b176-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="0b176-140">Детализировать файлы сверки по партнерам</span><span class="sxs-lookup"><span data-stu-id="0b176-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="0b176-141">Партнеры в **косвенной модели** могут использовать эти дополнительные поля в файлах согласования на основе лицензий и на основе использования для перечисления файлов по торговому посреднику.</span><span class="sxs-lookup"><span data-stu-id="0b176-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="0b176-142">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="0b176-142">MPN ID</span></span> | <span data-ttu-id="0b176-143">Описание</span><span class="sxs-lookup"><span data-stu-id="0b176-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="0b176-144">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="0b176-144">MPN ID</span></span> | <span data-ttu-id="0b176-145">Идентификатор Microsoft Partner Network (MPN) для партнера поставщика облачных решений (CSP) (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="0b176-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="0b176-146">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="0b176-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="0b176-147">[Идентификатор MPN торгового посредника записи для подписки](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="0b176-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="0b176-148">Это поле соответствует ИДЕНТИФИКАТОРу торгового посредника, указанному для конкретной подписки в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="0b176-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="0b176-149">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="0b176-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="0b176-150">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="0b176-150">Reseller MPN ID</span></span>

<span data-ttu-id="0b176-151">Если партнер CSP продавал подписку непосредственно клиенту, его **идентификатор MPN** указывается дважды, как **идентификатор MPN** и **Идентификатор торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="0b176-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="0b176-152">Если у партнера CSP есть посредника, у которого нет **идентификатора MPN**, вместо него задается **идентификатор MPN** партнера.</span><span class="sxs-lookup"><span data-stu-id="0b176-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="0b176-153">Если партнер CSP удалит **MPN ID торгового посредника**, это значение будет равно *-1*.</span><span class="sxs-lookup"><span data-stu-id="0b176-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="0b176-154">Чтобы просмотреть или изменить **идентификатор MPN торгового посредника**:</span><span class="sxs-lookup"><span data-stu-id="0b176-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="0b176-155">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="0b176-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="0b176-156">В меню Центра партнеров выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="0b176-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="0b176-157">Выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="0b176-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="0b176-158">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="0b176-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="0b176-159">Выберите подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="0b176-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="0b176-160">Выберите **обновить**, чтобы изменить пункт **Торговый посредник (идентификатор MPN)**.</span><span class="sxs-lookup"><span data-stu-id="0b176-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0b176-161">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="0b176-161">Next steps</span></span>

- [<span data-ttu-id="0b176-162">Как прочитать файл счета & разведывательную</span><span class="sxs-lookup"><span data-stu-id="0b176-162">How to read your bill & recon file</span></span>](read-your-bill.md) 