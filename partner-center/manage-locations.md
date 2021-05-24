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
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151786"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="6b086-103">Управление расположениями учетной записи MPN и добавление (удаление) расположения</span><span class="sxs-lookup"><span data-stu-id="6b086-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="6b086-104">**Соответствующие роли:** глобальный администратор | администратор учетной записи</span><span class="sxs-lookup"><span data-stu-id="6b086-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="6b086-105">Идентификатор MPN расположения определяет каждое конкретное расположение компании.</span><span class="sxs-lookup"><span data-stu-id="6b086-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="6b086-106">Идентификатор MPN расположения используется для регистрации в программах поощрения, выполнения бизнес-транзакций в рамках программы "Поставщик облачных решений" (CSP), а также для других бизнес-транзакций.</span><span class="sxs-lookup"><span data-stu-id="6b086-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="6b086-107">Глобальный идентификатор MPN используется для нетранзакционных действий, таких как запросы на поддержку.</span><span class="sxs-lookup"><span data-stu-id="6b086-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="6b086-108">Стандартный сценарий:</span><span class="sxs-lookup"><span data-stu-id="6b086-108">The following scenario is typical:</span></span>

<span data-ttu-id="6b086-109">Глобальная учетная запись партнера (PGA) компании Contoso расположена в Соединенном Королевстве.</span><span class="sxs-lookup"><span data-stu-id="6b086-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="6b086-110">PGA — это ее зарегистрированный юридический адрес, а для управления всеми нетранзакционными действиями используется глобальный идентификатор MPN компании.</span><span class="sxs-lookup"><span data-stu-id="6b086-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="6b086-111">Кроме того, у Contoso есть учетные записи расположения партнеров (PLA), эквивалентные дочерним подразделениям или отделениям, в других местах в Соединенном Королевстве, во Франции и в США.</span><span class="sxs-lookup"><span data-stu-id="6b086-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="6b086-112">В структуре учетной записи MPN эти PLA представлены в виде уникальных идентификаторов MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="6b086-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="6b086-113">PLA используются для бизнес-транзакций, например в рамках программы CSP или программ поощрения.</span><span class="sxs-lookup"><span data-stu-id="6b086-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="6b086-114">Выплаты привязываются к расположениям.</span><span class="sxs-lookup"><span data-stu-id="6b086-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="6b086-115">Между клиентом CSP и идентификатором расположения MPN существует отношение "один к одному".</span><span class="sxs-lookup"><span data-stu-id="6b086-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Структура расположений MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="6b086-117">Необходимые условия для добавления новой учетной записи для бизнеса CSP</span><span class="sxs-lookup"><span data-stu-id="6b086-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="6b086-118">Чтобы добавить новую учетную запись для бизнеса CSP, сначала убедитесь, что выполнены необходимые условия.</span><span class="sxs-lookup"><span data-stu-id="6b086-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="6b086-119">В стране, где вы хотите вести бизнес CSP, вам потребуется идентификатор MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="6b086-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="6b086-120">Чтобы создать новое расположение MPN, перейдите по ссылке "Добавить расположение MPN" ниже.</span><span class="sxs-lookup"><span data-stu-id="6b086-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="6b086-121">Чтобы создать новую регистрацию CSP Indirect Reseller, см. раздел [Работа с косвенными торговыми посредниками](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="6b086-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="6b086-122">Выполняя вход, обязательно используйте **новые** учетные данные для **новой** учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="6b086-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="6b086-123">Не используйте существующие учетные данные, так как Центр партнеров определит, что у вас уже есть учетная запись.</span><span class="sxs-lookup"><span data-stu-id="6b086-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="6b086-124">Примите условия Соглашения с партнером Майкрософт и активируйте учетную запись.</span><span class="sxs-lookup"><span data-stu-id="6b086-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="6b086-125">Если вы хотите зарегистрироваться в качестве партнера с прямым выставлением счетов, ознакомьтесь с [соответствующими требованиями](direct-partner-new-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="6b086-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="6b086-126">Просмотр и обновление расположений MPN</span><span class="sxs-lookup"><span data-stu-id="6b086-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="6b086-127">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home) Центра партнеров, указав учетные данные учетной записи MPN</span><span class="sxs-lookup"><span data-stu-id="6b086-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="6b086-128">(учетные данные MPN могут отличаться от учетных данных CSP).</span><span class="sxs-lookup"><span data-stu-id="6b086-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="6b086-129">Щелкните значок **Параметры**, а затем выберите элементы **Параметры учетной записи**, **Профиль организации** и **Юридические уведомления**.</span><span class="sxs-lookup"><span data-stu-id="6b086-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="6b086-130">Проверьте, не отображается ли на вкладке **Партнер** баннер с сообщением об ошибке и предложением исправить расположения после переноса из PMC.</span><span class="sxs-lookup"><span data-stu-id="6b086-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="6b086-131">Если расположения не были правильно настроены в PMC и еще не переведены на Центр партнеров, необходимо обновить эти расположения.</span><span class="sxs-lookup"><span data-stu-id="6b086-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Снимок экрана: обновление расположения.":::
 
