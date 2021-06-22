---
title: Устранение неполадок при настройке учетной записи центра партнеров или проблем с продлением MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Устранение неполадок при попытке регистрации в центре партнеров. Ответы на проблемы с методами оплаты, забытыми паролями и др.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431750"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="64208-104">Устранение проблем с настройкой учетной записи или обновлением MPN</span><span class="sxs-lookup"><span data-stu-id="64208-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="64208-105">**Соответствующие роли**: глобальный администратор | Администратор партнера MPN</span><span class="sxs-lookup"><span data-stu-id="64208-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="64208-106">Ниже приведены некоторые рекомендации по устранению распространенных проблем, возникающих при настройке учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="64208-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="64208-107">Что произойдет, если вы выполняете миграцию из центра членства в партнерах и не можете изменять поля сведений о компании</span><span class="sxs-lookup"><span data-stu-id="64208-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="64208-108">В случаях, когда у вашей компании уже есть присутствие в центре партнеров (например, учетная запись поставщика облачных решений (CSP)), отображается экран, который доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64208-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="64208-109">На этом экране отображаются все сведения о компании в том виде, в котором она существует в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="64208-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="64208-110">Вы не можете изменить сведения на этом экране.</span><span class="sxs-lookup"><span data-stu-id="64208-110">You can't change the details on this screen.</span></span> <span data-ttu-id="64208-111">Это вызвано проектированием, а не ошибкой.</span><span class="sxs-lookup"><span data-stu-id="64208-111">This is by design and not an error.</span></span>

<span data-ttu-id="64208-112">Чтобы продолжить, выберите **принять**, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="64208-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="64208-113">Если ИТ-отдел отключил регистрацию в **центре партнеров**</span><span class="sxs-lookup"><span data-stu-id="64208-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="64208-114">Это сообщение появляется, потому что вирусные пользователи отключены или в клиенте Azure Active Directory (AD) отключена антивирусная регистрация.</span><span class="sxs-lookup"><span data-stu-id="64208-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="64208-115">Глобальный администратор учетной записи Azure AD может включить необходимые компоненты, выполнив следующую команду PowerShell:</span><span class="sxs-lookup"><span data-stu-id="64208-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="64208-116">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="64208-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="64208-117">Дополнительные сведения см. в статье [самостоятельная регистрация](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="64208-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="64208-118">Вы забыли пароль</span><span class="sxs-lookup"><span data-stu-id="64208-118">You forgot your password</span></span>

<span data-ttu-id="64208-119">Если вы забыли пароль, на странице входа выберите **не удается получить доступ к своей учетной записи?**.</span><span class="sxs-lookup"><span data-stu-id="64208-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="64208-120">Этот параметр позволяет сбросить пароль или попросить глобального администратора назначить вам новые учетные данные.</span><span class="sxs-lookup"><span data-stu-id="64208-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="64208-121">На экране "Расскажите о своей компании" появляется сообщение об ошибке "что-то пошло не так"</span><span class="sxs-lookup"><span data-stu-id="64208-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="64208-122">Это сообщение об ошибке обычно появляется при непреднамеренном использовании специальных символов, пробелов или кода страны в номере телефона вашей компании.</span><span class="sxs-lookup"><span data-stu-id="64208-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="64208-123">Значение, указанное в поле номер телефона, может содержать не более 10 символов.</span><span class="sxs-lookup"><span data-stu-id="64208-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="64208-124">Покупка кредитной карты получит сообщение об ошибке "ваш заказ был отклонен.</span><span class="sxs-lookup"><span data-stu-id="64208-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="64208-125">Проверьте данные ".</span><span class="sxs-lookup"><span data-stu-id="64208-125">Please verify your information”</span></span>


<span data-ttu-id="64208-126">Всегда используйте адрес, соответствующий вашей кредитной карте, а не юридическому субъекту.</span><span class="sxs-lookup"><span data-stu-id="64208-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="64208-127">Кроме того, убедитесь, что почтовый индекс указан правильно и соответствует адресу, который вы используете.</span><span class="sxs-lookup"><span data-stu-id="64208-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="64208-128">Вы хотите переключиться с автономного платежа на интерактивный метод оплаты</span><span class="sxs-lookup"><span data-stu-id="64208-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="64208-129">Вам потребуется отменить исходный заказ и выполнить повторное приобретение с использованием предпочтительного метода оплаты.</span><span class="sxs-lookup"><span data-stu-id="64208-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="64208-130">Чтобы отменить заказ, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="64208-130">To cancel an order:</span></span>

1. <span data-ttu-id="64208-131">На панели мониторинга центра партнеров перейдите на вкладку **предложения членства** .</span><span class="sxs-lookup"><span data-stu-id="64208-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="64208-132">Выберите **отменить заказ**</span><span class="sxs-lookup"><span data-stu-id="64208-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="64208-133">Появится окно подтверждения, в котором необходимо подтвердить, чтобы отменить первоначальный порядок.</span><span class="sxs-lookup"><span data-stu-id="64208-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="64208-134">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="64208-134">Next steps</span></span>

- [<span data-ttu-id="64208-135">Управление учетной записью Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="64208-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="64208-136">Как прочитать файл Billing и разведывательную</span><span class="sxs-lookup"><span data-stu-id="64208-136">How to read your bill and recon file</span></span>](read-your-bill.md)
