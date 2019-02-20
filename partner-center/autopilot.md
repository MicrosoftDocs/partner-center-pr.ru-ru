---
title: Настроить out-of-box устройства с помощью профилей Windows Autopilot | Центр партнеров
description: Выполните предварительную настройку устройства out-of-box взаимодействие с профилями Autopilot.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, windows autopilot, microsoft autopilot, zero-touch deployment, oobe, экраны входа, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: d563ad09d1fa3b67b01835480a348a524455efbc
ms.sourcegitcommit: f1c269f4ac52d5206d65d9585855da309f0aae8a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2019
ms.locfileid: "9083407"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="b0bdb-104">Настроить out-of-box устройства с помощью профилей Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="b0bdb-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="b0bdb-105">Область применения</span><span class="sxs-lookup"><span data-stu-id="b0bdb-105">Applies to</span></span>**

- <span data-ttu-id="b0bdb-106">Партнерам CSP счет direct, непрямые поставщики и непрямые торговые посредники</span><span class="sxs-lookup"><span data-stu-id="b0bdb-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="b0bdb-107">Если вы управляете устройства пользователей, может потребоваться настроить out-of-box (OOBE) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="b0bdb-108">Можно предварительной конфигурации новых устройств с помощью профилей Windows Autopilot перед доставкой устройств для пользователей и применить новые профили для устройств, которые уже приобрели клиентов.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="b0bdb-109">В этой статье объясняется, как создавать и применять профили Autopilot на устройствах в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="b0bdb-110">Если вы еще не знакомы с помощью Autopilot, просмотрите сведения в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="b0bdb-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="b0bdb-111">Обзор Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="b0bdb-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="b0bdb-112">Справочник развертывания AutoPilot</span><span class="sxs-lookup"><span data-stu-id="b0bdb-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="b0bdb-113">Обзор</span><span class="sxs-lookup"><span data-stu-id="b0bdb-113">Overview</span></span>