4.  <span data-ttu-id="6b086-133">На экране **Review PMC locations** (Проверка расположений PMC) выберите элемент **Обновить**.</span><span class="sxs-lookup"><span data-stu-id="6b086-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="6b086-134">Измените следующие поля:</span><span class="sxs-lookup"><span data-stu-id="6b086-134">Update the following fields:</span></span>

- <span data-ttu-id="6b086-135">**Поле имени.** Убедитесь, что имя расположения компании указано правильно.</span><span class="sxs-lookup"><span data-stu-id="6b086-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="6b086-136">Если отображается сообщение об ошибке со сведениями о том, что имя дублируется, попробуйте заменить его, например с Contoso на Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="6b086-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="6b086-137">**Поле юридического лица.** Убедитесь, что выбрано юридическое лицо, к которому привязано расположение.</span><span class="sxs-lookup"><span data-stu-id="6b086-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="6b086-138">**Поля 1 и 2 строки адреса.** Убедитесь, что указан правильный адрес.</span><span class="sxs-lookup"><span data-stu-id="6b086-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="6b086-139">**Поля города и области, республики, края или округа.** Убедитесь, что указано правильное сочетание города и области, республики, края или округа.</span><span class="sxs-lookup"><span data-stu-id="6b086-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="6b086-140">Для некоторых стран отображается раскрывающееся меню для выбора области, республики, края или округа, а для других это поле нужно вставлять вручную.</span><span class="sxs-lookup"><span data-stu-id="6b086-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="6b086-141">**Поле почтового индекса.** Убедитесь, что почтовый индекс соответствует указанной стране, региону, городу или адресу.</span><span class="sxs-lookup"><span data-stu-id="6b086-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="6b086-142">**Поля основного контактного лица.** Убедитесь, что поля имени и фамилии заполнены, а адрес электронной почты определен как рабочий, а не как личный (например, @outlook.com, @live.com и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6b086-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="6b086-143">**Поле номера телефона.** Убедитесь, что номер телефона не содержит специальных символов, пробелов или кода страны.</span><span class="sxs-lookup"><span data-stu-id="6b086-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="6b086-144">Значение, указанное в поле номера телефона, должно содержать не более 10 символов.</span><span class="sxs-lookup"><span data-stu-id="6b086-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="6b086-145">Если сообщения об ошибке нет, то в разделе **Параметры** последовательно выберите элементы **Параметры учетной записи**, **Профиль организации** и **Идентификаторы**.</span><span class="sxs-lookup"><span data-stu-id="6b086-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="6b086-146">Найдите идентификатор MPN с типом Location (Расположение), который соответствует стране этой учетной записи CSP. Завершите связывание с помощью этого идентификатора.</span><span class="sxs-lookup"><span data-stu-id="6b086-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="6b086-147">Если не удается найти идентификатор MPN, соответствующий учетной записи CSP, которую вы хотите использовать, можно добавить новое расположение. Для него будет создан новый идентификатор MPN.</span><span class="sxs-lookup"><span data-stu-id="6b086-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="6b086-148">См. раздел **Добавление расположения MPN** ниже.</span><span class="sxs-lookup"><span data-stu-id="6b086-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="6b086-149">Добавление расположения MPN</span><span class="sxs-lookup"><span data-stu-id="6b086-149">Add an MPN location</span></span>

