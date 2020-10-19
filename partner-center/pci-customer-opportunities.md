---
title: Application Center Insights — отчеты о Клаудасцентии выручки
description: Сведения об отчетах о Клаудасцентии в центре партнеров. Содержит сведения о выручкой клиента для приобретения продуктов Майкрософт.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175287"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="ef292-104">Отчеты о Клаудасцентии доступности, доступные на панели мониторинга центра партнеров</span><span class="sxs-lookup"><span data-stu-id="ef292-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="ef292-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="ef292-105">**Appropriate roles**</span></span>
- <span data-ttu-id="ef292-106">Средство просмотра исполнительных отчетов</span><span class="sxs-lookup"><span data-stu-id="ef292-106">Executive report viewer</span></span>
- <span data-ttu-id="ef292-107">Средство просмотра отчетов</span><span class="sxs-lookup"><span data-stu-id="ef292-107">Report viewer</span></span>

<span data-ttu-id="ef292-108">На панели мониторинга центра партнеров содержатся загружаемые данные о выручкой из программы Клаудасцент.</span><span class="sxs-lookup"><span data-stu-id="ef292-108">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="ef292-109">В данных отображаются сведения о выручкой клиентов для приобретения продуктов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ef292-109">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="ef292-110">В этой статье описывается разбивка этих данных, использование оценки и то, что это значит.</span><span class="sxs-lookup"><span data-stu-id="ef292-110">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="ef292-111">Сводные определения</span><span class="sxs-lookup"><span data-stu-id="ef292-111">Summary definitions</span></span>

- <span data-ttu-id="ef292-112">**Пользователи SMC**— это общее число клиентов в загружаются загрузок.</span><span class="sxs-lookup"><span data-stu-id="ef292-112">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="ef292-113">Клиенты определяются партнером по записи.</span><span class="sxs-lookup"><span data-stu-id="ef292-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="ef292-114">**Соглашения об истечении срока действия**— в пределах текущего финансового года мы предоставляем число соглашений об истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="ef292-114">**Expire Agreements**– within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="ef292-115">**Срок действия дохода**— доход, связанный с соглашениями об истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="ef292-115">**Expiring Revenue**– the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="ef292-116">**Срок действия открытого дохода**— доход, связанный с открытыми соглашениями об истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="ef292-116">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="ef292-118">Сегментация SMB Клаудасцент</span><span class="sxs-lookup"><span data-stu-id="ef292-118">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="ef292-119">Сегмент малого и среднего бизнеса (SMB) дополнительно делится на три отдельных подсегмента.</span><span class="sxs-lookup"><span data-stu-id="ef292-119">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="ef292-120">" **Лучшие неуправляемые** " включает в себя наибольшее число клиентов SMB с наибольшими возможными сделками для Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ef292-120">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="ef292-121">Типичные лучшие неуправляемые клиенты имеют аналогичные характеристики в качестве управляемых учетных записей, с большим количеством сотрудников, большими ИТ бюджетами и расходами, а также большими объемами потенциального дохода корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ef292-121">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="ef292-122">Мы определяем первые неуправляемые два способа:</span><span class="sxs-lookup"><span data-stu-id="ef292-122">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="ef292-123">**Лучшие неуправляемые пользователи**— включает учетные записи с 300 или более сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="ef292-123">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="ef292-124">Учетные записи User-Based — это отличные цели для первого приобретения или расширения таких продуктов, как M365, D365 или Surface.</span><span class="sxs-lookup"><span data-stu-id="ef292-124">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="ef292-125">**Лучшие неуправляемые на основе вычислений** — включает учетные записи с потенциальным объемом Azure более чем на 10 000.</span><span class="sxs-lookup"><span data-stu-id="ef292-125">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="ef292-126">Учетные записи на основе вычислений включают существующий Azure.</span><span class="sxs-lookup"><span data-stu-id="ef292-126">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="ef292-127">учетные записи с значительным годом в будущем и учетными записями, у которых еще нет возможности приобрести Azure, но потенциально могут быть больше, чем на 10 000.</span><span class="sxs-lookup"><span data-stu-id="ef292-127">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="ef292-128">**Компания среднего бизнеса** включает в себя существующих клиентов и учетные записи делового отношения с 25 до 300 сотрудников.</span><span class="sxs-lookup"><span data-stu-id="ef292-128">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="ef292-129">**Малый бизнес** включает в себя все остальные компании, у которых менее 25 сотрудников.</span><span class="sxs-lookup"><span data-stu-id="ef292-129">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

