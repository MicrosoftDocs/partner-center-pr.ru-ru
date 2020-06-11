---
title: Консолидация клиента региональной авторизации CSP
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Соблюдайте эти инструкции, чтобы консолидировать клиентов для разных стран и регионов. Сюда входят действия по переносу учетных записей клиентов и клиентских подписок.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: перенос пользователей, подготовка, учетная запись клиента, консолидировать клиенты
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: c2667bf19f73dfb2498cd6f706bd97b595f67a31
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679071"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="a34c7-105">Инструкции для консолидации регионального клиента авторизации CSP</span><span class="sxs-lookup"><span data-stu-id="a34c7-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="a34c7-106">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="a34c7-106">**Applies to**</span></span>

-  <span data-ttu-id="a34c7-107">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="a34c7-107">Partner Center</span></span>
-  <span data-ttu-id="a34c7-108">Центр партнеров для Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="a34c7-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="a34c7-109">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="a34c7-109">**Appropriate roles**</span></span>

- <span data-ttu-id="a34c7-110">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a34c7-110">Global admin</span></span>
- <span data-ttu-id="a34c7-111">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="a34c7-111">Admin agent</span></span>

<span data-ttu-id="a34c7-112">\[Некоторые сведения относятся к предварительно выпущенному продукту, который может быть значительно изменен перед коммерческой выпуском.</span><span class="sxs-lookup"><span data-stu-id="a34c7-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="a34c7-113">Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, относительно предоставленной здесь информации.\]</span><span class="sxs-lookup"><span data-stu-id="a34c7-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="a34c7-114">Соблюдайте эти инструкции, чтобы консолидировать клиентов для разных стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="a34c7-115">Необходимо знать все подписки и количество рабочих мест для клиентов, подготовленных на основе учетных записей перехода.</span><span class="sxs-lookup"><span data-stu-id="a34c7-115">You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="a34c7-116">Вы будете снова настраивать те же самые подписки с тем же числом пользователей в новой учетной записи центрального CSP в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="a34c7-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="a34c7-117">Используйте функцию экспорта, чтобы создать список клиентов для перемещения в централизованный клиент.</span><span class="sxs-lookup"><span data-stu-id="a34c7-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="a34c7-118">Партнеры решают консолидировать своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="a34c7-119">После завершения консолидация партнеры не смогут вернуться в предыдущее состояние.</span><span class="sxs-lookup"><span data-stu-id="a34c7-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="a34c7-120">Также может потребоваться действие клиента.</span><span class="sxs-lookup"><span data-stu-id="a34c7-120">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="a34c7-121">Подготовка к переносу</span><span class="sxs-lookup"><span data-stu-id="a34c7-121">Prepare for migration</span></span>

- <span data-ttu-id="a34c7-122">Войдите в **Центр партнеров** с помощью учетной записи **перехода** (существующей) (которая будет перенесена) и ознакомьтесь со всеми клиентами и всеми службами, подготовленными для этих клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-122">Sign in to **Partner Center**  with the **Transitioning** (existing) account (the one you will transition) and review of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="список региональные клиентов":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="a34c7-124">Миграция учетных записей клиентов</span><span class="sxs-lookup"><span data-stu-id="a34c7-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="a34c7-125">Войдите в **Центр партнеров** с помощью учетной записи **перехода** (новой) (той, в которую вы переходите) и перейдите к списку клиентов из **списка заказчиков.**</span><span class="sxs-lookup"><span data-stu-id="a34c7-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="a34c7-126">Выберите клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-126">Select Customers.</span></span>

3. <span data-ttu-id="a34c7-127">Нажмите кнопку **Запросить установление взаимоотношений с торговым посредником**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="a34c7-128">Вы увидите сообщение по умолчанию для ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="a34c7-129">Это сообщение содержит URL-адрес с уникальным для новой учетной записи Центра партнеров кодом организации.</span><span class="sxs-lookup"><span data-stu-id="a34c7-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="a34c7-130">**Действие клиента:** убедитесь, что каждый из активных клиентов, которого вы хотите перенести, перейдет по этому URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="a34c7-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="a34c7-131">При открытии URL-адреса клиента попросят войти на портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="a34c7-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="a34c7-132">Клиент выполняет вход с помощью того же кода организации, который используется для доступа к порталам администрирования Azure и Office 365.</span><span class="sxs-lookup"><span data-stu-id="a34c7-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="a34c7-133">После входа в систему глобальному администратору учетной записи клиента предлагается отправить соглашение, чтобы предоставить права делегированного администратора новой учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="a34c7-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="a34c7-134">Если администратор соглашается, клиент устанавливает флажок и авторизует отношение.</span><span class="sxs-lookup"><span data-stu-id="a34c7-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="a34c7-135">Клиенты будут отображаться в списке клиентов партнера после отправки соглашения по одному.</span><span class="sxs-lookup"><span data-stu-id="a34c7-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="a34c7-136">Перенос подписок Office 365 и не связанных с Azure подписок с учетом использования</span><span class="sxs-lookup"><span data-stu-id="a34c7-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="a34c7-137">После подписи соглашения клиентом вы можете воссоздать их подписки в рамках централизованного клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="a34c7-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="a34c7-138">В **центре партнеров** выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-138">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="a34c7-139">Откройте название компании клиента, которого вы хотите перенести.</span><span class="sxs-lookup"><span data-stu-id="a34c7-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="a34c7-140">Выберите **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-140">Select **Add subscription**.</span></span>

5. <span data-ttu-id="a34c7-141">Добавьте нужные подписки и число пользователей из каталога.</span><span class="sxs-lookup"><span data-stu-id="a34c7-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="a34c7-142">Проверьте сведения в партнерских учетных записях, **из которых осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="список клиентов":::

6. <span data-ttu-id="a34c7-144">Нажмите кнопку **Отправить.**</span><span class="sxs-lookup"><span data-stu-id="a34c7-144">Click **Submit.**</span></span>

   <span data-ttu-id="a34c7-145">Службы теперь предоставляются клиенту из партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="a34c7-146">Повторите эти действия, чтобы перенести подписки для всех других клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="a34c7-147">Перед переходом к следующему разделу убедитесь, что все подписки клиентов в партнерских учетных записях, **из которых осуществляется перенос**, повторно подготовлены в партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="a34c7-148">Партнеры должны приостановить подписки на **Переход от** учетной записи клиента партнера в центре партнеров на тот же день, когда эти подписки будут перенесены и настроены в рамках **перехода на** учетную запись клиента партнера в центре партнеров, чтобы не происходило двойное выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="a34c7-149">Запросы поддержки будут отклонены из-за любого совпадения выставления счетов, вызванного неправильной настройкой **переносимых** подписок, которые следует отключить.</span><span class="sxs-lookup"><span data-stu-id="a34c7-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="a34c7-150">Отключение подписок Office 365 в переносимой партнерской учетной записи</span><span class="sxs-lookup"><span data-stu-id="a34c7-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="a34c7-151">Отключение подписки CSP в **переносимых** партнерских учетных записях останавливает последующее выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="a34c7-152">Вам не требуется вручную отключать подписки Azure, поскольку они отключаются автоматически в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="a34c7-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="a34c7-153">Войдите в **Центр партнеров** с помощью **перехода из** учетной записи CSP и перейдите к списку клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="a34c7-154">Откройте клиента с подписками, которые необходимо отключить, и выберите первое предложение для отключения.</span><span class="sxs-lookup"><span data-stu-id="a34c7-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="a34c7-155">**Приостановите** подписку и нажмите кнопку **отправить**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="a34c7-156">Приостановка подписки обеспечивает наличие двойного счета.</span><span class="sxs-lookup"><span data-stu-id="a34c7-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="a34c7-157">Теперь подписка отображается в списке как **приостановленная**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="a34c7-158">Повторите эти действия для всех подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="a34c7-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="a34c7-159">Убедитесь, что для всех подписок отображается состояние **приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="a34c7-160">Выберите следующего клиента в списке и повторите процедуру отключения всех подписок.</span><span class="sxs-lookup"><span data-stu-id="a34c7-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="a34c7-161">Миграция Azure подписки с учетом использования</span><span class="sxs-lookup"><span data-stu-id="a34c7-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="a34c7-162">Подписки CSP на основе использования Azure не нуждаются в переносе вручную, как в случае с подписками на Office 365 CSP.</span><span class="sxs-lookup"><span data-stu-id="a34c7-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="a34c7-163">Служба поддержки Microsoft Azure может перенести подписки Azure, а также все развернутые службы или ресурсы из **переносимых** учетных записей CSP торговых посредников в **целевую** учетную запись CSP торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="a34c7-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="a34c7-164">Служба не прекращает работу во время переноса.</span><span class="sxs-lookup"><span data-stu-id="a34c7-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="a34c7-165">Убедитесь, что клиенты, подписки Azure которых необходимо перенести, приняли соглашение для привязки к новой учетной записи CSP, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="a34c7-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="a34c7-166">Партнеры уведомляют Майкрософт, какие учетные записи клиентов с подписками Azure готовы к миграции, и предоставляют названия компаний клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="a34c7-167">Майкрософт переносит подписки Azure с учетом использования и уведомляет партнеров после завершения миграции.</span><span class="sxs-lookup"><span data-stu-id="a34c7-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="a34c7-168">Партнеры подтверждают, что подписка Azure в **переносимых** учетных записях CSP торговых посредников теперь отображается как приостановленная в Центре партнеров в разделе подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="a34c7-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="a34c7-169">Партнеры подтверждают, что подписка Azure в разделе **целевой** учетной записи CSP торгового посредника теперь находится в состоянии **активно** в Центре партнеров в разделе подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="a34c7-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="a34c7-170">Отключение подписок в клиенте не влияет на внешний вид клиента в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="a34c7-171">Сейчас нет возможности удалить клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="a34c7-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="a34c7-172">Партнерам следует избегать повторного добавления подписок к этим клиентам из **переносимой** учетной записи в будущем.</span><span class="sxs-lookup"><span data-stu-id="a34c7-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="a34c7-173">Повторите эти действия для всех подписок всех клиентов, чтобы остановить выставление счетов за **переносимые** учетные записи.</span><span class="sxs-lookup"><span data-stu-id="a34c7-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="a34c7-174">Партнеры получат последний счет с кредитом за неиспользованные дни между датой отмены и последним днем периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="a34c7-175">После этого периода счета больше не будут выставляться.</span><span class="sxs-lookup"><span data-stu-id="a34c7-175">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="a34c7-176">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="a34c7-176">Additional information</span></span>

- <span data-ttu-id="a34c7-177">Отключение подписки от **перехода от** учетной записи CSP не влияет на службу клиента, пока служба была подготовлена из **перехода на** учетную запись CSP перед отключением подписки.</span><span class="sxs-lookup"><span data-stu-id="a34c7-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="a34c7-178">Клиенты не могут использовать подписки и не создают оплату при приостановке или отмене.</span><span class="sxs-lookup"><span data-stu-id="a34c7-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="a34c7-179">Сейчас нет возможности полностью удалить клиента из списка клиентов.</span><span class="sxs-lookup"><span data-stu-id="a34c7-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

    >[!Note]
    > <span data-ttu-id="a34c7-180">Партнеры должны приостановить подписки на **Переход от** учетной записи клиента партнера в центре партнеров на тот же день, когда эти подписки будут перенесены и настроены в рамках **перехода на** учетную запись клиента партнера в центре партнеров, чтобы гарантировать, что двойная оплата не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="a34c7-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="a34c7-181">Корпорация Майкрософт не будет поддерживать запросы на кредиты в связи с перекрытием при выставлении счетов, которое происходит из-за неправильной настройки **перехода от** подписок на приостановленные.</span><span class="sxs-lookup"><span data-stu-id="a34c7-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="a34c7-182">Упрощение миграции с помощью экспорта</span><span class="sxs-lookup"><span data-stu-id="a34c7-182">Simplify migration using Export</span></span>

<span data-ttu-id="a34c7-183">С помощью **функции экспорта** вы можете получить подписки, которые необходимо использовать в новой консолидированной структуре.</span><span class="sxs-lookup"><span data-stu-id="a34c7-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="a34c7-184">Щелкните **Клиенты** в центре партнеров, чтобы просмотреть список клиентов в существующей структуре.</span><span class="sxs-lookup"><span data-stu-id="a34c7-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="a34c7-185">Откройте имя нужного клиента.</span><span class="sxs-lookup"><span data-stu-id="a34c7-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="a34c7-186">На странице **Подписки** щелкните **Экспорт подписок**, чтобы экспортировать данные подписок в файл Excel.</span><span class="sxs-lookup"><span data-stu-id="a34c7-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="a34c7-187">Используйте этот список, чтобы повторного создать подписки в новом консолидированном клиенте.</span><span class="sxs-lookup"><span data-stu-id="a34c7-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="a34c7-188">Регистрация API</span><span class="sxs-lookup"><span data-stu-id="a34c7-188">API registration</span></span>

<span data-ttu-id="a34c7-189">Дополнительные сведения о регистрации API см. [в статье Настройка доступа через API в центре партнеров](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="a34c7-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
