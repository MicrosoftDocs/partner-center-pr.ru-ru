---
title: Управление затратами Azure от Cloudyn для CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как зарегистрировать веб-приложение Cloudyn и использовать секретный ключ в центре партнеров, чтобы вы могли использовать приложение для мониторинга использования и затрат Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435913"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="ed3b6-103">Мониторинг использования и расходов Azure с помощью приложения "Управление затратами Azure" для партнеров CSP</span><span class="sxs-lookup"><span data-stu-id="ed3b6-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="ed3b6-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="ed3b6-104">**Applies to**</span></span>

- <span data-ttu-id="ed3b6-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="ed3b6-105">Partner Center</span></span>
- <span data-ttu-id="ed3b6-106">Партнеры по программе поставщиков облачных решений</span><span class="sxs-lookup"><span data-stu-id="ed3b6-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="ed3b6-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="ed3b6-107">**Appropriate roles**</span></span>

- <span data-ttu-id="ed3b6-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ed3b6-108">Global admin</span></span>
- <span data-ttu-id="ed3b6-109">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="ed3b6-109">Admin agent</span></span>

[<span data-ttu-id="ed3b6-110">Дополнительная информация об Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="ed3b6-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="ed3b6-111">Подготовка к работе</span><span class="sxs-lookup"><span data-stu-id="ed3b6-111">Before you begin</span></span>
<span data-ttu-id="ed3b6-112">До начала использования Azure Cost Management убедитесь, что соблюдаются следующие требования:</span><span class="sxs-lookup"><span data-stu-id="ed3b6-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="ed3b6-113">Вы являетесь партнером и участвуете в программе для поставщиков облачных решений (CSP).</span><span class="sxs-lookup"><span data-stu-id="ed3b6-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="ed3b6-114">Вы можете создать веб-приложение на основе API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="ed3b6-115">Обзор</span><span class="sxs-lookup"><span data-stu-id="ed3b6-115">Overview</span></span>

<span data-ttu-id="ed3b6-116">Cloudyn — это веб-приложение, которое позволяет контролировать объем использования Azure клиентами и управлять ими, а также затратами на их использование.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="ed3b6-117">Приложение доступно через API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="ed3b6-118">Регистрация своего веб-приложения в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="ed3b6-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="ed3b6-119">При регистрации веб-приложения Azure Active Directory в Центре партнеров вы предоставляете доступ к API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="ed3b6-120">Войдите в [Центр партнеров](https://partnercenter.microsoft.com/pcv/dashboard/overview) с помощью [учетной записи глобального администратора или агента администратора](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="ed3b6-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="ed3b6-121">В **центре партнеров**выберите **Параметры учетной записи** &gt; **[Управление приложениями](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-121">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="ed3b6-122">В разделе **Веб-приложение** щелкните **Добавить новое веб-приложение**.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-122">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="ed3b6-123">**Примечание**. Если ранее вы уже создали веб-приложение, шаг 3 можно пропустить.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-123">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="ed3b6-124">Копируйте и сохраните GUID **ИД коммерции** и GUID **ИД приложения** вашего веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="ed3b6-125">Для использования бесплатной пробной версии приложения Azure Cost Management на 30 дней потребуются оба идентификатора.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="ed3b6-126">Добавление секретного ключа в приложение</span><span class="sxs-lookup"><span data-stu-id="ed3b6-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="ed3b6-127">В раскрывающемся меню рядом с кнопкой **Добавить ключ** выберите период: 1 или 2 года.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="ed3b6-128">Нажмите кнопку **Добавить раздел**.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-128">Click **Add key**.</span></span> 
3. <span data-ttu-id="ed3b6-129">Копируйте и сохраните значение секретного ключа.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-129">Copy and save the secret key value.</span></span> <span data-ttu-id="ed3b6-130">Это необходимо для получения бесплатной пробной версии на 30 дней.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="ed3b6-131">Секретные ключи приложения подобны паролям с более длинными датами окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="ed3b6-132">Сохраните значение ключа в безопасном расположении для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="ed3b6-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ed3b6-133">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="ed3b6-133">Next steps</span></span>
<span data-ttu-id="ed3b6-134">Запустите [бесплатную пробную версию на 30 дней](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="ed3b6-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="ed3b6-135">Для запуска пробной версии потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="ed3b6-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="ed3b6-136">Учетные данные для входа в Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="ed3b6-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="ed3b6-137">GUID "ИД коммерции"</span><span class="sxs-lookup"><span data-stu-id="ed3b6-137">Commerce ID GUID</span></span>
- <span data-ttu-id="ed3b6-138">GUID "ИД приложения"</span><span class="sxs-lookup"><span data-stu-id="ed3b6-138">App ID GUID</span></span>
- <span data-ttu-id="ed3b6-139">Значение секретного ключа приложения</span><span class="sxs-lookup"><span data-stu-id="ed3b6-139">Application secret key value</span></span>