<span data-ttu-id="ef292-131">**Лучшие неуправляемые** и **средние** подсегменты представляют высокие значения времени жизни (ЛТВ) для партнеров Майкрософт и Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ef292-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="ef292-132">Поэтому они являются ведущими областями, влияющими на рост в этом сегменте.</span><span class="sxs-lookup"><span data-stu-id="ef292-132">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="ef292-133">В этих двух подсегментах мы лучше полагаться на приобретение сокета с помощью M365, монетизации в дальнейшем с D365 или бизнес-приложениями Azure, а также реализовать высокий ЛТВ для Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ef292-133">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="ef292-134">Сегодня у нас есть две основные области возможностей — 1.</span><span class="sxs-lookup"><span data-stu-id="ef292-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="ef292-135">Наши клиенты расширяют возможности роста; открыт.</span><span class="sxs-lookup"><span data-stu-id="ef292-135">our customer adds growth; 2.</span></span> <span data-ttu-id="ef292-136">Хотя мы очень хорошо получаем облачные сокеты, ведущие с M365, у нас есть большая возможность в D365 и Azure.</span><span class="sxs-lookup"><span data-stu-id="ef292-136">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="ef292-137">На следующем снимке экрана представлены три подсегмента SMB и оптимизированные маршруты к рынку.</span><span class="sxs-lookup"><span data-stu-id="ef292-137">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="ef292-138">Клаудасцент назначает приоритеты для профилирования, оценки и моделирования всех ведущих неуправляемых и средних бизнес-учетных записей.</span><span class="sxs-lookup"><span data-stu-id="ef292-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="ef292-140">Клаудасцент Машинное обучение</span><span class="sxs-lookup"><span data-stu-id="ef292-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="ef292-141">Протокол SMB использует технологию машинного обучения для управления прогнозами продаж и маркетинга в рамках основных неуправляемых и средних бизнес-сегментов.</span><span class="sxs-lookup"><span data-stu-id="ef292-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="ef292-142">Как собираются и включаются в рекомендации по выручкой?</span><span class="sxs-lookup"><span data-stu-id="ef292-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="ef292-143">**Сбор данных**. веб-обходчики проверяют и собираются миллиарды клиентских сигналов путем проверки связи с доменами компании и мониторинга: публикации в блогах, Пресс-релизы, социальные потоки и технические форумы.</span><span class="sxs-lookup"><span data-stu-id="ef292-143">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="ef292-144">Помимо собранных сигналов фирмографикс сведения собираются из внутренних и внешних источников, таких как D&B, внутренняя подписка Майкрософт и данные о транзакциях.</span><span class="sxs-lookup"><span data-stu-id="ef292-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="ef292-145">**Машинное обучение**. сигналы поступают в модель машинного обучения, которая выводит структурированный набор данных прогнозов продаж и маркетинга для каждого клиента по облачным продуктам и кластерам.</span><span class="sxs-lookup"><span data-stu-id="ef292-145">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="ef292-146">Каждый клиент оценивается с помощью похожих моделей на основные SMB Майкрософт, которые определяют соответствие клиента и алгоритмы машинного обучения, которые интегрируют интерактивное поведение клиента, определяются как намерение.</span><span class="sxs-lookup"><span data-stu-id="ef292-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="ef292-147">Эта оценка объединяется в кластеры, которые показывают, как выделяются покупатели для приобретения Microsoft Cloud продуктов.</span><span class="sxs-lookup"><span data-stu-id="ef292-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="ef292-148">**Оптимизация**. машинное обучение система оптимизирует модели, используя данные транзакций ежемесячно, а данные подписки ежеквартально.</span><span class="sxs-lookup"><span data-stu-id="ef292-148">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="ef292-149">Используя данные выигрыша и потери, Машинное обучение корректирует алгоритмы и проверяет, что модели работают должным образом, сравнивая рекомендации кластера с возможностями, выполненными на главном сервере.</span><span class="sxs-lookup"><span data-stu-id="ef292-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="ef292-151">Клаудасцентие выручки</span><span class="sxs-lookup"><span data-stu-id="ef292-151">CloudAscent Propensity</span></span>

