---
title: Переключить партнера прямых счетов на непрямые торговые посредники
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как партнер по программе CSP может использовать центр партнеров для перехода от партнеров прямого счета к непрямому торговому посреднику.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e7676df62aa6ea91492f9904ac810397fb0e5aa
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768760"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="fff9d-103">Переход со статуса партнера с прямым выставлением счетов в статус косвенного торгового посредника в рамках программы CSP</span><span class="sxs-lookup"><span data-stu-id="fff9d-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="fff9d-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="fff9d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fff9d-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fff9d-105">Global admin</span></span>

>[!Note]
><span data-ttu-id="fff9d-106">Эта статья предназначена для партнеров с прямыми счетами, которые решили перейти на непрямые торговые посредники.</span><span class="sxs-lookup"><span data-stu-id="fff9d-106">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="fff9d-107">Однако даже если вы еще не предоставили явное решение для регистрации в качестве непрямого торгового посредника, партнеры прямого счета, которые не соответствуют новым [требованиям](direct-partner-new-requirements.md) для партнерской программы прямого выставления счетов CSP, будут уведомлены корпорацией Майкрософт, если их [возможности прямого счета будут ограничены](restricted-direct-bill-capabilities.md).</span><span class="sxs-lookup"><span data-stu-id="fff9d-107">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="fff9d-108">По состоянию на 2021 января будет добавлено новое требование дохода.</span><span class="sxs-lookup"><span data-stu-id="fff9d-108">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="fff9d-109">Партнерам, зарегистрированным в качестве партнера по прямому счету, необходимо, чтобы в рамках программы поставщика облачных решений по крайней мере на уровне глобальной учетной записи в течение предыдущих 12 месяцев выдавалась заявка на использование транзакций не ниже USD $300 тыс</span><span class="sxs-lookup"><span data-stu-id="fff9d-109">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="fff9d-110">Вы сможете зарегистрироваться в программе непрямого торгового посредника с помощью существующего клиента прямого счета.</span><span class="sxs-lookup"><span data-stu-id="fff9d-110">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="fff9d-111">Начало работы</span><span class="sxs-lookup"><span data-stu-id="fff9d-111">Get started</span></span>

1. <span data-ttu-id="fff9d-112">Убедитесь, что профиль партнера в центре партнеров и идентификатор MPN актуальны.</span><span class="sxs-lookup"><span data-stu-id="fff9d-112">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="fff9d-113">Войдите в центр партнеров в качестве глобального администратора для клиента прямого счета, который вы переходите к непрямому торговому посреднику.</span><span class="sxs-lookup"><span data-stu-id="fff9d-113">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Обзор":::

3. <span data-ttu-id="fff9d-115">Проверьте сведения о партнере в форме регистрации.</span><span class="sxs-lookup"><span data-stu-id="fff9d-115">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Зарегистрироваться сейчас":::

4. <span data-ttu-id="fff9d-117">Выберите Зарегистрироваться сейчас.</span><span class="sxs-lookup"><span data-stu-id="fff9d-117">Select Enroll now.</span></span> <span data-ttu-id="fff9d-118">Компания непрямого торгового посредника будет использовать тот же клиент AAD, который вы используете для вашего прямого бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fff9d-118">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="fff9d-119">Изначально эта новая возможность перехода будет доступна для партнеров с датами сентября по Декабрьам.</span><span class="sxs-lookup"><span data-stu-id="fff9d-119">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="fff9d-120">Если у вас нет даты юбилея в диапазоне от сентября до декабря, эта возможность не будет отображаться в данный момент.</span><span class="sxs-lookup"><span data-stu-id="fff9d-120">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="fff9d-121">Партнеры с датами юбилеев после декабря 2018 будут уведомлены позже, когда функция будет включена для участников.</span><span class="sxs-lookup"><span data-stu-id="fff9d-121">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="fff9d-122">После утверждения регистрации войдите в центр партнеров еще раз.</span><span class="sxs-lookup"><span data-stu-id="fff9d-122">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="fff9d-123">Хотя утверждение обычно осуществляется немедленно, это может занять до пяти рабочих дней.</span><span class="sxs-lookup"><span data-stu-id="fff9d-123">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="fff9d-124">После утверждения вы получите уведомление по адресу электронной почты, указанному в разделе основное контактное лицо в форме регистрации.</span><span class="sxs-lookup"><span data-stu-id="fff9d-124">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="fff9d-125">Вы также можете проверить состояние регистрации в разделе **Параметры**  >  **учетной записи**  >  **профиль партнера** > сведения о программе.</span><span class="sxs-lookup"><span data-stu-id="fff9d-125">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="fff9d-126">На странице **обзора** вы увидите непрямое соглашение торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-126">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="fff9d-127">Выберите **Принять и продолжить**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-127">Select **Accept and continue**.</span></span> <span data-ttu-id="fff9d-128">Это действие включает косвенные возможности торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-128">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="fff9d-129">Если вы приняли соглашение о непрямом торговом посреднике, обратите внимание, что ваш профиль партнера определяет как прямой, **так** и непрямой Торговый посредник.</span><span class="sxs-lookup"><span data-stu-id="fff9d-129">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Непрямое соглашение торгового посредника":::

