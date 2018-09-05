---
title: Azure Cost Management от Cloudyn для партнеров CSP | Центр партнеров
description: Для использования Azure Cost Management от Cloudyn требуется предоставленный доступ к API Центра партнеров.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 6ab388f9a178a0bfd3b3d3133da855bcddee9d4f
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877454"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="bed4a-103">Приложение Azure Cost Management для партнеров Azure CSP</span><span class="sxs-lookup"><span data-stu-id="bed4a-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="bed4a-104">Область применения</span><span class="sxs-lookup"><span data-stu-id="bed4a-104">Applies to</span></span>**

-  <span data-ttu-id="bed4a-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="bed4a-105">Partner Center</span></span>

[<span data-ttu-id="bed4a-106">Дополнительная информация об Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="bed4a-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="bed4a-107">Перед началом работы</span><span class="sxs-lookup"><span data-stu-id="bed4a-107">Before you begin</span></span>
<span data-ttu-id="bed4a-108">До начала использования Azure Cost Management убедитесь, что соблюдаются следующие требования:</span><span class="sxs-lookup"><span data-stu-id="bed4a-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="bed4a-109">Вы являетесь партнером и участвуете в программе для поставщиков облачных решений (CSP).</span><span class="sxs-lookup"><span data-stu-id="bed4a-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="bed4a-110">Вы можете создать веб-приложение на основе API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="bed4a-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="bed4a-111">Обзор</span><span class="sxs-lookup"><span data-stu-id="bed4a-111">Overview</span></span>

<span data-ttu-id="bed4a-112">Azure Cost Management от Cloudyn— это веб-приложение, позволяющее отслеживать и контролировать объем и стоимость использования Azure вашими клиентами.</span><span class="sxs-lookup"><span data-stu-id="bed4a-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="bed4a-113">Приложение доступно через API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="bed4a-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="bed4a-114">Регистрация своего веб-приложения в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="bed4a-114">Register your web app in the Partner Center</span></span>
<span data-ttu-id="bed4a-115">При регистрации веб-приложения Azure Active Directory в Центре партнеров вы предоставляете доступ к API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="bed4a-115">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="bed4a-116">Войдите в [Центр партнеров](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) с помощью [учетной записи глобального администратора или агента администратора](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="bed4a-116">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="bed4a-117">В меню **Панель мониторинга** выберите пункт **Параметры учетной записи** &gt; **[Управление пользователями](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="bed4a-117">From the **Dashboard**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="bed4a-118">В разделе **Веб-приложение** щелкните **Добавить новое веб-приложение**.</span><span class="sxs-lookup"><span data-stu-id="bed4a-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="bed4a-119">**Примечание**. Если ранее вы уже создали веб-приложение, шаг 3 можно пропустить.</span><span class="sxs-lookup"><span data-stu-id="bed4a-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="bed4a-120">Копируйте и сохраните GUID **ИД коммерции** и GUID **ИД приложения** вашего веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="bed4a-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="bed4a-121">Для использования бесплатной пробной версии приложения Azure Cost Management на 30 дней потребуются оба идентификатора.</span><span class="sxs-lookup"><span data-stu-id="bed4a-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="bed4a-122">Добавление секретного ключа в приложение</span><span class="sxs-lookup"><span data-stu-id="bed4a-122">Add a secret key to your app</span></span>
1.  <span data-ttu-id="bed4a-123">В раскрывающемся меню рядом с кнопкой **Добавить ключ** выберите период: 1 или 2 года.</span><span class="sxs-lookup"><span data-stu-id="bed4a-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2.  <span data-ttu-id="bed4a-124">Нажмите кнопку **Добавить ключ**.</span><span class="sxs-lookup"><span data-stu-id="bed4a-124">Click **Add key**.</span></span> 
3.  <span data-ttu-id="bed4a-125">Копируйте и сохраните значение секретного ключа.</span><span class="sxs-lookup"><span data-stu-id="bed4a-125">Copy and save the secret key value.</span></span> <span data-ttu-id="bed4a-126">Это необходимо для получения бесплатной пробной версии на 30 дней.</span><span class="sxs-lookup"><span data-stu-id="bed4a-126">You will need this for the 30-day free trial.</span></span>
<br><span data-ttu-id="bed4a-127">**Примечание**. Секретные ключи приложения напоминают пароли с более длительным сроком действия.</span><span class="sxs-lookup"><span data-stu-id="bed4a-127">**Note**: The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="bed4a-128">Сохраните значение ключа в безопасном расположении для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="bed4a-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bed4a-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="bed4a-129">Next steps</span></span>
<span data-ttu-id="bed4a-130">Запустите [бесплатную пробную версию на 30 дней](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="bed4a-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="bed4a-131">Для запуска пробной версии потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="bed4a-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="bed4a-132">Учетные данные для входа в Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="bed4a-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="bed4a-133">GUID "ИД коммерции"</span><span class="sxs-lookup"><span data-stu-id="bed4a-133">Commerce ID GUID</span></span>
- <span data-ttu-id="bed4a-134">GUID "ИД приложения"</span><span class="sxs-lookup"><span data-stu-id="bed4a-134">App ID GUID</span></span>
- <span data-ttu-id="bed4a-135">Значение секретного ключа приложения</span><span class="sxs-lookup"><span data-stu-id="bed4a-135">Application secret key value</span></span>
