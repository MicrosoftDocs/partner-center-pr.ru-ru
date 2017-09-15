---
title: Azure Active Directory tenants and Partner Center | Partner Center
description: "To create a Partner Center account, your company must have an Azure Active Directory (Azure AD) tenant. Azure AD is Microsoft’s cloud-based directory and identity management service."
author: labrenne
robots: 
ms.openlocfilehash: ab16d167fc978d76c96fc6ef7c1b8eabe26a1ad5
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="088c0-104">Azure Active Directory tenants and Partner Center</span><span class="sxs-lookup"><span data-stu-id="088c0-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="088c0-105">Applies to</span><span class="sxs-lookup"><span data-stu-id="088c0-105">Applies to</span></span>**

-  <span data-ttu-id="088c0-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="088c0-106">Partner Center</span></span>

#<a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="088c0-107">Why you need an Azure AD tenant</span><span class="sxs-lookup"><span data-stu-id="088c0-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="088c0-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span><span class="sxs-lookup"><span data-stu-id="088c0-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="088c0-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="088c0-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

<span data-ttu-id="088c0-110">**Примечание.** Прежде чем использовать имеющийся клиент Azure AD, подумайте о том, какому количеству пользователей в клиенте необходимо будет работать в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="088c0-110">**Note** Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="088c0-111">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="088c0-111">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="088c0-112">Если у вашей компании еще нет клиента Azure AD, его можно создать бесплатно в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="088c0-112">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="088c0-113">Выберите **Создать новый клиент** на странице **Вход в Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="088c0-113">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 


## <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="088c0-114">Не уверены, если ли уже в вашей компании клиент Azure AD?</span><span class="sxs-lookup"><span data-stu-id="088c0-114">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="088c0-115">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span><span class="sxs-lookup"><span data-stu-id="088c0-115">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="088c0-116">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span><span class="sxs-lookup"><span data-stu-id="088c0-116">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="088c0-117">Sign in to the Azure admin portal at https://ms.portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="088c0-117">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="088c0-118">Select Azure Active Directory from the menu and then select Domain Names.</span><span class="sxs-lookup"><span data-stu-id="088c0-118">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="088c0-119">Если у вас уже есть клиент, отобразится имя вашего домена.</span><span class="sxs-lookup"><span data-stu-id="088c0-119">If you already have a tenant, your domain name will be listed.</span></span>

##<a name="using-an-existing-tenant"></a><span data-ttu-id="088c0-120">Используете уже имеющийся клиент?</span><span class="sxs-lookup"><span data-stu-id="088c0-120">Using an existing tenant</span></span>

<span data-ttu-id="088c0-121">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span><span class="sxs-lookup"><span data-stu-id="088c0-121">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![У вас есть клиент Azure AD или его требуется создать?](images/onboardingAADFlow.png)

<span data-ttu-id="088c0-123">Дополнительные сведения о добавлении доменов в Azure AD см. в разделе [Добавление или связывание домена в Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="088c0-123">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

# <a name="about-microsoft-azure"></a><span data-ttu-id="088c0-124">Сведения о Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="088c0-124">About Microsoft Azure</span></span>

<span data-ttu-id="088c0-125">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span><span class="sxs-lookup"><span data-stu-id="088c0-125">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="088c0-126">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span><span class="sxs-lookup"><span data-stu-id="088c0-126">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="088c0-127">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span><span class="sxs-lookup"><span data-stu-id="088c0-127">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="088c0-128">To the office building’s owner, your company is a tenant.</span><span class="sxs-lookup"><span data-stu-id="088c0-128">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="088c0-129">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span><span class="sxs-lookup"><span data-stu-id="088c0-129">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="088c0-130">В вашем клиенте размещаются ваши пользователи Azure AD и сведения о них: пароли, данные профиля, разрешения и т. д.</span><span class="sxs-lookup"><span data-stu-id="088c0-130">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="088c0-131">Клиент также содержит группы, приложения и другие сведения, относящиеся к компании и ее безопасности.</span><span class="sxs-lookup"><span data-stu-id="088c0-131">The tenant also contains groups, applications, and other information pertaining to a company and its security.</span></span> 
