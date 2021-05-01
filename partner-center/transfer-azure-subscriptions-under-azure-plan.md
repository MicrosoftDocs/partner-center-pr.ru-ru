---
title: Перенос подписки Azure в соответствии с планом Azure другому партнеру CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как изменить партнера по программе поставщика облачных решений, связанный с подписками Azure клиента в плане Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 12afa751d2e7cb6b6ef0cd7308f09746a8a43b52
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284508"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="73aa4-103">Перенос подписок на план Azure клиента на другого партнера</span><span class="sxs-lookup"><span data-stu-id="73aa4-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="73aa4-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="73aa4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="73aa4-105">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="73aa4-105">Account admin</span></span>
- <span data-ttu-id="73aa4-106">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="73aa4-106">Sales agent</span></span>
- <span data-ttu-id="73aa4-107">Агент выставления счетов</span><span class="sxs-lookup"><span data-stu-id="73aa4-107">Billing agent</span></span>

<span data-ttu-id="73aa4-108">В этой статье описывается, как клиент может переключить свои подписки Azure в рамках плана Azure от одного поставщика облачных решений (CSP) к другому.</span><span class="sxs-lookup"><span data-stu-id="73aa4-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="73aa4-109">Чтобы переключить подписки Azure клиента от другого партнера, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="73aa4-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="73aa4-110">Как партнер, так и клиент имеют необходимые шаги.</span><span class="sxs-lookup"><span data-stu-id="73aa4-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="73aa4-111">Доступ к средствам перехода могут получить только партнеры с прямыми отношениями выставления счетов с корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="73aa4-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="73aa4-112">Косвенные торговые посредники должны работать с непрямыми поставщиками для использования этого средства перехода.</span><span class="sxs-lookup"><span data-stu-id="73aa4-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="73aa4-113">Перед тем как использовать это средство, клиент должен быть в беседе с обоими участниками (текущими и будущими).</span><span class="sxs-lookup"><span data-stu-id="73aa4-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="73aa4-114">Автономный диалог должен быть необходим, чтобы избежать путаницы и изменения.</span><span class="sxs-lookup"><span data-stu-id="73aa4-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="73aa4-115">Кроме того, партнеры и клиенты должны понимать эти вопросы и условия перед началом перехода:</span><span class="sxs-lookup"><span data-stu-id="73aa4-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="73aa4-116">**Основные моменты:**</span><span class="sxs-lookup"><span data-stu-id="73aa4-116">**Key considerations:**</span></span>

- <span data-ttu-id="73aa4-117">Резервирование Azure не будет переноситься с подпиской на будущие партнеры</span><span class="sxs-lookup"><span data-stu-id="73aa4-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="73aa4-118">Цены CSP для служб Azure в рамках текущего партнера не будут перенесены</span><span class="sxs-lookup"><span data-stu-id="73aa4-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="73aa4-119">Ответственность за поддержку для клиента будет перенесена на будущее партнера</span><span class="sxs-lookup"><span data-stu-id="73aa4-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="73aa4-120">Счет и выставление счетов будут перенесены на будущее партнер во время передачи</span><span class="sxs-lookup"><span data-stu-id="73aa4-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="73aa4-121">На управление доступом Role-Based Azure (RBAC) не влияет перемещение</span><span class="sxs-lookup"><span data-stu-id="73aa4-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="73aa4-122">Администратор от имени (АОБО) не будет предоставляться по умолчанию для будущего партнера</span><span class="sxs-lookup"><span data-stu-id="73aa4-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="73aa4-123">Продукты сторонних производителей будут передаваться при условии, что продукты проходят проверку допустимости Marketplace.</span><span class="sxs-lookup"><span data-stu-id="73aa4-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="73aa4-124">Специальные скидки или региональные ограничения отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73aa4-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="73aa4-125">Продукты не основаны на подписках</span><span class="sxs-lookup"><span data-stu-id="73aa4-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="73aa4-126">Будущий партнер должен работать с издателем, чтобы убедиться в том, что они находятся в разрешенных для развертывания продукта.</span><span class="sxs-lookup"><span data-stu-id="73aa4-126">The future partner should work with the publisher to make sure they are on the allowlist for deployment of the product</span></span>
    - <span data-ttu-id="73aa4-127">Если не все эти условия выполнены для передачи продуктов Marketplace, то подписка Azure передается, а затем выполняется повторное приобретение продуктов Marketplace с новым партнером.</span><span class="sxs-lookup"><span data-stu-id="73aa4-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="73aa4-128">**Предварительные условия.**</span><span class="sxs-lookup"><span data-stu-id="73aa4-128">**Prerequisites:**</span></span>

