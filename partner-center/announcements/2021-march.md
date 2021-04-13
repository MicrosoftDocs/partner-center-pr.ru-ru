---
title: Объявления за март 2021 года
description: Объявления, касающиеся Центра партнеров Майкрософт, за март 2021 года со сведениями о новых возможностях, рекламных акциях, предложениях, рынках и изменениях существующих предложений.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374398"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="706a8-103">Объявления за март 2021 года</span><span class="sxs-lookup"><span data-stu-id="706a8-103">March 2021 announcements</span></span>

<span data-ttu-id="706a8-104">Эта страница содержит объявления, касающиеся Центра партнеров Майкрософт, за март 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="706a8-105">Доступен для тестирования обновленный API проверки адресов клиентов в рамках CSP</span><span class="sxs-lookup"><span data-stu-id="706a8-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-106">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-106">Categories</span></span>

- <span data-ttu-id="706a8-107">Дата: 31.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="706a8-108">Характеристики</span><span class="sxs-lookup"><span data-stu-id="706a8-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-109">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-109">Summary</span></span>

<span data-ttu-id="706a8-110">Так как мы стремимся помогать партнерам и клиентам вести бизнес на основе доверия, мы будем предлагать партнерам по всему миру тестировать изменения в API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="706a8-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-111">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-111">Impacted audience</span></span>

<span data-ttu-id="706a8-112">Все партнеры с прямым выставлением счетов и косвенные поставщики в рамках CSP, которые создают новые сведения об адресах клиентов или обновляют существующие.</span><span class="sxs-lookup"><span data-stu-id="706a8-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="706a8-113">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-113">Details</span></span>

<span data-ttu-id="706a8-114">Корпорация Майкрософт работает на основе принципов доверия,</span><span class="sxs-lookup"><span data-stu-id="706a8-114">Microsoft runs on trust.</span></span> <span data-ttu-id="706a8-115">Мы стремимся обеспечить соответствующий требованиям, безопасный и защищенный метод проверки отправки адреса клиента для работы с клиентскими подписками по программе "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="706a8-116">Сегодня, 31 марта 2021 г., мы добавили изменения в API ValidateAddress, которые мы предлагаем вам протестировать перед выпуском в июне 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="706a8-117">Обратите внимание, что эти изменения касаются только API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="706a8-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="706a8-118">API-интерфейсы CreateCustomer и CreateCustomer не будут затронуты.</span><span class="sxs-lookup"><span data-stu-id="706a8-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="706a8-119">Ответ будет содержать одно из следующих сообщений о состоянии:</span><span class="sxs-lookup"><span data-stu-id="706a8-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="706a8-120">Состояние</span><span class="sxs-lookup"><span data-stu-id="706a8-120">Status</span></span> | <span data-ttu-id="706a8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="706a8-121">Description</span></span> | <span data-ttu-id="706a8-122">Число возвращаемых предложенных адресов</span><span class="sxs-lookup"><span data-stu-id="706a8-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="706a8-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="706a8-123">VerifiedShippable</span></span> | <span data-ttu-id="706a8-124">Адрес проверен и готов к отправке.</span><span class="sxs-lookup"><span data-stu-id="706a8-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="706a8-125">Single</span><span class="sxs-lookup"><span data-stu-id="706a8-125">Single</span></span> |
| <span data-ttu-id="706a8-126">Проверено</span><span class="sxs-lookup"><span data-stu-id="706a8-126">Verified</span></span> | <span data-ttu-id="706a8-127">Адрес проверен.</span><span class="sxs-lookup"><span data-stu-id="706a8-127">Address is verified.</span></span> | <span data-ttu-id="706a8-128">Single</span><span class="sxs-lookup"><span data-stu-id="706a8-128">Single</span></span> |
| <span data-ttu-id="706a8-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="706a8-129">InteractionRequired</span></span> | <span data-ttu-id="706a8-130">Предлагаемые адреса были значительно изменены и требуют подтверждения пользователем.</span><span class="sxs-lookup"><span data-stu-id="706a8-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="706a8-131">Single</span><span class="sxs-lookup"><span data-stu-id="706a8-131">Single</span></span> |
| <span data-ttu-id="706a8-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="706a8-132">StreetPartial</span></span> | <span data-ttu-id="706a8-133">В адресе указано неполное название улицы. Требуются дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="706a8-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="706a8-134">Несколько (не более трех)</span><span class="sxs-lookup"><span data-stu-id="706a8-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="706a8-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="706a8-135">PremisesPartial</span></span> | <span data-ttu-id="706a8-136">Указаны неполные сведения о здании (номер дома, номер квартиры и т. д.). Требуется дополнительная информация.</span><span class="sxs-lookup"><span data-stu-id="706a8-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="706a8-137">Несколько (не более трех)</span><span class="sxs-lookup"><span data-stu-id="706a8-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="706a8-138">Несколько</span><span class="sxs-lookup"><span data-stu-id="706a8-138">Multiple</span></span> | <span data-ttu-id="706a8-139">В нескольких полях адреса указаны неполные сведения (возможно, также включая StreetPartial и PremisesPartial).</span><span class="sxs-lookup"><span data-stu-id="706a8-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="706a8-140">Несколько (не более трех)</span><span class="sxs-lookup"><span data-stu-id="706a8-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="706a8-141">Нет</span><span class="sxs-lookup"><span data-stu-id="706a8-141">None</span></span> | <span data-ttu-id="706a8-142">Неверный адрес.</span><span class="sxs-lookup"><span data-stu-id="706a8-142">Address is incorrect.</span></span> | <span data-ttu-id="706a8-143">Нет</span><span class="sxs-lookup"><span data-stu-id="706a8-143">None</span></span> |
| <span data-ttu-id="706a8-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="706a8-144">NotValidated</span></span> | <span data-ttu-id="706a8-145">Адрес не удалось отправить в процессе проверки.</span><span class="sxs-lookup"><span data-stu-id="706a8-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="706a8-146">Нет</span><span class="sxs-lookup"><span data-stu-id="706a8-146">None</span></span> |

<span data-ttu-id="706a8-147">После отправки адреса для проверки с помощью API ValidateAddress будет возвращен ответ следующего типа:</span><span class="sxs-lookup"><span data-stu-id="706a8-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="706a8-148">Просмотрите пример ответа.</span><span class="sxs-lookup"><span data-stu-id="706a8-148">Take a look at this sample response.</span></span> <span data-ttu-id="706a8-149">Обратите внимание, что в США при вводе только пяти цифр для почтового индекса в ответе будет возвращен дополнительный суффикс из четырех цифр для строки почтового индекса.</span><span class="sxs-lookup"><span data-stu-id="706a8-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="706a8-150">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-150">Next steps</span></span>

- <span data-ttu-id="706a8-151">Отправьте идентификатор арендатора песочницы нашему специалисту в предметной области (SME) Али Кхаки (Ali Khaki) для участия в тестировании возможностей, чтобы вы могли начать подготовку к обновлению.</span><span class="sxs-lookup"><span data-stu-id="706a8-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="706a8-152">Если вы используете решение поставщика панели управления (CPV), обратитесь к нему за консультацией.</span><span class="sxs-lookup"><span data-stu-id="706a8-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-153">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-153">Questions?</span></span>

<span data-ttu-id="706a8-154">Если у вас возникнут вопросы или вам потребуется поддержка по работе с Майкрософт, обратитесь в группу по поддержке партнеров в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="706a8-155">Новый интерфейс Центра администрирования Exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="706a8-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-156">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-156">Categories</span></span>

- <span data-ttu-id="706a8-157">Дата: 29.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="706a8-158">Характеристики</span><span class="sxs-lookup"><span data-stu-id="706a8-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-159">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-159">Summary</span></span>

<span data-ttu-id="706a8-160">27 апреля 2021 г. для Центра администрирования Exchange (EAC) начнется развертывание нового интерфейса, который повысит эффективность ежедневной работы пользователей.</span><span class="sxs-lookup"><span data-stu-id="706a8-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-161">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-161">Impacted audience</span></span>

<span data-ttu-id="706a8-162">Полномочные администраторы, которые осуществляют доступ к Exchange через Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="706a8-163">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-163">Details</span></span>

<span data-ttu-id="706a8-164">С 27 апреля 2021 г. партнеры, которые переходят к Exchange через Центр партнеров, будут перенаправляться в новый интерфейс EAC.</span><span class="sxs-lookup"><span data-stu-id="706a8-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="706a8-165">Сейчас доступна предварительная версия этого нового интерфейса. Администраторы могут активировать его, выбрав переключатель в правом верхнем углу классического интерфейса EAC.</span><span class="sxs-lookup"><span data-stu-id="706a8-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="706a8-166">Кроме того, можно перейти к новому интерфейсу EAC, выбрав баннер "Попробовать", отображаемый на всех страницах.</span><span class="sxs-lookup"><span data-stu-id="706a8-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="706a8-167">Преимущества нового интерфейса EAC:</span><span class="sxs-lookup"><span data-stu-id="706a8-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="706a8-168">добавлены механизмы аналитики, отчетов и оповещений для проблем, связанных с потоком почты;</span><span class="sxs-lookup"><span data-stu-id="706a8-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="706a8-169">персонализированы панели мониторинга для повышения производительности.</span><span class="sxs-lookup"><span data-stu-id="706a8-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="706a8-170">Чтобы упростить навигацию, мы разместили видео в разделе **обучения и руководств** по новому интерфейсу EAC.</span><span class="sxs-lookup"><span data-stu-id="706a8-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="706a8-171">Из них вы узнаете, как эффективнее всего использовать новый портал.</span><span class="sxs-lookup"><span data-stu-id="706a8-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="706a8-172">После внесения этого изменения классический интерфейс EAC не будет считаться нерекомендуемым.</span><span class="sxs-lookup"><span data-stu-id="706a8-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="706a8-173">Вы получите уведомление задолго до того, как будут реализованы какие-либо изменения.</span><span class="sxs-lookup"><span data-stu-id="706a8-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-174">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-174">Next steps</span></span>

