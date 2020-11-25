---
title: Управление расположениями в партнерской учетной записи
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Узнайте, как добавить новое расположение и каким образом идентификатор расположения MPN используется в программах поощрений, бизнес-операциях CSP, подписках и других транзакциях.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514808"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="c7d01-103">Управление расположениями учетной записи MPN и добавление нового расположения</span><span class="sxs-lookup"><span data-stu-id="c7d01-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="c7d01-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="c7d01-104">**Applies to**</span></span>

- <span data-ttu-id="c7d01-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="c7d01-105">Partner Center</span></span>

<span data-ttu-id="c7d01-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="c7d01-106">**Appropriate roles**</span></span>

- <span data-ttu-id="c7d01-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c7d01-107">Global admin</span></span>
- <span data-ttu-id="c7d01-108">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="c7d01-108">Account admin</span></span>

<span data-ttu-id="c7d01-109">Идентификатор MPN расположения определяет каждое конкретное расположение компании.</span><span class="sxs-lookup"><span data-stu-id="c7d01-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="c7d01-110">Идентификатор MPN расположения используется для регистрации в программах поощрения, выполнения бизнес-транзакций в рамках программы "Поставщик облачных решений" (CSP), а также для других бизнес-транзакций.</span><span class="sxs-lookup"><span data-stu-id="c7d01-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="c7d01-111">Глобальный идентификатор MPN используется для нетранзакционных действий, таких как запросы на поддержку.</span><span class="sxs-lookup"><span data-stu-id="c7d01-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="c7d01-112">Ниже приведен типичный сценарий:</span><span class="sxs-lookup"><span data-stu-id="c7d01-112">The following is a typical scenario:</span></span>

<span data-ttu-id="c7d01-113">Глобальная учетная запись партнера (PGA) компании Contoso расположена в Соединенном Королевстве.</span><span class="sxs-lookup"><span data-stu-id="c7d01-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="c7d01-114">Это ее зарегистрированный юридический адрес, а для управления всеми нетранзакционными действиями используется глобальный идентификатор MPN компании.</span><span class="sxs-lookup"><span data-stu-id="c7d01-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="c7d01-115">Кроме того, у Contoso есть учетные записи расположения партнеров (PLA), эквивалентные дочерним подразделениям или отделениям, в других местах в Соединенном Королевстве, во Франции и в США.</span><span class="sxs-lookup"><span data-stu-id="c7d01-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="c7d01-116">В структуре учетной записи MPN эти PLA представлены в виде уникальных идентификаторов MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="c7d01-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="c7d01-117">PLA используются для бизнес-транзакций, например в рамках программы CSP или программ поощрения.</span><span class="sxs-lookup"><span data-stu-id="c7d01-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="c7d01-118">Выплаты привязываются к расположениям.</span><span class="sxs-lookup"><span data-stu-id="c7d01-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="c7d01-119">Между клиентом CSP и идентификатором расположения MPN существует отношение "один к одному".</span><span class="sxs-lookup"><span data-stu-id="c7d01-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Структура расположений MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="c7d01-121">Необходимые условия для добавления нового расположения для бизнеса CSP</span><span class="sxs-lookup"><span data-stu-id="c7d01-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="c7d01-122">Чтобы добавить новое расположение для бизнеса CSP, необходимо выполнить несколько предварительных условий.</span><span class="sxs-lookup"><span data-stu-id="c7d01-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="c7d01-123">В стране, где вы хотите вести бизнес, требуется идентификатор MPN расположения.</span><span class="sxs-lookup"><span data-stu-id="c7d01-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="c7d01-124">В [регионе ведения бизнеса](regional-authorization-overview.md), еще не зарегистрированном в программе CSP, вам потребуется новый клиент Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7d01-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="c7d01-125">Создайте его при регистрации в программе CSP.</span><span class="sxs-lookup"><span data-stu-id="c7d01-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="c7d01-126">Используйте новый клиент AAD для регистрации в программе CSP в нужном регионе.</span><span class="sxs-lookup"><span data-stu-id="c7d01-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="c7d01-127">Укажите юридические сведения о компании, включая юридическое название компании, адрес и основное контактное лицо.</span><span class="sxs-lookup"><span data-stu-id="c7d01-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="c7d01-128">Эта учетная запись будет проверяться, поэтому предоставляйте действительную информацию.</span><span class="sxs-lookup"><span data-stu-id="c7d01-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="c7d01-129">При входе в систему обязательно используйте **новые** учетные данные для **нового** клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7d01-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="c7d01-130">Не используйте существующие учетные данные, так как Центр партнеров определит, что у вас уже есть учетная запись.</span><span class="sxs-lookup"><span data-stu-id="c7d01-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="c7d01-131">Примите условия Соглашения с партнером Майкрософт и активируйте учетную запись.</span><span class="sxs-lookup"><span data-stu-id="c7d01-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="c7d01-132">Добавление расположения MPN</span><span class="sxs-lookup"><span data-stu-id="c7d01-132">Add an MPN location</span></span>

1. <span data-ttu-id="c7d01-133">Войдите в Центр партнеров, используя учетную запись MPN.</span><span class="sxs-lookup"><span data-stu-id="c7d01-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="c7d01-134">Учетной записи MPN должны быть присвоены права глобального администратора или администратора учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c7d01-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="c7d01-135">Щелкните значок **Параметры** и выберите **Параметры организации**.</span><span class="sxs-lookup"><span data-stu-id="c7d01-135">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="c7d01-136">Выберите элементы **Legal** (Юридическая информация) и **Расположения**.</span><span class="sxs-lookup"><span data-stu-id="c7d01-136">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="c7d01-137">Выберите **Добавление расположения** и введите сведения об адресе расположения, которое требуется добавить для компании, а также основное контактное лицо для этого расположения.</span><span class="sxs-lookup"><span data-stu-id="c7d01-137">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="c7d01-138">После добавления расположения в Центр партнеров его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="c7d01-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="c7d01-139">Если вы использовали для входа правильный идентификатор MPN, в Центре партнеров в меню слева отобразится пункт **MPN**.</span><span class="sxs-lookup"><span data-stu-id="c7d01-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="c7d01-140">Изменение расположения глобальной учетной записи партнера</span><span class="sxs-lookup"><span data-stu-id="c7d01-140">Change Global partner account location</span></span>

1. <span data-ttu-id="c7d01-141">На странице **[Расположения офисов организации](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** проверьте список расположений, чтобы убедиться, что в нем указано расположение вашего юридического лица.</span><span class="sxs-lookup"><span data-stu-id="c7d01-141">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="c7d01-142">Если это не так, добавьте его.</span><span class="sxs-lookup"><span data-stu-id="c7d01-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Снимок экрана со списком всех текущих расположений на странице расположения учетных записей Центра партнеров.":::

2. <span data-ttu-id="c7d01-144">Выберите **Legal** (Юридическая информация) и щелкните **Update legal business profile** (Обновить официальный бизнес-профиль).</span><span class="sxs-lookup"><span data-stu-id="c7d01-144">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="c7d01-145">Выберите регион и юридическое лицо, а затем щелкните **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="c7d01-145">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="c7d01-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c7d01-146">Next steps</span></span>

- <span data-ttu-id="c7d01-147">Ознакомьтесь с [процессом проверки](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="c7d01-147">Learn about the [verification process](verification-responses.md).</span></span>
