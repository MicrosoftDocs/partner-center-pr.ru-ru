---
title: Профили для выплат и налогов в Центре партнеров
ms.topic: how-to
ms.date: 11/12/2020
description: Создайте и управляйте своим выплатами и налоговым профилем, чтобы вы могли получить оплату за работу по поощрениям. Включает создание, управление и использование различных профилей.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 66177c6e3cd0091081866e1508d28346f49ec713
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626037"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="79c88-104">Создание и управление выплатами и налоговыми профилями поощрения в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="79c88-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="79c88-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="79c88-105">**Applies to:**</span></span>

- <span data-ttu-id="79c88-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="79c88-106">Partner Center</span></span>

<span data-ttu-id="79c88-107">**Соответствующие роли:**</span><span class="sxs-lookup"><span data-stu-id="79c88-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="79c88-108">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="79c88-108">Incentives admin</span></span>
- <span data-ttu-id="79c88-109">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="79c88-109">Account admin</span></span>
- <span data-ttu-id="79c88-110">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="79c88-110">Global admin</span></span>

<span data-ttu-id="79c88-111">Чтобы получать выплаты по программе поощрений для определенного местонахождения MPN, завершите процесс регистрации, привязав к программе и местонахождению MPN действительный профиль для выплат и налогов.</span><span class="sxs-lookup"><span data-stu-id="79c88-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="79c88-112">Корпорация Майкрософт будет использовать этот платежный и налоговый профиль для осуществления платежей.</span><span class="sxs-lookup"><span data-stu-id="79c88-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="79c88-113">В зависимости от правила программы поощрений, вам может быть доступна оплата электронным банковским переводом или по кредитовому авизо.</span><span class="sxs-lookup"><span data-stu-id="79c88-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="79c88-114">Роли, валюты и другие программы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="79c88-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="79c88-115">Прежде чем начать работу с выплатами и налоговым профилем, важно понять приведенные ниже сведения.</span><span class="sxs-lookup"><span data-stu-id="79c88-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="79c88-116">Роли и разрешения</span><span class="sxs-lookup"><span data-stu-id="79c88-116">Roles and permissions</span></span>

