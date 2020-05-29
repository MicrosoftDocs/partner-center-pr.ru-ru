---
title: Соединитель для совместной продажи в центре партнеров для Salesforce CRM
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Синхронизация ссылок в центре партнеров с помощью Salesforce CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145108"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="c7fb5-103">Соединитель совместных продаж для Salesforce CRM — обзор</span><span class="sxs-lookup"><span data-stu-id="c7fb5-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="c7fb5-104">Соответствующие роли</span><span class="sxs-lookup"><span data-stu-id="c7fb5-104">Appropriate roles</span></span>

- <span data-ttu-id="c7fb5-105">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="c7fb5-105">Referrals admin</span></span>
- <span data-ttu-id="c7fb5-106">Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="c7fb5-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="c7fb5-107">Соединитель совместных продаж в центре партнеров позволяет продавцов совместную продажу с корпорацией Майкрософт в ваших системах CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="c7fb5-108">Они не должны быть обучены для использования центра партнеров для управления сделками в совместных продажах.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="c7fb5-109">Используя соединители совместной работы, вы можете создать новую ссылку для совместной продажи, чтобы привлечь продавца Майкрософт, получать ссылки от продавца Майкрософт, принимать или отклонять ссылки, изменять данные сделки, такие как стоимость сделки и дату закрытия.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="c7fb5-110">Вы также можете получить обновления от Microsoft продавцов для этих сделок совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="c7fb5-111">Все ваши ссылки можно выполнять при работе в CRM по вашему выбору, а не в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="c7fb5-112">Решение основано на решении Microsoft Power Автоматизируing и использует API-интерфейсы центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="c7fb5-113">Перед установкой предварительных требований</span><span class="sxs-lookup"><span data-stu-id="c7fb5-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="c7fb5-114">**Разделы**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-114">**Topics**</span></span>   |<span data-ttu-id="c7fb5-115">**Сведения**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-115">**Details**</span></span>   |<span data-ttu-id="c7fb5-116">**Ссылки**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="c7fb5-117">Идентификатор Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="c7fb5-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="c7fb5-118">Требуется допустимый идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="c7fb5-118">You need a valid MPN ID</span></span>|<span data-ttu-id="c7fb5-119">Присоединение к [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="c7fb5-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="c7fb5-120">Готовность к совместной продаже</span><span class="sxs-lookup"><span data-stu-id="c7fb5-120">Co-sell ready</span></span>|<span data-ttu-id="c7fb5-121">Ваше решение для работы с IP-адресами и службами должно быть готово к совместной продаже.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="c7fb5-122">Продажа с Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="c7fb5-123">Учетная запись Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="c7fb5-123">Partner Center account</span></span>|<span data-ttu-id="c7fb5-124">Идентификатор MPN, связанный с клиентом центра партнеров, должен совпадать с ИДЕНТИФИКАТОРом MPN, связанным с решением для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="c7fb5-125">Прежде чем развертывать соединители, убедитесь, что вы видите ссылки на совместные продажи на портале центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="c7fb5-126">Управление учетной записью</span><span class="sxs-lookup"><span data-stu-id="c7fb5-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c7fb5-127">Роли пользователей Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="c7fb5-127">Partner Center user roles</span></span>|<span data-ttu-id="c7fb5-128">Сотрудник, который будет устанавливать и использовать соединители, должен быть администратором ссылок.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="c7fb5-129">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="c7fb5-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c7fb5-130">SalesForce CRM</span><span class="sxs-lookup"><span data-stu-id="c7fb5-130">Salesforce CRM</span></span>|<span data-ttu-id="c7fb5-131">Роль пользователя CRM — системный администратор или Настройщик системы</span><span class="sxs-lookup"><span data-stu-id="c7fb5-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="c7fb5-132">Назначение ролей в Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="c7fb5-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="c7fb5-133">Учетная запись потока Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="c7fb5-133">Power Automate Flow Account</span></span>|<span data-ttu-id="c7fb5-134">Активная учетная запись [Power автоматизируется](https://flow.microsoft.com) для системного администратора CRM или настройщика системы.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="c7fb5-135">Этот пользователь должен войти в [Power автоматизиру](https://flow.microsoft.com) по крайней мере один раз перед установкой.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="c7fb5-136">Установка синхронизации ссылок центра партнеров для Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="c7fb5-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="c7fb5-137">Откройте [Power автоматизиру](https://flow.microsoft.com) и выберите **среды** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="c7fb5-138">Будут показаны доступные экземпляры CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="c7fb5-139">Выберите нужный экземпляр CRM в раскрывающемся списке в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="c7fb5-140">Выберите **решения** на панели навигации слева.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="c7fb5-141">Щелкните ссылку **Open AppSource (открыть** ) в верхнем меню.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Открыть AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="c7fb5-143">Найдите **соединители центров партнеров для Salesforce** во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

![Salesforce](images/salesforce/salesforce1.png)

6. <span data-ttu-id="c7fb5-145">Нажмите кнопку **получить сейчас** и **Продолжайте**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-145">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="c7fb5-146">Откроется страница, на которой можно выбрать среду CRM salesforce для установки приложения.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="c7fb5-147">Согласиться с условиями.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-147">Agree to terms and conditions.</span></span>

![Доступные КРМС](images/salesforce/available-crm.png)

8. <span data-ttu-id="c7fb5-149">Затем вы направляетесь на страницу **Управление решениями** .</span><span class="sxs-lookup"><span data-stu-id="c7fb5-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="c7fb5-150">Перейдите в раздел "ссылки центра партнеров" с помощью кнопок со стрелками в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="c7fb5-151">**Запланированная установка** должна отображаться рядом с решением "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="c7fb5-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="c7fb5-152">Установка займет 10-15 минут.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-152">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="c7fb5-153">После завершения установки вернитесь к [Power автоматизиру](https://flow.microsoft.com) и выберите **решения** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="c7fb5-154">Обратите внимание, что **Синхронизация ссылок центра партнеров по Salesforce** доступна в списке решений.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="c7fb5-155">Выберите **ссылку Центр партнеров синхронизация для Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="c7fb5-156">Доступны следующие потоки и сущности Power автоматизировать:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-156">The following Power Automate flows and entities are available:</span></span>

![Потоки Salesforce](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="c7fb5-158">Рекомендации: Протестируйте перед переходом в динамический</span><span class="sxs-lookup"><span data-stu-id="c7fb5-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="c7fb5-159">Прежде чем устанавливать, настраивать и настраивать решение Power Автоматизация в рабочей среде, обязательно протестируйте решение на промежуточном экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="c7fb5-160">Установите решение Microsoft Power автоматизируя в промежуточной среде или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="c7fb5-161">Создайте копию решения и запустите настройку потока настройки и автоматизации энергосбережения в промежуточной среде.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="c7fb5-162">Протестируйте решение в промежуточном или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="c7fb5-163">При успешном выполнении импортируйте в рабочий экземпляр как управляемое решение.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-163">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="c7fb5-164">Настройка решения</span><span class="sxs-lookup"><span data-stu-id="c7fb5-164">Configure the solution</span></span>

1. <span data-ttu-id="c7fb5-165">После установки решения в экземпляре CRM вернитесь к [Power автоматизиру](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="c7fb5-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="c7fb5-166">В раскрывающемся списке **среды** в правом верхнем углу выберите экземпляр CRM, в котором было установлено решение Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="c7fb5-167">Вам потребуется создать подключения, связывающие три учетные записи пользователей:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-167">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="c7fb5-168">Пользователь центра партнеров с учетными данными администратора ссылок</span><span class="sxs-lookup"><span data-stu-id="c7fb5-168">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="c7fb5-169">События Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="c7fb5-169">Partner Center Events</span></span>
- <span data-ttu-id="c7fb5-170">Администратор CRM с потоками Power автоматизиру в решении.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-170">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="c7fb5-171">a.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-171">a.</span></span> <span data-ttu-id="c7fb5-172">В области навигации слева выберите **подключения** и в списке выберите решение "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="c7fb5-172">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="c7fb5-173">b.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-173">b.</span></span> <span data-ttu-id="c7fb5-174">Создайте подключение, щелкнув **создать соединение**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-174">Create a connection by clicking **Create a connection**.</span></span> 

    ![Создание подключения](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="c7fb5-176">c.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-176">c.</span></span> <span data-ttu-id="c7fb5-177">Поиск **ссылок центра партнеров (Предварительная версия)** в строке поиска в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-177">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

    <span data-ttu-id="c7fb5-178">г.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-178">d.</span></span> <span data-ttu-id="c7fb5-179">Создайте подключение для пользователя центра партнеров с ролью учетных данных администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-179">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="c7fb5-180">Д.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-180">e.</span></span> <span data-ttu-id="c7fb5-181">Затем создайте подключение к событиям центра партнеров для пользователя центра партнеров с учетными данными администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-181">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>
    
    <span data-ttu-id="c7fb5-182">f.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-182">f.</span></span> <span data-ttu-id="c7fb5-183">Создайте подключение для Common Data Service (текущего окружения) для пользователя администратора CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-183">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="c7fb5-184">Чтобы связать Power автоматизирующие потоки с подключениями, измените каждый из потоков Power автоматизиру, чтобы подключиться к Common Data Service и ссылкам центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-184">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="c7fb5-185">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-185">Save the changes.</span></span>

5. <span data-ttu-id="c7fb5-186">**Включите** потоки Power автоматизирующие.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-186">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="c7fb5-187">Использование API веб-перехватчика для регистрации событий изменения ресурсов</span><span class="sxs-lookup"><span data-stu-id="c7fb5-187">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="c7fb5-188">Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-188">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="c7fb5-189">Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-189">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="c7fb5-190">Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-190">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="c7fb5-191">Добавить соединения для (a.) Пользователь центра партнеров с ссылками на учетные данные администратора (b). События центра партнеров, отмеченные ниже</span><span class="sxs-lookup"><span data-stu-id="c7fb5-191">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Триггер](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="c7fb5-193">При выполнении этих обновлений вы увидите</span><span class="sxs-lookup"><span data-stu-id="c7fb5-193">When you make these updates, you'll see</span></span>

![Веб-перехватчики](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="c7fb5-195">Сохраните изменения и выберите **включить**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-195">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="c7fb5-196">Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-196">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="c7fb5-197">Выберите **Центр партнеров для SALESFORCE CRM (Предварительная версия)**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-197">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="c7fb5-198">Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-198">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="c7fb5-199">Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-199">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Копирование URL-адреса](images/salesforce/copy-url.png)

8. <span data-ttu-id="c7fb5-201">Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-201">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="c7fb5-202">Убедитесь, что в правой части окна откроется окно "запуск потока", и нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-202">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="c7fb5-203">Введите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-203">Enter the following details:</span></span> 

    <span data-ttu-id="c7fb5-204">a.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-204">a.</span></span> <span data-ttu-id="c7fb5-205">**Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага</span><span class="sxs-lookup"><span data-stu-id="c7fb5-205">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="c7fb5-206">b.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-206">b.</span></span> <span data-ttu-id="c7fb5-207">**Регистрируемые события**: "Создание ссылок" и "обновление ссылок"</span><span class="sxs-lookup"><span data-stu-id="c7fb5-207">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="c7fb5-208">c.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-208">c.</span></span> <span data-ttu-id="c7fb5-209">**Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки).</span><span class="sxs-lookup"><span data-stu-id="c7fb5-209">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="c7fb5-210">Выберите **выполнить** , а затем нажмите кнопку **Готово.**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-210">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="c7fb5-211">Теперь веб-перехватчик может прослушивать события создания и обновления.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-211">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="c7fb5-212">Настройка шагов синхронизации</span><span class="sxs-lookup"><span data-stu-id="c7fb5-212">Customize synchronization steps</span></span>

<span data-ttu-id="c7fb5-213">Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-213">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="c7fb5-214">Часто системы CRM сильно настроены.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-214">Often CRM systems are highly customized.</span></span> <span data-ttu-id="c7fb5-215">Можно настроить потоки автоматизации Powering.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-215">You can customize the Power Automate flows.</span></span> <span data-ttu-id="c7fb5-216">Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-216">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="c7fb5-217">Предоставляются сопоставления центров партнеров Майкрософт с CRM, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-217">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="c7fb5-218">В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-218">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="c7fb5-219">Ниже приведены примеры доступных настроек.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-219">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="c7fb5-220">Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-220">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="c7fb5-221">a.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-221">a.</span></span> <span data-ttu-id="c7fb5-222">Выберите центр партнеров для Salesforce CRM (Предварительная версия).</span><span class="sxs-lookup"><span data-stu-id="c7fb5-222">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

    <span data-ttu-id="c7fb5-223">b.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-223">b.</span></span> <span data-ttu-id="c7fb5-224">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-224">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="c7fb5-225">c.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-225">c.</span></span> <span data-ttu-id="c7fb5-226">Выберите **(область) синхронизация интереса или возможной сделки**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-226">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="c7fb5-227">Чтобы настроить сопоставления полей CRM для создания событий, выберите **, если это новая доступная возможность, а затем**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-227">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="c7fb5-228">Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-228">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="c7fb5-229">Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-229">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="c7fb5-230">г.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-230">d.</span></span> <span data-ttu-id="c7fb5-231">Чтобы настроить сопоставления полей CRM для событий обновления, щелкните шаг "(область) синхронизация интереса или возможности".</span><span class="sxs-lookup"><span data-stu-id="c7fb5-231">To customize CRM field mappings for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="c7fb5-232">Д.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-232">e.</span></span> <span data-ttu-id="c7fb5-233">Выберите **, если это обновление возможной сделки, а затем**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-233">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="c7fb5-234">Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-234">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="c7fb5-235">f.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-235">f.</span></span> <span data-ttu-id="c7fb5-236">Выберите, **Если да** , а затем **обновить существующую возможную сделку**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-236">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="c7fb5-237">Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-237">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="c7fb5-238">a.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-238">a.</span></span> <span data-ttu-id="c7fb5-239">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="c7fb5-240">b.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-240">b.</span></span> <span data-ttu-id="c7fb5-241">Выберите **(область) синхронизировать возможную сделку**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-241">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="c7fb5-242">c.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-242">c.</span></span> <span data-ttu-id="c7fb5-243">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, установите флажок, **Если между ведущими объектами в центре партнеров и CRM есть различия**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-243">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="c7fb5-244">г.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-244">d.</span></span> <span data-ttu-id="c7fb5-245">Выберите подшаг, **Если да** , а затем разверните этот шаг, чтобы **Обновить ссылку на данные о возможностях**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-245">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="c7fb5-246">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-246">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="c7fb5-247">Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?</span><span class="sxs-lookup"><span data-stu-id="c7fb5-247">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="c7fb5-248">a.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-248">a.</span></span> <span data-ttu-id="c7fb5-249">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-249">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="c7fb5-250">b.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-250">b.</span></span> <span data-ttu-id="c7fb5-251">Выберите **(область) синхронизация ссылок.**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-251">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="c7fb5-252">c.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-252">c.</span></span> <span data-ttu-id="c7fb5-253">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-253">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="c7fb5-254">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="c7fb5-255">Создание отдельного раздела в макете возможностей CRM в Salesforce</span><span class="sxs-lookup"><span data-stu-id="c7fb5-255">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="c7fb5-256">Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, решение Power автоматизирует необходимость четко разграничения ссылочные поля Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-256">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="c7fb5-257">Это дает группам продавцов возможность выбирать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-257">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="c7fb5-258">Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможной сделки** CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-258">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="c7fb5-259">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="c7fb5-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="c7fb5-260">Пользователю с правами администратора Salesforce CRM потребуется создать отдельный раздел CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-260">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="c7fb5-261">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-261">The following custom fields should be part of the CRM section:</span></span>

<span data-ttu-id="c7fb5-262">• **Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-262">• **Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

<span data-ttu-id="c7fb5-263">• **Идентификатор ссылки**: поле идентификатора только для чтения для ссылки на центр партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-263">• **Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

<span data-ttu-id="c7fb5-264">• **Ссылка на ссылку:** ссылка только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-264">• **Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

<span data-ttu-id="c7fb5-265">• **Как может помочь Майкрософт?**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-265">• **How can Microsoft help?**</span></span> <span data-ttu-id="c7fb5-266">Справка, необходимая корпорации Майкрософт для ссылок</span><span class="sxs-lookup"><span data-stu-id="c7fb5-266">Help required from Microsoft for the referral</span></span>

<span data-ttu-id="c7fb5-267">• **Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="c7fb5-267">• **Products**: List of products associated with this opportunity</span></span>

<span data-ttu-id="c7fb5-268">• **Аудит**: журнал аудита только для чтения для синхронизации с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-268">• **Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="c7fb5-269">Настройка полей и связей</span><span class="sxs-lookup"><span data-stu-id="c7fb5-269">Set up fields and relationships</span></span>

1. <span data-ttu-id="c7fb5-270">Войдите в учетную запись Salesforce и перейдите к **возможности**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-270">Sign into your Salesforce account and go to **Opportunity**.</span></span> 

2. <span data-ttu-id="c7fb5-271">Щелкните Параметры **установки** и **изменения объекта** , чтобы добавить необходимые поля.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-271">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>


3. <span data-ttu-id="c7fb5-272">Выбор **полей & связей** в левой области навигации</span><span class="sxs-lookup"><span data-stu-id="c7fb5-272">Select **Fields & Relationships** from the left navigation</span></span>

![Поля](images/salesforce/fields1.png)

4. <span data-ttu-id="c7fb5-274">Добавьте следующие поля в таблицу "поля & связи":</span><span class="sxs-lookup"><span data-stu-id="c7fb5-274">Add the following fields in the “Fields & Relationship” table:</span></span>

|<span data-ttu-id="c7fb5-275">**Метка поля**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-275">**Field label**</span></span>   |<span data-ttu-id="c7fb5-276">**Имя поля**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-276">**Field name**</span></span>|<span data-ttu-id="c7fb5-277">**Data type**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-277">**Data type**</span></span>|<span data-ttu-id="c7fb5-278">**Индексированного**</span><span class="sxs-lookup"><span data-stu-id="c7fb5-278">**Indexed**</span></span>|
|---------------------|:-------------------|:--------------|:----------------|
|<span data-ttu-id="c7fb5-279">Синхронизация с центром партнеров</span><span class="sxs-lookup"><span data-stu-id="c7fb5-279">Sync with Partner Center</span></span>|<span data-ttu-id="c7fb5-280">Синхронизация с-Partner-Center-c</span><span class="sxs-lookup"><span data-stu-id="c7fb5-280">sync-with-partner-center-c</span></span>|<span data-ttu-id="c7fb5-281">Флажок (значение по умолчанию снято)</span><span class="sxs-lookup"><span data-stu-id="c7fb5-281">Checkbox (default unchecked)</span></span>||
|<span data-ttu-id="c7fb5-282">Продукты</span><span class="sxs-lookup"><span data-stu-id="c7fb5-282">Products</span></span>|<span data-ttu-id="c7fb5-283">Продукты-c</span><span class="sxs-lookup"><span data-stu-id="c7fb5-283">Products-c</span></span>|<span data-ttu-id="c7fb5-284">текст (255)</span><span class="sxs-lookup"><span data-stu-id="c7fb5-284">text (255)</span></span>||
|<span data-ttu-id="c7fb5-285">Referral</span><span class="sxs-lookup"><span data-stu-id="c7fb5-285">Referral</span></span> | <span data-ttu-id="c7fb5-286">Referral_Identifier__c</span><span class="sxs-lookup"><span data-stu-id="c7fb5-286">Referral_Identifier__c</span></span>|<span data-ttu-id="c7fb5-287">Текст (100) (внешний идентификатор)</span><span class="sxs-lookup"><span data-stu-id="c7fb5-287">Text(100)(External ID)</span></span>|<span data-ttu-id="c7fb5-288">да</span><span class="sxs-lookup"><span data-stu-id="c7fb5-288">yes</span></span>|
|<span data-ttu-id="c7fb5-289">Ссылка на ссылку</span><span class="sxs-lookup"><span data-stu-id="c7fb5-289">Referral Link</span></span>| <span data-ttu-id="c7fb5-290">Referral_Link__c_</span><span class="sxs-lookup"><span data-stu-id="c7fb5-290">Referral_Link__c_</span></span>|<span data-ttu-id="c7fb5-291">URL-АДРЕС (255)</span><span class="sxs-lookup"><span data-stu-id="c7fb5-291">URL(255)</span></span>||
|<span data-ttu-id="c7fb5-292">Аудит</span><span class="sxs-lookup"><span data-stu-id="c7fb5-292">Audit</span></span>| <span data-ttu-id="c7fb5-293">Audit__c</span><span class="sxs-lookup"><span data-stu-id="c7fb5-293">Audit__c</span></span>|<span data-ttu-id="c7fb5-294">Длинная текстовая область (100000) (видимая строка 4)</span><span class="sxs-lookup"><span data-stu-id="c7fb5-294">Long Text Area(100000)(visible line 4)</span></span>||
|<span data-ttu-id="c7fb5-295">Как можно получить справку Майкрософт?</span><span class="sxs-lookup"><span data-stu-id="c7fb5-295">How can Microsoft help?</span></span>|<span data-ttu-id="c7fb5-296">How_can_Microsoft_help__c</span><span class="sxs-lookup"><span data-stu-id="c7fb5-296">How_can_Microsoft_help__c</span></span>|<span data-ttu-id="c7fb5-297">Поля выбора</span><span class="sxs-lookup"><span data-stu-id="c7fb5-297">Picklist\*</span></span>|

<span data-ttu-id="c7fb5-298">\* Значения поля выбора:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-298">\*Picklist values:</span></span>

<span data-ttu-id="c7fb5-299">• Специальное значение для рабочей нагрузки</span><span class="sxs-lookup"><span data-stu-id="c7fb5-299">• Workload specific value proposition</span></span>

<span data-ttu-id="c7fb5-300">• Техническая архитектура клиента</span><span class="sxs-lookup"><span data-stu-id="c7fb5-300">• Customer technical architecture</span></span>

<span data-ttu-id="c7fb5-301">• Подтверждение концепции или демонстрации</span><span class="sxs-lookup"><span data-stu-id="c7fb5-301">• Proof of concept or demo</span></span>

<span data-ttu-id="c7fb5-302">• Кавычки или лицензирование</span><span class="sxs-lookup"><span data-stu-id="c7fb5-302">• Quotes or licensing</span></span>

<span data-ttu-id="c7fb5-303">• Учет успешных продаж клиентов</span><span class="sxs-lookup"><span data-stu-id="c7fb5-303">• Post sales customer success</span></span>

<span data-ttu-id="c7fb5-304">• Общие или другие</span><span class="sxs-lookup"><span data-stu-id="c7fb5-304">• General or other</span></span>

<span data-ttu-id="c7fb5-305">5. поля создаются в разделе "поля & связи".</span><span class="sxs-lookup"><span data-stu-id="c7fb5-305">5.The fields would get created under “Fields & Relationships”</span></span>

![Созданные поля](images/salesforce/fields2.png)

6. <span data-ttu-id="c7fb5-307">В макете возможности создайте отдельный раздел с полями, как показано выше.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-307">In the Opportunity layout, create a separate section with the fields as listed above.</span></span> 

    <span data-ttu-id="c7fb5-308">• Этот раздел должен быть доступен для продавцов в макете возможности.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-308">• This section should be available for the sellers in the Opportunity layout</span></span>


![Макет полей центра партнеров](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="c7fb5-310">Сквозная синхронизация двунаправленной совместной продажи</span><span class="sxs-lookup"><span data-stu-id="c7fb5-310">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="c7fb5-311">После установки, настройки и настройки решения Power автоматизиру вы можете протестировать синхронизацию ссылок для совместной продажи между Salesforce CRM и центром партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-311">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="c7fb5-312">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c7fb5-312">Pre-requisites</span></span>

<span data-ttu-id="c7fb5-313">Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, решение Power автоматизирует необходимость четко разграничения ссылочные поля Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-313">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="c7fb5-314">Эта идентификация предоставляет группам продавцов возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-314">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="c7fb5-315">Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможности** решения Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-315">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="c7fb5-316">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="c7fb5-316">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="c7fb5-317">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-317">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="c7fb5-318">**Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-318">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="c7fb5-319">**Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-319">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="c7fb5-320">**Ссылка на ссылку: ссылка**только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c7fb5-320">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="c7fb5-321">**Как можно**получить помощь от корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-321">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="c7fb5-322">**Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="c7fb5-322">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="c7fb5-323">**Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров</span><span class="sxs-lookup"><span data-stu-id="c7fb5-323">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="c7fb5-324">ВАРИАНТ</span><span class="sxs-lookup"><span data-stu-id="c7fb5-324">SCENARIOS:</span></span>

1. <span data-ttu-id="c7fb5-325">Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-325">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="c7fb5-326">a.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-326">a.</span></span> <span data-ttu-id="c7fb5-327">Войдите в среду Salesforce CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-327">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="c7fb5-328">b.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-328">b.</span></span> <span data-ttu-id="c7fb5-329">При создании "новой возможности" в среде Salesforce CRM убедитесь, что следующий раздел существует.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-329">Ensure that the following section is present when you create a “New Opportunity” in Salesforce CRM environment</span></span>

    ![Среда Salesforce](images/salesforce/salesforce-scenario-1.png)

   

    <span data-ttu-id="c7fb5-331">c.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-331">c.</span></span> <span data-ttu-id="c7fb5-332">Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-332">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="c7fb5-333">"Синхронизация с центром партнеров": Да</span><span class="sxs-lookup"><span data-stu-id="c7fb5-333">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="c7fb5-334">«Как можно получить справку Майкрософт?»: выберите следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-334">"How can Microsoft help?”: Select from the following options:</span></span>

   

    - <span data-ttu-id="c7fb5-335">Продукты: идентификаторы решений для продукта</span><span class="sxs-lookup"><span data-stu-id="c7fb5-335">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="c7fb5-336">г.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-336">d.</span></span> <span data-ttu-id="c7fb5-337">Установив для параметра синхронизация возможных сделок **с центром партнеров** значение **Да**, подождите 10 минут, войдите в свою учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-337">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="c7fb5-338">Ваши ссылки будут синхронизированы с Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-338">Your referrals will be synchronized with Salesforce CRM.</span></span>

    <span data-ttu-id="c7fb5-339">Д.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-339">e.</span></span> <span data-ttu-id="c7fb5-340">Если параметр "синхронизировать с центром партнеров" имеет значение "Да", то при обновлении возможной сделки в Salesforce CRM изменения будут синхронизироваться с учетной записью центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-340">When the “Sync with Partner Center” option is set to “Yes”, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

    <span data-ttu-id="c7fb5-341">f.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-341">f.</span></span> <span data-ttu-id="c7fb5-342">Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-342">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="c7fb5-343">Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="c7fb5-343">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span> 

    <span data-ttu-id="c7fb5-344">a.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-344">a.</span></span> <span data-ttu-id="c7fb5-345">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-345">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="c7fb5-346">b.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-346">b.</span></span> <span data-ttu-id="c7fb5-347">В меню слева выберите **ссылки** .</span><span class="sxs-lookup"><span data-stu-id="c7fb5-347">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="c7fb5-348">c.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-348">c.</span></span> <span data-ttu-id="c7fb5-349">Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".</span><span class="sxs-lookup"><span data-stu-id="c7fb5-349">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="c7fb5-350">г.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-350">d.</span></span> <span data-ttu-id="c7fb5-351">Войдите в среду Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-351">Sign into your Salesforce CRM environment.</span></span> 

    <span data-ttu-id="c7fb5-352">Д.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-352">e.</span></span> <span data-ttu-id="c7fb5-353">Перейдите к разделу **открытые возможности**.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-353">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="c7fb5-354">Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-354">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    ![Экран возможностей Salesforce](images/salesforce/salesforce-casino-e.png)

    <span data-ttu-id="c7fb5-356">f.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-356">f.</span></span> <span data-ttu-id="c7fb5-357">При выборе синхронизированной ссылки сведения о представлении карточки заполняются.</span><span class="sxs-lookup"><span data-stu-id="c7fb5-357">When you select a synchronized referral, the card view details are populated.</span></span>





## <a name="next-steps"></a><span data-ttu-id="c7fb5-358">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="c7fb5-358">Next steps</span></span>

- [<span data-ttu-id="c7fb5-359">Дополнительные сведения о платформе Microsoft Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="c7fb5-359">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="c7fb5-360">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="c7fb5-360">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="c7fb5-361">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="c7fb5-361">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="c7fb5-362">Веб-перехватчики Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="c7fb5-362">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)