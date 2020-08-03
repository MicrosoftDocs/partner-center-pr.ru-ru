---
title: Использование файлов сверки
ms.topic: article
ms.date: 06/08/2020
description: Сведения о выверке-файлах в центре партнеров и о том, как интерпретировать подробные представления строкового элемента для данного цикла выставления счетов.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05939dc5edaddeb2f74b3b75017e2062dff25e31
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468335"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="3186e-103">Узнайте, как читать элементы строк в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="3186e-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="3186e-104">Область применения:</span><span class="sxs-lookup"><span data-stu-id="3186e-104">Applies to:</span></span>

- <span data-ttu-id="3186e-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="3186e-105">Partner Center</span></span>
- <span data-ttu-id="3186e-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="3186e-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="3186e-107">Вы можете скачать файлы сверки из центра партнеров, чтобы получить подробное представление каждого из элементов в цикле выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="3186e-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="3186e-108">Сведения об элементе строки включают оплату за каждую из подписок клиента и подробные события (например, Добавление лицензий в подписку).</span><span class="sxs-lookup"><span data-stu-id="3186e-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="3186e-109">Соответствующие роли:</span><span class="sxs-lookup"><span data-stu-id="3186e-109">Appropriate roles:</span></span>

- <span data-ttu-id="3186e-110">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="3186e-110">Billing admin</span></span>
- <span data-ttu-id="3186e-111">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3186e-111">Global admin</span></span>

<span data-ttu-id="3186e-112">Сведения о том, как прочитать **счет**, см. в разделе [Чтение](read-your-bill.md)счета.</span><span class="sxs-lookup"><span data-stu-id="3186e-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="3186e-113">Общие сведения о полях файла сверки</span><span class="sxs-lookup"><span data-stu-id="3186e-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="3186e-114">Поля файла сверки на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="3186e-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="3186e-115">Поля файла сверки с учетом использования</span><span class="sxs-lookup"><span data-stu-id="3186e-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="3186e-116">Поля файла сверки с оценкой использования по дням</span><span class="sxs-lookup"><span data-stu-id="3186e-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="3186e-117">Понимание типов оплаты в файлах выверки</span><span class="sxs-lookup"><span data-stu-id="3186e-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="3186e-118">Сведения о типах начислений в файлах выверки (столбец **чаржетипе** ) см. в разделе [типы оплаты за файл выверки](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="3186e-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="3186e-119">Устранение проблем форматирования</span><span class="sxs-lookup"><span data-stu-id="3186e-119">Fix formatting issues</span></span>

<span data-ttu-id="3186e-120">Иногда файл сверки может содержать проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="3186e-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="3186e-121">Например, эта проблема может возникать, если языковой стандарт EN-US не используется.</span><span class="sxs-lookup"><span data-stu-id="3186e-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="3186e-122">Чтобы устранить проблемы форматирования в файлах сверки, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="3186e-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="3186e-123">Откройте файл сверки (в формате CSV) в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="3186e-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="3186e-124">Выберите первый столбец в файле.</span><span class="sxs-lookup"><span data-stu-id="3186e-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="3186e-125">Откройте **Мастер преобразования текста в столбцы**.</span><span class="sxs-lookup"><span data-stu-id="3186e-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="3186e-126">На ленте выберите **данные**, а затем выберите **текст в столбцах**.</span><span class="sxs-lookup"><span data-stu-id="3186e-126">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="3186e-127">В мастере выберите **Тип файла с разделителями**.</span><span class="sxs-lookup"><span data-stu-id="3186e-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="3186e-128">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="3186e-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="3186e-129">В поле **разделители** выберите **запятая**.</span><span class="sxs-lookup"><span data-stu-id="3186e-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="3186e-130">(Если **вкладка** уже выбрана, можно оставить этот параметр установленным.) Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="3186e-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="3186e-131">В поле **Формат данных столбца** выберите **Date: mdy**.</span><span class="sxs-lookup"><span data-stu-id="3186e-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="3186e-132">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="3186e-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="3186e-133">В поле **Формат данных столбца** выберите **текст** для всех столбцов суммы.</span><span class="sxs-lookup"><span data-stu-id="3186e-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="3186e-134">Щелкните **Готово**.</span><span class="sxs-lookup"><span data-stu-id="3186e-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="3186e-135">Программное скачивание файлов выверки</span><span class="sxs-lookup"><span data-stu-id="3186e-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="3186e-136">Файлы сверки могут быть очень большими и иногда трудно скачивать.</span><span class="sxs-lookup"><span data-stu-id="3186e-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="3186e-137">Сведения об программной загрузке файлов выверки см. в разделе [Получение элементов строки счета](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="3186e-137">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="3186e-138">Сопоставьте налоги или НДС</span><span class="sxs-lookup"><span data-stu-id="3186e-138">Map taxes or VAT</span></span>

<span data-ttu-id="3186e-139">Чтобы сопоставлять налоги или налог на добавленные значения (VAT) к счету, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="3186e-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="3186e-140">Суммировать **налоговый** столбец из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="3186e-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="3186e-141">Вычислите сумму столбца **таксамаунт** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="3186e-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="3186e-142">Детализировать файлы сверки по партнерам</span><span class="sxs-lookup"><span data-stu-id="3186e-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="3186e-143">Партнеры в **косвенной модели** могут использовать эти дополнительные поля в файлах согласования на основе лицензий и на основе использования для перечисления файлов по торговому посреднику.</span><span class="sxs-lookup"><span data-stu-id="3186e-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="3186e-144">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="3186e-144">MPN ID</span></span> | <span data-ttu-id="3186e-145">Описание</span><span class="sxs-lookup"><span data-stu-id="3186e-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="3186e-146">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="3186e-146">MPN ID</span></span> | <span data-ttu-id="3186e-147">Идентификатор Microsoft Partner Network (MPN) для партнера поставщика облачных решений (CSP) (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="3186e-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="3186e-148">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="3186e-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="3186e-149">[Идентификатор MPN торгового посредника записи для подписки](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="3186e-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="3186e-150">Это поле соответствует ИДЕНТИФИКАТОРу торгового посредника, указанному для конкретной подписки в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="3186e-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="3186e-151">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="3186e-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="3186e-152">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="3186e-152">Reseller MPN ID</span></span>

<span data-ttu-id="3186e-153">Если партнер CSP продавал подписку непосредственно клиенту, его **идентификатор MPN** указывается дважды, как **идентификатор MPN** и **Идентификатор торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="3186e-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="3186e-154">Если у партнера CSP есть посредника, у которого нет **идентификатора MPN**, вместо него задается **идентификатор MPN** партнера.</span><span class="sxs-lookup"><span data-stu-id="3186e-154">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="3186e-155">Если партнер CSP удалит **MPN ID торгового посредника**, это значение будет равно *-1*.</span><span class="sxs-lookup"><span data-stu-id="3186e-155">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="3186e-156">Чтобы просмотреть или изменить **идентификатор MPN торгового посредника**:</span><span class="sxs-lookup"><span data-stu-id="3186e-156">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="3186e-157">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="3186e-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="3186e-158">В меню Центра партнеров выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="3186e-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="3186e-159">Выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="3186e-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="3186e-160">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="3186e-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="3186e-161">Выберите подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="3186e-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="3186e-162">Выберите **обновить**, чтобы изменить пункт **Торговый посредник (идентификатор MPN)**.</span><span class="sxs-lookup"><span data-stu-id="3186e-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>