1. <span data-ttu-id="6b086-150">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="6b086-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="6b086-151">(Учетные данные MPN могут отличаться от учетных данных CSP.) Учетная запись MPN должна предоставлять права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6b086-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="6b086-152">Щелкните значок **Параметры**, а затем выберите **Параметры учетной записи** и **Профиль организации**.</span><span class="sxs-lookup"><span data-stu-id="6b086-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="6b086-153">Щелкните элемент **Юридические уведомления**, а затем на вкладке **Партнер** последовательно выберите элементы **Расположения офисов организации** и **Добавление расположения**.</span><span class="sxs-lookup"><span data-stu-id="6b086-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="6b086-154">Укажите необходимые сведения, включая название организации, адрес и контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="6b086-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="6b086-155">Выберите **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="6b086-155">Select **Add location**.</span></span> <span data-ttu-id="6b086-156">Будет создан новый идентификатор MPN для нового расположения, которое можно использовать для транзакций и программы поощрения в рамках CSP.</span><span class="sxs-lookup"><span data-stu-id="6b086-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Добавление нового юридического лица":::

> [!NOTE]
> <span data-ttu-id="6b086-158">После добавления расположения в Центр партнеров его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="6b086-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="6b086-159">Если вы использовали для входа правильный идентификатор MPN, в Центре партнеров в меню слева отобразится пункт **MPN**.</span><span class="sxs-lookup"><span data-stu-id="6b086-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="6b086-160">Добавление кода регистрации</span><span class="sxs-lookup"><span data-stu-id="6b086-160">Add the registration number ID</span></span>

<span data-ttu-id="6b086-161">Если вы являетесь косвенным поставщиком, партнером с прямым выставлением счетов или косвенным торговым посредником и ведете бизнес с новыми или существующими клиентами в перечисленных ниже странах, вам нужно указать код регистрации своей компании.</span><span class="sxs-lookup"><span data-stu-id="6b086-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="6b086-162">Если страна, в которой вы ведете бизнес, не указана ниже, указывать код регистрации не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6b086-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="6b086-163">Армения</span><span class="sxs-lookup"><span data-stu-id="6b086-163">Armenia</span></span> 
- <span data-ttu-id="6b086-164">Азербайджан</span><span class="sxs-lookup"><span data-stu-id="6b086-164">Azerbaijan</span></span> 
- <span data-ttu-id="6b086-165">Беларусь</span><span class="sxs-lookup"><span data-stu-id="6b086-165">Belarus</span></span> 
- <span data-ttu-id="6b086-166">Бразилия</span><span class="sxs-lookup"><span data-stu-id="6b086-166">Brazil</span></span> 
- <span data-ttu-id="6b086-167">Венгрия</span><span class="sxs-lookup"><span data-stu-id="6b086-167">Hungary</span></span> 
- <span data-ttu-id="6b086-168">Индия</span><span class="sxs-lookup"><span data-stu-id="6b086-168">India</span></span> 
- <span data-ttu-id="6b086-169">Ирак</span><span class="sxs-lookup"><span data-stu-id="6b086-169">Iraq</span></span> 
- <span data-ttu-id="6b086-170">Казахстан</span><span class="sxs-lookup"><span data-stu-id="6b086-170">Kazakhstan</span></span> 
- <span data-ttu-id="6b086-171">Киргизстан</span><span class="sxs-lookup"><span data-stu-id="6b086-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="6b086-172">Молдова</span><span class="sxs-lookup"><span data-stu-id="6b086-172">Moldova</span></span> 
- <span data-ttu-id="6b086-173">Мьянма</span><span class="sxs-lookup"><span data-stu-id="6b086-173">Myanmar</span></span> 
- <span data-ttu-id="6b086-174">Польша</span><span class="sxs-lookup"><span data-stu-id="6b086-174">Poland</span></span> 
- <span data-ttu-id="6b086-175">Россия</span><span class="sxs-lookup"><span data-stu-id="6b086-175">Russia</span></span> 
- <span data-ttu-id="6b086-176">Саудовская Аравия</span><span class="sxs-lookup"><span data-stu-id="6b086-176">Saudi Arabia</span></span> 
- <span data-ttu-id="6b086-177">Южно-Африканская Республика</span><span class="sxs-lookup"><span data-stu-id="6b086-177">South Africa</span></span> 
- <span data-ttu-id="6b086-178">Южный Судан</span><span class="sxs-lookup"><span data-stu-id="6b086-178">South Sudan</span></span>  
- <span data-ttu-id="6b086-179">Таджикистан</span><span class="sxs-lookup"><span data-stu-id="6b086-179">Tajikistan</span></span> 
- <span data-ttu-id="6b086-180">Таиланд</span><span class="sxs-lookup"><span data-stu-id="6b086-180">Thailand</span></span>
- <span data-ttu-id="6b086-181">Турция</span><span class="sxs-lookup"><span data-stu-id="6b086-181">Turkey</span></span> 
- <span data-ttu-id="6b086-182">Украина</span><span class="sxs-lookup"><span data-stu-id="6b086-182">Ukraine</span></span> 
- <span data-ttu-id="6b086-183">ОАЭ</span><span class="sxs-lookup"><span data-stu-id="6b086-183">United Arab Emirates</span></span> 
- <span data-ttu-id="6b086-184">Узбекистан</span><span class="sxs-lookup"><span data-stu-id="6b086-184">Uzbekistan</span></span> 
- <span data-ttu-id="6b086-185">Венесуэла</span><span class="sxs-lookup"><span data-stu-id="6b086-185">Venezuela</span></span>
- <span data-ttu-id="6b086-186">Вьетнам</span><span class="sxs-lookup"><span data-stu-id="6b086-186">Vietnam</span></span> 


