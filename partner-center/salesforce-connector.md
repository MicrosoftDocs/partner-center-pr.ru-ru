---
title: Соединитель для совместной продажи в центре партнеров для Salesforce CRM
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Использование соединителя Salesforce CRM для получения ссылок от Майкрософт
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825701"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="371dc-103">Соединитель совместных продаж для Salesforce CRM — обзор</span><span class="sxs-lookup"><span data-stu-id="371dc-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="371dc-104">Соответствующие роли</span><span class="sxs-lookup"><span data-stu-id="371dc-104">Appropriate roles</span></span>

- <span data-ttu-id="371dc-105">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="371dc-105">Referrals admin</span></span>
- <span data-ttu-id="371dc-106">Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="371dc-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="371dc-107">Соединитель совместных продаж в центре партнеров позволяет продавцов совместную продажу с корпорацией Майкрософт в ваших системах CRM.</span><span class="sxs-lookup"><span data-stu-id="371dc-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="371dc-108">Они не должны быть обучены для использования центра партнеров для управления сделками в совместных продажах.</span><span class="sxs-lookup"><span data-stu-id="371dc-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="371dc-109">Используя соединители совместной работы, вы сможете создать новую ссылку для совместной продажи, чтобы привлечь продавца Майкрософт, получать ссылки от продавцов Майкрософт, принимать/отклонять ссылки, изменять данные о сделках, такие как стоимость сделки, закрытие даты и т. д., а также получать обновления от Microsoft продавцов в отношении этих сделок совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="371dc-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="371dc-110">Все это можно сделать при работе в CRM по вашему выбору, а не в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="371dc-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="371dc-111">Решение основано на решении Microsoft Power Автоматизируing и использует API-интерфейсы центра партнеров Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="371dc-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="371dc-112">Перед установкой предварительных требований</span><span class="sxs-lookup"><span data-stu-id="371dc-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="371dc-113">**Разделы**</span><span class="sxs-lookup"><span data-stu-id="371dc-113">**Topics**</span></span>   |<span data-ttu-id="371dc-114">**Сведения**</span><span class="sxs-lookup"><span data-stu-id="371dc-114">**Details**</span></span>   |<span data-ttu-id="371dc-115">**Ссылки**</span><span class="sxs-lookup"><span data-stu-id="371dc-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="371dc-116">Идентификатор Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="371dc-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="371dc-117">Требуется допустимый идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="371dc-117">You need a valid MPN ID</span></span>|<span data-ttu-id="371dc-118">Присоединение к [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="371dc-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="371dc-119">Готовность к совместной продаже</span><span class="sxs-lookup"><span data-stu-id="371dc-119">Co-sell ready</span></span>|<span data-ttu-id="371dc-120">Ваше решение для работы с IP-адресами и службами должно быть готово к совместной продаже.</span><span class="sxs-lookup"><span data-stu-id="371dc-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="371dc-121">Продажа с Майкрософт</span><span class="sxs-lookup"><span data-stu-id="371dc-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="371dc-122">Учетная запись Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="371dc-122">Partner Center account</span></span>|<span data-ttu-id="371dc-123">Идентификатор MPN, связанный с клиентом центра партнеров, должен совпадать с ИДЕНТИФИКАТОРом MPN, связанным с решением для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="371dc-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="371dc-124">Прежде чем развертывать соединители, убедитесь, что вы видите ссылки на совместные продажи на портале центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="371dc-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="371dc-125">Управление учетной записью</span><span class="sxs-lookup"><span data-stu-id="371dc-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="371dc-126">Роли пользователей Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="371dc-126">Partner Center user roles</span></span>|<span data-ttu-id="371dc-127">Сотрудник, который будет устанавливать и использовать соединители, должен быть администратором ссылок.</span><span class="sxs-lookup"><span data-stu-id="371dc-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="371dc-128">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="371dc-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="371dc-129">SalesForce CRM</span><span class="sxs-lookup"><span data-stu-id="371dc-129">Salesforce CRM</span></span>|<span data-ttu-id="371dc-130">Роль пользователя CRM — системный администратор или Настройщик системы</span><span class="sxs-lookup"><span data-stu-id="371dc-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="371dc-131">Назначение ролей в Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="371dc-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="371dc-132">Учетная запись потока Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="371dc-132">Power Automate Flow Account</span></span>|<span data-ttu-id="371dc-133">Активная учетная запись [Power автоматизируется](https://flow.microsoft.com) для системного администратора CRM или настройщика системы.</span><span class="sxs-lookup"><span data-stu-id="371dc-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="371dc-134">Этот пользователь должен войти в [Power автоматизиру](https://flow.microsoft.com) по крайней мере один раз перед установкой.</span><span class="sxs-lookup"><span data-stu-id="371dc-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="371dc-135">Установка синхронизации ссылок центра партнеров для Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="371dc-135">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="371dc-136">Откройте [Power автоматизиру](https://flow.microsoft.com) и выберите **среды** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="371dc-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="371dc-137">Будут показаны доступные экземпляры CRM.</span><span class="sxs-lookup"><span data-stu-id="371dc-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="371dc-138">Выберите нужный экземпляр CRM в раскрывающемся списке в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="371dc-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="371dc-139">Выберите **решения** на панели навигации слева.</span><span class="sxs-lookup"><span data-stu-id="371dc-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="371dc-140">Щелкните ссылку **Open AppSource (открыть** ) в верхнем меню.</span><span class="sxs-lookup"><span data-stu-id="371dc-140">Click on the **Open AppSource** link on the top menu.</span></span>

![Открыть AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="371dc-142">Найдите **соединители центров партнеров для Salesforce** во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="371dc-142">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

6. <span data-ttu-id="371dc-143">Нажмите кнопку **получить сейчас** и **Продолжайте**.</span><span class="sxs-lookup"><span data-stu-id="371dc-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="371dc-144">Откроется страница, на которой можно выбрать среду CRM (Dynamics 365) для установки приложения.</span><span class="sxs-lookup"><span data-stu-id="371dc-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="371dc-145">Согласиться с условиями.</span><span class="sxs-lookup"><span data-stu-id="371dc-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="371dc-146">Затем вы направляетесь на страницу **Управление решениями** .</span><span class="sxs-lookup"><span data-stu-id="371dc-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="371dc-147">Перейдите в раздел "ссылки центра партнеров" с помощью кнопок со стрелками в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="371dc-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="371dc-148">**Запланированная установка** должна отображаться рядом с решением "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="371dc-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="371dc-149">Установка займет 10-15 минут.</span><span class="sxs-lookup"><span data-stu-id="371dc-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="371dc-150">После завершения установки вернитесь к [Power автоматизиру](https://flow.microsoft.com) и выберите **решения** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="371dc-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="371dc-151">Обратите внимание, что **Синхронизация ссылок центра партнеров по Salesforce** доступна в списке решений.</span><span class="sxs-lookup"><span data-stu-id="371dc-151">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="371dc-152">Выберите **ссылку Центр партнеров синхронизация для Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="371dc-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="371dc-153">Доступны следующие потоки и сущности Power автоматизировать:</span><span class="sxs-lookup"><span data-stu-id="371dc-153">The following Power Automate flows and entities are available:</span></span>

![Доступные КРМС](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="371dc-155">Рекомендации: Протестируйте перед переходом в динамический</span><span class="sxs-lookup"><span data-stu-id="371dc-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="371dc-156">Прежде чем устанавливать, настраивать и настраивать решение Power Автоматизация в рабочей среде, обязательно протестируйте решение на промежуточном экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="371dc-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="371dc-157">Установите решение Microsoft Power автоматизируя в промежуточной среде или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="371dc-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="371dc-158">Создайте копию решения, а затем выполните настройку и настройку потоков Power автоматизиру в промежуточной среде.</span><span class="sxs-lookup"><span data-stu-id="371dc-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="371dc-159">Протестируйте решение в промежуточном или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="371dc-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="371dc-160">При успешном выполнении импортируйте в рабочий экземпляр как управляемое решение.</span><span class="sxs-lookup"><span data-stu-id="371dc-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="371dc-161">Настройка решения</span><span class="sxs-lookup"><span data-stu-id="371dc-161">Configure the solution</span></span>

1. <span data-ttu-id="371dc-162">После установки решения в экземпляре CRM вернитесь к [Power автоматизиру](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="371dc-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="371dc-163">В раскрывающемся списке **среды** в правом верхнем углу выберите экземпляр CRM, в котором было установлено решение Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="371dc-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="371dc-164">Вам потребуется создать подключения, связывающие три учетные записи пользователей:</span><span class="sxs-lookup"><span data-stu-id="371dc-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="371dc-165">Пользователь центра партнеров с учетными данными администратора ссылок</span><span class="sxs-lookup"><span data-stu-id="371dc-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="371dc-166">События Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="371dc-166">Partner Center Events</span></span>
- <span data-ttu-id="371dc-167">Администратор CRM с потоками Power автоматизиру в решении.</span><span class="sxs-lookup"><span data-stu-id="371dc-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="371dc-168">а.</span><span class="sxs-lookup"><span data-stu-id="371dc-168">a.</span></span> <span data-ttu-id="371dc-169">В области навигации слева выберите **подключения** и в списке выберите решение "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="371dc-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="371dc-170">b.</span><span class="sxs-lookup"><span data-stu-id="371dc-170">b.</span></span> <span data-ttu-id="371dc-171">Создайте подключение, щелкнув **создать соединение**.</span><span class="sxs-lookup"><span data-stu-id="371dc-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![Создание подключения](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="371dc-173">c.</span><span class="sxs-lookup"><span data-stu-id="371dc-173">c.</span></span> <span data-ttu-id="371dc-174">Поиск **ссылок центра партнеров (Предварительная версия)** в строке поиска в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="371dc-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="371dc-175">г.</span><span class="sxs-lookup"><span data-stu-id="371dc-175">d.</span></span> <span data-ttu-id="371dc-176">Создайте подключение для пользователя центра партнеров с ролью учетных данных администратора ссылок. &.</span><span class="sxs-lookup"><span data-stu-id="371dc-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="371dc-177">Затем создайте подключение к событиям центра партнеров для пользователя центра партнеров с учетными данными администратора ссылок. ж.</span><span class="sxs-lookup"><span data-stu-id="371dc-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="371dc-178">Создайте подключение для Common Data Service (текущего окружения) для пользователя администратора CRM.</span><span class="sxs-lookup"><span data-stu-id="371dc-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="371dc-179">Чтобы связать Power автоматизирующие потоки с подключениями, измените каждый из потоков Power автоматизиру, чтобы подключиться к Common Data Service и ссылкам центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="371dc-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="371dc-180">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="371dc-180">Save the changes.</span></span>

5. <span data-ttu-id="371dc-181">**Включите** потоки Power автоматизирующие.</span><span class="sxs-lookup"><span data-stu-id="371dc-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="371dc-182">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="371dc-182">Next steps</span></span>

- [<span data-ttu-id="371dc-183">Использование веб-перехватчиков для получения событий изменения ресурсов</span><span class="sxs-lookup"><span data-stu-id="371dc-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="371dc-184">Дополнительные сведения о платформе Microsoft Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="371dc-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="371dc-185">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="371dc-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="371dc-186">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="371dc-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
