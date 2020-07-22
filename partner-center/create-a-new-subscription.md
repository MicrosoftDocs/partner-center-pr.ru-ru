---
title: Создание клиентских подписок в центре партнеров
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как продавать подписки клиентов на продукты, опубликованные корпорацией Майкрософт, а также продукты SaaS, опубликованные сторонними поставщиками программного обеспечения.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: e72c499cac9b2408e34a0f6fbf2e442f93faef47
ms.sourcegitcommit: 54f823f0e02e0e7add737d78de74d8eba8d9f381
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "86875230"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="ed87a-103">Создание, приостановка и отмена подписок клиентов</span><span class="sxs-lookup"><span data-stu-id="ed87a-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="ed87a-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="ed87a-104">**Applies to**</span></span>

- <span data-ttu-id="ed87a-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="ed87a-105">Partner Center</span></span>
- <span data-ttu-id="ed87a-106">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="ed87a-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="ed87a-107">Партнеры CSP</span><span class="sxs-lookup"><span data-stu-id="ed87a-107">CSP partners</span></span>

<span data-ttu-id="ed87a-108">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="ed87a-108">**Appropriate roles**</span></span>

- <span data-ttu-id="ed87a-109">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="ed87a-109">Admin agent</span></span>
- <span data-ttu-id="ed87a-110">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="ed87a-110">Billing admin</span></span>
- <span data-ttu-id="ed87a-111">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ed87a-111">Global admin</span></span>
- <span data-ttu-id="ed87a-112">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="ed87a-112">Helpdesk agent</span></span>
- <span data-ttu-id="ed87a-113">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="ed87a-113">Sales agent</span></span>

