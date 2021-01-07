---
title: Настройка многофакторной проверки подлинности для пользователей
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Узнайте, как настроить MFA для сотрудников
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "97578295"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="840bc-103">Настройка многофакторной проверки подлинности для пользователей</span><span class="sxs-lookup"><span data-stu-id="840bc-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="840bc-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="840bc-104">**Appropriate roles**</span></span>

- <span data-ttu-id="840bc-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="840bc-105">Global admin</span></span>

<span data-ttu-id="840bc-106">Более высокий уровень конфиденциальности и безопасности является одним из наших главных приоритетов.</span><span class="sxs-lookup"><span data-stu-id="840bc-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="840bc-107">Мы знаем, что лучшая защита — это предотвращение, и что мы не сильнее самого слабого звена.</span><span class="sxs-lookup"><span data-stu-id="840bc-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="840bc-108">Именно поэтому каждый элемент в нашей экосистеме должен работать должным образом, обеспечивая надлежащую защиту.</span><span class="sxs-lookup"><span data-stu-id="840bc-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="840bc-109">Настоятельно рекомендуем всем партнерам включить многофакторную проверку подлинности (MFA) для своих пользователей в арендаторе партнера.</span><span class="sxs-lookup"><span data-stu-id="840bc-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="840bc-110">Добавление многофакторной проверки подлинности для ваших пользователей</span><span class="sxs-lookup"><span data-stu-id="840bc-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="840bc-111">Для выполнения этой задачи необходимы права глобального администратора компании.</span><span class="sxs-lookup"><span data-stu-id="840bc-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="840bc-112">Проще всего включать MFA для пользователей по мере их добавления в арендатор Azure AD.</span><span class="sxs-lookup"><span data-stu-id="840bc-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="840bc-113">Войдите на [портал Azure](https://portal.azure.com) и перейдите к разделу **Управление пользователями**.</span><span class="sxs-lookup"><span data-stu-id="840bc-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="840bc-114">Выберите элемент **Многофакторная проверка подлинности**.</span><span class="sxs-lookup"><span data-stu-id="840bc-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="840bc-115">Выберите пользователя, для которого необходимо включить проверку, а затем выберите элемент **Включить**.</span><span class="sxs-lookup"><span data-stu-id="840bc-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="840bc-116">Для этого пользователя будет включена проверка MFA.</span><span class="sxs-lookup"><span data-stu-id="840bc-116">This will enable MFA for this user.</span></span> <span data-ttu-id="840bc-117">Значение "Включено" означает, что пользователю будет предложено настроить проверку MFA при первом входе.</span><span class="sxs-lookup"><span data-stu-id="840bc-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="840bc-118">Затем при входе в систему для пользователя отобразится запрос на ввод кода, отправленного ему по электронной почте или в текстовом сообщении (в зависимости от того, какой из вариантов настроил пользователь).</span><span class="sxs-lookup"><span data-stu-id="840bc-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Указание способа проверки":::

>[!NOTE]
><span data-ttu-id="840bc-120">Вы можете **принудительно применить** для пользователей требование прохождения MFA. Для этого выполните описанные выше действия и выберите элемент **Принудительно**.</span><span class="sxs-lookup"><span data-stu-id="840bc-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="840bc-121">Дополнительные сведения см. в статье о [включении Многофакторной идентификации Azure для защиты при входе](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="840bc-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="840bc-122">Начальное состояние для всех пользователей —  **Отключено**.</span><span class="sxs-lookup"><span data-stu-id="840bc-122">All users start out **Disabled**.</span></span> <span data-ttu-id="840bc-123">При регистрации пользователей для Многофакторной идентификации Azure состояние изменяется на  **Включено**.</span><span class="sxs-lookup"><span data-stu-id="840bc-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="840bc-124">Если пользователи, для которых включена проверка, входят в систему и завершают процесс регистрации, состояние меняется на  **Принудительно**.</span><span class="sxs-lookup"><span data-stu-id="840bc-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="840bc-125">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="840bc-125">Next steps</span></span>

- [<span data-ttu-id="840bc-126">Назначение ролей и разрешений пользователям</span><span class="sxs-lookup"><span data-stu-id="840bc-126">Assign roles and permissions to users</span></span>](permissions-overview.md)