<span data-ttu-id="ef292-152">Как создаются рекомендации по выручкой?</span><span class="sxs-lookup"><span data-stu-id="ef292-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="ef292-153">Используя сигналы, собранные с помощью веб-обходчиков и данных из различных источников, мы консолидируем данные фирмографикс и сигналы социальных сетей клиента.</span><span class="sxs-lookup"><span data-stu-id="ef292-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="ef292-154">Эта оценка использует эти сигналы и данные в моделях сравнения для соответствия и оценки моделей.</span><span class="sxs-lookup"><span data-stu-id="ef292-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="ef292-155">Соответствие учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="ef292-155">Customer Account Fit</span></span>

   - <span data-ttu-id="ef292-156">Внутренние и внешние точки данных, определяющие фирмографикс.</span><span class="sxs-lookup"><span data-stu-id="ef292-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="ef292-157">Оценка соответствия использует ту же модель, что и наш лучший протокол SMB для сравнения клиентов, и позволяет узнать, подходят ли они для Microsoft Cloud продуктов.</span><span class="sxs-lookup"><span data-stu-id="ef292-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="ef292-158">Оценка соответствия обновляется ежеквартально</span><span class="sxs-lookup"><span data-stu-id="ef292-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="ef292-159">Цель учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="ef292-159">Customer Account Intent</span></span>

   - <span data-ttu-id="ef292-160">Сигналы, связанные с социальными носителями и определением поведения клиента в Интернете, определяют намерение.</span><span class="sxs-lookup"><span data-stu-id="ef292-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="ef292-161">Оценка намерения перемещается поверх, чтобы определить кластеры.</span><span class="sxs-lookup"><span data-stu-id="ef292-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="ef292-162">Оценка намерения обновляется ежемесячно.</span><span class="sxs-lookup"><span data-stu-id="ef292-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

