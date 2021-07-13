---
title: Как подтвердить, что ваш клиент принял условия Клиентского соглашения Майкрософт для программы CSP
description: Прежде чем заказывать службы Майкрософт для клиентов, партнеры в рамках программы "Поставщик облачных решений" (CSP) должны подтвердить принятие условий Клиентского соглашения Майкрософт.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277017"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="bce30-103">Как подтвердить, что ваш клиент принял условия Клиентского соглашения Майкрософт для программы CSP</span><span class="sxs-lookup"><span data-stu-id="bce30-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="bce30-104">**Соответствующие роли**: агент по администрированию | агент по продажам</span><span class="sxs-lookup"><span data-stu-id="bce30-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="bce30-105">Клиенты могут принять условия Клиентского соглашения Майкрософт двумя способами.</span><span class="sxs-lookup"><span data-stu-id="bce30-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="bce30-106">**Вариант 1** Утверждение принятия условий партнером. Партнер может подтвердить согласие клиента с помощью API, пакета SDK или панели мониторинга Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="bce30-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="bce30-107">**Вариант 2** Прямое принятие условий клиентом. У партнера есть возможность пригласить клиента с помощью URL-адреса для просмотра и принятия условий соглашения в Центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce30-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="bce30-108">Получение шаблона Клиентского соглашения Майкрософт</span><span class="sxs-lookup"><span data-stu-id="bce30-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="bce30-109">Вы можете вручную скачать последнюю версию шаблона Клиентского соглашения Майкрософт [отсюда](https://aka.ms/customeragreement).</span><span class="sxs-lookup"><span data-stu-id="bce30-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="bce30-110">Клиентские соглашения Майкрософт для разных стран могут отличаться.</span><span class="sxs-lookup"><span data-stu-id="bce30-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="bce30-111">При запросе шаблона Клиентского соглашения Майкрософт обязательно выберите страну, в которой находится клиент.</span><span class="sxs-lookup"><span data-stu-id="bce30-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="bce30-112">Вариант 1. Подтверждение принятия клиентом условий соглашения в Центре партнеров</span><span class="sxs-lookup"><span data-stu-id="bce30-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="bce30-113">Партнеры с прямым выставлением счетов могут подтвердить принятие условий Клиентского соглашения Майкрософт в Центре партнеров для новых и уже имеющихся клиентов.</span><span class="sxs-lookup"><span data-stu-id="bce30-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="bce30-114">Косвенные торговые посредники не могут утверждать принятие условий от имени своих клиентов и должны обращаться к своему непрямому поставщику, чтобы подтвердить согласие клиентов.</span><span class="sxs-lookup"><span data-stu-id="bce30-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="bce30-115">Подтверждение принятия условий соглашения новыми клиентами</span><span class="sxs-lookup"><span data-stu-id="bce30-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="bce30-116">При создании нового клиента в Центре партнеров выполните следующие действия, чтобы подтвердить принятие условий соглашения клиентом.</span><span class="sxs-lookup"><span data-stu-id="bce30-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="bce30-117">Для выполнения этих действий необходимо быть агентом администрирования или агентом по продажам.</span><span class="sxs-lookup"><span data-stu-id="bce30-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="bce30-118">Выберите **Клиенты**, а затем — **Новый клиент**.</span><span class="sxs-lookup"><span data-stu-id="bce30-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="bce30-119">В разделе **Сведения об учетной записи** введите сведения о компании и ее основном контактном лице.</span><span class="sxs-lookup"><span data-stu-id="bce30-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="bce30-120">В разделе **Соглашение корпорации Майкрософт** установите флажок, чтобы подтвердить, что клиент принял условия Клиентского соглашения Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bce30-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="bce30-121">В разделе **Дата принятия условий соглашения** введите соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="bce30-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="bce30-122">Здесь нельзя указать дату, которая еще не наступила.</span><span class="sxs-lookup"><span data-stu-id="bce30-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="bce30-123">Убедитесь, что отображаются правильные контактные данные основного контактного лица.</span><span class="sxs-lookup"><span data-stu-id="bce30-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="bce30-124">Если это не так, выберите **Обновить** и введите точные сведения о лице, принявшем условия соглашения.</span><span class="sxs-lookup"><span data-stu-id="bce30-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="bce30-125">Выберите **Далее**, чтобы продолжить создание арендатора клиента.</span><span class="sxs-lookup"><span data-stu-id="bce30-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Новый клиент":::.  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="bce30-127">Подтвердите согласие клиента для существующих клиентов</span><span class="sxs-lookup"><span data-stu-id="bce30-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="bce30-128">Для выполнения этой процедуры вы должны быть агентом администрирования или агентом по продажам.</span><span class="sxs-lookup"><span data-stu-id="bce30-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="bce30-129">Выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="bce30-129">Select **Customers**.</span></span> <span data-ttu-id="bce30-130">Найдите и выберите клиента.</span><span class="sxs-lookup"><span data-stu-id="bce30-130">Find and select the customer.</span></span>

2. <span data-ttu-id="bce30-131">Выберите **Сведения об учетной записи**.</span><span class="sxs-lookup"><span data-stu-id="bce30-131">Select **Account info**.</span></span>

3. <span data-ttu-id="bce30-132">В разделе **Клиентское соглашение Майкрософт** выберите **Обновить**.</span><span class="sxs-lookup"><span data-stu-id="bce30-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="bce30-133">Введите **Имя**, **Фамилию**, **Адрес электронной почты** и **Номер телефона** (необязательно) пользователя, принявшего условия соглашения.</span><span class="sxs-lookup"><span data-stu-id="bce30-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="bce30-134">В разделе **Дата принятия условий соглашения** введите соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="bce30-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="bce30-135">Здесь нельзя указать дату, которая еще не наступила.</span><span class="sxs-lookup"><span data-stu-id="bce30-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="bce30-136">Выберите **Сохранить** и продолжайте.</span><span class="sxs-lookup"><span data-stu-id="bce30-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Существующий клиент":::.

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="bce30-138">Получение подтверждения о принятии условий клиентом</span><span class="sxs-lookup"><span data-stu-id="bce30-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="bce30-139">Чтобы получить подтверждение того, что существующий клиент принял условия Клиентского соглашения Майкрософт, выполните описанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="bce30-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="bce30-140">Для выполнения этой процедуры вы должны быть агентом администрирования или агентом по продажам.</span><span class="sxs-lookup"><span data-stu-id="bce30-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="bce30-141">Выберите **Клиенты**, а затем найдите и выберите необходимого клиента.</span><span class="sxs-lookup"><span data-stu-id="bce30-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="bce30-142">Выберите **Сведения об учетной записи**.</span><span class="sxs-lookup"><span data-stu-id="bce30-142">Select **Account info**.</span></span>

3. <span data-ttu-id="bce30-143">В разделе **Клиентское соглашение Майкрософт** просмотрите, было ли предоставлено этим клиентом подтверждение.</span><span class="sxs-lookup"><span data-stu-id="bce30-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="bce30-144">Подтверждение принятия клиентом условий использования API или пакета SDK Центра партнеров</span><span class="sxs-lookup"><span data-stu-id="bce30-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="bce30-145">Для подтверждения принятия клиентом условий Клиентского соглашения Майкрософт можно использовать API или пакет SDK Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="bce30-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="bce30-146">Дополнительные сведения об этом API или пакете SDK:</span><span class="sxs-lookup"><span data-stu-id="bce30-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="bce30-147">Получение метаданных соглашения для Клиентского соглашения Майкрософт</span><span class="sxs-lookup"><span data-stu-id="bce30-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="bce30-148">Подтверждение принятия клиентом условий Клиентского соглашения Майкрософт</span><span class="sxs-lookup"><span data-stu-id="bce30-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="bce30-149">Получение подтверждения принятия клиентом условий клиентского соглашения Майкрософт</span><span class="sxs-lookup"><span data-stu-id="bce30-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="bce30-150">Получение ссылки для скачивания шаблона клиентского соглашения Майкрософт</span><span class="sxs-lookup"><span data-stu-id="bce30-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="bce30-151">Вариант 2. Принятие клиентом условий в центре администрирования Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bce30-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="bce30-152">Партнеры могут пригласить новых и существующих клиентов, отправив им соответствующий URL-адрес, чтобы они могли просмотреть и принять условия соглашения в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce30-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="bce30-153">В следующих разделах описывается, как:</span><span class="sxs-lookup"><span data-stu-id="bce30-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="bce30-154">создать клиента и пригласить его для просмотра и принятия условий соглашения;</span><span class="sxs-lookup"><span data-stu-id="bce30-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="bce30-155">пригласить нового клиента для просмотра и принятия условий взаимоотношений с торговым посредником и условий соглашения;</span><span class="sxs-lookup"><span data-stu-id="bce30-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="bce30-156">пригласить имеющегося клиента для просмотра и принятия условий соглашения.</span><span class="sxs-lookup"><span data-stu-id="bce30-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="bce30-157">Вы можете использовать [пакет SDK или API Центра партнеров](/partner-center/develop/get-direct-sign-status-of-customer-agreement), чтобы получить состояние прямого принятия Клиентского соглашения Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bce30-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="bce30-158">Создание клиента и его приглашение для просмотра и принятия условий соглашения</span><span class="sxs-lookup"><span data-stu-id="bce30-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="bce30-159">Выполните следующие действия, чтобы создать учетные данные для клиента в Центре партнеров и пригласить его для просмотра и принятия условий Клиентского соглашения Майкрософт в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce30-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="bce30-160">На вкладке **Клиенты** в Центре партнеров выберите **Добавить клиента**.</span><span class="sxs-lookup"><span data-stu-id="bce30-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="bce30-161">В разделе **Сведения об учетной записи** введите сведения о новом клиенте во всех обязательных полях, включая название компании клиента и основное контактное лицо.</span><span class="sxs-lookup"><span data-stu-id="bce30-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="bce30-162">В разделе **Клиентское соглашение** выберите элемент **Клиенту будет предложено принять Клиентское соглашение Майкрософт в Центре администрирования Microsoft 365**.</span><span class="sxs-lookup"><span data-stu-id="bce30-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="bce30-163">Заполните все остальные обязательные поля на странице.</span><span class="sxs-lookup"><span data-stu-id="bce30-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="bce30-164">Выберите **Далее: отзыв** и выполните инструкции по созданию арендатора клиента.</span><span class="sxs-lookup"><span data-stu-id="bce30-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="bce30-165">Новые клиенты не смогут осуществить покупку, пока не примут условия Клиентского соглашения Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bce30-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Создание нового клиента":::.

5. <span data-ttu-id="bce30-167">При переходе на страницу **Подтверждение** в процессе создания клиента сохраните учетные данные этого клиента.</span><span class="sxs-lookup"><span data-stu-id="bce30-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="bce30-168">Позже эти учетные данные необходимо будет предоставить клиенту.</span><span class="sxs-lookup"><span data-stu-id="bce30-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="bce30-169">Вне Центра партнеров создайте и отправьте клиенту электронное сообщение с приглашением принять условия Клиентского соглашения Майкрософт в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce30-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="bce30-170">Обязательно добавьте в это электронное сообщение:</span><span class="sxs-lookup"><span data-stu-id="bce30-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="bce30-171">ссылку на этот [URL-адрес](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (требуется вход);</span><span class="sxs-lookup"><span data-stu-id="bce30-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="bce30-172">учетные данные клиента, которые вы сохранили на шаге 5.</span><span class="sxs-lookup"><span data-stu-id="bce30-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="bce30-173">Клиент получит приглашение от партнера по электронной почте и перейдет по предложенному [URL-адресу](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="bce30-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="bce30-174">Он войдет в Центр администрирования Microsoft 365, используя предоставленные вами учетные данные.</span><span class="sxs-lookup"><span data-stu-id="bce30-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="bce30-175">Клиент установит флажок, чтобы принять условия Клиентского соглашения Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bce30-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="bce30-176">Приглашение нового клиента для просмотра и принятия условий взаимоотношений с торговым посредником и условий соглашения</span><span class="sxs-lookup"><span data-stu-id="bce30-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="bce30-177">Чтобы пригласить нового клиента для просмотра и принятия условий взаимоотношений с торговым посредником и условий соглашения, выполните следующее.</span><span class="sxs-lookup"><span data-stu-id="bce30-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="bce30-178">На вкладке **Клиенты** в Центре партнеров щелкните ссылку **Запросить установление взаимоотношений с торговым посредником**.</span><span class="sxs-lookup"><span data-stu-id="bce30-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="bce30-179">Будет создан шаблон автоматического электронного сообщения, содержащего текст и ссылку с параметризованным URL-адресом для перехода в центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce30-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="bce30-180">Можно настроить автоматически создаваемый шаблон электронного сообщения, а затем выбрать **Скопировать в буфер обмена** или **Открыть в сообщении электронной почты**.</span><span class="sxs-lookup"><span data-stu-id="bce30-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="bce30-181">Используйте этот шаблон электронного сообщения, чтобы пригласить клиента для принятия запроса на установление **взаимосвязи с торговым посредником** и условий **Клиентского соглашения Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="bce30-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="bce30-182">(Примечание. В электронное приглашение партнер должен также добавить URL-адрес, предоставляемый автоматически, и учетные данные клиента, которые были недавно созданы.)</span><span class="sxs-lookup"><span data-stu-id="bce30-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Создание взаимосвязи":::.

5. <span data-ttu-id="bce30-184">Клиент получит приглашение по электронной почте и щелкнет ссылку на параметризованный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="bce30-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="bce30-185">Для входа в Центр администрирования Microsoft 365 он введет учетные данные, предоставленные вами в электронном сообщении.</span><span class="sxs-lookup"><span data-stu-id="bce30-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="bce30-186">Затем клиент установит флажок, чтобы принять условия **взаимосвязи с торговым посредником** и условия **Клиентского соглашения Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="bce30-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="bce30-187">С помощью того же URL-адреса клиент может просмотреть объединенный список доступных деловых партнеров.</span><span class="sxs-lookup"><span data-stu-id="bce30-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="bce30-188">Он может выбрать партнера для просмотра подробных сведений.</span><span class="sxs-lookup"><span data-stu-id="bce30-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Принятие соглашения.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="bce30-190">Приглашение имеющегося клиента для просмотра и принятия условий соглашения</span><span class="sxs-lookup"><span data-stu-id="bce30-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="bce30-191">Чтобы пригласить имеющегося клиента для просмотра и принятия условий Клиентского соглашения Майкрософт, выполните следующее.</span><span class="sxs-lookup"><span data-stu-id="bce30-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="bce30-192">Создайте электронное сообщение, приглашающее клиента принять условия Клиентского соглашения Майкрософт, и добавьте в него соответствующий URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="bce30-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="bce30-193">Клиент получит приглашение по электронной почте и щелкнет этот [URL-адрес](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="bce30-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="bce30-194">Клиент введет свои учетные данные в Центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce30-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="bce30-195">Затем клиент установит флажок, чтобы принять условия Клиентского соглашения Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bce30-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="bce30-196">С помощью того же URL-адреса он может просмотреть объединенный список доступных деловых партнеров.</span><span class="sxs-lookup"><span data-stu-id="bce30-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="bce30-197">Он может выбрать партнера для просмотра подробных сведений.</span><span class="sxs-lookup"><span data-stu-id="bce30-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Клиент":::.

>[!NOTE]
><span data-ttu-id="bce30-199">В некоторых случаях у клиентов может отсутствовать возможность напрямую принять условия Клиентского соглашения Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bce30-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="bce30-200">Чтобы узнать больше об этих ситуациях, прочтите представленный ниже раздел "Два сценария, в которых требуется утверждение от имени клиента".</span><span class="sxs-lookup"><span data-stu-id="bce30-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="bce30-201">Два сценария, в которых требуется утверждение от имени клиента</span><span class="sxs-lookup"><span data-stu-id="bce30-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="bce30-202">Есть два сценария, в которых клиенты не могут напрямую принять условия Клиентского соглашения Майкрософт в Центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce30-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="bce30-203">**Сценарий 1.** Существующий клиент приобрел что-либо из следующего в рамках установленных партнерских отношений: предложения, программное обеспечение или подписки на него, зарезервированные экземпляры либо план Azure.</span><span class="sxs-lookup"><span data-stu-id="bce30-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="bce30-204">Теперь клиент пытается осуществить новую покупку (это не относится к автоматическому продлению).</span><span class="sxs-lookup"><span data-stu-id="bce30-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="bce30-205">Когда этот клиент щелкнет URL-адрес, он увидит сообщение "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement" (Обратитесь к своему партнеру, чтобы подтвердить согласие с условиями Клиентского соглашения Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="bce30-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="bce30-206">**Как это исправить** Необходимо утвердить принятие условий от имени клиента.</span><span class="sxs-lookup"><span data-stu-id="bce30-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Снимок экрана со страницей Центра администрирования Microsoft 365 и предложением обратиться к партнеру, чтобы подтвердить принятие Клиентского соглашения Майкрософт.":::

<span data-ttu-id="bce30-208">**Сценарий 2** Существующий клиент приобрел что-либо из следующего: предложения, программное обеспечение и подписки на программное обеспечение, зарезервированные экземпляры, план Azure.</span><span class="sxs-lookup"><span data-stu-id="bce30-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="bce30-209">Теперь клиент пытается осуществить новую покупку через нового партнера.</span><span class="sxs-lookup"><span data-stu-id="bce30-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="bce30-210">Когда этот клиент щелкнет ссылку на Центр администрирования Microsoft 365, чтобы принять условия сотрудничества с новым партнером и соглашения, он увидит сообщение "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement" (Обратитесь к своему партнеру, чтобы подтвердить согласие с условиями Клиентского соглашения Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="bce30-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="bce30-211">**Как это исправить** Необходимо утвердить принятие условий от имени клиента.</span><span class="sxs-lookup"><span data-stu-id="bce30-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="bce30-212">Подтверждение того, что клиент принял соглашение</span><span class="sxs-lookup"><span data-stu-id="bce30-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="bce30-213">Если вы пытаетесь создать новый заказ для существующего клиента, от которого еще не получено подтверждение принятия условий соглашения, вам будет предложено выполнить процедуру подтверждения.</span><span class="sxs-lookup"><span data-stu-id="bce30-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="bce30-214">Выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="bce30-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="bce30-215">Введите **Имя**, **Фамилию**, **Адрес электронной почты** и **Номер телефона** (необязательно) пользователя, принявшего условия соглашения.</span><span class="sxs-lookup"><span data-stu-id="bce30-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="bce30-216">В разделе **Дата принятия условий соглашения** введите соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="bce30-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="bce30-217">Здесь нельзя указать дату, которая еще не наступила.</span><span class="sxs-lookup"><span data-stu-id="bce30-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="bce30-218">Выберите **Сохранить и продолжить**.</span><span class="sxs-lookup"><span data-stu-id="bce30-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bce30-219">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="bce30-219">Next steps</span></span>

- [<span data-ttu-id="bce30-220">Проверка или обновление сведений в профиле компании</span><span class="sxs-lookup"><span data-stu-id="bce30-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="bce30-221">Клиентские соглашения Майкрософт (по региону и языку)</span><span class="sxs-lookup"><span data-stu-id="bce30-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
