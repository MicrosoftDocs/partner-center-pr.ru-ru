---
title: Azure Cost Management от Cloudyn для партнеров CSP | Центр партнеров
ms.topic: article
ms.date: 03/15/2019
description: Для использования Azure Cost Management от Cloudyn требуется предоставленный доступ к API Центра партнеров.
author: Janet
ms.author: janet
Keywords: Приложение для управления затратами Azure, управление затратами, веб-приложения
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 27ff91d9d42f08e44f812663f3d4409e1080d580
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820299"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="db16b-104">Приложение Azure Cost Management для партнеров Azure CSP</span><span class="sxs-lookup"><span data-stu-id="db16b-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="db16b-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="db16b-105">**Applies to**</span></span>

-  <span data-ttu-id="db16b-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="db16b-106">Partner Center</span></span>

[<span data-ttu-id="db16b-107">Получение дополнительных сведений об управлении затратами Azure</span><span class="sxs-lookup"><span data-stu-id="db16b-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="db16b-108">Перед началом работы</span><span class="sxs-lookup"><span data-stu-id="db16b-108">Before you begin</span></span>
<span data-ttu-id="db16b-109">До начала использования Azure Cost Management убедитесь, что соблюдаются следующие требования:</span><span class="sxs-lookup"><span data-stu-id="db16b-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="db16b-110">Вы являетесь партнером и участвуете в программе для поставщиков облачных решений (CSP).</span><span class="sxs-lookup"><span data-stu-id="db16b-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="db16b-111">Вы можете создать веб-приложение на основе API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="db16b-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="db16b-112">Обзор</span><span class="sxs-lookup"><span data-stu-id="db16b-112">Overview</span></span>

<span data-ttu-id="db16b-113">Cloudyn — это веб-приложение, которое позволяет контролировать объем использования Azure клиентами и управлять ими, а также затратами на их использование.</span><span class="sxs-lookup"><span data-stu-id="db16b-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="db16b-114">Приложение доступно через API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="db16b-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="db16b-115">Регистрация своего веб-приложения в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="db16b-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="db16b-116">При регистрации веб-приложения Azure Active Directory в Центре партнеров вы предоставляете доступ к API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="db16b-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="db16b-117">Войдите в [Центр партнеров](https://partnercenter.microsoft.com/pcv/dashboard/overview) с помощью [учетной записи глобального администратора или агента администратора](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="db16b-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="db16b-118">В **центре партнеров**выберите **Параметры** &gt; учетной записи **[Управление приложениями](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="db16b-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="db16b-119">В разделе **Веб-приложение** щелкните **Добавить новое веб-приложение**.</span><span class="sxs-lookup"><span data-stu-id="db16b-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="db16b-120">**Примечание**. Если вы ранее создали веб-приложение, можно пропустить шаг 3.</span><span class="sxs-lookup"><span data-stu-id="db16b-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="db16b-121">Копируйте и сохраните GUID **ИД коммерции** и GUID **ИД приложения** вашего веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="db16b-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="db16b-122">Для использования бесплатной пробной версии приложения Azure Cost Management на 30 дней потребуются оба идентификатора.</span><span class="sxs-lookup"><span data-stu-id="db16b-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="db16b-123">Добавление секретного ключа в приложение</span><span class="sxs-lookup"><span data-stu-id="db16b-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="db16b-124">В раскрывающемся меню рядом с кнопкой **Добавить ключ** выберите период: 1 или 2 года.</span><span class="sxs-lookup"><span data-stu-id="db16b-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="db16b-125">Нажмите кнопку **Добавить ключ**.</span><span class="sxs-lookup"><span data-stu-id="db16b-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="db16b-126">Копируйте и сохраните значение секретного ключа.</span><span class="sxs-lookup"><span data-stu-id="db16b-126">Copy and save the secret key value.</span></span> <span data-ttu-id="db16b-127">Это необходимо для получения бесплатной пробной версии на 30 дней.</span><span class="sxs-lookup"><span data-stu-id="db16b-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="db16b-128">Секретные ключи приложения подобны паролям с более длинными датами окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="db16b-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="db16b-129">Сохраните значение ключа в безопасном расположении для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="db16b-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="db16b-130">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="db16b-130">Next steps</span></span>
<span data-ttu-id="db16b-131">Запустите [бесплатную пробную версию на 30 дней](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="db16b-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="db16b-132">Для запуска пробной версии потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="db16b-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="db16b-133">Учетные данные для входа в Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="db16b-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="db16b-134">GUID "ИД коммерции"</span><span class="sxs-lookup"><span data-stu-id="db16b-134">Commerce ID GUID</span></span>
- <span data-ttu-id="db16b-135">GUID "ИД приложения"</span><span class="sxs-lookup"><span data-stu-id="db16b-135">App ID GUID</span></span>
- <span data-ttu-id="db16b-136">Значение секретного ключа приложения</span><span class="sxs-lookup"><span data-stu-id="db16b-136">Application secret key value</span></span>