> [!IMPORTANT]
> <span data-ttu-id="fff9d-131">После регистрации в качестве непрямого торгового посредника с помощью новой возможности нет возможности выполнить откат до прямого клиента, предназначенного только для счета.</span><span class="sxs-lookup"><span data-stu-id="fff9d-131">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="fff9d-132">Прежде чем регистрировать непрямого торгового посредника, убедитесь, что вы полностью оцениваете бизнес-потребности.</span><span class="sxs-lookup"><span data-stu-id="fff9d-132">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="fff9d-133">При переходе от Direct к непрямому торговому посреднику</span><span class="sxs-lookup"><span data-stu-id="fff9d-133">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="fff9d-134">На этом этапе вы продолжите управлять потребностями ваших прямых клиентов, включая процесс выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="fff9d-134">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="fff9d-135">Вы также можете начать прием клиентов от непрямого поставщика и работать в качестве непрямого торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-135">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Вы как прямой, так и непрямой Торговый посредник":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="fff9d-137">Найти косвенного поставщика</span><span class="sxs-lookup"><span data-stu-id="fff9d-137">Find an indirect provider</span></span>

<span data-ttu-id="fff9d-138">После регистрации в левой панели навигации появится ссылка на непрямые поставщики.</span><span class="sxs-lookup"><span data-stu-id="fff9d-138">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="fff9d-139">В качестве непрямого торгового посредника вы будете устанавливать связь с непрямым поставщиком, который затем может выполнять выставление счетов, покупать продукты для клиентов и инфраструктуру поддержки.</span><span class="sxs-lookup"><span data-stu-id="fff9d-139">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="fff9d-140">Различные косвенные поставщики предлагают различную поддержку и службы, поэтому вам следует оценить поставщиков в своем регионе, чтобы определить, какие из них лучше всего соответствуют вашим требованиям.</span><span class="sxs-lookup"><span data-stu-id="fff9d-140">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="fff9d-141">Как правило, большинство поставщиков:</span><span class="sxs-lookup"><span data-stu-id="fff9d-141">Generally, most providers will:</span></span>

- <span data-ttu-id="fff9d-142">предоставляют вам техническое обучение и поддержку;</span><span class="sxs-lookup"><span data-stu-id="fff9d-142">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="fff9d-143">помогают вам с маркетингом продуктов и служб;</span><span class="sxs-lookup"><span data-stu-id="fff9d-143">Help you market your products and services</span></span>
- <span data-ttu-id="fff9d-144">Управляйте своими соглашениями о финансирования и кредитом</span><span class="sxs-lookup"><span data-stu-id="fff9d-144">Manage your financing and credit terms</span></span>

