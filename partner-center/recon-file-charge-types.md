---
title: Типы расходов в файле выверки
ms.topic: article
ms.date: 06/05/2020
description: Узнайте о типах начислений (например, на основе лицензий, на основе использования и одноразовых), кредиты и скидках в файлах сверки центра партнеров.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549232"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="f90c9-103">Изучите различные типы оплаты в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="f90c9-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="f90c9-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="f90c9-104">**Applies to**</span></span>

- <span data-ttu-id="f90c9-105">Центр партнеров для облака Microsoft для государственных организаций</span><span class="sxs-lookup"><span data-stu-id="f90c9-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="f90c9-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="f90c9-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f90c9-107">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="f90c9-107">Admin agent</span></span>
- <span data-ttu-id="f90c9-108">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="f90c9-108">Billing admin</span></span>
- <span data-ttu-id="f90c9-109">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f90c9-109">Global admin</span></span>

<span data-ttu-id="f90c9-110">В этой статье описываются сопоставления между разделом счета и связанными типами оплаты, которые могут находиться в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="f90c9-111">В счете представлена сводка по расходам.</span><span class="sxs-lookup"><span data-stu-id="f90c9-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="f90c9-112">Файл сверки содержит подробную разбивку транзакций по строкам, включая типы начислений.</span><span class="sxs-lookup"><span data-stu-id="f90c9-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="f90c9-113">Дополнительные сведения о файлах сверки см. [в разделе Использование файлов сверки](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="f90c9-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="f90c9-114">[Файлы согласованности на основе использования](usage-based-recon-files.md) и [файлы сверки на основе лицензий](license-based-recon-files.md) содержат только связанные с использованием транзакции и расходы (потребленные единицы и связанные с ней расходы).</span><span class="sxs-lookup"><span data-stu-id="f90c9-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="f90c9-115">Одноразовые кредиты, скидки или возмещения, которые отображаются в счете в качестве **корректировок** , не отображаются в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="f90c9-116">Сопоставьте типы расходов с накладными расходами</span><span class="sxs-lookup"><span data-stu-id="f90c9-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="f90c9-117">Для сбора сумм оплаты между счетом и файлом сверки используйте параметры фильтра в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="f90c9-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="f90c9-118">Фильтрация по типам оплаты в файле сверки для сопоставления расходов по счету с набором разбивки на счет для файла сверки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="f90c9-119">Оплата на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="f90c9-119">License-based charges</span></span>

<span data-ttu-id="f90c9-120">Чтобы связать эти расходы на основе лицензий с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="f90c9-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="f90c9-121">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="f90c9-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f90c9-122">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="f90c9-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f90c9-123">Сбор за активацию</span><span class="sxs-lookup"><span data-stu-id="f90c9-123">Activation fee</span></span> | <span data-ttu-id="f90c9-124">Сумма, выплаченная клиенту при использовании подписки после покупки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="f90c9-125">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="f90c9-125">Cancel fee</span></span> | <span data-ttu-id="f90c9-126">Распределенные расходы, которые были возвращены клиенту при изменении связанных с ним лицензий.</span><span class="sxs-lookup"><span data-stu-id="f90c9-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="f90c9-127">Отмена пропорционального распределения экземпляра</span><span class="sxs-lookup"><span data-stu-id="f90c9-127">Cancel instance prorate</span></span> | <span data-ttu-id="f90c9-128">Распределенные платежи отменяются, когда у клиента с месячной подпиской есть приостановленная подписка, а связанные с ней лицензии изменяются в тот же месяц.</span><span class="sxs-lookup"><span data-stu-id="f90c9-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="f90c9-129">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="f90c9-129">Cycle fee</span></span> | <span data-ttu-id="f90c9-130">Периодическая оплата за подписку.</span><span class="sxs-lookup"><span data-stu-id="f90c9-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="f90c9-131">Пропорциональное распределение экземпляра цикла</span><span class="sxs-lookup"><span data-stu-id="f90c9-131">Cycle instance prorate</span></span> | <span data-ttu-id="f90c9-132">При изменении связанных лицензий взимается плата за распределенные платежи от клиента.</span><span class="sxs-lookup"><span data-stu-id="f90c9-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="f90c9-133">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="f90c9-133">Prorate fees when cancel</span></span> | <span data-ttu-id="f90c9-134">Пропорциональное возмещение за неиспользуемую часть службы при отмене.</span><span class="sxs-lookup"><span data-stu-id="f90c9-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="f90c9-135">Пропорциональное количество выплат при преобразовании из текущего предложения</span><span class="sxs-lookup"><span data-stu-id="f90c9-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="f90c9-136">Плата распределяется пропорционально после преобразования текущей ежемесячной подписки в годовую.</span><span class="sxs-lookup"><span data-stu-id="f90c9-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="f90c9-137">Пропорциональное количество выплат при преобразовании в новое предложение</span><span class="sxs-lookup"><span data-stu-id="f90c9-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="f90c9-138">Плата распределяется пропорционально после преобразования месячной подписки в новую годовую подписку.</span><span class="sxs-lookup"><span data-stu-id="f90c9-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="f90c9-139">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="f90c9-139">Prorate fees when purchase</span></span> | <span data-ttu-id="f90c9-140">Тип оплаты для подписки при использовании ежемесячного или годового счета.</span><span class="sxs-lookup"><span data-stu-id="f90c9-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="f90c9-141">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="f90c9-141">Prorate fee when renew</span></span> | <span data-ttu-id="f90c9-142">Пропорциональное вознаграждение при обновлении подписки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="f90c9-143">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="f90c9-143">Renew fee</span></span> | <span data-ttu-id="f90c9-144">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="f90c9-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="f90c9-145">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="f90c9-145">Prorate fees when activate</span></span> | <span data-ttu-id="f90c9-146">Пропорциональное количество выплат с активации до окончания расчетного периода.</span><span class="sxs-lookup"><span data-stu-id="f90c9-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="f90c9-147">Оплата за один раз</span><span class="sxs-lookup"><span data-stu-id="f90c9-147">One-time charges</span></span>

<span data-ttu-id="f90c9-148">Чтобы связать эти одноразовые платежи с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="f90c9-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="f90c9-149">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="f90c9-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f90c9-150">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="f90c9-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f90c9-151">Оператор new</span><span class="sxs-lookup"><span data-stu-id="f90c9-151">New</span></span> | <span data-ttu-id="f90c9-152">Используется при создании новой покупки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="f90c9-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="f90c9-153">addQuantity</span></span> | <span data-ttu-id="f90c9-154">Используется как для возврата первоначальной покупки, так и для нового количества после увеличения.</span><span class="sxs-lookup"><span data-stu-id="f90c9-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="f90c9-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="f90c9-155">removeQuantity</span></span> | <span data-ttu-id="f90c9-156">Используется как для возврата первоначальной покупки, так и для нового количества после уменьшения.</span><span class="sxs-lookup"><span data-stu-id="f90c9-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="f90c9-157">Отменить</span><span class="sxs-lookup"><span data-stu-id="f90c9-157">Cancel</span></span> | <span data-ttu-id="f90c9-158">Используется при отмене подписки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="f90c9-159">Convert</span><span class="sxs-lookup"><span data-stu-id="f90c9-159">Convert</span></span> | <span data-ttu-id="f90c9-160">Используется при обновлении лицензии, но число лицензий остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="f90c9-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="f90c9-161">Плата за использование</span><span class="sxs-lookup"><span data-stu-id="f90c9-161">Usage charges</span></span>

<span data-ttu-id="f90c9-162">Чтобы сопоставлять расходы на использование с накладной, вычислите столбец **PretaxCharges** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="f90c9-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="f90c9-163">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="f90c9-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f90c9-164">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="f90c9-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f90c9-165">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="f90c9-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="f90c9-166">Плата за пользование при аннулировании за неоплачиваемое использование в течение текущего платежного периода.</span><span class="sxs-lookup"><span data-stu-id="f90c9-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="f90c9-167">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="f90c9-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="f90c9-168">Плата за пользование для текущего периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="f90c9-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="f90c9-169">Благодарности</span><span class="sxs-lookup"><span data-stu-id="f90c9-169">Credits</span></span>

<span data-ttu-id="f90c9-170">Чтобы связать эти кредиты с накладной:</span><span class="sxs-lookup"><span data-stu-id="f90c9-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="f90c9-171">Вычислите сумму **тоталфоркустомер** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="f90c9-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="f90c9-172">Вычислите сумму столбца **PostTaxTotal** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="f90c9-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="f90c9-173">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="f90c9-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f90c9-174">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="f90c9-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f90c9-175">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="f90c9-175">Offset a line item</span></span> | <span data-ttu-id="f90c9-176">Частичное или полное возмещение за позицию в строке (с налогом).</span><span class="sxs-lookup"><span data-stu-id="f90c9-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="f90c9-177">Скидки на основе использования</span><span class="sxs-lookup"><span data-stu-id="f90c9-177">Usage-based discounts</span></span>

<span data-ttu-id="f90c9-178">Чтобы связать скидки на основе использования с накладной, суммируйте столбец **PretaxCharges** из файла, основанного на использовании.</span><span class="sxs-lookup"><span data-stu-id="f90c9-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="f90c9-179">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="f90c9-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f90c9-180">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="f90c9-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f90c9-181">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="f90c9-181">Activation discount</span></span> | <span data-ttu-id="f90c9-182">Скидка, применяемая при активации подписки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="f90c9-183">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="f90c9-183">Cycle discount</span></span> | <span data-ttu-id="f90c9-184">Скидка, действующая на периодические платежи.</span><span class="sxs-lookup"><span data-stu-id="f90c9-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="f90c9-185">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="f90c9-185">Renew discount</span></span> | <span data-ttu-id="f90c9-186">Скидка, применяемая при продлении подписки.</span><span class="sxs-lookup"><span data-stu-id="f90c9-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="f90c9-187">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="f90c9-187">Cancel discount</span></span> | <span data-ttu-id="f90c9-188">Плата, которая взимается при отмене скидок.</span><span class="sxs-lookup"><span data-stu-id="f90c9-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="f90c9-189">Скидки на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="f90c9-189">License-based discounts</span></span>

<span data-ttu-id="f90c9-190">Чтобы сопоставлять скидки на основе лицензий с накладной, суммируйте столбец **тоталосердискаунт** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="f90c9-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="f90c9-191">*Скидки на основе лицензий могут применяться к нескольким типам оплаты.*</span><span class="sxs-lookup"><span data-stu-id="f90c9-191">*License-based discounts may be applied to multiple charge types.*</span></span>
