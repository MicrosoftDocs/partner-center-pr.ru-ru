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
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "91980265"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="3c3c2-103">Перенос подписок на план Azure клиента на другого партнера</span><span class="sxs-lookup"><span data-stu-id="3c3c2-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

## <a name="applies-to"></a><span data-ttu-id="3c3c2-104">Применяется к</span><span class="sxs-lookup"><span data-stu-id="3c3c2-104">Applies to</span></span>

- <span data-ttu-id="3c3c2-105">Партнерам в программе поставщиков облачных решений.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="3c3c2-106">В этой статье описывается, как клиент может переключить свои подписки Azure в рамках плана Azure от одного поставщика облачных решений (CSP) к другому.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="3c3c2-107">Чтобы переключить подписки Azure клиента от другого партнера, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="3c3c2-108">Как партнер, так и клиент имеют необходимые шаги.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="3c3c2-109">Доступ к средствам перехода могут получить только партнеры с прямыми отношениями выставления счетов с корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="3c3c2-110">Косвенные торговые посредники должны работать с непрямыми поставщиками для использования этого средства перехода.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="3c3c2-111">Перед тем как использовать это средство, клиент должен быть в беседе с обоими участниками (текущими и будущими).</span><span class="sxs-lookup"><span data-stu-id="3c3c2-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="3c3c2-112">Автономный диалог должен быть необходим, чтобы избежать путаницы и изменения.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="3c3c2-113">Кроме того, партнеры и клиенты должны понимать эти вопросы и условия перед началом перехода:</span><span class="sxs-lookup"><span data-stu-id="3c3c2-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="3c3c2-114">**Основные моменты:**</span><span class="sxs-lookup"><span data-stu-id="3c3c2-114">**Key considerations:**</span></span>

- <span data-ttu-id="3c3c2-115">Резервирование Azure не будет переноситься с подпиской на будущие партнеры</span><span class="sxs-lookup"><span data-stu-id="3c3c2-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="3c3c2-116">Цены CSP для служб Azure в рамках текущего партнера не будут перенесены</span><span class="sxs-lookup"><span data-stu-id="3c3c2-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="3c3c2-117">Ответственность за поддержку для клиента будет перенесена на будущее партнера</span><span class="sxs-lookup"><span data-stu-id="3c3c2-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="3c3c2-118">Счет и выставление счетов будут перенесены на будущее партнер во время передачи</span><span class="sxs-lookup"><span data-stu-id="3c3c2-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="3c3c2-119">На управление доступом Role-Based Azure (RBAC) не влияет перемещение</span><span class="sxs-lookup"><span data-stu-id="3c3c2-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="3c3c2-120">Администратор от имени (АОБО) не будет предоставляться по умолчанию для будущего партнера</span><span class="sxs-lookup"><span data-stu-id="3c3c2-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="3c3c2-121">Продукты сторонних производителей будут передаваться при условии, что продукты проходят проверку допустимости Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="3c3c2-122">Специальные скидки или региональные ограничения отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="3c3c2-123">Продукты не основаны на подписках</span><span class="sxs-lookup"><span data-stu-id="3c3c2-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="3c3c2-124">Будущий партнер должен работать с издателем, чтобы убедиться, что они находятся в списке разрешений для развертывания продукта.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="3c3c2-125">Если не все эти условия выполнены для передачи продуктов Marketplace, то подписка Azure передается, а затем выполняется повторное приобретение продуктов Marketplace с новым партнером.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="3c3c2-126">**Предварительные условия.**</span><span class="sxs-lookup"><span data-stu-id="3c3c2-126">**Prerequisites:**</span></span>

- <span data-ttu-id="3c3c2-127">Клиент применяет текущего партнера CSP по их намерению к переходу</span><span class="sxs-lookup"><span data-stu-id="3c3c2-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="3c3c2-128">Будущий партнер CSP работает с клиентом для обеспечения соответствия требованиям клиентов.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="3c3c2-129">Будущий партнер по CSP устанавливает связь с клиентом до начала перехода</span><span class="sxs-lookup"><span data-stu-id="3c3c2-129">Future CSP partner establishes a relationship with customer before transition begins</span></span>  
- <span data-ttu-id="3c3c2-130">Клиент должен подписать соглашение клиента Майкрософт с помощью следующего партнера CSP</span><span class="sxs-lookup"><span data-stu-id="3c3c2-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="3c3c2-131">Для использования этого средства в будущем партнере CSP должно быть подписано соглашение Microsoft Partner.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="3c3c2-132">Задачи клиента для выполнения</span><span class="sxs-lookup"><span data-stu-id="3c3c2-132">Customer tasks to be completed</span></span>