- <span data-ttu-id="73aa4-129">Клиент применяет текущего партнера CSP по их намерению к переходу</span><span class="sxs-lookup"><span data-stu-id="73aa4-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="73aa4-130">Будущий партнер CSP работает с клиентом для обеспечения соответствия требованиям клиентов.</span><span class="sxs-lookup"><span data-stu-id="73aa4-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="73aa4-131">Будущий партнер по CSP устанавливает связь с клиентом и приобретает план Azure до начала перехода.</span><span class="sxs-lookup"><span data-stu-id="73aa4-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="73aa4-132">Клиент должен подписать соглашение клиента Майкрософт с помощью следующего партнера CSP</span><span class="sxs-lookup"><span data-stu-id="73aa4-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="73aa4-133">Для использования этого средства в будущем партнере CSP должно быть подписано соглашение Microsoft Partner.</span><span class="sxs-lookup"><span data-stu-id="73aa4-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="73aa4-134">Задачи клиента для выполнения</span><span class="sxs-lookup"><span data-stu-id="73aa4-134">Customer tasks to be completed</span></span>

<span data-ttu-id="73aa4-135">Чтобы переместить подписку Azure в рамках плана Azure, клиент должен запустить процесс, обратившись к его текущему партнеру.</span><span class="sxs-lookup"><span data-stu-id="73aa4-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="73aa4-136">Они должны сослать свое имя компании и домен текущего партнера, чтобы их будущий партнер мог заполнять форму запроса на перемещение от их имени.</span><span class="sxs-lookup"><span data-stu-id="73aa4-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="73aa4-137">Клиент должен также указывать подписки, которые они хотят передавать от текущего партнера.</span><span class="sxs-lookup"><span data-stu-id="73aa4-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="73aa4-138">Вы не можете изменить партнеров для Office 365, Enterprise Mobility Suite или подписок Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="73aa4-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="73aa4-139">Он является будущей обязанностью партнера по заполнению формы запроса на перемещение, которая инициирует процесс перемещения.</span><span class="sxs-lookup"><span data-stu-id="73aa4-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="73aa4-140">Корпорация Майкрософт не может проделать от имени клиента или текущего партнера.</span><span class="sxs-lookup"><span data-stu-id="73aa4-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="73aa4-141">Клиент должен работать в тесном сотрудничестве со своим будущим и текущим партнером, чтобы обеспечить плавность перехода.</span><span class="sxs-lookup"><span data-stu-id="73aa4-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="73aa4-142">Будущие задачи партнеров для выполнения</span><span class="sxs-lookup"><span data-stu-id="73aa4-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="73aa4-143">Будущий партнер подписки должен заполнить форму запроса на перемещение от центра партнеров, чтобы запросить перенос подписки.</span><span class="sxs-lookup"><span data-stu-id="73aa4-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="73aa4-144">В меню Центр партнеров выберите **Клиенты**, а затем выберите клиента, которому требуется завершить форму запроса на перемещение от имени.</span><span class="sxs-lookup"><span data-stu-id="73aa4-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="73aa4-145">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="73aa4-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="73aa4-146">Выберите раздел **запрос на перемещение** .</span><span class="sxs-lookup"><span data-stu-id="73aa4-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="73aa4-147">В **разделе запрос на перемещение** выберите **Добавить новый запрос**.</span><span class="sxs-lookup"><span data-stu-id="73aa4-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Раздел &quot;передачи&quot;":::

