---
title: Использование веб-перехватчиков для получения событий изменения ресурсов
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте API-интерфейсы веб-перехватчика центра партнеров, чтобы узнать, когда происходят изменения ресурсов ссылок для Dynamics 365 CRM или Salesforce CRM.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ссылки, API веб-перехватчика, события изменения ресурсов
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89628fd6ccab6a943d8bd816afa7b5d3b0f241f7
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749177"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="636a8-104">Использование API-интерфейсов веб-перехватчика для регистрации событий изменения ресурсов для Dynamics 365 CRM и Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="636a8-104">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="636a8-105">Соответствующие роли</span><span class="sxs-lookup"><span data-stu-id="636a8-105">Appropriate roles</span></span>

- <span data-ttu-id="636a8-106">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="636a8-106">Referrals admin</span></span>
- <span data-ttu-id="636a8-107">Системный администратор или Настройщик системы для Dynamics 365 CRM или Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="636a8-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="636a8-108">Интерфейсы API веб-перехватчиков центра партнеров позволяют регистрироваться для событий изменения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="636a8-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="636a8-109">Эти события изменения отправляются на URL-адрес в виде HTTP-сообщений.</span><span class="sxs-lookup"><span data-stu-id="636a8-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="636a8-110">В этом разделе объясняются интерфейсы API веб-перехватчика для Dynamics 365 CRM и Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="636a8-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="636a8-111">Настройка объекта webhook</span><span class="sxs-lookup"><span data-stu-id="636a8-111">Configure the webhook</span></span>

1. <span data-ttu-id="636a8-112">Чтобы зарегистрировать URL-адрес, выберите **"регистрация центра партнеров" (Предварительная версия)** Power автоматизирующий поток.</span><span class="sxs-lookup"><span data-stu-id="636a8-112">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="636a8-113">Добавить соединения для (a.) Пользователь центра партнеров с ссылками на учетные данные администратора (b). События центра партнеров, отмеченные ниже</span><span class="sxs-lookup"><span data-stu-id="636a8-113">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Триггер":::

3. <span data-ttu-id="636a8-115">После выполнения этих обновлений вы увидите</span><span class="sxs-lookup"><span data-stu-id="636a8-115">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Веб-перехватчики":::

4. <span data-ttu-id="636a8-117">Сохраните изменения и выберите **включить**.</span><span class="sxs-lookup"><span data-stu-id="636a8-117">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="636a8-118">Чтобы разрешить веб-перехватчикам центра партнеров прослушивать изменения событий в партнерских объектах и ссылках объектов в центре партнеров и CRM, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="636a8-118">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="636a8-119">Выберите пункт **Центр партнеров для Dynamics 365 (Предварительная версия)** или **Центр партнеров в Salesforce (Предварительная версия для предварительной версии)**.</span><span class="sxs-lookup"><span data-stu-id="636a8-119">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="636a8-120">Щелкните значок **редактирования** и выберите **время получения HTTP-запроса**.</span><span class="sxs-lookup"><span data-stu-id="636a8-120">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="636a8-121">Щелкните значок **копирования** , чтобы скопировать предоставленный URL-адрес HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="636a8-121">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Копирование URL-адреса":::

8. <span data-ttu-id="636a8-123">Теперь выберите пункт "регистрация в Power Center (Предварительная версия)" и нажмите кнопку **запустить**.</span><span class="sxs-lookup"><span data-stu-id="636a8-123">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="636a8-124">Убедитесь, что в правой части окна откроется окно "запуск потока", и нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="636a8-124">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="636a8-125">Введите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="636a8-125">Enter the following details:</span></span>

    1. <span data-ttu-id="636a8-126">**Конечная точка триггера HTTP**: URL-адрес, скопированный с предыдущего шага</span><span class="sxs-lookup"><span data-stu-id="636a8-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="636a8-127">**Регистрируемые события**: "Создание ссылок" и "обновление ссылок"</span><span class="sxs-lookup"><span data-stu-id="636a8-127">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="636a8-128">**Перезаписать существующие конечные точки триггера (при наличии**): Да (при этом перезаписываются все существующие конечные точки).</span><span class="sxs-lookup"><span data-stu-id="636a8-128">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="636a8-129">Теперь веб-перехватчик может прослушивать изменения (создавать и обновлять события).</span><span class="sxs-lookup"><span data-stu-id="636a8-129">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="636a8-130">Выберите **выполнить** , а затем нажмите кнопку **Готово.**</span><span class="sxs-lookup"><span data-stu-id="636a8-130">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="636a8-131">Настройка шагов синхронизации</span><span class="sxs-lookup"><span data-stu-id="636a8-131">Customize synchronization steps</span></span>