<span data-ttu-id="3c3c2-133">Чтобы переместить подписку Azure в рамках плана Azure, клиент должен запустить процесс, обратившись к его текущему партнеру.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="3c3c2-134">Они должны сослать свое имя компании и домен текущего партнера, чтобы их будущий партнер мог заполнять форму запроса на перемещение от их имени.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="3c3c2-135">Клиент должен также указывать подписки, которые они хотят передавать от текущего партнера.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="3c3c2-136">Вы не можете изменить партнеров для Office 365, Enterprise Mobility Suite или подписок Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="3c3c2-137">Он является будущей обязанностью партнера по заполнению формы запроса на перемещение, которая инициирует процесс перемещения.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="3c3c2-138">Корпорация Майкрософт не может проделать от имени клиента или текущего партнера.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="3c3c2-139">Клиент должен работать в тесном сотрудничестве со своим будущим и текущим партнером, чтобы обеспечить плавность перехода.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="3c3c2-140">Будущие задачи партнеров для выполнения</span><span class="sxs-lookup"><span data-stu-id="3c3c2-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="3c3c2-141">Будущий партнер подписки должен заполнить форму запроса на перемещение от центра партнеров, чтобы запросить перенос подписки.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="3c3c2-142">В меню Центр партнеров выберите **Клиенты**, а затем выберите клиента, которому требуется завершить форму запроса на перемещение от имени.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="3c3c2-143">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="3c3c2-144">Выберите раздел **запрос на перемещение** .</span><span class="sxs-lookup"><span data-stu-id="3c3c2-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="3c3c2-145">В **разделе запрос на перемещение**выберите **Добавить новый запрос**.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Раздел &quot;передачи&quot;":::

5.  <span data-ttu-id="3c3c2-147">Заполните **новую форму запроса на перемещение** .</span><span class="sxs-lookup"><span data-stu-id="3c3c2-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="3c3c2-148">Выберите Отправить **запрос на передачу**отправка  >  **Send**.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Раздел &quot;передачи&quot;":::

7.  <span data-ttu-id="3c3c2-150">Подтверждение запроса на перемещение</span><span class="sxs-lookup"><span data-stu-id="3c3c2-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Раздел &quot;передачи&quot;":::

    >[!Note]
    ><span data-ttu-id="3c3c2-152">Будущий партнер может отменить запрос на передачу, выбрав **отменить запрос** в правом верхнем углу, только если состояние запроса на передачу — "ожидание".</span><span class="sxs-lookup"><span data-stu-id="3c3c2-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="3c3c2-153">Когда состояние запроса на перемещение — "выполняется" или "завершено", отмены будут невозможны.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="3c3c2-154">Текущие партнерские задачи для выполнения</span><span class="sxs-lookup"><span data-stu-id="3c3c2-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="3c3c2-155">Агент администрирования текущего партнера клиента получит сообщение электронной почты о том, что клиент запрашивает перенос своих подписок:</span><span class="sxs-lookup"><span data-stu-id="3c3c2-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Раздел &quot;передачи&quot;":::

<span data-ttu-id="3c3c2-157">Проверьте и примите форму запроса на перемещение от центра партнеров, чтобы завершить перенос подписки.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="3c3c2-158">Если текущий партнер не предпримет никаких действий в течение 30 дней, срок действия запроса истечет, и будущий партнер будет иметь возможность создать новый запрос на перемещение.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="3c3c2-159">Выберите **проверить запрос на перемещение** из сообщения электронной почты или</span><span class="sxs-lookup"><span data-stu-id="3c3c2-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="3c3c2-160">В меню Центр партнеров выберите **Клиенты**, а затем выберите клиента, которому был отправлен запрос на перемещение от имени.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="3c3c2-161">В меню клиент выберите пункт **подписки**.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="3c3c2-162">Выберите раздел **запрос на перемещение** .</span><span class="sxs-lookup"><span data-stu-id="3c3c2-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="3c3c2-163">Разверните сведения о переносе, выбрав выбранный **идентификатор запроса на перемещение** в списке **полученных запросов** .</span><span class="sxs-lookup"><span data-stu-id="3c3c2-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Раздел &quot;передачи&quot;":::

