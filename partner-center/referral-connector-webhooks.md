---
title: Использование веб-перехватчиков для получения событий изменения ресурсов
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Использование API-интерфейсов веб-перехватчика для выяснения того, когда происходят изменения ресурсов ссылок
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ссылки, API веб-перехватчика, события изменения ресурсов
ms.localizationpriority: medium
ms.openlocfilehash: a141776f1b591ebe41bb740051802b4b55cf36f0
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "83796210"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="0ff8a-104">Использование API веб-перехватчика для регистрации событий изменения ресурсов</span><span class="sxs-lookup"><span data-stu-id="0ff8a-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="0ff8a-105">Соответствующие роли</span><span class="sxs-lookup"><span data-stu-id="0ff8a-105">Appropriate roles</span></span>

- <span data-ttu-id="0ff8a-106">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="0ff8a-106">Referrals admin</span></span>
- <span data-ttu-id="0ff8a-107">Системный администратор или Настройщик системы для Dynamics 365 CRM или Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="0ff8a-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="0ff8a-108">Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="0ff8a-109">Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="0ff8a-110">В этом разделе объясняются интерфейсы API веб-перехватчика для Dynamics 365 CRM и Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="0ff8a-111">Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="0ff8a-112">Добавить соединения для (a.) Пользователь центра партнеров с ссылками на учетные данные администратора (b). События центра партнеров, отмеченные ниже</span><span class="sxs-lookup"><span data-stu-id="0ff8a-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Триггер](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="0ff8a-114">После выполнения этих обновлений вы увидите</span><span class="sxs-lookup"><span data-stu-id="0ff8a-114">When you make these updates, you will see</span></span>

![Веб-перехватчики](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="0ff8a-116">Сохраните изменения и выберите **включить**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="0ff8a-117">Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий в партнерских объектах и ссылках объектов в центре партнеров и CRM, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="0ff8a-118">Выберите пункт **Центр партнеров для Dynamics 365 (Предварительная версия)** или **Центр партнеров в Salesforce (Предварительная версия для предварительной версии)**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="0ff8a-119">Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="0ff8a-120">Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Копирование URL-адреса](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="0ff8a-122">Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="0ff8a-123">Убедитесь, что в правой части окна откроется окно "запуск потока", и нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="0ff8a-124">Введите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-124">Enter the following details:</span></span> 

    <span data-ttu-id="0ff8a-125">а.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-125">a.</span></span> <span data-ttu-id="0ff8a-126">**Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага</span><span class="sxs-lookup"><span data-stu-id="0ff8a-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="0ff8a-127">б.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-127">b.</span></span> <span data-ttu-id="0ff8a-128">**Регистрируемые события**: "Создание ссылок" и "обновление ссылок"</span><span class="sxs-lookup"><span data-stu-id="0ff8a-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="0ff8a-129">в.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-129">c.</span></span> <span data-ttu-id="0ff8a-130">**Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки).</span><span class="sxs-lookup"><span data-stu-id="0ff8a-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="0ff8a-131">Теперь веб-перехватчик может прослушивать изменения (создавать и обновлять события).</span><span class="sxs-lookup"><span data-stu-id="0ff8a-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="0ff8a-132">Выберите **выполнить** , а затем нажмите кнопку **Готово.**</span><span class="sxs-lookup"><span data-stu-id="0ff8a-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="0ff8a-133">Настройка шагов синхронизации</span><span class="sxs-lookup"><span data-stu-id="0ff8a-133">Customize synchronization steps</span></span>

<span data-ttu-id="0ff8a-134">Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="0ff8a-135">Часто системы CRM сильно настроены.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="0ff8a-136">Можно настроить потоки автоматизации Powering.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="0ff8a-137">Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="0ff8a-138">Сопоставление Microsoft Partner Center с CRM предоставляется, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="0ff8a-139">В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="0ff8a-140">Ниже приведены примеры доступных настроек.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="0ff8a-141">Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="0ff8a-142">а.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-142">a.</span></span> <span data-ttu-id="0ff8a-143">Выберите пункт Центр партнеров для Dynamics 365 (Предварительная версия) или центр партнеров в Salesforce (Предварительная версия для предварительной версии).</span><span class="sxs-lookup"><span data-stu-id="0ff8a-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="0ff8a-144">б.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-144">b.</span></span> <span data-ttu-id="0ff8a-145">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="0ff8a-146">в.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-146">c.</span></span> <span data-ttu-id="0ff8a-147">Выберите **(область) синхронизация интереса или возможной сделки**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="0ff8a-148">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **, если это новая доступная возможность, а затем**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="0ff8a-149">Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="0ff8a-150">Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="0ff8a-151">г.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-151">d.</span></span> <span data-ttu-id="0ff8a-152">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, щелкните шаг "(область) синхронизация интереса или возможности".</span><span class="sxs-lookup"><span data-stu-id="0ff8a-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="0ff8a-153">Д.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-153">e.</span></span> <span data-ttu-id="0ff8a-154">Выберите **, если это обновление возможной сделки, а затем**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="0ff8a-155">Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="0ff8a-156">f.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-156">f.</span></span> <span data-ttu-id="0ff8a-157">Выберите, **Если да** , а затем **обновить существующую возможную сделку**</span><span class="sxs-lookup"><span data-stu-id="0ff8a-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="0ff8a-158">Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="0ff8a-159">а.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-159">a.</span></span> <span data-ttu-id="0ff8a-160">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="0ff8a-161">б.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-161">b.</span></span> <span data-ttu-id="0ff8a-162">Выберите **(область) синхронизировать возможную сделку**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="0ff8a-163">в.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-163">c.</span></span> <span data-ttu-id="0ff8a-164">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, установите флажок, **Если между ведущими объектами в центре партнеров и CRM есть различия**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="0ff8a-165">г.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-165">d.</span></span> <span data-ttu-id="0ff8a-166">Выберите подшаг, **Если да** , а затем разверните шаг **Обновление ссылки на данные о возможностях**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="0ff8a-167">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="0ff8a-168">Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?</span><span class="sxs-lookup"><span data-stu-id="0ff8a-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="0ff8a-169">а.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-169">a.</span></span> <span data-ttu-id="0ff8a-170">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="0ff8a-171">б.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-171">b.</span></span> <span data-ttu-id="0ff8a-172">Выберите **(область) синхронизация ссылок.**</span><span class="sxs-lookup"><span data-stu-id="0ff8a-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="0ff8a-173">в.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-173">c.</span></span> <span data-ttu-id="0ff8a-174">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="0ff8a-175">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="0ff8a-176">Сквозная синхронизация двунаправленной совместной продажи</span><span class="sxs-lookup"><span data-stu-id="0ff8a-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="0ff8a-177">После установки, настройки и настройки решения Power автоматизиру вы можете проверить синхронизацию ссылок совместной продажи между Dynamics 365 или Salesforce и центром партнеров.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="0ff8a-178">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0ff8a-178">Pre-requisites</span></span>

<span data-ttu-id="0ff8a-179">Чтобы синхронизировать ссылки в центре партнеров и Dynamics 365 CRM или в центре партнеров и Salesforce CRM, в решении Power автоматизируется четкое разграничения полей ссылок, относящихся к корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="0ff8a-180">Это дает группам продавцов возможность выбирать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="0ff8a-181">Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможности** решения Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="0ff8a-182">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="0ff8a-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="0ff8a-183">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="0ff8a-184">**Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="0ff8a-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="0ff8a-185">**Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="0ff8a-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="0ff8a-186">**Ссылка на ссылку: ссылка**только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="0ff8a-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="0ff8a-187">**Как можно получить справку Майкрософт?**: Помогите корпорации Майкрософт получить ссылку</span><span class="sxs-lookup"><span data-stu-id="0ff8a-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="0ff8a-188">**Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="0ff8a-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="0ff8a-189">**Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров</span><span class="sxs-lookup"><span data-stu-id="0ff8a-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="0ff8a-190">ВАРИАНТ</span><span class="sxs-lookup"><span data-stu-id="0ff8a-190">SCENARIOS:</span></span>

1. <span data-ttu-id="0ff8a-191">Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="0ff8a-192">а.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-192">a.</span></span> <span data-ttu-id="0ff8a-193">Войдите в среду Dynamics 365 CRM или среду Salesforce CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-193">Sign into your Dynamics 365 CRM environment or Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="0ff8a-194">б.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-194">b.</span></span> <span data-ttu-id="0ff8a-195">При создании "новой возможности" в среде Dynamics 365 убедитесь, что указан следующий раздел:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Opportunity;](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="0ff8a-197">в.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-197">c.</span></span> <span data-ttu-id="0ff8a-198">Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="0ff8a-199">"Синхронизация с центром партнеров": Да</span><span class="sxs-lookup"><span data-stu-id="0ff8a-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="0ff8a-200">«Как можно получить справку Майкрософт?»: выберите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![Параметры справки](images/cosellconnectors/help.png)

    - <span data-ttu-id="0ff8a-202">Продукты: идентификаторы решений для продукта</span><span class="sxs-lookup"><span data-stu-id="0ff8a-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="0ff8a-203">г.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-203">d.</span></span> <span data-ttu-id="0ff8a-204">После создания возможности в Dynamics 365 с параметром **Синхронизация с центром партнеров** задайте значение **Да**, подождите 10 минут, войдите в свою учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="0ff8a-205">Ваши ссылки будут синхронизированы с Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="0ff8a-206">Д.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-206">e.</span></span> <span data-ttu-id="0ff8a-207">Следовательно, если для возможной сделки с параметром "Синхронизация с центром партнеров" установлено значение "Да", то при обновлении возможности в Dynamics 365 CRM изменения будут синхронизированы в учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="0ff8a-208">f.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-208">f.</span></span> <span data-ttu-id="0ff8a-209">Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="0ff8a-210">Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="0ff8a-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="0ff8a-211">а.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-211">a.</span></span> <span data-ttu-id="0ff8a-212">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="0ff8a-213">б.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-213">b.</span></span> <span data-ttu-id="0ff8a-214">В меню слева выберите **ссылки** .</span><span class="sxs-lookup"><span data-stu-id="0ff8a-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="0ff8a-215">в.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-215">c.</span></span> <span data-ttu-id="0ff8a-216">Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".</span><span class="sxs-lookup"><span data-stu-id="0ff8a-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="0ff8a-217">г.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-217">d.</span></span> <span data-ttu-id="0ff8a-218">Войдите в среду Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="0ff8a-219">Д.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-219">e.</span></span> <span data-ttu-id="0ff8a-220">Перейдите к разделу **открытые возможности**.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="0ff8a-221">Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="0ff8a-222">f.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-222">f.</span></span> <span data-ttu-id="0ff8a-223">При выборе синхронизированной ссылки сведения о представлении карточки заполняются.</span><span class="sxs-lookup"><span data-stu-id="0ff8a-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="0ff8a-224">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="0ff8a-224">Next steps</span></span>

- [<span data-ttu-id="0ff8a-225">Дополнительные сведения о платформе Microsoft Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="0ff8a-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="0ff8a-226">События веб-перехватчика центра партнеров</span><span class="sxs-lookup"><span data-stu-id="0ff8a-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="0ff8a-227">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="0ff8a-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="0ff8a-228">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="0ff8a-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
