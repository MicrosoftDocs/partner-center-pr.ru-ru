---
title: Устранение неполадок при настройке учетной записи центра партнеров или проблем с продлением MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Устранение неполадок при регистрации в центре партнеров
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1d850663224469f24d5d4442e33cc17c1bb6704
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220242"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="eaf24-103">Устранение проблем с настройкой учетной записи или обновлением MPN</span><span class="sxs-lookup"><span data-stu-id="eaf24-103">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="eaf24-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="eaf24-104">**Applies to**</span></span>

- <span data-ttu-id="eaf24-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="eaf24-105">Partner Center</span></span>
 
<span data-ttu-id="eaf24-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="eaf24-106">**Appropriate roles**</span></span>

- <span data-ttu-id="eaf24-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="eaf24-107">Global admin</span></span>
- <span data-ttu-id="eaf24-108">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="eaf24-108">MPN partner admin</span></span> 
 
<span data-ttu-id="eaf24-109">Ниже приведены некоторые рекомендации по устранению распространенных проблем, возникающих при настройке учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="eaf24-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="eaf24-110">Что произойдет, если вы выполняете миграцию из центра членства в партнерах и не можете изменять поля сведений о компании</span><span class="sxs-lookup"><span data-stu-id="eaf24-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="eaf24-111">Это происходит в тех случаях, когда у компании уже есть присутствие в центре партнеров (например, учетная запись CSP). Вы увидите экран, предназначенный только для чтения, в котором отображаются все сведения о компании в том виде, в котором она существует в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="eaf24-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="eaf24-112">Вы не можете изменить сведения на этом экране.</span><span class="sxs-lookup"><span data-stu-id="eaf24-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="eaf24-113">Это вызвано проектированием, а не ошибкой.</span><span class="sxs-lookup"><span data-stu-id="eaf24-113">This is by design and not an error.</span></span>

<span data-ttu-id="eaf24-114">Выберите **принять** и **продолжить** , чтобы продолжить.</span><span class="sxs-lookup"><span data-stu-id="eaf24-114">Select **Accept** and **Continue** to proceed.</span></span>

## <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="eaf24-115">Вы пытаетесь зарегистрироваться или выполнить миграцию из центра членства в партнере, и вы получаете сообщение об ошибке, сообщающее, что ИТ-отдел отключил **регистрацию в центре партнеров**.</span><span class="sxs-lookup"><span data-stu-id="eaf24-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="eaf24-116">Это сообщение появляется, потому что вирусные пользователи отключены или вирусная регистрация отключена в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eaf24-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="eaf24-117">Глобальный администратор учетной записи Azure AD может включить необходимые компоненты, выполнив следующую команду PowerShell:</span><span class="sxs-lookup"><span data-stu-id="eaf24-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="eaf24-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="eaf24-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="eaf24-119">Дополнительные сведения см. в статье [самостоятельная регистрация](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup) .</span><span class="sxs-lookup"><span data-stu-id="eaf24-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="eaf24-120">Вы забыли пароль</span><span class="sxs-lookup"><span data-stu-id="eaf24-120">You forgot your password</span></span>

<span data-ttu-id="eaf24-121">Если вы забыли пароль, выберите ссылку **не удается получить доступ к своей учетной записи?** на странице входа, чтобы сбросить пароль, или попросите глобального администратора назначить вам новые учетные данные.</span><span class="sxs-lookup"><span data-stu-id="eaf24-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="eaf24-122">На экране "Расскажите нам о своей компании" появляется ошибка "что пошло не так"</span><span class="sxs-lookup"><span data-stu-id="eaf24-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="eaf24-123">Обычно это происходит при случайном использовании специальных символов, пробелов или кода страны в номере телефона вашей компании.</span><span class="sxs-lookup"><span data-stu-id="eaf24-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="eaf24-124">Значение, указанное в поле номер телефона, может содержать не более 10 символов.</span><span class="sxs-lookup"><span data-stu-id="eaf24-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

## <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="eaf24-125">Вы пытаетесь выполнить покупку с помощью кредитной карты, но вы получаете сообщение об ошибке "ваш заказ отклонен.</span><span class="sxs-lookup"><span data-stu-id="eaf24-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="eaf24-126">Проверьте данные ".</span><span class="sxs-lookup"><span data-stu-id="eaf24-126">Please verify your information”</span></span>

<span data-ttu-id="eaf24-127">Всегда следует вставлять адрес, соответствующий вашей кредитной карте, а не соответствующим юридическим субъектам.</span><span class="sxs-lookup"><span data-stu-id="eaf24-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="eaf24-128">Кроме того, убедитесь, что почтовый индекс указан правильно и соответствует адресу, который вы используете.</span><span class="sxs-lookup"><span data-stu-id="eaf24-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="eaf24-129">Вы хотите переключиться с автономного платежа на интерактивный метод оплаты</span><span class="sxs-lookup"><span data-stu-id="eaf24-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="eaf24-130">Вам потребуется отменить исходный заказ и выполнить повторное приобретение с использованием предпочтительного метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="eaf24-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="eaf24-131">Чтобы отменить заказ, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="eaf24-131">To cancel an order:</span></span>

1. <span data-ttu-id="eaf24-132">Выберите вкладку **предложения членства** на панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="eaf24-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="eaf24-133">Выберите **отменить заказ**</span><span class="sxs-lookup"><span data-stu-id="eaf24-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="eaf24-134">Появится окно подтверждения, в котором необходимо подтвердить, чтобы отменить первоначальный порядок.</span><span class="sxs-lookup"><span data-stu-id="eaf24-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
