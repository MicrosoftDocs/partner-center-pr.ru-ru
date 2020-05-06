---
title: Настройка встроенного интерфейса устройства с помощью профилей Windows "Автопилот" | Центр партнеров
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Сведения о настройке и предварительной настройке нового интерфейса устройства с профилями для автопилота перед доставкой устройства клиенту.
author: LauraBrenner
ms.author: labrenne
keywords: Автопилот, Windows автопилот, Microsoft для автопилота, развертывание без вмешательства пользователя, OOBE, экраны входа, готовые
ms.localizationpriority: medium
ms.openlocfilehash: 7fed49f9fd06be8765e3435862e3bee48b717ce7
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798612"
---
# <a name="customize-the-out-of-box-experience-for-a-device-with-windows-autopilot-profiles"></a><span data-ttu-id="be392-104">Настройка готового интерфейса для устройства с профилями Windows "Автопилот"</span><span class="sxs-lookup"><span data-stu-id="be392-104">Customize the out-of-box experience for a device with Windows Autopilot profiles</span></span>

<span data-ttu-id="be392-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="be392-105">**Applies to**</span></span>

- <span data-ttu-id="be392-106">Партнеры с прямым выставлением счетов, косвенные поставщики и непрямые торговые посредники</span><span class="sxs-lookup"><span data-stu-id="be392-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="be392-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="be392-107">**Appropriate roles**</span></span>

- <span data-ttu-id="be392-108">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="be392-108">Admin agent</span></span>
- <span data-ttu-id="be392-109">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="be392-109">Global admin</span></span>
- <span data-ttu-id="be392-110">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="be392-110">Sales agent</span></span>
- <span data-ttu-id="be392-111">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="be392-111">User management admin</span></span>

<span data-ttu-id="be392-112">Если вы управляете клиентскими устройствами, может потребоваться настроить предварительный запуск (OOBE) для пользователей клиента.</span><span class="sxs-lookup"><span data-stu-id="be392-112">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="be392-113">Вы можете предварительно настроить новые устройства с помощью профилей Windows "Автопилот", прежде чем доставлять устройства клиентам и применять новые профили к устройствам, которые клиенты уже приобрели.</span><span class="sxs-lookup"><span data-stu-id="be392-113">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="be392-114">Обратите внимание, что изготовители оборудования начали включать метку доставки за пределы поля устройства автопилота, которое показывает **идентификатор ключа продукта (пкид)** устройства.</span><span class="sxs-lookup"><span data-stu-id="be392-114">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="be392-115">Этот одномерный доступный для чтения штрих-код предоставляет подчиненным партнерам способ регистрации устройств для автопилота без распаковки устройств и сбора идентификатора устройства с помощью альтернативных средств.</span><span class="sxs-lookup"><span data-stu-id="be392-115">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="be392-116">В этой статье объясняется, как создавать и применять профили автопилота к устройствам в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="be392-116">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="be392-117">Если вы еще не знакомы с автопилотом, ознакомьтесь со сведениями в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="be392-117">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="be392-118">Общие сведения об автопилоте Windows</span><span class="sxs-lookup"><span data-stu-id="be392-118">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="be392-119">Справочное руководство по развертыванию по для автопилота</span><span class="sxs-lookup"><span data-stu-id="be392-119">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="be392-120">Обзор</span><span class="sxs-lookup"><span data-stu-id="be392-120">Overview</span></span>