<span data-ttu-id="b0bdb-114">С помощью компонента Windows Autopilot в центре партнеров вы можете создать пользовательские профили, чтобы применить к устройствам клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="b0bdb-115">Следующие параметры профиля были доступны на момент публикации этой статьи:</span><span class="sxs-lookup"><span data-stu-id="b0bdb-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="b0bdb-116">Пропуск параметров конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-116">Skip privacy settings.</span></span> <span data-ttu-id="b0bdb-117">Это необязательный параметр профиля Autopilot позволяет организациям не Узнайте о параметрах конфиденциальности во время запуска при первом Включении.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="b0bdb-118">Отключение создания учетной записи локального администратора на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="b0bdb-119">Организации могут выбирать, будут ли настройки устройства пользователь должен иметь доступ с правами администратора, после завершения процесса.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="b0bdb-120">Автоматически настроить устройство для работы или учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="b0bdb-121">Все устройства, зарегистрированные с помощью Autopilot автоматически будет считаться рабочих или учебных устройств, поэтому этот вопрос не придется во время запуска при первом Включении.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="b0bdb-122">Пропустить страницы регистрации настройки Кортаны, OneDrive и OEM.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="b0bdb-123">Все устройства, зарегистрированные с помощью Autopilot автоматически пропустит одной страницы на другую в процессе out-of-box experience (OOBE).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="b0bdb-124">Пропустите лицензионное соглашение (EULA).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="b0bdb-125">Начиная с Windows 10 версии 1709, организации могут решили пропустить страницу лицензионного соглашения, отображаются во время запуска при первом Включении.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="b0bdb-126">См. в разделе [Windows Autopilot отказе](#windows-autopilot-eula-dismissal) ниже важные сведения необходимо учитывать о пропуск странице Лицензионное соглашение во время установки Windows.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="b0bdb-127">Примените следующие разрешения профиля и устройства управления и ограничения:</span><span class="sxs-lookup"><span data-stu-id="b0bdb-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="b0bdb-128">Партнеры CSP могут продолжать управлять профилями Autopilot существующих клиентов, с которыми они отношения торгового посредника, даже если клиенты отобрали делегированные права администратора партнера.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="b0bdb-129">Можно управлять имеющимися устройствами за ваших клиентов, которые были добавлены вами или другим партнером CSP.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="b0bdb-130">Вы не можете управлять устройствами, которые загрузил ваш клиент магазин Майкрософт для бизнеса или портала Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="b0bdb-131">Создание и управление профилями Autopilot в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="b0bdb-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="b0bdb-132">В центре партнеров можно создать развертывания Windows AutoPilot и применить их к устройствам.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="b0bdb-133">Только агенты можно создавать и применять профили.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="b0bdb-134">Создайте новый профиль Autopilot</span><span class="sxs-lookup"><span data-stu-id="b0bdb-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="b0bdb-135">Выберите **клиентов** в меню центра партнеров, а затем выберите клиента, которого вы создаете профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="b0bdb-136">На странице сведений о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b0bdb-137">**Профили Windows Autopilot** установите **Добавить новый профиль**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="b0bdb-138">Введите имя и описание профиля, а затем настройте параметры OOBE.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="b0bdb-139">Выберите:</span><span class="sxs-lookup"><span data-stu-id="b0bdb-139">Choose from:</span></span>  

   - <span data-ttu-id="b0bdb-140">Пропуск параметров конфиденциальности при настройке</span><span class="sxs-lookup"><span data-stu-id="b0bdb-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="b0bdb-141">Отключение учетной записи локального администратора при настройке</span><span class="sxs-lookup"><span data-stu-id="b0bdb-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="b0bdb-142">Автоматический пропуск страниц при настройке</span><span class="sxs-lookup"><span data-stu-id="b0bdb-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="b0bdb-143">(Включает *Автоматический выбор конфигурации для работы или учебного заведения* и *Пропустить Кортаны, OneDrive и OEM страницы регистрации для установки*)</span><span class="sxs-lookup"><span data-stu-id="b0bdb-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="b0bdb-144">Пропустите лицензионное соглашение (EULA)</span><span class="sxs-lookup"><span data-stu-id="b0bdb-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="b0bdb-145">См. в разделе [Windows Autopilot отказе](#windows-autopilot-eula-dismissal) ниже важные сведения необходимо учитывать о пропуск странице Лицензионное соглашение во время установки Windows.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="b0bdb-146">По завершении нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="b0bdb-147">Примените профиль Autopilot на устройствах пользователей</span><span class="sxs-lookup"><span data-stu-id="b0bdb-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="b0bdb-148">Приведенные ниже инструкции предполагается, что вы уже добавили устройств клиента в центр партнеров и что есть доступ к их списка устройств.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="b0bdb-149">Если вы еще не добавили устройств клиента, следуйте инструкциям в [устройствах добавить учетную запись клиента](#add-devices-to-a-customers-account) , а затем выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="b0bdb-150">После создания профиля Autopilot для клиента, его можно применить к устройствам клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="b0bdb-151">Выберите **клиентов** в меню центра партнеров, а затем выберите клиента, которого вы создали профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b0bdb-152">На странице сведений о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b0bdb-153">В группе **Профили применить к устройствам** выберите устройства или группы устройств, которые вы хотите добавить профили для, а затем выберите **применить профиль**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="b0bdb-154">Профиль, который вы только что применили отображается в столбце " **профиль** ".</span><span class="sxs-lookup"><span data-stu-id="b0bdb-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="b0bdb-155">Выполните следующие действия, чтобы убедиться, что профиль будет успешно применена к устройству.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="b0bdb-156">А.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-156">a.</span></span>  <span data-ttu-id="b0bdb-157">Подключите устройство к сети и включите его.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="b0bdb-158">b.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-158">b.</span></span>  <span data-ttu-id="b0bdb-159">Убедитесь, что отображаются соответствующие экраны OOBE (если они должны отображаться).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="b0bdb-160">c.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-160">c.</span></span>  <span data-ttu-id="b0bdb-161">При остановке процесс запуска при первом Включении, сбросьте устройство к заводским настройкам по умолчанию для подготовки для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="b0bdb-162">Удалить профиль Autopilot на устройстве пользователя</span><span class="sxs-lookup"><span data-stu-id="b0bdb-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="b0bdb-163">Выберите **клиентов** в меню центра партнеров, а затем выберите клиента, которого вы создали профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b0bdb-164">На странице сведений о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b0bdb-165">В группе **Профили применить к устройствам** выберите устройства, которые вы хотите удалить профиль, а затем выберите **Удалить профиль**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="b0bdb-166">Удаление профиля с устройства не приводит к удалению профиля из списка.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="b0bdb-167">Если вы хотите удалить профиль, следуйте инструкциям в [обновление или удаление профиля Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="b0bdb-168">Обновление или удаление профиля Autopilot</span><span class="sxs-lookup"><span data-stu-id="b0bdb-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="b0bdb-169">Если пользователь может изменить работу out-of-box после того, как поставки устройств на них, вы можете изменить профиль в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="b0bdb-170">При подключении устройства пользователя к Интернету, оно будет последняя версия профиля во время запуска при первом Включении.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="b0bdb-171">Кроме того любое время, клиент восстановит устройство к заводским настройкам по умолчанию, устройство будет снова последняя версия профиля во время запуска при первом Включении.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="b0bdb-172">Выберите **клиентов** в меню центра партнеров, а затем выберите клиента, желающего вам потребуется изменить профиль Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="b0bdb-173">На странице сведений о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b0bdb-174">В разделе **профили Windows Autopilot** выберите профиль, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="b0bdb-175">Внесите необходимые изменения, а затем выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="b0bdb-176">Для удаления этого профиля, выберите **Удалить профиль** в верхнем правом углу страницы.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="b0bdb-177">Добавление устройств для учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="b0bdb-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="b0bdb-178">Агентов по продажам и агенты можно добавить устройства для учетной записи клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="b0bdb-179">Прежде чем применять настраиваемые профили Autopilot на устройствах пользователей, необходимо будет получать доступ к списку устройств клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="b0bdb-180">Если вы планируете использовать имя изготовителя Оборудования, серийный номер и комбинации модели, следует учитывать следующие ограничения:</span><span class="sxs-lookup"><span data-stu-id="b0bdb-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="b0bdb-181">Эта кортежа работает только для новых устройств (4 k хэши, например) и не поддерживается для хэши 128b (RS2 и предыдущие устройства).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="b0bdb-182">Регистрация кортежа чувствителен к регистру, поэтому данные в файле должен модели и производителя имена ***точно*** предоставляется поставщиком Оборудования (поставщик оборудования).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="b0bdb-183">Следуйте приведенным ниже инструкциям для добавления устройств для учетной записи клиента в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="b0bdb-184">Выберите **клиентов** в меню центра партнеров, а затем выберите клиента, которого вы хотите управлять устройствами.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="b0bdb-185">На странице сведений о клиенте выберите **устройства**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b0bdb-186">В группе **Профили применить к устройствам** выберите **Добавить устройства**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="b0bdb-187">Введите имя для списка устройств, а затем выберите **Обзор** , чтобы передать список клиента (в формат CSV-файла) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b0bdb-188">Вы должны были получить этот CSV-файл с помощью покупки устройства.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="b0bdb-189">Если вы не получаете CSV-файл, можно создать один самостоятельно, выполнив действия, описанные в [Добавление устройств Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="b0bdb-190">Отправка CSV-файл, а затем выберите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="b0bdb-191">Если вы получите сообщение об ошибке при попытке загрузки CSV-файла, проверьте формат файла.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="b0bdb-192">Можно использовать только хэш оборудования или имя изготовителя Оборудования, серийный номер и модель (в указанном порядке столбов) или код продукта Windows.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="b0bdb-193">Также можно использовать образец CSV-файла, предоставляемый по ссылке рядом с **Добавить устройства** для создания списка устройств.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="b0bdb-194">Windows Autopilot отказе</span><span class="sxs-lookup"><span data-stu-id="b0bdb-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="b0bdb-195">ВАЖНАЯ ИНФОРМАЦИЯ</span><span class="sxs-lookup"><span data-stu-id="b0bdb-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="b0bdb-196">Windows Autopilot позволяет настроить пользовательские установки Windows на устройствах, которыми вы управляете для своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="b0bdb-197">Если для этого клиента, можно отключить или скрыть некоторые экраны, которые обычно отображаются для пользователей при настройке Windows, включая экран принятия лицензионного соглашения (лицензионного соглашения).</span><span class="sxs-lookup"><span data-stu-id="b0bdb-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="b0bdb-198">Используя эту функцию, вы соглашаетесь, что отключение или скрытие экранов, предназначенных для предоставления пользователям уведомления или принятие условий, означает, что вы получили достаточное согласие и от своего клиента для скрытия условия и что вы лица Ваш клиент (ли организации или отдельного пользователя может быть), согласие на любые уведомления и принимаете любые условия, применимые к вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="b0bdb-199">Это включает согласие с условиями лицензии или уведомления, которое отображалось бы для пользователя, если не бы вы не отключили или не скрыли его с помощью этого средства.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="b0bdb-200">Ваш клиент не может использовать программное обеспечение Windows на этих устройствах, если ваш клиент не приобрел законным способом лицензию на программное обеспечение у Майкрософт или лицензированных дистрибьюторов.</span><span class="sxs-lookup"><span data-stu-id="b0bdb-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>