---
title: Удаление связи между торговыми посредниками с клиентом
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как Microsoft Direct Partner может удалять клиентов из списка, удалять делегированные права администратора и прекращать поддержку или покупку для клиента.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551475"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="4e379-103">Как удалить связь торгового посредника с клиентом в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="4e379-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="4e379-104">**Соответствующие роли** — глобальный администратор.</span><span class="sxs-lookup"><span data-stu-id="4e379-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="4e379-105">В этой статье описывается, как удалить связь через торгового посредника с клиентом в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="4e379-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="4e379-106">Прямые партнеры или косвенные поставщики. Если вы больше не собираетесь работать с клиентом, вы можете удалить эту связь в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="4e379-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="4e379-107">Удаление связи имеет следующие последствия.</span><span class="sxs-lookup"><span data-stu-id="4e379-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="4e379-108">удаляет клиента из списка клиентов в Центре партнеров;</span><span class="sxs-lookup"><span data-stu-id="4e379-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="4e379-109">Удаляет вас из [списка доступных контактов поддержки](assign-support-contacts.md) для вашего клиента</span><span class="sxs-lookup"><span data-stu-id="4e379-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="4e379-110">удаляет ваши права делегированного администратора для клиента;</span><span class="sxs-lookup"><span data-stu-id="4e379-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="4e379-111">Не позволяет клиенту делать покупки в дальнейшем</span><span class="sxs-lookup"><span data-stu-id="4e379-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="4e379-112">Удаление связи</span><span class="sxs-lookup"><span data-stu-id="4e379-112">How to remove a relationship</span></span>

<span data-ttu-id="4e379-113">Чтобы удалить связь, необходимо сначала отменить резервирования зарезервированных экземпляров Azure (RI), отменить покупки программного обеспечения и приостановить все оставшиеся активные подписки.</span><span class="sxs-lookup"><span data-stu-id="4e379-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="4e379-114">**Приостановите все активные подписки.**</span><span class="sxs-lookup"><span data-stu-id="4e379-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="4e379-115">В центре партнеров перейдите к разделу **Клиенты** и выберите клиента.</span><span class="sxs-lookup"><span data-stu-id="4e379-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="4e379-116">В разделе **подписки** выберите подписку.</span><span class="sxs-lookup"><span data-stu-id="4e379-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="4e379-117">Выбор **приостановлена**</span><span class="sxs-lookup"><span data-stu-id="4e379-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="4e379-118">Повторите эти действия для каждой активной подписки.</span><span class="sxs-lookup"><span data-stu-id="4e379-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="4e379-119">**Удалите связь в центре партнеров:**</span><span class="sxs-lookup"><span data-stu-id="4e379-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="4e379-120">а.</span><span class="sxs-lookup"><span data-stu-id="4e379-120">a.</span></span> <span data-ttu-id="4e379-121">В центре партнеров перейдите к разделу **Клиенты** и выберите клиента.</span><span class="sxs-lookup"><span data-stu-id="4e379-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="4e379-122">b.</span><span class="sxs-lookup"><span data-stu-id="4e379-122">b.</span></span> <span data-ttu-id="4e379-123">Выберите **Учетная запись**.</span><span class="sxs-lookup"><span data-stu-id="4e379-123">Select the **Account**.</span></span>

   <span data-ttu-id="4e379-124">c.</span><span class="sxs-lookup"><span data-stu-id="4e379-124">c.</span></span> <span data-ttu-id="4e379-125">Выберите **Удалить связь с торговым посредником**.</span><span class="sxs-lookup"><span data-stu-id="4e379-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="4e379-126">Если какие-либо подписки активны, ссылка **Удалить связь с торговыми посредниками** будет неактивна.</span><span class="sxs-lookup"><span data-stu-id="4e379-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4e379-127">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="4e379-127">Next steps</span></span>

- [<span data-ttu-id="4e379-128">Запрос или повторное создание связи с клиентом</span><span class="sxs-lookup"><span data-stu-id="4e379-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
