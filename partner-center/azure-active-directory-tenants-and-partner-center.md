---
title: "Клиенты Azure Active Directory и Центр партнеров | Центр партнеров"
description: "Чтобы создать учетную запись Центра партнеров, у вашей компании должен быть клиент Azure Active Directory (Azure AD). Azure AD— это облачная служба каталогов Майкрософт, обеспечивающая управление удостоверениями."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="45df5-104">Клиенты Azure Active Directory и Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="45df5-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="45df5-105">Область применения</span><span class="sxs-lookup"><span data-stu-id="45df5-105">Applies to</span></span>**

-  <span data-ttu-id="45df5-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="45df5-106">Partner Center</span></span>

## <a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="45df5-107">Зачем нужен клиент Azure AD?</span><span class="sxs-lookup"><span data-stu-id="45df5-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="45df5-108">Нам необходимо связать клиент Azure AD вашей организации с вашей новой учетной записью Центра партнеров, чтобы ваши пользователей клиента могли осуществлять вход в Центр партнеров, используя свои имена пользователей и пароли Azure AD (учетная запись Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="45df5-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="45df5-109">Если у вашей компании уже есть клиент Azure AD, вы можете связать его со своей учетной записью Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="45df5-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

>**<span data-ttu-id="45df5-110">Примечание.</span><span class="sxs-lookup"><span data-stu-id="45df5-110">Note</span></span>**<br> <span data-ttu-id="45df5-111">Прежде чем использовать имеющийся клиент Azure AD, подумайте о том, какому количеству пользователей в клиенте необходимо будет работать в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="45df5-111">Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="45df5-112">Если у вас есть пользователи в клиенте, которым не нужно будет работать в Центре партнеров, рассмотрите возможность создания нового клиента только для тех пользователей, которым будет необходимо работать в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="45df5-112">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="45df5-113">Если у вашей компании еще нет клиента Azure AD, его можно создать бесплатно в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="45df5-113">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="45df5-114">Выберите **Создать новый клиент** на странице **Вход в Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="45df5-114">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="45df5-115">Не уверены, если ли уже в вашей компании клиент Azure AD?</span><span class="sxs-lookup"><span data-stu-id="45df5-115">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="45df5-116">Если вы не знаете, есть ли у вашей организации клиент Azure AD, выполните следующие действия для проверки.</span><span class="sxs-lookup"><span data-stu-id="45df5-116">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="45df5-117">Примечание. Если у вас есть действующая подписка на Microsoft Azure или Office 365, это значит, что вы уже создали клиент Azure AD.</span><span class="sxs-lookup"><span data-stu-id="45df5-117">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="45df5-118">Войдите на портал администрирования Azure по адресу https://ms.portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="45df5-118">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="45df5-119">Выберите в меню пункт "Azure Active Directory", а затем пункт "Доменные имена".</span><span class="sxs-lookup"><span data-stu-id="45df5-119">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="45df5-120">Если у вас уже есть клиент, отобразится имя вашего домена.</span><span class="sxs-lookup"><span data-stu-id="45df5-120">If you already have a tenant, your domain name will be listed.</span></span>

### <a name="using-an-existing-tenant"></a><span data-ttu-id="45df5-121">Используете уже имеющийся клиент?</span><span class="sxs-lookup"><span data-stu-id="45df5-121">Using an existing tenant?</span></span>

<span data-ttu-id="45df5-122">Если вы хотите использовать имеющийся клиент Azure AD, но не можете войти в систему, найдите сценарий на схеме ниже, который наилучшим образом соответствует вашей ситуации, и выполните рекомендуемые действия.</span><span class="sxs-lookup"><span data-stu-id="45df5-122">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![У вас есть клиент Azure AD или его требуется создать?](images/onboardingAADFlow.png)

<span data-ttu-id="45df5-124">Дополнительные сведения о добавлении доменов в Azure AD см. в разделе [Добавление или связывание домена в Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="45df5-124">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="45df5-125">Сведения о Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="45df5-125">About Microsoft Azure</span></span>

<span data-ttu-id="45df5-126">Microsoft Azure— это платформа общедоступного облака, которую компании могут использовать для разработки, развертывания и администрирования приложений в глобальной сети центров обработки данных под управлением Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="45df5-126">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="45df5-127">Компании используют Azure для создания виртуальной ИТ-инфраструктуры с виртуальными функциями или виртуальных служб вместо физических компьютеров.</span><span class="sxs-lookup"><span data-stu-id="45df5-127">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="45df5-128">При покупке подписки на Azure вы фактически арендуете специальное безопасное пространство в общедоступном облаке Azure, что почти не отличается от аренды этажа в офисном здании для размещения физического бизнеса вашей компании.</span><span class="sxs-lookup"><span data-stu-id="45df5-128">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="45df5-129">Для владельца офисного здания ваша компания является арендатором (или клиентом).</span><span class="sxs-lookup"><span data-stu-id="45df5-129">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="45df5-130">Клиент Azure AD— это специальное и изолированное виртуальное представление вашей компании в общедоступном облаке Azure, создаваемое для вас при оформлении вами подписки на облачную службу Майкрософт, например Azure, Microsoft Intune или Office 365.</span><span class="sxs-lookup"><span data-stu-id="45df5-130">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="45df5-131">В вашем клиенте размещаются ваши пользователи Azure AD и сведения о них: пароли, данные профиля, разрешения и т. д.</span><span class="sxs-lookup"><span data-stu-id="45df5-131">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="45df5-132">Клиент также содержит группы, приложения и другие сведения, относящиеся к компании и ее безопасности.</span><span class="sxs-lookup"><span data-stu-id="45df5-132">The tenant also contains groups,applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="45df5-133">Подробнее об Azure AD см. в разделе [документации по Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="45df5-133">To learn more about Azure AD, see the [Azure Active Directory Documentation](https://docs.microsoft.com/ azure/active-directory/).</span></span> 