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
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855885"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="d8f98-103">Изучите различные типы оплаты в файлах сверки центра партнеров</span><span class="sxs-lookup"><span data-stu-id="d8f98-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="d8f98-104">Область **применения**: центр партнеров | Центр партнеров по Microsoft Cloud для государственных организаций США</span><span class="sxs-lookup"><span data-stu-id="d8f98-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d8f98-105">**Соответствующие роли**: Агент администрирования | Администратор выставления счетов | Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d8f98-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="d8f98-106">В этой статье описываются сопоставления между разделом счета и связанными типами оплаты, которые могут находиться в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="d8f98-107">В счете представлена сводка по расходам.</span><span class="sxs-lookup"><span data-stu-id="d8f98-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="d8f98-108">Файл сверки содержит подробную разбивку транзакций по строкам, включая типы начислений.</span><span class="sxs-lookup"><span data-stu-id="d8f98-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="d8f98-109">Дополнительные сведения о файлах сверки см. [в разделе Использование файлов сверки](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="d8f98-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="d8f98-110">[Файлы согласованности на основе использования](usage-based-recon-files.md) и [файлы сверки на основе лицензий](license-based-recon-files.md) содержат только связанные с использованием транзакции и расходы (потребленные единицы и связанные с ней расходы).</span><span class="sxs-lookup"><span data-stu-id="d8f98-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="d8f98-111">Одноразовые кредиты, скидки или возмещения, которые отображаются в счете в качестве **корректировок** , не отображаются в файле сверки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="d8f98-112">Сопоставьте типы расходов с накладными расходами</span><span class="sxs-lookup"><span data-stu-id="d8f98-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="d8f98-113">Для сбора сумм оплаты между счетом и файлом сверки используйте параметры фильтра в Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="d8f98-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="d8f98-114">Фильтрация по типам оплаты в файле сверки для сопоставления расходов по счету с набором разбивки на счет для файла сверки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="d8f98-115">Оплата на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="d8f98-115">License-based charges</span></span>

<span data-ttu-id="d8f98-116">Чтобы связать эти расходы на основе лицензий с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="d8f98-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="d8f98-117">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="d8f98-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d8f98-118">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="d8f98-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d8f98-119">Сбор за активацию</span><span class="sxs-lookup"><span data-stu-id="d8f98-119">Activation fee</span></span> | <span data-ttu-id="d8f98-120">Сумма, выплаченная клиенту при использовании подписки после покупки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="d8f98-121">Сбор за отмену</span><span class="sxs-lookup"><span data-stu-id="d8f98-121">Cancel fee</span></span> | <span data-ttu-id="d8f98-122">Распределенные расходы, которые были возвращены клиенту при изменении связанных с ним лицензий.</span><span class="sxs-lookup"><span data-stu-id="d8f98-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="d8f98-123">Отмена пропорционального распределения экземпляра</span><span class="sxs-lookup"><span data-stu-id="d8f98-123">Cancel instance prorate</span></span> | <span data-ttu-id="d8f98-124">Распределенные платежи отменяются, когда у клиента с месячной подпиской есть приостановленная подписка, а связанные с ней лицензии изменяются в тот же месяц.</span><span class="sxs-lookup"><span data-stu-id="d8f98-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="d8f98-125">Оплата цикла</span><span class="sxs-lookup"><span data-stu-id="d8f98-125">Cycle fee</span></span> | <span data-ttu-id="d8f98-126">Периодическая оплата за подписку.</span><span class="sxs-lookup"><span data-stu-id="d8f98-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="d8f98-127">Пропорциональное распределение экземпляра цикла</span><span class="sxs-lookup"><span data-stu-id="d8f98-127">Cycle instance prorate</span></span> | <span data-ttu-id="d8f98-128">При изменении связанных лицензий взимается плата за распределенные платежи от клиента.</span><span class="sxs-lookup"><span data-stu-id="d8f98-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="d8f98-129">Пропорциональные сборы при отмене</span><span class="sxs-lookup"><span data-stu-id="d8f98-129">Prorate fees when cancel</span></span> | <span data-ttu-id="d8f98-130">Пропорциональное возмещение за неиспользуемую часть службы при отмене.</span><span class="sxs-lookup"><span data-stu-id="d8f98-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="d8f98-131">Пропорциональное количество выплат при преобразовании из текущего предложения</span><span class="sxs-lookup"><span data-stu-id="d8f98-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="d8f98-132">Плата распределяется пропорционально после преобразования текущей ежемесячной подписки в годовую.</span><span class="sxs-lookup"><span data-stu-id="d8f98-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="d8f98-133">Пропорциональное количество выплат при преобразовании в новое предложение</span><span class="sxs-lookup"><span data-stu-id="d8f98-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="d8f98-134">Плата распределяется пропорционально после преобразования месячной подписки в новую годовую подписку.</span><span class="sxs-lookup"><span data-stu-id="d8f98-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="d8f98-135">Пропорциональные сборы при покупке</span><span class="sxs-lookup"><span data-stu-id="d8f98-135">Prorate fees when purchase</span></span> | <span data-ttu-id="d8f98-136">Тип оплаты для подписки при использовании ежемесячного или годового счета.</span><span class="sxs-lookup"><span data-stu-id="d8f98-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="d8f98-137">Пропорциональные сборы при обновлении</span><span class="sxs-lookup"><span data-stu-id="d8f98-137">Prorate fee when renew</span></span> | <span data-ttu-id="d8f98-138">Пропорциональное вознаграждение при обновлении подписки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="d8f98-139">Плата за обновление</span><span class="sxs-lookup"><span data-stu-id="d8f98-139">Renew fee</span></span> | <span data-ttu-id="d8f98-140">Платеж за обновление подписки</span><span class="sxs-lookup"><span data-stu-id="d8f98-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="d8f98-141">Пропорциональные сборы при активации</span><span class="sxs-lookup"><span data-stu-id="d8f98-141">Prorate fees when activate</span></span> | <span data-ttu-id="d8f98-142">Пропорциональное количество выплат с активации до окончания расчетного периода.</span><span class="sxs-lookup"><span data-stu-id="d8f98-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="d8f98-143">Оплата за один раз</span><span class="sxs-lookup"><span data-stu-id="d8f98-143">One-time charges</span></span>

<span data-ttu-id="d8f98-144">Чтобы связать эти одноразовые платежи с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="d8f98-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="d8f98-145">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="d8f98-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d8f98-146">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="d8f98-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d8f98-147">Создать</span><span class="sxs-lookup"><span data-stu-id="d8f98-147">New</span></span> | <span data-ttu-id="d8f98-148">Используется при создании новой покупки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="d8f98-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="d8f98-149">addQuantity</span></span> | <span data-ttu-id="d8f98-150">Используется как для возврата первоначальной покупки, так и для нового количества после увеличения.</span><span class="sxs-lookup"><span data-stu-id="d8f98-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="d8f98-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="d8f98-151">removeQuantity</span></span> | <span data-ttu-id="d8f98-152">Используется как для возврата первоначальной покупки, так и для нового количества после уменьшения.</span><span class="sxs-lookup"><span data-stu-id="d8f98-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="d8f98-153">Отменить</span><span class="sxs-lookup"><span data-stu-id="d8f98-153">Cancel</span></span> | <span data-ttu-id="d8f98-154">Используется при отмене подписки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="d8f98-155">Convert</span><span class="sxs-lookup"><span data-stu-id="d8f98-155">Convert</span></span> | <span data-ttu-id="d8f98-156">Используется при обновлении лицензии, но число лицензий остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="d8f98-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="d8f98-157">Плата за использование</span><span class="sxs-lookup"><span data-stu-id="d8f98-157">Usage charges</span></span>

<span data-ttu-id="d8f98-158">Чтобы сопоставлять расходы на использование с накладной, вычислите столбец **PretaxCharges** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="d8f98-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="d8f98-159">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="d8f98-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d8f98-160">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="d8f98-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d8f98-161">Плата за использование Assess при отмене</span><span class="sxs-lookup"><span data-stu-id="d8f98-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="d8f98-162">Плата за пользование при аннулировании за неоплачиваемое использование в течение текущего платежного периода.</span><span class="sxs-lookup"><span data-stu-id="d8f98-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="d8f98-163">Плата за использование Assess для текущего цикла</span><span class="sxs-lookup"><span data-stu-id="d8f98-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="d8f98-164">Плата за пользование для текущего периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d8f98-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="d8f98-165">Благодарности</span><span class="sxs-lookup"><span data-stu-id="d8f98-165">Credits</span></span>

<span data-ttu-id="d8f98-166">Чтобы связать эти кредиты с накладной:</span><span class="sxs-lookup"><span data-stu-id="d8f98-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="d8f98-167">Вычислите сумму **тоталфоркустомер** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="d8f98-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="d8f98-168">Вычислите сумму столбца **PostTaxTotal** из файла на основе использования.</span><span class="sxs-lookup"><span data-stu-id="d8f98-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="d8f98-169">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="d8f98-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d8f98-170">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="d8f98-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d8f98-171">Смещение позиции строки</span><span class="sxs-lookup"><span data-stu-id="d8f98-171">Offset a line item</span></span> | <span data-ttu-id="d8f98-172">Частичное или полное возмещение за позицию в строке (с налогом).</span><span class="sxs-lookup"><span data-stu-id="d8f98-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="d8f98-173">Скидки на основе использования</span><span class="sxs-lookup"><span data-stu-id="d8f98-173">Usage-based discounts</span></span>

<span data-ttu-id="d8f98-174">Чтобы связать скидки на основе использования с накладной, суммируйте столбец **PretaxCharges** из файла, основанного на использовании.</span><span class="sxs-lookup"><span data-stu-id="d8f98-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="d8f98-175">Описание платы (столбец Чаржетипе в файле сверки)</span><span class="sxs-lookup"><span data-stu-id="d8f98-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="d8f98-176">Объяснение затрат</span><span class="sxs-lookup"><span data-stu-id="d8f98-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="d8f98-177">Скидка при активации</span><span class="sxs-lookup"><span data-stu-id="d8f98-177">Activation discount</span></span> | <span data-ttu-id="d8f98-178">Скидка, применяемая при активации подписки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="d8f98-179">Скидка на цикл</span><span class="sxs-lookup"><span data-stu-id="d8f98-179">Cycle discount</span></span> | <span data-ttu-id="d8f98-180">Скидка, действующая на периодические платежи.</span><span class="sxs-lookup"><span data-stu-id="d8f98-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="d8f98-181">Скидка при возобновлении</span><span class="sxs-lookup"><span data-stu-id="d8f98-181">Renew discount</span></span> | <span data-ttu-id="d8f98-182">Скидка, применяемая при продлении подписки.</span><span class="sxs-lookup"><span data-stu-id="d8f98-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="d8f98-183">Скидка при отмене</span><span class="sxs-lookup"><span data-stu-id="d8f98-183">Cancel discount</span></span> | <span data-ttu-id="d8f98-184">Плата, которая взимается при отмене скидок.</span><span class="sxs-lookup"><span data-stu-id="d8f98-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="d8f98-185">Скидки на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="d8f98-185">License-based discounts</span></span>

<span data-ttu-id="d8f98-186">Чтобы сопоставлять скидки на основе лицензий с накладной, суммируйте столбец **тоталосердискаунт** из файла, основанного на лицензии.</span><span class="sxs-lookup"><span data-stu-id="d8f98-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="d8f98-187">*Скидки на основе лицензий могут применяться к нескольким типам оплаты.*</span><span class="sxs-lookup"><span data-stu-id="d8f98-187">*License-based discounts may be applied to multiple charge types.*</span></span>
