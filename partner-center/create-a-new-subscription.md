---
title: Создание клиентских подписок в центре партнеров
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как продавать подписки клиентам о продуктах, опубликованных корпорацией Майкрософт, а также о продуктах SaaS, опубликованных сторонними поставщиками программного обеспечения.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201414"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="d343d-103">Создание, приостановка и отмена подписок клиентов</span><span class="sxs-lookup"><span data-stu-id="d343d-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="d343d-104">Область **применения**: центр партнеров | Центр партнеров по Microsoft Cloud для государственных организаций США</span><span class="sxs-lookup"><span data-stu-id="d343d-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d343d-105">**Соответствующие роли**: Агент администрирования | Администратор выставления счетов | Глобальный администратор | Агент службы технической поддержки | Агент продаж</span><span class="sxs-lookup"><span data-stu-id="d343d-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="d343d-106">После регистрации клиентов в Центре партнеров можно продать им подписки на продукты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d343d-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="d343d-107">Сюда входят продукты, опубликованные корпорацией Майкрософт и программным обеспечением как услуга (SaaS), опубликованные сторонними поставщиками программного обеспечения (ISV) на [коммерческом рынке](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="d343d-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="d343d-108">Некоторые предложения ограничены одной подпиской на каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="d343d-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="d343d-109">Чтобы просмотреть список ограниченных предложений, посетите страницу "Цены и предложения" в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="d343d-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d343d-110">Как партнер в программе CSP, вы можете приобрести подписки **на основе лицензий** или **лимитного использования** SaaS от издателей независимых поставщиков программного обеспечения в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="d343d-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="d343d-111">Это означает, что вы можете приобрести любое предложение, **основанное на лицензиях** , или **лимитное** SaaS, который издатель ISV сделал доступным, включая [исключительные предложения](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , к которым у вас есть доступ.</span><span class="sxs-lookup"><span data-stu-id="d343d-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="d343d-112">Для приобретения или управления другими, коммерческими предложениями из независимых поставщиков программных продуктов (таких как предложения на основе использования, включающие приложения Azure, контейнеры или виртуальные машины) необходимо переходить на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d343d-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="d343d-113">Все даты и время в центре партнеров задаются по стандарту Всемирного времени (UTC).</span><span class="sxs-lookup"><span data-stu-id="d343d-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="d343d-114">Это может отличаться от местного времени до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="d343d-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="d343d-115">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="d343d-115">Create a new subscription</span></span>

1. <span data-ttu-id="d343d-116">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d343d-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d343d-117">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="d343d-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d343d-118">Выберите **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="d343d-118">Select **Add subscription**.</span></span> <span data-ttu-id="d343d-119">На вкладке " **веб-службы** " будут показаны все доступные предложения SaaS Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d343d-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="d343d-120">Чтобы просмотреть только определенные типы подписок, сделайте выбор в доступных фильтрах:</span><span class="sxs-lookup"><span data-stu-id="d343d-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="d343d-121">**Издатель**: выберите **Майкрософт** , чтобы просмотреть только предложения от корпорации Майкрософт или **партнера** , чтобы просмотреть продукты коммерческого рынка, опубликованные независимыми поставщиками программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="d343d-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="d343d-122">**Тип выставления счетов**: выберите тип оплаты по подписке, который вы хотите использовать: **Лицензия** или **Использование**.</span><span class="sxs-lookup"><span data-stu-id="d343d-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="d343d-123">Сведения, которые помогут выбрать месячную и ежегодную частоту выставления счетов, см. в разделе [выставление счетов на основе лицензий](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="d343d-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="d343d-124">**Категория**: выберите **предприятие**, **малый бизнес** или **пробная версия**.</span><span class="sxs-lookup"><span data-stu-id="d343d-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="d343d-125">Дополнительные сведения о пробных подписках см. в разделе [Предложение клиентам пробных версий продуктов Майкрософт](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="d343d-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="d343d-126">Выберите подписки на продукт, которые вы хотите приобрести для клиента.</span><span class="sxs-lookup"><span data-stu-id="d343d-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="d343d-127">Отображаемые продукты зависят от типа сегмента клиента (образование, правительственные учреждения и т. д.) и примененных фильтров.</span><span class="sxs-lookup"><span data-stu-id="d343d-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="d343d-128">Некоторые предложения, отображаемые в Marketplace, могут не всегда быть доступны конкретному клиенту или определенному партнеру CSP.</span><span class="sxs-lookup"><span data-stu-id="d343d-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="d343d-129">Это может быть вызвано:</span><span class="sxs-lookup"><span data-stu-id="d343d-129">This can be because:</span></span>

   - <span data-ttu-id="d343d-130">У клиента уже есть подписка на этот продукт, и допускается только один</span><span class="sxs-lookup"><span data-stu-id="d343d-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="d343d-131">Возможно, подписка клиента приостановлена (в этом случае вы можете повторно активировать подписку, а не приобрести новую).</span><span class="sxs-lookup"><span data-stu-id="d343d-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="d343d-132">Для предложений SaaS ISV может быть несколько причин, по которым предложение недоступно для приобретения. независимого поставщика программного обеспечения может не поддерживать страну или регион выставления счетов. возможно, ISV не сделает предложение доступным через программу CSP. или независимый поставщик программного обеспечения может сделать предложение [эксклюзивным](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) только определенным партнерам CSP.</span><span class="sxs-lookup"><span data-stu-id="d343d-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="d343d-133">Предложение ISV также может быть недоступно для языка в центре партнеров (например, в контейнерах или в некоторых предложениях на основе использования).</span><span class="sxs-lookup"><span data-stu-id="d343d-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="d343d-134">Для каждой подписки, которую необходимо добавить, введите число лицензий (если необходимо) и выберите **Добавить в корзину**.</span><span class="sxs-lookup"><span data-stu-id="d343d-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="d343d-135">По завершении добавления подписок выберите **Проверка** и проверьте свой заказ.</span><span class="sxs-lookup"><span data-stu-id="d343d-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="d343d-136">После рассмотрения заказов и готовности приобрести эти подписки выберите **купить**.</span><span class="sxs-lookup"><span data-stu-id="d343d-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="d343d-137">После приобретения подписки для клиента произойдет следующее:</span><span class="sxs-lookup"><span data-stu-id="d343d-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="d343d-138">Чтобы проверить или изменить подписку, выберите имя подписки на странице **подписки** этого клиента.</span><span class="sxs-lookup"><span data-stu-id="d343d-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="d343d-139">Здесь можно выбрать дополнительные лицензии, если они доступны, изменить количество лицензий или приостановить подписку.</span><span class="sxs-lookup"><span data-stu-id="d343d-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="d343d-140">**Для подписок ISV (на основе лицензий и с оплатой):**</span><span class="sxs-lookup"><span data-stu-id="d343d-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="d343d-141">Вы получите ссылку на сайт издателя ISV.</span><span class="sxs-lookup"><span data-stu-id="d343d-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="d343d-142">Эта ссылка поможет вам завершить настройку развертывания или учетной записи для подписки клиента.</span><span class="sxs-lookup"><span data-stu-id="d343d-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="d343d-143">Ни вы, ни клиент не получит сообщение электронной почты с инструкциями по завершению настройки или подготовки учетной записи для этого типа подписки ISV.)</span><span class="sxs-lookup"><span data-stu-id="d343d-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="d343d-144">Если ваша подписка поставляется с 30-дневной бесплатной пробной версией, бесплатный пробный период будет применен автоматически.</span><span class="sxs-lookup"><span data-stu-id="d343d-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="d343d-145">Как партнер в программе CSP вы не можете отказаться от использования бесплатного пробного периода на предложениях, приобретенных для клиентов.</span><span class="sxs-lookup"><span data-stu-id="d343d-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="d343d-146">По окончании бесплатного пробного периода срок действия подписки начнется, а подписка будет преобразована в состояние оплачена.</span><span class="sxs-lookup"><span data-stu-id="d343d-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="d343d-147">Подписка будет обновлена в соответствии с тем же расписанием.</span><span class="sxs-lookup"><span data-stu-id="d343d-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="d343d-148">Обновление подписок с помощью подписок</span><span class="sxs-lookup"><span data-stu-id="d343d-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="d343d-149">Чтобы приобрести надстройку, у клиента должна быть активная базовая подписка.</span><span class="sxs-lookup"><span data-stu-id="d343d-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="d343d-150">Приобретение надстроек через каталог невозможно.</span><span class="sxs-lookup"><span data-stu-id="d343d-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="d343d-151">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d343d-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d343d-152">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="d343d-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d343d-153">Выберите подписку, которую необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="d343d-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d343d-154">Под разделом **состояние** представлен список доступных надстроек для подписки.</span><span class="sxs-lookup"><span data-stu-id="d343d-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="d343d-155">Обновите количество лицензий для каждой обязательной надстройки.</span><span class="sxs-lookup"><span data-stu-id="d343d-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="d343d-156">Затем **отправьте** изменения.</span><span class="sxs-lookup"><span data-stu-id="d343d-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="d343d-157">Возможность приобретения надстроек через центр партнеров доступна только для прямых и косвенных поставщиков.</span><span class="sxs-lookup"><span data-stu-id="d343d-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="d343d-158">На основе базовых требований и региональных доступности отображаются только доступные надстройки.</span><span class="sxs-lookup"><span data-stu-id="d343d-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="d343d-159">Дополнительные сведения о ценах и предложениях см. в этой матрице.</span><span class="sxs-lookup"><span data-stu-id="d343d-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="d343d-160">Приостановка базовой подписки также приведет к приостановке всех связанных надстроек.</span><span class="sxs-lookup"><span data-stu-id="d343d-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="d343d-161">Даты начала для надстроек совпадают с датой базовой подписки, а плата рассчитывается на основе даты начала и даты окончания платежей с пропорциональными затратами в первой накладной.</span><span class="sxs-lookup"><span data-stu-id="d343d-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="d343d-162">Дополнительные сведения см. в разделе [выставление счетов на основе лицензий](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="d343d-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="d343d-163">Приостановка и отмена подписки</span><span class="sxs-lookup"><span data-stu-id="d343d-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="d343d-164">Партнеры могут приостановить или отменить подписку по просьбе клиента либо в случаях неплатежа или мошенничества.</span><span class="sxs-lookup"><span data-stu-id="d343d-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="d343d-165">Приостановка подписки</span><span class="sxs-lookup"><span data-stu-id="d343d-165">Suspend a subscription</span></span>

<span data-ttu-id="d343d-166">При изменении статуса подписки на **Приостановленная** пользователи не смогут входить в систему или получать доступ к службам.</span><span class="sxs-lookup"><span data-stu-id="d343d-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="d343d-167">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d343d-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d343d-168">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="d343d-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d343d-169">Выберите подписку, которую необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="d343d-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d343d-170">В разделе **Состояние** выберите **Приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="d343d-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="d343d-171">Затем **отправьте** изменения.</span><span class="sxs-lookup"><span data-stu-id="d343d-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d343d-172">Все данные будут удалены, если подписка не будет повторно активирована в течение 90 дней, либо 90 дней плюс количество дней от момента открытия учетной записи до первого периода выставления счетов (не более 120 дней).</span><span class="sxs-lookup"><span data-stu-id="d343d-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="d343d-173">При приостановке подписки дата, отображаемая под кнопкой **Приостановлено**, указывает, когда автоматически истечет срок действия подписки, если вы не активируете ее повторно.</span><span class="sxs-lookup"><span data-stu-id="d343d-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="d343d-174">У подписок CSP нет срока действия (так же, как это делаются веб-непосредственными подписками), в течение которых службы продолжают работать, но в подписке не взимается плата за выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="d343d-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="d343d-175">Подписки CSP либо активны, либо приостановлены (или полностью удалены).</span><span class="sxs-lookup"><span data-stu-id="d343d-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="d343d-176">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="d343d-176">Cancel a subscription</span></span>

<span data-ttu-id="d343d-177">Подписки SaaS на основе лицензий от сторонних издателей программного обеспечения можно отменить в [коммерческом рынке](csp-commercial-marketplace-overview.md)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d343d-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="d343d-178">При условии отмены в течение периода отмены вы получите полный возмещение.</span><span class="sxs-lookup"><span data-stu-id="d343d-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="d343d-179">Для ISV предлагает ежемесячные счета:</span><span class="sxs-lookup"><span data-stu-id="d343d-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="d343d-180">Если после размещения заказа вы отменили менее 24 часов, вы получите полный кредит для следующего счета.</span><span class="sxs-lookup"><span data-stu-id="d343d-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d343d-181">Если после размещения заказа вы отменили позже, чем через 24 часа, отмена будет запланирована на момент обновления.</span><span class="sxs-lookup"><span data-stu-id="d343d-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d343d-182">Для предложений, которые выставляются ежегодно:</span><span class="sxs-lookup"><span data-stu-id="d343d-182">For offers billed annually:</span></span>

- <span data-ttu-id="d343d-183">Если после появления заказа вы отменили менее 14 дней, вы получите полный кредит для следующего счета.</span><span class="sxs-lookup"><span data-stu-id="d343d-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d343d-184">Если вы отменили позже через 14 дней после размещения заказа, то отмена будет запланирована при обновлении.</span><span class="sxs-lookup"><span data-stu-id="d343d-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d343d-185">После выполнения этих периодов больше не будет отображаться возможность отмены подписки.</span><span class="sxs-lookup"><span data-stu-id="d343d-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="d343d-186">Службы независимых поставщиков программного обеспечения (например, использующие виртуальные машины или контейнеры) не могут возвращать данные на основе использования и измерения.</span><span class="sxs-lookup"><span data-stu-id="d343d-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="d343d-187">В качестве метода отмены можно отменить подготовку служб на основе использования.</span><span class="sxs-lookup"><span data-stu-id="d343d-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="d343d-188">Так как плата взимается за использование, эти службы не могут получить возмещение.</span><span class="sxs-lookup"><span data-stu-id="d343d-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="d343d-189">Чтобы отменить подписку SaaS на основе лицензий от издателя ISV, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="d343d-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="d343d-190">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d343d-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d343d-191">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="d343d-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d343d-192">Выберите подписку, которую нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="d343d-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="d343d-193">В столбце **состояние** выберите **Отмена**.</span><span class="sxs-lookup"><span data-stu-id="d343d-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="d343d-194">Затем **отправьте** изменения.</span><span class="sxs-lookup"><span data-stu-id="d343d-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d343d-195">Если появится диалоговое окно, заполните все необходимые сведения и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="d343d-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="d343d-196">Чтобы подтвердить отмену, выберите **Да, отмена**.</span><span class="sxs-lookup"><span data-stu-id="d343d-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="d343d-197">Вы также можете отменить подписку Azure Marketplace с помощью интерфейсов API.</span><span class="sxs-lookup"><span data-stu-id="d343d-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="d343d-198">Дополнительные сведения см. в разделе [Отмена подписки Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="d343d-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="d343d-199">Выберите, следует ли автоматически продлить подписку на продукты коммерческого Marketplace</span><span class="sxs-lookup"><span data-stu-id="d343d-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="d343d-200">По умолчанию активные подписки настроены на автоматическое продление по истечении периода действия подписки.</span><span class="sxs-lookup"><span data-stu-id="d343d-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="d343d-201">Для [подписок на коммерческие продукты Marketplace](csp-commercial-marketplace-overview.md)можно дополнительно отказаться от автоматического продления подписки.</span><span class="sxs-lookup"><span data-stu-id="d343d-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="d343d-202">Чтобы отключить автоматическое продление действующей подписки на коммерческий рынок, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="d343d-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="d343d-203">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d343d-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d343d-204">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="d343d-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d343d-205">Выберите **Подписки**.</span><span class="sxs-lookup"><span data-stu-id="d343d-205">Select **Subscriptions**.</span></span> <span data-ttu-id="d343d-206">Здесь перечислены все подписки на основе лицензий, приобретенные для клиента.</span><span class="sxs-lookup"><span data-stu-id="d343d-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="d343d-207">В столбце **Подписка** выберите подписку, которую необходимо изменить.</span><span class="sxs-lookup"><span data-stu-id="d343d-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="d343d-208">На странице сведения о подписке выберите раздел **состояние** и снимите флажок **Auto-продление** .</span><span class="sxs-lookup"><span data-stu-id="d343d-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="d343d-209">Нажмите кнопку **Submit** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="d343d-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d343d-210">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d343d-210">Next steps</span></span>

- [<span data-ttu-id="d343d-211">Приобретение продуктов коммерческого Marketplace для клиентов</span><span class="sxs-lookup"><span data-stu-id="d343d-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="d343d-212">Управляйте продуктами коммерческих рынков для своих клиентов</span><span class="sxs-lookup"><span data-stu-id="d343d-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="d343d-213">Обзор коммерческой платформы</span><span class="sxs-lookup"><span data-stu-id="d343d-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)