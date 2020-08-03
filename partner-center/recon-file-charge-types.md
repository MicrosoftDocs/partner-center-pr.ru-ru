---
title: Типы расходов в файле выверки
ms.topic: article
ms.date: 06/05/2020
description: Узнайте о типах начислений (например, на основе лицензий, на основе использования и одноразовых), кредиты и скидках в файлах сверки центра партнеров.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2020
ms.locfileid: "87479117"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="af97a-103">Изучите различные типы оплаты в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="af97a-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="af97a-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="af97a-104">**Applies to**</span></span>

- <span data-ttu-id="af97a-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="af97a-105">Partner Center</span></span>
- <span data-ttu-id="af97a-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="af97a-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="af97a-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="af97a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="af97a-108">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="af97a-108">Admin agent</span></span>
- <span data-ttu-id="af97a-109">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="af97a-109">Billing admin</span></span>
- <span data-ttu-id="af97a-110">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="af97a-110">Global admin</span></span>

<span data-ttu-id="af97a-111">В этом разделе описываются сопоставления между разделом счета и связанными типами затрат, которые могут находиться в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="af97a-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="af97a-112">В счете представлена сводка по расходам.</span><span class="sxs-lookup"><span data-stu-id="af97a-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="af97a-113">Файл сверки содержит подробную разбивку транзакций по строкам, включая типы начислений.</span><span class="sxs-lookup"><span data-stu-id="af97a-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="af97a-114">Дополнительные сведения о файлах сверки см. [в разделе Использование файлов сверки](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="af97a-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="af97a-115">[Файлы согласованности на основе использования](usage-based-recon-files.md) и [файлы сверки на основе лицензий](license-based-recon-files.md) содержат только связанные с использованием транзакции и расходы (потребленные единицы и связанные с ней расходы).</span><span class="sxs-lookup"><span data-stu-id="af97a-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="af97a-116">Одноразовые кредиты, скидки или возмещения, которые отображаются в счете в качестве **корректировок** , не отображаются в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="af97a-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="af97a-117">Сопоставьте типы расходов с накладными расходами</span><span class="sxs-lookup"><span data-stu-id="af97a-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="af97a-118">Для сбора сумм оплаты между счетом и файлом сверки используйте параметры фильтра в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="af97a-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="af97a-119">Фильтрация по типам оплаты в файле сверки для сопоставления расходов по счету с набором разбивки на счет для файла сверки.</span><span class="sxs-lookup"><span data-stu-id="af97a-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="af97a-120">Оплата на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="af97a-120">License-based charges</span></span>

<span data-ttu-id="af97a-121">Чтобы связать эти расходы на основе лицензий с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="af97a-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="af97a-122">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="af97a-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="af97a-123">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="af97a-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="af97a-124">Сбор за активацию</span><span class="sxs-lookup"><span data-stu-id="af97a-124">Activation fee</span></span> | <span data-ttu-id="af97a-125">Сумма, выплаченная клиенту при использовании подписки после покупки.</span><span class="sxs-lookup"><span data-stu-id="af97a-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="af97a-126">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="af97a-126">Cancel fee</span></span> | <span data-ttu-id="af97a-127">Распределенные расходы, которые были возвращены клиенту при изменении связанных с ним лицензий.</span><span class="sxs-lookup"><span data-stu-id="af97a-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="af97a-128">Отмена пропорционального распределения экземпляра</span><span class="sxs-lookup"><span data-stu-id="af97a-128">Cancel instance prorate</span></span> | <span data-ttu-id="af97a-129">Распределенные платежи отменяются, когда у клиента с месячной подпиской есть приостановленная подписка, а связанные с ней лицензии изменяются в тот же месяц.</span><span class="sxs-lookup"><span data-stu-id="af97a-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="af97a-130">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="af97a-130">Cycle fee</span></span> | <span data-ttu-id="af97a-131">Периодическая оплата за подписку.</span><span class="sxs-lookup"><span data-stu-id="af97a-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="af97a-132">Пропорциональное распределение экземпляра цикла</span><span class="sxs-lookup"><span data-stu-id="af97a-132">Cycle instance prorate</span></span> | <span data-ttu-id="af97a-133">При изменении связанных лицензий взимается плата за распределенные платежи от клиента.</span><span class="sxs-lookup"><span data-stu-id="af97a-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="af97a-134">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="af97a-134">Prorate fees when cancel</span></span> | <span data-ttu-id="af97a-135">Пропорциональное возмещение за неиспользуемую часть службы при отмене.</span><span class="sxs-lookup"><span data-stu-id="af97a-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="af97a-136">Пропорциональное количество выплат при преобразовании из текущего предложения</span><span class="sxs-lookup"><span data-stu-id="af97a-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="af97a-137">Плата распределяется пропорционально после преобразования текущей ежемесячной подписки в годовую.</span><span class="sxs-lookup"><span data-stu-id="af97a-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="af97a-138">Пропорциональное количество выплат при преобразовании в новое предложение</span><span class="sxs-lookup"><span data-stu-id="af97a-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="af97a-139">Плата распределяется пропорционально после преобразования месячной подписки в новую годовую подписку.</span><span class="sxs-lookup"><span data-stu-id="af97a-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="af97a-140">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="af97a-140">Prorate fees when purchase</span></span> | <span data-ttu-id="af97a-141">Тип оплаты для подписки при использовании ежемесячного или годового счета.</span><span class="sxs-lookup"><span data-stu-id="af97a-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="af97a-142">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="af97a-142">Prorate fee when renew</span></span> | <span data-ttu-id="af97a-143">Пропорциональное вознаграждение при обновлении подписки.</span><span class="sxs-lookup"><span data-stu-id="af97a-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="af97a-144">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="af97a-144">Renew fee</span></span> | <span data-ttu-id="af97a-145">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="af97a-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="af97a-146">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="af97a-146">Prorate fees when activate</span></span> | <span data-ttu-id="af97a-147">Пропорциональное количество выплат с активации до окончания расчетного периода.</span><span class="sxs-lookup"><span data-stu-id="af97a-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="af97a-148">Оплата за один раз</span><span class="sxs-lookup"><span data-stu-id="af97a-148">One-time charges</span></span>

