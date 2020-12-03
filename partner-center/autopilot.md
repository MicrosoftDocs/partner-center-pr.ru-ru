---
title: Настройка встроенного интерфейса устройства
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Прежде чем приступать к новому устройству клиента, можно использовать профили Windows для автопилота, чтобы настроить или предварительно настроить внешний интерфейс устройства (OOBE).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96535001"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="cbe4f-103">Использование профилей Windows Autopilot на новых устройствах для настройки готового интерфейса клиента</span><span class="sxs-lookup"><span data-stu-id="cbe4f-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="cbe4f-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="cbe4f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="cbe4f-105">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="cbe4f-105">Admin agent</span></span>
- <span data-ttu-id="cbe4f-106">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="cbe4f-106">Global admin</span></span>
- <span data-ttu-id="cbe4f-107">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="cbe4f-107">Sales agent</span></span>
- <span data-ttu-id="cbe4f-108">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="cbe4f-108">User management admin</span></span>

<span data-ttu-id="cbe4f-109">Если вы управляете клиентскими устройствами, может потребоваться настроить предварительный запуск (OOBE) для пользователей клиента.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="cbe4f-110">Вы можете предварительно настроить новые устройства с помощью профилей Windows "Автопилот", прежде чем доставлять устройства клиентам и применять новые профили к устройствам, которые клиенты уже приобрели.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="cbe4f-111">Обратите внимание, что изготовители оборудования начали включать метку доставки за пределы поля устройства автопилота, которое показывает **идентификатор ключа продукта (пкид)** устройства.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="cbe4f-112">Этот одномерный доступный для чтения штрих-код предоставляет подчиненным партнерам способ регистрации устройств для автопилота без распаковки устройств и сбора идентификатора устройства с помощью альтернативных средств.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="cbe4f-113">В этой статье объясняется, как создавать и применять профили автопилота к устройствам в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="cbe4f-114">Если вы еще не знакомы с автопилотом, ознакомьтесь со сведениями в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="cbe4f-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="cbe4f-115">Обзор Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="cbe4f-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="cbe4f-116">Справочное руководство по развертыванию по для автопилота</span><span class="sxs-lookup"><span data-stu-id="cbe4f-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="cbe4f-117">Обзор</span><span class="sxs-lookup"><span data-stu-id="cbe4f-117">Overview</span></span>

