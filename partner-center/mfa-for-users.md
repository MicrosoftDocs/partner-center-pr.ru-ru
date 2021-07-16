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
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450813"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="8dac7-103">Настройка многофакторной проверки подлинности для пользователей</span><span class="sxs-lookup"><span data-stu-id="8dac7-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="8dac7-104">**Соответствующие роли** — глобальный администратор.</span><span class="sxs-lookup"><span data-stu-id="8dac7-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="8dac7-105">Более высокий уровень конфиденциальности и безопасности является одним из наших главных приоритетов.</span><span class="sxs-lookup"><span data-stu-id="8dac7-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="8dac7-106">Мы знаем, что лучшая защита — это предотвращение, и что мы не сильнее самого слабого звена.</span><span class="sxs-lookup"><span data-stu-id="8dac7-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="8dac7-107">Именно поэтому каждый элемент в нашей экосистеме должен работать должным образом, обеспечивая надлежащую защиту.</span><span class="sxs-lookup"><span data-stu-id="8dac7-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="8dac7-108">Настоятельно рекомендуем всем партнерам включить многофакторную проверку подлинности (MFA) для своих пользователей в арендаторе партнера.</span><span class="sxs-lookup"><span data-stu-id="8dac7-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="8dac7-109">Добавление многофакторной проверки подлинности для ваших пользователей</span><span class="sxs-lookup"><span data-stu-id="8dac7-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="8dac7-110">Для выполнения этой задачи необходимы права глобального администратора компании.</span><span class="sxs-lookup"><span data-stu-id="8dac7-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="8dac7-111">Проще всего включать MFA для пользователей по мере их добавления в арендатор Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8dac7-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="8dac7-112">Войдите на [портал Azure](https://portal.azure.com) и перейдите к разделу **Управление пользователями**.</span><span class="sxs-lookup"><span data-stu-id="8dac7-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="8dac7-113">Выберите элемент **Многофакторная проверка подлинности**.</span><span class="sxs-lookup"><span data-stu-id="8dac7-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="8dac7-114">Выберите пользователя, для которого необходимо включить проверку, а затем выберите элемент **Включить**.</span><span class="sxs-lookup"><span data-stu-id="8dac7-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="8dac7-115">Для этого пользователя будет включена проверка MFA.</span><span class="sxs-lookup"><span data-stu-id="8dac7-115">This will enable MFA for this user.</span></span> <span data-ttu-id="8dac7-116">Значение "Включено" означает, что пользователю будет предложено настроить проверку MFA при первом входе.</span><span class="sxs-lookup"><span data-stu-id="8dac7-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="8dac7-117">Затем при входе в систему для пользователя отобразится запрос на ввод кода, отправленного ему по электронной почте или в текстовом сообщении (в зависимости от того, какой из вариантов настроил пользователь).</span><span class="sxs-lookup"><span data-stu-id="8dac7-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Укажите способ проверки.":::

>[!NOTE]
><span data-ttu-id="8dac7-119">Вы можете **принудительно применить** для пользователей требование прохождения MFA. Для этого выполните описанные выше действия и выберите элемент **Принудительно**.</span><span class="sxs-lookup"><span data-stu-id="8dac7-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="8dac7-120">Дополнительные сведения см. в статье о [включении Многофакторной идентификации Azure для защиты при входе](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="8dac7-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="8dac7-121">Начальное состояние для всех пользователей —  **Отключено**.</span><span class="sxs-lookup"><span data-stu-id="8dac7-121">All users start out **Disabled**.</span></span> <span data-ttu-id="8dac7-122">При регистрации пользователей для Многофакторной идентификации Azure Active Directory состояние изменяется на  **Включено**.</span><span class="sxs-lookup"><span data-stu-id="8dac7-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="8dac7-123">Если пользователи, для которых включена проверка, входят в систему и завершают процесс регистрации, состояние меняется на  **Принудительно**.</span><span class="sxs-lookup"><span data-stu-id="8dac7-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="8dac7-124">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8dac7-124">Next steps</span></span>

- [<span data-ttu-id="8dac7-125">Назначение ролей и разрешений пользователям</span><span class="sxs-lookup"><span data-stu-id="8dac7-125">Assign roles and permissions to users</span></span>](permissions-overview.md)