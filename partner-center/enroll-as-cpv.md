---
title: Регистрация в качестве поставщика панелей управления
description: Узнайте, как зарегистрироваться в качестве поставщика панели управления (КПВ) в центре партнеров, чтобы вы могли лучше интегрировать партнерские системы CSP с API-интерфейсами центра партнеров.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031897"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="2660f-103">Регистрация в качестве поставщика панели управления, что поспособствует интеграции систем партнеров в рамках CSP с помощью API-интерфейсов Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="2660f-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="2660f-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="2660f-104">**Applies to**</span></span>

- <span data-ttu-id="2660f-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="2660f-105">Partner Center</span></span>

<span data-ttu-id="2660f-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="2660f-106">**Appropriate roles**</span></span>

- <span data-ttu-id="2660f-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2660f-107">Global admin</span></span>

<span data-ttu-id="2660f-108">Поставщик панели управления (КПВ) — это независимый поставщик программного обеспечения, который разрабатывает приложения для партнеров поставщика облачных решений (CSP), позволяя им интегрировать свои системы с API-интерфейсами центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2660f-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="2660f-109">Поставщик панели управления не является партнером CSP с прямым доступом к панели мониторинга центра партнеров или к API-интерфейсам центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2660f-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="2660f-110">Есть ли у вас текущий поставщик панели управления (КПВ) или новый КПВ, желающий работать с партнерами Майкрософт, Майкрософт теперь требует регистрации в центре партнеров для регистрации приложений и поддержки партнеров поставщиков облачных решений.</span><span class="sxs-lookup"><span data-stu-id="2660f-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="2660f-111">Чтобы создать учетную запись, партнер КПВ может использовать существующий клиент-партнер CSP или существующий клиент КПВ или создать новый клиент в рамках процесса адаптации.</span><span class="sxs-lookup"><span data-stu-id="2660f-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="2660f-112">Если партнер КПВ выбирает использование существующего клиента CSP, ему потребуется создать отдельные приложения с несколькими клиентами и зарегистрировать их в центре партнеров для действий КПВ.</span><span class="sxs-lookup"><span data-stu-id="2660f-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="2660f-113">Приложение не может быть зарегистрировано как приложение CSP и КПВ.</span><span class="sxs-lookup"><span data-stu-id="2660f-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="2660f-114">После регистрации в центре партнеров и регистрации приложений вы получите доступ к API-интерфейсам центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2660f-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="2660f-115">Корпорация Майкрософт свяжется с вами через уведомление центра партнеров со сведениями о песочнице.</span><span class="sxs-lookup"><span data-stu-id="2660f-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="2660f-116">Если у вас уже есть учетная запись "песочница", продолжайте ее использовать.</span><span class="sxs-lookup"><span data-stu-id="2660f-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="2660f-117">Вам не потребуется новая песочница.</span><span class="sxs-lookup"><span data-stu-id="2660f-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="2660f-118">Ознакомьтесь с [соглашением для поставщиков панели управления Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="2660f-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="2660f-119">Работа в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="2660f-119">Working in Partner Center</span></span>
<span data-ttu-id="2660f-120">После регистрации в центре партнеров КПВ опыта и принятия соглашения КПВ вы можете:</span><span class="sxs-lookup"><span data-stu-id="2660f-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="2660f-121">Управление приложениями с несколькими клиентами (Добавление приложений для портал Azure, регистрация и Отмена регистрации приложений в центре партнеров).</span><span class="sxs-lookup"><span data-stu-id="2660f-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="2660f-122">КПВС должны зарегистрировать свои приложения в центре партнеров, чтобы получить разрешения для API-интерфейсов центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2660f-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="2660f-123">Добавление приложений только на портал Azure не дает приложениям CPV право на использование интерфейсов API Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2660f-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="2660f-124">Просмотр профиля CPV и управление им.</span><span class="sxs-lookup"><span data-stu-id="2660f-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="2660f-125">Просматривать пользователей, которым требуется доступ к возможностям CPV, и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="2660f-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="2660f-126">Глобальный администратор является единственной ролью, которую может иметь КПВ.</span><span class="sxs-lookup"><span data-stu-id="2660f-126">Global admin is the only role a CPV can have.</span></span>