5.  <span data-ttu-id="73aa4-149">Заполните **новую форму запроса на перемещение** .</span><span class="sxs-lookup"><span data-stu-id="73aa4-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="73aa4-150">Выберите Отправить **запрос на передачу** отправка  >  .</span><span class="sxs-lookup"><span data-stu-id="73aa4-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Заполнение формы запроса на перемещение":::

7.  <span data-ttu-id="73aa4-152">Подтверждение запроса на перемещение</span><span class="sxs-lookup"><span data-stu-id="73aa4-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Проверка ожидающего перемещения":::

    >[!Note]
    ><span data-ttu-id="73aa4-154">Будущий партнер может отменить запрос на передачу, выбрав **отменить запрос** в правом верхнем углу, только если состояние запроса на передачу — "ожидание".</span><span class="sxs-lookup"><span data-stu-id="73aa4-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="73aa4-155">Когда состояние запроса на перемещение — "выполняется" или "завершено", отмены будут невозможны.</span><span class="sxs-lookup"><span data-stu-id="73aa4-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="73aa4-156">Текущие партнерские задачи для выполнения</span><span class="sxs-lookup"><span data-stu-id="73aa4-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="73aa4-157">Агент администрирования текущего партнера клиента получит сообщение электронной почты о том, что клиент запрашивает перенос своих подписок:</span><span class="sxs-lookup"><span data-stu-id="73aa4-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Просмотр":::

<span data-ttu-id="73aa4-159">Проверьте и примите форму запроса на перемещение от центра партнеров, чтобы завершить перенос подписки.</span><span class="sxs-lookup"><span data-stu-id="73aa4-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="73aa4-160">Если текущий партнер не предпримет никаких действий в течение 30 дней, срок действия запроса истечет, и будущий партнер будет иметь возможность создать новый запрос на перемещение.</span><span class="sxs-lookup"><span data-stu-id="73aa4-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="73aa4-161">Выберите **проверить запрос на перемещение** из сообщения электронной почты или</span><span class="sxs-lookup"><span data-stu-id="73aa4-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="73aa4-162">В меню Центр партнеров выберите **Клиенты**, а затем выберите клиента, которому был отправлен запрос на перемещение от имени.</span><span class="sxs-lookup"><span data-stu-id="73aa4-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="73aa4-163">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="73aa4-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="73aa4-164">Выберите раздел **запрос на перемещение** .</span><span class="sxs-lookup"><span data-stu-id="73aa4-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="73aa4-165">Разверните сведения о переносе, выбрав выбранный **идентификатор запроса на перемещение** в списке **полученных запросов** .</span><span class="sxs-lookup"><span data-stu-id="73aa4-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Запрос на перемещение проверок источника":::

5.  <span data-ttu-id="73aa4-167">Проверка запроса на перемещение.</span><span class="sxs-lookup"><span data-stu-id="73aa4-167">Review transfer request.</span></span> <span data-ttu-id="73aa4-168">Выберите запрошенные подписки Azure для перемещения.</span><span class="sxs-lookup"><span data-stu-id="73aa4-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="73aa4-169">Прежде чем продолжать, обратите внимание: у вас больше не будет доступа к выбранным подпискам.</span><span class="sxs-lookup"><span data-stu-id="73aa4-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="73aa4-170">Вы не будете выставлять счета за дальнейшее использование.</span><span class="sxs-lookup"><span data-stu-id="73aa4-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="73aa4-171">Резервирование Azure не передается вместе с подписками.</span><span class="sxs-lookup"><span data-stu-id="73aa4-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="73aa4-172">Затем выберите **принять и переместить** , чтобы завершить процесс перемещения.</span><span class="sxs-lookup"><span data-stu-id="73aa4-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Выбор подписок для переноса в планах Azure":::

