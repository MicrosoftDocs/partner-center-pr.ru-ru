---
title: Соединитель для совместной продажи в центре партнеров для Salesforce CRM
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Синхронизация ссылок в центре партнеров с помощью Salesforce CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 1b658f04b1348eb48f694fac069518a7a7fc6a70
ms.sourcegitcommit: 505c38436780a31692f5f5694830fcfe01502977
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "91372854"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="5fdf5-103">Соединитель для совместных продаж для Salesforce CRM — обзор</span><span class="sxs-lookup"><span data-stu-id="5fdf5-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="5fdf5-104">Соответствующие роли</span><span class="sxs-lookup"><span data-stu-id="5fdf5-104">Appropriate roles</span></span>

- <span data-ttu-id="5fdf5-105">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="5fdf5-105">Referrals admin</span></span>
- <span data-ttu-id="5fdf5-106">Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="5fdf5-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="5fdf5-107">Соединитель совместных продаж в центре партнеров позволяет продавцов совместную продажу с корпорацией Майкрософт в ваших системах CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="5fdf5-108">Они не должны быть обучены для использования центра партнеров для управления сделками в совместных продажах.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="5fdf5-109">Используя соединители совместной работы, вы можете создать новую ссылку для совместной продажи, чтобы привлечь продавца Майкрософт, получать ссылки от продавца Майкрософт, принимать или отклонять ссылки, изменять данные сделки, такие как стоимость сделки и дату закрытия.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="5fdf5-110">Вы также можете получить обновления от Microsoft продавцов для этих сделок совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="5fdf5-111">Все ваши ссылки можно выполнять при работе в CRM по вашему выбору, а не в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="5fdf5-112">Решение основано на решении Microsoft Power Автоматизируing и использует API-интерфейсы центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="5fdf5-113">Перед установкой предварительных требований</span><span class="sxs-lookup"><span data-stu-id="5fdf5-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="5fdf5-114">**Разделы**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-114">**Topics**</span></span>   |<span data-ttu-id="5fdf5-115">**Сведения**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-115">**Details**</span></span>   |<span data-ttu-id="5fdf5-116">**Ссылки**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="5fdf5-117">Идентификатор Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="5fdf5-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="5fdf5-118">Требуется допустимый идентификатор MPN</span><span class="sxs-lookup"><span data-stu-id="5fdf5-118">You need a valid MPN ID</span></span>|<span data-ttu-id="5fdf5-119">Присоединение к [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="5fdf5-120">Готовность к совместной продаже</span><span class="sxs-lookup"><span data-stu-id="5fdf5-120">Co-sell ready</span></span>|<span data-ttu-id="5fdf5-121">Ваше решение для работы с IP-адресами и службами должно быть готово к совместной продаже.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="5fdf5-122">Продажа с Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5fdf5-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="5fdf5-123">Учетная запись Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5fdf5-123">Partner Center account</span></span>|<span data-ttu-id="5fdf5-124">Идентификатор MPN, связанный с клиентом центра партнеров, должен совпадать с ИДЕНТИФИКАТОРом MPN, связанным с решением для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="5fdf5-125">Прежде чем развертывать соединители, убедитесь, что вы видите ссылки на совместные продажи на портале центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="5fdf5-126">Управление учетной записью</span><span class="sxs-lookup"><span data-stu-id="5fdf5-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="5fdf5-127">Роли пользователей Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5fdf5-127">Partner Center user roles</span></span>|<span data-ttu-id="5fdf5-128">Сотрудник, который будет устанавливать и использовать соединители, должен быть администратором ссылок.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="5fdf5-129">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="5fdf5-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="5fdf5-130">SalesForce CRM</span><span class="sxs-lookup"><span data-stu-id="5fdf5-130">Salesforce CRM</span></span>|<span data-ttu-id="5fdf5-131">Роль пользователя CRM — системный администратор или Настройщик системы</span><span class="sxs-lookup"><span data-stu-id="5fdf5-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="5fdf5-132">Назначение ролей в Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="5fdf5-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="5fdf5-133">Учетная запись потока Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="5fdf5-133">Power Automate Flow Account</span></span>|<span data-ttu-id="5fdf5-134">Активная учетная запись [Power автоматизируется](https://flow.microsoft.com) для системного администратора CRM или настройщика системы.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="5fdf5-135">Этот пользователь должен войти в [Power автоматизиру](https://flow.microsoft.com) по крайней мере один раз перед установкой.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="5fdf5-136">Установка пакета salesforce для настраиваемых полей Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5fdf5-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="5fdf5-137">Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, в решении Power автоматизировать необходимо четко определить конкретные поля ссылок Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="5fdf5-138">Эта разделительной предоставляет группам продавцов-партнеров возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="5fdf5-139">В Salesforce активируйте **заметки** и добавьте их в список возможных сделок.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="5fdf5-140">Ссылки</span><span class="sxs-lookup"><span data-stu-id="5fdf5-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="5fdf5-141">Активируйте **группы возможных сделок** , выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="5fdf5-142">В программе установки используйте поле **Быстрый поиск** , чтобы найти параметры группы возможных сделок.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="5fdf5-143">При необходимости задайте необходимые параметры.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-143">Define the settings as needed.</span></span>
[<span data-ttu-id="5fdf5-144">Ссылки</span><span class="sxs-lookup"><span data-stu-id="5fdf5-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="5fdf5-145">В Salesforce установите настраиваемые поля и объекты с помощью установщика пакетов ниже.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="5fdf5-146">Перейдите [сюда](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) , чтобы установить пакет в любую компанию:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="5fdf5-147">Примечание. при установке в песочницу необходимо заменить начальную часть URL-адреса на http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="5fdf5-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="5fdf5-148">В Salesforce добавьте решения Майкрософт в список, связанный с **возможной сделкой** .</span><span class="sxs-lookup"><span data-stu-id="5fdf5-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="5fdf5-149">После добавления щелкните значок **гаечного ключа** и обновите свойства.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="5fdf5-150">Рекомендации: Протестируйте перед переходом в динамический</span><span class="sxs-lookup"><span data-stu-id="5fdf5-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="5fdf5-151">Прежде чем устанавливать, настраивать и настраивать решение Power Автоматизация в рабочей среде, обязательно протестируйте решение на промежуточном экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="5fdf5-152">Установите решение Microsoft Power автоматизируя в промежуточной среде или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="5fdf5-153">Создайте копию решения и запустите настройку потока настройки и автоматизации энергосбережения в промежуточной среде.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="5fdf5-154">Протестируйте решение в промежуточном или экземпляре CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="5fdf5-155">В случае успеха импортируйте в рабочий экземпляр в качестве управляемого решения.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="5fdf5-156">Установка синхронизации ссылок центра партнеров для Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="5fdf5-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="5fdf5-157">Откройте [Power автоматизиру](https://flow.microsoft.com) и выберите **среды** в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="5fdf5-158">Будут показаны доступные экземпляры CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="5fdf5-159">Выберите нужный экземпляр CRM в раскрывающемся списке в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="5fdf5-160">Выберите **решения** на панели навигации слева.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="5fdf5-161">Щелкните ссылку **Open AppSource (открыть** ) в верхнем меню.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Открыть AppSource":::

5. <span data-ttu-id="5fdf5-163">Найдите **соединители центров партнеров для Salesforce** во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="5fdf5-165">Нажмите кнопку **получить сейчас** и **Продолжайте**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="5fdf5-166">Откроется страница, на которой можно выбрать среду CRM salesforce для установки приложения.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="5fdf5-167">Согласиться с условиями.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Доступные КРМС":::

8. <span data-ttu-id="5fdf5-169">Затем вы направляетесь на страницу **Управление решениями** .</span><span class="sxs-lookup"><span data-stu-id="5fdf5-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="5fdf5-170">Перейдите в раздел "ссылки центра партнеров" с помощью кнопок со стрелками в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="5fdf5-171">**Запланированная установка** должна отображаться рядом с решением "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="5fdf5-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="5fdf5-172">Установка займет 10-15 минут.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="5fdf5-173">После завершения установки вернитесь к [Power автоматизиру](https://flow.microsoft.com) и выберите **решения** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="5fdf5-174">Обратите внимание, что **Синхронизация ссылок центра партнеров по Salesforce** доступна в списке решений.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="5fdf5-175">Выберите **ссылку Центр партнеров синхронизация для Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="5fdf5-176">Доступны следующие потоки и сущности Power автоматизировать:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Потоки Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="5fdf5-178">Настройка решения</span><span class="sxs-lookup"><span data-stu-id="5fdf5-178">Configure the solution</span></span>

1. <span data-ttu-id="5fdf5-179">После установки решения в экземпляре CRM вернитесь к [Power автоматизиру](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="5fdf5-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="5fdf5-180">В раскрывающемся списке **среды** в правом верхнем углу выберите экземпляр CRM, в котором было установлено решение Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="5fdf5-181">Вам потребуется создать подключения, связывающие три учетные записи пользователей:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="5fdf5-182">Пользователь центра партнеров с учетными данными администратора ссылок</span><span class="sxs-lookup"><span data-stu-id="5fdf5-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="5fdf5-183">События Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5fdf5-183">Partner Center Events</span></span>
    - <span data-ttu-id="5fdf5-184">Администратор CRM с потоками Power автоматизиру в решении.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="5fdf5-185">В области навигации слева выберите **подключения** и в списке выберите решение "ссылки центра партнеров".</span><span class="sxs-lookup"><span data-stu-id="5fdf5-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="5fdf5-186">Создайте подключение, щелкнув **создать соединение**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Создание подключения":::

- <span data-ttu-id="5fdf5-188">Поиск ссылок центра партнеров (Предварительная версия) в строке поиска в правом верхнем углу.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="5fdf5-189">Создайте подключение для пользователя центра партнеров с ролью учетных данных администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="5fdf5-190">Затем создайте подключение к событиям центра партнеров для пользователя центра партнеров с учетными данными администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="5fdf5-191">Создайте подключение для Common Data Service (текущего окружения) для пользователя администратора CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="5fdf5-192">После добавления всех подключений в вашей среде должны отобразиться следующие подключения:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Наблюдение за подключениями":::

### <a name="edit-the-connections"></a><span data-ttu-id="5fdf5-194">Изменение подключений</span><span class="sxs-lookup"><span data-stu-id="5fdf5-194">Edit the connections</span></span>

1. <span data-ttu-id="5fdf5-195">Вернитесь на страницу решения и выберите **решение по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="5fdf5-196">Выберите **ссылку на подключение (Предварительная версия)** , щелкнув **все**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Начать изменение соединителя":::

2. <span data-ttu-id="5fdf5-198">Измените каждое из подключений одним, щелкнув значок с тремя точками.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="5fdf5-199">Добавьте соответствующие подключения.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Изменение соединителей":::

3. <span data-ttu-id="5fdf5-201">Включите потоки в следующей последовательности:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="5fdf5-202">Регистрация веб-перехватчика центра партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="5fdf5-203">Создание ссылки на совместную продажу — Salesforce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="5fdf5-204">Центр партнеров обновления справочных обновлений в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="5fdf5-205">Центр партнеров в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="5fdf5-206">SalesForce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="5fdf5-207">Возможность Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="5fdf5-208">Решения Майкрософт для Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="5fdf5-209">Использование API веб-перехватчика для регистрации событий изменения ресурсов</span><span class="sxs-lookup"><span data-stu-id="5fdf5-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="5fdf5-210">Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="5fdf5-211">Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="5fdf5-212">Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="5fdf5-213">Добавьте подключения для пользователя центра партнеров (a.) с ссылками на учетные данные администратора (b), как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Триггер":::

3. <span data-ttu-id="5fdf5-215">При выполнении этих обновлений вы увидите</span><span class="sxs-lookup"><span data-stu-id="5fdf5-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Объекты Webhook":::

4. <span data-ttu-id="5fdf5-217">Сохраните изменения и выберите **включить**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="5fdf5-218">Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="5fdf5-219">Выберите **Центр партнеров для SALESFORCE CRM (Предварительная версия)**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="5fdf5-220">Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="5fdf5-221">Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Копирование URL-адреса":::

8. <span data-ttu-id="5fdf5-223">Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="5fdf5-224">Убедитесь, что в правой части окна откроется окно "запуск потока", и нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="5fdf5-225">Введите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-225">Enter the following details:</span></span>

    1. <span data-ttu-id="5fdf5-226">**Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага</span><span class="sxs-lookup"><span data-stu-id="5fdf5-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="5fdf5-227">**Регистрируемые события**: "Создание ссылок" и "обновление ссылок"</span><span class="sxs-lookup"><span data-stu-id="5fdf5-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="5fdf5-228">**Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки).</span><span class="sxs-lookup"><span data-stu-id="5fdf5-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="5fdf5-229">Выберите **выполнить** , а затем нажмите кнопку **Готово.**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="5fdf5-230">Теперь веб-перехватчик может прослушивать события создания и обновления.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="5fdf5-231">Настройка шагов синхронизации</span><span class="sxs-lookup"><span data-stu-id="5fdf5-231">Customize synchronization steps</span></span>

<span data-ttu-id="5fdf5-232">Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="5fdf5-233">Часто системы CRM сильно настроены.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="5fdf5-234">Можно настроить потоки автоматизации Powering.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="5fdf5-235">Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="5fdf5-236">Предоставляются сопоставления центров партнеров Майкрософт с CRM, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="5fdf5-237">В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="5fdf5-238">Ниже приведены примеры доступных настроек.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="5fdf5-239">Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="5fdf5-240">Выберите центр партнеров для Salesforce CRM (Предварительная версия).</span><span class="sxs-lookup"><span data-stu-id="5fdf5-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="5fdf5-241">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="5fdf5-242">Выберите **(область) синхронизация интереса или возможной сделки**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="5fdf5-243">Чтобы настроить сопоставления полей CRM для создания событий, выберите **, если это новая доступная возможность, а затем**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="5fdf5-244">Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="5fdf5-245">Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="5fdf5-246">Чтобы настроить сопоставления полей CRM для событий обновления, щелкните шаг "(область) синхронизация интереса или возможности".</span><span class="sxs-lookup"><span data-stu-id="5fdf5-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="5fdf5-247">Выберите **, если это обновление возможной сделки, а затем**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="5fdf5-248">Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="5fdf5-249">Выберите, **Если да** , а затем **обновить существующую возможную сделку**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="5fdf5-250">Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="5fdf5-251">Выберите **изменить**  , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="5fdf5-252">Выберите **(область) синхронизировать возможную сделку**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="5fdf5-253">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, установите флажок, **Если между ведущими объектами в центре партнеров и CRM есть различия**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="5fdf5-254">Выберите подшаг, **Если да** , а затем разверните этот шаг, чтобы **Обновить ссылку на данные о возможностях**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="5fdf5-255">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="5fdf5-256">Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?</span><span class="sxs-lookup"><span data-stu-id="5fdf5-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="5fdf5-257">Выберите **изменить**  , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="5fdf5-258">Выберите **(область) синхронизация ссылок.**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="5fdf5-259">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="5fdf5-260">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="5fdf5-261">Настройка полей и связей</span><span class="sxs-lookup"><span data-stu-id="5fdf5-261">Set up fields and relationships</span></span>

1. <span data-ttu-id="5fdf5-262">Войдите в учетную запись Salesforce и перейдите к **возможности**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-262">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="5fdf5-263">Щелкните Параметры **установки** и **изменения объекта** , чтобы добавить необходимые поля.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-263">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="5fdf5-264">Выбор **полей & связей** в левой области навигации</span><span class="sxs-lookup"><span data-stu-id="5fdf5-264">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. <span data-ttu-id="5fdf5-266">Добавьте в **поля & таблицу связей** следующие поля:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-266">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="5fdf5-267">**Метка поля**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-267">**Field label**</span></span>   |<span data-ttu-id="5fdf5-268">**Имя поля**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-268">**Field name**</span></span>|<span data-ttu-id="5fdf5-269">**Data type**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-269">**Data type**</span></span>|<span data-ttu-id="5fdf5-270">**Индексированного**</span><span class="sxs-lookup"><span data-stu-id="5fdf5-270">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="5fdf5-271">Аудит</span><span class="sxs-lookup"><span data-stu-id="5fdf5-271">Audit</span></span>| <span data-ttu-id="5fdf5-272">Audit__c</span><span class="sxs-lookup"><span data-stu-id="5fdf5-272">Audit__c</span></span>|<span data-ttu-id="5fdf5-273">Длинная текстовая область (100000) (видимая строка 4)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-273">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="5fdf5-274">Как можно получить справку Майкрософт?</span><span class="sxs-lookup"><span data-stu-id="5fdf5-274">How can Microsoft help?</span></span>|<span data-ttu-id="5fdf5-275">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="5fdf5-275">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="5fdf5-276">Поля выбора</span><span class="sxs-lookup"><span data-stu-id="5fdf5-276">Picklist\*</span></span>|
   |<span data-ttu-id="5fdf5-277">Продукты</span><span class="sxs-lookup"><span data-stu-id="5fdf5-277">Products</span></span>|<span data-ttu-id="5fdf5-278">Products_c</span><span class="sxs-lookup"><span data-stu-id="5fdf5-278">Products_c</span></span>|<span data-ttu-id="5fdf5-279">текст (255)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-279">text (255)</span></span>||
   |<span data-ttu-id="5fdf5-280">Referral</span><span class="sxs-lookup"><span data-stu-id="5fdf5-280">Referral</span></span> | <span data-ttu-id="5fdf5-281">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="5fdf5-281">Referral_Identfier_c</span></span>|<span data-ttu-id="5fdf5-282">Текст (100) (внешний идентификатор)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-282">Text(100)(External ID)</span></span>|<span data-ttu-id="5fdf5-283">да</span><span class="sxs-lookup"><span data-stu-id="5fdf5-283">yes</span></span>|
   |<span data-ttu-id="5fdf5-284">Ссылка на ссылку</span><span class="sxs-lookup"><span data-stu-id="5fdf5-284">Referral Link</span></span>| <span data-ttu-id="5fdf5-285">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="5fdf5-285">Referral_Link_c_</span></span>|<span data-ttu-id="5fdf5-286">URL-АДРЕС (255)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-286">URL(255)</span></span>||
   |<span data-ttu-id="5fdf5-287">Синхронизация с центром партнеров</span><span class="sxs-lookup"><span data-stu-id="5fdf5-287">Sync with Partner Center</span></span>|<span data-ttu-id="5fdf5-288">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="5fdf5-288">sync_with_partner_center_c</span></span>|<span data-ttu-id="5fdf5-289">Флажок (значение по умолчанию снято)</span><span class="sxs-lookup"><span data-stu-id="5fdf5-289">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="5fdf5-290">\* Значения поля выбора:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-290">\*Picklist values:</span></span>

   - <span data-ttu-id="5fdf5-291">Зависящее от рабочей нагрузки предложение ценности</span><span class="sxs-lookup"><span data-stu-id="5fdf5-291">Workload specific value proposition</span></span>
   - <span data-ttu-id="5fdf5-292">Техническая архитектура клиента</span><span class="sxs-lookup"><span data-stu-id="5fdf5-292">Customer technical architecture</span></span>
   - <span data-ttu-id="5fdf5-293">Подтверждение концепции или демонстрационной версии</span><span class="sxs-lookup"><span data-stu-id="5fdf5-293">Proof of concept or demo</span></span>
   - <span data-ttu-id="5fdf5-294">Кавычки или лицензирование</span><span class="sxs-lookup"><span data-stu-id="5fdf5-294">Quotes or licensing</span></span>
   - <span data-ttu-id="5fdf5-295">Опубликовать успешные продажи клиента</span><span class="sxs-lookup"><span data-stu-id="5fdf5-295">Post sales customer success</span></span>
   - <span data-ttu-id="5fdf5-296">Общие или другие</span><span class="sxs-lookup"><span data-stu-id="5fdf5-296">General or other</span></span>

5. <span data-ttu-id="5fdf5-297">Поля будут созданы в разделе **поля & связи** .</span><span class="sxs-lookup"><span data-stu-id="5fdf5-297">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Созданные поля":::

6. <span data-ttu-id="5fdf5-299">В макете возможности создайте отдельный раздел с полями, как показано выше.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-299">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="5fdf5-300">Этот раздел должен быть доступен для продавцов в макете возможности.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-300">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Макет полей центра партнеров":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="5fdf5-302">Сквозная синхронизация двунаправленной совместной продажи</span><span class="sxs-lookup"><span data-stu-id="5fdf5-302">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="5fdf5-303">После установки, настройки и настройки решения Power автоматизиру вы можете протестировать синхронизацию ссылок для совместной продажи между Salesforce CRM и центром партнеров.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-303">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="5fdf5-304">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5fdf5-304">Pre-requisites</span></span>

<span data-ttu-id="5fdf5-305">Чтобы синхронизировать ссылки в центре партнеров и Salesforce CRM, решение Power автоматизирует необходимость четко разграничения ссылочные поля Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-305">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="5fdf5-306">Эта идентификация предоставляет группам продавцов возможность решать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-306">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="5fdf5-307">Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможности** решения Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-307">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="5fdf5-308">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="5fdf5-308">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="5fdf5-309">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-309">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="5fdf5-310">**Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5fdf5-310">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="5fdf5-311">**Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5fdf5-311">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="5fdf5-312">**Ссылка на ссылку: ссылка**только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5fdf5-312">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="5fdf5-313">**Как можно**получить помощь от корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-313">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="5fdf5-314">**Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="5fdf5-314">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="5fdf5-315">**Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5fdf5-315">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="5fdf5-316">ВАРИАНТ</span><span class="sxs-lookup"><span data-stu-id="5fdf5-316">SCENARIOS:</span></span>

1. <span data-ttu-id="5fdf5-317">Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-317">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="5fdf5-318">Войдите в среду Salesforce CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-318">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="5fdf5-319">При создании "новой возможности" в среде Salesforce CRM убедитесь, что следующий раздел существует.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-319">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Среда Salesforce":::

   3. <span data-ttu-id="5fdf5-321">Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-321">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="5fdf5-322">"Синхронизация с центром партнеров": Да</span><span class="sxs-lookup"><span data-stu-id="5fdf5-322">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="5fdf5-323">«Как можно получить справку Майкрософт?»: выберите следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-323">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="5fdf5-324">Продукты: идентификаторы решений для продукта</span><span class="sxs-lookup"><span data-stu-id="5fdf5-324">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="5fdf5-325">Установив для параметра синхронизация возможных сделок  **с центром партнеров** значение **Да**, подождите 10 минут, войдите в свою учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-325">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="5fdf5-326">Ваши ссылки будут синхронизированы с Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-326">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="5fdf5-327">Если параметр "синхронизировать с центром партнеров" имеет значение "Да", то при обновлении возможной сделки в Salesforce CRM изменения будут синхронизироваться с учетной записью центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-327">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="5fdf5-328">Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-328">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="5fdf5-329">Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="5fdf5-329">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="5fdf5-330">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-330">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="5fdf5-331">В меню слева выберите **ссылки** .</span><span class="sxs-lookup"><span data-stu-id="5fdf5-331">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="5fdf5-332">Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".</span><span class="sxs-lookup"><span data-stu-id="5fdf5-332">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="5fdf5-333">Войдите в среду Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-333">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="5fdf5-334">Перейдите к разделу **открытые возможности**.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-334">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="5fdf5-335">Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-335">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Экран возможностей Salesforce":::

    6. <span data-ttu-id="5fdf5-337">При выборе синхронизированной ссылки сведения о представлении карточки заполняются.</span><span class="sxs-lookup"><span data-stu-id="5fdf5-337">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5fdf5-338">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5fdf5-338">Next steps</span></span>

- [<span data-ttu-id="5fdf5-339">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="5fdf5-339">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="5fdf5-340">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="5fdf5-340">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="5fdf5-341">Веб-перехватчики Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="5fdf5-341">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)