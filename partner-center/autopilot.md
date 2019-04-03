---
title: Фирменную out-of-box устройства с помощью профилей Windows Autopilot | Центр партнеров
description: Выполните предварительную настройку устройства out-of-box опыт профилей Autopilot.
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, windows autopilot, microsoft autopilot, развертывания без участия пользователя, oobe, экраны входа, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162224"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="2b51a-104">Настройка устройства out-of-box опыт профили Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b51a-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="2b51a-105">**Применяется к**</span><span class="sxs-lookup"><span data-stu-id="2b51a-105">**Applies to**</span></span>

- <span data-ttu-id="2b51a-106">Билл direct партнеров CSP, непрямые поставщики и непрямые торговые посредники</span><span class="sxs-lookup"><span data-stu-id="2b51a-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="2b51a-107">Если вы управляете устройствами клиента, может потребоваться настроить для out-of-box experience (OOBE) для пользователей клиента.</span><span class="sxs-lookup"><span data-stu-id="2b51a-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="2b51a-108">Можно предварительно настроить новые устройства с помощью профилей Windows Autopilot перед поставкой клиентам устройств и применить новые профили устройств, которые уже приобрели клиентов.</span><span class="sxs-lookup"><span data-stu-id="2b51a-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="2b51a-109">В этой статье объясняется, как создать и применить профили Autopilot для устройств в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="2b51a-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="2b51a-110">Если вы еще не знакомы с Autopilot, просмотрите сведения в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="2b51a-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="2b51a-111">Обзор Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b51a-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="2b51a-112">Справочное руководство для развертывания AutoPilot</span><span class="sxs-lookup"><span data-stu-id="2b51a-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="2b51a-113">Обзор</span><span class="sxs-lookup"><span data-stu-id="2b51a-113">Overview</span></span>

