---
title: Управление расположениями в партнерской учетной записи
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Узнайте, как добавить новое расположение и каким образом идентификатор расположения MPN используется в программах поощрений, бизнес-операциях CSP, подписках и других транзакциях.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702898"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="58841-103">Управление расположениями учетной записи MPN и добавление (удаление) расположения</span><span class="sxs-lookup"><span data-stu-id="58841-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="58841-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="58841-104">**Appropriate roles**</span></span>

- <span data-ttu-id="58841-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="58841-105">Global admin</span></span>
- <span data-ttu-id="58841-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="58841-106">Account admin</span></span>

<span data-ttu-id="58841-107">Идентификатор MPN расположения определяет каждое конкретное расположение компании.</span><span class="sxs-lookup"><span data-stu-id="58841-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="58841-108">Идентификатор MPN расположения используется для регистрации в программах поощрения, выполнения бизнес-транзакций в рамках программы "Поставщик облачных решений" (CSP), а также для других бизнес-транзакций.</span><span class="sxs-lookup"><span data-stu-id="58841-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="58841-109">Глобальный идентификатор MPN используется для нетранзакционных действий, таких как запросы на поддержку.</span><span class="sxs-lookup"><span data-stu-id="58841-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="58841-110">Стандартный сценарий:</span><span class="sxs-lookup"><span data-stu-id="58841-110">The following scenario is typical:</span></span>

<span data-ttu-id="58841-111">Глобальная учетная запись партнера (PGA) компании Contoso расположена в Соединенном Королевстве.</span><span class="sxs-lookup"><span data-stu-id="58841-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="58841-112">PGA — это ее зарегистрированный юридический адрес, а для управления всеми нетранзакционными действиями используется глобальный идентификатор MPN компании.</span><span class="sxs-lookup"><span data-stu-id="58841-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="58841-113">Кроме того, у Contoso есть учетные записи расположения партнеров (PLA), эквивалентные дочерним подразделениям или отделениям, в других местах в Соединенном Королевстве, во Франции и в США.</span><span class="sxs-lookup"><span data-stu-id="58841-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="58841-114">В структуре учетной записи MPN эти PLA представлены в виде уникальных идентификаторов MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="58841-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="58841-115">PLA используются для бизнес-транзакций, например в рамках программы CSP или программ поощрения.</span><span class="sxs-lookup"><span data-stu-id="58841-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="58841-116">Выплаты привязываются к расположениям.</span><span class="sxs-lookup"><span data-stu-id="58841-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="58841-117">Между клиентом CSP и идентификатором расположения MPN существует отношение "один к одному".</span><span class="sxs-lookup"><span data-stu-id="58841-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Структура расположений MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="58841-119">Необходимые условия для добавления новой учетной записи для бизнеса CSP</span><span class="sxs-lookup"><span data-stu-id="58841-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="58841-120">Чтобы добавить новую учетную запись для бизнеса CSP, сначала убедитесь, что выполнены необходимые условия.</span><span class="sxs-lookup"><span data-stu-id="58841-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="58841-121">В стране, где вы хотите вести бизнес CSP, вам потребуется идентификатор MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="58841-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="58841-122">Чтобы создать новое расположение MPN, перейдите по ссылке "Добавить расположение MPN" ниже.</span><span class="sxs-lookup"><span data-stu-id="58841-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="58841-123">Чтобы создать новую регистрацию CSP Indirect Reseller, см. раздел [Работа с косвенными торговыми посредниками](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="58841-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="58841-124">Выполняя вход, обязательно используйте **новые** учетные данные для **новой** учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="58841-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="58841-125">Не используйте существующие учетные данные, так как Центр партнеров определит, что у вас уже есть учетная запись.</span><span class="sxs-lookup"><span data-stu-id="58841-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="58841-126">Примите условия Соглашения с партнером Майкрософт и активируйте учетную запись.</span><span class="sxs-lookup"><span data-stu-id="58841-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="58841-127">Если вы хотите зарегистрироваться в качестве партнера с прямым выставлением счетов, ознакомьтесь с [соответствующими требованиями](direct-partner-new-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="58841-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="58841-128">Просмотр и обновление расположений MPN</span><span class="sxs-lookup"><span data-stu-id="58841-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="58841-129">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home) Центра партнеров, указав учетные данные учетной записи MPN</span><span class="sxs-lookup"><span data-stu-id="58841-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="58841-130">(учетные данные MPN могут отличаться от учетных данных CSP).</span><span class="sxs-lookup"><span data-stu-id="58841-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="58841-131">Щелкните значок **Параметры**, а затем выберите элементы **Параметры учетной записи**, **Профиль организации** и **Юридические уведомления**.</span><span class="sxs-lookup"><span data-stu-id="58841-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="58841-132">Проверьте, не отображается ли на вкладке **Партнер** баннер с сообщением об ошибке и предложением исправить расположения после переноса из PMC.</span><span class="sxs-lookup"><span data-stu-id="58841-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="58841-133">Если расположения не были правильно настроены в PMC и еще не переведены на Центр партнеров, необходимо обновить эти расположения.</span><span class="sxs-lookup"><span data-stu-id="58841-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Снимок экрана: обновление расположения.":::
 
