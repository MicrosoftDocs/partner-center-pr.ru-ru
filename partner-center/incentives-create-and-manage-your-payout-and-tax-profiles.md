---
title: Создание профилей для выплат и налогов и управление ими в Центре партнеров
ms.topic: how-to
ms.date: 06/29/2020
description: Прежде чем вы сможете получить оплату за работу по поощрениям, необходимо создать профили выплат и налогов.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 3e7424ff1329d9c2bf13e9a6c4181c312396e073
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/04/2020
ms.locfileid: "87546045"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="91875-103">Профили для выплат и налогов в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="91875-103">Payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="91875-104">Область применения:</span><span class="sxs-lookup"><span data-stu-id="91875-104">Applies to:</span></span>

- <span data-ttu-id="91875-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="91875-105">Partner Center</span></span>

<span data-ttu-id="91875-106">Чтобы получать выплаты по программе поощрений для определенного местонахождения MPN, завершите процесс регистрации, привязав к программе и местонахождению MPN действительный профиль для выплат и налогов.</span><span class="sxs-lookup"><span data-stu-id="91875-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="91875-107">Корпорация Майкрософт будет использовать этот платежный и налоговый профиль для осуществления платежей.</span><span class="sxs-lookup"><span data-stu-id="91875-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="91875-108">В зависимости от правила программы поощрений, вам может быть доступна оплата электронным банковским переводом или по кредитовому авизо.</span><span class="sxs-lookup"><span data-stu-id="91875-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

<span data-ttu-id="91875-109">Соответствующие роли:</span><span class="sxs-lookup"><span data-stu-id="91875-109">Appropriate roles:</span></span>