<span data-ttu-id="2b51a-114">С помощью функции Windows Autopilot в центре партнеров можно создать настраиваемые профили для применения к устройствам пользователей.</span><span class="sxs-lookup"><span data-stu-id="2b51a-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="2b51a-115">Следующие параметры профиля были доступны во время публикации в этой статье:</span><span class="sxs-lookup"><span data-stu-id="2b51a-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="2b51a-116">Пропустить параметры конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2b51a-116">Skip privacy settings.</span></span> <span data-ttu-id="2b51a-117">Этот необязательный параметр профиля Autopilot позволяет организациям не интересовались параметры конфиденциальности во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b51a-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="2b51a-118">Отключение создания учетной записи локального администратора на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2b51a-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="2b51a-119">Компании могут сами решать ли настройке устройства пользователь должен иметь доступ с правами администратора, после завершения процесса.</span><span class="sxs-lookup"><span data-stu-id="2b51a-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="2b51a-120">Автоматически настройте устройство для работы или учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2b51a-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="2b51a-121">Все устройства, зарегистрированные с помощью Autopilot автоматически будет считаться рабочих или учебных устройств, поэтому этот вопрос не будет запрашиваться во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b51a-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="2b51a-122">Пропустить страницы настройки регистрации OEM, OneDrive и Cortana.</span><span class="sxs-lookup"><span data-stu-id="2b51a-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="2b51a-123">Все устройства, зарегистрированные с помощью Autopilot автоматически будет пропускать эти страницы во время процесса out-of-box experience (OOBE).</span><span class="sxs-lookup"><span data-stu-id="2b51a-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="2b51a-124">Пропустить лицензионное соглашение (EULA).</span><span class="sxs-lookup"><span data-stu-id="2b51a-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="2b51a-125">Начиная с Windows 10 версии 1709, организации могут принять решение о пропуске страницы лицензионного соглашения, представленные в процессе OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b51a-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="2b51a-126">См. в разделе [увольнения лицензионное соглашение Windows Autopilot](#windows-autopilot-eula-dismissal) ниже важные сведения, касающиеся пропуска страницы лицензионного соглашения во время Windows установки.</span><span class="sxs-lookup"><span data-stu-id="2b51a-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="2b51a-127">Применяются следующие разрешения на управление профиль и устройства и ограничения.</span><span class="sxs-lookup"><span data-stu-id="2b51a-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="2b51a-128">Партнеры CSP могут продолжать управлять профилей Autopilot для существующих клиентов, с которыми у них есть отношений торгового посредника, даже если клиенты были удалены права делегированного администрирования партнера.</span><span class="sxs-lookup"><span data-stu-id="2b51a-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="2b51a-129">Вы можете управлять существующих устройств для ваших клиентов, которые были добавлены.</span><span class="sxs-lookup"><span data-stu-id="2b51a-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="2b51a-130">Нельзя управлять устройствами, которые клиент загруженные пользователем в Microsoft Store для бизнеса или на портале Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="2b51a-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="2b51a-131">Создание и управление ими профилей Autopilot в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="2b51a-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="2b51a-132">В центре партнеров можно создать профили развертывания Windows Autopilot и применить их к устройствам.</span><span class="sxs-lookup"><span data-stu-id="2b51a-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="2b51a-133">Только агенты администрирования можно создать и применить профили.</span><span class="sxs-lookup"><span data-stu-id="2b51a-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="2b51a-134">Создать новый профиль Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b51a-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="2b51a-135">Выберите **клиентов** меню центра партнеров, а затем выберите клиента вы создаете профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b51a-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b51a-136">На странице сведений клиента, выберите **устройств**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b51a-137">В разделе **профили Windows Autopilot** выберите **добавить новый профиль**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="2b51a-138">Введите имя и описание профиля, а затем настройте параметры OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b51a-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="2b51a-139">Выберите один из следующих вариантов:</span><span class="sxs-lookup"><span data-stu-id="2b51a-139">Choose from:</span></span>  

   - <span data-ttu-id="2b51a-140">Пропустить параметров конфиденциальности в программе установки</span><span class="sxs-lookup"><span data-stu-id="2b51a-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="2b51a-141">Отключение учетной записи локального администратора при настройке</span><span class="sxs-lookup"><span data-stu-id="2b51a-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="2b51a-142">Автоматический пропуск страниц при настройке</span><span class="sxs-lookup"><span data-stu-id="2b51a-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="2b51a-143">(Включает в себя *автоматически выберите настройку для работы или учебы* и *OEM, OneDrive и Cortana пропустить страницы настройки регистрации*)</span><span class="sxs-lookup"><span data-stu-id="2b51a-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="2b51a-144">Пропустить лицензионное соглашение (EULA)</span><span class="sxs-lookup"><span data-stu-id="2b51a-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="2b51a-145">См. в разделе [увольнения лицензионное соглашение Windows Autopilot](#windows-autopilot-eula-dismissal) ниже важные сведения, касающиеся пропуска страницы лицензионного соглашения во время Windows установки.</span><span class="sxs-lookup"><span data-stu-id="2b51a-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="2b51a-146">По завершении нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="2b51a-147">Профиль Autopilot, применяются к устройствам клиента</span><span class="sxs-lookup"><span data-stu-id="2b51a-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="2b51a-148">В инструкциях ниже предполагается, что вы уже добавили клиента устройства для центра партнеров и, можно приступить к их список устройств.</span><span class="sxs-lookup"><span data-stu-id="2b51a-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="2b51a-149">Если не было добавлено устройства клиента, следуйте инструкциям в [добавить устройства в учетной записи клиента](#add-devices-to-a-customers-account) и затем выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="2b51a-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="2b51a-150">После создания профиля Autopilot для клиента, его можно применить для клиента устройства.</span><span class="sxs-lookup"><span data-stu-id="2b51a-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="2b51a-151">Выберите **клиентов** меню центра партнеров, а затем выберите клиента, вы создали профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b51a-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b51a-152">На странице сведений клиента, выберите **устройств**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b51a-153">В разделе **профили, применяются к устройствам** выберите устройства или группы устройств, которые вы хотите добавить профили для, а затем выберите **применить профиль**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="2b51a-154">Появится новый профиль, примененных в **профиль** столбца.</span><span class="sxs-lookup"><span data-stu-id="2b51a-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="2b51a-155">Выполните следующие действия, чтобы проверить, что профиль будет успешно применена к устройству.</span><span class="sxs-lookup"><span data-stu-id="2b51a-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="2b51a-156">1.</span><span class="sxs-lookup"><span data-stu-id="2b51a-156">a.</span></span>  <span data-ttu-id="2b51a-157">Подключите устройство к сети и включить его.</span><span class="sxs-lookup"><span data-stu-id="2b51a-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="2b51a-158">2.</span><span class="sxs-lookup"><span data-stu-id="2b51a-158">b.</span></span>  <span data-ttu-id="2b51a-159">Убедитесь, что отображаются соответствующие экраны OOBE (если они должны отображаться).</span><span class="sxs-lookup"><span data-stu-id="2b51a-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="2b51a-160">В.</span><span class="sxs-lookup"><span data-stu-id="2b51a-160">c.</span></span>  <span data-ttu-id="2b51a-161">При остановке процесса OOBE, сброс устройства до заводских настроек по умолчанию для подготовки его для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b51a-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="2b51a-162">Удаление профиля Autopilot с устройства клиента</span><span class="sxs-lookup"><span data-stu-id="2b51a-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="2b51a-163">Выберите **клиентов** меню центра партнеров, а затем выберите клиента, вы создали профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b51a-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b51a-164">На странице сведений клиента, выберите **устройств**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b51a-165">В разделе **профили, применяются к устройствам** выберите устройства, которые вы хотите удалить профиль из, а затем выберите **удалить профиль**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="2b51a-166">Удаление профиля с устройства не приводит к удалению профиля из списка.</span><span class="sxs-lookup"><span data-stu-id="2b51a-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="2b51a-167">Если вы хотите удалить профиль, следуйте инструкциям в [обновления или удаления профиля Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="2b51a-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="2b51a-168">Обновление или удаление профиля Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b51a-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="2b51a-169">Если клиент хочет меняют взаимодействие с out-of-box после поставки устройств к ним, вы можете изменить профиль в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="2b51a-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="2b51a-170">При подключении устройства клиента к Интернету, он будет последняя версия профиля во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b51a-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="2b51a-171">Кроме того любое время, клиент восстанавливает на устройстве заводские настройки, устройство будет снова последняя версия профиля во время процесса OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b51a-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="2b51a-172">Выберите **клиентов** в меню центра партнеров и затем выберите клиента, который хочет, чтобы изменить профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b51a-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="2b51a-173">На странице сведений клиента, выберите **устройств**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b51a-174">В разделе **профили Windows Autopilot** выберите профиль, необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2b51a-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="2b51a-175">Внесите необходимые изменения, а затем выберите **отправить**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="2b51a-176">Чтобы удалить этот профиль, выберите **удалить профиль** в правом верхнем углу страницы.</span><span class="sxs-lookup"><span data-stu-id="2b51a-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="2b51a-177">Добавить устройства в учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="2b51a-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="2b51a-178">Агентов по продажам и агенты администрирования можно добавить устройства к учетной записи клиента.</span><span class="sxs-lookup"><span data-stu-id="2b51a-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="2b51a-179">Перед применением настраиваемых профилей Autopilot на устройствах пользователей, необходимо для доступа к списку устройств клиента.</span><span class="sxs-lookup"><span data-stu-id="2b51a-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="2b51a-180">Если вы планируете использовать имя изготовителя Оборудования, серийный номер и комбинации модели, необходимо учитывать следующие ограничения.</span><span class="sxs-lookup"><span data-stu-id="2b51a-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="2b51a-181">Эта кортежа работает только для новых устройств (4 k хеш-коды, например) и не поддерживается для 128b хэши (предыдущий устройств и RS2).</span><span class="sxs-lookup"><span data-stu-id="2b51a-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="2b51a-182">Регистрации кортежа чувствительно к регистру, поэтому данные в файле должны совпадать с именами модели и производителя ***точно*** как предоставляемых поставщиком OEM (поставщик оборудования).</span><span class="sxs-lookup"><span data-stu-id="2b51a-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="2b51a-183">Следуйте инструкциям для добавления устройств в учетной записи клиента в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="2b51a-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="2b51a-184">Выберите **клиентов** в меню центра партнеров и затем выберите клиента устройства, на которых вы хотите управлять.</span><span class="sxs-lookup"><span data-stu-id="2b51a-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="2b51a-185">На странице сведений клиента, выберите **устройств**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b51a-186">В разделе **профили, применяются к устройствам** выберите **добавить устройства**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="2b51a-187">Введите имя для списка устройств, а затем выберите **Обзор** для отправки списка клиента (в формат CSV-файла) в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="2b51a-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2b51a-188">Вы должны были получить этот CSV-файл при приобретении устройств.</span><span class="sxs-lookup"><span data-stu-id="2b51a-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="2b51a-189">Если вы не получили в CSV-файл, можно создать самостоятельно, выполнив действия, описанные в [добавлению устройств Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="2b51a-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="2b51a-190">Отправить CSV-файл, а затем выберите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="2b51a-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="2b51a-191">Если появится сообщение об ошибке при попытке отправить CSV-файл, проверьте формат файла.</span><span class="sxs-lookup"><span data-stu-id="2b51a-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="2b51a-192">Можно использовать хэш-код оборудования, или название OEM, серийный номер и модель (в таком порядке столбцов) или идентификатор продукта Windows.</span><span class="sxs-lookup"><span data-stu-id="2b51a-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="2b51a-193">Можно также использовать образец CSV-файла, предоставляемые по ссылке рядом с полем **добавить устройства** для создания списка устройств.</span><span class="sxs-lookup"><span data-stu-id="2b51a-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="2b51a-194">Лицензионное соглашение Windows Autopilot увольнения</span><span class="sxs-lookup"><span data-stu-id="2b51a-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="2b51a-195">ВАЖНЫЕ СВЕДЕНИЯ</span><span class="sxs-lookup"><span data-stu-id="2b51a-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="2b51a-196">Windows Autopilot позволяет настроить настраиваемой установки Windows на устройствах, которыми вы управляете для ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="2b51a-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="2b51a-197">Если разрешение для этого клиента, можно отключить или скрыть определенные экраны настройки, которые обычно представляются пользователю при настройке Windows, в том числе экран принятия лицензионного соглашения (лицензионное соглашение).</span><span class="sxs-lookup"><span data-stu-id="2b51a-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="2b51a-198">С помощью этой функции, вы подтверждаете, что отключение или скрытие любых экранов, которые предназначены для предоставления пользователям уведомления или принятия условий означает, что вы получили достаточно согласия и авторизации у вашего клиента, чтобы скрыть условия и вами, от имени Клиент (организация или отдельного пользователя как в случае может ли быть), согласие на все уведомления и принимает любые условия, применимые к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="2b51a-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="2b51a-199">Это включает согласие с условиями лицензии или уведомления, которое отображалось бы для пользователя, если не бы вы не отключили или не скрыли его с помощью этого средства.</span><span class="sxs-lookup"><span data-stu-id="2b51a-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="2b51a-200">Ваш клиент не может использовать программное обеспечение Windows на этих устройствах, если ваш клиент не приобрел законным способом лицензию на программное обеспечение у Майкрософт или лицензированных дистрибьюторов.</span><span class="sxs-lookup"><span data-stu-id="2b51a-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>