<span data-ttu-id="af97a-149">Чтобы связать эти одноразовые платежи с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="af97a-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="af97a-150">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="af97a-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="af97a-151">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="af97a-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="af97a-152">Оператор new</span><span class="sxs-lookup"><span data-stu-id="af97a-152">New</span></span> | <span data-ttu-id="af97a-153">Используется при создании новой покупки.</span><span class="sxs-lookup"><span data-stu-id="af97a-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="af97a-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="af97a-154">addQuantity</span></span> | <span data-ttu-id="af97a-155">Используется как для возврата первоначальной покупки, так и для нового количества после увеличения.</span><span class="sxs-lookup"><span data-stu-id="af97a-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="af97a-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="af97a-156">removeQuantity</span></span> | <span data-ttu-id="af97a-157">Используется как для возврата первоначальной покупки, так и для нового количества после уменьшения.</span><span class="sxs-lookup"><span data-stu-id="af97a-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="af97a-158">Отменить</span><span class="sxs-lookup"><span data-stu-id="af97a-158">Cancel</span></span> | <span data-ttu-id="af97a-159">Используется при отмене подписки.</span><span class="sxs-lookup"><span data-stu-id="af97a-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="af97a-160">Convert</span><span class="sxs-lookup"><span data-stu-id="af97a-160">Convert</span></span> | <span data-ttu-id="af97a-161">Используется при обновлении лицензии, но число лицензий остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="af97a-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="af97a-162">Плата за использование</span><span class="sxs-lookup"><span data-stu-id="af97a-162">Usage charges</span></span>

<span data-ttu-id="af97a-163">Чтобы сопоставлять расходы на использование с накладной, вычислите столбец **PretaxCharges** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="af97a-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="af97a-164">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="af97a-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="af97a-165">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="af97a-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="af97a-166">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="af97a-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="af97a-167">Плата за пользование при аннулировании за неоплачиваемое использование в течение текущего платежного периода.</span><span class="sxs-lookup"><span data-stu-id="af97a-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="af97a-168">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="af97a-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="af97a-169">Плата за пользование для текущего периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="af97a-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="af97a-170">Благодарности</span><span class="sxs-lookup"><span data-stu-id="af97a-170">Credits</span></span>

<span data-ttu-id="af97a-171">Чтобы связать эти кредиты с накладной:</span><span class="sxs-lookup"><span data-stu-id="af97a-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="af97a-172">Вычислите сумму **тоталфоркустомер** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="af97a-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="af97a-173">Вычислите сумму столбца **PostTaxTotal** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="af97a-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="af97a-174">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="af97a-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="af97a-175">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="af97a-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="af97a-176">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="af97a-176">Offset a line item</span></span> | <span data-ttu-id="af97a-177">Частичное или полное возмещение за позицию в строке (с налогом).</span><span class="sxs-lookup"><span data-stu-id="af97a-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="af97a-178">Скидки на основе использования</span><span class="sxs-lookup"><span data-stu-id="af97a-178">Usage-based discounts</span></span>

<span data-ttu-id="af97a-179">Чтобы связать скидки на основе использования с накладной, суммируйте столбец **PretaxCharges** из файла, основанного на использовании.</span><span class="sxs-lookup"><span data-stu-id="af97a-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="af97a-180">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="af97a-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="af97a-181">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="af97a-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="af97a-182">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="af97a-182">Activation discount</span></span> | <span data-ttu-id="af97a-183">Скидка, применяемая при активации подписки.</span><span class="sxs-lookup"><span data-stu-id="af97a-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="af97a-184">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="af97a-184">Cycle discount</span></span> | <span data-ttu-id="af97a-185">Скидка, действующая на периодические платежи.</span><span class="sxs-lookup"><span data-stu-id="af97a-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="af97a-186">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="af97a-186">Renew discount</span></span> | <span data-ttu-id="af97a-187">Скидка, применяемая при продлении подписки.</span><span class="sxs-lookup"><span data-stu-id="af97a-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="af97a-188">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="af97a-188">Cancel discount</span></span> | <span data-ttu-id="af97a-189">Плата, которая взимается при отмене скидок.</span><span class="sxs-lookup"><span data-stu-id="af97a-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="af97a-190">Скидки на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="af97a-190">License-based discounts</span></span>

<span data-ttu-id="af97a-191">Чтобы сопоставлять скидки на основе лицензий с накладной, суммируйте столбец **тоталосердискаунт** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="af97a-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="af97a-192">*Скидки на основе лицензий могут применяться к нескольким типам оплаты.*</span><span class="sxs-lookup"><span data-stu-id="af97a-192">*License-based discounts may be applied to multiple charge types.*</span></span>