- <span data-ttu-id="91875-110">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="91875-110">Incentives admin</span></span>
- <span data-ttu-id="91875-111">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="91875-111">Billing admin</span></span>
- <span data-ttu-id="91875-112">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="91875-112">Global admin</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="91875-113">Создание профилей для выплат и налогов и управление ими в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="91875-113">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="91875-114">В следующих разделах описывается процесс создания и управления платежами и налоговыми профилями в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="91875-114">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="91875-115">Для создания профилей платежей и управления ими в центре партнеров необходимо быть администратором-стимулом.</span><span class="sxs-lookup"><span data-stu-id="91875-115">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="91875-116">Роли стимула должны быть назначены каждому MPN расположению в рамках каждой программы поощрения.</span><span class="sxs-lookup"><span data-stu-id="91875-116">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="91875-117">Дополнительные сведения о добавлении поощрительных администраторов в центре партнеров см. в статье [Добавление поощрений пользователей или администраторов в центре партнеров](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="91875-117">For more information on how to add Incentive admins in Partner Center, see [How to add incentive users or admins in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="91875-118">Доступ к разделу выплата и налог в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="91875-118">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="91875-119">Войдите в центр партнеров, используя учетную запись AAD (учетную запись компании), или соответствующий адрес электронной почты, если он был назначен.</span><span class="sxs-lookup"><span data-stu-id="91875-119">Log into Partner Center using your AAD account (company account), or the appropriate email address if one was assigned.</span></span> 

   - <span data-ttu-id="91875-120">Несколько доменов можно зарегистрировать в одной учетной записи AAD.</span><span class="sxs-lookup"><span data-stu-id="91875-120">Multiple domains can be registered within one AAD account.</span></span> <span data-ttu-id="91875-121">Обратитесь к глобальному администратору, чтобы определить, какие домены связаны.</span><span class="sxs-lookup"><span data-stu-id="91875-121">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="91875-122">Если вы можете войти только в **@onmicrosoft.com** домен, обратитесь к администратору учетной записи, чтобы добавить дополнительные домены в учетную запись AAD.</span><span class="sxs-lookup"><span data-stu-id="91875-122">If you are only able to login with **@onmicrosoft.com** domain, contact your Account admin to add additional domains to the AAD account.</span></span>
   - <span data-ttu-id="91875-123">Если будет предложено выбрать **рабочую или учебную учетную запись** или **личную учетную**запись, выберите **Рабочая или учебная учетная запись**.</span><span class="sxs-lookup"><span data-stu-id="91875-123">If prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="91875-124">Щелкните значок шестеренки, чтобы открыть меню **Параметры** , а затем выберите **Параметры партнера**.</span><span class="sxs-lookup"><span data-stu-id="91875-124">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="91875-125">В меню **Параметры учетной записи** выберите **выплата и налог**.</span><span class="sxs-lookup"><span data-stu-id="91875-125">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="91875-126">Назначение профилей выплата и налоговый профиль отдельным программам</span><span class="sxs-lookup"><span data-stu-id="91875-126">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="91875-127">В центре партнеров выберите значок шестеренки, чтобы открыть меню **параметров** .</span><span class="sxs-lookup"><span data-stu-id="91875-127">In Partner Center, select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="91875-128">Выберите **Параметры партнеров**, разверните **раздел выплата и налог**, а затем выберите **выплата и назначение профиля налога**.</span><span class="sxs-lookup"><span data-stu-id="91875-128">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="91875-129">Отобразится список программ.</span><span class="sxs-lookup"><span data-stu-id="91875-129">A list of your programs will be displayed.</span></span> <span data-ttu-id="91875-130">Щелкните стрелку рядом с программой, чтобы просмотреть сведения о профиле.</span><span class="sxs-lookup"><span data-stu-id="91875-130">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="91875-131">В раскрывающемся меню " **налоговый профиль** " выберите нужный профиль налога или выберите вариант создания нового профиля.</span><span class="sxs-lookup"><span data-stu-id="91875-131">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="91875-132">При выборе варианта создания нового профиля вы будете перенаправлены соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="91875-132">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="91875-133">Нажмите кнопку продолжить во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="91875-133">Select Continue in the pop-up window.</span></span> <span data-ttu-id="91875-134">Ниже приведен процесс создания нового профиля налогов.</span><span class="sxs-lookup"><span data-stu-id="91875-134">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="91875-135">Выберите **метод оплаты**.</span><span class="sxs-lookup"><span data-stu-id="91875-135">Select **Payment method**.</span></span>

   - <span data-ttu-id="91875-136">Если в качестве метода оплаты выбран параметр **электронный банк** , то в раскрывающемся списке профиль оплаты выберите нужный профиль оплаты или выберите вариант создания нового профиля.</span><span class="sxs-lookup"><span data-stu-id="91875-136">If you have selected **Electronic bank transfer** as payment method then in the payment profile dropdown select the payment profile you want or select the option to create a new profile.</span></span> <span data-ttu-id="91875-137">При выборе варианта создания нового профиля вы будете перенаправлены соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="91875-137">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="91875-138">Нажмите кнопку продолжить во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="91875-138">Select Continue in the pop-up window.</span></span> <span data-ttu-id="91875-139">Ниже приведен процесс создания нового профиля оплаты.</span><span class="sxs-lookup"><span data-stu-id="91875-139">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="91875-140">Если вы выбрали **кредит** -ноту в качестве метода оплаты, выполните проверку, чтобы убедиться, что указанный номер SAP принадлежит вашей организации.</span><span class="sxs-lookup"><span data-stu-id="91875-140">If you have selected **Credit Note** as the payment method then complete the verification to confirm that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="91875-141">Если в списке есть несколько бизнес-сущностей Майкрософт, необходимо выбрать профиль оплаты для каждой сущности.</span><span class="sxs-lookup"><span data-stu-id="91875-141">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="91875-142">Доступность метода оплаты зависит от правил программы поощрения.</span><span class="sxs-lookup"><span data-stu-id="91875-142">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="91875-143">Выберите **валюту**.</span><span class="sxs-lookup"><span data-stu-id="91875-143">Select the **Currency**.</span></span>

6. <span data-ttu-id="91875-144">Завершив все поля оплаты, выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="91875-144">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="91875-145">Создание профиля банка</span><span class="sxs-lookup"><span data-stu-id="91875-145">Create your bank profile</span></span>

<span data-ttu-id="91875-146">Профили банка создаются на уровне Организации, что позволяет назначать один и тот же профиль банка между несколькими программами MPN ID и стимулами в Организации.</span><span class="sxs-lookup"><span data-stu-id="91875-146">Bank profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="91875-147">При применении профиля банка к разным странам могут возникнуть исключения, так как могут применяться различные банковские и налоговые правила.</span><span class="sxs-lookup"><span data-stu-id="91875-147">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="91875-148">На следующих страницах требуются поля со звездочкой.</span><span class="sxs-lookup"><span data-stu-id="91875-148">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="91875-149">Если вы не уверены, что такое поле, щелкните значок сведений.</span><span class="sxs-lookup"><span data-stu-id="91875-149">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="91875-150">На странице **сведения** заполните следующие поля: **имя профиля:** введите уникальное имя для указания этого профиля оплаты.</span><span class="sxs-lookup"><span data-stu-id="91875-150">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="91875-151">**Расположение банковского счета:** Страна, в которой находится банк вашей компании.</span><span class="sxs-lookup"><span data-stu-id="91875-151">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="91875-152">**Способ оплаты:** Предпочтительный способ оплаты — это перевод электронного банка в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="91875-152">**Payment method:** The preferred payment method is for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="91875-153">Выберите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="91875-153">Select **Next**.</span></span>

3. <span data-ttu-id="91875-154">На странице " **банковский счет** " введите свои данные.</span><span class="sxs-lookup"><span data-stu-id="91875-154">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="91875-155">Поля, показанные на этой странице, будут зависеть от страны.</span><span class="sxs-lookup"><span data-stu-id="91875-155">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="91875-156">Выберите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="91875-156">Select **Next**.</span></span>

5. <span data-ttu-id="91875-157">На странице **бенефициар** введите соответствующие сведения.</span><span class="sxs-lookup"><span data-stu-id="91875-157">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="91875-158">Бенефициар — это лицо в вашей организации, к которому будет обращаться банк при необходимости обсудить вашу учетную запись.</span><span class="sxs-lookup"><span data-stu-id="91875-158">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="91875-159">После заполнения полей нажмите кнопку **Готово**, а затем нажмите кнопку **подтвердить** , чтобы создать свой банковский профиль.</span><span class="sxs-lookup"><span data-stu-id="91875-159">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="91875-160">Вы будете перенаправлены на страницу **выплата и профили налогов** .</span><span class="sxs-lookup"><span data-stu-id="91875-160">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="91875-161">Состояние нового профиля будет отражать **ожидаемую проверку Майкрософт** до завершения проверки.</span><span class="sxs-lookup"><span data-stu-id="91875-161">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="91875-162">Это может занять до 48 часов.</span><span class="sxs-lookup"><span data-stu-id="91875-162">This may take up to 48 hours.</span></span> <span data-ttu-id="91875-163">После завершения проверки профиль будет отображаться как **утвержденный** , так и **требуемый действие**.</span><span class="sxs-lookup"><span data-stu-id="91875-163">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="91875-164">Если **требуется действие**, повторите описанные выше действия, предоставив необходимые сведения.</span><span class="sxs-lookup"><span data-stu-id="91875-164">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="91875-165">Создание профиля налога</span><span class="sxs-lookup"><span data-stu-id="91875-165">Create your tax profile</span></span>

<span data-ttu-id="91875-166">Следующая процедура используется для предоставления корпорации Майкрософт сведений о налогах, необходимых для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="91875-166">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="91875-167">Страницы в этом разделе являются динамическими и будут отличаться в зависимости от страны или региона.</span><span class="sxs-lookup"><span data-stu-id="91875-167">The pages in this section are dynamic and will vary according your country or region.</span></span> <span data-ttu-id="91875-168">Если вам нужна помощь с определением правильных сведений о налогах, обратитесь к соответствующим правительственным источникам в вашей стране.</span><span class="sxs-lookup"><span data-stu-id="91875-168">If you need help identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="91875-169">Для компаний-партнеров в Americas, если вам нужны сведения о заполнении форм W8 или W9, следующие адреса переведут Вас на сайт IRS:</span><span class="sxs-lookup"><span data-stu-id="91875-169">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="91875-170">Введите только сведения для своей компании.</span><span class="sxs-lookup"><span data-stu-id="91875-170">Enter only details for your company.</span></span> <span data-ttu-id="91875-171">Никогда не вводите личные данные.</span><span class="sxs-lookup"><span data-stu-id="91875-171">Never enter personal details.</span></span>

1. <span data-ttu-id="91875-172">На странице **Бизнес-профиль** заполните обязательные поля и нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="91875-172">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="91875-173">На странице **Установка** выберите вариант, применяемый к вашей компании.</span><span class="sxs-lookup"><span data-stu-id="91875-173">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="91875-174">Выберите параметр слева, если ваша компания включена только в США или если этот профиль предназначен для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="91875-174">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span> 
   - <span data-ttu-id="91875-175">Выберите параметр справа, если ваша компания включена за пределами США, а затем выберите страну или регион из списка.</span><span class="sxs-lookup"><span data-stu-id="91875-175">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="91875-176">Выберите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="91875-176">Select **Next**.</span></span> 

4. <span data-ttu-id="91875-177">На странице " **состояние налога** " введите необходимые сведения, а затем нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="91875-177">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="91875-178">Поля на этой странице будут зависеть от страны.</span><span class="sxs-lookup"><span data-stu-id="91875-178">Fields on this page will vary by country.</span></span> <span data-ttu-id="91875-179">сведения.</span><span class="sxs-lookup"><span data-stu-id="91875-179">your details.</span></span> 

5. <span data-ttu-id="91875-180">На странице **Дополнительная документация** укажите обязательные поля и нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="91875-180">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="91875-181">Нажмите кнопку **Обзор** , чтобы отправить все документы, необходимые для вашей страны или региона.</span><span class="sxs-lookup"><span data-stu-id="91875-181">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="91875-182">Когда отобразится имя документа, выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="91875-182">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="91875-183">Если необходимо удалить документ, выберите **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="91875-183">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="91875-184">Чтобы сохранить и продолжить, нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="91875-184">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="91875-185">Выберите **подтвердить** во всплывающем сообщении.</span><span class="sxs-lookup"><span data-stu-id="91875-185">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="91875-186">Вы вернетесь на страницу **Настройка выплата и налог** .</span><span class="sxs-lookup"><span data-stu-id="91875-186">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="payout-and-tax-profile-faqs"></a><span data-ttu-id="91875-187">Часто задаваемые вопросы о выплатах и профиле налогов</span><span class="sxs-lookup"><span data-stu-id="91875-187">Payout and tax profile FAQs</span></span>

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a><span data-ttu-id="91875-188">Зачем нужно предоставлять сведения о выплатах и налогах?</span><span class="sxs-lookup"><span data-stu-id="91875-188">Why do I need to provide my payout and/or tax details?</span></span>

<span data-ttu-id="91875-189">Чтобы получать выдачи для программ поощрения Майкрософт, необходимо выполнить регистрацию, предоставив сведения о выплатах и налогах.</span><span class="sxs-lookup"><span data-stu-id="91875-189">In order to receive payouts for Microsoft incentive programs, you need to complete enrollment by providing valid payout and tax details.</span></span> <span data-ttu-id="91875-190">Регистрация считается завершенной только в том случае, если указанная вами проверка выдачи и налогового профиля проверяется корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="91875-190">An enrollment is considered complete only when the payout and tax profile you provide is validated by Microsoft.</span></span>

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a><span data-ttu-id="91875-191">Разделы справки знать, что мне нужно предоставить или обновить сведения о выплатах и налогах?</span><span class="sxs-lookup"><span data-stu-id="91875-191">How do I know that I need to provide/update my payout and/or tax details?</span></span>

<span data-ttu-id="91875-192">Все партнеры, которые регистрируются в новой программе-стимуле, должны предоставить действительные сведения о выплатах и налогах для завершения регистрации.</span><span class="sxs-lookup"><span data-stu-id="91875-192">All partners enrolling in a new incentive program must provide valid payout and tax details to complete the enrollment.</span></span>

<span data-ttu-id="91875-193">Вам также может потребоваться предоставить обновленную информацию при изменении правил для программы поощрения или в случае истечения срока действия профиля или его устаревания.</span><span class="sxs-lookup"><span data-stu-id="91875-193">You may also need to provide updated information if the rules for your incentive program change, or if aspects of the profile expire or become outdated.</span></span> <span data-ttu-id="91875-194">В этом случае на странице обзора отобразится состояние **требуется действие — Обновить банк и/или налоговый профиль**.</span><span class="sxs-lookup"><span data-stu-id="91875-194">If this happens, your Overview page will show a status of **Action required – Update bank and/or tax profile**.</span></span>

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a><span data-ttu-id="91875-195">Как указать/обновить данные в профиле выплат и налогов?</span><span class="sxs-lookup"><span data-stu-id="91875-195">How do I provide/ update my payout and/ or tax details?</span></span>

<span data-ttu-id="91875-196">Подробные сведения об обновлении платежей и сведений о налогах в центре партнеров см. в статье [Создание банковских и налоговых профилей и управление ими в центре партнеров](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center) .</span><span class="sxs-lookup"><span data-stu-id="91875-196">For detailed information on how to on how to update payment and tax details in Partner Center, see [How to create and manage bank and tax profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span></span>

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a><span data-ttu-id="91875-197">Почему мои регистрации не отображаются при заполнении профиля выплат и налогов?</span><span class="sxs-lookup"><span data-stu-id="91875-197">Why don't I see my enrollments when I go to assign my payout and tax profile?</span></span>

<span data-ttu-id="91875-198">Создавать профили выплат и налогов и управлять ими могут только администраторы программы поощрений для вашего расположения MPN.</span><span class="sxs-lookup"><span data-stu-id="91875-198">Only incentive admins for your MPN location can create or manage payout and tax profiles.</span></span> <span data-ttu-id="91875-199">Возможно, у вас нет необходимых разрешений или вы вошли в учетную запись, у которой нет этих разрешений.</span><span class="sxs-lookup"><span data-stu-id="91875-199">It could be that you don’t have the proper permissions, or that you’re logged in with an account that does not have these permissions.</span></span> <span data-ttu-id="91875-200">Обратитесь к администратору своей организации за разрешением на работу с банковским и налоговым профилями.</span><span class="sxs-lookup"><span data-stu-id="91875-200">Contact your organization administrator to manage permissions for bank and tax.</span></span>

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a><span data-ttu-id="91875-201">Где можно увидеть платежные и налоговые профили для моей организации, которые я могу использовать?</span><span class="sxs-lookup"><span data-stu-id="91875-201">Where can I see the payout and tax profiles for my organization that I can use?</span></span>

<span data-ttu-id="91875-202">Используйте следующую процедуру, чтобы просмотреть профили выплат и налогов.</span><span class="sxs-lookup"><span data-stu-id="91875-202">Use the following procedure to see payout and tax profiles:</span></span>

1. <span data-ttu-id="91875-203">Войдите в Центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="91875-203">Log into Partner Center.</span></span>

2. <span data-ttu-id="91875-204">Нажмите значок шестеренки, чтобы открыть меню **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="91875-204">Select the gear icon to open the **Settings** menu.</span></span>

3. <span data-ttu-id="91875-205">Выберите **Параметры партнера**.</span><span class="sxs-lookup"><span data-stu-id="91875-205">Select **Partner settings**.</span></span>

4. <span data-ttu-id="91875-206">В разделе **Параметры учетной записи** выберите **Выплаты и налоги**, а затем выберите **Профиль для выплат и налогов**.</span><span class="sxs-lookup"><span data-stu-id="91875-206">Under **Account settings**, select **Payout and tax**, and then select **Payout and tax profile**.</span></span> <span data-ttu-id="91875-207">Вы увидите все существующие профили для выплат и налогов с их состоянием и возможностью изменения.</span><span class="sxs-lookup"><span data-stu-id="91875-207">You’ll see all existing payment and tax profiles along with status and ability to edit.</span></span>

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a><span data-ttu-id="91875-208">Моя организация участвует в нескольких поощрениях программ.</span><span class="sxs-lookup"><span data-stu-id="91875-208">My organization is participating in multiple incentive programs.</span></span> <span data-ttu-id="91875-209">Нужно ли предоставлять свой платежный и налоговый профиль несколько раз?</span><span class="sxs-lookup"><span data-stu-id="91875-209">Do I need to provide my payment and tax profile multiple times?</span></span>

<span data-ttu-id="91875-210">Что касается профилей для выплат, как правило, это на ваше усмотрение.</span><span class="sxs-lookup"><span data-stu-id="91875-210">With payment profiles, it’s usually up to you.</span></span> <span data-ttu-id="91875-211">Профили для выплат создаются на уровне организации, что позволяет назначать один и тот же профиль банка нескольким идентификаторам MPN ID и программам поощрений одной организации.</span><span class="sxs-lookup"><span data-stu-id="91875-211">Payment profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="91875-212">В большинстве случаев можно либо повторно использовать существующий профиль, либо создать новый.</span><span class="sxs-lookup"><span data-stu-id="91875-212">In most cases, you can either reuse an existing profile or create a new one.</span></span>

<span data-ttu-id="91875-213">Исключения касаются тех случаев, когда один и тот же профиль банка применяется в разных странах или регионах, так как там могут действовать местные банковские или налоговые правила.</span><span class="sxs-lookup"><span data-stu-id="91875-213">There may be exceptions, however, when applying your bank profile to different countries or regions, as local bank or tax rules may apply.</span></span>

<span data-ttu-id="91875-214">Налоговые профили, созданные для расположения MPN, можно использовать многократно, и когда одно и то же расположение MPN участвует в другой программе поощрения, налоговый профиль заполняется автоматически.</span><span class="sxs-lookup"><span data-stu-id="91875-214">Tax profiles created for an MPN location get reused and automatically populated when the same MPN location participates in other incentive program.</span></span> <span data-ttu-id="91875-215">Но здесь тоже могут быть исключения.</span><span class="sxs-lookup"><span data-stu-id="91875-215">But there can be exceptions.</span></span> <span data-ttu-id="91875-216">Например, согласно правилам выплат в новой программе поощрения может требоваться дополнительная информация для налогового профиля.</span><span class="sxs-lookup"><span data-stu-id="91875-216">For example, the payout rules of a new incentive program may require additional details for the tax profile.</span></span>  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a><span data-ttu-id="91875-217">Я могу войти только с помощью моего @onmicrosoft.com домена.</span><span class="sxs-lookup"><span data-stu-id="91875-217">I am only able to log in with my @onmicrosoft.com domain.</span></span> <span data-ttu-id="91875-218">  Что следует делать?</span><span class="sxs-lookup"><span data-stu-id="91875-218">What should I do?</span></span>

<span data-ttu-id="91875-219">Обратитесь к своему администратору учетной записи, чтобы он добавил дополнительные домены в учетную запись AAD.</span><span class="sxs-lookup"><span data-stu-id="91875-219">Contact your Account administrator to add additional domains to the AAD account.</span></span>