5.  <span data-ttu-id="3c3c2-165">Проверка запроса на перемещение.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-165">Review transfer request.</span></span> <span data-ttu-id="3c3c2-166">Выберите запрошенные подписки Azure для перемещения.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="3c3c2-167">Прежде чем продолжать, обратите внимание: у вас больше не будет доступа к выбранным подпискам.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="3c3c2-168">Вы не будете выставлять счета за дальнейшее использование.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="3c3c2-169">Резервирование Azure не передается вместе с подписками.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="3c3c2-170">Затем выберите **принять и переместить** , чтобы завершить процесс перемещения.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Раздел &quot;передачи&quot;":::

7.  <span data-ttu-id="3c3c2-172">Просмотр подтверждения приема на перемещение.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="3c3c2-173">На этом этапе будущий партнер, клиент и текущий партнер будут уведомлены о принятии запроса на перемещение по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="3c3c2-174">После этого переход принимает состояние переноса, которое может остаться в ожидании до 15 минут при обновлении системы.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="3c3c2-175">Если он занимает больше времени, система продолжит попытки в течение трех дней.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="3c3c2-176">Если состояние передачи по-прежнему остается ожидающим, партнер должен отправить запрос на обслуживание.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="3c3c2-177">После завершения перемещения подписки, включенные в запрос, будут отображаться в плане Azure в будущем партнере и больше не будут отображаться вместе с вами.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="3c3c2-178">Для косвенных поставщиков. Сообщите непрямому торговому посреднику, что запрос на перемещение принят.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="3c3c2-179">Управление передаваемыми подписками клиентов</span><span class="sxs-lookup"><span data-stu-id="3c3c2-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="3c3c2-180">Переход не влияет на доступ для существующих пользователей, групп или субъектов-служб, которые были назначены с помощью управления доступом на основе ролей Azure (RBAC).</span><span class="sxs-lookup"><span data-stu-id="3c3c2-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="3c3c2-181">Управление доступом на основе ролей Azure [(Azure RBAC)](/azure/role-based-access-control/overview) помогает Вашим заказчикам управлять доступом к ресурсам Azure, а также тем, что они могут делать с этими ресурсами и к каким областям они имеют доступ.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="3c3c2-182">Так как новому партнеру не предоставляется доступ RBAC к ресурсам клиента после перемещения подписки.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="3c3c2-183">У предыдущего партнера клиента есть доступ RBAC.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="3c3c2-184">Поработайте с клиентом, чтобы понять, кто имеет представление о своих подписках и как вносить необходимые изменения.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="3c3c2-185">Следовательно, важно, чтобы ваш клиент удаляет доступ к Azure RBAC для предыдущего участника и добавляет доступ для нового участника.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="3c3c2-186">Дополнительные сведения о клиенте, предоставляющем новый доступ, см. в статье [что такое управление доступом на основе ролей Azure (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="3c3c2-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="3c3c2-187">Дополнительные сведения о клиентах, удаляющих доступ RBAC предыдущего партнера, см. в разделе [Удаление назначения ролей](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="3c3c2-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="3c3c2-188">Кроме того, вы не получаете автоматическое получение прав [администратора от имени (Аобо)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) к вашим подпискам.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="3c3c2-189">АОБО требуется для партнеров, чтобы управлять подписками Azure клиента от их имени.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="3c3c2-190">Дополнительные сведения о правах доступа Azure см [. в разделе Получение разрешений для управления службой или подпиской клиента.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="3c3c2-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="3c3c2-191">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3c3c2-191">Next steps:</span></span>

- [<span data-ttu-id="3c3c2-192">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="3c3c2-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="3c3c2-193">Получите разрешения для управления службой или подпиской клиента.</span><span class="sxs-lookup"><span data-stu-id="3c3c2-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)