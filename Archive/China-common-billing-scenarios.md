---
title: Распространенные сценарии выставления счетов (под управлением 21vianet центра партнеров)
ms.topic: article
ms.date: 10/29/2018
description: В этом разделе рассказывается, что вам следует ожидать увидеть на вашем счете после того, как вы добавите новые подписки, скорректируете количество мест в подписке или отмените подписку.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132344"
---
# <a name="common-billing-scenarios"></a><span data-ttu-id="0dffc-103">Распространенные сценарии выставления счетов</span><span class="sxs-lookup"><span data-stu-id="0dffc-103">Common billing scenarios</span></span>

<span data-ttu-id="0dffc-104">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="0dffc-104">**Applies to**</span></span>

-   <span data-ttu-id="0dffc-105">Центр партнеров, предоставляемый 21Vianet</span><span class="sxs-lookup"><span data-stu-id="0dffc-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="0dffc-106">В этом разделе рассказывается, что вам следует ожидать увидеть на вашем счете после того, как вы добавите новые подписки, скорректируете количество мест в подписке или отмените подписку.</span><span class="sxs-lookup"><span data-stu-id="0dffc-106">This topic explains what you should expect to see on your bill after you add new subscriptions, adjust the number of seats in a subscription, or cancel a subscription.</span></span> 


## <a name="licence-based-billing"></a><span data-ttu-id="0dffc-107">Выставление счетов на основе лицензии</span><span class="sxs-lookup"><span data-stu-id="0dffc-107">Licence-based billing</span></span>


