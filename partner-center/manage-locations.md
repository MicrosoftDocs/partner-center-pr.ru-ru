---
title: Управление расположениями в партнерской учетной записи
ms.topic: how-to
ms.date: 02/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Узнайте, как добавить новое расположение и каким образом идентификатор расположения MPN используется в программах поощрений, бизнес-операциях CSP, подписках и других транзакциях.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c5ac31b772c6757468c5ea9d463643731571b31f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624278"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="e0ed7-103">Управление расположениями учетной записи MPN и добавление нового расположения</span><span class="sxs-lookup"><span data-stu-id="e0ed7-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="e0ed7-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="e0ed7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e0ed7-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e0ed7-105">Global admin</span></span>
- <span data-ttu-id="e0ed7-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="e0ed7-106">Account admin</span></span>

<span data-ttu-id="e0ed7-107">Идентификатор MPN расположения определяет каждое конкретное расположение компании.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="e0ed7-108">Идентификатор MPN расположения используется для регистрации в программах поощрения, выполнения бизнес-транзакций в рамках программы "Поставщик облачных решений" (CSP), а также для других бизнес-транзакций.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="e0ed7-109">Глобальный идентификатор MPN используется для нетранзакционных действий, таких как запросы на поддержку.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="e0ed7-110">Ниже приведен типичный сценарий:</span><span class="sxs-lookup"><span data-stu-id="e0ed7-110">The following is a typical scenario:</span></span>

<span data-ttu-id="e0ed7-111">Глобальная учетная запись партнера (PGA) компании Contoso расположена в Соединенном Королевстве.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="e0ed7-112">Это ее зарегистрированный юридический адрес, а для управления всеми нетранзакционными действиями используется глобальный идентификатор MPN компании.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="e0ed7-113">Кроме того, у Contoso есть учетные записи расположения партнеров (PLA), эквивалентные дочерним подразделениям или отделениям, в других местах в Соединенном Королевстве, во Франции и в США.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="e0ed7-114">В структуре учетной записи MPN эти PLA представлены в виде уникальных идентификаторов MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="e0ed7-115">PLA используются для бизнес-транзакций, например в рамках программы CSP или программ поощрения.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="e0ed7-116">Выплаты привязываются к расположениям.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="e0ed7-117">Между клиентом CSP и идентификатором расположения MPN существует отношение "один к одному".</span><span class="sxs-lookup"><span data-stu-id="e0ed7-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Структура расположений MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="e0ed7-119">Необходимые условия для добавления новой учетной записи для бизнеса CSP</span><span class="sxs-lookup"><span data-stu-id="e0ed7-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="e0ed7-120">Чтобы добавить новую учетную запись для бизнеса CSP, сначала убедитесь, что выполнены необходимые условия.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="e0ed7-121">В стране, где вы хотите вести бизнес CSP, вам потребуется идентификатор MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="e0ed7-122">Чтобы создать новое расположение MPN, перейдите по ссылке "Добавить расположение MPN" ниже.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="e0ed7-123">Чтобы создать новую регистрацию CSP Indirect Reseller, см. раздел [Работа с косвенными торговыми посредниками](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="e0ed7-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="e0ed7-124">Выполняя вход, обязательно используйте **новые** учетные данные для **новой** учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="e0ed7-125">Не используйте существующие учетные данные, так как Центр партнеров определит, что у вас уже есть учетная запись.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="e0ed7-126">Примите условия Соглашения с партнером Майкрософт и активируйте учетную запись.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="e0ed7-127">Если вы хотите зарегистрироваться в качестве партнера с прямым выставлением счетов, ознакомьтесь с [соответствующими требованиями](direct-partner-new-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="e0ed7-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="e0ed7-128">Просмотр расположений MPN</span><span class="sxs-lookup"><span data-stu-id="e0ed7-128">View your MPN locations</span></span>

1. <span data-ttu-id="e0ed7-129">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home) Центра партнеров, указав учетные данные учетной записи MPN</span><span class="sxs-lookup"><span data-stu-id="e0ed7-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="e0ed7-130">(учетные данные MPN могут отличаться от учетных данных CSP).</span><span class="sxs-lookup"><span data-stu-id="e0ed7-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="e0ed7-131">Щелкните значок **Параметры**, а затем выберите элементы **Параметры учетной записи**, **Профиль организации** и **Юридические уведомления**.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="e0ed7-132">Проверьте, не отображается ли на вкладке **Партнер** баннер с сообщением об ошибке и предложением исправить расположения после переноса из PMC.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="e0ed7-133">Если это так, выполните инструкции по исправлению этих расположений.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="e0ed7-134">Если сообщения об ошибке нет, то в разделе **Параметры** последовательно выберите элементы **Параметры учетной записи**, **Профиль организации** и **Идентификаторы**.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="e0ed7-135">Найдите идентификатор MPN с типом Location (Расположение), который соответствует стране этой учетной записи CSP. Выполните по нему поиск (ниже) и завершите связывание.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="e0ed7-136">Если не удается найти идентификатор MPN, соответствующий учетной записи CSP, которую вы хотите использовать, можно добавить новое расположение. Для него будет создан новый идентификатор MPN.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="e0ed7-137">См. раздел **Добавление расположения MPN** ниже.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="e0ed7-138">Добавление расположения MPN</span><span class="sxs-lookup"><span data-stu-id="e0ed7-138">Add an MPN location</span></span>

