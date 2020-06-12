---
title: Управление расположениями в партнерской учетной записи
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как в Центре партнеров добавить новое расположение и каким образом идентификатор расположения MPN используется в программах поощрений, бизнес-операциях CSP, подписках и других транзакциях.
author: LauraBrenner
ms.author: labrenne
keywords: учетная запись партнера, расположения
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 943299cc4c68a6252c69a96204ef6001b89eda09
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453211"
---
# <a name="manage-your-partner-account-locations-in-partner-center-and-add-a-new-location"></a><span data-ttu-id="9f3d9-104">Управление расположениями учетной записи партнера в Центре партнеров и добавление нового расположения</span><span class="sxs-lookup"><span data-stu-id="9f3d9-104">Manage your partner account locations in Partner Center and add a new location</span></span>

<span data-ttu-id="9f3d9-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="9f3d9-105">**Appropriate roles**</span></span>
- <span data-ttu-id="9f3d9-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9f3d9-106">Global admin</span></span>
- <span data-ttu-id="9f3d9-107">администратор пользователей.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-107">User admin</span></span>
- <span data-ttu-id="9f3d9-108">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="9f3d9-108">Billing admin</span></span>
- <span data-ttu-id="9f3d9-109">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="9f3d9-109">Admin agent</span></span>
- <span data-ttu-id="9f3d9-110">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="9f3d9-110">Sales agent</span></span>

<span data-ttu-id="9f3d9-111">Идентификатор MPN расположения определяет каждое конкретное расположение компании.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-111">The location MPN IDs identify each specific location of your company.</span></span> <span data-ttu-id="9f3d9-112">Идентификатор MPN расположения используется для регистрации в программах поощрения, выполнения бизнес-транзакций в рамках программы поставщиков облачных решений (CSP), добавления новых подписок, а также для других бизнес-транзакций.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-112">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, to add new subscriptions, and other business transactions.</span></span> <span data-ttu-id="9f3d9-113">Идентификатор компании MPN используется для нетранзакционных действий, таких как запросы на поддержку.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-113">The company MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="9f3d9-114">Ниже приведен типичный сценарий:</span><span class="sxs-lookup"><span data-stu-id="9f3d9-114">The following is a typical scenario:</span></span>

<span data-ttu-id="9f3d9-115">Партнерская компания может вести бизнес в рамках CSP и осуществлять издательскую деятельность.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-115">A partner company can have a CSP business and a publishing business.</span></span> <span data-ttu-id="9f3d9-116">Она может работать как CSP в одних расположениях, а как издатель — в других. Как юридическое лицо компания использует один идентификатор MPN для всех не связанных с бизнес-транзакциями операций, таких как добавление пользователей или регистрация запросов на поддержку.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-116">Their CSP business can be located in several locales and their pub business may be located in other locales.Their registered legal business has one MPN ID used for managing all non-transactional business such as adding users or logging support requests.</span></span>


<span data-ttu-id="9f3d9-117">Каждое из расположений компании имеет свой идентификатор MPN для бизнес-транзакций, например для CSP или программ поощрения.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-117">Each of their locations has an MPN ID used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="9f3d9-118">Выплаты привязываются к расположениям.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-118">Payouts are tied to specific locations.</span></span>

<span data-ttu-id="9f3d9-119">У пользователей могут быть роли, охватывающие разные расположения.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-119">Users may have roles that cross locations.</span></span> <span data-ttu-id="9f3d9-120">Например, администратор программы поощрения может использовать эту роль для всех расположений в Европе.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-120">For example, the incentives admin could have that role for all locations in Europe.</span></span>

## <a name="to-add-a-location"></a><span data-ttu-id="9f3d9-121">Добавление расположения</span><span class="sxs-lookup"><span data-stu-id="9f3d9-121">To add a location</span></span>

1. <span data-ttu-id="9f3d9-122">Щелкните значок **Параметры** и выберите **Параметры партнеров**.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-122">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="9f3d9-123">Выберите **Расположения**.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-123">Select **Locations.**</span></span>

3. <span data-ttu-id="9f3d9-124">Выберите **Добавить расположение**.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-124">Select **Add a location**.</span></span>  

4. <span data-ttu-id="9f3d9-125">На странице **Добавление расположения** введите сведения об адресе расположения, которое требуется добавить в компанию, а также основной контакт для этого расположения.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-125">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="9f3d9-126">После добавления расположения в Центр партнеров его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-126">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-legal-headquarters-location"></a><span data-ttu-id="9f3d9-127">Изменение расположения главного офиса</span><span class="sxs-lookup"><span data-stu-id="9f3d9-127">Change legal headquarters location</span></span>

1. <span data-ttu-id="9f3d9-128">На странице **Расположения** проверьте список расположений, чтобы убедиться, что в нем указано расположение вашего юридического лица.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-128">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="9f3d9-129">Если это не так, добавьте его.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-129">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Изменение расположения организации":::

2. <span data-ttu-id="9f3d9-131">Выберите **Профиль партнера** и щелкните **Update legal business profile** (Обновить официальный бизнес-профиль).</span><span class="sxs-lookup"><span data-stu-id="9f3d9-131">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Изменение расположения организации":::

3. <span data-ttu-id="9f3d9-133">Выберите регион и юридическое лицо, а затем щелкните **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-133">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Изменение расположения организации":::