4.  <span data-ttu-id="58841-135">На экране **Review PMC locations** (Проверка расположений PMC) выберите элемент **Обновить**.</span><span class="sxs-lookup"><span data-stu-id="58841-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="58841-136">Измените следующие поля:</span><span class="sxs-lookup"><span data-stu-id="58841-136">Update the following fields:</span></span>

- <span data-ttu-id="58841-137">**Поле имени.** Убедитесь, что имя расположения компании указано правильно.</span><span class="sxs-lookup"><span data-stu-id="58841-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="58841-138">Если отображается сообщение об ошибке со сведениями о том, что имя дублируется, попробуйте заменить его, например с Contoso на Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="58841-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="58841-139">**Поле юридического лица.** Убедитесь, что выбрано юридическое лицо, к которому привязано расположение.</span><span class="sxs-lookup"><span data-stu-id="58841-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="58841-140">**Поля 1 и 2 строки адреса.** Убедитесь, что указан правильный адрес.</span><span class="sxs-lookup"><span data-stu-id="58841-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="58841-141">**Поля города и области, республики, края или округа.** Убедитесь, что указано правильное сочетание города и области, республики, края или округа.</span><span class="sxs-lookup"><span data-stu-id="58841-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="58841-142">Для некоторых стран отображается раскрывающееся меню для выбора области, республики, края или округа, а для других это поле нужно вставлять вручную.</span><span class="sxs-lookup"><span data-stu-id="58841-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="58841-143">**Поле почтового индекса.** Убедитесь, что почтовый индекс соответствует указанной стране, региону, городу или адресу.</span><span class="sxs-lookup"><span data-stu-id="58841-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="58841-144">**Поля основного контактного лица.** Убедитесь, что поля имени и фамилии заполнены, а адрес электронной почты определен как рабочий, а не как личный (например, @outlook.com, @live.com и т. д.).</span><span class="sxs-lookup"><span data-stu-id="58841-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="58841-145">**Поле номера телефона.** Убедитесь, что номер телефона не содержит специальных символов, пробелов или кода страны.</span><span class="sxs-lookup"><span data-stu-id="58841-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="58841-146">Значение, указанное в поле номера телефона, должно содержать не более 10 символов.</span><span class="sxs-lookup"><span data-stu-id="58841-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="58841-147">Если сообщения об ошибке нет, то в разделе **Параметры** последовательно выберите элементы **Параметры учетной записи**, **Профиль организации** и **Идентификаторы**.</span><span class="sxs-lookup"><span data-stu-id="58841-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="58841-148">Найдите идентификатор MPN с типом Location (Расположение), который соответствует стране этой учетной записи CSP. Завершите связывание с помощью этого идентификатора.</span><span class="sxs-lookup"><span data-stu-id="58841-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="58841-149">Если не удается найти идентификатор MPN, соответствующий учетной записи CSP, которую вы хотите использовать, можно добавить новое расположение. Для него будет создан новый идентификатор MPN.</span><span class="sxs-lookup"><span data-stu-id="58841-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="58841-150">См. раздел **Добавление расположения MPN** ниже.</span><span class="sxs-lookup"><span data-stu-id="58841-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="58841-151">Добавление расположения MPN</span><span class="sxs-lookup"><span data-stu-id="58841-151">Add an MPN location</span></span>

