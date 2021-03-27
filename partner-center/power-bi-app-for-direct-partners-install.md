---
title: Установка аналитики центра партнеров для Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Выполните действия, описанные в этой статье, чтобы установить и просмотреть приложение аналитики центра партнеров для Power BI (для прямых партнеров в CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ad0c2f3ee7d130c49dea6ba354e6794e29fd9e9f
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633698"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="1a2df-103">Установить и ознакомиться с приложением "Аналитика Центра партнеров для Microsoft Power BI"</span><span class="sxs-lookup"><span data-stu-id="1a2df-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="1a2df-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="1a2df-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1a2df-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1a2df-105">Global admin</span></span>
- <span data-ttu-id="1a2df-106">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="1a2df-106">User management admin</span></span>
- <span data-ttu-id="1a2df-107">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="1a2df-107">Sales agent</span></span>
- <span data-ttu-id="1a2df-108">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="1a2df-108">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="1a2df-109">Подготовка</span><span class="sxs-lookup"><span data-stu-id="1a2df-109">Before you begin</span></span>

<span data-ttu-id="1a2df-110">Выберите приложение, которое наиболее релевантно для вашего бизнеса, в следующем списке доступных Power BI приложений:</span><span class="sxs-lookup"><span data-stu-id="1a2df-110">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>

- [<span data-ttu-id="1a2df-111">Прямой поставщик</span><span class="sxs-lookup"><span data-stu-id="1a2df-111">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="1a2df-112">Косвенный поставщик</span><span class="sxs-lookup"><span data-stu-id="1a2df-112">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="1a2df-113">Непрямой Торговый посредник</span><span class="sxs-lookup"><span data-stu-id="1a2df-113">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="1a2df-114">Перед установкой предварительной версии приложения "Аналитика Центра партнеров" убедитесь, что соблюдены следующие требования.</span><span class="sxs-lookup"><span data-stu-id="1a2df-114">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="1a2df-115">Выберите нужное приложение Power BI для вашего бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1a2df-115">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="1a2df-116">У вас есть лицензия Power BI Pro.</span><span class="sxs-lookup"><span data-stu-id="1a2df-116">You have a Power BI pro license.</span></span>

- <span data-ttu-id="1a2df-117">У вас есть разрешения на установку шаблонов приложений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1a2df-117">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="1a2df-118">Вы можете войти в Power BI.</span><span class="sxs-lookup"><span data-stu-id="1a2df-118">You can sign in to Power BI.</span></span>

- <span data-ttu-id="1a2df-119">Вы можете войти в систему в качестве глобального администратора, агента администратора или администратора выставления счетов в [клиенте Azure Active Directory (Azure AD) вашей компании](azure-active-directory-tenants-and-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="1a2df-119">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="1a2df-120">Установка приложения</span><span class="sxs-lookup"><span data-stu-id="1a2df-120">To install the app</span></span>

1. <span data-ttu-id="1a2df-121">Выберите исходную ссылку приложения (прямой поставщик, косвенный поставщик или непрямого торгового посредника) в приведенном выше разделе.</span><span class="sxs-lookup"><span data-stu-id="1a2df-121">Select the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="1a2df-122">Выберите **Загрузить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="1a2df-122">Select **GET IT NOW**.</span></span> 

3. <span data-ttu-id="1a2df-123">Примите условия принятия условий, выбрав **"продолжить"**.</span><span class="sxs-lookup"><span data-stu-id="1a2df-123">Agree terms and conditions by selecting **Continue**.</span></span>

4. <span data-ttu-id="1a2df-124">В разделе Уже есть учетная запись? выберите **Вход**.</span><span class="sxs-lookup"><span data-stu-id="1a2df-124">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="1a2df-125">На следующей странице введите имя пользователя и пароль Power BI, а затем выберите **Вход**.</span><span class="sxs-lookup"><span data-stu-id="1a2df-125">On the next page, enter your Power BI user name and password and then select **Sign In**.</span></span>

6. <span data-ttu-id="1a2df-126">Установите рабочую область, указав имя рабочей области.</span><span class="sxs-lookup"><span data-stu-id="1a2df-126">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="1a2df-127">Вы можете найти приложения шаблонов, установленные в разделе "приложения".</span><span class="sxs-lookup"><span data-stu-id="1a2df-127">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="1a2df-128">Выберите **приложения** и выберите установленные приложения.</span><span class="sxs-lookup"><span data-stu-id="1a2df-128">Select **Apps** and choose the installed apps.</span></span>

9. <span data-ttu-id="1a2df-129">Откроется экран Начало работы с новым приложением.</span><span class="sxs-lookup"><span data-stu-id="1a2df-129">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="1a2df-130">Чтобы подключиться к данным, нажмите кнопку **подключить**.</span><span class="sxs-lookup"><span data-stu-id="1a2df-130">To connect to the data, select **Connect**.</span></span>

11. <span data-ttu-id="1a2df-131">На всплывающем окне **Подключение к аналитике центра партнеров** убедитесь, что для **метода проверки подлинности** задано значение **oAuth2** , или выберите **oAuth2** из списка, если это не так.</span><span class="sxs-lookup"><span data-stu-id="1a2df-131">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="1a2df-132">Для отображение окна может потребоваться несколько минут.</span><span class="sxs-lookup"><span data-stu-id="1a2df-132">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="1a2df-133">На странице **соединителя аналитики центра партнеров** выполните вход с помощью глобального администратора, агента администратора или учетных данных администратора выставления счетов для клиента Azure AD Организации, а затем выберите **Вход**.</span><span class="sxs-lookup"><span data-stu-id="1a2df-133">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="1a2df-134">Когда появится запрос доступа, нажмите кнопку **Принять**.</span><span class="sxs-lookup"><span data-stu-id="1a2df-134">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="1a2df-135">После подключения служба аналитики Центра партнеров к Power BI начнется загрузка данных.</span><span class="sxs-lookup"><span data-stu-id="1a2df-135">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="1a2df-136">Это может занять до 10 минут в зависимости от объема данных.</span><span class="sxs-lookup"><span data-stu-id="1a2df-136">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="1a2df-137">После завершения загрузки данных вы можете приступить к использованию информационной панели и отчетов приложения "Аналитика Центра партнеров" в Power BI.</span><span class="sxs-lookup"><span data-stu-id="1a2df-137">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1a2df-138">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="1a2df-138">Next steps</span></span>

[<span data-ttu-id="1a2df-139">Просматривайте бизнес-данные с помощью приложения "Аналитика Центра партнеров для Microsoft Power BI"</span><span class="sxs-lookup"><span data-stu-id="1a2df-139">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