<span data-ttu-id="0dffc-108">Месяцев без изменения подписки на основе лицензии вы увидите элемент строку для каждой подписки в сверочном файле и счета по advance плата за ближайшие месяца.</span><span class="sxs-lookup"><span data-stu-id="0dffc-108">For months without changes to licence-based subscriptions, you'll see a single line item for each subscription on your reconciliation file and invoice for the advance charge for the coming month.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0dffc-109">Сценарий</span><span class="sxs-lookup"><span data-stu-id="0dffc-109">Scenario</span></span></td>
<td><span data-ttu-id="0dffc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0dffc-110">Description</span></span></td>
<td><span data-ttu-id="0dffc-111">Пример</span><span class="sxs-lookup"><span data-stu-id="0dffc-111">Example</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0dffc-112">Новая подписка</span><span class="sxs-lookup"><span data-stu-id="0dffc-112">New subscription</span></span></td>
<td><p><span data-ttu-id="0dffc-113">Период между датой начала подписки и первой датой выставления счетов БЕСПЛАТНЫЙ.</span><span class="sxs-lookup"><span data-stu-id="0dffc-113">The period between the start date of the subscription and the first billing date is FREE.</span></span></p>
<p><span data-ttu-id="0dffc-114">Ваш файл выверки будет содержать один строковый элемент:</span><span class="sxs-lookup"><span data-stu-id="0dffc-114">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="0dffc-115">предоплату за следующий месяц</span><span class="sxs-lookup"><span data-stu-id="0dffc-115">next month's advance charge</span></span></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0dffc-116">Новая подписка: отменена до выставления счета</span><span class="sxs-lookup"><span data-stu-id="0dffc-116">New subscription: cancelled before the billing cut</span></span></td>
<td><span data-ttu-id="0dffc-117">Оплата не будет применяться к учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0dffc-117">Charges will not be applied to the account.</span></span> <span data-ttu-id="0dffc-118">Подписка не отобразится в файле выверки.</span><span class="sxs-lookup"><span data-stu-id="0dffc-118">The subscription won't appear in the reconciliation file.</span></span> <span data-ttu-id="0dffc-119">Это полезно, если вы хотите выполнять тестирование без оплаты расходов на подписку.</span><span class="sxs-lookup"><span data-stu-id="0dffc-119">This is useful if you want to perform testing without incurring subscription charges.</span></span></td>
<td></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0dffc-120">Новая подписка: с корректировкой количества лицензий в течение бесплатного периода</span><span class="sxs-lookup"><span data-stu-id="0dffc-120">New subscription: with licence quantity adjustments during the free period</span></span></td>
<td><p><span data-ttu-id="0dffc-121">Ваш файл выверки будет содержать несколько строковых элементов:</span><span class="sxs-lookup"><span data-stu-id="0dffc-121">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="0dffc-122">изменения количества лицензий по цене 0 за единицу.</span><span class="sxs-lookup"><span data-stu-id="0dffc-122">license quantity changes, charged at 0 Unit Price.</span></span> <span data-ttu-id="0dffc-123">(Оплата за изменение количества мест не взимается во время бесплатного периода);</span><span class="sxs-lookup"><span data-stu-id="0dffc-123">(There is no cost for seat changes during the free period)</span></span></li>
<li><span data-ttu-id="0dffc-124">предоплата за следующий месяц, отражающая новое количество.</span><span class="sxs-lookup"><span data-stu-id="0dffc-124">advance charge for the next month, reflecting the new quantity.</span></span></li>
</ul></td>
<td><span data-ttu-id="0dffc-125">Пропорциональное использование:</span><span class="sxs-lookup"><span data-stu-id="0dffc-125">Prorated usage:</span></span>
<ul>
<li><span data-ttu-id="0dffc-126">С 3 июня по 7 июля за 10 мест = НОЛЬ</span><span class="sxs-lookup"><span data-stu-id="0dffc-126">June 3rd to June 7th for 10 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="0dffc-127">С 8 по 11 июня за 20 мест = НОЛЬ</span><span class="sxs-lookup"><span data-stu-id="0dffc-127">June 8th to June 11th for 20 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="0dffc-128">С 12 по 14 июня за 15 мест = НОЛЬ</span><span class="sxs-lookup"><span data-stu-id="0dffc-128">June 12th to June 14th for 15 seats = ZERO charge</span></span></li>
</ul>
<p><span data-ttu-id="0dffc-129">Вырезать выставления счетов: Плата за целый месяц период с 15 июня перейдите к руководству 14 июля для 15 рабочих мест.</span><span class="sxs-lookup"><span data-stu-id="0dffc-129">Billing cut: Advance charge for the whole month period from June 15th to July 14th for 15 seats.</span></span> <span data-ttu-id="0dffc-130">Если допустить, что плата за подписку составляет 10 долл. США в месяц, общая сумма будет составлять 10 долл. США x 15 мест = 150 долл. США.</span><span class="sxs-lookup"><span data-stu-id="0dffc-130">Assuming the charge per subscription per month is 10 USD, the charge would be 10 USD x 15 seats = 150 USD.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0dffc-131">Существующей подписки: Увеличение или уменьшение количества лицензий</span><span class="sxs-lookup"><span data-stu-id="0dffc-131">Existing subscription: Increase or decrease in licence quantity</span></span></td>
<td><p><span data-ttu-id="0dffc-132">Ваш файл выверки будет содержать несколько строковых элементов:</span><span class="sxs-lookup"><span data-stu-id="0dffc-132">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="0dffc-133">возврат досрочного платежа</span><span class="sxs-lookup"><span data-stu-id="0dffc-133">the advance charge reversal</span></span></li>
<li><span data-ttu-id="0dffc-134">плата за пропорциональное использование</span><span class="sxs-lookup"><span data-stu-id="0dffc-134">prorated usage charges</span></span></li>
<li><span data-ttu-id="0dffc-135">предоплату за следующий месяц</span><span class="sxs-lookup"><span data-stu-id="0dffc-135">next month's advance charge</span></span></li>
</ul></td>
<td><p><span data-ttu-id="0dffc-136">Пропорциональное использование:</span><span class="sxs-lookup"><span data-stu-id="0dffc-136">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="0dffc-137">С 15 по 19 июля за 15 мест = 26,61 долл. США</span><span class="sxs-lookup"><span data-stu-id="0dffc-137">July 15th to July 19th for 15 seats = 26.61 USD</span></span></li>
<li><span data-ttu-id="0dffc-138">С 20 по 30 июля за 12 мест = 46,84 долл. США</span><span class="sxs-lookup"><span data-stu-id="0dffc-138">July 20th to July 30th for 12 seats = 46.84 USD</span></span></li>
<li><span data-ttu-id="0dffc-139">С 31 июля по 9 августа за 18 мест = 63,87 долл. США</span><span class="sxs-lookup"><span data-stu-id="0dffc-139">July 31st to August 9th for 18 seats = 63.87 USD</span></span></li>
<li><span data-ttu-id="0dffc-140">С 10 по 14 августа за 10 мест = 17,74 долл. США</span><span class="sxs-lookup"><span data-stu-id="0dffc-140">August 10th to August 14th for 10 seats = 17.74 USD</span></span></li>
</ul>
<span data-ttu-id="0dffc-141">Возврат досрочного платежа за целый месяц с 15 июля по 14 августа = -165 долл. США.</span><span class="sxs-lookup"><span data-stu-id="0dffc-141">Reversal of the advance charge for the whole month period from July 15th to August 14th = -165 USD.</span></span>
<p><span data-ttu-id="0dffc-142">Вырезать выставления счетов: Плата за целый месяц период с 15 августа перейдите к руководству 14 сентября для 10 рабочих мест = 110 долл. США.</span><span class="sxs-lookup"><span data-stu-id="0dffc-142">Billing cut: Advance charge for the whole month period from August 15th to September 14th for 10 seats = 110 USD.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0dffc-143">Отмена: без предварительного изменения мест</span><span class="sxs-lookup"><span data-stu-id="0dffc-143">Cancellation: no prior seat changes</span></span></td>
<td><p><span data-ttu-id="0dffc-144">Ваш файл выверки будет содержать один строковый элемент:</span><span class="sxs-lookup"><span data-stu-id="0dffc-144">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="0dffc-145">Кредит за неиспользованные дни, поскольку счет за весь период был выставлен заранее в предыдущем сводном счете.</span><span class="sxs-lookup"><span data-stu-id="0dffc-145">A credit for unused days, because the whole period was billed in advance in the previous billing statement.</span></span> <span data-ttu-id="0dffc-146">Он рассчитывается на основании даты окончания подписки.</span><span class="sxs-lookup"><span data-stu-id="0dffc-146">This is calculated based on the Subscription End date.</span></span></li>
</ul></td>
<td><span data-ttu-id="0dffc-147">Ранее взимается плата advance: 15 августа, чтобы 14 сентября, 10 рабочих мест = 100 долларов США.</span><span class="sxs-lookup"><span data-stu-id="0dffc-147">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="0dffc-148">Потребленная часть досрочного платежа с 15 по 24 августа.</span><span class="sxs-lookup"><span data-stu-id="0dffc-148">Consumed portion of the advance charge from August 15th to August 24th.</span></span></p>
<p><span data-ttu-id="0dffc-149">Кредит для неиспользуемых дней: 25 августа, чтобы 14 сентября, 10 рабочих мест =-74.51.</span><span class="sxs-lookup"><span data-stu-id="0dffc-149">Credit for unused days: August 25th to September 14th for 10 seats = -74.51.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0dffc-150">Отмена: с предварительным изменением мест</span><span class="sxs-lookup"><span data-stu-id="0dffc-150">Cancellation: with prior seat changes</span></span></td>
<td><p><span data-ttu-id="0dffc-151">Ваш файл выверки будет содержать несколько строковых элементов:</span><span class="sxs-lookup"><span data-stu-id="0dffc-151">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="0dffc-152">возврат досрочного платежа</span><span class="sxs-lookup"><span data-stu-id="0dffc-152">the advance charge reversal</span></span></li>
<li><span data-ttu-id="0dffc-153">плата за пропорциональное использование</span><span class="sxs-lookup"><span data-stu-id="0dffc-153">prorated usage charges</span></span></li>
<li><span data-ttu-id="0dffc-154">кредит за неиспользуемые дни</span><span class="sxs-lookup"><span data-stu-id="0dffc-154">a credit for any unused days</span></span></li>
</ul></td>
<td><span data-ttu-id="0dffc-155">Ранее взимается плата advance: 15 августа, чтобы 14 сентября, 10 рабочих мест = 100 долларов США.</span><span class="sxs-lookup"><span data-stu-id="0dffc-155">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="0dffc-156">Пропорциональное использование:</span><span class="sxs-lookup"><span data-stu-id="0dffc-156">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="0dffc-157">С 15 по 24-го августа для 10 мест</span><span class="sxs-lookup"><span data-stu-id="0dffc-157">August 15th to August 24th for 10 seats</span></span></li>
<li><span data-ttu-id="0dffc-158">С 25 августа по 14 сентября за 5 мест</span><span class="sxs-lookup"><span data-stu-id="0dffc-158">August 25th to September 14th for 5 seats</span></span></li>
</ul>
<p><span data-ttu-id="0dffc-159">Кредит для неиспользуемых дней: 1 сентября для 14 сентября для 5 рабочих мест.</span><span class="sxs-lookup"><span data-stu-id="0dffc-159">Credit for unused days: September 1st to September 14th for 5 seats.</span></span></p>
<p><span data-ttu-id="0dffc-160">Возврат досрочного платежа за целый месяц с 15 августа по 14 сентября = -100 долл. США.</span><span class="sxs-lookup"><span data-stu-id="0dffc-160">Reversal of the advance charge for the whole month period from August 15th to September 14th = -100 USD.</span></span></p></td>
</tr>
</tbody>
</table>