<span data-ttu-id="ed87a-114">После регистрации клиентов в Центре партнеров можно продать им подписки на продукты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ed87a-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="ed87a-115">Сюда входят продукты, опубликованные корпорацией Майкрософт, а также продукты SaaS (программное обеспечение как услуга), опубликованные сторонними поставщиками программного обеспечения (ISV) для [коммерческого рынка](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="ed87a-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="ed87a-116">Некоторые предложения ограничены одной подпиской на каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="ed87a-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="ed87a-117">Чтобы просмотреть список ограниченных предложений, посетите страницу "Цены и предложения" в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ed87a-118">Как партнер в программе CSP, вы можете приобрести подписки SaaS **на основе лицензий** только от издателей ISV в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="ed87a-119">Это означает, что вы можете приобрести любое предложение SaaS **на основе лицензий** . издатель ISV стал доступным вам, включая [исключительные предложения](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , к которым у вас есть доступ.</span><span class="sxs-lookup"><span data-stu-id="ed87a-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="ed87a-120">Для приобретения или управления другими, коммерческими предложениями от независимых поставщиков программных продуктов (например, **на основе использования**, лимитных или на основе потребления, включающих приложения Azure, контейнеры или виртуальные машины), необходимо посетить [портал управления Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ed87a-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="ed87a-121">Дополнительные сведения см. в статье [приобретение продуктов для коммерческого рынка](csp-commercial-marketplace-purchase.md).</span><span class="sxs-lookup"><span data-stu-id="ed87a-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="ed87a-122">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="ed87a-122">Create a new subscription</span></span>

1. <span data-ttu-id="ed87a-123">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="ed87a-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ed87a-124">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ed87a-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ed87a-125">Выберите **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-125">Select **Add subscription**.</span></span> <span data-ttu-id="ed87a-126">На вкладке " **веб-службы** " будут показаны все доступные предложения SaaS Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ed87a-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="ed87a-127">Чтобы просмотреть только определенные типы подписок, сделайте выбор в доступных фильтрах:</span><span class="sxs-lookup"><span data-stu-id="ed87a-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="ed87a-128">**Издатель**: выберите **Майкрософт** , чтобы просмотреть только предложения от корпорации Майкрософт или **партнера** , чтобы просмотреть продукты коммерческого рынка, опубликованные независимыми поставщиками программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="ed87a-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="ed87a-129">**Тип выставления счетов**: выберите тип оплаты по подписке, который вы хотите использовать: **Лицензия** или **Использование**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="ed87a-130">В разделе [Вопросы и ответы по новым возможностям выставления счетов](faq-about-new-billing-features.md) предоставлены сведения, которые помогут выбрать удобную периодичность выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ed87a-130">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="ed87a-131">**Категория**: выберите **предприятие**, **малый бизнес**или **пробная версия**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="ed87a-132">Дополнительные сведения о пробных подписках см. в разделе [Предложение клиентам пробных версий продуктов Майкрософт](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="ed87a-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="ed87a-133">Выберите подписки на продукт, которые вы хотите приобрести для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed87a-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="ed87a-134">Отображаемые продукты зависят от типа сегмента клиента (образование, правительственные учреждения и т. д.) и примененных фильтров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="ed87a-135">Некоторые предложения, отображаемые в Marketplace, могут не всегда быть доступны конкретному клиенту или определенному партнеру CSP.</span><span class="sxs-lookup"><span data-stu-id="ed87a-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="ed87a-136">Это может быть вызвано:</span><span class="sxs-lookup"><span data-stu-id="ed87a-136">This can be because:</span></span>

   - <span data-ttu-id="ed87a-137">У клиента уже есть подписка на этот продукт, и допускается только один</span><span class="sxs-lookup"><span data-stu-id="ed87a-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="ed87a-138">Возможно, подписка клиента приостановлена (в этом случае вы можете повторно активировать подписку, а не приобрести новую).</span><span class="sxs-lookup"><span data-stu-id="ed87a-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="ed87a-139">Для предложений SaaS ISV может быть несколько причин, по которым предложение недоступно для приобретения. независимого поставщика программного обеспечения может не поддерживать страну или регион выставления счетов. возможно, ISV не сделает предложение доступным через программу CSP. или независимый поставщик программного обеспечения может сделать предложение [эксклюзивным](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) только определенным партнерам CSP.</span><span class="sxs-lookup"><span data-stu-id="ed87a-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="ed87a-140">Предложение ISV также может быть недоступно для языка в центре партнеров (например, в контейнерах или в некоторых предложениях на основе использования).</span><span class="sxs-lookup"><span data-stu-id="ed87a-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="ed87a-141">Для каждой подписки, которую необходимо добавить, введите число лицензий (если необходимо) и выберите **Добавить в корзину**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="ed87a-142">По завершении добавления подписок выберите **Проверка** и проверьте свой заказ.</span><span class="sxs-lookup"><span data-stu-id="ed87a-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="ed87a-143">После рассмотрения заказов и готовности приобрести эти подписки выберите **купить**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="ed87a-144">После приобретения подписки для клиента произойдет следующее:</span><span class="sxs-lookup"><span data-stu-id="ed87a-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="ed87a-145">Чтобы проверить или изменить подписку, выберите имя подписки на странице **подписки** этого клиента.</span><span class="sxs-lookup"><span data-stu-id="ed87a-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="ed87a-146">Здесь можно выбрать дополнительные лицензии, если они доступны, изменить количество лицензий или приостановить подписку.</span><span class="sxs-lookup"><span data-stu-id="ed87a-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="ed87a-147">**Для подписок ISV (на основе лицензий):**</span><span class="sxs-lookup"><span data-stu-id="ed87a-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="ed87a-148">Вы получите ссылку на сайт издателя ISV.</span><span class="sxs-lookup"><span data-stu-id="ed87a-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="ed87a-149">Эта ссылка поможет вам завершить настройку развертывания или учетной записи для подписки клиента.</span><span class="sxs-lookup"><span data-stu-id="ed87a-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="ed87a-150">Ни вы, ни клиент не получит сообщение электронной почты с инструкциями по завершению настройки или подготовки учетной записи для этого типа подписки ISV.)</span><span class="sxs-lookup"><span data-stu-id="ed87a-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="ed87a-151">Если ваша подписка поставляется с 30-дневной бесплатной пробной версией, бесплатный пробный период будет применен автоматически.</span><span class="sxs-lookup"><span data-stu-id="ed87a-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="ed87a-152">Как партнер в программе CSP вы не можете отказаться от использования бесплатного пробного периода на предложениях, приобретенных для клиентов.</span><span class="sxs-lookup"><span data-stu-id="ed87a-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="ed87a-153">По окончании бесплатного пробного периода срок действия подписки начнется, а подписка будет преобразована в состояние оплачена.</span><span class="sxs-lookup"><span data-stu-id="ed87a-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="ed87a-154">Подписка будет обновляться в соответствии с тем же расписанием.</span><span class="sxs-lookup"><span data-stu-id="ed87a-154">The subscription will then autorenew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="ed87a-155">Обновление подписок с помощью надстроек</span><span class="sxs-lookup"><span data-stu-id="ed87a-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="ed87a-156">Чтобы приобрести надстройку, клиент должен сначала получить активную базовую подписку.</span><span class="sxs-lookup"><span data-stu-id="ed87a-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="ed87a-157">Вы не можете приобретать надстройки через каталог.</span><span class="sxs-lookup"><span data-stu-id="ed87a-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="ed87a-158">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ed87a-159">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ed87a-159">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ed87a-160">Выберите подписку, которую необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="ed87a-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="ed87a-161">Под разделом **состояние** представлен список доступных надстроек для подписки.</span><span class="sxs-lookup"><span data-stu-id="ed87a-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="ed87a-162">Обновите количество лицензий для каждой обязательной надстройки.</span><span class="sxs-lookup"><span data-stu-id="ed87a-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="ed87a-163">Затем **отправьте** изменения.</span><span class="sxs-lookup"><span data-stu-id="ed87a-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="ed87a-164">Возможность приобретения надстроек через центр партнеров доступна только для партнеров CSP.</span><span class="sxs-lookup"><span data-stu-id="ed87a-164">The ability to purchase add-ons through Partner Center is only available to CSP partners.</span></span>
<span data-ttu-id="ed87a-165">На основе базовых требований и региональных доступности отображаются только доступные надстройки.</span><span class="sxs-lookup"><span data-stu-id="ed87a-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="ed87a-166">Дополнительные сведения о ценах и предложениях см. в этой матрице.</span><span class="sxs-lookup"><span data-stu-id="ed87a-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="ed87a-167">Приостановка базовой подписки также приведет к приостановке всех связанных надстроек.</span><span class="sxs-lookup"><span data-stu-id="ed87a-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="ed87a-168">Даты начала для надстроек совпадают с базовой подпиской, а расходы рассчитываются с учетом даты начала и окончания оплаты за Pro-Рата в первой счете.</span><span class="sxs-lookup"><span data-stu-id="ed87a-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> 


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="ed87a-169">Приостановка и отмена подписки</span><span class="sxs-lookup"><span data-stu-id="ed87a-169">Suspend or cancel a subscription</span></span>

<span data-ttu-id="ed87a-170">Партнеры могут приостановить или отменить подписку по просьбе клиента либо в случаях неплатежа или мошенничества.</span><span class="sxs-lookup"><span data-stu-id="ed87a-170">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="ed87a-171">Приостановка подписки</span><span class="sxs-lookup"><span data-stu-id="ed87a-171">Suspend a subscription</span></span>

<span data-ttu-id="ed87a-172">При изменении статуса подписки на **Приостановленная** пользователи не смогут входить в систему или получать доступ к службам.</span><span class="sxs-lookup"><span data-stu-id="ed87a-172">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="ed87a-173">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-173">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ed87a-174">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ed87a-174">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ed87a-175">Выберите подписку, которую необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="ed87a-175">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="ed87a-176">В разделе **Состояние** выберите **Приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-176">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="ed87a-177">Затем **отправьте** изменения.</span><span class="sxs-lookup"><span data-stu-id="ed87a-177">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="ed87a-178">Все данные будут удалены, если подписка не будет повторно активирована в течение 90 дней, либо 90 дней плюс количество дней от момента открытия учетной записи до первого периода выставления счетов (не более 120 дней).</span><span class="sxs-lookup"><span data-stu-id="ed87a-178">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="ed87a-179">При приостановке подписки дата, отображаемая под кнопкой **Приостановлено**, указывает, когда автоматически истечет срок действия подписки, если вы не активируете ее повторно.</span><span class="sxs-lookup"><span data-stu-id="ed87a-179">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="ed87a-180">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="ed87a-180">Cancel a subscription</span></span>

<span data-ttu-id="ed87a-181">Вы можете отменить подписки SaaS на основе лицензий сторонних издателей программного обеспечения в [коммерческом рынке](csp-commercial-marketplace-overview.md)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-181">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="ed87a-182">При условии отмены в течение периода отмены вы получите полный возмещение.</span><span class="sxs-lookup"><span data-stu-id="ed87a-182">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="ed87a-183">Для ISV предлагает ежемесячные счета:</span><span class="sxs-lookup"><span data-stu-id="ed87a-183">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="ed87a-184">Если после размещения заказа вы отменили менее 24 часов, вы получите полный кредит для следующего счета.</span><span class="sxs-lookup"><span data-stu-id="ed87a-184">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="ed87a-185">Если после размещения заказа вы отменили позже, чем через 24 часа, отмена будет запланирована на момент обновления.</span><span class="sxs-lookup"><span data-stu-id="ed87a-185">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="ed87a-186">Для предложений, которые выставляются ежегодно:</span><span class="sxs-lookup"><span data-stu-id="ed87a-186">For offers billed annually:</span></span>

- <span data-ttu-id="ed87a-187">Если после появления заказа вы отменили менее 14 дней, вы получите полный кредит для следующего счета.</span><span class="sxs-lookup"><span data-stu-id="ed87a-187">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="ed87a-188">Если вы отменили позже через 14 дней после размещения заказа, то отмена будет запланирована при обновлении.</span><span class="sxs-lookup"><span data-stu-id="ed87a-188">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="ed87a-189">После выполнения этих периодов больше не будет отображаться возможность отмены подписки.</span><span class="sxs-lookup"><span data-stu-id="ed87a-189">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="ed87a-190">Службы независимых поставщиков программного обеспечения (например, использующие виртуальные машины или контейнеры) не могут возвращать данные на основе использования и измерения.</span><span class="sxs-lookup"><span data-stu-id="ed87a-190">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="ed87a-191">В качестве метода отмены можно отменить подготовку служб на основе использования.</span><span class="sxs-lookup"><span data-stu-id="ed87a-191">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="ed87a-192">Так как плата взимается за использование, эти службы не могут получить возмещение.</span><span class="sxs-lookup"><span data-stu-id="ed87a-192">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="ed87a-193">Чтобы отменить подписку SaaS на основе лицензий от издателя ISV, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="ed87a-193">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="ed87a-194">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ed87a-195">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ed87a-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ed87a-196">Выберите подписку, которую нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="ed87a-196">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="ed87a-197">В столбце **состояние** выберите **Отмена**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-197">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="ed87a-198">Затем **отправьте** изменения.</span><span class="sxs-lookup"><span data-stu-id="ed87a-198">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="ed87a-199">Если появится диалоговое окно, заполните все необходимые сведения и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-199">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="ed87a-200">Чтобы подтвердить отмену, выберите **Да, отмена**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-200">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="ed87a-201">Вы также можете отменить подписку Azure Marketplace с помощью интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="ed87a-201">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="ed87a-202">Дополнительные сведения см. в разделе [Отмена подписки Azure Marketplace](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="ed87a-202">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="ed87a-203">Выберите, следует ли автоматически продлить подписку на продукты коммерческого Marketplace</span><span class="sxs-lookup"><span data-stu-id="ed87a-203">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="ed87a-204">По умолчанию активные подписки настроены на автоматическое продление по истечении периода действия подписки.</span><span class="sxs-lookup"><span data-stu-id="ed87a-204">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="ed87a-205">Для [подписок на коммерческие продукты Marketplace](csp-commercial-marketplace-overview.md)можно дополнительно отказаться от автоматического продления подписки.</span><span class="sxs-lookup"><span data-stu-id="ed87a-205">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="ed87a-206">Чтобы отключить автоматическое продление действующей подписки на коммерческий рынок, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="ed87a-206">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="ed87a-207">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed87a-207">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ed87a-208">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ed87a-208">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ed87a-209">Выберите **Подписки**.</span><span class="sxs-lookup"><span data-stu-id="ed87a-209">Select **Subscriptions**.</span></span> <span data-ttu-id="ed87a-210">Здесь перечислены все подписки на основе лицензий, приобретенные для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed87a-210">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="ed87a-211">В столбце **Подписка** выберите подписку, которую необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="ed87a-211">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="ed87a-212">На странице сведения о подписке выберите раздел **состояние** и снимите флажок **Auto-продление** .</span><span class="sxs-lookup"><span data-stu-id="ed87a-212">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="ed87a-213">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="ed87a-213">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ed87a-214">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ed87a-214">Next steps</span></span>

- [<span data-ttu-id="ed87a-215">Приобретение продуктов коммерческого Marketplace для клиентов</span><span class="sxs-lookup"><span data-stu-id="ed87a-215">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="ed87a-216">Управляйте продуктами коммерческих рынков для своих клиентов</span><span class="sxs-lookup"><span data-stu-id="ed87a-216">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="ed87a-217">Обзор коммерческой платформы</span><span class="sxs-lookup"><span data-stu-id="ed87a-217">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
