---
title: Azure Cost Management от Cloudyn для партнеров CSP | Центр партнеров
ms.topic: article
ms.date: 10/29/2018
description: Для использования Azure Cost Management от Cloudyn требуется предоставленный доступ к API Центра партнеров.
author: Janet
ms.author: janet
Keywords: Приложение для управления расходами, управлять затратами, веб-приложения
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586087"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="99666-104">Приложение Azure Cost Management для партнеров Azure CSP</span><span class="sxs-lookup"><span data-stu-id="99666-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="99666-105">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="99666-105">**Applies to**</span></span>

-  <span data-ttu-id="99666-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="99666-106">Partner Center</span></span>

[<span data-ttu-id="99666-107">Получить дополнительные сведения о службе управления затратами Azure</span><span class="sxs-lookup"><span data-stu-id="99666-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="99666-108">Перед началом работы</span><span class="sxs-lookup"><span data-stu-id="99666-108">Before you begin</span></span>
<span data-ttu-id="99666-109">До начала использования Azure Cost Management убедитесь, что соблюдаются следующие требования:</span><span class="sxs-lookup"><span data-stu-id="99666-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="99666-110">Вы являетесь партнером и участвуете в программе для поставщиков облачных решений (CSP).</span><span class="sxs-lookup"><span data-stu-id="99666-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="99666-111">Вы можете создать веб-приложение на основе API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="99666-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="99666-112">Обзор</span><span class="sxs-lookup"><span data-stu-id="99666-112">Overview</span></span>

<span data-ttu-id="99666-113">Azure Cost Management от Cloudyn — это веб-приложение, позволяющее отслеживать и контролировать объем и стоимость использования Azure вашими клиентами.</span><span class="sxs-lookup"><span data-stu-id="99666-113">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="99666-114">Приложение доступно через API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="99666-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="99666-115">Регистрация своего веб-приложения в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="99666-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="99666-116">При регистрации веб-приложения Azure Active Directory в Центре партнеров вы предоставляете доступ к API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="99666-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="99666-117">Войдите в [Центр партнеров](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) с помощью [учетной записи глобального администратора или агента администратора](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="99666-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="99666-118">Из **центра партнеров**выберите **параметры учетной записи** &gt;  **[управления приложениями](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="99666-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="99666-119">В разделе **Веб-приложение** щелкните **Добавить новое веб-приложение**.</span><span class="sxs-lookup"><span data-stu-id="99666-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="99666-120">**Примечание**. Если вы ранее создали веб-приложения, можно пропустить шаг 3.</span><span class="sxs-lookup"><span data-stu-id="99666-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="99666-121">Копируйте и сохраните GUID **ИД коммерции** и GUID **ИД приложения** вашего веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="99666-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="99666-122">Для использования бесплатной пробной версии приложения Azure Cost Management на 30 дней потребуются оба идентификатора.</span><span class="sxs-lookup"><span data-stu-id="99666-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="99666-123">Добавление секретного ключа в приложение</span><span class="sxs-lookup"><span data-stu-id="99666-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="99666-124">В раскрывающемся меню рядом с кнопкой **Добавить ключ** выберите период: 1 или 2 года.</span><span class="sxs-lookup"><span data-stu-id="99666-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="99666-125">Нажмите кнопку **Добавить ключ**.</span><span class="sxs-lookup"><span data-stu-id="99666-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="99666-126">Копируйте и сохраните значение секретного ключа.</span><span class="sxs-lookup"><span data-stu-id="99666-126">Copy and save the secret key value.</span></span> <span data-ttu-id="99666-127">Это необходимо для получения бесплатной пробной версии на 30 дней.</span><span class="sxs-lookup"><span data-stu-id="99666-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="99666-128">Секретный ключ приложения, такие как пароли с больше даты окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="99666-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="99666-129">Сохраните значение ключа в безопасном расположении для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="99666-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="99666-130">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="99666-130">Next steps</span></span>
<span data-ttu-id="99666-131">Запустите [бесплатную пробную версию на 30 дней](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="99666-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="99666-132">Для запуска пробной версии потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="99666-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="99666-133">Учетные данные для входа в Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="99666-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="99666-134">GUID "ИД коммерции"</span><span class="sxs-lookup"><span data-stu-id="99666-134">Commerce ID GUID</span></span>
- <span data-ttu-id="99666-135">GUID "ИД приложения"</span><span class="sxs-lookup"><span data-stu-id="99666-135">App ID GUID</span></span>
- <span data-ttu-id="99666-136">Значение секретного ключа приложения</span><span class="sxs-lookup"><span data-stu-id="99666-136">Application secret key value</span></span>