<span data-ttu-id="be392-121">Функция автопилота Windows в центре партнеров позволяет создавать пользовательские профили для применения к устройствам клиентов.</span><span class="sxs-lookup"><span data-stu-id="be392-121">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="be392-122">На момент публикации этой статьи были доступны следующие параметры профиля:</span><span class="sxs-lookup"><span data-stu-id="be392-122">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="be392-123">Пропустить параметры конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="be392-123">Skip privacy settings.</span></span> <span data-ttu-id="be392-124">Этот необязательный параметр профиля автопилота позволяет организациям не запрашивать сведения о параметрах конфиденциальности во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="be392-124">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="be392-125">Отключить создание учетной записи локального администратора на устройстве.</span><span class="sxs-lookup"><span data-stu-id="be392-125">Disable local admin account creation on the device.</span></span> <span data-ttu-id="be392-126">Организации могут определить, должен ли пользователь настроить устройство для доступа администратора после завершения процесса.</span><span class="sxs-lookup"><span data-stu-id="be392-126">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="be392-127">Автоматически настроить устройство для работы или учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="be392-127">Automatically set up device for work or school.</span></span> <span data-ttu-id="be392-128">Все устройства, зарегистрированные с помощью автопилота, будут автоматически считаться рабочими или учебными устройствами, поэтому этот вопрос не будет запрашиваться во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="be392-128">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="be392-129">Пропускать страницы настройки регистрации Кортаны, OneDrive и OEM.</span><span class="sxs-lookup"><span data-stu-id="be392-129">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="be392-130">Все устройства, зарегистрированные с помощью автопилота, автоматически пропускают эти страницы во время готового процесса (OOBE).</span><span class="sxs-lookup"><span data-stu-id="be392-130">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="be392-131">Пропустить лицензионное соглашение (EULA).</span><span class="sxs-lookup"><span data-stu-id="be392-131">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="be392-132">Начиная с Windows 10 версии 1709, организации могут решить пропустить страницу лицензионного соглашения, представленную в процессе OOBE.</span><span class="sxs-lookup"><span data-stu-id="be392-132">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="be392-133">Важные сведения о пропуске страницы лицензионного соглашения во время установки Windows см. в статье об [отклонении лицензионного соглашения Windows для автопилота](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="be392-133">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="be392-134">Применяются следующие разрешения и ограничения на управление профилями и устройствами.</span><span class="sxs-lookup"><span data-stu-id="be392-134">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="be392-135">Партнеры CSP могут продолжать управлять профилями автопилота для существующих клиентов, которым назначены связи через торгового посредника, даже если клиенты удалили права делегированного администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="be392-135">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="be392-136">Вы можете управлять существующими устройствами для добавленных клиентов.</span><span class="sxs-lookup"><span data-stu-id="be392-136">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="be392-137">Вы не можете управлять устройствами, отправленными клиентом в Microsoft Store для бизнеса или на портале Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="be392-137">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="be392-138">Создание профилей автопилотного развертывания и управление ими в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="be392-138">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="be392-139">В центре партнеров можно создать профили развертывания Windows для автопилота и применить их к устройствам.</span><span class="sxs-lookup"><span data-stu-id="be392-139">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="be392-140">Только агенты администрирования могут создавать и применять профили.</span><span class="sxs-lookup"><span data-stu-id="be392-140">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="be392-141">Создать новый профиль для автопилота</span><span class="sxs-lookup"><span data-stu-id="be392-141">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="be392-142">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, для которого создается профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="be392-142">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="be392-143">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="be392-143">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="be392-144">В разделе **профили Windows для автопилота** выберите **Добавить новый профиль**.</span><span class="sxs-lookup"><span data-stu-id="be392-144">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="be392-145">Введите имя и описание профиля, а затем настройте параметры OOBE.</span><span class="sxs-lookup"><span data-stu-id="be392-145">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="be392-146">Выберите один из следующих типов.</span><span class="sxs-lookup"><span data-stu-id="be392-146">Choose from:</span></span>  

   - <span data-ttu-id="be392-147">Пропустить параметры конфиденциальности в программе установки</span><span class="sxs-lookup"><span data-stu-id="be392-147">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="be392-148">Отключение учетной записи локального администратора при настройке</span><span class="sxs-lookup"><span data-stu-id="be392-148">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="be392-149">Автоматический пропуск страниц при настройке</span><span class="sxs-lookup"><span data-stu-id="be392-149">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="be392-150">(В том числе *автоматически выберите Настройка для рабочей или учебной* программы и *пропустите страницы настройки регистрации кортаны, OneDrive и OEM*).</span><span class="sxs-lookup"><span data-stu-id="be392-150">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="be392-151">Пропустить лицензионное соглашение с конечным пользователем (EULA)</span><span class="sxs-lookup"><span data-stu-id="be392-151">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="be392-152">Важные сведения о пропуске страницы лицензионного соглашения во время установки Windows см. в статье об [отклонении лицензионного соглашения Windows для автопилота](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="be392-152">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="be392-153">По завершении нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="be392-153">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="be392-154">Применение профиля автопилота для клиентских устройств</span><span class="sxs-lookup"><span data-stu-id="be392-154">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="be392-155">В приведенных ниже инструкциях предполагается, что вы уже добавили устройства клиента в центр партнеров и можете получить доступ к списку устройств.</span><span class="sxs-lookup"><span data-stu-id="be392-155">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="be392-156">Если вы еще не добавили устройства клиента, следуйте инструкциям в разделе [Добавление устройств в учетную запись клиента](#add-devices-to-a-customers-account) , а затем выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="be392-156">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="be392-157">После создания профиля автопилота для клиента его можно применить к устройствам клиента.</span><span class="sxs-lookup"><span data-stu-id="be392-157">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="be392-158">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, для которого был создан профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="be392-158">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="be392-159">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="be392-159">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="be392-160">В разделе **применить профили к устройствам** выберите устройства или группы устройств, в которые необходимо добавить профили, а затем нажмите кнопку **Применить профиль**.</span><span class="sxs-lookup"><span data-stu-id="be392-160">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="be392-161">Только что примененный профиль появится в столбце **профиль** .</span><span class="sxs-lookup"><span data-stu-id="be392-161">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="be392-162">Выполните следующие действия, чтобы убедиться, что профиль будет успешно применен к устройству.</span><span class="sxs-lookup"><span data-stu-id="be392-162">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="be392-163">a.</span><span class="sxs-lookup"><span data-stu-id="be392-163">a.</span></span>  <span data-ttu-id="be392-164">Подключите устройство к сети и включите его.</span><span class="sxs-lookup"><span data-stu-id="be392-164">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="be392-165">b.</span><span class="sxs-lookup"><span data-stu-id="be392-165">b.</span></span>  <span data-ttu-id="be392-166">Убедитесь, что отображаются соответствующие экраны OOBE (если они должны отображаться).</span><span class="sxs-lookup"><span data-stu-id="be392-166">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="be392-167">c.</span><span class="sxs-lookup"><span data-stu-id="be392-167">c.</span></span>  <span data-ttu-id="be392-168">Когда процесс OOBE останавливается, верните устройство к заводским параметрам по умолчанию, чтобы подготовить его для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="be392-168">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="be392-169">Удаление профиля автопилота с устройства клиента</span><span class="sxs-lookup"><span data-stu-id="be392-169">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="be392-170">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, для которого был создан профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="be392-170">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="be392-171">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="be392-171">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="be392-172">В разделе **применить профили к устройствам** выберите устройства, из которых нужно удалить профиль, а затем щелкните **удалить профиль**.</span><span class="sxs-lookup"><span data-stu-id="be392-172">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="be392-173">Удаление профиля с устройства не приводит к удалению профиля из списка.</span><span class="sxs-lookup"><span data-stu-id="be392-173">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="be392-174">Если вы хотите удалить профиль, следуйте инструкциям в разделе [обновление или удаление профиля автопилота](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="be392-174">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="be392-175">Обновление или удаление профиля автопилота</span><span class="sxs-lookup"><span data-stu-id="be392-175">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="be392-176">Если клиент хочет изменить готовый интерфейс после отправки им устройств, можно изменить профиль в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="be392-176">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="be392-177">Когда устройство клиента подключается к Интернету, оно скачивает последнюю версию профиля во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="be392-177">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="be392-178">Кроме того, каждый раз, когда клиент восстанавливает заводские параметры по умолчанию, устройство снова загрузит последнюю версию профиля во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="be392-178">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="be392-179">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, желающего изменить профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="be392-179">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="be392-180">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="be392-180">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="be392-181">В разделе **профили Windows для автопилота** выберите профиль, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="be392-181">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="be392-182">Внесите необходимые изменения и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="be392-182">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="be392-183">Чтобы удалить этот профиль, выберите **удалить профиль** в правом верхнем углу страницы.</span><span class="sxs-lookup"><span data-stu-id="be392-183">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="be392-184">Добавление устройств в учетную запись клиента</span><span class="sxs-lookup"><span data-stu-id="be392-184">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="be392-185">Агенты продаж и администраторы могут добавлять устройства в учетную запись клиента.</span><span class="sxs-lookup"><span data-stu-id="be392-185">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="be392-186">Перед применением пользовательских профилей для автопилота к устройствам клиентов необходимо иметь возможность доступа к списку устройств клиента.</span><span class="sxs-lookup"><span data-stu-id="be392-186">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="be392-187">Если вы планируете использовать имя изготовителя оборудования, серийный номер и модель, учитывайте следующие ограничения.</span><span class="sxs-lookup"><span data-stu-id="be392-187">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="be392-188">Этот кортеж работает только для новых устройств (например, 4 КБ) и не поддерживается для хэшей 128B (RS2 и предыдущих устройств).</span><span class="sxs-lookup"><span data-stu-id="be392-188">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="be392-189">При регистрации кортежа учитывается регистр, поэтому данные в файле должны совпадать с именами модели и производителя ***точно*** так же, как это обеспечивает поставщик OEM (поставщик оборудования).</span><span class="sxs-lookup"><span data-stu-id="be392-189">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="be392-190">Следуйте приведенным ниже инструкциям, чтобы добавить устройства в учетную запись клиента в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="be392-190">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="be392-191">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, устройства которого требуется управлять.</span><span class="sxs-lookup"><span data-stu-id="be392-191">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="be392-192">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="be392-192">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="be392-193">В разделе **применить профили к устройствам** выберите **Добавить устройства**.</span><span class="sxs-lookup"><span data-stu-id="be392-193">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="be392-194">Введите имя для списка устройств и нажмите кнопку **Обзор** , чтобы отправить список клиента (в формате CSV-файла) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="be392-194">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="be392-195">Вы должны получить этот CSV-файл с покупкой устройства.</span><span class="sxs-lookup"><span data-stu-id="be392-195">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="be392-196">Если вы не получили CSV-файл, вы можете создать его самостоятельно, выполнив действия, описанные в разделе [Добавление устройств в Windows автопилот](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="be392-196">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="be392-197">Отправьте CSV-файл и нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="be392-197">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="be392-198">Если при попытке отправить CSV-файл появляется сообщение об ошибке, проверьте формат файла.</span><span class="sxs-lookup"><span data-stu-id="be392-198">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="be392-199">Можно использовать только хэш оборудования или имя изготовителя оборудования, серийный номер и модель (в этом порядке столбцов) или идентификатор продукта Windows.</span><span class="sxs-lookup"><span data-stu-id="be392-199">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="be392-200">Вы также можете использовать файл Sample. csv, приведенный по ссылке далее, чтобы **Добавить устройства** для создания списка устройств.</span><span class="sxs-lookup"><span data-stu-id="be392-200">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="be392-201">CSV-файл должен выглядеть примерно так:</span><span class="sxs-lookup"><span data-stu-id="be392-201">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="be392-202">**Серийный номер устройства, идентификатор продукта Windows, хэш оборудования, имя производителя, модель устройства**</span><span class="sxs-lookup"><span data-stu-id="be392-202">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="be392-203">**{serialNumber},,, корпорация Майкрософт, портативный компьютер**</span><span class="sxs-lookup"><span data-stu-id="be392-203">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

<span data-ttu-id="be392-204">Обратите внимание, что "имя производителя" и "модель устройства" учитывают регистр.</span><span class="sxs-lookup"><span data-stu-id="be392-204">Note that "Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="be392-205">Если вы не узнаете, какое значение следует указать для имени производителя и модели устройства, можно запустить его на устройстве, чтобы собрать правильные значения:</span><span class="sxs-lookup"><span data-stu-id="be392-205">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="be392-206">Закрытие лицензионного соглашения Windows для автопилота</span><span class="sxs-lookup"><span data-stu-id="be392-206">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="be392-207">ВАЖНАЯ ИНФОРМАЦИЯ</span><span class="sxs-lookup"><span data-stu-id="be392-207">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="be392-208">Windows автопилот позволяет настраивать настроенные установки Windows на устройствах, которыми вы управляете для клиентов.</span><span class="sxs-lookup"><span data-stu-id="be392-208">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="be392-209">Если это разрешено клиентом, вы можете подавлять или скрывать определенные экраны настройки, которые обычно предоставляются пользователям при настройке Windows, включая экран подтверждения лицензионного соглашения (лицензионное соглашение).</span><span class="sxs-lookup"><span data-stu-id="be392-209">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="be392-210">С помощью этой функции вы соглашаетесь, что подавление или скрытие экранов, предназначенных для предоставления пользователям уведомления или принятия условий, означает, что вы получили достаточное согласие и авторизацию от клиента, чтобы скрыть термины, а также от имени клиента (будь то Организация или отдельный пользователь), согласие на любые уведомления и принимать любые условия, применимые к клиенту.</span><span class="sxs-lookup"><span data-stu-id="be392-210">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="be392-211">Это включает согласие с условиями лицензии или уведомления, которое отображалось бы для пользователя, если не бы вы не отключили или не скрыли его с помощью этого средства.</span><span class="sxs-lookup"><span data-stu-id="be392-211">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="be392-212">Ваш клиент не может использовать программное обеспечение Windows на этих устройствах, если ваш клиент не приобрел законным способом лицензию на программное обеспечение у Майкрософт или лицензированных дистрибьюторов.</span><span class="sxs-lookup"><span data-stu-id="be392-212">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