3. <span data-ttu-id="ef292-164">Кластеризация</span><span class="sxs-lookup"><span data-stu-id="ef292-164">Clustering</span></span>

   <span data-ttu-id="ef292-165">Сигналы для соответствия и намерения объединяются в оценку кластеризации.</span><span class="sxs-lookup"><span data-stu-id="ef292-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="ef292-166">Клаудасцент имеет четыре кластера:</span><span class="sxs-lookup"><span data-stu-id="ef292-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="ef292-167">Действующие сейчас — клиенты, готовые к продажам</span><span class="sxs-lookup"><span data-stu-id="ef292-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="ef292-168">Оцените клиентов, готовых к маркетингу</span><span class="sxs-lookup"><span data-stu-id="ef292-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="ef292-169">Обучайте — кампании по осведомленности о поддержке дисков</span><span class="sxs-lookup"><span data-stu-id="ef292-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="ef292-170">Обучение — обучение и отслеживание намерения</span><span class="sxs-lookup"><span data-stu-id="ef292-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="ef292-171">Кластеризация позволяет пользователям ориентироваться на конкретные клиенты по продажам и маркетингу на основе коэффициентов сегментов, например: продукта, географической, отрасли и вертикальной.</span><span class="sxs-lookup"><span data-stu-id="ef292-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="ef292-172">На вкладке **модель выручки** в книгах клаудасцент используются общие показатели выручки и предполагаемого пробела.</span><span class="sxs-lookup"><span data-stu-id="ef292-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="ef292-173">Чтобы определить кластеризацию и цель, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="ef292-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="ef292-174">Используя модели машинного обучения, мы сначала Рассчитайте оценку соответствия и оценку намерения заказчика на шкале 100.</span><span class="sxs-lookup"><span data-stu-id="ef292-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="ef292-175">Точные показатели будут зависеть от моделей машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="ef292-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="ef292-176">Пример оценки ниже:</span><span class="sxs-lookup"><span data-stu-id="ef292-176">Example Scores Below:</span></span>

         |<span data-ttu-id="ef292-177">**Классификация**</span><span class="sxs-lookup"><span data-stu-id="ef292-177">**Classification**</span></span>|<span data-ttu-id="ef292-178">**Оценка**</span><span class="sxs-lookup"><span data-stu-id="ef292-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="ef292-179">Высокий</span><span class="sxs-lookup"><span data-stu-id="ef292-179">High</span></span>|<span data-ttu-id="ef292-180">75-100</span><span class="sxs-lookup"><span data-stu-id="ef292-180">75 - 100</span></span>|
         |<span data-ttu-id="ef292-181">Средний</span><span class="sxs-lookup"><span data-stu-id="ef292-181">Medium</span></span>|<span data-ttu-id="ef292-182">55-74</span><span class="sxs-lookup"><span data-stu-id="ef292-182">55 - 74</span></span>|
         |<span data-ttu-id="ef292-183">Низкий</span><span class="sxs-lookup"><span data-stu-id="ef292-183">Low</span></span>|<span data-ttu-id="ef292-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="ef292-184">30 - 54</span></span>|
         |<span data-ttu-id="ef292-185">Очень низкий</span><span class="sxs-lookup"><span data-stu-id="ef292-185">Very Low</span></span>|<span data-ttu-id="ef292-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="ef292-186">0 - 29</span></span>|

      2. <span data-ttu-id="ef292-187">Используя приведенное выше правило, мы будем классифицировать компании как высокие, средние, низкие и очень низкие по отношению к обоим клиентам.</span><span class="sxs-lookup"><span data-stu-id="ef292-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="ef292-188">Мы выводите сигналы соответствия и намерения клиентов по двухмерной матрице с каждым пересечением, представляющим выручкой.</span><span class="sxs-lookup"><span data-stu-id="ef292-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="ef292-189">Например, высокая степень соответствия + высокая цель = a1, представляющая наибольшую степень выручки.</span><span class="sxs-lookup"><span data-stu-id="ef292-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="ef292-190">Наконец, эти сегменты группируются в виде кластеров.</span><span class="sxs-lookup"><span data-stu-id="ef292-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="ef292-191">Например, a1, a2, A3, A4 формируют кластер "подготовить сейчас".</span><span class="sxs-lookup"><span data-stu-id="ef292-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

   <span data-ttu-id="ef292-193">Для этих клиентов рекомендуется ориентироваться на "действовать сейчас" и оценивать клиентов.</span><span class="sxs-lookup"><span data-stu-id="ef292-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="ef292-194">Клаудасцент Products & Models</span><span class="sxs-lookup"><span data-stu-id="ef292-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="ef292-195">На следующем рисунке представлено представление каждой модели выручки в Клаудасцент:</span><span class="sxs-lookup"><span data-stu-id="ef292-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Снимок экрана информационной панели сводки по возможностям клиентов.":::

<span data-ttu-id="ef292-197">Модели пробельных символов состоят из прогнозов для существующих клиентов Майкрософт, где они не имеют продукта и (или) являются клиентами новых перспективных клиентов.</span><span class="sxs-lookup"><span data-stu-id="ef292-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="ef292-198">При продаже моделей используются данные транзакций для прогнозирования потенциальных продаж в Azure и SKU M365.</span><span class="sxs-lookup"><span data-stu-id="ef292-198">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="ef292-199">EOS использует конечные клиенты для Win 7, Office 2010, SQL Server и Windows Server.</span><span class="sxs-lookup"><span data-stu-id="ef292-199">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="ef292-200">Данные EOS извлекаются из MS Sales и перемещаются с моделированием Клаудасцентя, где это возможно.</span><span class="sxs-lookup"><span data-stu-id="ef292-200">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="ef292-201">Данные EOS находятся в современных работах и в продажах Azure.</span><span class="sxs-lookup"><span data-stu-id="ef292-201">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
