---
title: Соединитель совместной продажи для Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Синхронизируйте ссылки в центре партнеров с соединителем совместных продаж для Dynamics 365 CRM. Продавцов может совместно продаваться с корпорацией Майкрософт в ваших системах CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8ea803e675ce7c2d21d680491bbdaedf792e631f
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031337"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="5abc4-104">Соединитель совместных продаж для Dynamics 365 CRM — обзор</span><span class="sxs-lookup"><span data-stu-id="5abc4-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="5abc4-105">Соответствующие роли</span><span class="sxs-lookup"><span data-stu-id="5abc4-105">Appropriate roles</span></span>

- <span data-ttu-id="5abc4-106">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="5abc4-106">Referrals admin</span></span>
- <span data-ttu-id="5abc4-107">Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="5abc4-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="5abc4-108">Соединитель совместных продаж в центре партнеров позволяет продавцов совместную продажу с корпорацией Майкрософт в ваших системах CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="5abc4-109">Они не должны быть обучены для использования центра партнеров для управления сделками в совместных продажах.</span><span class="sxs-lookup"><span data-stu-id="5abc4-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="5abc4-110">Используйте соединители совместной продажи, чтобы создать новую ссылку для совместной продажи, которая будет использоваться для привлечения к торговому представителю корпорации Майкрософт, получать ссылки от продавца корпорации Майкрософт, принимать или отклонять ссылки, изменять данные сделки, такие как стоимость сделки и дату закрытия.</span><span class="sxs-lookup"><span data-stu-id="5abc4-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="5abc4-111">Вы также можете получить обновления от Microsoft продавцов для этих сделок совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="5abc4-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="5abc4-112">Все ваши ссылки можно использовать в любом выбранном вами CRM, а не в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="5abc4-113">Решение основано на решении Microsoft Power Автоматизируing и использует API-интерфейсы центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="5abc4-114">Перед установкой предварительных требований</span><span class="sxs-lookup"><span data-stu-id="5abc4-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="5abc4-115">**Разделы**</span><span class="sxs-lookup"><span data-stu-id="5abc4-115">**Topics**</span></span>   |<span data-ttu-id="5abc4-116">**Сведения**</span><span class="sxs-lookup"><span data-stu-id="5abc4-116">**Details**</span></span>   |<span data-ttu-id="5abc4-117">**Ссылки**</span><span class="sxs-lookup"><span data-stu-id="5abc4-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="5abc4-118">Идентификатор Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="5abc4-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="5abc4-119">Требуется допустимый идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="5abc4-119">You need a valid MPN ID</span></span>|<span data-ttu-id="5abc4-120">Присоединение к [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="5abc4-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="5abc4-121">Готовность к совместной продаже</span><span class="sxs-lookup"><span data-stu-id="5abc4-121">Cosell ready</span></span>|<span data-ttu-id="5abc4-122">Ваше решение для работы с IP-адресами и службами должно быть готово к совместной продаже.</span><span class="sxs-lookup"><span data-stu-id="5abc4-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="5abc4-123">Продажа с Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5abc4-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="5abc4-124">Учетная запись Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5abc4-124">Partner Center account</span></span>|<span data-ttu-id="5abc4-125">Идентификатор MPN, связанный с клиентом центра партнеров, должен совпадать с ИДЕНТИФИКАТОРом MPN, связанным с решением для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="5abc4-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="5abc4-126">Прежде чем развертывать соединители, убедитесь, что вы видите ссылки на совместные продажи на портале центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="5abc4-127">Управление учетной записью</span><span class="sxs-lookup"><span data-stu-id="5abc4-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="5abc4-128">Роли пользователей Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5abc4-128">Partner Center user roles</span></span>|<span data-ttu-id="5abc4-129">Сотрудник, который будет устанавливать и использовать соединители, должен быть администратором ссылок.</span><span class="sxs-lookup"><span data-stu-id="5abc4-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="5abc4-130">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="5abc4-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="5abc4-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="5abc4-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="5abc4-132">Роль пользователя CRM — системный администратор или Настройщик системы</span><span class="sxs-lookup"><span data-stu-id="5abc4-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="5abc4-133">Назначение ролей в Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="5abc4-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="5abc4-134">Учетная запись потока Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="5abc4-134">Power Automate Flow Account</span></span>|<span data-ttu-id="5abc4-135">Активная учетная запись [Power автоматизируется](https://flow.microsoft.com) для системного администратора CRM или настройщика системы.</span><span class="sxs-lookup"><span data-stu-id="5abc4-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="5abc4-136">Этот пользователь должен войти в [Power автоматизиру](https://flow.microsoft.com) по крайней мере один раз перед установкой.</span><span class="sxs-lookup"><span data-stu-id="5abc4-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="5abc4-137">Установка синхронизации ссылок центра партнеров для Dynamics 365 (решение Power Автоматизация)</span><span class="sxs-lookup"><span data-stu-id="5abc4-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="5abc4-138">Откройте [Power автоматизиру](https://flow.microsoft.com) и выберите **среды** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="5abc4-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="5abc4-139">На этом шаге будут показаны доступные экземпляры CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="5abc4-140">Выберите нужный экземпляр CRM в раскрывающемся списке в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="5abc4-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="5abc4-141">Выберите **решения** на панели навигации слева.</span><span class="sxs-lookup"><span data-stu-id="5abc4-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="5abc4-142">Щелкните ссылку **Open AppSource (открыть** ) в верхнем меню.</span><span class="sxs-lookup"><span data-stu-id="5abc4-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Открыть AppSource":::

5. <span data-ttu-id="5abc4-144">Найдите **соединители центров партнеров для Dynamics365** во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="5abc4-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="5abc4-145">Нажмите кнопку **получить сейчас** и **Продолжайте**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="5abc4-146">Откроется страница, на которой можно выбрать среду CRM (Dynamics 365) для установки приложения.</span><span class="sxs-lookup"><span data-stu-id="5abc4-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="5abc4-147">Согласиться с условиями.</span><span class="sxs-lookup"><span data-stu-id="5abc4-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="5abc4-148">Затем вы направляетесь на страницу **Управление решениями** .</span><span class="sxs-lookup"><span data-stu-id="5abc4-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="5abc4-149">Перейдите в раздел "ссылки центра партнеров" с помощью кнопок со стрелками в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="5abc4-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="5abc4-150">**Запланированная установка** должна отображаться рядом с решением "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="5abc4-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="5abc4-151">Установка займет 10-15 минут.</span><span class="sxs-lookup"><span data-stu-id="5abc4-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="5abc4-152">После завершения установки вернитесь к [Power автоматизиру](https://flow.microsoft.com) и выберите **решения** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="5abc4-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="5abc4-153">Обратите внимание, что в списке решений можно найти **ссылку Центр партнеров синхронизация для Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="5abc4-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="5abc4-154">Выберите **ссылку Центр партнеров синхронизация для Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="5abc4-155">Доступны следующие потоки и сущности Power автоматизировать:</span><span class="sxs-lookup"><span data-stu-id="5abc4-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Открыть AppSource":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="5abc4-157">Рекомендации: Протестируйте перед переходом в динамический</span><span class="sxs-lookup"><span data-stu-id="5abc4-157">Best practice: test before you go live</span></span>

<span data-ttu-id="5abc4-158">Прежде чем устанавливать, настраивать и настраивать решение Power Автоматизация в рабочей среде, обязательно протестируйте решение на промежуточном экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="5abc4-159">Установите решение Microsoft Power автоматизируя в промежуточной среде или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="5abc4-160">Создайте копию решения и запустите настройку потока настройки и автоматизации энергосбережения в промежуточной среде.</span><span class="sxs-lookup"><span data-stu-id="5abc4-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="5abc4-161">Протестируйте решение в промежуточном или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="5abc4-162">При успешном выполнении импортируйте в рабочий экземпляр как управляемое решение.</span><span class="sxs-lookup"><span data-stu-id="5abc4-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="5abc4-163">Настройка решения</span><span class="sxs-lookup"><span data-stu-id="5abc4-163">Configure the solution</span></span>

1. <span data-ttu-id="5abc4-164">После установки решения в экземпляре CRM вернитесь к [Power автоматизиру](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="5abc4-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="5abc4-165">В раскрывающемся списке **среды** в правом верхнем углу выберите экземпляр CRM, в котором было установлено решение Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5abc4-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="5abc4-166">Вам потребуется создать подключения, связывающие три учетные записи пользователей:</span><span class="sxs-lookup"><span data-stu-id="5abc4-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="5abc4-167">Пользователь центра партнеров с учетными данными администратора ссылок</span><span class="sxs-lookup"><span data-stu-id="5abc4-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="5abc4-168">События Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5abc4-168">Partner Center Events</span></span>

   - <span data-ttu-id="5abc4-169">Администратор CRM с потоками Power автоматизиру в решении.</span><span class="sxs-lookup"><span data-stu-id="5abc4-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="5abc4-170">В области навигации слева выберите **подключения** и в списке выберите решение "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="5abc4-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="5abc4-171">Создайте подключение, щелкнув **создать соединение**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Открыть AppSource":::

      3. <span data-ttu-id="5abc4-173">Поиск **ссылок центра партнеров (Предварительная версия)** на панели поиска в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="5abc4-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="5abc4-174">Создайте подключение для пользователя центра партнеров с ролью учетных данных администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="5abc4-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="5abc4-175">Затем создайте подключение к событиям центра партнеров для пользователя центра партнеров с учетными данными администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="5abc4-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="5abc4-176">Создайте подключение для Common Data Service (текущего окружения) для пользователя администратора CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="5abc4-177">Чтобы связать Power автоматизирующие потоки с подключениями, измените каждый из потоков Power автоматизиру, чтобы подключиться к Common Data Service и ссылкам центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-177">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="5abc4-178">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="5abc4-178">Save the changes.</span></span>

5. <span data-ttu-id="5abc4-179">**Включите** потоки Power автоматизирующие.</span><span class="sxs-lookup"><span data-stu-id="5abc4-179">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="5abc4-180">Использование API веб-перехватчика для регистрации событий изменения ресурсов</span><span class="sxs-lookup"><span data-stu-id="5abc4-180">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="5abc4-181">Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5abc4-181">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="5abc4-182">Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.</span><span class="sxs-lookup"><span data-stu-id="5abc4-182">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="5abc4-183">Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.</span><span class="sxs-lookup"><span data-stu-id="5abc4-183">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="5abc4-184">Добавьте подключения для пользователя центра партнеров (a.) с ссылками на учетные данные администратора (b), как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="5abc4-184">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Открыть AppSource":::

3. <span data-ttu-id="5abc4-186">При выполнении этих обновлений вы увидите</span><span class="sxs-lookup"><span data-stu-id="5abc4-186">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Открыть AppSource":::

4. <span data-ttu-id="5abc4-188">Сохраните изменения и выберите **включить**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-188">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="5abc4-189">Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5abc4-189">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="5abc4-190">Выберите пункт **Центр партнеров для Dynamics 365 (Предварительная версия)**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-190">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="5abc4-191">Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-191">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="5abc4-192">Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="5abc4-192">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Открыть AppSource":::

8. <span data-ttu-id="5abc4-194">Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-194">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="5abc4-195">Убедитесь, что в правой части окна откроется окно "запуск потока", и нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-195">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="5abc4-196">Введите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="5abc4-196">Enter the following details:</span></span>

    1. <span data-ttu-id="5abc4-197">**Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага</span><span class="sxs-lookup"><span data-stu-id="5abc4-197">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="5abc4-198">**Регистрируемые события**: "Создание ссылок" и "обновление ссылок"</span><span class="sxs-lookup"><span data-stu-id="5abc4-198">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="5abc4-199">**Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки).</span><span class="sxs-lookup"><span data-stu-id="5abc4-199">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="5abc4-200">Выберите **выполнить** , а затем нажмите кнопку **Готово.**</span><span class="sxs-lookup"><span data-stu-id="5abc4-200">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="5abc4-201">Теперь веб-перехватчик может прослушивать события создания и обновления.</span><span class="sxs-lookup"><span data-stu-id="5abc4-201">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="5abc4-202">Настройка шагов синхронизации</span><span class="sxs-lookup"><span data-stu-id="5abc4-202">Customize synchronization steps</span></span>

<span data-ttu-id="5abc4-203">Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.</span><span class="sxs-lookup"><span data-stu-id="5abc4-203">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="5abc4-204">Часто системы CRM сильно настроены.</span><span class="sxs-lookup"><span data-stu-id="5abc4-204">Often CRM systems are highly customized.</span></span> <span data-ttu-id="5abc4-205">Можно настроить потоки автоматизации Powering.</span><span class="sxs-lookup"><span data-stu-id="5abc4-205">You can customize the Power Automate flows.</span></span> <span data-ttu-id="5abc4-206">Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5abc4-206">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="5abc4-207">Предоставляются сопоставления центров партнеров Майкрософт с CRM, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.</span><span class="sxs-lookup"><span data-stu-id="5abc4-207">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="5abc4-208">В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать.</span><span class="sxs-lookup"><span data-stu-id="5abc4-208">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="5abc4-209">Ниже приведены примеры доступных настроек.</span><span class="sxs-lookup"><span data-stu-id="5abc4-209">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="5abc4-210">Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="5abc4-210">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="5abc4-211">a.</span><span class="sxs-lookup"><span data-stu-id="5abc4-211">a.</span></span> <span data-ttu-id="5abc4-212">Выберите пункт Центр партнеров для Dynamics 365 (Предварительная версия) или центр партнеров в Salesforce (Предварительная версия для предварительной версии).</span><span class="sxs-lookup"><span data-stu-id="5abc4-212">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="5abc4-213">b.</span><span class="sxs-lookup"><span data-stu-id="5abc4-213">b.</span></span> <span data-ttu-id="5abc4-214">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5abc4-214">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="5abc4-215">c.</span><span class="sxs-lookup"><span data-stu-id="5abc4-215">c.</span></span> <span data-ttu-id="5abc4-216">Выберите **(область) синхронизация интереса или возможной сделки**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-216">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="5abc4-217">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **, если это новая доступная возможность, а затем**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-217">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="5abc4-218">Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-218">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="5abc4-219">Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="5abc4-219">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="5abc4-220">d.</span><span class="sxs-lookup"><span data-stu-id="5abc4-220">d.</span></span> <span data-ttu-id="5abc4-221">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, щелкните шаг "(область) синхронизация интереса или возможности".</span><span class="sxs-lookup"><span data-stu-id="5abc4-221">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="5abc4-222">д)</span><span class="sxs-lookup"><span data-stu-id="5abc4-222">e.</span></span> <span data-ttu-id="5abc4-223">Выберите **, если это обновление возможной сделки, а затем**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-223">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="5abc4-224">Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-224">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="5abc4-225">е)</span><span class="sxs-lookup"><span data-stu-id="5abc4-225">f.</span></span> <span data-ttu-id="5abc4-226">Выберите, **Если да** , а затем **обновить существующую возможную сделку**</span><span class="sxs-lookup"><span data-stu-id="5abc4-226">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="5abc4-227">Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5abc4-227">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="5abc4-228">a.</span><span class="sxs-lookup"><span data-stu-id="5abc4-228">a.</span></span> <span data-ttu-id="5abc4-229">Выберите **изменить**  , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5abc4-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="5abc4-230">b.</span><span class="sxs-lookup"><span data-stu-id="5abc4-230">b.</span></span> <span data-ttu-id="5abc4-231">Выберите **(область) синхронизировать возможную сделку**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-231">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="5abc4-232">c.</span><span class="sxs-lookup"><span data-stu-id="5abc4-232">c.</span></span> <span data-ttu-id="5abc4-233">Чтобы настроить сопоставления полей CRM для событий обновления, выберите **в случае разницы между ведущими объектами в центре партнеров и CRM**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-233">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="5abc4-234">d.</span><span class="sxs-lookup"><span data-stu-id="5abc4-234">d.</span></span> <span data-ttu-id="5abc4-235">Выберите подшаг, **Если да** , а затем разверните этот шаг, чтобы **Обновить ссылку на данные о возможностях**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-235">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="5abc4-236">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="5abc4-236">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="5abc4-237">Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?</span><span class="sxs-lookup"><span data-stu-id="5abc4-237">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="5abc4-238">a.</span><span class="sxs-lookup"><span data-stu-id="5abc4-238">a.</span></span> <span data-ttu-id="5abc4-239">Выберите **изменить**  , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5abc4-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="5abc4-240">b.</span><span class="sxs-lookup"><span data-stu-id="5abc4-240">b.</span></span> <span data-ttu-id="5abc4-241">Выберите **(область) синхронизация ссылок.**</span><span class="sxs-lookup"><span data-stu-id="5abc4-241">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="5abc4-242">c.</span><span class="sxs-lookup"><span data-stu-id="5abc4-242">c.</span></span> <span data-ttu-id="5abc4-243">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-243">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="5abc4-244">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="5abc4-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="5abc4-245">Сквозная синхронизация двунаправленной совместной продажи</span><span class="sxs-lookup"><span data-stu-id="5abc4-245">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="5abc4-246">После установки, настройки и настройки решения Power автоматизиру вы можете протестировать синхронизацию ссылок совместной продажи между Dynamics 365 и центром партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-246">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="5abc4-247">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5abc4-247">Pre-requisites</span></span>

<span data-ttu-id="5abc4-248">Чтобы синхронизировать ссылки в центре партнеров и Dynamics 365 CRM, решение Power автоматизиру четко обозначает поля ссылок, относящиеся к корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5abc4-248">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="5abc4-249">Эта идентификация дает группе продавцов возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="5abc4-249">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="5abc4-250">Набор настраиваемых полей доступен как часть сущности **возможной сделки** .</span><span class="sxs-lookup"><span data-stu-id="5abc4-250">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="5abc4-251">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="5abc4-251">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="5abc4-252">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="5abc4-252">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="5abc4-253">**Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5abc4-253">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="5abc4-254">**Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5abc4-254">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="5abc4-255">**Ссылка на ссылку: ссылка**только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5abc4-255">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="5abc4-256">**Как можно получить справку Майкрософт?**: Помогите корпорации Майкрософт получить ссылку</span><span class="sxs-lookup"><span data-stu-id="5abc4-256">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="5abc4-257">**Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="5abc4-257">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="5abc4-258">**Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5abc4-258">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="5abc4-259">ВАРИАНТ</span><span class="sxs-lookup"><span data-stu-id="5abc4-259">SCENARIOS:</span></span>

1. <span data-ttu-id="5abc4-260">Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="5abc4-260">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="5abc4-261">Войдите в среду Dynamics 365 CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-261">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="5abc4-262">При создании "новой возможности" в среде Dynamics 365 убедитесь, что указан следующий раздел:</span><span class="sxs-lookup"><span data-stu-id="5abc4-262">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Открыть AppSource":::

   3. <span data-ttu-id="5abc4-264">Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="5abc4-264">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="5abc4-265">**Синхронизация с центром партнеров**: Да</span><span class="sxs-lookup"><span data-stu-id="5abc4-265">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="5abc4-266">**Как можно получить справку Майкрософт?**: выберите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="5abc4-266">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Открыть AppSource":::

      - <span data-ttu-id="5abc4-268">**Продукты**: идентификаторы решений для продукта</span><span class="sxs-lookup"><span data-stu-id="5abc4-268">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="5abc4-269">После создания возможности в Dynamics 365 с параметром **Синхронизация с центром партнеров** задайте значение **Да**, подождите 10 минут и войдите в свою учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-269">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="5abc4-270">Ваши ссылки будут синхронизированы с Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5abc4-270">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="5abc4-271">Аналогично, для возможности, для которой параметр "Синхронизация с центром партнеров" имеет значение "Да", при обновлении возможности в Dynamics 365 CRM изменения будут синхронизированы в учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-271">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="5abc4-272">Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5abc4-272">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="5abc4-273">Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="5abc4-273">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="5abc4-274">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5abc4-274">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="5abc4-275">В меню слева выберите **ссылки** .</span><span class="sxs-lookup"><span data-stu-id="5abc4-275">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="5abc4-276">Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".</span><span class="sxs-lookup"><span data-stu-id="5abc4-276">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="5abc4-277">Войдите в среду Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-277">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="5abc4-278">Перейдите к разделу **открытые возможности**.</span><span class="sxs-lookup"><span data-stu-id="5abc4-278">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="5abc4-279">Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="5abc4-279">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="5abc4-280">При выборе синхронизированной ссылки сведения о представлении карточки заполняются.</span><span class="sxs-lookup"><span data-stu-id="5abc4-280">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5abc4-281">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5abc4-281">Next steps</span></span>

- [<span data-ttu-id="5abc4-282">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="5abc4-282">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="5abc4-283">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="5abc4-283">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="5abc4-284">Дополнительные сведения о платформе Microsoft Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="5abc4-284">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="5abc4-285">Веб-перехватчики Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5abc4-285">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)