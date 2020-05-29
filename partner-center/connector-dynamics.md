---
title: Соединитель совместной продажи для Dynamics 365 CRM Partner Center
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Синхронизация ссылок в центре партнеров с Dynamics 365 CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 87b1d27fa2f42eeba3b0f8308648536c0686911e
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145138"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="22004-103">Соединитель совместных продаж для Dynamics 365 CRM — обзор</span><span class="sxs-lookup"><span data-stu-id="22004-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="22004-104">Соответствующие роли</span><span class="sxs-lookup"><span data-stu-id="22004-104">Appropriate roles</span></span>

- <span data-ttu-id="22004-105">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="22004-105">Referrals admin</span></span>
- <span data-ttu-id="22004-106">Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="22004-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="22004-107">Соединитель совместных продаж в центре партнеров позволяет продавцов совместную продажу с корпорацией Майкрософт в ваших системах CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="22004-108">Они не должны быть обучены для использования центра партнеров для управления сделками в совместных продажах.</span><span class="sxs-lookup"><span data-stu-id="22004-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="22004-109">Используйте соединители совместной продажи, чтобы создать новую ссылку для совместной продажи, которая будет использоваться для привлечения к торговому представителю корпорации Майкрософт, получать ссылки от продавца корпорации Майкрософт, принимать или отклонять ссылки, изменять данные сделки, такие как стоимость сделки и дату закрытия.</span><span class="sxs-lookup"><span data-stu-id="22004-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="22004-110">Вы также можете получить обновления от Microsoft продавцов для этих сделок совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="22004-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="22004-111">Все ваши ссылки можно использовать в любом выбранном вами CRM, а не в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="22004-112">Решение основано на решении Microsoft Power Автоматизируing и использует API-интерфейсы центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="22004-113">Перед установкой предварительных требований</span><span class="sxs-lookup"><span data-stu-id="22004-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="22004-114">**Разделы**</span><span class="sxs-lookup"><span data-stu-id="22004-114">**Topics**</span></span>   |<span data-ttu-id="22004-115">**Сведения**</span><span class="sxs-lookup"><span data-stu-id="22004-115">**Details**</span></span>   |<span data-ttu-id="22004-116">**Ссылки**</span><span class="sxs-lookup"><span data-stu-id="22004-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="22004-117">Идентификатор Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="22004-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="22004-118">Требуется допустимый идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="22004-118">You need a valid MPN ID</span></span>|<span data-ttu-id="22004-119">Присоединение к [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="22004-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="22004-120">Готовность к совместной продаже</span><span class="sxs-lookup"><span data-stu-id="22004-120">Cosell ready</span></span>|<span data-ttu-id="22004-121">Ваше решение для работы с IP-адресами и службами должно быть готово к совместной продаже.</span><span class="sxs-lookup"><span data-stu-id="22004-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="22004-122">Продажа с Майкрософт</span><span class="sxs-lookup"><span data-stu-id="22004-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="22004-123">Учетная запись Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="22004-123">Partner Center account</span></span>|<span data-ttu-id="22004-124">Идентификатор MPN, связанный с клиентом центра партнеров, должен совпадать с ИДЕНТИФИКАТОРом MPN, связанным с решением для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="22004-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="22004-125">Прежде чем развертывать соединители, убедитесь, что вы видите ссылки на совместные продажи на портале центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="22004-126">Управление учетной записью</span><span class="sxs-lookup"><span data-stu-id="22004-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="22004-127">Роли пользователей Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="22004-127">Partner Center user roles</span></span>|<span data-ttu-id="22004-128">Сотрудник, который будет устанавливать и использовать соединители, должен быть администратором ссылок.</span><span class="sxs-lookup"><span data-stu-id="22004-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="22004-129">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="22004-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="22004-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="22004-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="22004-131">Роль пользователя CRM — системный администратор или Настройщик системы</span><span class="sxs-lookup"><span data-stu-id="22004-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="22004-132">Назначение ролей в Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="22004-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="22004-133">Учетная запись потока Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="22004-133">Power Automate Flow Account</span></span>|<span data-ttu-id="22004-134">Активная учетная запись [Power автоматизируется](https://flow.microsoft.com) для системного администратора CRM или настройщика системы.</span><span class="sxs-lookup"><span data-stu-id="22004-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="22004-135">Этот пользователь должен войти в [Power автоматизиру](https://flow.microsoft.com) по крайней мере один раз перед установкой.</span><span class="sxs-lookup"><span data-stu-id="22004-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="22004-136">Установка синхронизации ссылок центра партнеров для Dynamics 365 (решение Power Автоматизация)</span><span class="sxs-lookup"><span data-stu-id="22004-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span> 

1. <span data-ttu-id="22004-137">Откройте [Power автоматизиру](https://flow.microsoft.com) и выберите **среды** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="22004-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="22004-138">На этом шаге будут показаны доступные экземпляры CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="22004-139">Выберите нужный экземпляр CRM в раскрывающемся списке в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="22004-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="22004-140">Выберите **решения** на панели навигации слева.</span><span class="sxs-lookup"><span data-stu-id="22004-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="22004-141">Щелкните ссылку **Open AppSource (открыть** ) в верхнем меню.</span><span class="sxs-lookup"><span data-stu-id="22004-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Открыть AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="22004-143">Найдите **соединители центров партнеров для Dynamics365** во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="22004-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="22004-144">Нажмите кнопку **получить сейчас** и **Продолжайте**.</span><span class="sxs-lookup"><span data-stu-id="22004-144">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="22004-145">Откроется страница, на которой можно выбрать среду CRM (Dynamics 365) для установки приложения.</span><span class="sxs-lookup"><span data-stu-id="22004-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="22004-146">Согласиться с условиями.</span><span class="sxs-lookup"><span data-stu-id="22004-146">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="22004-147">Затем вы направляетесь на страницу **Управление решениями** .</span><span class="sxs-lookup"><span data-stu-id="22004-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="22004-148">Перейдите в раздел "ссылки центра партнеров" с помощью кнопок со стрелками в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="22004-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="22004-149">**Запланированная установка** должна отображаться рядом с решением "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="22004-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="22004-150">Установка займет 10-15 минут.</span><span class="sxs-lookup"><span data-stu-id="22004-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="22004-151">После завершения установки вернитесь к [Power автоматизиру](https://flow.microsoft.com) и выберите **решения** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="22004-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="22004-152">Обратите внимание, что в списке решений можно найти **ссылку Центр партнеров синхронизация для Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="22004-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="22004-153">Выберите **ссылку Центр партнеров синхронизация для Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="22004-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="22004-154">Доступны следующие потоки и сущности Power автоматизировать:</span><span class="sxs-lookup"><span data-stu-id="22004-154">The following Power Automate flows and entities are available:</span></span>

![Доступные КРМС](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="22004-156">Рекомендации: Протестируйте перед переходом в динамический</span><span class="sxs-lookup"><span data-stu-id="22004-156">Best practice: test before you go live</span></span>

<span data-ttu-id="22004-157">Прежде чем устанавливать, настраивать и настраивать решение Power Автоматизация в рабочей среде, обязательно протестируйте решение на промежуточном экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="22004-158">Установите решение Microsoft Power автоматизируя в промежуточной среде или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="22004-159">Создайте копию решения и запустите настройку потока настройки и автоматизации энергосбережения в промежуточной среде.</span><span class="sxs-lookup"><span data-stu-id="22004-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="22004-160">Протестируйте решение в промежуточном или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="22004-161">При успешном выполнении импортируйте в рабочий экземпляр как управляемое решение.</span><span class="sxs-lookup"><span data-stu-id="22004-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="22004-162">Настройка решения</span><span class="sxs-lookup"><span data-stu-id="22004-162">Configure the solution</span></span>

1. <span data-ttu-id="22004-163">После установки решения в экземпляре CRM вернитесь к [Power автоматизиру](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="22004-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="22004-164">В раскрывающемся списке **среды** в правом верхнем углу выберите экземпляр CRM, в котором было установлено решение Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="22004-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="22004-165">Вам потребуется создать подключения, связывающие три учетные записи пользователей:</span><span class="sxs-lookup"><span data-stu-id="22004-165">You'll need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="22004-166">Пользователь центра партнеров с учетными данными администратора ссылок</span><span class="sxs-lookup"><span data-stu-id="22004-166">Partner Center user with referrals admin credentials</span></span> 

- <span data-ttu-id="22004-167">События Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="22004-167">Partner Center Events</span></span>

- <span data-ttu-id="22004-168">Администратор CRM с потоками Power автоматизиру в решении.</span><span class="sxs-lookup"><span data-stu-id="22004-168">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="22004-169">a.</span><span class="sxs-lookup"><span data-stu-id="22004-169">a.</span></span> <span data-ttu-id="22004-170">В области навигации слева выберите **подключения** и в списке выберите решение "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="22004-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="22004-171">b.</span><span class="sxs-lookup"><span data-stu-id="22004-171">b.</span></span> <span data-ttu-id="22004-172">Создайте подключение, щелкнув **создать соединение**.</span><span class="sxs-lookup"><span data-stu-id="22004-172">Create a connection by clicking **Create a connection**.</span></span>

    ![Создание подключения](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="22004-174">c.</span><span class="sxs-lookup"><span data-stu-id="22004-174">c.</span></span> <span data-ttu-id="22004-175">Поиск **ссылок центра партнеров (Предварительная версия)** на панели поиска в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="22004-175">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

    <span data-ttu-id="22004-176">г.</span><span class="sxs-lookup"><span data-stu-id="22004-176">d.</span></span> <span data-ttu-id="22004-177">Создайте подключение для пользователя центра партнеров с ролью учетных данных администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="22004-177">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="22004-178">Д.</span><span class="sxs-lookup"><span data-stu-id="22004-178">e.</span></span> <span data-ttu-id="22004-179">Затем создайте подключение к событиям центра партнеров для пользователя центра партнеров с учетными данными администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="22004-179">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

    <span data-ttu-id="22004-180">f.</span><span class="sxs-lookup"><span data-stu-id="22004-180">f.</span></span> <span data-ttu-id="22004-181">Создайте подключение для Common Data Service (текущего окружения) для пользователя администратора CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-181">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="22004-182">Чтобы связать Power автоматизирующие потоки с подключениями, измените каждый из потоков Power автоматизиру, чтобы подключиться к Common Data Service и ссылкам центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-182">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="22004-183">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="22004-183">Save the changes.</span></span>

5. <span data-ttu-id="22004-184">**Включите** потоки Power автоматизирующие.</span><span class="sxs-lookup"><span data-stu-id="22004-184">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="22004-185">Использование API веб-перехватчика для регистрации событий изменения ресурсов</span><span class="sxs-lookup"><span data-stu-id="22004-185">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="22004-186">Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="22004-186">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="22004-187">Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.</span><span class="sxs-lookup"><span data-stu-id="22004-187">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="22004-188">Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.</span><span class="sxs-lookup"><span data-stu-id="22004-188">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="22004-189">Добавить соединения для (a.) Пользователь центра партнеров с ссылками на учетные данные администратора (b). События центра партнеров, отмеченные ниже</span><span class="sxs-lookup"><span data-stu-id="22004-189">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Триггер](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="22004-191">При выполнении этих обновлений вы увидите</span><span class="sxs-lookup"><span data-stu-id="22004-191">When you make these updates, you'll see</span></span>

![Веб-перехватчики](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="22004-193">Сохраните изменения и выберите **включить**.</span><span class="sxs-lookup"><span data-stu-id="22004-193">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="22004-194">Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="22004-194">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="22004-195">Выберите пункт **Центр партнеров для Dynamics 365 (Предварительная версия)**.</span><span class="sxs-lookup"><span data-stu-id="22004-195">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="22004-196">Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.</span><span class="sxs-lookup"><span data-stu-id="22004-196">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="22004-197">Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="22004-197">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Копирование URL-адреса](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="22004-199">Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.</span><span class="sxs-lookup"><span data-stu-id="22004-199">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="22004-200">Убедитесь, что в правой части окна откроется окно "запуск потока", и нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="22004-200">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="22004-201">Введите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="22004-201">Enter the following details:</span></span> 

    <span data-ttu-id="22004-202">a.</span><span class="sxs-lookup"><span data-stu-id="22004-202">a.</span></span> <span data-ttu-id="22004-203">**Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага</span><span class="sxs-lookup"><span data-stu-id="22004-203">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="22004-204">b.</span><span class="sxs-lookup"><span data-stu-id="22004-204">b.</span></span> <span data-ttu-id="22004-205">**Регистрируемые события**: "Создание ссылок" и "обновление ссылок"</span><span class="sxs-lookup"><span data-stu-id="22004-205">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="22004-206">c.</span><span class="sxs-lookup"><span data-stu-id="22004-206">c.</span></span> <span data-ttu-id="22004-207">**Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки).</span><span class="sxs-lookup"><span data-stu-id="22004-207">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="22004-208">Выберите **выполнить** , а затем нажмите кнопку **Готово.**</span><span class="sxs-lookup"><span data-stu-id="22004-208">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="22004-209">Теперь веб-перехватчик может прослушивать события создания и обновления.</span><span class="sxs-lookup"><span data-stu-id="22004-209">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="22004-210">Настройка шагов синхронизации</span><span class="sxs-lookup"><span data-stu-id="22004-210">Customize synchronization steps</span></span>

<span data-ttu-id="22004-211">Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.</span><span class="sxs-lookup"><span data-stu-id="22004-211">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="22004-212">Часто системы CRM сильно настроены.</span><span class="sxs-lookup"><span data-stu-id="22004-212">Often CRM systems are highly customized.</span></span> <span data-ttu-id="22004-213">Можно настроить потоки автоматизации Powering.</span><span class="sxs-lookup"><span data-stu-id="22004-213">You can customize the Power Automate flows.</span></span> <span data-ttu-id="22004-214">Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="22004-214">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="22004-215">Предоставляются сопоставления центров партнеров Майкрософт с CRM, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.</span><span class="sxs-lookup"><span data-stu-id="22004-215">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="22004-216">В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать.</span><span class="sxs-lookup"><span data-stu-id="22004-216">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="22004-217">Ниже приведены примеры доступных настроек.</span><span class="sxs-lookup"><span data-stu-id="22004-217">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="22004-218">Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="22004-218">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="22004-219">a.</span><span class="sxs-lookup"><span data-stu-id="22004-219">a.</span></span> <span data-ttu-id="22004-220">Выберите пункт Центр партнеров для Dynamics 365 (Предварительная версия) или центр партнеров в Salesforce (Предварительная версия для предварительной версии).</span><span class="sxs-lookup"><span data-stu-id="22004-220">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="22004-221">b.</span><span class="sxs-lookup"><span data-stu-id="22004-221">b.</span></span> <span data-ttu-id="22004-222">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="22004-222">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="22004-223">c.</span><span class="sxs-lookup"><span data-stu-id="22004-223">c.</span></span> <span data-ttu-id="22004-224">Выберите **(область) синхронизация интереса или возможной сделки**.</span><span class="sxs-lookup"><span data-stu-id="22004-224">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="22004-225">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **, если это новая доступная возможность, а затем**.</span><span class="sxs-lookup"><span data-stu-id="22004-225">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="22004-226">Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**.</span><span class="sxs-lookup"><span data-stu-id="22004-226">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="22004-227">Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="22004-227">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="22004-228">г.</span><span class="sxs-lookup"><span data-stu-id="22004-228">d.</span></span> <span data-ttu-id="22004-229">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, щелкните шаг "(область) синхронизация интереса или возможности".</span><span class="sxs-lookup"><span data-stu-id="22004-229">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="22004-230">Д.</span><span class="sxs-lookup"><span data-stu-id="22004-230">e.</span></span> <span data-ttu-id="22004-231">Выберите **, если это обновление возможной сделки, а затем**.</span><span class="sxs-lookup"><span data-stu-id="22004-231">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="22004-232">Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.</span><span class="sxs-lookup"><span data-stu-id="22004-232">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="22004-233">f.</span><span class="sxs-lookup"><span data-stu-id="22004-233">f.</span></span> <span data-ttu-id="22004-234">Выберите, **Если да** , а затем **обновить существующую возможную сделку**</span><span class="sxs-lookup"><span data-stu-id="22004-234">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="22004-235">Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="22004-235">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="22004-236">a.</span><span class="sxs-lookup"><span data-stu-id="22004-236">a.</span></span> <span data-ttu-id="22004-237">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="22004-237">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="22004-238">b.</span><span class="sxs-lookup"><span data-stu-id="22004-238">b.</span></span> <span data-ttu-id="22004-239">Выберите **(область) синхронизировать возможную сделку**.</span><span class="sxs-lookup"><span data-stu-id="22004-239">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="22004-240">c.</span><span class="sxs-lookup"><span data-stu-id="22004-240">c.</span></span> <span data-ttu-id="22004-241">Чтобы настроить сопоставления полей CRM для событий обновления, выберите **в случае разницы между ведущими объектами в центре партнеров и CRM**.</span><span class="sxs-lookup"><span data-stu-id="22004-241">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="22004-242">г.</span><span class="sxs-lookup"><span data-stu-id="22004-242">d.</span></span> <span data-ttu-id="22004-243">Выберите подшаг, **Если да** , а затем разверните этот шаг, чтобы **Обновить ссылку на данные о возможностях**.</span><span class="sxs-lookup"><span data-stu-id="22004-243">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="22004-244">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="22004-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="22004-245">Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?</span><span class="sxs-lookup"><span data-stu-id="22004-245">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="22004-246">a.</span><span class="sxs-lookup"><span data-stu-id="22004-246">a.</span></span> <span data-ttu-id="22004-247">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="22004-247">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="22004-248">b.</span><span class="sxs-lookup"><span data-stu-id="22004-248">b.</span></span> <span data-ttu-id="22004-249">Выберите **(область) синхронизация ссылок.**</span><span class="sxs-lookup"><span data-stu-id="22004-249">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="22004-250">c.</span><span class="sxs-lookup"><span data-stu-id="22004-250">c.</span></span> <span data-ttu-id="22004-251">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="22004-251">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="22004-252">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="22004-252">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="22004-253">Сквозная синхронизация двунаправленной совместной продажи</span><span class="sxs-lookup"><span data-stu-id="22004-253">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="22004-254">После установки, настройки и настройки решения Power автоматизиру вы можете протестировать синхронизацию ссылок совместной продажи между Dynamics 365 и центром партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-254">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="22004-255">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="22004-255">Pre-requisites</span></span>

<span data-ttu-id="22004-256">Чтобы синхронизировать ссылки в центре партнеров и Dynamics 365 CRM, решение Power автоматизиру четко обозначает поля ссылок, относящиеся к корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="22004-256">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="22004-257">Эта идентификация дает группе продавцов возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="22004-257">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="22004-258">Набор настраиваемых полей доступен как часть сущности **возможной сделки** .</span><span class="sxs-lookup"><span data-stu-id="22004-258">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="22004-259">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="22004-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="22004-260">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="22004-260">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="22004-261">**Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="22004-261">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="22004-262">**Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="22004-262">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="22004-263">**Ссылка на ссылку: ссылка**только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="22004-263">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="22004-264">**Как можно получить справку Майкрософт?**: Помогите корпорации Майкрософт получить ссылку</span><span class="sxs-lookup"><span data-stu-id="22004-264">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="22004-265">**Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="22004-265">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="22004-266">**Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров</span><span class="sxs-lookup"><span data-stu-id="22004-266">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="22004-267">ВАРИАНТ</span><span class="sxs-lookup"><span data-stu-id="22004-267">SCENARIOS:</span></span>

1. <span data-ttu-id="22004-268">Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="22004-268">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="22004-269">a.</span><span class="sxs-lookup"><span data-stu-id="22004-269">a.</span></span> <span data-ttu-id="22004-270">Войдите в среду Dynamics 365 CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-270">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="22004-271">b.</span><span class="sxs-lookup"><span data-stu-id="22004-271">b.</span></span> <span data-ttu-id="22004-272">При создании "новой возможности" в среде Dynamics 365 убедитесь, что указан следующий раздел:</span><span class="sxs-lookup"><span data-stu-id="22004-272">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Opportunity;](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="22004-274">c.</span><span class="sxs-lookup"><span data-stu-id="22004-274">c.</span></span> <span data-ttu-id="22004-275">Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="22004-275">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="22004-276">**Синхронизация с центром партнеров**: Да</span><span class="sxs-lookup"><span data-stu-id="22004-276">**Sync with Partner Center**: Yes</span></span>

    - <span data-ttu-id="22004-277">**Как можно получить справку Майкрософт?**: выберите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="22004-277">**How can Microsoft help?**: Select from the following:</span></span>

    ![Параметры справки](images/cosellconnectors/help.png)

    - <span data-ttu-id="22004-279">**Продукты**: идентификаторы решений для продукта</span><span class="sxs-lookup"><span data-stu-id="22004-279">**Products**: Solution IDs of the product</span></span>

    <span data-ttu-id="22004-280">г.</span><span class="sxs-lookup"><span data-stu-id="22004-280">d.</span></span> <span data-ttu-id="22004-281">После создания возможности в Dynamics 365 с параметром **Синхронизация с центром партнеров** задайте значение **Да**, подождите 10 минут и войдите в свою учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-281">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="22004-282">Ваши ссылки будут синхронизированы с Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="22004-282">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="22004-283">Д.</span><span class="sxs-lookup"><span data-stu-id="22004-283">e.</span></span> <span data-ttu-id="22004-284">Аналогично, для возможности, для которой параметр "Синхронизация с центром партнеров" имеет значение "Да", при обновлении возможности в Dynamics 365 CRM изменения будут синхронизированы в учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-284">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="22004-285">f.</span><span class="sxs-lookup"><span data-stu-id="22004-285">f.</span></span> <span data-ttu-id="22004-286">Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="22004-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="22004-287">Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="22004-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

    <span data-ttu-id="22004-288">a.</span><span class="sxs-lookup"><span data-stu-id="22004-288">a.</span></span> <span data-ttu-id="22004-289">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="22004-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="22004-290">b.</span><span class="sxs-lookup"><span data-stu-id="22004-290">b.</span></span> <span data-ttu-id="22004-291">В меню слева выберите **ссылки** .</span><span class="sxs-lookup"><span data-stu-id="22004-291">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="22004-292">c.</span><span class="sxs-lookup"><span data-stu-id="22004-292">c.</span></span> <span data-ttu-id="22004-293">Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".</span><span class="sxs-lookup"><span data-stu-id="22004-293">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="22004-294">г.</span><span class="sxs-lookup"><span data-stu-id="22004-294">d.</span></span> <span data-ttu-id="22004-295">Войдите в среду Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-295">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="22004-296">Д.</span><span class="sxs-lookup"><span data-stu-id="22004-296">e.</span></span> <span data-ttu-id="22004-297">Перейдите к разделу **открытые возможности**.</span><span class="sxs-lookup"><span data-stu-id="22004-297">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="22004-298">Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="22004-298">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="22004-299">f.</span><span class="sxs-lookup"><span data-stu-id="22004-299">f.</span></span> <span data-ttu-id="22004-300">При выборе синхронизированной ссылки сведения о представлении карточки заполняются.</span><span class="sxs-lookup"><span data-stu-id="22004-300">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="22004-301">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="22004-301">Next steps</span></span>

- [<span data-ttu-id="22004-302">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="22004-302">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="22004-303">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="22004-303">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="22004-304">Дополнительные сведения о платформе Microsoft Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="22004-304">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="22004-305">Веб-перехватчики Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="22004-305">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)