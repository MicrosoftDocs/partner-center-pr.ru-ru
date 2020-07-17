---
title: Проверка работоспособности службы для клиента
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как использовать центр партнеров для проверки работоспособности службы для клиента при возникновении проблем со службой.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 11ec4cfcfc9326c1e9d6598dce528410c0e02542
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435483"
---
# <a name="check-service-health-for-a-customer-reporting-a-potential-service-problem-or-outage"></a><span data-ttu-id="1dd60-103">Проверка работоспособности службы для клиента, который сообщает о возможной проблеме или сбое службы</span><span class="sxs-lookup"><span data-stu-id="1dd60-103">Check service health for a customer reporting a potential service problem or outage</span></span>

<span data-ttu-id="1dd60-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="1dd60-104">**Applies to**</span></span>

- <span data-ttu-id="1dd60-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="1dd60-105">Partner Center</span></span>

<span data-ttu-id="1dd60-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="1dd60-106">**Appropriate roles**</span></span>

- <span data-ttu-id="1dd60-107">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="1dd60-107">Admin agent</span></span>
- <span data-ttu-id="1dd60-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1dd60-108">Global admin</span></span>
- <span data-ttu-id="1dd60-109">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="1dd60-109">Helpdesk agent</span></span>
- <span data-ttu-id="1dd60-110">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="1dd60-110">Sales agent</span></span>

<span data-ttu-id="1dd60-111">В числе первых действий, которые можно предпринять, если клиент испытывает проблемы с использованием службы, является проверка ее работоспособности.</span><span class="sxs-lookup"><span data-stu-id="1dd60-111">One of the first things you can do when a customer is experiencing problems with a service is to check the service health.</span></span> 

## <a name="check-service-health"></a><span data-ttu-id="1dd60-112">Проверка работоспособности службы</span><span class="sxs-lookup"><span data-stu-id="1dd60-112">Check service health</span></span>

1. <span data-ttu-id="1dd60-113">Выберите **клиента** , у которого возникла эта неполадка, из **списка клиентов**.</span><span class="sxs-lookup"><span data-stu-id="1dd60-113">Select the **Customer** that is having the issue from the **Customer list**.</span></span>

2. <span data-ttu-id="1dd60-114">В меню слева выберите **Управление службами** .</span><span class="sxs-lookup"><span data-stu-id="1dd60-114">Select **Service management** from the left menu.</span></span> <span data-ttu-id="1dd60-115">В нем будут перечислены службы, подготовленные для клиента, и сведения о работоспособности службы для каждого из них.</span><span class="sxs-lookup"><span data-stu-id="1dd60-115">This will list the services provisioned for the customer and the service health for each.</span></span> <span data-ttu-id="1dd60-116">Партнеры могут щелкнуть службу, которой они интересуют, чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="1dd60-116">Partners can click the service they are interested in to get more information.</span></span> 

>[!NOTE] 
> <span data-ttu-id="1dd60-117">Ссылки на страницы "работоспособность службы" на страницах **управления службами** принимают партнера в центре администрирования M365 или портал Azure в качестве **полномочного администратора**. Когда партнер получает доступ к любому назначению, он может переходить на страницу работоспособности службы на любом портале, чтобы получить дополнительные сведения о сбоях.</span><span class="sxs-lookup"><span data-stu-id="1dd60-117">Service health links on the **Service management** pages will take the partner to either the M365 admin center or the Azure portal as **delegated admin**. Once the partner gets to either destination, the partner can navigate to the service health pages in either portal for more details about the outage.</span></span>
 
<span data-ttu-id="1dd60-118">Во время простоя службы Майкрософт постоянно сообщает о ходе устранения проблемы.</span><span class="sxs-lookup"><span data-stu-id="1dd60-118">During a service outage, Microsoft provides regular updates as we work to address the problem.</span></span> <span data-ttu-id="1dd60-119">Эти уведомления также отображаются либо в портал Microsoft Azure, либо в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1dd60-119">These notifications are also displayed on either the Microsoft Azure portal or the Microsoft 365 admin Center.</span></span>

<span data-ttu-id="1dd60-120">Если проблема повторяется после завершения сбоя службы, отправьте запрос на обслуживание.</span><span class="sxs-lookup"><span data-stu-id="1dd60-120">If the problem persists after the end of the service outage, submit a service request.</span></span> <span data-ttu-id="1dd60-121">См. раздел [Сообщение о проблемах от имени клиента](report-problems-on-behalf-of-a-customer.md).</span><span class="sxs-lookup"><span data-stu-id="1dd60-121">See [Report problems on behalf of a customer](report-problems-on-behalf-of-a-customer.md).</span></span>

<span data-ttu-id="1dd60-122">Microsoft 365 и Microsoft Azure каждый предоставляют [интерфейсы API, которые могут использоваться партнерами для получения сведений о работоспособности службы в режиме реального времени](get-automated-service-notifications-with-our-apis.md), связи с центром сообщений и плановых событий обслуживания.</span><span class="sxs-lookup"><span data-stu-id="1dd60-122">Microsoft 365 and Microsoft Azure each provide [APIs that partners can use to retrieve real-time service health](get-automated-service-notifications-with-our-apis.md), message center communications, and planned maintenance events.</span></span>

 