7.  <span data-ttu-id="73aa4-174">Просмотр подтверждения приема на перемещение.</span><span class="sxs-lookup"><span data-stu-id="73aa4-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="73aa4-175">На этом этапе будущий партнер, клиент и текущий партнер будут уведомлены о принятии запроса на перемещение по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="73aa4-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="73aa4-176">После этого переход принимает состояние переноса, которое может остаться в ожидании до 15 минут при обновлении системы.</span><span class="sxs-lookup"><span data-stu-id="73aa4-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="73aa4-177">Если он занимает больше времени, система продолжит попытки в течение трех дней.</span><span class="sxs-lookup"><span data-stu-id="73aa4-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="73aa4-178">Если состояние передачи по-прежнему остается ожидающим, партнер должен отправить запрос на обслуживание.</span><span class="sxs-lookup"><span data-stu-id="73aa4-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="73aa4-179">После завершения перемещения подписки, включенные в запрос, будут отображаться в плане Azure в будущем партнере и больше не будут отображаться вместе с вами.</span><span class="sxs-lookup"><span data-stu-id="73aa4-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="73aa4-180">Для косвенных поставщиков. Сообщите непрямому торговому посреднику, что запрос на перемещение принят.</span><span class="sxs-lookup"><span data-stu-id="73aa4-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="73aa4-181">Управление передаваемыми подписками клиентов</span><span class="sxs-lookup"><span data-stu-id="73aa4-181">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="73aa4-182">Переход не влияет на доступ для существующих пользователей, групп или субъектов-служб, которые были назначены с помощью управления доступом на основе ролей Azure (RBAC).</span><span class="sxs-lookup"><span data-stu-id="73aa4-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="73aa4-183">Управление доступом на основе ролей Azure [(Azure RBAC)](/azure/role-based-access-control/overview) помогает Вашим заказчикам управлять доступом к ресурсам Azure, а также тем, что они могут делать с этими ресурсами и к каким областям они имеют доступ.</span><span class="sxs-lookup"><span data-stu-id="73aa4-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="73aa4-184">Так как новому партнеру не предоставляется доступ RBAC к ресурсам клиента после перемещения подписки.</span><span class="sxs-lookup"><span data-stu-id="73aa4-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="73aa4-185">У предыдущего партнера клиента есть доступ RBAC.</span><span class="sxs-lookup"><span data-stu-id="73aa4-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="73aa4-186">Поработайте с клиентом, чтобы понять, кто имеет представление о своих подписках и как вносить необходимые изменения.</span><span class="sxs-lookup"><span data-stu-id="73aa4-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="73aa4-187">Следовательно, важно, чтобы ваш клиент удаляет доступ к Azure RBAC для предыдущего участника и добавляет доступ для нового участника.</span><span class="sxs-lookup"><span data-stu-id="73aa4-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="73aa4-188">Дополнительные сведения о клиенте, предоставляющем новый доступ, см. в статье [что такое управление доступом на основе ролей Azure (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="73aa4-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="73aa4-189">Дополнительные сведения о клиентах, удаляющих доступ RBAC предыдущего партнера, см. в разделе [Удаление назначения ролей](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="73aa4-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="73aa4-190">Кроме того, вы не получаете автоматическое получение прав [администратора от имени (Аобо)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) к вашим подпискам.</span><span class="sxs-lookup"><span data-stu-id="73aa4-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="73aa4-191">АОБО требуется для партнеров, чтобы управлять подписками Azure клиента от их имени.</span><span class="sxs-lookup"><span data-stu-id="73aa4-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="73aa4-192">Дополнительные сведения о правах доступа Azure см [. в разделе Получение разрешений для управления службой или подпиской клиента.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="73aa4-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="73aa4-193">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="73aa4-193">Next steps:</span></span>

- [<span data-ttu-id="73aa4-194">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="73aa4-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="73aa4-195">Получите разрешения для управления службой или подпиской клиента.</span><span class="sxs-lookup"><span data-stu-id="73aa4-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