<span data-ttu-id="6b086-187">Дополнительные сведения см. в статье [Сведения о коде регистрации](reg-number-id.md).</span><span class="sxs-lookup"><span data-stu-id="6b086-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="6b086-188">Удаление расположения</span><span class="sxs-lookup"><span data-stu-id="6b086-188">Delete a location</span></span>

<span data-ttu-id="6b086-189">Чтобы удалить расположение из учетной записи, необходимо обратиться в [службу поддержки партнеров](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="6b086-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="6b086-190">Вы должны понимать последствия этого действия.</span><span class="sxs-lookup"><span data-stu-id="6b086-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="6b086-191">Сведения об удаленных расположениях нельзя получить, и все, что связано с этим конкретным идентификатором MPN, больше не будет распознаваться и будет неактивно для вашей компании.</span><span class="sxs-lookup"><span data-stu-id="6b086-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="6b086-192">Изменение страны глобальной учетной записи партнера</span><span class="sxs-lookup"><span data-stu-id="6b086-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="6b086-193">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="6b086-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="6b086-194">(Учетные данные MPN могут отличаться от учетных данных CSP.) Учетная запись MPN должна предоставлять права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6b086-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="6b086-195">На вкладке **Партнер** перейдите в раздел **Расположения офисов организации** и проверьте список расположений, чтобы убедиться, что в нем указано расположение вашего юридического лица.</span><span class="sxs-lookup"><span data-stu-id="6b086-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="6b086-196">Чтобы добавить расположение, щелкните **Добавить расположение** и во всплывающем элементе управления укажите необходимые сведения, включая название организации, адрес и основное контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="6b086-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="6b086-197">Выберите элемент **Изменить страну** рядом с раскрывающимся списком **Страна или регион** и выполните описанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="6b086-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Всплывающий элемент управления с данными профиля юридического лица":::

5. <span data-ttu-id="6b086-199">Щелкните **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="6b086-199">Select **Save**.</span></span>

6. <span data-ttu-id="6b086-200">Страна глобальной учетной записи MPN будет изменена на новую страну.</span><span class="sxs-lookup"><span data-stu-id="6b086-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="6b086-201">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="6b086-201">Next steps</span></span>

- <span data-ttu-id="6b086-202">Ознакомьтесь с [процессом проверки](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="6b086-202">Learn about the [verification process](verification-responses.md).</span></span>
