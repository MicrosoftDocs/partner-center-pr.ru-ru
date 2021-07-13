---
title: Подключение рабочей учетной записи для доступа к Центру партнеров
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Создайте рабочую учетную запись, которая свяжет вашу компанию с учетной записью Центра партнеров. Это позволит предоставить доступ к Центру партнеров сотрудникам вашей организации.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 6/17/2021
ms.openlocfilehash: 69aa45de55a4356eaab1bcd4cd309feb14de9f6e
ms.sourcegitcommit: 0410e2a3f91b7e6b592cc47e7af1dfbe468c7881
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112318067"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="974da-104">Создайте рабочую учетную запись для связи вашей компании с учетной записью Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="974da-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="974da-105">**Соответствующие роли:** глобальный администратор | администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="974da-105">**Appropriate roles**: Global admin | User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="974da-106">Зачем нужна рабочая учетная запись?</span><span class="sxs-lookup"><span data-stu-id="974da-106">Why you need a work account</span></span>

<span data-ttu-id="974da-107">Майкрософт требует связать с новой учетной записью Центра партнеров рабочую учетную запись вашей компании.</span><span class="sxs-lookup"><span data-stu-id="974da-107">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="974da-108">Эта ссылка позволяет пользователям вашей учетной записи входить в Центр партнеров с именами пользователей и паролями рабочей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="974da-108">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="974da-109">Адрес электронной почты рабочей учетной записи</span><span class="sxs-lookup"><span data-stu-id="974da-109">The work account email address</span></span>

<span data-ttu-id="974da-110">Адрес электронной почты рабочей учетной записи (рабочий адрес электронной почты) — это адрес электронной почты, предоставленный вашей компанией.</span><span class="sxs-lookup"><span data-stu-id="974da-110">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="974da-111">Адрес электронной почты рабочей учетной записи обычно имеет формат `you@yourcompany.com`.</span><span class="sxs-lookup"><span data-stu-id="974da-111">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="974da-112">Личные адреса электронной почты, такие как Hotmail, Gmail или Yahoo, не являются рабочими и их нельзя использовать для учетной записи Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="974da-112">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="974da-113">Если у вас есть несколько действующих рабочих адресов электронной почты, используйте тот, который связан с центральным офисом, а не с региональным подразделением. Например, используйте адрес электронной почты `contoso.com`, а не `contoso.uk`.</span><span class="sxs-lookup"><span data-stu-id="974da-113">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="974da-114">Прежде чем использовать существующую рабочую учетную запись, подумайте о том, какому количеству пользователей в рабочей учетной записи потребуется доступ к Центру партнеров.</span><span class="sxs-lookup"><span data-stu-id="974da-114">Before you use an existing work account, think about how many users in the work account will need to access Partner Center.</span></span> <span data-ttu-id="974da-115">Если в рабочей учетной записи есть пользователи, которым не нужен доступ к Центру партнеров, создайте новую учетную запись только для тех пользователей, которым потребуется такой доступ.</span><span class="sxs-lookup"><span data-stu-id="974da-115">If you have users in the work account who won't need access to Partner Center, consider creating a new account for only those users who will need Partner Center access.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="974da-116">Не уверены, есть ли уже в вашей компании рабочая учетная запись?</span><span class="sxs-lookup"><span data-stu-id="974da-116">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="974da-117">Если вы не знаете, есть ли у вашей компании рабочая учетная запись, выполните следующие действия для проверки.</span><span class="sxs-lookup"><span data-stu-id="974da-117">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="974da-118">Если у вас есть действующая подписка на Microsoft Azure или Office 365, это значит, что вы уже создали рабочую учетную запись.</span><span class="sxs-lookup"><span data-stu-id="974da-118">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="974da-119">Войдите на [портал Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="974da-119">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="974da-120">Выберите "Azure Active Directory" в меню навигации и затем выберите **Пользовательские доменные имена**.</span><span class="sxs-lookup"><span data-stu-id="974da-120">Select Azure Active Directory from the navigation menu and select **Custom Domain Names**.</span></span>

3. <span data-ttu-id="974da-121">Если у вас уже есть рабочая учетная запись, отобразится имя вашего домена.</span><span class="sxs-lookup"><span data-stu-id="974da-121">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="974da-122">Если у вашей компании еще нет рабочей учетной записи, ее можно создать в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="974da-122">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="974da-123">На приведенной ниже схеме представлены пошаговые инструкции для нескольких типичных сценариев:</span><span class="sxs-lookup"><span data-stu-id="974da-123">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="974da-124">определение наличия рабочей учетной записи;</span><span class="sxs-lookup"><span data-stu-id="974da-124">determine if you have a work account</span></span>
- <span data-ttu-id="974da-125">определение способа входа в рабочую учетную запись;</span><span class="sxs-lookup"><span data-stu-id="974da-125">determine how to sign into your work account</span></span>
- <span data-ttu-id="974da-126">определение необходимости создания новой рабочей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="974da-126">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="У вас есть рабочая учетная запись или ее необходимо создать?":::

<span data-ttu-id="974da-128">Дополнительные сведения о добавлении доменов в Azure AD см. в [этой статье](/azure/active-directory/active-directory-add-domain).</span><span class="sxs-lookup"><span data-stu-id="974da-128">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="974da-129">Сведения о Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="974da-129">About Microsoft Azure</span></span>

<span data-ttu-id="974da-130">Microsoft Azure — это платформа общедоступного облака, которую компании могут использовать для разработки, развертывания и администрирования приложений в глобальной сети центров обработки данных под управлением Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="974da-130">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="974da-131">Компании используют Azure для создания виртуальной ИТ-инфраструктуры с виртуальными функциями или службами вместо физических компьютеров.</span><span class="sxs-lookup"><span data-stu-id="974da-131">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="974da-132">При покупке подписки на Azure вы фактически арендуете специальное безопасное пространство в общедоступном облаке Azure, что почти не отличается от аренды этажа в офисном здании для размещения физического бизнеса вашей компании.</span><span class="sxs-lookup"><span data-stu-id="974da-132">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="974da-133">Для владельца офисного здания ваша компания является арендатором (или клиентом).</span><span class="sxs-lookup"><span data-stu-id="974da-133">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="974da-134">Рабочая учетная запись Azure — это специальное и изолированное виртуальное представление вашей компании в общедоступном облаке Azure, создаваемое для вас при оформлении вами подписки на облачную службу Майкрософт, например Azure, Microsoft Intune или Office 365.</span><span class="sxs-lookup"><span data-stu-id="974da-134">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="974da-135">В вашей рабочей учетной записи размещаются ваши пользователи Azure AD и сведения о них: пароли, данные профиля, разрешения и т. д.</span><span class="sxs-lookup"><span data-stu-id="974da-135">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="974da-136">Рабочая учетная запись также содержит группы, приложения и другие сведения, относящиеся к компании и ее безопасности.</span><span class="sxs-lookup"><span data-stu-id="974da-136">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>

## <a name="next-steps"></a><span data-ttu-id="974da-137">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="974da-137">Next steps</span></span>

- [<span data-ttu-id="974da-138">Управление учетной записью Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="974da-138">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="974da-139">Отслеживание состояния проверки</span><span class="sxs-lookup"><span data-stu-id="974da-139">Track verification status</span></span>](verification-responses.md)