<span data-ttu-id="636a8-132">Когда ссылки на совместные продажи синхронизируются между центром партнеров и системой CRM, поля, синхронизированные на ПК центра партнеров, перечислены здесь.</span><span class="sxs-lookup"><span data-stu-id="636a8-132">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="636a8-133">Часто системы CRM сильно настроены.</span><span class="sxs-lookup"><span data-stu-id="636a8-133">Often CRM systems are highly customized.</span></span> <span data-ttu-id="636a8-134">Можно настроить потоки автоматизации Powering.</span><span class="sxs-lookup"><span data-stu-id="636a8-134">You can customize the Power Automate flows.</span></span> <span data-ttu-id="636a8-135">Следуйте указаниям в руководстве по сопоставлению полей и при необходимости внесите соответствующие изменения в действиях потоков Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="636a8-135">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="636a8-136">Сопоставление Microsoft Partner Center с CRM предоставляется, но в зависимости от среды CRM вы можете выбрать дальнейшую настройку полей.</span><span class="sxs-lookup"><span data-stu-id="636a8-136">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="636a8-137">В зависимости от ваших потребностей можно настроить несколько шагов из каждого потока Power автоматизировать.</span><span class="sxs-lookup"><span data-stu-id="636a8-137">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="636a8-138">Ниже приведены примеры доступных настроек.</span><span class="sxs-lookup"><span data-stu-id="636a8-138">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="636a8-139">Чтобы настроить поля для событий создания или обновления в центре партнеров на синхронизацию ссылок CRM, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="636a8-139">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="636a8-140">Выберите пункт Центр партнеров для Dynamics 365 (Предварительная версия) или центр партнеров в Salesforce (Предварительная версия для предварительной версии).</span><span class="sxs-lookup"><span data-stu-id="636a8-140">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="636a8-141">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="636a8-141">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="636a8-142">Выберите **(область) синхронизация интереса или возможной сделки**.</span><span class="sxs-lookup"><span data-stu-id="636a8-142">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="636a8-143">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **, если это новая доступная возможность, а затем**.</span><span class="sxs-lookup"><span data-stu-id="636a8-143">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="636a8-144">Выберите подшаг, **Если да** , а затем — **Создание новой возможности в CRM**.</span><span class="sxs-lookup"><span data-stu-id="636a8-144">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="636a8-145">Сопоставления в этом разделе можно изменить с помощью инструкции по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="636a8-145">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="636a8-146">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, щелкните шаг "(область) синхронизация интереса или возможности".</span><span class="sxs-lookup"><span data-stu-id="636a8-146">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="636a8-147">Выберите **, если это обновление возможной сделки, а затем**.</span><span class="sxs-lookup"><span data-stu-id="636a8-147">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="636a8-148">Выберите подшаг, **Если да** , а затем — **различие между объектами возможности в центре партнеров и модулем CRM**.</span><span class="sxs-lookup"><span data-stu-id="636a8-148">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="636a8-149">Выберите, **Если да** , а затем **обновить существующую возможную сделку**</span><span class="sxs-lookup"><span data-stu-id="636a8-149">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="636a8-150">Чтобы настроить поля для синхронизации ссылок CRM и PC для событий обновления, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="636a8-150">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="636a8-151">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="636a8-151">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="636a8-152">Выберите **(область) синхронизировать возможную сделку**.</span><span class="sxs-lookup"><span data-stu-id="636a8-152">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="636a8-153">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для событий обновления, установите флажок, **Если между ведущими объектами в центре партнеров и CRM есть различия**.</span><span class="sxs-lookup"><span data-stu-id="636a8-153">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="636a8-154">Выберите подшаг, **Если да** , а затем разверните шаг **Обновление ссылки на данные о возможностях**.</span><span class="sxs-lookup"><span data-stu-id="636a8-154">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="636a8-155">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="636a8-155">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="636a8-156">Чтобы настроить поля для синхронизации ссылок CRM и PC для создания событий?</span><span class="sxs-lookup"><span data-stu-id="636a8-156">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="636a8-157">Выберите **изменить** , чтобы изменить или настроить поток Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="636a8-157">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="636a8-158">Выберите **(область) синхронизация ссылок.**</span><span class="sxs-lookup"><span data-stu-id="636a8-158">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="636a8-159">Чтобы настроить сопоставления полей CRM (в соответствии с руководством по сопоставлениям полей) для создания событий, выберите **создать ссылку Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="636a8-159">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="636a8-160">Сопоставления в этом разделе можно изменить в соответствии с руководством по сопоставлению полей.</span><span class="sxs-lookup"><span data-stu-id="636a8-160">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="636a8-161">Сквозная синхронизация двунаправленной совместной продажи</span><span class="sxs-lookup"><span data-stu-id="636a8-161">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="636a8-162">После установки, настройки и настройки решения Power автоматизиру вы можете проверить синхронизацию ссылок совместной продажи между Dynamics 365 или Salesforce и центром партнеров.</span><span class="sxs-lookup"><span data-stu-id="636a8-162">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="636a8-163">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="636a8-163">Pre-requisites</span></span>

