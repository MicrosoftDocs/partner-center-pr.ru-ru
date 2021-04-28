---
title: Вычисление фактической цены за единицу
ms.topic: how-to
ms.date: 04/02/2021
description: Сведения о эффективной цене за единицу и способах ее вычисления. В этой статье также приводится пример вычисления.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172223"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="e1b8d-104">Фактическое Вычисление цены за единицу для использования плана Azure</span><span class="sxs-lookup"><span data-stu-id="e1b8d-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="e1b8d-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="e1b8d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e1b8d-106">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="e1b8d-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="e1b8d-107">Эффективная цена за единицу</span><span class="sxs-lookup"><span data-stu-id="e1b8d-107">The effective unit price</span></span>

<span data-ttu-id="e1b8d-108">Эффективная цена за единицу рассчитывается на уровне счетчика (в отличие от уровня ресурса) и корректируется ежедневно в соответствии с использованием счетчика.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="e1b8d-109">Мы вычисляем эффективные цены за единицу, используя следующие три фактора:</span><span class="sxs-lookup"><span data-stu-id="e1b8d-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="e1b8d-110">Потребление, которое отслеживается ежедневно в рамках цикла выставления счетов</span><span class="sxs-lookup"><span data-stu-id="e1b8d-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="e1b8d-111">Оплачиваемые затраты для счетчика</span><span class="sxs-lookup"><span data-stu-id="e1b8d-111">Billable cost for the meter</span></span>
- <span data-ttu-id="e1b8d-112">Распределение по уровням (если применимо)</span><span class="sxs-lookup"><span data-stu-id="e1b8d-112">Tiering (if applicable)</span></span>

<span data-ttu-id="e1b8d-113">Так как мы отслеживаем ежедневное потребление на протяжении всего цикла выставления счетов, Цена за единицу будет меняться.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="e1b8d-114">Окончательная цена за указанный цикл выставления счетов будет доступна после отключения расчета потребления и закрытия периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="e1b8d-115">Вы увидите большинство изменений в использовании после четвертого или пятого десятичного разряда.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="e1b8d-116">Узнайте, использует ли ваш счетчик многоуровневые цены</span><span class="sxs-lookup"><span data-stu-id="e1b8d-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="e1b8d-117">Если вы не хотите узнать, использует ли ваш счетчик многоуровневые цены, воспользуйтесь приведенной ниже процедурой.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="e1b8d-118">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="e1b8d-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="e1b8d-119">Выберите **Продажа**, выберите **цены и предложения**, а затем выберите пункт **цены на план Azure**.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="e1b8d-120">Найдите свой счетчик по ИДЕНТИФИКАТОРу, а затем скачайте данные о ценах.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="e1b8d-121">Пример вычисления</span><span class="sxs-lookup"><span data-stu-id="e1b8d-121">Sample calculation</span></span>

<span data-ttu-id="e1b8d-122">В таблице ниже приведен пример того, как вычисляется эффективная цена за единицу в течение периода открытия.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="e1b8d-123">В таблице применяются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="e1b8d-124">**Up** = Цена за единицу ресурса/час = 0,868</span><span class="sxs-lookup"><span data-stu-id="e1b8d-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="e1b8d-125">**БКУ** = оплачиваемая единица потребления для счетчика</span><span class="sxs-lookup"><span data-stu-id="e1b8d-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="e1b8d-126">**BC** = оплачиваемые затраты для счетчика = БКУ \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="e1b8d-127">Это отражает корректировку для скидки с 15% на PEC.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="e1b8d-128">Затем мы используем нижний предел функции, чтобы ограничить значение двумя цифрами после десятичной запятой, чтобы вычислить минимальную сумму.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="e1b8d-129">**Эффективная цена единицы** = БКУ/BC</span><span class="sxs-lookup"><span data-stu-id="e1b8d-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="e1b8d-130">Примечание. в этом примере у измерения нет уровней ценообразования или других скидок — эффективных коэффициентов единиц измерения в процентах скидки и других корректировок.</span><span class="sxs-lookup"><span data-stu-id="e1b8d-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="e1b8d-131">Дата</span><span class="sxs-lookup"><span data-stu-id="e1b8d-131">Date</span></span> | <span data-ttu-id="e1b8d-132">БКУ (оплачиваемая единица потребления)</span><span class="sxs-lookup"><span data-stu-id="e1b8d-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="e1b8d-133">BC (оплачиваемая стоимость)</span><span class="sxs-lookup"><span data-stu-id="e1b8d-133">BC (Billable cost)</span></span> | <span data-ttu-id="e1b8d-134">Эффективная цена за единицу</span><span class="sxs-lookup"><span data-stu-id="e1b8d-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="e1b8d-135">3 — Авг</span><span class="sxs-lookup"><span data-stu-id="e1b8d-135">3-Aug</span></span> | <span data-ttu-id="e1b8d-136">29</span><span class="sxs-lookup"><span data-stu-id="e1b8d-136">29</span></span> | <span data-ttu-id="e1b8d-137">21,39</span><span class="sxs-lookup"><span data-stu-id="e1b8d-137">21.39</span></span> | <span data-ttu-id="e1b8d-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="e1b8d-138">0.737586206896552</span></span> |
| <span data-ttu-id="e1b8d-139">10 августа</span><span class="sxs-lookup"><span data-stu-id="e1b8d-139">10-Aug</span></span> | <span data-ttu-id="e1b8d-140">210,950039</span><span class="sxs-lookup"><span data-stu-id="e1b8d-140">210.950039</span></span> | <span data-ttu-id="e1b8d-141">155,63</span><span class="sxs-lookup"><span data-stu-id="e1b8d-141">155.63</span></span> | <span data-ttu-id="e1b8d-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="e1b8d-142">0.737757626107858</span></span> |
| <span data-ttu-id="e1b8d-143">25-Авг</span><span class="sxs-lookup"><span data-stu-id="e1b8d-143">25-Aug</span></span> | <span data-ttu-id="e1b8d-144">555,950039</span><span class="sxs-lookup"><span data-stu-id="e1b8d-144">555.950039</span></span> | <span data-ttu-id="e1b8d-145">410,17</span><span class="sxs-lookup"><span data-stu-id="e1b8d-145">410.17</span></span> | <span data-ttu-id="e1b8d-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="e1b8d-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="e1b8d-147">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e1b8d-147">Next steps</span></span>

- [<span data-ttu-id="e1b8d-148">Выставление счетов и налоги</span><span class="sxs-lookup"><span data-stu-id="e1b8d-148">Billing and taxes</span></span>](billing.md)
