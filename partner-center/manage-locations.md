---
title: Управление расположениями в партнерской учетной записи
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Узнайте, как добавить новое расположение и каким образом идентификатор расположения MPN используется в программах поощрений, бизнес-операциях CSP, подписках и других транзакциях.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925011"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="27b2e-103">Управление расположениями учетной записи MPN и добавление нового расположения</span><span class="sxs-lookup"><span data-stu-id="27b2e-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="27b2e-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="27b2e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="27b2e-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="27b2e-105">Global admin</span></span>
- <span data-ttu-id="27b2e-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="27b2e-106">Account admin</span></span>

<span data-ttu-id="27b2e-107">Идентификатор MPN расположения определяет каждое конкретное расположение компании.</span><span class="sxs-lookup"><span data-stu-id="27b2e-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="27b2e-108">Идентификатор MPN расположения используется для регистрации в программах поощрения, выполнения бизнес-транзакций в рамках программы "Поставщик облачных решений" (CSP), а также для других бизнес-транзакций.</span><span class="sxs-lookup"><span data-stu-id="27b2e-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="27b2e-109">Глобальный идентификатор MPN используется для нетранзакционных действий, таких как запросы на поддержку.</span><span class="sxs-lookup"><span data-stu-id="27b2e-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="27b2e-110">Ниже приведен типичный сценарий:</span><span class="sxs-lookup"><span data-stu-id="27b2e-110">The following is a typical scenario:</span></span>

<span data-ttu-id="27b2e-111">Глобальная учетная запись партнера (PGA) компании Contoso расположена в Соединенном Королевстве.</span><span class="sxs-lookup"><span data-stu-id="27b2e-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="27b2e-112">Это ее зарегистрированный юридический адрес, а для управления всеми нетранзакционными действиями используется глобальный идентификатор MPN компании.</span><span class="sxs-lookup"><span data-stu-id="27b2e-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="27b2e-113">Кроме того, у Contoso есть учетные записи расположения партнеров (PLA), эквивалентные дочерним подразделениям или отделениям, в других местах в Соединенном Королевстве, во Франции и в США.</span><span class="sxs-lookup"><span data-stu-id="27b2e-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="27b2e-114">В структуре учетной записи MPN эти PLA представлены в виде уникальных идентификаторов MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="27b2e-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="27b2e-115">PLA используются для бизнес-транзакций, например в рамках программы CSP или программ поощрения.</span><span class="sxs-lookup"><span data-stu-id="27b2e-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="27b2e-116">Выплаты привязываются к расположениям.</span><span class="sxs-lookup"><span data-stu-id="27b2e-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="27b2e-117">Между клиентом CSP и идентификатором расположения MPN существует отношение "один к одному".</span><span class="sxs-lookup"><span data-stu-id="27b2e-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Структура расположений MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="27b2e-119">Необходимые условия для добавления новой учетной записи для бизнеса CSP</span><span class="sxs-lookup"><span data-stu-id="27b2e-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="27b2e-120">Чтобы добавить новую учетную запись для бизнеса CSP, сначала убедитесь, что выполнены необходимые условия.</span><span class="sxs-lookup"><span data-stu-id="27b2e-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="27b2e-121">В стране, где вы хотите вести бизнес CSP, вам потребуется идентификатор MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="27b2e-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="27b2e-122">Чтобы создать новое расположение MPN, перейдите по ссылке "Добавить расположение MPN" ниже.</span><span class="sxs-lookup"><span data-stu-id="27b2e-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="27b2e-123">Чтобы создать новую регистрацию CSP Indirect Reseller, см. раздел [Работа с косвенными торговыми посредниками](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="27b2e-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="27b2e-124">Выполняя вход, обязательно используйте **новые** учетные данные для **новой** учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="27b2e-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="27b2e-125">Не используйте существующие учетные данные, так как Центр партнеров определит, что у вас уже есть учетная запись.</span><span class="sxs-lookup"><span data-stu-id="27b2e-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="27b2e-126">Примите условия Соглашения с партнером Майкрософт и активируйте учетную запись.</span><span class="sxs-lookup"><span data-stu-id="27b2e-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="27b2e-127">Добавление расположения MPN</span><span class="sxs-lookup"><span data-stu-id="27b2e-127">Add an MPN location</span></span>

1. <span data-ttu-id="27b2e-128">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="27b2e-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="27b2e-129">(Учетные данные MPN могут отличаться от учетных данных CSP.)</span><span class="sxs-lookup"><span data-stu-id="27b2e-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="27b2e-130">Учетной записи MPN должны быть присвоены права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="27b2e-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="27b2e-131">Щелкните значок **Параметры**, а затем выберите **Параметры учетной записи** и **Профиль организации**.</span><span class="sxs-lookup"><span data-stu-id="27b2e-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="27b2e-132">Щелкните **Юридические сведения**, а затем на вкладке **Партнер** выберите **Бизнес-расположения** и **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="27b2e-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="27b2e-133">Укажите необходимые сведения, включая название организации, адрес и контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="27b2e-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="27b2e-134">Щелкните **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="27b2e-134">Click **Add location**.</span></span> <span data-ttu-id="27b2e-135">При этом будет создан новый идентификатор MPN для нового расположения, которое можно использовать для транзакций и программы поощрения CSP.</span><span class="sxs-lookup"><span data-stu-id="27b2e-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Добавление нового юридического лица":::

> [!NOTE]
> <span data-ttu-id="27b2e-137">После добавления расположения в Центр партнеров его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="27b2e-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="27b2e-138">Если вы использовали для входа правильный идентификатор MPN, в Центре партнеров в меню слева отобразится пункт **MPN**.</span><span class="sxs-lookup"><span data-stu-id="27b2e-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="27b2e-139">Изменение страны глобальной учетной записи партнера</span><span class="sxs-lookup"><span data-stu-id="27b2e-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="27b2e-140">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="27b2e-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="27b2e-141">(Учетные данные MPN могут отличаться от учетных данных CSP.)</span><span class="sxs-lookup"><span data-stu-id="27b2e-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="27b2e-142">Учетной записи MPN должны быть присвоены права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="27b2e-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="27b2e-143">На вкладке **Партнер** перейдите в раздел **Расположения офисов организации** и проверьте список расположений, чтобы убедиться, что в нем указано расположение вашего юридического лица.</span><span class="sxs-lookup"><span data-stu-id="27b2e-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="27b2e-144">Чтобы добавить расположение, щелкните **Добавить расположение** и во всплывающем элементе управления укажите необходимые сведения, включая название организации, адрес и основное контактное лицо, для расположения, которое вы хотите добавить для компании.</span><span class="sxs-lookup"><span data-stu-id="27b2e-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="27b2e-145">Выберите **Изменить страну** рядом с раскрывающимся списком **Страна или регион** и выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="27b2e-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Всплывающий элемент управления с данными профиля юридического лица":::

5. <span data-ttu-id="27b2e-147">Нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="27b2e-147">Click **Save**.</span></span>

6. <span data-ttu-id="27b2e-148">Страна глобальной учетной записи MPN будет изменена на новую страну.</span><span class="sxs-lookup"><span data-stu-id="27b2e-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="27b2e-149">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="27b2e-149">Next steps</span></span>

- <span data-ttu-id="27b2e-150">Ознакомьтесь с [процессом проверки](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="27b2e-150">Learn about the [verification process](verification-responses.md).</span></span>
