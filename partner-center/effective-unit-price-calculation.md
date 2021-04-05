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
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374404"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="8a09c-104">Фактическое Вычисление цены за единицу для использования плана Azure</span><span class="sxs-lookup"><span data-stu-id="8a09c-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="8a09c-105">Эффективная цена за единицу</span><span class="sxs-lookup"><span data-stu-id="8a09c-105">The effective unit price</span></span>

<span data-ttu-id="8a09c-106">Эффективная цена за единицу рассчитывается на уровне счетчика (в отличие от уровня ресурса) и корректируется ежедневно в соответствии с использованием счетчика.</span><span class="sxs-lookup"><span data-stu-id="8a09c-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="8a09c-107">Мы вычисляем эффективные цены за единицу, используя следующие три фактора:</span><span class="sxs-lookup"><span data-stu-id="8a09c-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="8a09c-108">Потребление, которое отслеживается ежедневно в рамках цикла выставления счетов</span><span class="sxs-lookup"><span data-stu-id="8a09c-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="8a09c-109">Оплачиваемые затраты для счетчика</span><span class="sxs-lookup"><span data-stu-id="8a09c-109">Billable cost for the meter</span></span>
- <span data-ttu-id="8a09c-110">Распределение по уровням (если применимо)</span><span class="sxs-lookup"><span data-stu-id="8a09c-110">Tiering (if applicable)</span></span>

<span data-ttu-id="8a09c-111">Так как мы отслеживаем ежедневное потребление на протяжении всего цикла выставления счетов, Цена за единицу будет меняться.</span><span class="sxs-lookup"><span data-stu-id="8a09c-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="8a09c-112">Окончательная цена за указанный цикл выставления счетов будет доступна после отключения расчета потребления и закрытия периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="8a09c-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="8a09c-113">Вы увидите большинство изменений в использовании после четвертого или пятого десятичного разряда.</span><span class="sxs-lookup"><span data-stu-id="8a09c-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="8a09c-114">Узнайте, использует ли ваш счетчик многоуровневые цены</span><span class="sxs-lookup"><span data-stu-id="8a09c-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="8a09c-115">Если вы не хотите узнать, использует ли ваш счетчик многоуровневые цены, воспользуйтесь приведенной ниже процедурой.</span><span class="sxs-lookup"><span data-stu-id="8a09c-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="8a09c-116">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8a09c-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="8a09c-117">Выберите **Продажа**, выберите **цены и предложения**, а затем выберите пункт **цены на план Azure**.</span><span class="sxs-lookup"><span data-stu-id="8a09c-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="8a09c-118">Найдите свой счетчик по ИДЕНТИФИКАТОРу, а затем скачайте данные о ценах.</span><span class="sxs-lookup"><span data-stu-id="8a09c-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="8a09c-119">Пример вычисления</span><span class="sxs-lookup"><span data-stu-id="8a09c-119">Sample calculation</span></span>

<span data-ttu-id="8a09c-120">В таблице ниже приведен пример того, как вычисляется эффективная цена за единицу в течение периода открытия.</span><span class="sxs-lookup"><span data-stu-id="8a09c-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="8a09c-121">В таблице применяются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="8a09c-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="8a09c-122">**Up** = Цена за единицу ресурса/час = 0,868</span><span class="sxs-lookup"><span data-stu-id="8a09c-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="8a09c-123">**БКУ** = оплачиваемая единица потребления для счетчика</span><span class="sxs-lookup"><span data-stu-id="8a09c-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="8a09c-124">**BC** = оплачиваемые затраты для счетчика = БКУ \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="8a09c-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="8a09c-125">Это отражает корректировку для скидки с 15% на PEC.</span><span class="sxs-lookup"><span data-stu-id="8a09c-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="8a09c-126">Затем мы используем нижний предел функции, чтобы ограничить значение двумя цифрами после десятичной запятой, чтобы вычислить минимальную сумму.</span><span class="sxs-lookup"><span data-stu-id="8a09c-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="8a09c-127">**Эффективная цена единицы** = БКУ/BC</span><span class="sxs-lookup"><span data-stu-id="8a09c-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="8a09c-128">В этом примере счетчик не имеет уровней цен.</span><span class="sxs-lookup"><span data-stu-id="8a09c-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="8a09c-129">Эффективные коэффициенты цены за единицу в процентах скидки и других корректировках.</span><span class="sxs-lookup"><span data-stu-id="8a09c-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="8a09c-130">Дата</span><span class="sxs-lookup"><span data-stu-id="8a09c-130">Date</span></span> | <span data-ttu-id="8a09c-131">БКУ (оплачиваемая единица потребления)</span><span class="sxs-lookup"><span data-stu-id="8a09c-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="8a09c-132">BC (оплачиваемая стоимость)</span><span class="sxs-lookup"><span data-stu-id="8a09c-132">BC (Billable cost)</span></span> | <span data-ttu-id="8a09c-133">Эффективная цена за единицу</span><span class="sxs-lookup"><span data-stu-id="8a09c-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="8a09c-134">3 — Авг</span><span class="sxs-lookup"><span data-stu-id="8a09c-134">3-Aug</span></span> | <span data-ttu-id="8a09c-135">29</span><span class="sxs-lookup"><span data-stu-id="8a09c-135">29</span></span> | <span data-ttu-id="8a09c-136">21,39</span><span class="sxs-lookup"><span data-stu-id="8a09c-136">21.39</span></span> | <span data-ttu-id="8a09c-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="8a09c-137">0.737586206896552</span></span> |
| <span data-ttu-id="8a09c-138">10 августа</span><span class="sxs-lookup"><span data-stu-id="8a09c-138">10-Aug</span></span> | <span data-ttu-id="8a09c-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="8a09c-139">210.950039</span></span> | <span data-ttu-id="8a09c-140">155,63</span><span class="sxs-lookup"><span data-stu-id="8a09c-140">155.63</span></span> | <span data-ttu-id="8a09c-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="8a09c-141">0.737757626107858</span></span> |
| <span data-ttu-id="8a09c-142">25-Авг</span><span class="sxs-lookup"><span data-stu-id="8a09c-142">25-Aug</span></span> | <span data-ttu-id="8a09c-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="8a09c-143">555.950039</span></span> | <span data-ttu-id="8a09c-144">410,17</span><span class="sxs-lookup"><span data-stu-id="8a09c-144">410.17</span></span> | <span data-ttu-id="8a09c-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="8a09c-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="8a09c-146">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="8a09c-146">Next steps</span></span>

- [<span data-ttu-id="8a09c-147">Выставление счетов и налоги</span><span class="sxs-lookup"><span data-stu-id="8a09c-147">Billing and taxes</span></span>](billing.md)
