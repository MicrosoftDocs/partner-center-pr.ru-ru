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
ms.openlocfilehash: 403899b73dda09dded582c94cabe4219ef56c568
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000618"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="8c154-103">Устранение проблем с настройкой учетной записи или обновлением MPN</span><span class="sxs-lookup"><span data-stu-id="8c154-103">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="8c154-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="8c154-104">**Applies to**</span></span>

- <span data-ttu-id="8c154-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="8c154-105">Partner Center</span></span>
 
<span data-ttu-id="8c154-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="8c154-106">**Appropriate roles**</span></span>

- <span data-ttu-id="8c154-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8c154-107">Global admin</span></span>
- <span data-ttu-id="8c154-108">Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="8c154-108">MPN partner admin</span></span> 
 
<span data-ttu-id="8c154-109">Ниже приведены некоторые рекомендации по устранению распространенных проблем, возникающих при настройке учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="8c154-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="8c154-110">Что произойдет, если вы выполняете миграцию из центра членства в партнерах и не можете изменять поля сведений о компании</span><span class="sxs-lookup"><span data-stu-id="8c154-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="8c154-111">В случаях, когда у вашей компании уже есть присутствие в центре партнеров (например, учетная запись CSP), вы увидите экран, предназначенный только для чтения, в котором отображаются все сведения о компании в том виде, в котором она существует в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="8c154-111">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="8c154-112">Вы не можете изменить сведения на этом экране.</span><span class="sxs-lookup"><span data-stu-id="8c154-112">You can't change the details on this screen.</span></span> <span data-ttu-id="8c154-113">Это вызвано проектированием, а не ошибкой.</span><span class="sxs-lookup"><span data-stu-id="8c154-113">This is by design and not an error.</span></span>

<span data-ttu-id="8c154-114">Выберите **принять** и **продолжить** , чтобы продолжить.</span><span class="sxs-lookup"><span data-stu-id="8c154-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="8c154-115">Если ИТ-отдел отключил регистрацию в **центре партнеров**.</span><span class="sxs-lookup"><span data-stu-id="8c154-115">If the IT department has turned off **sign up for Partner Center**.</span></span>


<span data-ttu-id="8c154-116">Это сообщение появляется, потому что вирусные пользователи отключены или вирусная регистрация отключена в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8c154-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="8c154-117">Глобальный администратор учетной записи Azure AD может включить необходимые компоненты, выполнив следующую команду PowerShell:</span><span class="sxs-lookup"><span data-stu-id="8c154-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="8c154-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="8c154-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="8c154-119">Дополнительные сведения см. в статье [самостоятельная регистрация](/azure/active-directory/users-groups-roles/directory-self-service-signup) .</span><span class="sxs-lookup"><span data-stu-id="8c154-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="8c154-120">Вы забыли пароль</span><span class="sxs-lookup"><span data-stu-id="8c154-120">You forgot your password</span></span>

<span data-ttu-id="8c154-121">Если вы забыли пароль, выберите ссылку **не удается получить доступ к своей учетной записи?** на странице входа, чтобы сбросить пароль, или попросите глобального администратора назначить вам новые учетные данные.</span><span class="sxs-lookup"><span data-stu-id="8c154-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="8c154-122">На экране "Расскажите нам о своей компании" появляется ошибка "что пошло не так"</span><span class="sxs-lookup"><span data-stu-id="8c154-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="8c154-123">Это сообщение об ошибке обычно появляется при непреднамеренном использовании специальных символов, пробелов или кода страны в номере телефона вашей компании.</span><span class="sxs-lookup"><span data-stu-id="8c154-123">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="8c154-124">Значение, указанное в поле номер телефона, может содержать не более 10 символов.</span><span class="sxs-lookup"><span data-stu-id="8c154-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="8c154-125">Покупка кредитной карты получит сообщение об ошибке "ваш заказ был отклонен.</span><span class="sxs-lookup"><span data-stu-id="8c154-125">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="8c154-126">Проверьте данные ".</span><span class="sxs-lookup"><span data-stu-id="8c154-126">Please verify your information”</span></span>


<span data-ttu-id="8c154-127">Всегда используйте адрес, соответствующий вашей кредитной карте, а не юридическому субъекту.</span><span class="sxs-lookup"><span data-stu-id="8c154-127">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="8c154-128">Кроме того, убедитесь, что почтовый индекс указан правильно и соответствует адресу, который вы используете.</span><span class="sxs-lookup"><span data-stu-id="8c154-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="8c154-129">Вы хотите переключиться с автономного платежа на интерактивный метод оплаты</span><span class="sxs-lookup"><span data-stu-id="8c154-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="8c154-130">Вам потребуется отменить исходный заказ и выполнить повторное приобретение с использованием предпочтительного метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="8c154-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="8c154-131">Чтобы отменить заказ, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="8c154-131">To cancel an order:</span></span>

1. <span data-ttu-id="8c154-132">Выберите вкладку **предложения членства** на панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="8c154-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="8c154-133">Выберите **отменить заказ**</span><span class="sxs-lookup"><span data-stu-id="8c154-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="8c154-134">Появится окно подтверждения, в котором необходимо подтвердить, чтобы отменить первоначальный порядок.</span><span class="sxs-lookup"><span data-stu-id="8c154-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8c154-135">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8c154-135">Next steps</span></span>

- [<span data-ttu-id="8c154-136">Управление учетной записью Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="8c154-136">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="8c154-137">Как прочитать файл Billing и разведывательную</span><span class="sxs-lookup"><span data-stu-id="8c154-137">How to read your bill and recon file</span></span>](read-your-bill.md)