1. <span data-ttu-id="58841-152">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="58841-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="58841-153">(Учетные данные MPN могут отличаться от учетных данных CSP.)</span><span class="sxs-lookup"><span data-stu-id="58841-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="58841-154">Учетной записи MPN должны быть присвоены права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="58841-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="58841-155">Щелкните значок **Параметры**, а затем выберите **Параметры учетной записи** и **Профиль организации**.</span><span class="sxs-lookup"><span data-stu-id="58841-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="58841-156">Щелкните **Юридические сведения**, а затем на вкладке **Партнер** выберите **Бизнес-расположения** и **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="58841-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="58841-157">Укажите необходимые сведения, включая название организации, адрес и контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="58841-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="58841-158">Щелкните **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="58841-158">Click **Add location**.</span></span> <span data-ttu-id="58841-159">При этом будет создан новый идентификатор MPN для нового расположения, которое можно использовать для транзакций и программы поощрения CSP.</span><span class="sxs-lookup"><span data-stu-id="58841-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Добавление нового юридического лица":::

> [!NOTE]
> <span data-ttu-id="58841-161">После добавления расположения в Центр партнеров его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="58841-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="58841-162">Если вы использовали для входа правильный идентификатор MPN, в Центре партнеров в меню слева отобразится пункт **MPN**.</span><span class="sxs-lookup"><span data-stu-id="58841-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="58841-163">Добавление кода регистрации</span><span class="sxs-lookup"><span data-stu-id="58841-163">Add the registration number ID</span></span>

<span data-ttu-id="58841-164">Если вы являетесь косвенным поставщиком, партнером с прямым выставлением счетов или косвенным торговым посредником и ведете бизнес с новыми или существующими клиентами в перечисленных ниже странах, вам нужно указать код регистрации своей компании.</span><span class="sxs-lookup"><span data-stu-id="58841-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="58841-165">Если страна, в которой вы ведете бизнес, не указана ниже, вводить код регистрации не обязательно.</span><span class="sxs-lookup"><span data-stu-id="58841-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="58841-166">Армения</span><span class="sxs-lookup"><span data-stu-id="58841-166">Armenia</span></span> 
- <span data-ttu-id="58841-167">Азербайджан</span><span class="sxs-lookup"><span data-stu-id="58841-167">Azerbaijan</span></span> 
- <span data-ttu-id="58841-168">Беларусь</span><span class="sxs-lookup"><span data-stu-id="58841-168">Belarus</span></span> 
- <span data-ttu-id="58841-169">Бразилия</span><span class="sxs-lookup"><span data-stu-id="58841-169">Brazil</span></span> 
- <span data-ttu-id="58841-170">Венгрия</span><span class="sxs-lookup"><span data-stu-id="58841-170">Hungary</span></span> 
- <span data-ttu-id="58841-171">Индия</span><span class="sxs-lookup"><span data-stu-id="58841-171">India</span></span> 
- <span data-ttu-id="58841-172">Ирак</span><span class="sxs-lookup"><span data-stu-id="58841-172">Iraq</span></span> 
- <span data-ttu-id="58841-173">Казахстан</span><span class="sxs-lookup"><span data-stu-id="58841-173">Kazakhstan</span></span> 
- <span data-ttu-id="58841-174">Киргизстан</span><span class="sxs-lookup"><span data-stu-id="58841-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="58841-175">Молдова</span><span class="sxs-lookup"><span data-stu-id="58841-175">Moldova</span></span> 
- <span data-ttu-id="58841-176">Мьянма</span><span class="sxs-lookup"><span data-stu-id="58841-176">Myanmar</span></span> 
- <span data-ttu-id="58841-177">Польша</span><span class="sxs-lookup"><span data-stu-id="58841-177">Poland</span></span> 
- <span data-ttu-id="58841-178">Россия</span><span class="sxs-lookup"><span data-stu-id="58841-178">Russia</span></span> 
- <span data-ttu-id="58841-179">Саудовская Аравия</span><span class="sxs-lookup"><span data-stu-id="58841-179">Saudi Arabia</span></span> 
- <span data-ttu-id="58841-180">ЮАР</span><span class="sxs-lookup"><span data-stu-id="58841-180">South Africa</span></span> 
- <span data-ttu-id="58841-181">Южный Судан</span><span class="sxs-lookup"><span data-stu-id="58841-181">South Sudan</span></span>  
- <span data-ttu-id="58841-182">Таджикистан</span><span class="sxs-lookup"><span data-stu-id="58841-182">Tajikistan</span></span> 
- <span data-ttu-id="58841-183">Таиланд</span><span class="sxs-lookup"><span data-stu-id="58841-183">Thailand</span></span>
- <span data-ttu-id="58841-184">Турция</span><span class="sxs-lookup"><span data-stu-id="58841-184">Turkey</span></span> 
- <span data-ttu-id="58841-185">Украина</span><span class="sxs-lookup"><span data-stu-id="58841-185">Ukraine</span></span> 
- <span data-ttu-id="58841-186">ОАЭ</span><span class="sxs-lookup"><span data-stu-id="58841-186">United Arab Emirates</span></span> 
- <span data-ttu-id="58841-187">Узбекистан</span><span class="sxs-lookup"><span data-stu-id="58841-187">Uzbekistan</span></span> 
- <span data-ttu-id="58841-188">Венесуэла</span><span class="sxs-lookup"><span data-stu-id="58841-188">Venezuela</span></span>
- <span data-ttu-id="58841-189">Вьетнам</span><span class="sxs-lookup"><span data-stu-id="58841-189">Vietnam</span></span> 


