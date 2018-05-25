---
title: Уведомления об операциях криптомайнинга на панели мониторинга Центра партнеров | Панель мониторинга Центра партнеров
description: Уведомление о потенциальных операциях криптомайнинга.
author: v-petand
Keywords: crypto-mining, cryptocurrency mining, security
robots: noindex, nofollow
ms.openlocfilehash: 1e7e695ec19600fd1f32138982c8f609db168cc7
ms.sourcegitcommit: 2d3203dd5e2653af031a8009aa3b999a454acef5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2018
---
# <a name="partner-dashboard-notification-for-cryptocurrency-mining-activity"></a><span data-ttu-id="f0272-103">Уведомление об операциях майнинга криптовалют на панели мониторинга Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="f0272-103">Partner Dashboard notification for cryptocurrency mining activity</span></span>

**<span data-ttu-id="f0272-104">Область применения</span><span class="sxs-lookup"><span data-stu-id="f0272-104">Applies to</span></span>**

-  <span data-ttu-id="f0272-105">Панель мониторинга Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="f0272-105">Partner Dashboard</span></span>
-  <span data-ttu-id="f0272-106">Партнеры CSP</span><span class="sxs-lookup"><span data-stu-id="f0272-106">CSP partners</span></span>

<span data-ttu-id="f0272-107">Возможно, вы уже видели уведомление о майнинге криптовалют на панели мониторинга Центра партнеров:</span><span class="sxs-lookup"><span data-stu-id="f0272-107">You may have received the following Partner Dashboard notification about cryptocurrency mining:</span></span>
 
![](images/crypto1.png)

<span data-ttu-id="f0272-108">Цель данного уведомления — сообщить о том, что в течение прошлой недели были обнаружены попытки майнинга криптовалют в одной или нескольких подписках Azure.</span><span class="sxs-lookup"><span data-stu-id="f0272-108">The purpose of this notification is to inform you that we've detected cryptocurrency mining on one or more of your Azure subscriptions within the past week.</span></span> <span data-ttu-id="f0272-109">Майнинг криптовалют не всегда указывает на мошенничество.</span><span class="sxs-lookup"><span data-stu-id="f0272-109">Cryptocurrency mining does not necessarily equal fraudulent activity.</span></span> <span data-ttu-id="f0272-110">Тем не менее, это нетипичная ситуация, поскольку затраты на майнинг криптовалют в Azure, как правило, превышают потенциальные финансовые выгоды.</span><span class="sxs-lookup"><span data-stu-id="f0272-110">However, it's unusual because the cost of running cryptocurrency mining in Azure tends to outweigh any potential financial rewards.</span></span> <span data-ttu-id="f0272-111">Чтобы защитить себя и своих клиентов от финансового мошенничества, рекомендуется принять следующие меры:</span><span class="sxs-lookup"><span data-stu-id="f0272-111">To protect against financial fraud that may impact you or your customer, consider the following steps:</span></span>

1.  <span data-ttu-id="f0272-112">Проверьте учетную запись клиента и убедитесь, что она не скомпрометирована.</span><span class="sxs-lookup"><span data-stu-id="f0272-112">Review and confirm that the customer account is in good standing.</span></span> <span data-ttu-id="f0272-113">Чтобы быстро перейти к подписке, нажмите на уведомление.</span><span class="sxs-lookup"><span data-stu-id="f0272-113">You can access the subscription directly by clicking on the notification.</span></span>

2.  <span data-ttu-id="f0272-114">Проверьте тенденции использования Azure для этой подписки.</span><span class="sxs-lookup"><span data-stu-id="f0272-114">Review Azure usage patterns for the subscription.</span></span> <span data-ttu-id="f0272-115">Внезапные всплески могут означать нетипичную активность.</span><span class="sxs-lookup"><span data-stu-id="f0272-115">Sudden spikes may suggest unexpected activity.</span></span>

3.  <span data-ttu-id="f0272-116">Свяжитесь с клиентом и убедитесь, что ему известно об этой активности.</span><span class="sxs-lookup"><span data-stu-id="f0272-116">Contact the customer to confirm that the activity is expected.</span></span>

<span data-ttu-id="f0272-117">Если это нормальная активность, вернитесь к странице сведений о подписке Azure этого клиента и подтвердите законность майнинга криптовалют.</span><span class="sxs-lookup"><span data-stu-id="f0272-117">If the activity is expected, return to the customer's Azure subscription detail page and confirm that the cryptocurrency mining is legitimate.</span></span> 


![](images/crypto2.png)

<span data-ttu-id="f0272-118">Если эта активность нетипична, рекомендуется сделать следующее:</span><span class="sxs-lookup"><span data-stu-id="f0272-118">If the activity is unexpected, consider the following:</span></span>

1.  <span data-ttu-id="f0272-119">Убедитесь, что ресурсы Azure, используемые для майнинга криптовалют, не являются необходимыми, и удалите их во избежание дальнейших расходов.</span><span class="sxs-lookup"><span data-stu-id="f0272-119">Confirm that the Azure resources for cryptocurrency mining are not needed and delete them to avoid further Azure charges.</span></span>

2.  <span data-ttu-id="f0272-120">Узнайте, как были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="f0272-120">Understand how the resources were created in the first place.</span></span> <span data-ttu-id="f0272-121">Для этого могут потребоваться данные из журналов управления ресурсами Azure, где регистрируется развертывание ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f0272-121">This may require you to review the Azure Resource Management logs for resource provisioning activities.</span></span>

3.  <span data-ttu-id="f0272-122">Если нужно узнать, кто создал подписку, посмотрите журналы активности на панели мониторинга Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="f0272-122">If you need to find out who created the subscription, review Partner Dashboard activity logs.</span></span>

<span data-ttu-id="f0272-123">Удаление операций майнинга криптовалют основывается на эвристическом методе и не является стопроцентно точным.</span><span class="sxs-lookup"><span data-stu-id="f0272-123">Detection of cryptocurrency mining activities is based on heuristics and may not be 100% accurate.</span></span> <span data-ttu-id="f0272-124">Всегда используйте системы контроля и мониторинга для защиты от мошенничества и прочих запрещенных операций.</span><span class="sxs-lookup"><span data-stu-id="f0272-124">Be sure to have governance and monitoring systems in place to protect against fraudulent or other unpermitted activities.</span></span> <span data-ttu-id="f0272-125">Дополнительные сведения см. в разделе [Неуплата, мошенничество и нарушение правил использования](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse).</span><span class="sxs-lookup"><span data-stu-id="f0272-125">For more information, see [Non-payment, fraud, or misuse](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse).</span></span>




