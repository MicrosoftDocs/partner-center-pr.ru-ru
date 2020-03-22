---
title: Использование файлов сверки | Центр партнеров
ms.topic: article
ms.date: 11/21/2019
description: Используйте файлы сверки, чтобы ознакомиться с подробными представлениями элементов в центре партнеров.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: 36b8242cc8c47ed36d16f86338a075080c2441e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "80114966"
---
# <a name="use-your-reconciliation-files"></a><span data-ttu-id="98283-103">Использование файлов сверки</span><span class="sxs-lookup"><span data-stu-id="98283-103">Use your reconciliation files</span></span>

<span data-ttu-id="98283-104">Область применения:</span><span class="sxs-lookup"><span data-stu-id="98283-104">Applies to:</span></span>

- <span data-ttu-id="98283-105">Партнерский центр</span><span class="sxs-lookup"><span data-stu-id="98283-105">Partner Center</span></span>
- <span data-ttu-id="98283-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="98283-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="98283-107">Вы можете скачать файлы сверки из центра партнеров, чтобы получить подробное представление каждого из элементов в цикле выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="98283-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="98283-108">Сведения об элементе строки включают в себя расходы на каждую из подписок клиента и подробные события (например, добавление мест в подписку).</span><span class="sxs-lookup"><span data-stu-id="98283-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="98283-109">Соответствующие роли:</span><span class="sxs-lookup"><span data-stu-id="98283-109">Appropriate roles:</span></span>

- <span data-ttu-id="98283-110">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="98283-110">Billing admin</span></span>
- <span data-ttu-id="98283-111">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="98283-111">Global admin</span></span>

<span data-ttu-id="98283-112">Сведения о том, как прочитать **счет**, см. в разделе [Чтение](read-your-bill.md)счета.</span><span class="sxs-lookup"><span data-stu-id="98283-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="98283-113">Общие сведения о полях файла сверки</span><span class="sxs-lookup"><span data-stu-id="98283-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="98283-114">Поля файла сверки на основе лицензий</span><span class="sxs-lookup"><span data-stu-id="98283-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="98283-115">Поля файла сверки с учетом использования</span><span class="sxs-lookup"><span data-stu-id="98283-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="98283-116">Поля файла одноразовой и повторяющейся сверки</span><span class="sxs-lookup"><span data-stu-id="98283-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="98283-117">Поля файла сверки с оценкой использования по дням</span><span class="sxs-lookup"><span data-stu-id="98283-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="98283-118">Понимание типов оплаты в файлах выверки</span><span class="sxs-lookup"><span data-stu-id="98283-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="98283-119">Сведения о типах начислений в файлах выверки (столбец **чаржетипе** ) см. в разделе [типы оплаты за файл выверки](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="98283-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="98283-120">Устранение проблем форматирования</span><span class="sxs-lookup"><span data-stu-id="98283-120">Fix formatting issues</span></span>

<span data-ttu-id="98283-121">Иногда файл сверки может содержать проблемы форматирования.</span><span class="sxs-lookup"><span data-stu-id="98283-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="98283-122">Например, эта проблема может возникать, если языковой стандарт EN-US не используется.</span><span class="sxs-lookup"><span data-stu-id="98283-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="98283-123">Чтобы устранить проблемы форматирования в файлах сверки, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="98283-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="98283-124">Откройте файл сверки (в формате CSV) в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="98283-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="98283-125">Выберите первый столбец в файле.</span><span class="sxs-lookup"><span data-stu-id="98283-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="98283-126">Откройте **Мастер преобразования текста в столбцы**.</span><span class="sxs-lookup"><span data-stu-id="98283-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="98283-127">На ленте выберите **данные**, а затем выберите **текст в столбцах**.</span><span class="sxs-lookup"><span data-stu-id="98283-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="98283-128">В мастере выберите **Тип файла с разделителями**.</span><span class="sxs-lookup"><span data-stu-id="98283-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="98283-129">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="98283-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="98283-130">В поле **разделители** выберите **запятая**.</span><span class="sxs-lookup"><span data-stu-id="98283-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="98283-131">(Если **вкладка** уже выбрана, можно оставить этот параметр установленным.) Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="98283-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="98283-132">В поле **Формат данных столбца** выберите **Date: mdy**.</span><span class="sxs-lookup"><span data-stu-id="98283-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="98283-133">Затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="98283-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="98283-134">В поле **Формат данных столбца** выберите **текст** для всех столбцов суммы.</span><span class="sxs-lookup"><span data-stu-id="98283-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="98283-135">Затем нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="98283-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="98283-136">Программное скачивание файлов выверки</span><span class="sxs-lookup"><span data-stu-id="98283-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="98283-137">Файлы сверки могут быть очень большими и иногда трудно скачивать.</span><span class="sxs-lookup"><span data-stu-id="98283-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="98283-138">Сведения об программной загрузке файлов выверки см. в разделе [Получение элементов строки счета](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="98283-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="98283-139">Сопоставьте налоги или НДС</span><span class="sxs-lookup"><span data-stu-id="98283-139">Map taxes or VAT</span></span>

