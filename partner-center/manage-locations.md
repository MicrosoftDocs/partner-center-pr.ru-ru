---
title: Управление расположениями в партнерской учетной записи
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Узнайте, как добавить новое расположение и каким образом идентификатор расположения MPN используется в программах поощрений, бизнес-операциях CSP, подписках и других транзакциях.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663903"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="85c66-103">Управление расположениями учетной записи MPN и добавление нового расположения</span><span class="sxs-lookup"><span data-stu-id="85c66-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="85c66-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="85c66-104">**Applies to**</span></span>

- <span data-ttu-id="85c66-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="85c66-105">Partner Center</span></span>

<span data-ttu-id="85c66-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="85c66-106">**Appropriate roles**</span></span>

- <span data-ttu-id="85c66-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="85c66-107">Global admin</span></span>
- <span data-ttu-id="85c66-108">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="85c66-108">Account admin</span></span>

<span data-ttu-id="85c66-109">Идентификатор MPN расположения определяет каждое конкретное расположение компании.</span><span class="sxs-lookup"><span data-stu-id="85c66-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="85c66-110">Идентификатор MPN расположения используется для регистрации в программах поощрения, выполнения бизнес-транзакций в рамках программы "Поставщик облачных решений" (CSP), а также для других бизнес-транзакций.</span><span class="sxs-lookup"><span data-stu-id="85c66-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="85c66-111">Глобальный идентификатор MPN используется для нетранзакционных действий, таких как запросы на поддержку.</span><span class="sxs-lookup"><span data-stu-id="85c66-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="85c66-112">Ниже приведен типичный сценарий:</span><span class="sxs-lookup"><span data-stu-id="85c66-112">The following is a typical scenario:</span></span>

<span data-ttu-id="85c66-113">Глобальная учетная запись партнера (PGA) компании Contoso расположена в Соединенном Королевстве.</span><span class="sxs-lookup"><span data-stu-id="85c66-113">Contoso has its Partner global account (PGA) location in the UK.</span></span> <span data-ttu-id="85c66-114">Это ее зарегистрированный юридический адрес. У компании нее есть один идентификатор MPN, используемый для управления всеми нетранзакционными действиями.</span><span class="sxs-lookup"><span data-stu-id="85c66-114">This is their registered legal business, and it has one MPN ID used for managing all non-transactional business.</span></span> <span data-ttu-id="85c66-115">Кроме того, у Contoso есть учетные записи расположения партнеров (PLA), эквивалентные дочерним подразделениям или отделениям, в других местах в Соединенном Королевстве, во Франции и в США.</span><span class="sxs-lookup"><span data-stu-id="85c66-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="85c66-116">В структуре учетной записи MPN эти PLA представлены в виде уникальных идентификаторов MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="85c66-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="85c66-117">PLA используются для бизнес-транзакций, например в рамках программы CSP или программ поощрения.</span><span class="sxs-lookup"><span data-stu-id="85c66-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="85c66-118">Выплаты привязываются к расположениям.</span><span class="sxs-lookup"><span data-stu-id="85c66-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="85c66-119">Между клиентом CSP и идентификатором расположения MPN существует отношение "один к одному".</span><span class="sxs-lookup"><span data-stu-id="85c66-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="Структура расположений MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="85c66-121">Необходимые условия для добавления нового расположения для бизнеса CSP</span><span class="sxs-lookup"><span data-stu-id="85c66-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="85c66-122">Чтобы добавить новое расположение для бизнеса CSP, необходимо выполнить несколько предварительных условий.</span><span class="sxs-lookup"><span data-stu-id="85c66-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="85c66-123">В стране, где вы хотите вести бизнес, требуется идентификатор MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="85c66-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="85c66-124">В регионе ведения бизнеса, еще не зарегистрированном в программе CSP, вам потребуется новый клиент Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85c66-124">You need a new Azure AD tenant in the region of business which is not already enrolled into CSP.</span></span> <span data-ttu-id="85c66-125">Создайте его при регистрации в программе CSP.</span><span class="sxs-lookup"><span data-stu-id="85c66-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="85c66-126">Используйте новый клиент AAD для регистрации в программе CSP в нужном регионе.</span><span class="sxs-lookup"><span data-stu-id="85c66-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="85c66-127">Укажите юридические сведения о компании, включая юридическое название компании, адрес и основное контактное лицо.</span><span class="sxs-lookup"><span data-stu-id="85c66-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="85c66-128">Эта учетная запись будет проверяться, поэтому предоставляйте действительную информацию.</span><span class="sxs-lookup"><span data-stu-id="85c66-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="85c66-129">При входе в систему обязательно используйте **новые** учетные данные для **нового** клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85c66-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="85c66-130">Не используйте существующие учетные данные, так как Центр партнеров определит, что у вас уже есть учетная запись.</span><span class="sxs-lookup"><span data-stu-id="85c66-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="85c66-131">Примите условия Соглашения с партнером Майкрософт и активируйте учетную запись.</span><span class="sxs-lookup"><span data-stu-id="85c66-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="85c66-132">Добавление расположения</span><span class="sxs-lookup"><span data-stu-id="85c66-132">Add a location</span></span>

1. <span data-ttu-id="85c66-133">Щелкните значок **Параметры** и выберите **Параметры партнеров**.</span><span class="sxs-lookup"><span data-stu-id="85c66-133">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="85c66-134">Выберите **Расположения**.</span><span class="sxs-lookup"><span data-stu-id="85c66-134">Select **Locations.**</span></span>

3. <span data-ttu-id="85c66-135">Выберите **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="85c66-135">Select **Add a location**.</span></span>  

4. <span data-ttu-id="85c66-136">На странице **Добавление расположения** введите сведения об адресе расположения, которое требуется добавить в компанию, а также основной контакт для этого расположения.</span><span class="sxs-lookup"><span data-stu-id="85c66-136">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="85c66-137">После добавления расположения в Центр партнеров его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="85c66-137">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="85c66-138">Изменение расположения глобальной учетной записи партнера</span><span class="sxs-lookup"><span data-stu-id="85c66-138">Change Global partner account location</span></span>

1. <span data-ttu-id="85c66-139">На странице **Расположения** проверьте список расположений, чтобы убедиться, что в нем указано расположение вашего юридического лица.</span><span class="sxs-lookup"><span data-stu-id="85c66-139">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="85c66-140">Если это не так, добавьте его.</span><span class="sxs-lookup"><span data-stu-id="85c66-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Структура расположений MPN":::

2. <span data-ttu-id="85c66-142">Выберите **Профиль партнера** и щелкните **Update legal business profile** (Обновить официальный бизнес-профиль).</span><span class="sxs-lookup"><span data-stu-id="85c66-142">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Структура расположений MPN":::

3. <span data-ttu-id="85c66-144">Выберите регион и юридическое лицо, а затем щелкните **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="85c66-144">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Структура расположений MPN":::

## <a name="next-steps"></a><span data-ttu-id="85c66-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="85c66-146">Next steps</span></span>

- <span data-ttu-id="85c66-147">Ознакомьтесь с [процессом проверки](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="85c66-147">Learn about the [verification process](verification-responses.md).</span></span>