<span data-ttu-id="79c88-117">Вы должны быть администратором поощрения, чтобы вводить банковские и налоговые данные для поощрения платежей.</span><span class="sxs-lookup"><span data-stu-id="79c88-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="79c88-118">Если вы являетесь администратором MPN или учетной записи, вы можете назначить себя и (или) коллегу в качестве администратора поощрения.</span><span class="sxs-lookup"><span data-stu-id="79c88-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="79c88-119">Если вам нужно запросить разрешения администратора поощрения, обратитесь к администратору MPN или глобальному администратору. Чтобы узнать, кто в вашей компании имеет эти роли, войдите на [панель мониторинга центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="79c88-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="79c88-120">На значке **параметров** в правом верхнем углу выберите **Управление пользователями** , а затем выполните фильтрацию по глобальному администратору.</span><span class="sxs-lookup"><span data-stu-id="79c88-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="79c88-121">Пользователи поощрения могут просматривать сведения о поощрении и отчетах об оплате, но не могут изменять банковские и налоговые данные.</span><span class="sxs-lookup"><span data-stu-id="79c88-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="79c88-122">Выбор денежной суммы</span><span class="sxs-lookup"><span data-stu-id="79c88-122">Choose your disbursement currency</span></span>

<span data-ttu-id="79c88-123">Поощрительные платежи выполняются в валюте, выбранной при настройке профиля оплаты.</span><span class="sxs-lookup"><span data-stu-id="79c88-123">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="79c88-124">Платежи будут рассчитываться с использованием обменного курса, установленного ежемесячно корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="79c88-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="79c88-125">Вы несете ответственность за любые изменения в значении из-за выбранной валюты.</span><span class="sxs-lookup"><span data-stu-id="79c88-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="79c88-126">Использование различных профилей для различных программ Майкрософт</span><span class="sxs-lookup"><span data-stu-id="79c88-126">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="79c88-127">Если ваша компания зарегистрирована в нескольких поощрениях программ, вы можете использовать один и тот же платежный счет для всех из них или использовать разные платежные счета для разных программ.</span><span class="sxs-lookup"><span data-stu-id="79c88-127">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="79c88-128">Создание профилей для выплат и налогов и управление ими в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="79c88-128">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="79c88-129">В следующих разделах описывается процесс создания и управления платежами и налоговыми профилями в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="79c88-129">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="79c88-130">Для создания профилей платежей и управления ими в центре партнеров необходимо быть администратором-стимулом.</span><span class="sxs-lookup"><span data-stu-id="79c88-130">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="79c88-131">Роли стимула должны быть назначены каждому MPN расположению в рамках каждой программы поощрения.</span><span class="sxs-lookup"><span data-stu-id="79c88-131">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="79c88-132">Дополнительные сведения о добавлении поощрительных администраторов в центре партнеров см. в разделе [Создание учетных записей пользователей](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="79c88-132">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="79c88-133">Доступ к разделу выплата и налог в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="79c88-133">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="79c88-134">Войдите на [панель мониторинга центра партнеров](https://partner.microsoft.com/dashboard/) , используя учетную запись Azure Active Directory (Azure AD) (учетная запись организации) или соответствующий адрес электронной почты, если он был назначен.</span><span class="sxs-lookup"><span data-stu-id="79c88-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="79c88-135">Несколько доменов можно зарегистрировать в одной учетной записи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="79c88-135">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="79c88-136">Обратитесь к глобальному администратору, чтобы определить, какие домены связаны.</span><span class="sxs-lookup"><span data-stu-id="79c88-136">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="79c88-137">Если вы можете войти только с помощью @onmicrosoft.com домена, обратитесь к администратору учетной записи, чтобы добавить дополнительные домены в учетную запись Azure AD.</span><span class="sxs-lookup"><span data-stu-id="79c88-137">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="79c88-138">Если будет предложено выбрать **рабочую или учебную учетную запись** или **личную учетную** запись, выберите **Рабочая или учебная учетная запись**.</span><span class="sxs-lookup"><span data-stu-id="79c88-138">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account**.</span></span>

2. <span data-ttu-id="79c88-139">Щелкните значок шестеренки, чтобы открыть меню **Параметры** , а затем выберите **Параметры партнера**.</span><span class="sxs-lookup"><span data-stu-id="79c88-139">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="79c88-140">В меню **Параметры учетной записи** выберите **выплата и налог**.</span><span class="sxs-lookup"><span data-stu-id="79c88-140">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="79c88-141">Назначение профилей выплата и налоговый профиль отдельным программам</span><span class="sxs-lookup"><span data-stu-id="79c88-141">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="79c88-142">Войдите на [панель мониторинга центра партнеров](https://partner.microsoft.com/dashboard/), а затем щелкните значок шестеренки, чтобы открыть меню **параметров** .</span><span class="sxs-lookup"><span data-stu-id="79c88-142">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="79c88-143">Выберите **Параметры партнеров** , разверните **раздел выплата и налог** , а затем выберите **выплата и назначение профиля налога**.</span><span class="sxs-lookup"><span data-stu-id="79c88-143">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="79c88-144">Отобразится список программ.</span><span class="sxs-lookup"><span data-stu-id="79c88-144">A list of your programs will be displayed.</span></span> <span data-ttu-id="79c88-145">Щелкните стрелку рядом с программой, чтобы просмотреть сведения о профиле.</span><span class="sxs-lookup"><span data-stu-id="79c88-145">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="79c88-146">В раскрывающемся меню " **налоговый профиль** " выберите нужный профиль налога или выберите вариант создания нового профиля.</span><span class="sxs-lookup"><span data-stu-id="79c88-146">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="79c88-147">При выборе варианта создания нового профиля вы будете перенаправлены соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="79c88-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="79c88-148">Нажмите кнопку продолжить во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="79c88-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="79c88-149">Ниже приведен процесс создания нового профиля налогов.</span><span class="sxs-lookup"><span data-stu-id="79c88-149">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="79c88-150">Выберите **метод оплаты**.</span><span class="sxs-lookup"><span data-stu-id="79c88-150">Select **Payment method**.</span></span>

   - <span data-ttu-id="79c88-151">Если в качестве метода оплаты выбран параметр **электронный банк** , выберите нужный профиль оплаты или выберите вариант создания нового профиля.</span><span class="sxs-lookup"><span data-stu-id="79c88-151">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="79c88-152">При выборе варианта создания нового профиля вы будете перенаправлены соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="79c88-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="79c88-153">Нажмите кнопку продолжить во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="79c88-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="79c88-154">Ниже приведен процесс создания нового профиля оплаты.</span><span class="sxs-lookup"><span data-stu-id="79c88-154">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="79c88-155">Если вы выбрали **кредит** -ноту в качестве метода оплаты, завершите проверку.</span><span class="sxs-lookup"><span data-stu-id="79c88-155">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="79c88-156">Это подтверждает, что указанный номер SAP принадлежит вашей организации.</span><span class="sxs-lookup"><span data-stu-id="79c88-156">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="79c88-157">Если в списке есть несколько бизнес-сущностей Майкрософт, необходимо выбрать профиль оплаты для каждой сущности.</span><span class="sxs-lookup"><span data-stu-id="79c88-157">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="79c88-158">Доступность метода оплаты зависит от правил программы поощрения.</span><span class="sxs-lookup"><span data-stu-id="79c88-158">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="79c88-159">Выберите **валюту**.</span><span class="sxs-lookup"><span data-stu-id="79c88-159">Select the **Currency**.</span></span>

6. <span data-ttu-id="79c88-160">Завершив все поля оплаты, выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="79c88-160">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="79c88-161">Создание профиля банка</span><span class="sxs-lookup"><span data-stu-id="79c88-161">Create your bank profile</span></span>

<span data-ttu-id="79c88-162">Профили банка создаются на уровне Организации.</span><span class="sxs-lookup"><span data-stu-id="79c88-162">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="79c88-163">Это позволяет назначить один банковский профиль между несколькими программами MPN ID и стимулами в Организации.</span><span class="sxs-lookup"><span data-stu-id="79c88-163">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="79c88-164">При применении профиля банка к разным странам могут возникнуть исключения, так как могут применяться различные банковские и налоговые правила.</span><span class="sxs-lookup"><span data-stu-id="79c88-164">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="79c88-165">На следующих страницах требуются поля со звездочкой.</span><span class="sxs-lookup"><span data-stu-id="79c88-165">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="79c88-166">Если вы не уверены, что такое поле, щелкните значок сведений.</span><span class="sxs-lookup"><span data-stu-id="79c88-166">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="79c88-167">На странице **сведения** заполните следующие поля: **имя профиля:** введите уникальное имя для указания этого профиля оплаты.</span><span class="sxs-lookup"><span data-stu-id="79c88-167">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="79c88-168">**Расположение банковского счета:** Страна, в которой находится банк вашей компании.</span><span class="sxs-lookup"><span data-stu-id="79c88-168">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="79c88-169">**Способ оплаты:** Предпочтительным методом оплаты для центра партнеров является перенос в электронном банке.</span><span class="sxs-lookup"><span data-stu-id="79c88-169">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="79c88-170">Выберите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="79c88-170">Select **Next**.</span></span>

3. <span data-ttu-id="79c88-171">На странице " **банковский счет** " введите свои данные.</span><span class="sxs-lookup"><span data-stu-id="79c88-171">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="79c88-172">Поля, показанные на этой странице, будут зависеть от страны.</span><span class="sxs-lookup"><span data-stu-id="79c88-172">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="79c88-173">Выберите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="79c88-173">Select **Next**.</span></span>

5. <span data-ttu-id="79c88-174">На странице **бенефициар** введите соответствующие сведения.</span><span class="sxs-lookup"><span data-stu-id="79c88-174">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="79c88-175">Бенефициар — это лицо в вашей организации, к которому будет обращаться банк при необходимости обсудить вашу учетную запись.</span><span class="sxs-lookup"><span data-stu-id="79c88-175">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="79c88-176">После заполнения полей нажмите кнопку **Готово** , а затем нажмите кнопку **подтвердить** , чтобы создать свой банковский профиль.</span><span class="sxs-lookup"><span data-stu-id="79c88-176">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="79c88-177">Вы будете перенаправлены на страницу **выплата и профили налогов** .</span><span class="sxs-lookup"><span data-stu-id="79c88-177">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="79c88-178">Состояние нового профиля будет отражать **ожидаемую проверку Майкрософт** до завершения проверки.</span><span class="sxs-lookup"><span data-stu-id="79c88-178">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="79c88-179">Этот процесс может занять до 48 часов.</span><span class="sxs-lookup"><span data-stu-id="79c88-179">This process may take up to 48 hours.</span></span> <span data-ttu-id="79c88-180">После завершения проверки профиль будет отображаться как **утвержденный** , так и **требуемый действие**.</span><span class="sxs-lookup"><span data-stu-id="79c88-180">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="79c88-181">Если **требуется действие** , повторите описанные выше действия, предоставив необходимые сведения.</span><span class="sxs-lookup"><span data-stu-id="79c88-181">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="79c88-182">Создание профиля налога</span><span class="sxs-lookup"><span data-stu-id="79c88-182">Create your tax profile</span></span>

<span data-ttu-id="79c88-183">Следующая процедура используется для предоставления корпорации Майкрософт сведений о налогах, необходимых для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="79c88-183">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="79c88-184">Страницы в этом разделе являются динамическими и будут отличаться в зависимости от страны или региона.</span><span class="sxs-lookup"><span data-stu-id="79c88-184">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="79c88-185">Если вам нужна помощь с определением правильных сведений о налогах, обратитесь к соответствующим государственным источникам в вашей стране.</span><span class="sxs-lookup"><span data-stu-id="79c88-185">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="79c88-186">Для компаний-партнеров в Americas, если вам нужны сведения о заполнении форм W8 или W9, следующие адреса переведут Вас на сайт IRS:</span><span class="sxs-lookup"><span data-stu-id="79c88-186">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="79c88-187">Введите только сведения для своей компании.</span><span class="sxs-lookup"><span data-stu-id="79c88-187">Enter only details for your company.</span></span> <span data-ttu-id="79c88-188">Никогда не вводите личные данные.</span><span class="sxs-lookup"><span data-stu-id="79c88-188">Never enter personal details.</span></span>

1. <span data-ttu-id="79c88-189">На странице **Бизнес-профиль** заполните обязательные поля и нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="79c88-189">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="79c88-190">На странице **Установка** выберите вариант, применяемый к вашей компании.</span><span class="sxs-lookup"><span data-stu-id="79c88-190">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="79c88-191">Выберите параметр слева, если ваша компания включена только в США или если этот профиль предназначен для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="79c88-191">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="79c88-192">Выберите параметр справа, если ваша компания включена за пределами США, а затем выберите страну или регион из списка.</span><span class="sxs-lookup"><span data-stu-id="79c88-192">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="79c88-193">Выберите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="79c88-193">Select **Next**.</span></span> 

4. <span data-ttu-id="79c88-194">На странице " **состояние налога** " введите необходимые сведения, а затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="79c88-194">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="79c88-195">Поля на этой странице будут зависеть от страны.</span><span class="sxs-lookup"><span data-stu-id="79c88-195">Fields on this page will vary by country.</span></span> <span data-ttu-id="79c88-196">сведения.</span><span class="sxs-lookup"><span data-stu-id="79c88-196">your details.</span></span> 

5. <span data-ttu-id="79c88-197">На странице **Дополнительная документация** укажите обязательные поля и нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="79c88-197">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="79c88-198">Нажмите кнопку **Обзор** , чтобы отправить все документы, необходимые для вашей страны или региона.</span><span class="sxs-lookup"><span data-stu-id="79c88-198">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="79c88-199">Когда отобразится имя документа, выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="79c88-199">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="79c88-200">Если необходимо удалить документ, выберите **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="79c88-200">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="79c88-201">Чтобы сохранить и продолжить, нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="79c88-201">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="79c88-202">Выберите **подтвердить** во всплывающем сообщении.</span><span class="sxs-lookup"><span data-stu-id="79c88-202">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="79c88-203">Вы вернетесь на страницу **Настройка выплата и налог** .</span><span class="sxs-lookup"><span data-stu-id="79c88-203">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="79c88-204">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="79c88-204">Next steps</span></span>

- [<span data-ttu-id="79c88-205">Часто задаваемые вопросы о профилях для выплат и налогов в рамках программы поощрения</span><span class="sxs-lookup"><span data-stu-id="79c88-205">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