<span data-ttu-id="636a8-164">Чтобы синхронизировать ссылки в центре партнеров и Dynamics 365 CRM или в центре партнеров и Salesforce CRM, в решении Power автоматизируется четкое разграничения полей ссылок, относящихся к корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="636a8-164">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="636a8-165">Это дает группам продавцов возможность выбирать, какие ссылки должны предоставляться корпорации Майкрософт для совместной продажи.</span><span class="sxs-lookup"><span data-stu-id="636a8-165">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="636a8-166">Набор настраиваемых полей доступен в рамках синхронизации ссылок центра партнеров для сущности **возможности** решения Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="636a8-166">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="636a8-167">Пользователь с правами администратора CRM должен создать отдельный раздел CRM с настраиваемыми полями **возможностей** .</span><span class="sxs-lookup"><span data-stu-id="636a8-167">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="636a8-168">Следующие настраиваемые поля должны быть частью раздела CRM:</span><span class="sxs-lookup"><span data-stu-id="636a8-168">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="636a8-169">**Синхронизация с центром партнеров**: следует ли синхронизировать возможность с центром партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="636a8-169">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="636a8-170">**Идентификатор ссылки**: поле идентификатора только для чтения для ссылки в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="636a8-170">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="636a8-171">**Ссылка на ссылку: ссылка**только для чтения на ссылку в центре партнеров Майкрософт</span><span class="sxs-lookup"><span data-stu-id="636a8-171">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="636a8-172">**Как можно получить справку Майкрософт?**: Помогите корпорации Майкрософт получить ссылку</span><span class="sxs-lookup"><span data-stu-id="636a8-172">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="636a8-173">**Продукты**: список продуктов, связанных с этой возможностью</span><span class="sxs-lookup"><span data-stu-id="636a8-173">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="636a8-174">**Аудит**: журнал аудита только для чтения для синхронизации с ссылками центра партнеров</span><span class="sxs-lookup"><span data-stu-id="636a8-174">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="636a8-175">ВАРИАНТ</span><span class="sxs-lookup"><span data-stu-id="636a8-175">SCENARIOS:</span></span>

1. <span data-ttu-id="636a8-176">Синхронизация ссылок при создании или обновлении ссылок в CRM и синхронизации в центре партнеров:</span><span class="sxs-lookup"><span data-stu-id="636a8-176">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="636a8-177">Войдите в среду Dynamics 365 CRM с помощью пользователя, который обладает видимостью в разделе **возможности** CRM.</span><span class="sxs-lookup"><span data-stu-id="636a8-177">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="636a8-178">При создании "новой возможности" в среде Dynamics 365 убедитесь, что указан следующий раздел:</span><span class="sxs-lookup"><span data-stu-id="636a8-178">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Opportunity;":::

   3. <span data-ttu-id="636a8-180">Чтобы синхронизировать эту возможность с центром партнеров Майкрософт, убедитесь, что в представлении карточка установлены следующие поля:</span><span class="sxs-lookup"><span data-stu-id="636a8-180">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="636a8-181">**Синхронизация с центром партнеров**: Да</span><span class="sxs-lookup"><span data-stu-id="636a8-181">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="636a8-182">**Как можно получить справку Майкрософт?**: выберите следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="636a8-182">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Параметры справки":::

      - <span data-ttu-id="636a8-184">**Продукты**: идентификаторы решений для продукта</span><span class="sxs-lookup"><span data-stu-id="636a8-184">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="636a8-185">После создания возможности в Dynamics 365 с параметром **Синхронизация с центром партнеров** задайте значение **Да**, подождите 10 минут, войдите в свою учетную запись центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="636a8-185">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="636a8-186">Ваши ссылки будут синхронизированы с Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="636a8-186">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="636a8-187">Следовательно, если для возможной сделки с параметром "Синхронизация с центром партнеров" установлено значение "Да", то при обновлении возможности в Dynamics 365 CRM изменения будут синхронизированы в учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="636a8-187">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="636a8-188">Возможности, успешно синхронизированные с центром партнеров, будут идентифицированы с помощью значка ✔ в Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="636a8-188">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="636a8-189">Синхронизация ссылок при создании или обновлении ссылок в центре партнеров Майкрософт и синхронизации в среде Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="636a8-189">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="636a8-190">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard/home)центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="636a8-190">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="636a8-191">В меню слева выберите **ссылки** .</span><span class="sxs-lookup"><span data-stu-id="636a8-191">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="636a8-192">Чтобы создать новую ссылку для совместной продажи из центра партнеров, щелкните "Новая сделка".</span><span class="sxs-lookup"><span data-stu-id="636a8-192">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="636a8-193">Войдите в среду Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="636a8-193">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="636a8-194">Перейдите к разделу **открытые возможности**.</span><span class="sxs-lookup"><span data-stu-id="636a8-194">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="636a8-195">Ссылка, созданная в центре партнеров Майкрософт, теперь синхронизируется в Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="636a8-195">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="636a8-196">При выборе синхронизированной ссылки сведения о представлении карточки заполняются.</span><span class="sxs-lookup"><span data-stu-id="636a8-196">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="636a8-197">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="636a8-197">Next steps</span></span>

- [<span data-ttu-id="636a8-198">Дополнительные сведения о платформе Microsoft Power автоматизиру</span><span class="sxs-lookup"><span data-stu-id="636a8-198">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="636a8-199">События веб-перехватчика центра партнеров</span><span class="sxs-lookup"><span data-stu-id="636a8-199">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="636a8-200">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="636a8-200">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="636a8-201">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="636a8-201">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
