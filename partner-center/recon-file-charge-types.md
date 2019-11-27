---
title: Типы оплаты файлов выверки | Центр партнеров
ms.topic: article
ms.date: 08/26/2019
description: Типы расходов (на основе лицензий, на основе использования и одноразовое время), кредиты и скидки по файлам сверки центра партнеров.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389812"
---
# <a name="understand-charge-types"></a><span data-ttu-id="dfb15-103">Общие сведения о типах затрат</span><span class="sxs-lookup"><span data-stu-id="dfb15-103">Understand charge types</span></span>

<span data-ttu-id="dfb15-104">Относится к:</span><span class="sxs-lookup"><span data-stu-id="dfb15-104">Applies to:</span></span>

- <span data-ttu-id="dfb15-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="dfb15-105">Partner Center</span></span>
- <span data-ttu-id="dfb15-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="dfb15-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="dfb15-107">В этом разделе описываются сопоставления между разделом счета и связанными типами затрат, которые могут находиться в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="dfb15-108">В счете представлена сводка по расходам.</span><span class="sxs-lookup"><span data-stu-id="dfb15-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="dfb15-109">Файл сверки содержит подробную разбивку транзакций по строкам, включая типы начислений.</span><span class="sxs-lookup"><span data-stu-id="dfb15-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="dfb15-110">Дополнительные сведения о файлах сверки см. [в разделе Использование файлов сверки](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="dfb15-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="dfb15-111">[Файлы согласованности на основе использования](usage-based-recon-files.md) и [файлы сверки на основе лицензий](license-based-recon-files.md) содержат только связанные с использованием транзакции и расходы (потребленные единицы и связанные с ней расходы).</span><span class="sxs-lookup"><span data-stu-id="dfb15-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="dfb15-112">Одноразовые кредиты, скидки или возмещения, которые отображаются в счете в качестве **корректировок** , не отображаются в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="dfb15-113">Сопоставьте типы расходов с накладными расходами</span><span class="sxs-lookup"><span data-stu-id="dfb15-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="dfb15-114">Для сбора сумм оплаты между счетом и файлом сверки используйте параметры фильтра в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="dfb15-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="dfb15-115">Фильтрация по типам оплаты в файле сверки для сопоставления расходов по счету с набором разбивки на счет для файла сверки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="dfb15-116">Оплата на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="dfb15-116">License-based charges</span></span>

<span data-ttu-id="dfb15-117">Чтобы связать эти расходы на основе лицензий с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="dfb15-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="dfb15-118">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="dfb15-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="dfb15-119">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="dfb15-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="dfb15-120">Сбор за активацию</span><span class="sxs-lookup"><span data-stu-id="dfb15-120">Activation fee</span></span> | <span data-ttu-id="dfb15-121">Сумма, выплаченная клиенту при использовании подписки после покупки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="dfb15-122">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="dfb15-122">Cancel fee</span></span> | <span data-ttu-id="dfb15-123">Пропорционально распределяется на клиент при изменении связанных мест.</span><span class="sxs-lookup"><span data-stu-id="dfb15-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="dfb15-124">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="dfb15-124">Cycle fee</span></span> | <span data-ttu-id="dfb15-125">Периодическая оплата за подписку.</span><span class="sxs-lookup"><span data-stu-id="dfb15-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="dfb15-126">Пропорциональное распределение экземпляра цикла</span><span class="sxs-lookup"><span data-stu-id="dfb15-126">Cycle instance prorate</span></span> | <span data-ttu-id="dfb15-127">При изменении связанных мест взимается плата за распределенные платежи от клиента.</span><span class="sxs-lookup"><span data-stu-id="dfb15-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="dfb15-128">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="dfb15-128">Prorate fees when cancel</span></span> | <span data-ttu-id="dfb15-129">Пропорциональное возмещение за неиспользуемую часть службы при отмене.</span><span class="sxs-lookup"><span data-stu-id="dfb15-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="dfb15-130">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="dfb15-130">Prorate fees when purchase</span></span> | <span data-ttu-id="dfb15-131">Тип оплаты для подписки при использовании годового счета.</span><span class="sxs-lookup"><span data-stu-id="dfb15-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="dfb15-132">Сбор при покупке</span><span class="sxs-lookup"><span data-stu-id="dfb15-132">Purchase fee</span></span> | <span data-ttu-id="dfb15-133">Тип оплаты для подписки при ежемесячном выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="dfb15-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="dfb15-134">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="dfb15-134">Prorate fee when renew</span></span> | <span data-ttu-id="dfb15-135">Пропорциональное вознаграждение при обновлении подписки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="dfb15-136">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="dfb15-136">Renew fee</span></span> | <span data-ttu-id="dfb15-137">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="dfb15-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="dfb15-138">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="dfb15-138">Prorate fees when activate</span></span> | <span data-ttu-id="dfb15-139">> распределяется за период с момента активации до окончания расчетного периода.</span><span class="sxs-lookup"><span data-stu-id="dfb15-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="dfb15-140">Оплата за один раз</span><span class="sxs-lookup"><span data-stu-id="dfb15-140">One-time charges</span></span>

<span data-ttu-id="dfb15-141">Чтобы связать эти одноразовые платежи с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="dfb15-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="dfb15-142">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="dfb15-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="dfb15-143">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="dfb15-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="dfb15-144">Оператор new</span><span class="sxs-lookup"><span data-stu-id="dfb15-144">New</span></span> | <span data-ttu-id="dfb15-145">Используется при создании новой покупки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="dfb15-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="dfb15-146">addQuantity</span></span> | <span data-ttu-id="dfb15-147">Используется как для возврата первоначальной покупки, так и для нового количества после увеличения.</span><span class="sxs-lookup"><span data-stu-id="dfb15-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="dfb15-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="dfb15-148">removeQuantity</span></span> | <span data-ttu-id="dfb15-149">Используется как для возврата первоначальной покупки, так и для нового количества после уменьшения.</span><span class="sxs-lookup"><span data-stu-id="dfb15-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="dfb15-150">Отмена</span><span class="sxs-lookup"><span data-stu-id="dfb15-150">Cancel</span></span> | <span data-ttu-id="dfb15-151">Используется при отмене подписки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="dfb15-152">Преобразование</span><span class="sxs-lookup"><span data-stu-id="dfb15-152">Convert</span></span> | <span data-ttu-id="dfb15-153">Используется при обновлении лицензии, но количество рабочих мест остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="dfb15-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="dfb15-154">Плата за использование</span><span class="sxs-lookup"><span data-stu-id="dfb15-154">Usage charges</span></span>

<span data-ttu-id="dfb15-155">Чтобы сопоставлять расходы на использование с накладной, вычислите столбец **PretaxCharges** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="dfb15-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="dfb15-156">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="dfb15-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="dfb15-157">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="dfb15-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="dfb15-158">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="dfb15-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="dfb15-159">Получите доступ к оплате за использование при отмене неоплачиваемого использования в течение текущего расчетного периода.</span><span class="sxs-lookup"><span data-stu-id="dfb15-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="dfb15-160">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="dfb15-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="dfb15-161">Плата за использование за текущий расчетный период.</span><span class="sxs-lookup"><span data-stu-id="dfb15-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="dfb15-162">Кредиты</span><span class="sxs-lookup"><span data-stu-id="dfb15-162">Credits</span></span>

<span data-ttu-id="dfb15-163">Чтобы связать эти кредиты с накладной:</span><span class="sxs-lookup"><span data-stu-id="dfb15-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="dfb15-164">Вычислите сумму **тоталфоркустомер** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="dfb15-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="dfb15-165">Вычислите сумму столбца **PostTaxTotal** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="dfb15-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="dfb15-166">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="dfb15-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="dfb15-167">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="dfb15-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="dfb15-168">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="dfb15-168">Offset a line item</span></span> | <span data-ttu-id="dfb15-169">Частичный или полный возврат к элементу строки, включая налоги.</span><span class="sxs-lookup"><span data-stu-id="dfb15-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="dfb15-170">Скидки на основе использования</span><span class="sxs-lookup"><span data-stu-id="dfb15-170">Usage-based discounts</span></span>

<span data-ttu-id="dfb15-171">Чтобы связать скидки на основе использования с накладной, суммируйте столбец **PretaxCharges** из файла, основанного на использовании.</span><span class="sxs-lookup"><span data-stu-id="dfb15-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="dfb15-172">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="dfb15-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="dfb15-173">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="dfb15-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="dfb15-174">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="dfb15-174">Activation discount</span></span> | <span data-ttu-id="dfb15-175">Скидка, применяемая при активации подписки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="dfb15-176">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="dfb15-176">Cycle discount</span></span> | <span data-ttu-id="dfb15-177">Скидка, применяемая к периодической оплате.</span><span class="sxs-lookup"><span data-stu-id="dfb15-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="dfb15-178">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="dfb15-178">Renew discount</span></span> | <span data-ttu-id="dfb15-179">Скидка, применяемая при продлении подписки.</span><span class="sxs-lookup"><span data-stu-id="dfb15-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="dfb15-180">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="dfb15-180">Cancel discount</span></span> | <span data-ttu-id="dfb15-181">Расходы, применяемые при отмене скидок.</span><span class="sxs-lookup"><span data-stu-id="dfb15-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="dfb15-182">Скидки на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="dfb15-182">License-based discounts</span></span>

<span data-ttu-id="dfb15-183">Чтобы сопоставлять скидки на основе лицензий с накладной, суммируйте столбец **тоталосердискаунт** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="dfb15-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="dfb15-184">*Скидки на основе лицензий могут применяться к нескольким типам оплаты.*</span><span class="sxs-lookup"><span data-stu-id="dfb15-184">*License-based discounts may be applied to multiple charge types.*</span></span>