<span data-ttu-id="fff9d-145">Поиск в списке официальных [непрямых поставщиков Майкрософт](https://partnercenter.microsoft.com/partner/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="fff9d-145">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="fff9d-146">Дополнительные сведения, чтение  [партнера с непрямыми поставщиками](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="fff9d-146">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="fff9d-147">Принятие приглашения на партнерство от непрямого поставщика</span><span class="sxs-lookup"><span data-stu-id="fff9d-147">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="fff9d-148">При обнаружении косвенного поставщика для партнера установите связь с косвенным поставщиком в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="fff9d-148">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="fff9d-149">Выбранный косвенный поставщик отправит вам по электронной почте ссылку на приглашение партнерства, которая перейдет к приглашению в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="fff9d-149">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="fff9d-150">Убедитесь, что глобальный администратор входит в центр партнеров и находится по ссылке с приглашением.</span><span class="sxs-lookup"><span data-stu-id="fff9d-150">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="fff9d-151">Когда вы принимаете приглашение, имя поставщика появится в списке непрямого поставщика.</span><span class="sxs-lookup"><span data-stu-id="fff9d-151">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="fff9d-152">Приобретение новых клиентов в качестве непрямого торгового посредника</span><span class="sxs-lookup"><span data-stu-id="fff9d-152">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="fff9d-153">И вы, и ваш косвенный поставщик должны иметь связи между торговыми посредниками и клиентами.</span><span class="sxs-lookup"><span data-stu-id="fff9d-153">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="fff9d-154">Эти связи между торговыми посредниками позволяют управлять подписками и службами клиента от их имени.</span><span class="sxs-lookup"><span data-stu-id="fff9d-154">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="fff9d-155">Чтобы получить нового клиента с существующим клиентом Azure AD, можно пригласить клиента на одновременное создание связи с вами и вашим поставщиком.</span><span class="sxs-lookup"><span data-stu-id="fff9d-155">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="fff9d-156">Чтобы создать приглашение косвенного торгового посредника, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="fff9d-156">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="fff9d-157">В левой панели навигации центра партнеров выберите **непрямые поставщики** .</span><span class="sxs-lookup"><span data-stu-id="fff9d-157">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="fff9d-158">Выберите **Пригласить новых клиентов**, чтобы пригласить клиента для установления отношений торгового посредника одновременно с вами и косвенным поставщиком.</span><span class="sxs-lookup"><span data-stu-id="fff9d-158">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="fff9d-159">Поставщик должен иметь связь с клиентом, чтобы они могли отправлять заказы от своего имени клиента, когда клиент хочет купить новые подписки или добавить новые лицензии в существующие подписки.</span><span class="sxs-lookup"><span data-stu-id="fff9d-159">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="fff9d-160">На следующей странице просмотрите черновик сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fff9d-160">On the next page, review the draft email message.</span></span> <span data-ttu-id="fff9d-161">Вы можете открыть черновик сообщения в сообщении электронной почты или скопировать сообщение в буфер обмена и вставить его в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fff9d-161">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="fff9d-162">Измените текст в сообщении электронной почты, чтобы сказать, что вам нужно, но не забудьте включить ссылку, так как она является персонализированной для подключения клиента непосредственно к вашей учетной записи и учетной записи поставщика.</span><span class="sxs-lookup"><span data-stu-id="fff9d-162">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="fff9d-163">Затем выберите **Готово**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-163">Then select **Done**.</span></span>

5. <span data-ttu-id="fff9d-164">После того как клиент разрешит вам и вашему поставщику быть его торговыми посредниками, вам будут предоставлены права администратора для управления его подписками, лицензиями и пользователями от его имени, и ваш косвенный поставщик сможет делать заказы от его имени.</span><span class="sxs-lookup"><span data-stu-id="fff9d-164">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="fff9d-165">Чтобы управлять учетной записью, службами, пользователями и лицензиями клиента, разверните его запись, нажав кнопку со стрелкой вниз рядом с его именем.</span><span class="sxs-lookup"><span data-stu-id="fff9d-165">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="fff9d-166">В отличие от прямых партнеров, косвенные торговые посредники не могут создавать клиенты Azure AD для новых клиентов в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="fff9d-166">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="fff9d-167">Поставщик создаст клиент и укажет вас в качестве непрямого торгового посредника для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="fff9d-167">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="fff9d-168">Это гарантирует, что клиент будет отображаться в списке клиентов в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="fff9d-168">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="fff9d-169">Вы не сможете использовать прямую оплату, чтобы создавать покупки для клиентов, приобретенных в качестве непрямого торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-169">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="fff9d-170">Управление клиентами прямого счета и клиентами непрямого торгового посредника</span><span class="sxs-lookup"><span data-stu-id="fff9d-170">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="fff9d-171">Вы управляете клиентами прямого счета и клиентами непрямого торгового посредника по-разному.</span><span class="sxs-lookup"><span data-stu-id="fff9d-171">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="fff9d-172">Клиенты с прямым выставлением счетов (что не является непрямым торговым посредником)</span><span class="sxs-lookup"><span data-stu-id="fff9d-172">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="fff9d-173">Создание заказов для продуктов</span><span class="sxs-lookup"><span data-stu-id="fff9d-173">Create orders for products</span></span>
- <span data-ttu-id="fff9d-174">Управление резервированиями Azure</span><span class="sxs-lookup"><span data-stu-id="fff9d-174">Manage Azure reservations</span></span>
- <span data-ttu-id="fff9d-175">Управление журналом заказов</span><span class="sxs-lookup"><span data-stu-id="fff9d-175">Manage their order history</span></span>
- <span data-ttu-id="fff9d-176">Приобретение программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="fff9d-176">Purchase software</span></span>
- <span data-ttu-id="fff9d-177">Выставление счетов клиентам напрямую</span><span class="sxs-lookup"><span data-stu-id="fff9d-177">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="fff9d-178">Клиенты косвенного торгового посредника</span><span class="sxs-lookup"><span data-stu-id="fff9d-178">Indirect reseller customers</span></span>

- <span data-ttu-id="fff9d-179">Продукты непрямого поставщика заказа для ваших клиентов</span><span class="sxs-lookup"><span data-stu-id="fff9d-179">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="fff9d-180">Управление лицензиями и пользователями клиентов</span><span class="sxs-lookup"><span data-stu-id="fff9d-180">Manage customers' licenses and users</span></span>
- <span data-ttu-id="fff9d-181">Работа с обновлениями подписки</span><span class="sxs-lookup"><span data-stu-id="fff9d-181">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="fff9d-182">Для поиска клиентов, приобретенных в качестве партнера прямого счета</span><span class="sxs-lookup"><span data-stu-id="fff9d-182">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="fff9d-183">Выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-183">Select **Customers**.</span></span>

2. <span data-ttu-id="fff9d-184">Выберите клиента, чтобы просмотреть сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="fff9d-184">Select a customer to view their details.</span></span>

3. <span data-ttu-id="fff9d-185">Если это клиент, который вы приобрели в качестве партнера прямого счета, вы увидите варианты **добавления** или **просмотра продуктов** , и вы увидите их подписки.</span><span class="sxs-lookup"><span data-stu-id="fff9d-185">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="fff9d-186">Если у клиента есть непрямая связь с вами, эти параметры будут недоступны.</span><span class="sxs-lookup"><span data-stu-id="fff9d-186">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="fff9d-187">Перемещение клиентов прямого счета на непрямой поставщик</span><span class="sxs-lookup"><span data-stu-id="fff9d-187">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="fff9d-188">Ваш косвенный поставщик не может отправлять заказы или существующие передачи для существующих клиентов с прямым счетом, пока они не будут связаны с ними через торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-188">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="fff9d-189">Чтобы установить связь между прямым поставщиком и клиентом, имеющим прямое выставление счетов, можно использовать один из следующих методов.</span><span class="sxs-lookup"><span data-stu-id="fff9d-189">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="fff9d-190">Расширение связи торгового посредника</span><span class="sxs-lookup"><span data-stu-id="fff9d-190">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="fff9d-191">Отправка приглашения косвенного торгового посредника клиенту</span><span class="sxs-lookup"><span data-stu-id="fff9d-191">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="fff9d-192">Подробный обзор пошагового процесса см. в [документе Direct to опосредованный переход](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) .</span><span class="sxs-lookup"><span data-stu-id="fff9d-192">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="fff9d-193">Расширение связи торгового посредника</span><span class="sxs-lookup"><span data-stu-id="fff9d-193">Reseller relationship extension</span></span>

<span data-ttu-id="fff9d-194">Вы можете использовать функцию расширения отношений торгового посредника, чтобы установить связь между существующими клиентами прямого счета и прямым поставщиком с помощью панели мониторинга центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="fff9d-194">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="fff9d-195">Перед использованием этой функции Обратите внимание на следующее.</span><span class="sxs-lookup"><span data-stu-id="fff9d-195">Before using the feature, note the following:</span></span>

- <span data-ttu-id="fff9d-196">Эта функция доступна только прямым счетам, которые участвуют в непрямом торговом посреднике и прошли прямую [регистрацию торгового посредника](#get-started).</span><span class="sxs-lookup"><span data-stu-id="fff9d-196">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="fff9d-197">Эту функцию можно применить только к существующим клиентам с прямым счетом.</span><span class="sxs-lookup"><span data-stu-id="fff9d-197">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="fff9d-198">Он неприменим к [клиентам косвенных торговых посредников](#acquire-new-customers-as-indirect-reseller).</span><span class="sxs-lookup"><span data-stu-id="fff9d-198">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="fff9d-199">Вы можете выбрать только косвенного поставщика, которому вы [приняли приглашение от непрямого поставщика](#accept-a-partnership-invitation-from-your-indirect-provider).</span><span class="sxs-lookup"><span data-stu-id="fff9d-199">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="fff9d-200">Копия сведений о счете для этого клиента будет предоставляться косвенному поставщику.</span><span class="sxs-lookup"><span data-stu-id="fff9d-200">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="fff9d-201">Доступ к сведениям о счете можно получить, перейдя на страницу учетной записи для этого клиента на панели мониторинга центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="fff9d-201">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="fff9d-202">С помощью функции расширения отношений торгового посредника вы даете согласие на совместное использование сведений о счете для этого клиента с косвенным поставщиком.</span><span class="sxs-lookup"><span data-stu-id="fff9d-202">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="fff9d-203">Непрямой поставщик не будет предоставляться с [делегированными привилегиями на администрирование](customers-revoke-admin-privileges.md) клиенту клиента.</span><span class="sxs-lookup"><span data-stu-id="fff9d-203">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="fff9d-204">Если непрямому поставщику требуются права делегированного администрирования, необходимо отправить клиенту приглашение непрямого торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-204">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="fff9d-205">После того как связь с торговыми посредниками установлена, косвенный поставщик будет отображаться в качестве партнера CSP для клиента на странице связи партнеров в [Microsoft 365 центре администрирования](https://admin.microsoft.com/AdminPortal/Home#/partners) и [Microsoft Store для бизнеса](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="fff9d-205">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="fff9d-206">Чтобы избежать путаницы и неправильного понимания, вы по договору обязани от соглашения партнера, чтобы уведомить и получить согласие от клиента прямого счета, прежде чем использовать функцию расширения связи для установления связи между существующим прямым клиентом счета и косвенным поставщиком.</span><span class="sxs-lookup"><span data-stu-id="fff9d-206">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="fff9d-207">Чтобы использовать эту функцию в существующем клиенте клиента, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="fff9d-207">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="fff9d-208">Войдите в центр партнеров как **Агент администратора**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-208">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="fff9d-209">На **странице клиенты** выберите существующего клиента и щелкните значок **быстрые ссылки** , чтобы развернуть сводное представление клиента.</span><span class="sxs-lookup"><span data-stu-id="fff9d-209">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="fff9d-210">В разделе **непрямые поставщики** щелкните **передавать клиента для косвенного поставщика**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-210">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Передавать клиента косвенному поставщику":::

4. <span data-ttu-id="fff9d-212">Во всплывающем диалоговом окне выберите **косвенного поставщика** , которому вы хотите получить связь между торговыми посредниками и клиентом.</span><span class="sxs-lookup"><span data-stu-id="fff9d-212">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="fff9d-213">Щелкните **Сохранить и продолжить**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-213">Click **Save and continue**.</span></span>

6. <span data-ttu-id="fff9d-214">Убедитесь, что выбранный косвенный поставщик отображается в разделе **непрямые поставщики (s)**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-214">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Список косвенных поставщиков":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="fff9d-216">Отправка приглашения косвенного торгового посредника клиенту</span><span class="sxs-lookup"><span data-stu-id="fff9d-216">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="fff9d-217">Ваш косвенный поставщик не может отправлять заказы для ваших существующих клиентов с прямым выставлением счетов, пока им не будет назначена связь через торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-217">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="fff9d-218">Чтобы установить связь между существующими клиентами и непрямым поставщиком услуг, пригласите клиента с помощью приглашения косвенного торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="fff9d-218">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="fff9d-219">В левой панели навигации центра партнеров выберите **непрямые поставщики** .</span><span class="sxs-lookup"><span data-stu-id="fff9d-219">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="fff9d-220">Выберите **Пригласить новых клиентов**, чтобы пригласить клиента для установления отношений торгового посредника одновременно с вами и косвенным поставщиком.</span><span class="sxs-lookup"><span data-stu-id="fff9d-220">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="fff9d-221">Поставщик должен иметь связь с клиентом, чтобы они могли отправлять заказы от своего имени клиента, когда клиент хочет купить новые подписки или добавить новые лицензии в существующие подписки.</span><span class="sxs-lookup"><span data-stu-id="fff9d-221">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Пригласить новых клиентов":::

3. <span data-ttu-id="fff9d-223">На следующей странице просмотрите черновик сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fff9d-223">On the next page, review the draft email message.</span></span> <span data-ttu-id="fff9d-224">Вы можете открыть черновик сообщения в сообщении электронной почты или скопировать сообщение в буфер обмена и вставить его в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fff9d-224">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="fff9d-225">Измените текст в сообщении электронной почты, чтобы сказать, что вам нужно, но не забудьте включить ссылку, так как она является персонализированной для подключения клиента непосредственно к вашей учетной записи и учетной записи поставщика.</span><span class="sxs-lookup"><span data-stu-id="fff9d-225">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="fff9d-226">Затем выберите **Готово**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-226">Then select **Done**.</span></span>

5. <span data-ttu-id="fff9d-227">После того как клиент разрешит вам и вашему поставщику быть его торговыми посредниками, вам будут предоставлены права администратора для управления его подписками, лицензиями и пользователями от его имени, и ваш косвенный поставщик сможет делать заказы от его имени.</span><span class="sxs-lookup"><span data-stu-id="fff9d-227">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="fff9d-228">Чтобы управлять учетной записью, службами, пользователями и лицензиями клиента, разверните его запись, нажав кнопку со стрелкой вниз рядом с его именем.</span><span class="sxs-lookup"><span data-stu-id="fff9d-228">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="fff9d-229">Принятие условий соглашения для клиентов Майкрософт</span><span class="sxs-lookup"><span data-stu-id="fff9d-229">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="fff9d-230">Соглашение Microsoft Cloud действует до 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="fff9d-230">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="fff9d-231">После этой даты все клиенты, существующие и новые, должны подписать новое [Соглашение клиента Майкрософт](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="fff9d-231">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="fff9d-232">Для перехода клиентов, если:</span><span class="sxs-lookup"><span data-stu-id="fff9d-232">For transitioning customers, if:</span></span>

- <span data-ttu-id="fff9d-233">**Клиент еще не принял Соглашение клиента Майкрософт**</span><span class="sxs-lookup"><span data-stu-id="fff9d-233">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="fff9d-234">Обратитесь к косвенному поставщику, чтобы [он принимал соглашение клиента Майкрософт](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="fff9d-234">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="fff9d-235">**Клиент принял соглашение с клиентами корпорации Майкрософт в центре администрирования Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="fff9d-235">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="fff9d-236">Принятие будет храниться, когда связь торгового посредника устанавливается с косвенным поставщиком.</span><span class="sxs-lookup"><span data-stu-id="fff9d-236">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="fff9d-237">Ничего делать не нужно.</span><span class="sxs-lookup"><span data-stu-id="fff9d-237">There is nothing you need to do.</span></span>

- <span data-ttu-id="fff9d-238">**Клиент принял соглашение с клиентами Майкрософт за вас с помощью аттестации партнеров**</span><span class="sxs-lookup"><span data-stu-id="fff9d-238">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="fff9d-239">Принятие не будет сохранены.</span><span class="sxs-lookup"><span data-stu-id="fff9d-239">The acceptance will not be retained.</span></span> <span data-ttu-id="fff9d-240">Обратитесь к косвенному поставщику, чтобы [Обновить принятие клиента в центре партнеров](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="fff9d-240">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="fff9d-241">Перенос существующих прямых подписок на счета косвенного поставщика</span><span class="sxs-lookup"><span data-stu-id="fff9d-241">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="fff9d-242">В разделе непрямая модель CSP непрямые торговые посредники не имеют отношений выставления счетов с корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="fff9d-242">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="fff9d-243">Вместо этого непрямые торговые посредники получают подписки для своих клиентов через их косвенные поставщики.</span><span class="sxs-lookup"><span data-stu-id="fff9d-243">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="fff9d-244">При переходе от прямого счета счетов к непрямому торговому посреднику необходимо перенести имеющиеся подписки в качестве партнера по прямым счетам на непрямой поставщик.</span><span class="sxs-lookup"><span data-stu-id="fff9d-244">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="fff9d-245">Для этого можно использовать функцию самостоятельной пересылки подписок на панели мониторинга центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="fff9d-245">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="fff9d-246">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fff9d-246">Prerequisites</span></span>

- <span data-ttu-id="fff9d-247">Эта функция доступна только для партнеров, которые выполнили регистрацию непрямого торгового посредника с помощью существующих клиентов прямого счета.</span><span class="sxs-lookup"><span data-stu-id="fff9d-247">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="fff9d-248">Перед передачей подписок, связанных с данным клиентом, партнер по переходу должен переместить клиента косвенному поставщику.</span><span class="sxs-lookup"><span data-stu-id="fff9d-248">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="fff9d-249">Клиент должен [принять соглашение с клиентом Майкрософт через косвенного поставщика](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="fff9d-249">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="fff9d-250">Переход к непрямому статусу торгового посредника</span><span class="sxs-lookup"><span data-stu-id="fff9d-250">How to transition to indirect reseller status</span></span>

<span data-ttu-id="fff9d-251">Эта функция является 4-шаговым процессом, где:</span><span class="sxs-lookup"><span data-stu-id="fff9d-251">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="fff9d-252">Партнер по переходу создает запрос на передачу подписки.</span><span class="sxs-lookup"><span data-stu-id="fff9d-252">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="fff9d-253">Запрос содержит одну или несколько существующих подписок, связанных с тем же клиентом и адресованных косвенному поставщику.</span><span class="sxs-lookup"><span data-stu-id="fff9d-253">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="fff9d-254">Косвенный поставщик проверяет и принимает (или отвергает) запрос на перемещение.</span><span class="sxs-lookup"><span data-stu-id="fff9d-254">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="fff9d-255">Косвенный поставщик проверяет, что запрос на перемещение завершен.</span><span class="sxs-lookup"><span data-stu-id="fff9d-255">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="fff9d-256">Партнер по переходу проверяет, что запрос на передачу завершен.</span><span class="sxs-lookup"><span data-stu-id="fff9d-256">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="fff9d-257">Партнер по переходу</span><span class="sxs-lookup"><span data-stu-id="fff9d-257">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="fff9d-258">Вы также можете использовать [API или пакет SDK центра партнеров](/partner-center/develop/manage-customers) для перемещения существующих подписок на непрямой поставщик.</span><span class="sxs-lookup"><span data-stu-id="fff9d-258">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="fff9d-259">Получение права на перемещение подписок клиента</span><span class="sxs-lookup"><span data-stu-id="fff9d-259">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="fff9d-260">Создание операции перемещения для клиента</span><span class="sxs-lookup"><span data-stu-id="fff9d-260">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="fff9d-261">Вывод сведений о перемещении для клиента</span><span class="sxs-lookup"><span data-stu-id="fff9d-261">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="fff9d-262">Принятие операции перемещения для клиента</span><span class="sxs-lookup"><span data-stu-id="fff9d-262">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="fff9d-263">Отклонение перемещения клиента</span><span class="sxs-lookup"><span data-stu-id="fff9d-263">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="fff9d-264">Получение сведений об операциях перемещения для клиента</span><span class="sxs-lookup"><span data-stu-id="fff9d-264">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="fff9d-265">Получение сведений о переносе по идентификатору</span><span class="sxs-lookup"><span data-stu-id="fff9d-265">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="fff9d-266">Перемещение партнера — создание запроса на передачу</span><span class="sxs-lookup"><span data-stu-id="fff9d-266">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="fff9d-267">Чтобы создать запрос на передачу в качестве партнера по переходу:</span><span class="sxs-lookup"><span data-stu-id="fff9d-267">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="fff9d-268">Войдите в центр партнеров как **Агент администратора**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-268">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="fff9d-269">На странице **Клиенты** выберите требуемого клиента и щелкните значок быстрые ссылки, чтобы развернуть сводное представление клиента.</span><span class="sxs-lookup"><span data-stu-id="fff9d-269">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="fff9d-270">В разделе **непрямые поставщики** убедитесь, что указан непрямой поставщик.</span><span class="sxs-lookup"><span data-stu-id="fff9d-270">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="fff9d-271">Щелкните **Просмотр подписок**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-271">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="fff9d-272">На странице **подписки** найдите параметр **Подписка перенос**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-272">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="fff9d-273">В разделе **Перемещение подписки** щелкните **запрос на перемещение подписки**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-273">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Запрос на перемещение подписки":::

7. <span data-ttu-id="fff9d-275">В диалоговом окне Запрос передачи выберите одну или несколько подписок для передачи.</span><span class="sxs-lookup"><span data-stu-id="fff9d-275">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Создать запрос на перемещение":::

8. <span data-ttu-id="fff9d-277">Нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-277">Click **Create**.</span></span>

9. <span data-ttu-id="fff9d-278">В разделе " **Перемещение подписки**" появится запрос на перенос активных подписок.</span><span class="sxs-lookup"><span data-stu-id="fff9d-278">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Список запросов на перемещение":::

10. <span data-ttu-id="fff9d-280">Сообщите непрямому поставщику, что вы создали в них запрос на перемещение подписки.</span><span class="sxs-lookup"><span data-stu-id="fff9d-280">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="fff9d-281">Косвенный поставщик — принять запрос на перенос</span><span class="sxs-lookup"><span data-stu-id="fff9d-281">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="fff9d-282">Чтобы проверить и принять запрос на перемещение в качестве косвенного поставщика:</span><span class="sxs-lookup"><span data-stu-id="fff9d-282">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="fff9d-283">Войдите в центр партнеров в качестве агента **администратора** или **агента по продажам**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-283">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="fff9d-284">На странице **Клиенты** выберите требуемого клиента и щелкните значок быстрые ссылки, чтобы развернуть представление сводки для клиента.</span><span class="sxs-lookup"><span data-stu-id="fff9d-284">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="fff9d-285">В разделе **непрямые торговые посредники** убедитесь, что в списке указан партнер по переходу.</span><span class="sxs-lookup"><span data-stu-id="fff9d-285">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="fff9d-286">Щелкните **Просмотр подписок**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-286">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="fff9d-287">На странице **подписки** найдите параметр **Подписка перенос**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-287">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Просмотр запроса на перемещение":::

6. <span data-ttu-id="fff9d-289">В разделе **Перемещение подписки** щелкните запрос на перемещение, чтобы проверить его.</span><span class="sxs-lookup"><span data-stu-id="fff9d-289">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="fff9d-290">По необходимости нажмите кнопку **принять** (или **отклонить**).</span><span class="sxs-lookup"><span data-stu-id="fff9d-290">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Принять запрос на перенос":::

8. <span data-ttu-id="fff9d-292">Дождитесь завершения запроса на перемещение.</span><span class="sxs-lookup"><span data-stu-id="fff9d-292">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="fff9d-293">Косвенный поставщик — Проверка завершения запроса на перемещение</span><span class="sxs-lookup"><span data-stu-id="fff9d-293">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="fff9d-294">После успешного завершения запроса на перемещение убедитесь, что подписки отображаются в разделе **подписки**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-294">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="fff9d-295">Сообщите партнеру по переходу.</span><span class="sxs-lookup"><span data-stu-id="fff9d-295">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="fff9d-296">Переходный партнер — подтверждение завершения передачи запроса</span><span class="sxs-lookup"><span data-stu-id="fff9d-296">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="fff9d-297">Партнер по переходу должен выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="fff9d-297">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="fff9d-298">Войдите в центр партнеров в качестве **агента администратора** или **агента по продажам**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-298">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="fff9d-299">На странице **Клиенты** выберите требуемого клиента и щелкните значок **быстрые ссылки** , чтобы развернуть сводное представление клиента.</span><span class="sxs-lookup"><span data-stu-id="fff9d-299">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="fff9d-300">Щелкните **Просмотр подписок**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-300">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="fff9d-301">На странице **подписки** найдите параметр **Подписка перенос**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-301">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="fff9d-302">Убедитесь, что запрос на перемещение помечен как **полный**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-302">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="fff9d-303">Убедитесь, что подписки больше не отображаются как активные на странице " **подписки** ".</span><span class="sxs-lookup"><span data-stu-id="fff9d-303">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="fff9d-304">Если это подписка Azure (MS-AZR-0145P), она больше не будет отображаться.</span><span class="sxs-lookup"><span data-stu-id="fff9d-304">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="fff9d-305">Если это подписка на основе лицензий (Office 365, Dynamics, Intune), она будет отображаться в состоянии **suspended**.</span><span class="sxs-lookup"><span data-stu-id="fff9d-305">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Подписка приостановлена":::

### <a name="considerations"></a><span data-ttu-id="fff9d-307">Рекомендации</span><span class="sxs-lookup"><span data-stu-id="fff9d-307">Considerations</span></span>

- <span data-ttu-id="fff9d-308">**Идентификатор подписки будет отличаться после перемещения.**</span><span class="sxs-lookup"><span data-stu-id="fff9d-308">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="fff9d-309">Если это подписка Azure (MS-AZR-0145P), Кроме того, у нее будет идентификатор подписки Azure, который хранится у предыдущего владельца и будет отображаться на портале управления Azure.</span><span class="sxs-lookup"><span data-stu-id="fff9d-309">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="fff9d-310">**На одну и ту же подписку нельзя ссылаться несколькими запросами на перемещение.**</span><span class="sxs-lookup"><span data-stu-id="fff9d-310">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="fff9d-311">После создания запроса на перемещение, который включает существующую подписку, нельзя создавать дополнительные запросы на перемещение, включая ту же подписку, пока не будет отменен первый запрос на перемещение.</span><span class="sxs-lookup"><span data-stu-id="fff9d-311">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="fff9d-312">**Надстройки для подписок на основе лицензий должны передаваться вместе с базовой подпиской.**</span><span class="sxs-lookup"><span data-stu-id="fff9d-312">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="fff9d-313">Если при создании запроса на перемещение выбрать существующую подписку с одной или несколькими надстройками, надстройки будут автоматически включаться в запрос на перемещение.</span><span class="sxs-lookup"><span data-stu-id="fff9d-313">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="fff9d-314">**Число лицензий, внесенных в подписку, не будет отражено в существующем запросе на перемещение.**</span><span class="sxs-lookup"><span data-stu-id="fff9d-314">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="fff9d-315">После создания запроса на перемещение, который включает существующую подписку, следует избегать обновления количества лицензий в подписке (или связанных с ней надстроек).</span><span class="sxs-lookup"><span data-stu-id="fff9d-315">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="fff9d-316">В этом случае новое количество не будет отражено в запросе на перемещение.</span><span class="sxs-lookup"><span data-stu-id="fff9d-316">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="fff9d-317">После того как косвенный поставщик принимает запрос на перемещение, результирующая подписка будет иметь старое количество.</span><span class="sxs-lookup"><span data-stu-id="fff9d-317">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="fff9d-318">Если вы хотите, чтобы новое количество было передано косвенному поставщику, необходимо отменить существующий запрос на передачу и создать новый.</span><span class="sxs-lookup"><span data-stu-id="fff9d-318">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="fff9d-319">**Не все покупки можно передавать с помощью самостоятельного переноса подписок.**</span><span class="sxs-lookup"><span data-stu-id="fff9d-319">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="fff9d-320">Сейчас с помощью этой функции можно передавать только подписки O365 и подписки Azure PAYG (MS-AZR-0145P).</span><span class="sxs-lookup"><span data-stu-id="fff9d-320">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="fff9d-321">Другие покупки, включая планы Azure, зарезервированные экземпляры Azure, подписки на основе терминов и подписки SaaS для Azure Marketplace, не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="fff9d-321">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="fff9d-322">Вы увидите причину, по которой подписка не может быть передана на странице Отправка запроса на передачу.</span><span class="sxs-lookup"><span data-stu-id="fff9d-322">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="fff9d-323">Чтобы переместить эти подписки, необходимо [отменить существующую подписку](create-a-new-subscription.md#suspend-or-cancel-a-subscription) и приобрести новое предложение для клиента через косвенного поставщика.</span><span class="sxs-lookup"><span data-stu-id="fff9d-323">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="fff9d-324">**Невозможно протестировать с помощью среды "песочницы".**</span><span class="sxs-lookup"><span data-stu-id="fff9d-324">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="fff9d-325">Регистрация для поощрения непрямого торгового посредника</span><span class="sxs-lookup"><span data-stu-id="fff9d-325">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="fff9d-326">После успешной регистрации в качестве непрямого торгового посредника у существующего клиента прямого счета вы получите приглашение на регистрацию косвенного стимула для торгового посредника в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="fff9d-326">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="fff9d-327">Приглашение основано на учетной записи партнера MPN, которая в настоящее время связана с вашим клиентом-партнером CSP.</span><span class="sxs-lookup"><span data-stu-id="fff9d-327">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="fff9d-328">Приглашение будет отправлено на адрес электронной почты, связанный с учетной записью партнера MPN.</span><span class="sxs-lookup"><span data-stu-id="fff9d-328">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="fff9d-329">Вы также можете зарегистрироваться для получения программ с прямым выставлением счетов с тем же клиентом-партнером.</span><span class="sxs-lookup"><span data-stu-id="fff9d-329">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="fff9d-330">Необходимо управлять программами отдельно.</span><span class="sxs-lookup"><span data-stu-id="fff9d-330">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fff9d-331">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="fff9d-331">Next steps</span></span>

- [<span data-ttu-id="fff9d-332">Дополнительные сведения о том, как стать косвенным торговым посредником</span><span class="sxs-lookup"><span data-stu-id="fff9d-332">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="fff9d-333">Новые требования к прямым партнерам CSP</span><span class="sxs-lookup"><span data-stu-id="fff9d-333">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="fff9d-334">Ограниченные возможности прямых счетов</span><span class="sxs-lookup"><span data-stu-id="fff9d-334">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