<span data-ttu-id="cbe4f-118">Функция автопилота Windows в центре партнеров позволяет создавать пользовательские профили для применения к устройствам клиентов.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="cbe4f-119">На момент публикации этой статьи были доступны следующие параметры профиля:</span><span class="sxs-lookup"><span data-stu-id="cbe4f-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="cbe4f-120">Пропустить параметры конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-120">Skip privacy settings.</span></span> <span data-ttu-id="cbe4f-121">Этот необязательный параметр профиля автопилота позволяет организациям не запрашивать сведения о параметрах конфиденциальности во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="cbe4f-122">Отключить создание учетной записи локального администратора на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="cbe4f-123">Организации могут определить, должен ли пользователь настроить устройство для доступа администратора после завершения процесса.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="cbe4f-124">Автоматически настроить устройство для работы или учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="cbe4f-125">Все устройства, зарегистрированные с помощью автопилота, будут автоматически считаться рабочими или учебными устройствами, поэтому этот вопрос не будет запрашиваться во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="cbe4f-126">Пропускать страницы настройки регистрации Кортаны, OneDrive и OEM.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="cbe4f-127">Все устройства, зарегистрированные с помощью автопилота, автоматически пропускают эти страницы во время готового процесса (OOBE).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="cbe4f-128">Пропустить лицензионное соглашение (EULA).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="cbe4f-129">Начиная с Windows 10 версии 1709, организации могут решить пропустить страницу лицензионного соглашения, представленную в процессе OOBE.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="cbe4f-130">Важные сведения о пропуске страницы лицензионного соглашения во время установки Windows см. в статье об [отклонении лицензионного соглашения Windows для автопилота](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="cbe4f-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="cbe4f-131">Применяются следующие разрешения и ограничения на управление профилями и устройствами:</span><span class="sxs-lookup"><span data-stu-id="cbe4f-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="cbe4f-132">Партнеры CSP могут продолжать управлять профилями Autopilot для существующих клиентов, с которыми установлены торговые отношения, даже если клиенты удалили делегированные административные привилегии партнера.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="cbe4f-133">Вы можете управлять существующими устройствами для добавленных клиентов.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="cbe4f-134">Вы не можете управлять устройствами, которые клиент отправил в Microsoft Store для бизнеса или на портал Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="cbe4f-135">Создание профилей автопилотного развертывания и управление ими в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="cbe4f-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="cbe4f-136">В центре партнеров можно создать профили развертывания Windows для автопилота и применить их к устройствам.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="cbe4f-137">Только агенты администрирования могут создавать и применять профили.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="cbe4f-138">Создать новый профиль для автопилота</span><span class="sxs-lookup"><span data-stu-id="cbe4f-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="cbe4f-139">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, для которого создается профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="cbe4f-140">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cbe4f-141">В разделе **профили Windows для автопилота** выберите **Добавить новый профиль**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="cbe4f-142">Введите имя и описание профиля, а затем настройте параметры OOBE.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="cbe4f-143">Выберите один из следующих типов.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-143">Choose from:</span></span>  

   - <span data-ttu-id="cbe4f-144">Пропустить параметры конфиденциальности в программе установки</span><span class="sxs-lookup"><span data-stu-id="cbe4f-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="cbe4f-145">Отключение учетной записи локального администратора при настройке</span><span class="sxs-lookup"><span data-stu-id="cbe4f-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="cbe4f-146">Автоматический пропуск страниц при настройке</span><span class="sxs-lookup"><span data-stu-id="cbe4f-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="cbe4f-147">(В том числе *автоматически выберите Настройка для рабочей или учебной* программы и *пропустите страницы настройки регистрации кортаны, OneDrive и OEM*).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="cbe4f-148">Пропустить лицензионное соглашение с конечным пользователем (EULA)</span><span class="sxs-lookup"><span data-stu-id="cbe4f-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="cbe4f-149">Важные сведения о пропуске страницы лицензионного соглашения во время установки Windows см. в статье об [отклонении лицензионного соглашения Windows для автопилота](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="cbe4f-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="cbe4f-150">По завершении нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="cbe4f-151">Применение профиля автопилота для клиентских устройств</span><span class="sxs-lookup"><span data-stu-id="cbe4f-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="cbe4f-152">В приведенных ниже инструкциях предполагается, что вы уже добавили устройства клиента в центр партнеров и можете получить доступ к списку устройств.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="cbe4f-153">Если вы еще не добавили устройства клиента, следуйте инструкциям в разделе [Добавление устройств в учетную запись клиента](#add-devices-to-a-customers-account) , а затем выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="cbe4f-154">После создания профиля автопилота для клиента его можно применить к устройствам клиента.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="cbe4f-155">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, для которого был создан профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="cbe4f-156">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cbe4f-157">В разделе **применить профили к устройствам** выберите устройства или группы устройств, в которые необходимо добавить профили, а затем нажмите кнопку **Применить профиль**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="cbe4f-158">Только что примененный профиль появится в столбце **профиль** .</span><span class="sxs-lookup"><span data-stu-id="cbe4f-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="cbe4f-159">Выполните следующие действия, чтобы убедиться, что профиль будет успешно применен к устройству.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="cbe4f-160">а.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-160">a.</span></span>  <span data-ttu-id="cbe4f-161">Подключите устройство к сети и включите его.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="cbe4f-162">b.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-162">b.</span></span>  <span data-ttu-id="cbe4f-163">Убедитесь, что отображаются соответствующие экраны OOBE (если они должны отображаться).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="cbe4f-164">c.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-164">c.</span></span>  <span data-ttu-id="cbe4f-165">Когда процесс OOBE останавливается, верните устройство к заводским параметрам по умолчанию, чтобы подготовить его для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="cbe4f-166">Удаление профиля автопилота с устройства клиента</span><span class="sxs-lookup"><span data-stu-id="cbe4f-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="cbe4f-167">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, для которого был создан профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="cbe4f-168">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cbe4f-169">В разделе **применить профили к устройствам** выберите устройства, из которых нужно удалить профиль, а затем щелкните **удалить профиль**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="cbe4f-170">Удаление профиля с устройства не приводит к удалению профиля из списка.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="cbe4f-171">Если вы хотите удалить профиль, следуйте инструкциям в разделе [обновление или удаление профиля автопилота](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="cbe4f-172">Обновление или удаление профиля автопилота</span><span class="sxs-lookup"><span data-stu-id="cbe4f-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="cbe4f-173">Если клиент хочет изменить готовый интерфейс после отправки им устройств, можно изменить профиль в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="cbe4f-174">Когда устройство клиента подключается к Интернету, оно скачивает последнюю версию профиля во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="cbe4f-175">Кроме того, каждый раз, когда клиент восстанавливает заводские параметры по умолчанию, устройство снова загрузит последнюю версию профиля во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="cbe4f-176">В меню Центр партнеров выберите **Клиенты** , а затем выберите клиента, желающего изменить профиль автопилота.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="cbe4f-177">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cbe4f-178">В разделе **профили Windows для автопилота** выберите профиль, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="cbe4f-179">Внесите необходимые изменения и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="cbe4f-180">Чтобы удалить этот профиль, выберите **удалить профиль** в правом верхнем углу страницы.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="cbe4f-181">Добавление устройств в учетную запись клиента</span><span class="sxs-lookup"><span data-stu-id="cbe4f-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="cbe4f-182">Агенты продаж и администраторы могут добавлять устройства в учетную запись клиента.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="cbe4f-183">Перед применением пользовательских профилей для автопилота к устройствам клиентов необходимо иметь возможность доступа к списку устройств клиента.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="cbe4f-184">Если вы планируете использовать имя изготовителя оборудования, серийный номер и модель, учитывайте следующие ограничения.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="cbe4f-185">Этот кортеж работает только для новых устройств (например, 4 КБ) и не поддерживается для хэшей 128B (RS2 и предыдущих устройств).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="cbe4f-186">При регистрации кортежа учитывается регистр, поэтому данные в файле должны совпадать с именами модели и производителя \**_точно так_* же, как указано поставщиком OEM (поставщик оборудования).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="cbe4f-187">Следуйте приведенным ниже инструкциям, чтобы добавить устройства в учетную запись клиента в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="cbe4f-188">Выберите _ *Customers*\* в меню Центр партнеров, а затем выберите клиента, устройства которого требуется управлять.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="cbe4f-189">На странице сведения о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cbe4f-190">В разделе **применить профили к устройствам** выберите **Добавить устройства**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="cbe4f-191">Введите имя для списка устройств и нажмите кнопку **Обзор** , чтобы отправить список клиента (в формате CSV-файла) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="cbe4f-192">Вы должны получить этот CSV-файл с покупкой устройства.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="cbe4f-193">Если вы не получили CSV-файл, вы можете создать его самостоятельно, выполнив действия, описанные в разделе [Добавление устройств в Windows автопилот](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="cbe4f-194">Отправьте CSV-файл и нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="cbe4f-195">Если при попытке отправить CSV-файл появляется сообщение об ошибке, проверьте формат файла.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="cbe4f-196">Вы можете использовать только хэш оборудования или имя OEM, серийный номер и модель (в указанном порядке столбцов) или идентификатор продукта Windows.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="cbe4f-197">Вы также можете использовать файл Sample. csv, приведенный по ссылке далее, чтобы **Добавить устройства** для создания списка устройств.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="cbe4f-198">CSV-файл должен выглядеть примерно так:</span><span class="sxs-lookup"><span data-stu-id="cbe4f-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="cbe4f-199">**Серийный номер устройства, идентификатор продукта Windows, хэш оборудования, имя производителя, модель устройства**</span><span class="sxs-lookup"><span data-stu-id="cbe4f-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="cbe4f-200">**{serialNumber},,, корпорация Майкрософт, портативный компьютер**</span><span class="sxs-lookup"><span data-stu-id="cbe4f-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="cbe4f-201">Для "имени производителя" и "модель устройства" учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="cbe4f-202">Если вы не узнаете, какое значение следует указать для имени производителя и модели устройства, можно запустить его на устройстве, чтобы собрать правильные значения:</span><span class="sxs-lookup"><span data-stu-id="cbe4f-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="cbe4f-203">Закрытие лицензионного соглашения Windows для автопилота</span><span class="sxs-lookup"><span data-stu-id="cbe4f-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="cbe4f-204">ВАЖНАЯ ИНФОРМАЦИЯ</span><span class="sxs-lookup"><span data-stu-id="cbe4f-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="cbe4f-205">Windows автопилот позволяет настраивать настроенные установки Windows на устройствах, которыми вы управляете для клиентов.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="cbe4f-206">Если это разрешено клиентом, вы можете подавлять или скрывать определенные экраны настройки, которые обычно предоставляются пользователям при настройке Windows, включая экран подтверждения лицензионного соглашения (лицензионное соглашение).</span><span class="sxs-lookup"><span data-stu-id="cbe4f-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="cbe4f-207">С помощью этой функции вы соглашаетесь, что подавление или скрытие экранов, предназначенных для предоставления пользователям уведомления или принятия условий, означает, что вы получили достаточное согласие и авторизацию от клиента, чтобы скрыть термины, а также от имени клиента (будь то Организация или отдельный пользователь), согласие на любые уведомления и принимать любые условия, применимые к клиенту.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="cbe4f-208">Это включает согласие с условиями лицензии или уведомления, которое отображалось бы для пользователя, если не бы вы не отключили или не скрыли его с помощью этого средства.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="cbe4f-209">Ваш клиент не может использовать программное обеспечение Windows на этих устройствах, если ваш клиент не приобрел законным способом лицензию на программное обеспечение у Майкрософт или лицензированных дистрибьюторов.</span><span class="sxs-lookup"><span data-stu-id="cbe4f-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>