- <span data-ttu-id="706a8-175">Ознакомьтесь с [материалами по этой теме](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), где можно просмотреть снимки экрана нового интерфейса.</span><span class="sxs-lookup"><span data-stu-id="706a8-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="706a8-176">Передайте эти сведения соответствующим заинтересованным лицам в своей организации.</span><span class="sxs-lookup"><span data-stu-id="706a8-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="706a8-177">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-177">Questions?</span></span>

<span data-ttu-id="706a8-178">С любыми вопросами по этим изменениям обращайтесь в соответствующее сообщество в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="706a8-179">Microsoft Operations: представляем календарь выпуска продуктов</span><span class="sxs-lookup"><span data-stu-id="706a8-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-180">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-180">Categories</span></span>

- <span data-ttu-id="706a8-181">Дата: 25.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="706a8-182">Предложения | Современные рабочие места</span><span class="sxs-lookup"><span data-stu-id="706a8-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-183">Итоги</span><span class="sxs-lookup"><span data-stu-id="706a8-183">Summary</span></span>

<span data-ttu-id="706a8-184">В ответ на отзывы партнеров Microsoft Operations будет оптимизировать отправку сообщений о выпуске продуктов.</span><span class="sxs-lookup"><span data-stu-id="706a8-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-185">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-185">Impacted audience</span></span>

<span data-ttu-id="706a8-186">Партнеры в рамках программы "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="706a8-187">Подробнее</span><span class="sxs-lookup"><span data-stu-id="706a8-187">Details</span></span>