<span data-ttu-id="58841-190">Дополнительные сведения см. в статье [Сведения о коде регистрации](reg-number-id.md).</span><span class="sxs-lookup"><span data-stu-id="58841-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="58841-191">Удаление расположения</span><span class="sxs-lookup"><span data-stu-id="58841-191">Delete a location</span></span>

<span data-ttu-id="58841-192">Чтобы удалить расположение из учетной записи, необходимо обратиться в [службу поддержки партнеров](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="58841-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="58841-193">Вы должны понимать последствия этого действия.</span><span class="sxs-lookup"><span data-stu-id="58841-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="58841-194">Сведения об удаленных расположениях нельзя получить, и все, что связано с этим конкретным идентификатором MPN, больше не будет распознаваться и будет неактивно для вашей компании.</span><span class="sxs-lookup"><span data-stu-id="58841-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="58841-195">Изменение страны глобальной учетной записи партнера</span><span class="sxs-lookup"><span data-stu-id="58841-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="58841-196">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="58841-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="58841-197">(Учетные данные MPN могут отличаться от учетных данных CSP.)</span><span class="sxs-lookup"><span data-stu-id="58841-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="58841-198">Учетной записи MPN должны быть присвоены права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="58841-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="58841-199">На вкладке **Партнер** перейдите в раздел **Расположения офисов организации** и проверьте список расположений, чтобы убедиться, что в нем указано расположение вашего юридического лица.</span><span class="sxs-lookup"><span data-stu-id="58841-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="58841-200">Чтобы добавить расположение, щелкните **Добавить расположение** и во всплывающем элементе управления укажите необходимые сведения, включая название организации, адрес и основное контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="58841-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="58841-201">Выберите **Изменить страну** рядом с раскрывающимся списком **Страна или регион** и выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="58841-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Всплывающий элемент управления с данными профиля юридического лица":::

5. <span data-ttu-id="58841-203">Нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="58841-203">Click **Save**.</span></span>

6. <span data-ttu-id="58841-204">Страна глобальной учетной записи MPN будет изменена на новую страну.</span><span class="sxs-lookup"><span data-stu-id="58841-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="58841-205">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="58841-205">Next steps</span></span>

- <span data-ttu-id="58841-206">Ознакомьтесь с [процессом проверки](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="58841-206">Learn about the [verification process](verification-responses.md).</span></span>