1. <span data-ttu-id="e0ed7-139">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e0ed7-140">(Учетные данные MPN могут отличаться от учетных данных CSP.)</span><span class="sxs-lookup"><span data-stu-id="e0ed7-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e0ed7-141">Учетной записи MPN должны быть присвоены права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="e0ed7-142">Щелкните значок **Параметры**, а затем выберите **Параметры учетной записи** и **Профиль организации**.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="e0ed7-143">Щелкните **Юридические сведения**, а затем на вкладке **Партнер** выберите **Бизнес-расположения** и **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="e0ed7-144">Укажите необходимые сведения, включая название организации, адрес и контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="e0ed7-145">Щелкните **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-145">Click **Add location**.</span></span> <span data-ttu-id="e0ed7-146">При этом будет создан новый идентификатор MPN для нового расположения, которое можно использовать для транзакций и программы поощрения CSP.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Добавление нового юридического лица":::

> [!NOTE]
> <span data-ttu-id="e0ed7-148">После добавления расположения в Центр партнеров его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-148">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="e0ed7-149">Если вы использовали для входа правильный идентификатор MPN, в Центре партнеров в меню слева отобразится пункт **MPN**.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="e0ed7-150">Изменение страны глобальной учетной записи партнера</span><span class="sxs-lookup"><span data-stu-id="e0ed7-150">Change country of Partner global account</span></span> 

1. <span data-ttu-id="e0ed7-151">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-151">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e0ed7-152">(Учетные данные MPN могут отличаться от учетных данных CSP.)</span><span class="sxs-lookup"><span data-stu-id="e0ed7-152">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e0ed7-153">Учетной записи MPN должны быть присвоены права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-153">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="e0ed7-154">На вкладке **Партнер** перейдите в раздел **Расположения офисов организации** и проверьте список расположений, чтобы убедиться, что в нем указано расположение вашего юридического лица.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-154">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="e0ed7-155">Чтобы добавить расположение, щелкните **Добавить расположение** и во всплывающем элементе управления укажите необходимые сведения, включая название организации, адрес и основное контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-155">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="e0ed7-156">Выберите **Изменить страну** рядом с раскрывающимся списком **Страна или регион** и выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-156">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Всплывающий элемент управления с данными профиля юридического лица":::

5. <span data-ttu-id="e0ed7-158">Нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-158">Click **Save**.</span></span>

6. <span data-ttu-id="e0ed7-159">Страна глобальной учетной записи MPN будет изменена на новую страну.</span><span class="sxs-lookup"><span data-stu-id="e0ed7-159">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="e0ed7-160">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e0ed7-160">Next steps</span></span>

- <span data-ttu-id="e0ed7-161">Ознакомьтесь с [процессом проверки](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="e0ed7-161">Learn about the [verification process](verification-responses.md).</span></span>