<span data-ttu-id="706a8-188">Корпорация Майкрософт стремится непрерывно улучшать взаимодействие с партнерами.</span><span class="sxs-lookup"><span data-stu-id="706a8-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="706a8-189">В своих отзывах вы указывали, что получали слишком много сообщений от корпорации Майкрософт, включая дублирующиеся объявления о выпуске продуктов.</span><span class="sxs-lookup"><span data-stu-id="706a8-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="706a8-190">В ответ на ваши отзывы корпорация Майкрософт упростила процесс подготовки к выпуску продуктов для новых и существующих предложений.</span><span class="sxs-lookup"><span data-stu-id="706a8-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="706a8-191">Теперь мы ежемесячно размещаем одно представление со сведениями обо всех выпусках продуктов в коллекции ресурсов по подготовке к работе.</span><span class="sxs-lookup"><span data-stu-id="706a8-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="706a8-192">Это ежемесячное [календарное представление выпуска продуктов](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) заменит сообщения о выпуске отдельных продуктов в коллекции ресурсов по подготовке к работе и в объявлениях Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="706a8-193">Кроме того, вы можете получить доступ к этому [календарю выпуска продуктов](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) из [коллекций сообщества](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [представлений календаря](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) и [информационных бюллетеней CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="706a8-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="706a8-194">Мы будем уведомлять вас при ежемесячной публикации календаря выпуска продуктов в объявлении в коллекции ресурсов по подготовке к работе.</span><span class="sxs-lookup"><span data-stu-id="706a8-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="706a8-195">Вы по-прежнему можете найти информацию о новых и существующих предложениях в журналах изменений прейскурантов и их предварительных версий, а также в блогах по продуктам, руководствах по лицензированию и на страницах продуктов с маркетинговыми материалами.</span><span class="sxs-lookup"><span data-stu-id="706a8-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="706a8-196">Изменение касается выпусков следующих продуктов:</span><span class="sxs-lookup"><span data-stu-id="706a8-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="706a8-197">локальные продукты Dynamics;</span><span class="sxs-lookup"><span data-stu-id="706a8-197">Dynamics on-premises</span></span>
- <span data-ttu-id="706a8-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="706a8-198">Microsoft 365</span></span>
- <span data-ttu-id="706a8-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="706a8-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="706a8-200">Windows</span><span class="sxs-lookup"><span data-stu-id="706a8-200">Windows</span></span>
- <span data-ttu-id="706a8-201">Сервер</span><span class="sxs-lookup"><span data-stu-id="706a8-201">Server</span></span>  
- <span data-ttu-id="706a8-202">Инструменты</span><span class="sxs-lookup"><span data-stu-id="706a8-202">Tools</span></span>
- <span data-ttu-id="706a8-203">Teams и Telco.</span><span class="sxs-lookup"><span data-stu-id="706a8-203">Teams and Telco</span></span>

<span data-ttu-id="706a8-204">Мы будем и дальше отправлять определенные объявления о выпуске продуктов, для использования которых необходимо изучить сведения о подготовке к работе.</span><span class="sxs-lookup"><span data-stu-id="706a8-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-205">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-205">Next steps</span></span>

<span data-ttu-id="706a8-206">Изучите доступные ресурсы на эту тему и поделитесь этой информацией с соответствующими заинтересованными лицами в своей организации.</span><span class="sxs-lookup"><span data-stu-id="706a8-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-207">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-207">Questions?</span></span>

<span data-ttu-id="706a8-208">С вопросами по этим предложениям обращайтесь в соответствующее сообщество в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="706a8-209">Изменения в требованиях к подключению клиентов для участников программы CSP</span><span class="sxs-lookup"><span data-stu-id="706a8-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-210">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-210">Categories</span></span>

- <span data-ttu-id="706a8-211">Дата: 25.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="706a8-212">Характеристики</span><span class="sxs-lookup"><span data-stu-id="706a8-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-213">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-213">Summary</span></span>

<span data-ttu-id="706a8-214">Так как мы стремимся поддерживать доверительные отношения с партнерами и клиентами при оказании им помощи в ведении бизнеса, мы будем запрашивать дополнительные сведения о клиентах с 25 марта 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-215">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-215">Impacted audience</span></span>

<span data-ttu-id="706a8-216">Партнеры с прямым выставлением счетов по программе "Поставщик облачных решений" (CSP) и косвенные поставщики с новыми или существующими клиентами в странах, указанных в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="706a8-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="706a8-217">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-217">Details</span></span>

<span data-ttu-id="706a8-218">Корпорация Майкрософт работает на основе принципов доверия,</span><span class="sxs-lookup"><span data-stu-id="706a8-218">Microsoft runs on trust.</span></span> <span data-ttu-id="706a8-219">Мы стремимся обеспечить соответствующий требованиям, безопасный и защищенный метод проверки клиентов для работы с клиентскими подписками по программе "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="706a8-220">25 марта 2021 г. мы представим улучшения API и пользовательского интерфейса Центра партнеров, которые повлияют на работу партнеров, соответствующих обоим следующим критериям:</span><span class="sxs-lookup"><span data-stu-id="706a8-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="706a8-221">партнер, напрямую получающий счета от Майкрософт (то есть партнер с прямым выставлением счетов или косвенный поставщик);</span><span class="sxs-lookup"><span data-stu-id="706a8-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="706a8-222">партнер, ведущий бизнес с новыми или существующими клиентами в таких странах:</span><span class="sxs-lookup"><span data-stu-id="706a8-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="706a8-223">Таиланд</span><span class="sxs-lookup"><span data-stu-id="706a8-223">Thailand</span></span>
    - <span data-ttu-id="706a8-224">Вьетнам</span><span class="sxs-lookup"><span data-stu-id="706a8-224">Vietnam</span></span>
    - <span data-ttu-id="706a8-225">Турция</span><span class="sxs-lookup"><span data-stu-id="706a8-225">Turkey</span></span>
    - <span data-ttu-id="706a8-226">Польша</span><span class="sxs-lookup"><span data-stu-id="706a8-226">Poland</span></span>
    - <span data-ttu-id="706a8-227">ЮАР</span><span class="sxs-lookup"><span data-stu-id="706a8-227">South Africa</span></span>
    - <span data-ttu-id="706a8-228">Индия</span><span class="sxs-lookup"><span data-stu-id="706a8-228">India</span></span>
    - <span data-ttu-id="706a8-229">Бразилия</span><span class="sxs-lookup"><span data-stu-id="706a8-229">Brazil</span></span>
    - <span data-ttu-id="706a8-230">Ирак</span><span class="sxs-lookup"><span data-stu-id="706a8-230">Iraq</span></span>
    - <span data-ttu-id="706a8-231">Мьянма</span><span class="sxs-lookup"><span data-stu-id="706a8-231">Myanmar</span></span>
    - <span data-ttu-id="706a8-232">Южный Судан</span><span class="sxs-lookup"><span data-stu-id="706a8-232">South Sudan</span></span>
    - <span data-ttu-id="706a8-233">Саудовская Аравия</span><span class="sxs-lookup"><span data-stu-id="706a8-233">Saudi Arabia</span></span>
    - <span data-ttu-id="706a8-234">ОАЭ</span><span class="sxs-lookup"><span data-stu-id="706a8-234">United Arab Emirates</span></span>
    - <span data-ttu-id="706a8-235">Венесуэла</span><span class="sxs-lookup"><span data-stu-id="706a8-235">Venezuela</span></span>

<span data-ttu-id="706a8-236">Партнерам, которые соответствуют критериям, нужно будет сообщить нам **идентификатор регистрации компании** клиента (также называемый **ИНН организации** клиента) и его **номер телефона** при подключении новых клиентов или изменении сведений о существующих.</span><span class="sxs-lookup"><span data-stu-id="706a8-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="706a8-237">Такие партнеры теперь также могут при желании указать **отчество** клиента.</span><span class="sxs-lookup"><span data-stu-id="706a8-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="706a8-238">Обратите внимание, что при добавлении идентификатора регистрации компании следует использовать идентификационный номер налогоплательщика вашего предприятия, а не личный идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="706a8-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="706a8-239">Партнеры, которые ведут бизнес с новыми или существующими клиентами в следующих странах, уже были подключены после предыдущего выпуска в ноябре 2020 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="706a8-240">Армения</span><span class="sxs-lookup"><span data-stu-id="706a8-240">Armenia</span></span>
- <span data-ttu-id="706a8-241">Азербайджан</span><span class="sxs-lookup"><span data-stu-id="706a8-241">Azerbaijan</span></span>
- <span data-ttu-id="706a8-242">Беларусь</span><span class="sxs-lookup"><span data-stu-id="706a8-242">Belarus</span></span>
- <span data-ttu-id="706a8-243">Венгрия</span><span class="sxs-lookup"><span data-stu-id="706a8-243">Hungary</span></span>
- <span data-ttu-id="706a8-244">Казахстан</span><span class="sxs-lookup"><span data-stu-id="706a8-244">Kazakhstan</span></span>
- <span data-ttu-id="706a8-245">Киргизстан</span><span class="sxs-lookup"><span data-stu-id="706a8-245">Kyrgyzstan</span></span>
- <span data-ttu-id="706a8-246">Молдова</span><span class="sxs-lookup"><span data-stu-id="706a8-246">Moldova</span></span>
- <span data-ttu-id="706a8-247">Россия</span><span class="sxs-lookup"><span data-stu-id="706a8-247">Russia</span></span>
- <span data-ttu-id="706a8-248">Таджикистан</span><span class="sxs-lookup"><span data-stu-id="706a8-248">Tajikistan</span></span>
- <span data-ttu-id="706a8-249">Украина</span><span class="sxs-lookup"><span data-stu-id="706a8-249">Ukraine</span></span>
- <span data-ttu-id="706a8-250">Узбекистан</span><span class="sxs-lookup"><span data-stu-id="706a8-250">Uzbekistan</span></span>

<span data-ttu-id="706a8-251">С 25 марта 2021 г. партнеры, у которых есть клиенты в других странах, смогут при желании указывать **идентификатор регистрации компании**, **номер телефона** и **отчество или второе имя** клиента.</span><span class="sxs-lookup"><span data-stu-id="706a8-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-252">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-252">Next steps</span></span>

- <span data-ttu-id="706a8-253">Более подробные инструкции см. в технической документации и часто задаваемых вопросах в соответствующей [коллекции для партнеров](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).</span><span class="sxs-lookup"><span data-stu-id="706a8-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="706a8-254">Подготовьтесь к реализации изменений в использовании API и веб-интерфейса Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="706a8-255">API и пакеты SDK будут доступны для тестирования.</span><span class="sxs-lookup"><span data-stu-id="706a8-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="706a8-256">Обязательно отправьте дополнительные данные при подключении новых клиентов или изменении существующих сведений о клиентах.</span><span class="sxs-lookup"><span data-stu-id="706a8-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="706a8-257">Если вы используете решение поставщика панели управления (CPV), обратитесь к нему за консультацией.</span><span class="sxs-lookup"><span data-stu-id="706a8-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-258">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-258">Questions?</span></span>

<span data-ttu-id="706a8-259">Обратитесь к налоговому консультанту или в местную налоговую службу, если у вас возникли вопросы, касающиеся юридического идентификатора (также называется ИНН или TIN).</span><span class="sxs-lookup"><span data-stu-id="706a8-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="706a8-260">Корпорация Майкрософт не предоставляет рекомендации по налогообложению.</span><span class="sxs-lookup"><span data-stu-id="706a8-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="706a8-261">Если вам требуется поддержка при операциях с Майкрософт, [создайте запрос на обслуживание](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="706a8-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="706a8-262">Исправления, внесенные в прейскурант на программное обеспечение с бессрочной лицензией за 1 марта 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-263">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-263">Categories</span></span>

- <span data-ttu-id="706a8-264">Дата: 23.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="706a8-265">Предложения и рынки</span><span class="sxs-lookup"><span data-stu-id="706a8-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-266">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-266">Impacted audience</span></span>

<span data-ttu-id="706a8-267">Косвенные поставщики и партнеры с прямым выставлением счетов, которые предоставляют программное обеспечение с бессрочной лицензией в рамках программы "Поставщик облачных решений".</span><span class="sxs-lookup"><span data-stu-id="706a8-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="706a8-268">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-268">Details</span></span>

<span data-ttu-id="706a8-269">Прейскурант на программное обеспечение с бессрочной лицензией, опубликованный 1 марта 2021 г., включал лишние рынки.</span><span class="sxs-lookup"><span data-stu-id="706a8-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="706a8-270">Прейскурант на программное обеспечение с бессрочной лицензией был обновлен 17 марта 2021 г. с внесением исправлений.</span><span class="sxs-lookup"><span data-stu-id="706a8-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="706a8-271">Такие исправления применялись только к следующему:</span><span class="sxs-lookup"><span data-stu-id="706a8-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="706a8-272">идентификатор продукта: DF77X4D43RKT;</span><span class="sxs-lookup"><span data-stu-id="706a8-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="706a8-273">имя продукта: "Обновление Windows 10 Домашняя до Профессиональная для Microsoft 365 бизнес";</span><span class="sxs-lookup"><span data-stu-id="706a8-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="706a8-274">удаленные или неподдерживаемые рынки: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW.</span><span class="sxs-lookup"><span data-stu-id="706a8-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="706a8-275">Эти изменения касаются только указанного выше продукта.</span><span class="sxs-lookup"><span data-stu-id="706a8-275">These changes only apply to the above product.</span></span> <span data-ttu-id="706a8-276">Исправления для других продуктов не вносились.</span><span class="sxs-lookup"><span data-stu-id="706a8-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="706a8-277">Дальнейшие действия и ресурсы</span><span class="sxs-lookup"><span data-stu-id="706a8-277">Next steps and resources</span></span>

- <span data-ttu-id="706a8-278">Партнеры, предлагающие программное обеспечение с бессрочной лицензией, должны скачать последний прейскурант на такое ПО.</span><span class="sxs-lookup"><span data-stu-id="706a8-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="706a8-279">Расшифровку двухбуквенных сокращений см. на странице с [региональными кодами стран](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries).</span><span class="sxs-lookup"><span data-stu-id="706a8-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a><span data-ttu-id="706a8-280">Выпуск пакета SDK для .NET Standard (версия 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="706a8-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-281">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-281">Categories</span></span>

- <span data-ttu-id="706a8-282">Дата: 23.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="706a8-283">Характеристики</span><span class="sxs-lookup"><span data-stu-id="706a8-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="706a8-284">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-284">Impacted audience</span></span>

<span data-ttu-id="706a8-285">Партнеры с прямым выставлением счетов и непрямые поставщики, которые участвуют в программе CSP и используют пакет SDK Центра партнеров для .NET.</span><span class="sxs-lookup"><span data-stu-id="706a8-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="706a8-286">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-286">Details</span></span>

<span data-ttu-id="706a8-287">С 23 марта 2021 г. партнеры могут скачать версию пакета SDK [MicrosoftPartnerCenter.NETSDK (коллекция NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), а также обновленные общедоступные [примеры для пакетов SDK Центра партнеров на GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span><span class="sxs-lookup"><span data-stu-id="706a8-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="706a8-288">Эта версия включает обновления в следующих методах:</span><span class="sxs-lookup"><span data-stu-id="706a8-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="706a8-289">Аудит обновлен: новые типы операций</span><span class="sxs-lookup"><span data-stu-id="706a8-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="706a8-290">Добавлены новые [типы операций](https://docs.microsoft.com/partner-center/develop/auditing-resources), которые позволяют получать данные о том, когда клиент утвердил права DAP или приостановил их действие.</span><span class="sxs-lookup"><span data-stu-id="706a8-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="706a8-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="706a8-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="706a8-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="706a8-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="706a8-293">Аудит обновлен: новые типы ресурсов и операций</span><span class="sxs-lookup"><span data-stu-id="706a8-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="706a8-294">Добавлены новые [типы ресурсов и операций](https://docs.microsoft.com/partner-center/develop/auditing-resources) для поддержки сценария с ролью каталога клиента.</span><span class="sxs-lookup"><span data-stu-id="706a8-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="706a8-295">Новый тип ресурса CustomerDirectoryRole.</span><span class="sxs-lookup"><span data-stu-id="706a8-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="706a8-296">Типы операций AddUserMember и RemoveUserMember.</span><span class="sxs-lookup"><span data-stu-id="706a8-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="706a8-297">Обновления пакета SDK для учетных записей клиентов</span><span class="sxs-lookup"><span data-stu-id="706a8-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="706a8-298">Поддержка GET /customers/{идентификатор_арендатора_клиента}/directSignedMicrosoftCustomerAgreementStatus.</span><span class="sxs-lookup"><span data-stu-id="706a8-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="706a8-299">GET /customers/{идентификатор_арендатора_клиента}/qualifications</span><span class="sxs-lookup"><span data-stu-id="706a8-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="706a8-300">POST /customers/{идентификатор_клиента}/qualifications?code={проверочный_код}</span><span class="sxs-lookup"><span data-stu-id="706a8-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="706a8-301">Дополнительные изменения</span><span class="sxs-lookup"><span data-stu-id="706a8-301">Additional changes</span></span>

<span data-ttu-id="706a8-302">В рамках новой коммерческой платформы реализованы следующие изменения, которые в настоящее время доступны только по приглашениям тем партнерам, которым предоставлена техническая версия возможностей новой коммерческой платформы M365/D365.</span><span class="sxs-lookup"><span data-stu-id="706a8-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="706a8-303">Партнеры без доступа к технической версии новой коммерческой платформы не заметят изменений и смогут пользоваться преимуществами обратной совместимости.</span><span class="sxs-lookup"><span data-stu-id="706a8-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="706a8-304">Изменения каталога:</span><span class="sxs-lookup"><span data-stu-id="706a8-304">Catalog Changes:</span></span>

  - <span data-ttu-id="706a8-305">GET /products/{идентификатор_продукта}/skus/{идентификатор_SKU}</span><span class="sxs-lookup"><span data-stu-id="706a8-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="706a8-306">Приобретение и управление:</span><span class="sxs-lookup"><span data-stu-id="706a8-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="706a8-307">GET /customers/{идентификатор_клиента}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="706a8-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="706a8-308">GET /customers/{идентификато_клиента}/subscriptions/{идентификатор_подписки}</span><span class="sxs-lookup"><span data-stu-id="706a8-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="706a8-309">PATCH /customers/{идентификатор_клиента}/subscriptions/{идентификатор_подписки}</span><span class="sxs-lookup"><span data-stu-id="706a8-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="706a8-310">GET /customers/{идентификатор_клиента}/subscriptions/{идентификатор_подписки}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="706a8-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="706a8-311">GET /customers/{идентификатор_клиента}/subscriptions/{идентификатор_подписки}/transitions</span><span class="sxs-lookup"><span data-stu-id="706a8-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="706a8-312">POST /customers/{идентификатор_клиента}/subscriptions/{идентификатор_подписки}/transitions</span><span class="sxs-lookup"><span data-stu-id="706a8-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-313">Next Steps</span><span class="sxs-lookup"><span data-stu-id="706a8-313">Next Steps</span></span>

- <span data-ttu-id="706a8-314">Скачайте последнюю версию [MicrosoftPartnerCenter.NETSDK (коллекция NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0).</span><span class="sxs-lookup"><span data-stu-id="706a8-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="706a8-315">Скачайте и просмотрите [примеры с сайта GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span><span class="sxs-lookup"><span data-stu-id="706a8-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="706a8-316">Предложение на коммерческой платформе в рамках CSP и поощрения за соответствующие предложения в рамках CSP за 2021 финансовый год</span><span class="sxs-lookup"><span data-stu-id="706a8-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-317">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-317">Categories</span></span>

- <span data-ttu-id="706a8-318">Дата: 18.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="706a8-319">Характеристики</span><span class="sxs-lookup"><span data-stu-id="706a8-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-320">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-320">Impacted audience</span></span>

<span data-ttu-id="706a8-321">Косвенные поставщики и партнеры с прямым выставлением счетов в программе "Поставщик облачных решений".</span><span class="sxs-lookup"><span data-stu-id="706a8-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="706a8-322">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-322">Details</span></span>

<span data-ttu-id="706a8-323">Косвенные поставщики и партнеры с прямым выставлением счетов в рамках программы "Поставщик облачных решений" могут продавать сторонние предложения и получать бонусы за каждое соответствующее предложение третьей стороны, предоставленное через Центр партнеров или портал Azure.</span><span class="sxs-lookup"><span data-stu-id="706a8-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="706a8-324">Такие поощрения имеют вид бонусов за продажи с выставлением счетов соответствующих предложений и **будут доступны до 30 июня 2021 г.**</span><span class="sxs-lookup"><span data-stu-id="706a8-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="706a8-325">Подробнее об этом предложении коммерческой платформы для партнеров CSP можно узнать ниже. Свяжитесь со своими клиентами уже сегодня, чтобы помочь им найти оптимальные предложения для достижения успеха и реализации цифровой трансформации.</span><span class="sxs-lookup"><span data-stu-id="706a8-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="706a8-326">Мы сотрудничаем с независимыми поставщиками программного обеспечения (ISV) над предоставлением клиентам Майкрософт новейших решений IaaS и SaaS.</span><span class="sxs-lookup"><span data-stu-id="706a8-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="706a8-327">Издатели независимых поставщиков программного обеспечения могут реализовать продажу своих предложений через канал партнеров Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="706a8-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="706a8-328">Наши предложения, по которым выплачиваются поощрения, делятся на две категории:</span><span class="sxs-lookup"><span data-stu-id="706a8-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="706a8-329">Избранные предложения SaaS и IaaS сторонних поставщиков со статусом поощрений за совместные продажи интеллектуальной собственности в Azure.</span><span class="sxs-lookup"><span data-stu-id="706a8-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="706a8-330">Приложения SaaS, интегрированные с Teams или по меньшей мере с двумя офисными приложениями Microsoft 365, такими как PowerPoint, Word, Excel, Outlook или SharePoint.</span><span class="sxs-lookup"><span data-stu-id="706a8-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="706a8-331">Дальнейшие действия и ресурсы</span><span class="sxs-lookup"><span data-stu-id="706a8-331">Next steps and resources</span></span>

- <span data-ttu-id="706a8-332">Узнайте, как получить [поощрения для партнеров](https://partner.microsoft.com/membership/partner-incentives) за продажу соответствующих приложений на коммерческой платформе.</span><span class="sxs-lookup"><span data-stu-id="706a8-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="706a8-333">Каждый месяц мы добавляем новые предложения.</span><span class="sxs-lookup"><span data-stu-id="706a8-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="706a8-334">Ресурсы по поощрениям для партнеров с прямым выставлением счетов в программе "Поставщик облачных решений"</span><span class="sxs-lookup"><span data-stu-id="706a8-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="706a8-335">Ресурсы по поощрениям для косвенных поставщиков в программе "Поставщик облачных решений"</span><span class="sxs-lookup"><span data-stu-id="706a8-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="706a8-336">Просмотрите эту [презентацию](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf), чтобы узнать больше о продаже приложений на коммерческой платформе.</span><span class="sxs-lookup"><span data-stu-id="706a8-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="706a8-337">Ознакомьтесь с дополнительными ресурсами [здесь](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="706a8-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="706a8-338">Изучите каталог коммерческой платформы в [Центре партнеров](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) или на [портале Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="706a8-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="706a8-339">Воспользуйтесь [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) для интеграции приложений нас страницу своей компании на коммерческой платформе.</span><span class="sxs-lookup"><span data-stu-id="706a8-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="706a8-340">Обратитесь к независимым поставщикам программного обеспечения, с которыми вы хотели бы вести бизнес.</span><span class="sxs-lookup"><span data-stu-id="706a8-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="706a8-341">Косвенным поставщикам необходимо выполнить интеграцию с помощью API и сообщить торговым посредникам, какие приложения нужно продавать.</span><span class="sxs-lookup"><span data-stu-id="706a8-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-342">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-342">Questions?</span></span>  

<span data-ttu-id="706a8-343">Общие сведения о коммерческой платформе в Центре партнеров см. в [этой статье](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview).</span><span class="sxs-lookup"><span data-stu-id="706a8-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="706a8-344">Если вам требуется дополнительная помощь, вы можете создать запрос на поддержку в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="706a8-345">Подробная информация собрана на странице [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span><span class="sxs-lookup"><span data-stu-id="706a8-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="706a8-346">Изменение названия предложения и обновление необходимых компонентов для Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="706a8-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-347">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-347">Categories</span></span>

- <span data-ttu-id="706a8-348">Дата: 18.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="706a8-349">Характеристики</span><span class="sxs-lookup"><span data-stu-id="706a8-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-350">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-350">Summary</span></span>

<span data-ttu-id="706a8-351">1 апреля 2021 г. будет обновлен окончательный прейскурант с добавлением разъяснений по наименованию и необходимым компонентам для предложений Power BI Premium на пользователя.</span><span class="sxs-lookup"><span data-stu-id="706a8-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-352">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-352">Impacted audience</span></span>

<span data-ttu-id="706a8-353">Прямые и косвенные партнеры по программе "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="706a8-354">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-354">Details</span></span>

<span data-ttu-id="706a8-355">1 апреля 2021 г. будет обновлен окончательный прейскурант с добавлением разъяснений по наименованию и необходимым компонентам для предложений Power BI Premium на пользователя.</span><span class="sxs-lookup"><span data-stu-id="706a8-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="706a8-356">До обновления окончательного прейскуранта пользуйтесь информацией из этого раздела, чтобы избежать ошибок при заказе продуктов.</span><span class="sxs-lookup"><span data-stu-id="706a8-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="706a8-357">Ниже приведены затронутые SKU и сведения о необходимых компонентах.</span><span class="sxs-lookup"><span data-stu-id="706a8-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="706a8-358">Отображаемое имя предложения в предварительной версии прейскуранта по состоянию на 1 марта</span><span class="sxs-lookup"><span data-stu-id="706a8-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="706a8-359">Обновленное отображаемое имя предложения в окончательном прейскуранте по состоянию на 1 апреля</span><span class="sxs-lookup"><span data-stu-id="706a8-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="706a8-360">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="706a8-361">Надстройка Power BI Premium на пользователя (цены для сотрудников некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="706a8-362">Надстройка Power BI Premium на пользователя **(Office)** (цены для сотрудников некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="706a8-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="706a8-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="706a8-364">Для приобретения этого предложения клиенты должны иметь один из следующих необходимых компонентов:</span><span class="sxs-lookup"><span data-stu-id="706a8-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="706a8-365">Отображаемое имя предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-365">Offer display name</span></span> | <span data-ttu-id="706a8-366">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="706a8-367">Microsoft 365 E5 (расценки для некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="706a8-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="706a8-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="706a8-369">Microsoft 365 E5 без аудиоконференций (расценки для некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="706a8-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="706a8-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="706a8-371">Office 365 E5 (расценки для некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="706a8-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="706a8-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="706a8-373">Пробная версия Office 365 E5 (расценки для некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="706a8-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="706a8-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="706a8-375">Office 365 E5 без аудиоконференций (расценки для некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="706a8-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="706a8-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="706a8-377">Для приобретения следующего предложения Power BI Premium требуется иметь необходимый компонент:</span><span class="sxs-lookup"><span data-stu-id="706a8-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="706a8-378">Отображаемое имя предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-378">Offer display name</span></span> | <span data-ttu-id="706a8-379">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="706a8-380">Надстройка Power BI Premium на пользователя (цены для сотрудников некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="706a8-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="706a8-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="706a8-382">Для приобретения этого предложения клиентам требуется иметь следующий необходимый компонент:</span><span class="sxs-lookup"><span data-stu-id="706a8-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="706a8-383">Отображаемое имя предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-383">Offer display name</span></span> | <span data-ttu-id="706a8-384">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="706a8-385">Power BI Pro (расценки для некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="706a8-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="706a8-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="706a8-387">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-387">Next steps</span></span>

<span data-ttu-id="706a8-388">Изучите доступные ресурсы и на эту тему поделитесь этой информацией с соответствующими заинтересованными лицами в своей организации.</span><span class="sxs-lookup"><span data-stu-id="706a8-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="706a8-389">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-389">Questions?</span></span>

<span data-ttu-id="706a8-390">С любыми вопросами по этим предложениям обращайтесь в соответствующее сообщество в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a><span data-ttu-id="706a8-391">Обновления цен на март для Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="706a8-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-392">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-392">Categories</span></span>

- <span data-ttu-id="706a8-393">Дата: 16.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="706a8-394">Предложения и рынки</span><span class="sxs-lookup"><span data-stu-id="706a8-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-395">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-395">Summary</span></span>

<span data-ttu-id="706a8-396">Были исправлены неверные цены за март 2021 г. для Microsoft 365 F3 в фунтах стерлингов (GBP) и евро (EUR).</span><span class="sxs-lookup"><span data-stu-id="706a8-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-397">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-397">Impacted audience</span></span>

<span data-ttu-id="706a8-398">Партнеры, которые приобрели Microsoft 365 F3 за фунты стерлингов (GBP) или евро (EUR) в период с 1 по 17 марта 2021 г. через программу "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="706a8-399">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-399">Details</span></span>

<span data-ttu-id="706a8-400">Корпорация Майкрософт устранила ошибки в ценах для Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="706a8-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="706a8-401">Неправильные цены были указаны только для фунта стерлингов (GBP) и евро (EUR) и только для тех предложений, которые были приобретены в период с 1 по 17 марта 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="706a8-402">Затронутые предложения и валюты приведены ниже.</span><span class="sxs-lookup"><span data-stu-id="706a8-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="706a8-403">Название предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-403">Offer name</span></span> | <span data-ttu-id="706a8-404">Валюта</span><span class="sxs-lookup"><span data-stu-id="706a8-404">Currency</span></span> | <span data-ttu-id="706a8-405">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-405">Offer ID</span></span> | <span data-ttu-id="706a8-406">Идентификатор материалов</span><span class="sxs-lookup"><span data-stu-id="706a8-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="706a8-407">Microsoft 365 F3 (для благотворительных организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="706a8-408">GBP</span><span class="sxs-lookup"><span data-stu-id="706a8-408">GBP</span></span> | <span data-ttu-id="706a8-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="706a8-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="706a8-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="706a8-410">AAD-11626</span></span> |
| <span data-ttu-id="706a8-411">Microsoft 365 F3 (для коммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="706a8-412">EUR</span><span class="sxs-lookup"><span data-stu-id="706a8-412">EUR</span></span>| <span data-ttu-id="706a8-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="706a8-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="706a8-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="706a8-414">AAA-89898</span></span> |
 
<span data-ttu-id="706a8-415">Предварительные версии прейскурантов на основе лицензий за март и апрель были обновлены в 17:00 (PST) 16 марта.</span><span class="sxs-lookup"><span data-stu-id="706a8-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-416">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="706a8-416">Next steps</span></span>

- <span data-ttu-id="706a8-417">Партнерам нужно повторно скачать актуальные прейскуранты на основе лицензий (предварительные версии за март и апрель) с такими исправлениями цен (если применимо).</span><span class="sxs-lookup"><span data-stu-id="706a8-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="706a8-418">В ближайшие недели специалисты корпорации Майкрософт свяжутся с затронутыми партнерами по электронной почте и сообщат им о дальнейших шагах для корректировки соответствующих транзакций.</span><span class="sxs-lookup"><span data-stu-id="706a8-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-419">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-419">Questions?</span></span>

<span data-ttu-id="706a8-420">С вопросами обращайтесь в соответствующее сообщество CSP в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="706a8-421">Обновление юридического названия компании в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="706a8-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-422">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-422">Categories</span></span>

- <span data-ttu-id="706a8-423">Дата: 16.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="706a8-424">Повышение эффективности и масштабируемости</span><span class="sxs-lookup"><span data-stu-id="706a8-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-425">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-425">Summary</span></span>

<span data-ttu-id="706a8-426">Начиная с марта 2021 г. партнеры из Microsoft Partner Network (MPN) и косвенные торговые посредники в рамках программы "Поставщик облачных решений" (CSP) смогут изменить юридическое название своей компании в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-427">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-427">Impacted audience</span></span>

<span data-ttu-id="706a8-428">Партнеры MPN и косвенные торговые посредники по программе CSP (не касается партнеров по программе CSP с прямым выставлением счетов).</span><span class="sxs-lookup"><span data-stu-id="706a8-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="706a8-429">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-429">Details</span></span>

<span data-ttu-id="706a8-430">Начиная с марта 2021 г. партнеры MPN и косвенные торговые посредники по программе CSP смогут самостоятельно изменить юридическое название своей компании в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="706a8-431">Теперь партнерам не нужно будет отправлять запрос в службу поддержки Центра партнеров, чтобы выполнить эту операцию.</span><span class="sxs-lookup"><span data-stu-id="706a8-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="706a8-432">Это сэкономит партнерам значительное количество времени, которое требовалось на выполнение этих действий.</span><span class="sxs-lookup"><span data-stu-id="706a8-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="706a8-433">Дополнительные сведения см. в разделе [Обновление юридического бизнес-профиля](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="706a8-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="706a8-434">Убедитесь, что название в вашем юридическом бизнес-профиле указано без орфографических ошибок и сокращений и точно соответствует официальным записям бизнес-регистрации вашей компании.</span><span class="sxs-lookup"><span data-stu-id="706a8-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="706a8-435">Дополнительные сведения об изменении профиля организации см. в статье [Проверка или обновление сведений в профиле компании](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="706a8-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-436">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-436">Next steps</span></span>

<span data-ttu-id="706a8-437">Передайте эти сведения сотрудникам своей организации, чтобы соответствующая команда могла проверить процессы и внести в них необходимые изменения.</span><span class="sxs-lookup"><span data-stu-id="706a8-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-438">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-438">Questions?</span></span>

<span data-ttu-id="706a8-439">С вопросами обращайтесь в соответствующее сообщество CSP в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="706a8-440">Обновление в развитии программы "Поставщик облачных решений" (CSP) и изменения в программе Open License</span><span class="sxs-lookup"><span data-stu-id="706a8-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-441">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-441">Categories</span></span>

- <span data-ttu-id="706a8-442">Дата: 15.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="706a8-443">Возможности</span><span class="sxs-lookup"><span data-stu-id="706a8-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-444">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-444">Summary</span></span>

<span data-ttu-id="706a8-445">В рамках программы "Поставщик облачных решений" (CSP) станут доступны новые предложения программного обеспечения с бессрочной лицензией для коммерческого и государственного секторов, а в программу Open License будут внесены изменения.</span><span class="sxs-lookup"><span data-stu-id="706a8-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-446">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-446">Impacted audience</span></span>

<span data-ttu-id="706a8-447">Коммерческие дистрибьюторы и управляемые торговые посредники, которые ведут продажи в рамках программы Open License, а также все партнеры CSP, предоставляющие программное обеспечение с бессрочной лицензией.</span><span class="sxs-lookup"><span data-stu-id="706a8-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="706a8-448">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-448">Details</span></span>

<span data-ttu-id="706a8-449">В сентябре 2020 г. корпорация Майкрософт [объявила](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) о новых мероприятиях по поддержке цифровой трансформации, которые расширяют возможности партнеров по программе CSP, в том числе о доступе к локальному программному обеспечению для партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="706a8-450">Эти нововведения помогут партнерам в развитии бизнеса и увеличении охвата с помощью лицензий на программное обеспечение в рамках CSP, а также в достижении успеха в современном облачном мире.</span><span class="sxs-lookup"><span data-stu-id="706a8-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="706a8-451">Они также ускорят переход клиентов в облако и предоставят партнерам необходимую гибкость для работы с гибридными облачными средами клиентов.</span><span class="sxs-lookup"><span data-stu-id="706a8-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="706a8-452">В рамках дальнейшей цифровой трансформации мы объявляем о следующих изменениях:</span><span class="sxs-lookup"><span data-stu-id="706a8-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="706a8-453">1 июля 2021 г.: в прейскурант программы Open License не будут добавляться новые SKU, продукты или акции.</span><span class="sxs-lookup"><span data-stu-id="706a8-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="706a8-454">7 июля 2021 г.: в прейскурант программного обеспечения с бессрочной лицензией в рамках CSP будут добавлены два коммерческих предложения (Get Genuine Windows и Visual Studio Professional), а также предложения для государственного сектора (правительственных, образовательных и некоммерческих организаций — см. [объявление](./2020-december.md#9)).</span><span class="sxs-lookup"><span data-stu-id="706a8-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="706a8-455">Прейскурант можно найти в разделе "Программное обеспечение" на странице [Продажи > Цены и предложения](https://partnercenter.microsoft.com/pcv/sales) в Центре партнеров. В этот день он будет опубликован повторно.</span><span class="sxs-lookup"><span data-stu-id="706a8-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="706a8-456">Ссылки на статьи с полными сведениями об изменениях в программах CSP и Open License см. в разделе **Дальнейшие действия** ниже.</span><span class="sxs-lookup"><span data-stu-id="706a8-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-457">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-457">Next Steps:</span></span>

- <span data-ttu-id="706a8-458">Изменения в программе CSP: просмотрите материалы по подготовке [Бессрочное лицензирование ПО в рамках программы "Поставщик облачных решений" (CSP)](https://partner.microsoft.com/resources/collection/software-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="706a8-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="706a8-459">Воспользуйтесь этой [картой готовности](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf), чтобы быстро найти нужную информацию для своей роли.</span><span class="sxs-lookup"><span data-stu-id="706a8-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="706a8-460">Изменения в программе Open License: просмотрите материалы по подготовке [Изменения в программе CSP и в программе Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/).</span><span class="sxs-lookup"><span data-stu-id="706a8-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="706a8-461">Воспользуйтесь этой [картой готовности](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf), чтобы быстро найти нужную информацию для своей роли.</span><span class="sxs-lookup"><span data-stu-id="706a8-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-462">Вопросы</span><span class="sxs-lookup"><span data-stu-id="706a8-462">Questions</span></span>

<span data-ttu-id="706a8-463">С вопросами обращайтесь в соответствующее сообщество CSP в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="706a8-464">Обновление предыдущего объявления о выпуске решения "Оценки" категории "Премиум" — надстройки к диспетчеру соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="706a8-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-465">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-465">Categories</span></span>

- <span data-ttu-id="706a8-466">Дата: 15.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="706a8-467">Рост вашего бизнеса</span><span class="sxs-lookup"><span data-stu-id="706a8-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-468">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-468">Summary</span></span>

<span data-ttu-id="706a8-469">Пробные версии не должны указываться в прейскуранте и будут удалены.</span><span class="sxs-lookup"><span data-stu-id="706a8-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-470">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-470">Impacted audience</span></span>

<span data-ttu-id="706a8-471">Партнеры, заключающие сделки в рамках программы "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="706a8-472">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-472">Details</span></span>

<span data-ttu-id="706a8-473">Пробные версии не должны указываться в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="706a8-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="706a8-474">1 мая 2021 г. они будут удалены из него.</span><span class="sxs-lookup"><span data-stu-id="706a8-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="706a8-475">Первоначальное объявление можно найти [здесь](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="706a8-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="706a8-476">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="706a8-476">Additional resources</span></span>

- [<span data-ttu-id="706a8-477">Безопасность и соответствие требованиям Microsoft 365 E5</span><span class="sxs-lookup"><span data-stu-id="706a8-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="706a8-478">Создание оценок и управление ими в диспетчере соответствия требованиям (Майкрософт) — Центр соответствия Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="706a8-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="706a8-479">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-479">Next steps</span></span>

<span data-ttu-id="706a8-480">Изучите доступные ресурсы и на эту тему поделитесь этой информацией с соответствующими заинтересованными лицами в своей организации.</span><span class="sxs-lookup"><span data-stu-id="706a8-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-481">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-481">Questions?</span></span>

<span data-ttu-id="706a8-482">С любыми вопросами по этим предложениям обращайтесь в соответствующее сообщество в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="706a8-483">Перенос решений из средства вывода на рынок (GTM) для One Commercial Partner (OCP) на коммерческую платформу Майкрософт</span><span class="sxs-lookup"><span data-stu-id="706a8-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-484">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-484">Categories</span></span>

- <span data-ttu-id="706a8-485">Дата: 12.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="706a8-486">Возможности</span><span class="sxs-lookup"><span data-stu-id="706a8-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-487">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-487">Summary</span></span>

<span data-ttu-id="706a8-488">С 29 марта 2021 г. возможности One Commercial Partner (OCP) в средстве вывода на рынок (GTM) будут ограничены.</span><span class="sxs-lookup"><span data-stu-id="706a8-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="706a8-489">Рекомендуем вам перенести свои решения на коммерческую платформу в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-490">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-490">Impacted audience</span></span>

<span data-ttu-id="706a8-491">Организации, ведущие совместные продажи с решениями в OCP GTM.</span><span class="sxs-lookup"><span data-stu-id="706a8-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="706a8-492">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-492">Details</span></span>

<span data-ttu-id="706a8-493">В декабре 2020 г. мы начали переход со средства Microsoft OCP GTM на коммерческую платформу Майкрософт в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="706a8-494">Это позволит расширить возможности коммерческой платформы, на которой вы можете предоставлять свои решения миллионам клиентов, обмениваться информацией с другими специалистами по продажам Майкрософт и партнерами, а также совместно продавать инновационные решения.</span><span class="sxs-lookup"><span data-stu-id="706a8-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="706a8-495">Следующий этап перехода запланирован на 29 марта 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="706a8-496">Именно с этой даты возможности OCP GTM будут ограничены — некоторые поля станут доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="706a8-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="706a8-497">Если вы сейчас ведете совместные продажи с решениями в OCP GTM, рекомендуем вам перенести решения на коммерческую платформу, чтобы воспользоваться всеми ее преимуществами и упростить процесс публикации.</span><span class="sxs-lookup"><span data-stu-id="706a8-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="706a8-498">После перехода на коммерческую платформу Центр партнеров станет основным порталом для публикации и совместных продаж.</span><span class="sxs-lookup"><span data-stu-id="706a8-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="706a8-499">С ее помощью вы сможете ускорить рост бизнеса, расширив охват для продажи своих решений нашим общим клиентам с помощью знакомых вам каналов и возможностей, которые мы используем для продуктов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="706a8-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="706a8-500">[Подробнее о коммерческой платформе.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)</span><span class="sxs-lookup"><span data-stu-id="706a8-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-501">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-501">Next steps</span></span>

- <span data-ttu-id="706a8-502">Если вы еще не переместили свои решения, следуйте инструкциям из [руководства по переходу](/azure/marketplace/co-sell-solution-migration) или посмотрите [видеоучебник с пошаговыми инструкциями](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4), чтобы выполнить все шаги миграции и начать публиковать свои решения на коммерческой платформе.</span><span class="sxs-lookup"><span data-stu-id="706a8-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="706a8-503">Вопросы, касающиеся ограниченных возможностей в OCP GTM, см. в [статье с вопросами и ответами о требованиях к совместным продажам для публикации на коммерческой платформе Майкрософт](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)</span><span class="sxs-lookup"><span data-stu-id="706a8-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="706a8-504">(см. раздел "Ограниченные возможности в OCP GTM с 29 марта 2021 г.).</span><span class="sxs-lookup"><span data-stu-id="706a8-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-505">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-505">Questions?</span></span>

<span data-ttu-id="706a8-506">Если у вас возникнут вопросы или вам потребуется дополнительная информация, обратитесь в [службу поддержки](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="706a8-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="706a8-507">Развертывание новой коммерческой платформы в рамках программы "Поставщик облачных решений" (CSP) для Azure в России</span><span class="sxs-lookup"><span data-stu-id="706a8-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-508">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-508">Categories</span></span>

- <span data-ttu-id="706a8-509">Дата: 10.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="706a8-510">Характеристики</span><span class="sxs-lookup"><span data-stu-id="706a8-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-511">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-511">Impacted audience</span></span>

<span data-ttu-id="706a8-512">Все партнеры в России, заключающие сделки в рамках программы "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="706a8-513">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-513">Details</span></span>

<span data-ttu-id="706a8-514">Начиная с 10 марта 2021 г. мы предоставляем доступ к **новому интерфейсу коммерческой платформы для партнеров по программе CSP, которые работают с Azure в России**.</span><span class="sxs-lookup"><span data-stu-id="706a8-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="706a8-515">Этот интерфейс упростит и улучшит приобретение и использование клиентами служб Azure.</span><span class="sxs-lookup"><span data-stu-id="706a8-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="706a8-516">Он также предоставит партнерам по программе CSP согласованное представление с ценами на коммерческие предложения в Azure, с ценами в долларах США (для согласованности с мировым рынком), данные о датах выставления счетов и доступ к Управлению затратами в Azure.</span><span class="sxs-lookup"><span data-stu-id="706a8-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-517">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-517">Next steps</span></span>

<span data-ttu-id="706a8-518">Мы подготовили несколько ресурсов, которые познакомят вас с новым интерфейсом коммерческой платформы для Azure и содержат дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="706a8-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="706a8-519">Последние вопросы и ответы, презентации, видео и другие материалы можно найти в [коллекции ресурсов с обновлениями по программе CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="706a8-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="706a8-520">Обработка лицензионных ключей и скачивание программного обеспечения в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="706a8-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-521">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-521">Categories</span></span>

- <span data-ttu-id="706a8-522">Дата: 04.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="706a8-523">Возможности</span><span class="sxs-lookup"><span data-stu-id="706a8-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-524">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-524">Summary</span></span>

<span data-ttu-id="706a8-525">Возможность скачивания программного обеспечения и обработки лицензионных ключей в Центре партнеров восстановлена.</span><span class="sxs-lookup"><span data-stu-id="706a8-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-526">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-526">Impacted audience</span></span>

<span data-ttu-id="706a8-527">Все партнеры в рамках программы "Поставщик облачных решений" (CSP), заключающие сделки по заказам на программное обеспечение по бессрочной и серверной подписке через Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="706a8-528">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-528">Details</span></span>

<span data-ttu-id="706a8-529">В ответ на отзывы партнеров мы восстанавливаем возможности Центра партнеров по получению программного обеспечения и лицензионных ключей в рамках заказов на программное обеспечение по бессрочной и серверной подписке.</span><span class="sxs-lookup"><span data-stu-id="706a8-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="706a8-530">Эта возможность будет восстановлена до состояния перед ее удалением 19 января 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="706a8-531">(См. [объявление](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="706a8-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="706a8-532">Учтите, что лицензионные ключи и ссылки на скачивание программного обеспечения — это ценные и востребованные активы интеллектуальной собственности.</span><span class="sxs-lookup"><span data-stu-id="706a8-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="706a8-533">В случае их утечки доступные активации могут быстро закончиться, а работа клиентов и партнеров ухудшится.</span><span class="sxs-lookup"><span data-stu-id="706a8-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-534">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-534">Next steps</span></span>

<span data-ttu-id="706a8-535">Инструкции по использованию и важные рекомендации по распространению ключей программного обеспечения см. в следующих ресурсах:</span><span class="sxs-lookup"><span data-stu-id="706a8-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="706a8-536">Продажа локального программного обеспечения через программу CSP</span><span class="sxs-lookup"><span data-stu-id="706a8-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="706a8-537">[Новое руководство по коммерческим операциям в Центре партнеров](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (см. раздел **Рекомендации по распространению ключей программного обеспечения**).</span><span class="sxs-lookup"><span data-stu-id="706a8-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-538">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-538">Questions?</span></span>

<span data-ttu-id="706a8-539">Если у вас есть дополнительные вопросы по этому уведомлению, обращайтесь в соответствующее сообщество в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="706a8-540">Перенос сделок из Partner Sales Connect (PSC) в Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="706a8-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-541">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-541">Categories</span></span>

- <span data-ttu-id="706a8-542">Дата: 04.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="706a8-543">Возможности</span><span class="sxs-lookup"><span data-stu-id="706a8-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-544">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-544">Summary</span></span>

<span data-ttu-id="706a8-545">С 31 марта 2021 г. портал Partner Sales Connect (PSC) будет доступен только для чтения, поэтому мы настоятельно рекомендуем вам начать перенос сделок из PSC в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-546">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-546">Impacted audience</span></span>

<span data-ttu-id="706a8-547">Партнеры, у которых есть сделки в PSC</span><span class="sxs-lookup"><span data-stu-id="706a8-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="706a8-548">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-548">Details</span></span>

<span data-ttu-id="706a8-549">В рамках нашего общего стремления к развитию **совместные продажи с Майкрософт** — это способ, благодаря которому вы можете **заявить о себе, поделиться своим опытом и расширить круг своих клиентов** для получения положительных результатов работы с клиентами.</span><span class="sxs-lookup"><span data-stu-id="706a8-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="706a8-550">При средней скорости заключения сделки, которая в **3,5 раза выше**, чем обычно, управление совместными продажами в Центре партнеров позволяет вам осуществлять продажи через прямые каналы клиентов, партнеров и специалистов Майкрософт по продажам, а также управлять всей цепочкой клиентов по рекомендации в одном расположении.</span><span class="sxs-lookup"><span data-stu-id="706a8-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="706a8-551">С **31 марта 2021 г.** портал **PSC** будет **доступен только для чтения**, поэтому мы настоятельно рекомендуем вам начать перенос сделок из PSC в Центр партнеров, чтобы использовать следующие улучшенные возможности:</span><span class="sxs-lookup"><span data-stu-id="706a8-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="706a8-552">**более точное направление сделок**, которые вы ведете совместно с Майкрософт, к нужному продавцу в зависимости от типа необходимой вам помощи;</span><span class="sxs-lookup"><span data-stu-id="706a8-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="706a8-553">**предварительная проверка соответствия сделки** для решений, на которые распространяется программа поощрения, а также для соответствия критериям программы ISV Connect, что упрощает процесс утверждения и окончательное подтверждение выполнения (POE);</span><span class="sxs-lookup"><span data-stu-id="706a8-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="706a8-554">**удобный пользовательский интерфейс** для централизованного управления всеми возможными сделками, а также клиентами с подтвержденной потребностью в продукте или услуге компании в рамках совместных продаж.</span><span class="sxs-lookup"><span data-stu-id="706a8-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="706a8-555">Кроме того, недавно мы добавили в Центр партнеров новые функции, которые помогут вам при миграции:</span><span class="sxs-lookup"><span data-stu-id="706a8-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- <span data-ttu-id="706a8-556">[массовые операции для возможных сделок в рамках совместных продаж](../bulk-operations.md);</span><span class="sxs-lookup"><span data-stu-id="706a8-556">[Bulk operations for co-sell opportunities](../bulk-operations.md)</span></span>
- <span data-ttu-id="706a8-557">[функция переноса сделок](../psc-to-pc.md) (см. раздел о **переносе сделок из PSC**).</span><span class="sxs-lookup"><span data-stu-id="706a8-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="706a8-558">Используя возможности совместной продажи в Центре партнеров, ваши специалисты по продажам смогут сосредоточиться на тщательной проработке потенциальных клиентов и возможных сделок, закрытии сделок и создании долгосрочных отношений с клиентами.</span><span class="sxs-lookup"><span data-stu-id="706a8-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="706a8-559">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-559">Next steps</span></span>

<span data-ttu-id="706a8-560">Прочтите [руководство по переходу](../psc-to-pc.md) в Центр партнеров, чтобы получить пошаговые инструкции по переносу сделок из PSC в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="706a8-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-561">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-561">Questions?</span></span>

<span data-ttu-id="706a8-562">Если у вас есть дополнительные вопросы, обращайтесь в [службу поддержки](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="706a8-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="706a8-563">Новые продукты и предложения Microsoft Dynamics 365, которые станут доступны 1 апреля 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-564">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-564">Categories</span></span>

- <span data-ttu-id="706a8-565">Дата: 04.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="706a8-566">Возможности</span><span class="sxs-lookup"><span data-stu-id="706a8-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-567">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-567">Summary</span></span>

<span data-ttu-id="706a8-568">1 апреля 2021 г. корпорация Майкрософт выпустит несколько новых продуктов и предложений в рамках программы "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-569">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-569">Impacted audience</span></span>

<span data-ttu-id="706a8-570">Все партнеры, заключающие сделки в рамках программы "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="706a8-571">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-571">Details</span></span>

<span data-ttu-id="706a8-572">1 апреля 2021 г. корпорация Майкрософт выпустит следующие новые продукты и предложения:</span><span class="sxs-lookup"><span data-stu-id="706a8-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="706a8-573">Power BI Premium на пользователя;</span><span class="sxs-lookup"><span data-stu-id="706a8-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="706a8-574">расширение географии и сегментов для лицензий USL на Customer Voice и Marketing.</span><span class="sxs-lookup"><span data-stu-id="706a8-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="706a8-575">**Power BI Premium на пользователя**</span><span class="sxs-lookup"><span data-stu-id="706a8-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="706a8-576">Майкрософт представит первые предложения Power BI Premium на пользователя.</span><span class="sxs-lookup"><span data-stu-id="706a8-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="706a8-577">Сейчас Power BI Premium продается только в рамках модели на основе емкости.</span><span class="sxs-lookup"><span data-stu-id="706a8-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="706a8-578">Power BI Premium на пользователя предоставляет доступ к возможностям корпоративной бизнес-аналитики и анализа.</span><span class="sxs-lookup"><span data-stu-id="706a8-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="706a8-579">Гибкие возможности лицензирования отдельных рабочих мест предназначены для малых и средних предприятий.</span><span class="sxs-lookup"><span data-stu-id="706a8-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="706a8-580">Дополнительную информацию об этом предложении см. в [сведениях о выпуске Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features).</span><span class="sxs-lookup"><span data-stu-id="706a8-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="706a8-581">**Подробности предложения**</span><span class="sxs-lookup"><span data-stu-id="706a8-581">**Offer details**</span></span>

<span data-ttu-id="706a8-582">Обратите внимание, что название предложения немного отличается от названия предварительной версии, указанного в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="706a8-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="706a8-583">Название предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-583">Offer name</span></span> | <span data-ttu-id="706a8-584">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="706a8-585">Power BI Premium на пользователя</span><span class="sxs-lookup"><span data-stu-id="706a8-585">Power BI Premium Per User</span></span> | <span data-ttu-id="706a8-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="706a8-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="706a8-587">Power BI Premium на пользователя для преподавателей</span><span class="sxs-lookup"><span data-stu-id="706a8-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="706a8-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="706a8-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="706a8-589">Power BI Premium на пользователя для учащихся</span><span class="sxs-lookup"><span data-stu-id="706a8-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="706a8-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="706a8-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="706a8-591">Power BI Premium на пользователя (цены для сотрудников некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="706a8-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="706a8-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="706a8-593">Надстройка Power BI Premium на пользователя</span><span class="sxs-lookup"><span data-stu-id="706a8-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="706a8-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="706a8-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="706a8-595">Надстройка Power BI Premium на пользователя для преподавателей</span><span class="sxs-lookup"><span data-stu-id="706a8-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="706a8-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="706a8-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="706a8-597">Надстройка Power BI Premium на пользователя для учащихся</span><span class="sxs-lookup"><span data-stu-id="706a8-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="706a8-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="706a8-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="706a8-599">Надстройка Power BI Premium на пользователя (цены для сотрудников некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="706a8-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="706a8-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="706a8-601">**Расширение географии и сегментов для лицензий USL на Customer Voice и Marketing**</span><span class="sxs-lookup"><span data-stu-id="706a8-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="706a8-602">Вслед за выпуском в декабре 2020 года в предложения лицензий USL на Dynamics 365 Customer Voice и Marketing добавлены новые страны и дополнительные номера SKU для некоммерческих организаций и образовательных учреждений.</span><span class="sxs-lookup"><span data-stu-id="706a8-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="706a8-603">Название предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-603">Offer name</span></span> | <span data-ttu-id="706a8-604">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="706a8-605">USL на Dynamics 365 Customer Voice (цены для сотрудников некоммерческих организаций)</span><span class="sxs-lookup"><span data-stu-id="706a8-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="706a8-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="706a8-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="706a8-607">USL на Dynamics 365 Customer Voice для преподавателей</span><span class="sxs-lookup"><span data-stu-id="706a8-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="706a8-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="706a8-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="706a8-609">Чтобы узнать больше об этих предложениях, посетите следующие страницы:</span><span class="sxs-lookup"><span data-stu-id="706a8-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="706a8-610">Домашняя страница Dynamics 365 Customer Service Voice</span><span class="sxs-lookup"><span data-stu-id="706a8-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="706a8-611">Домашняя страница Dynamics 365 Marketing</span><span class="sxs-lookup"><span data-stu-id="706a8-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="706a8-612">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-612">Next steps</span></span>

<span data-ttu-id="706a8-613">Изучите доступные ресурсы на эту тему и поделитесь этой информацией с соответствующими заинтересованными лицами в своей организации.</span><span class="sxs-lookup"><span data-stu-id="706a8-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="706a8-614">У вас появились вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-614">Questions?</span></span>

<span data-ttu-id="706a8-615">С любыми вопросами по этим предложениям обращайтесь в соответствующее сообщество в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="706a8-616">Теперь в некоторых наборах доступна Универсальная печать (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="706a8-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="706a8-617">Категории</span><span class="sxs-lookup"><span data-stu-id="706a8-617">Categories</span></span>

- <span data-ttu-id="706a8-618">Дата: 03.03.2021</span><span class="sxs-lookup"><span data-stu-id="706a8-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="706a8-619">Возможности</span><span class="sxs-lookup"><span data-stu-id="706a8-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="706a8-620">Сводка</span><span class="sxs-lookup"><span data-stu-id="706a8-620">Summary</span></span>

<span data-ttu-id="706a8-621">C 1 марта 2021 г. Универсальная печать (Майкрософт) будет доступна для сделок в составе некоторых пакетов Microsoft 365 и в виде отдельной надстройки.</span><span class="sxs-lookup"><span data-stu-id="706a8-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="706a8-622">Затронутая аудитория</span><span class="sxs-lookup"><span data-stu-id="706a8-622">Impacted audience</span></span>

<span data-ttu-id="706a8-623">Все партнеры, заключающие сделки в рамках программы "Поставщик облачных решений" (CSP).</span><span class="sxs-lookup"><span data-stu-id="706a8-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="706a8-624">Сведения</span><span class="sxs-lookup"><span data-stu-id="706a8-624">Details</span></span>

<span data-ttu-id="706a8-625">[Универсальная печать](https://aka.ms/universalprint) — это служба печати Microsoft 365, которая устраняет необходимость в использовании локальных серверов печати и позволяет устройствам Windows печатать на принтерах, зарегистрированных в Azure.</span><span class="sxs-lookup"><span data-stu-id="706a8-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="706a8-626">Она станет доступна для сделок 1 марта 2021 г.</span><span class="sxs-lookup"><span data-stu-id="706a8-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="706a8-627">Сотрудники оценят преимущества в виде печати без драйверов, упрощенного обнаружения принтеров на основе расположения и интуитивно понятный интерфейс печати, для работы с которым не требуется обучение.</span><span class="sxs-lookup"><span data-stu-id="706a8-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="706a8-628">Устройства, подключенные к Azure Active Directory (Azure AD), используют для безопасной печати существующие учетные данные Azure AD.</span><span class="sxs-lookup"><span data-stu-id="706a8-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="706a8-629">Администраторы управляют печатью с помощью портала Azure и могут легко подключаться к принтерам с нативной поддержкой Универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="706a8-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="706a8-630">Универсальную печать можно развернуть на несовместимых принтерах с помощью коннектора универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="706a8-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="706a8-631">После выпуска Универсальная печать будет добавлена в Windows E3, A3, E5 и A5, а также Microsoft 365 BP, F3, E3, A3, E5 и A5.</span><span class="sxs-lookup"><span data-stu-id="706a8-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="706a8-632">**Подробности предложения**</span><span class="sxs-lookup"><span data-stu-id="706a8-632">**Offer details**</span></span>

<span data-ttu-id="706a8-633">Обратите внимание, что название предложения немного отличается от названия предварительной версии, указанного в прейскуранте.</span><span class="sxs-lookup"><span data-stu-id="706a8-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="706a8-634">Название предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-634">Offer name</span></span> | <span data-ttu-id="706a8-635">Идентификатор предложения</span><span class="sxs-lookup"><span data-stu-id="706a8-635">Offer ID</span></span> | <span data-ttu-id="706a8-636">Идентификатор материалов</span><span class="sxs-lookup"><span data-stu-id="706a8-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="706a8-637">Надстройка объема Универсальной печати (500 заданий) — Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="706a8-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="706a8-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="706a8-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="706a8-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="706a8-639">9BI-00004</span></span>   |
| <span data-ttu-id="706a8-640">Надстройка объема Универсальной печати (500 заданий) для преподавателей — Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="706a8-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="706a8-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="706a8-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="706a8-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="706a8-642">9BK-00004</span></span>   |
| <span data-ttu-id="706a8-643">Надстройка объема Универсальной печати (500 заданий) — Windows</span><span class="sxs-lookup"><span data-stu-id="706a8-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="706a8-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="706a8-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="706a8-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="706a8-645">9BI-00002</span></span>   |
| <span data-ttu-id="706a8-646">Надстройка объема Универсальной печати (500 заданий) для преподавателей — Windows</span><span class="sxs-lookup"><span data-stu-id="706a8-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="706a8-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="706a8-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="706a8-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="706a8-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="706a8-649">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="706a8-649">Next steps</span></span>

<span data-ttu-id="706a8-650">Ознакомьтесь с прейскурантом и [обзором Универсальной печати](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="706a8-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="706a8-651">Передайте эти сведения всем соответствующим лицам в своей организации.</span><span class="sxs-lookup"><span data-stu-id="706a8-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="706a8-652">Есть вопросы?</span><span class="sxs-lookup"><span data-stu-id="706a8-652">Questions?</span></span>

<span data-ttu-id="706a8-653">С любыми вопросами по этим предложениям обращайтесь в соответствующее сообщество в Yammer.</span><span class="sxs-lookup"><span data-stu-id="706a8-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
