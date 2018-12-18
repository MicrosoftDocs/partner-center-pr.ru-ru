---
title: Регистрация в центре партнеров в качестве поставщика панель управления | Центр партнеров
ms.topic: article
ms.date: 12/11/2018
Description: How to enroll in Partner Center as a Control Panel Vendor
author: labrenne
ms.author: labrenne
keywords: Поставщик панели управления, регистрация CPV приложений, управление приложениями CPV
ms.localizationpriority: medium
ms.openlocfilehash: 47c404c7620d66cecb1dcb1572a7c8ac85d17261
ms.sourcegitcommit: 98bcceea95b8d9ee5d386456a723f0b8da3ebd58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2018
ms.locfileid: "8972131"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="c063b-103">Регистрация в центре партнеров в качестве поставщика панели управления</span><span class="sxs-lookup"><span data-stu-id="c063b-103">Enroll in Partner Center as a Control Panel Vendor</span></span>

**<span data-ttu-id="c063b-104">Область применения</span><span class="sxs-lookup"><span data-stu-id="c063b-104">Applies to</span></span>**

- <span data-ttu-id="c063b-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="c063b-105">Partner Center</span></span>

<span data-ttu-id="c063b-106">Поставщик панели управления (CPV) — это независимый поставщик программного обеспечения, Разработка приложения для использования партнерами поставщиков облачных решений (CSP), чтобы включить их для интеграции систем с помощью API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c063b-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="c063b-107">Панель управления поставщика не API центра партнеров или партнер CSP, прямой доступ к информационной панели центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c063b-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="c063b-108">Указывает, нужно ли вам текущего поставщика панели управления (CPV) или новый CPV, кто хочет работать с партнерами корпорации Майкрософт, корпорация Майкрософт теперь требует регистрация в центре партнеров для регистрации вашего приложения и поддерживают поставщиков облачных решений партнеров.</span><span class="sxs-lookup"><span data-stu-id="c063b-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="c063b-109">Создать учетную запись, партнер CPV можно использовать имеющийся клиент партнеров CSP, или существующему клиенту CPV или можно создать новый клиент как часть процесса адаптации.</span><span class="sxs-lookup"><span data-stu-id="c063b-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="c063b-110">Если партнер CPV решает использовать имеющийся клиент CSP, они потребуется создать отдельный мультитенантные приложения и зарегистрировать их в центре партнеров для CPV действий.</span><span class="sxs-lookup"><span data-stu-id="c063b-110">If the CPV partner chooses to use the existing CSP tenant, then they’ll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="c063b-111">Приложения не могут зарегистрироваться в качестве CSP и CPV приложения.</span><span class="sxs-lookup"><span data-stu-id="c063b-111">An application can’t be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="c063b-112">После регистрации в центре партнеров и зарегистрированных приложений, вы получите доступ к API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c063b-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="c063b-113">Корпорация Майкрософт свяжется с вами через Центр партнеров уведомление с данными вашей песочницы.</span><span class="sxs-lookup"><span data-stu-id="c063b-113">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="c063b-114">Если, тем не менее, вас еще нет учетной записи песочницы, продолжить использовать его.</span><span class="sxs-lookup"><span data-stu-id="c063b-114">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="c063b-115">Не требуется, новый "песочнице".</span><span class="sxs-lookup"><span data-stu-id="c063b-115">You won’t need a new sandbox.</span></span>   


## <a name="working-in-partner-center"></a><span data-ttu-id="c063b-116">Работа в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="c063b-116">Working in Partner Center</span></span>
<span data-ttu-id="c063b-117">После регистрации на расстоянии CPV центра партнеров и приняты CPV соглашений, которые вы можете:</span><span class="sxs-lookup"><span data-stu-id="c063b-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="c063b-118">Управление мультитенантные приложения (Добавление приложений на портале Azure, регистрация и Отмена регистрации приложения в центре партнеров).</span><span class="sxs-lookup"><span data-stu-id="c063b-118">Manage multi-tenant applications (add applications to Azure portal, register and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="c063b-119">CPVs необходимо зарегистрировать свои приложения в центре партнеров, чтобы получить авторизованы для API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c063b-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="c063b-120">Добавление приложений на портале Azure само по себе не предоставляет авторизацию приложений CPV по API центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="c063b-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="c063b-121">Просмотр и управлять профилем CPV</span><span class="sxs-lookup"><span data-stu-id="c063b-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="c063b-122">Просмотр и управление пользователям, которым требуется доступ к возможностям CPV.</span><span class="sxs-lookup"><span data-stu-id="c063b-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="c063b-123">Только роль, которую может иметь CPV — глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="c063b-123">The only role a CPV can have is global admin.</span></span>


