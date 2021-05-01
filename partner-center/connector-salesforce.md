---
title: Соединитель для совместной продажи в центре партнеров для Salesforce CRM
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Синхронизируйте свои ссылки в центре партнеров с помощью Salesforce CRM. Продавцов может совместно продаваться с корпорацией Майкрософт в ваших системах CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284389"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="e3090-104">Соединитель для совместных продаж для Salesforce CRM — обзор</span><span class="sxs-lookup"><span data-stu-id="e3090-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="e3090-105">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="e3090-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e3090-106">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="e3090-106">Referrals admin</span></span>
- <span data-ttu-id="e3090-107">Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="e3090-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="e3090-108">Соединитель совместных продаж в центре партнеров позволяет продавцов совместную продажу с корпорацией Майкрософт в ваших системах CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="e3090-109">Они не должны быть обучены для использования центра партнеров для управления сделками в совместных продажах.</span><span class="sxs-lookup"><span data-stu-id="e3090-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="e3090-110">Используя соединители совместной работы, вы можете создать новую ссылку для совместной продажи, чтобы привлечь продавца Майкрософт, получать ссылки от продавца Майкрософт, принимать или отклонять ссылки, изменять данные сделки, такие как стоимость сделки и дату закрытия.</span><span class="sxs-lookup"><span data-stu-id="e3090-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="e3090-111">Вы также можете получить обновления от Microsoft продавцов для этих сделок совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="e3090-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="e3090-112">Все ваши ссылки можно выполнять при работе в CRM по вашему выбору, а не в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="e3090-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="e3090-113">Решение основано на решении Microsoft Power Автоматизируing и использует API-интерфейсы центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="e3090-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="e3090-114">Перед установкой предварительных требований</span><span class="sxs-lookup"><span data-stu-id="e3090-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="e3090-115">**Разделы**</span><span class="sxs-lookup"><span data-stu-id="e3090-115">**Topics**</span></span>   |<span data-ttu-id="e3090-116">**Сведения**</span><span class="sxs-lookup"><span data-stu-id="e3090-116">**Details**</span></span>   |<span data-ttu-id="e3090-117">**Ссылки**</span><span class="sxs-lookup"><span data-stu-id="e3090-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="e3090-118">Идентификатор Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="e3090-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="e3090-119">Требуется допустимый идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="e3090-119">You need a valid MPN ID</span></span>|<span data-ttu-id="e3090-120">Присоединение к [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="e3090-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="e3090-121">Готовность к совместной продаже</span><span class="sxs-lookup"><span data-stu-id="e3090-121">Co-sell ready</span></span>|<span data-ttu-id="e3090-122">Ваше решение для работы с IP-адресами и службами должно быть готово к совместной продаже.</span><span class="sxs-lookup"><span data-stu-id="e3090-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="e3090-123">Продажа с Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e3090-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="e3090-124">Учетная запись Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="e3090-124">Partner Center account</span></span>|<span data-ttu-id="e3090-125">Идентификатор MPN, связанный с клиентом центра партнеров, должен совпадать с ИДЕНТИФИКАТОРом MPN, связанным с решением для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="e3090-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="e3090-126">Прежде чем развертывать соединители, убедитесь, что вы видите ссылки на совместные продажи на портале центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="e3090-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="e3090-127">Управляйте своей учетной записью</span><span class="sxs-lookup"><span data-stu-id="e3090-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="e3090-128">Роли пользователей Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="e3090-128">Partner Center user roles</span></span>|<span data-ttu-id="e3090-129">Сотрудник, который будет устанавливать и использовать соединители, должен быть администратором ссылок.</span><span class="sxs-lookup"><span data-stu-id="e3090-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="e3090-130">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="e3090-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="e3090-131">SalesForce CRM</span><span class="sxs-lookup"><span data-stu-id="e3090-131">Salesforce CRM</span></span>|<span data-ttu-id="e3090-132">Роль пользователя CRM — системный администратор или Настройщик системы</span><span class="sxs-lookup"><span data-stu-id="e3090-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="e3090-133">Назначение ролей в Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e3090-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="e3090-134">Учетная запись потока Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="e3090-134">Power Automate Flow Account</span></span>|<span data-ttu-id="e3090-135">Активная учетная запись [Power автоматизируется](https://flow.microsoft.com) для системного администратора CRM или настройщика системы.</span><span class="sxs-lookup"><span data-stu-id="e3090-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="e3090-136">Этот пользователь должен войти в [Power автоматизиру](https://flow.microsoft.com) по крайней мере один раз перед установкой.</span><span class="sxs-lookup"><span data-stu-id="e3090-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="e3090-137">Установка пакета salesforce для настраиваемых полей Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e3090-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="e3090-138">Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, в решении Power автоматизируется необходимость четко определять поля ссылок, относящиеся к корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e3090-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="e3090-139">Эта разделительной предоставляет группам продавцов-партнеров возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="e3090-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="e3090-140">В Salesforce активируйте **заметки** и добавьте их в список возможных сделок.</span><span class="sxs-lookup"><span data-stu-id="e3090-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="e3090-141">Ссылка</span><span class="sxs-lookup"><span data-stu-id="e3090-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="e3090-142">Активируйте **группы возможных сделок** , выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="e3090-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="e3090-143">В программе установки используйте поле **Быстрый поиск** , чтобы найти параметры группы возможных сделок.</span><span class="sxs-lookup"><span data-stu-id="e3090-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="e3090-144">При необходимости задайте необходимые параметры.</span><span class="sxs-lookup"><span data-stu-id="e3090-144">Define the settings as needed.</span></span>
[<span data-ttu-id="e3090-145">Ссылка</span><span class="sxs-lookup"><span data-stu-id="e3090-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="e3090-146">В Salesforce установите настраиваемые поля и объекты с помощью [установщика пакетов](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="e3090-146">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="e3090-147">Используйте его для установки пакета в любую компанию.</span><span class="sxs-lookup"><span data-stu-id="e3090-147">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="e3090-148">При установке в песочницу необходимо заменить начальную часть URL-адреса на http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="e3090-148">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="e3090-149">В Salesforce добавьте решения Майкрософт в список, связанный с **возможной сделкой** .</span><span class="sxs-lookup"><span data-stu-id="e3090-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="e3090-150">После добавления щелкните значок **гаечного ключа** и обновите свойства.</span><span class="sxs-lookup"><span data-stu-id="e3090-150">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="e3090-151">Рекомендации: Протестируйте перед переходом в динамический</span><span class="sxs-lookup"><span data-stu-id="e3090-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="e3090-152">Прежде чем устанавливать, настраивать и настраивать решение Power Автоматизация в рабочей среде, обязательно протестируйте решение на промежуточном экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="e3090-153">Установите решение Microsoft Power автоматизируя в промежуточной среде или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="e3090-154">Создайте копию решения и запустите настройку потока настройки и автоматизации энергосбережения в промежуточной среде.</span><span class="sxs-lookup"><span data-stu-id="e3090-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="e3090-155">Протестируйте решение в промежуточном или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="e3090-156">В случае успеха импортируйте в рабочий экземпляр в качестве управляемого решения.</span><span class="sxs-lookup"><span data-stu-id="e3090-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="e3090-157">Установка синхронизации ссылок центра партнеров для Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e3090-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="e3090-158">Откройте [Power автоматизиру](https://flow.microsoft.com) и выберите **среды** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="e3090-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="e3090-159">Будут показаны доступные экземпляры CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="e3090-160">Выберите нужный экземпляр CRM в раскрывающемся списке в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="e3090-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="e3090-161">Выберите **решения** на панели навигации слева.</span><span class="sxs-lookup"><span data-stu-id="e3090-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="e3090-162">Выберите ссылку **Open AppSource (открыть** ) в верхнем меню.</span><span class="sxs-lookup"><span data-stu-id="e3090-162">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Открыть AppSource":::

5. <span data-ttu-id="e3090-164">Найдите **соединители центров партнеров для Salesforce** во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="e3090-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="e3090-166">Нажмите кнопку **получить сейчас** и **Продолжайте**.</span><span class="sxs-lookup"><span data-stu-id="e3090-166">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="e3090-167">Откроется страница, на которой можно выбрать среду CRM salesforce для установки приложения.</span><span class="sxs-lookup"><span data-stu-id="e3090-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="e3090-168">Согласиться с условиями.</span><span class="sxs-lookup"><span data-stu-id="e3090-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Доступные КРМС":::

8. <span data-ttu-id="e3090-170">Затем вы направляетесь на страницу **Управление решениями** .</span><span class="sxs-lookup"><span data-stu-id="e3090-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="e3090-171">Перейдите в раздел "ссылки центра партнеров" с помощью кнопок со стрелками в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="e3090-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="e3090-172">**Запланированная установка** должна отображаться рядом с решением "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="e3090-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="e3090-173">Установка займет 10-15 минут.</span><span class="sxs-lookup"><span data-stu-id="e3090-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="e3090-174">После завершения установки вернитесь к [Power автоматизиру](https://flow.microsoft.com) и выберите **решения** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="e3090-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="e3090-175">Обратите внимание, что **Синхронизация ссылок центра партнеров по Salesforce** доступна в списке решений.</span><span class="sxs-lookup"><span data-stu-id="e3090-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="e3090-176">Выберите **ссылку Центр партнеров синхронизация для Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="e3090-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="e3090-177">Доступны следующие потоки и сущности Power автоматизировать:</span><span class="sxs-lookup"><span data-stu-id="e3090-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Потоки Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="e3090-179">Настройка решения</span><span class="sxs-lookup"><span data-stu-id="e3090-179">Configure the solution</span></span>

1. <span data-ttu-id="e3090-180">После установки решения в экземпляре CRM вернитесь к [Power автоматизиру](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="e3090-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="e3090-181">В раскрывающемся списке **среды** в правом верхнем углу выберите экземпляр CRM, в котором было установлено решение Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="e3090-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="e3090-182">Вам потребуется создать подключения, связывающие три учетные записи пользователей:</span><span class="sxs-lookup"><span data-stu-id="e3090-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="e3090-183">Пользователь центра партнеров с учетными данными администратора ссылок</span><span class="sxs-lookup"><span data-stu-id="e3090-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="e3090-184">События Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="e3090-184">Partner Center Events</span></span>
    - <span data-ttu-id="e3090-185">Администратор CRM с потоками Power автоматизиру в решении.</span><span class="sxs-lookup"><span data-stu-id="e3090-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="e3090-186">В области навигации слева выберите **подключения** и в списке выберите решение "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="e3090-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="e3090-187">Создайте подключение, щелкнув **создать соединение**.</span><span class="sxs-lookup"><span data-stu-id="e3090-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Создание подключения":::

- <span data-ttu-id="e3090-189">Поиск ссылок центра партнеров (Предварительная версия) на панели поиска в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="e3090-189">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="e3090-190">Создайте подключение для пользователя центра партнеров с ролью учетных данных администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="e3090-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="e3090-191">Затем создайте подключение к событиям центра партнеров для пользователя центра партнеров с учетными данными администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="e3090-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="e3090-192">Создайте подключение для Salesforce для пользователя администратора CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="e3090-193">После добавления всех подключений в вашей среде должны отобразиться следующие подключения:</span><span class="sxs-lookup"><span data-stu-id="e3090-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Наблюдение за подключениями":::

### <a name="edit-the-connections"></a><span data-ttu-id="e3090-195">Изменение подключений</span><span class="sxs-lookup"><span data-stu-id="e3090-195">Edit the connections</span></span>

1. <span data-ttu-id="e3090-196">Вернитесь на страницу решения и выберите **решение по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="e3090-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="e3090-197">Выберите **ссылку на подключение (Предварительная версия)** , щелкнув **все**.</span><span class="sxs-lookup"><span data-stu-id="e3090-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Начать изменение соединителя":::

2. <span data-ttu-id="e3090-199">Измените каждое подключение по отдельности, щелкнув значок с тремя точками.</span><span class="sxs-lookup"><span data-stu-id="e3090-199">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="e3090-200">Добавьте соответствующие подключения.</span><span class="sxs-lookup"><span data-stu-id="e3090-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Изменение соединителей":::

3. <span data-ttu-id="e3090-202">Включите потоки в следующей последовательности:</span><span class="sxs-lookup"><span data-stu-id="e3090-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="e3090-203">Регистрация веб-перехватчика центра партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3090-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="e3090-204">Создание ссылки на совместную продажу — Salesforce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3090-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e3090-205">Центр партнеров обновления справочных обновлений в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3090-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e3090-206">Центр партнеров в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3090-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e3090-207">SalesForce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3090-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e3090-208">Возможность Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3090-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e3090-209">Решения Майкрософт для Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3090-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="e3090-210">Использование API веб-перехватчика для регистрации событий изменения ресурсов</span><span class="sxs-lookup"><span data-stu-id="e3090-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="e3090-211">Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e3090-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="e3090-212">Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.</span><span class="sxs-lookup"><span data-stu-id="e3090-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="e3090-213">Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.</span><span class="sxs-lookup"><span data-stu-id="e3090-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="e3090-214">Добавьте подключения для пользователя центра партнеров (a.) с ссылками на учетные данные администратора (b), как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="e3090-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Триггер":::

3. <span data-ttu-id="e3090-216">При выполнении этих обновлений вы увидите</span><span class="sxs-lookup"><span data-stu-id="e3090-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Объекты Webhook":::

4. <span data-ttu-id="e3090-218">Сохраните изменения и выберите **включить**.</span><span class="sxs-lookup"><span data-stu-id="e3090-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="e3090-219">Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="e3090-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="e3090-220">Выберите **Центр партнеров для SALESFORCE CRM (Предварительная версия)**.</span><span class="sxs-lookup"><span data-stu-id="e3090-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="e3090-221">Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.</span><span class="sxs-lookup"><span data-stu-id="e3090-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="e3090-222">Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="e3090-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Копирование URL-адреса":::

8. <span data-ttu-id="e3090-224">Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.</span><span class="sxs-lookup"><span data-stu-id="e3090-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="e3090-225">Убедитесь, что окно "запуск потока" открывается на правой панели, и нажмите кнопку " **продолжить**".</span><span class="sxs-lookup"><span data-stu-id="e3090-225">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="e3090-226">Введите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="e3090-226">Enter the following details:</span></span>

    1. <span data-ttu-id="e3090-227">**Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага</span><span class="sxs-lookup"><span data-stu-id="e3090-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="e3090-228">**Регистрируемые события**: "Создание ссылок" и "обновление ссылок"</span><span class="sxs-lookup"><span data-stu-id="e3090-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="e3090-229">**Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки).</span><span class="sxs-lookup"><span data-stu-id="e3090-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="e3090-230">Выберите **выполнить** , а затем нажмите кнопку **Готово.**</span><span class="sxs-lookup"><span data-stu-id="e3090-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="e3090-231">Теперь веб-перехватчик может прослушивать события создания и обновления.</span><span class="sxs-lookup"><span data-stu-id="e3090-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="e3090-232">Настройка шагов синхронизации</span><span class="sxs-lookup"><span data-stu-id="e3090-232">Customize synchronization steps</span></span>

<span data-ttu-id="e3090-233">Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.</span><span class="sxs-lookup"><span data-stu-id="e3090-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="e3090-234">Часто системы CRM сильно настроены.</span><span class="sxs-lookup"><span data-stu-id="e3090-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="e3090-235">Можно настроить потоки автоматизации Powering.</span><span class="sxs-lookup"><span data-stu-id="e3090-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="e3090-236">Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="e3090-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="e3090-237">Предоставляются сопоставления центров партнеров Майкрософт с CRM, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.</span><span class="sxs-lookup"><span data-stu-id="e3090-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="e3090-238">В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать.</span><span class="sxs-lookup"><span data-stu-id="e3090-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="e3090-239">Ниже приведены примеры доступных настроек.</span><span class="sxs-lookup"><span data-stu-id="e3090-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="e3090-240">Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="e3090-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="e3090-241">Выберите центр партнеров для Salesforce CRM (Предварительная версия).</span><span class="sxs-lookup"><span data-stu-id="e3090-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="e3090-242">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="e3090-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="e3090-243">Выберите **(область) синхронизация интереса или возможной сделки**.</span><span class="sxs-lookup"><span data-stu-id="e3090-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="e3090-244">Чтобы настроить сопоставления полей CRM для создания событий, выберите **, если это новая доступная возможность, а затем**.</span><span class="sxs-lookup"><span data-stu-id="e3090-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="e3090-245">Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**.</span><span class="sxs-lookup"><span data-stu-id="e3090-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="e3090-246">Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="e3090-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="e3090-247">Чтобы настроить сопоставления полей CRM для событий обновления, выберите шаг "(область) синхронизация интереса или возможности".</span><span class="sxs-lookup"><span data-stu-id="e3090-247">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="e3090-248">Выберите **, если это обновление возможной сделки, а затем**.</span><span class="sxs-lookup"><span data-stu-id="e3090-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="e3090-249">Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.</span><span class="sxs-lookup"><span data-stu-id="e3090-249">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="e3090-250">Выберите, **Если да** , а затем **обновить существующую возможную сделку**</span><span class="sxs-lookup"><span data-stu-id="e3090-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="e3090-251">Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="e3090-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="e3090-252">Выберите **изменить**  , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="e3090-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="e3090-253">Выберите **(область) синхронизировать возможную сделку**.</span><span class="sxs-lookup"><span data-stu-id="e3090-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="e3090-254">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, установите флажок, **Если между ведущими объектами в центре партнеров и CRM есть различия**.</span><span class="sxs-lookup"><span data-stu-id="e3090-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="e3090-255">Выберите подшаг, **Если да** , а затем разверните этот шаг, чтобы **Обновить ссылку на данные о возможностях**.</span><span class="sxs-lookup"><span data-stu-id="e3090-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="e3090-256">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="e3090-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="e3090-257">Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?</span><span class="sxs-lookup"><span data-stu-id="e3090-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="e3090-258">Выберите **изменить**  , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="e3090-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="e3090-259">Выберите **(область) синхронизация ссылок.**</span><span class="sxs-lookup"><span data-stu-id="e3090-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="e3090-260">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="e3090-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="e3090-261">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="e3090-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="e3090-262">Сквозная синхронизация двунаправленной совместной продажи</span><span class="sxs-lookup"><span data-stu-id="e3090-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="e3090-263">После установки, настройки и настройки решения Power автоматизиру вы можете протестировать синхронизацию ссылок для совместной продажи между Salesforce CRM и центром партнеров.</span><span class="sxs-lookup"><span data-stu-id="e3090-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="e3090-264">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e3090-264">Pre-requisites</span></span>

<span data-ttu-id="e3090-265">Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, решение Power автоматизирует необходимость четко разграничения ссылочные поля Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e3090-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="e3090-266">Эта идентификация предоставляет группам продавцов возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="e3090-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="e3090-267">Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможности** решения Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="e3090-268">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="e3090-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="e3090-269">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="e3090-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="e3090-270">**Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e3090-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="e3090-271">**Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e3090-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="e3090-272">**Ссылка на ссылку: ссылка** только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e3090-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="e3090-273">**Как можно** получить помощь от корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e3090-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="e3090-274">**Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="e3090-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="e3090-275">**Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров</span><span class="sxs-lookup"><span data-stu-id="e3090-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="e3090-276">ВАРИАНТ</span><span class="sxs-lookup"><span data-stu-id="e3090-276">SCENARIOS:</span></span>

1. <span data-ttu-id="e3090-277">Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="e3090-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="e3090-278">Войдите в среду Salesforce CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="e3090-279">При создании "новой возможности" в среде Salesforce CRM убедитесь, что следующий раздел существует.</span><span class="sxs-lookup"><span data-stu-id="e3090-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Среда Salesforce":::

   3. <span data-ttu-id="e3090-281">Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="e3090-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="e3090-282">"Синхронизация с центром партнеров": Да</span><span class="sxs-lookup"><span data-stu-id="e3090-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="e3090-283">«Как можно получить справку Майкрософт?»: выберите следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="e3090-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="e3090-284">Продукты: идентификаторы решений для продукта</span><span class="sxs-lookup"><span data-stu-id="e3090-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="e3090-285">Установив для параметра синхронизация возможных сделок  **с центром партнеров** значение **Да**, подождите 10 минут, войдите в свою учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="e3090-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="e3090-286">Ваши ссылки будут синхронизированы с Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="e3090-287">Если параметр "синхронизировать с центром партнеров" имеет значение "Да", то при обновлении возможной сделки в Salesforce CRM изменения будут синхронизироваться с учетной записью центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="e3090-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="e3090-288">Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="e3090-289">Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="e3090-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="e3090-290">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="e3090-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="e3090-291">В меню слева выберите **ссылки** .</span><span class="sxs-lookup"><span data-stu-id="e3090-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="e3090-292">Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".</span><span class="sxs-lookup"><span data-stu-id="e3090-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="e3090-293">Войдите в среду Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="e3090-294">Перейдите к разделу **открытые возможности**.</span><span class="sxs-lookup"><span data-stu-id="e3090-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="e3090-295">Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="e3090-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Экран возможностей Salesforce":::

    6. <span data-ttu-id="e3090-297">При выборе синхронизированной ссылки сведения о представлении карточки заполняются.</span><span class="sxs-lookup"><span data-stu-id="e3090-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e3090-298">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e3090-298">Next steps</span></span>

- [<span data-ttu-id="e3090-299">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="e3090-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="e3090-300">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="e3090-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="e3090-301">Веб-перехватчики Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="e3090-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