<span data-ttu-id="98283-140">Чтобы сопоставлять налоги или налог на добавленные значения (VAT) к счету, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="98283-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="98283-141">Суммировать **налоговый** столбец из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="98283-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="98283-142">Вычислите сумму столбца **таксамаунт** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="98283-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="98283-143">Детализировать файлы сверки по партнерам</span><span class="sxs-lookup"><span data-stu-id="98283-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="98283-144">Партнеры в **косвенной модели** могут использовать эти дополнительные поля в файлах согласования на основе лицензий и на основе использования для перечисления файлов по торговому посреднику.</span><span class="sxs-lookup"><span data-stu-id="98283-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="98283-145">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="98283-145">MPN ID</span></span> | <span data-ttu-id="98283-146">Описание</span><span class="sxs-lookup"><span data-stu-id="98283-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="98283-147">Идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="98283-147">MPN ID</span></span> | <span data-ttu-id="98283-148">Идентификатор Microsoft Partner Network (MPN) для партнера поставщика облачных решений (CSP) (прямой или косвенный).</span><span class="sxs-lookup"><span data-stu-id="98283-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="98283-149">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="98283-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="98283-150">[Идентификатор MPN торгового посредника записи для подписки](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="98283-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="98283-151">Это поле соответствует ИДЕНТИФИКАТОРу торгового посредника, указанному для конкретной подписки в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="98283-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="98283-152">Отображается только в файлах выверки для партнеров в косвенной модели.</span><span class="sxs-lookup"><span data-stu-id="98283-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="98283-153">Идентификатор MPN торгового посредника</span><span class="sxs-lookup"><span data-stu-id="98283-153">Reseller MPN ID</span></span>

<span data-ttu-id="98283-154">Если партнер CSP продавал подписку непосредственно клиенту, его **идентификатор MPN** указывается дважды, как **идентификатор MPN** и **Идентификатор торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="98283-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="98283-155">Если у партнера CSP есть посредника, у которого нет **идентификатора MPN**, вместо него задается **идентификатор MPN** партнера.</span><span class="sxs-lookup"><span data-stu-id="98283-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="98283-156">Если партнер CSP удалит **MPN ID торгового посредника**, это значение будет равно *-1*.</span><span class="sxs-lookup"><span data-stu-id="98283-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="98283-157">Чтобы просмотреть или изменить **идентификатор MPN торгового посредника**:</span><span class="sxs-lookup"><span data-stu-id="98283-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="98283-158">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="98283-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="98283-159">В меню Центра партнеров выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="98283-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="98283-160">Выберите клиента в списке.</span><span class="sxs-lookup"><span data-stu-id="98283-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="98283-161">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="98283-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="98283-162">Выберите подписку из списка.</span><span class="sxs-lookup"><span data-stu-id="98283-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="98283-163">Выберите **обновить**, чтобы изменить пункт **Торговый посредник (идентификатор MPN)** .</span><span class="sxs-lookup"><span data-stu-id="98283-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
