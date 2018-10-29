---
title: Консолидация клиента региональной авторизации CSP | Центр партнеров
ms.topic: article
ms.date: 10/29/2018
description: Соблюдайте эти инструкции, чтобы консолидировать клиентов для разных стран и регионов.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: перенос пользователей, подготовка, учетная запись клиента, консолидировать клиенты
ms.localizationpriority: medium
ms.openlocfilehash: 6285b9dfe88052939a50d6675a190f3e5419cdbb
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2018
ms.locfileid: "5797287"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="ffdcf-104">Консолидация клиента региональной авторизации CSP</span><span class="sxs-lookup"><span data-stu-id="ffdcf-104">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="ffdcf-105">Относится к:</span><span class="sxs-lookup"><span data-stu-id="ffdcf-105">Applies to</span></span>**

-  <span data-ttu-id="ffdcf-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="ffdcf-106">Partner Center</span></span>
-  <span data-ttu-id="ffdcf-107">Центр партнеров для Microsoft Cloud для правительства США</span><span class="sxs-lookup"><span data-stu-id="ffdcf-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="ffdcf-108">Центр партнеров Microsoft Cloud для Германии</span><span class="sxs-lookup"><span data-stu-id="ffdcf-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="ffdcf-109">\[Некоторые сведения относятся к предварительным версиям продуктов, в которые перед коммерческим выпуском могут быть внесены существенные изменения.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-109">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="ffdcf-110">Корпорация Майкрософт не дает никаких гарантий, прямых или косвенных, в отношении указанной здесь информации.\]</span><span class="sxs-lookup"><span data-stu-id="ffdcf-110">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="ffdcf-111">Соблюдайте эти инструкции, чтобы консолидировать клиентов для разных стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-111">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="ffdcf-112">**Примечание**необходимо учитывать все подписки и число пользователей для ваших клиентов, подготовленных на основе переходных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-112">**Note**You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="ffdcf-113">Вы будете снова настраивать те же самые подписки с тем же числом пользователей в новой учетной записи центрального CSP в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-113">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="ffdcf-114">Используйте функцию экспорта, чтобы создать список клиентов для перемещения в централизованный клиент.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-114">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="ffdcf-115">Партнеры решают консолидировать своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-115">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="ffdcf-116">После завершения консолидация партнеры не смогут вернуться в предыдущее состояние.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-116">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="ffdcf-117">Обратите внимание, что также может потребоваться действие клиента.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-117">Note that customer action may also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="ffdcf-118">Подготовка к миграции</span><span class="sxs-lookup"><span data-stu-id="ffdcf-118">Prepare for migration</span></span>


-   <span data-ttu-id="ffdcf-119">Войдите **Центр партнеров** с **переходной** (существующей) учетной записью (с той вы перейдете на основную) и запишите всех клиентов и все службы, настроенные для них.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-119">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![список региональные клиентов](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="ffdcf-121">Миграция учетных записей клиентов</span><span class="sxs-lookup"><span data-stu-id="ffdcf-121">Migrate customer accounts</span></span>


1.  <span data-ttu-id="ffdcf-122">Войдите **Центр партнеров** с **переходной** (новое) учетной записью (то, что вы осуществляете переход) и перейдите к списку пользователей от **клиентов**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-122">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="ffdcf-123">Выберите клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-123">Select Customers.</span></span>

3.  <span data-ttu-id="ffdcf-124">Нажмите кнопку **Запросить установление взаимоотношений с торговым посредником**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-124">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="ffdcf-125">Вы увидите сообщение по умолчанию для ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-125">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="ffdcf-126">Это сообщение содержит URL-адрес с уникальным для новой учетной записи Центра партнеров кодом организации.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-126">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="ffdcf-127">**Действие клиента:** убедитесь, что каждый из активных клиентов, которого вы хотите перенести, перейдет по этому URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-127">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="ffdcf-128">При открытии URL-адреса клиента попросят войти на портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-128">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="ffdcf-129">Клиент выполняет вход с помощью того же кода организации, который используется для доступа к порталам администрирования Azure и Office 365.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-129">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="ffdcf-130">После входа в систему глобальному администратору учетной записи клиента предлагается отправить соглашение, чтобы предоставить права делегированного администратора новой учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-130">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="ffdcf-131">Если администратор соглашается, клиент устанавливает флажок и авторизует отношение.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-131">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="ffdcf-132">Клиенты появятся в списке клиентов партнера после отправки соглашения один за одним.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-132">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="ffdcf-133">Перенос подписок Office 365 и не связанных с Azure подписок с учетом использования</span><span class="sxs-lookup"><span data-stu-id="ffdcf-133">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="ffdcf-134">После подписи соглашения клиентом вы можете воссоздать их подписки в рамках централизованного клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-134">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="ffdcf-135">Выберите **клиентов**в **Центре партнеров** .</span><span class="sxs-lookup"><span data-stu-id="ffdcf-135">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="ffdcf-136">Откройте название компании клиента, которого вы хотите перенести.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-136">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="ffdcf-137">Нажмите кнопку **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-137">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="ffdcf-138">Добавьте нужные подписки и число пользователей из каталога.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-138">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="ffdcf-139">Проверьте сведения в партнерских учетных записях, **из которых осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-139">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![снимок экрана: список клиентов](images/regionalcustomer2.png)

6.  <span data-ttu-id="ffdcf-141">Нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-141">Click **Submit.**</span></span>

<span data-ttu-id="ffdcf-142">Службы теперь предоставляются клиенту из партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-142">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ffdcf-143">Повторите эти действия, чтобы перенести подписки для всех других клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-143">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="ffdcf-144">Перед переходом к следующему разделу убедитесь, что все подписки клиентов в партнерских учетных записях, **из которых осуществляется перенос**, повторно подготовлены в партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-144">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ffdcf-145">**Примечание**партнерам необходимо приостановить подписки, в **Переносимой** партнерской учетной записи клиента в центре партнеров тот же день, они преобразованы и настройка в **Которую осуществляется перенос** клиента партнера учетной записи в в центр партнеров, чтобы избежать двойного выставления счетов не происходит.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-145">**Note**Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ffdcf-146">Запросы поддержки будут отклонены из-за любого совпадения выставления счетов, вызванного неправильной настройкой **переносимых** подписок, которые следует отключить.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-146">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="ffdcf-147">Отключение подписок Office 365 в переносимой партнерской учетной записи</span><span class="sxs-lookup"><span data-stu-id="ffdcf-147">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="ffdcf-148">Отключение подписки CSP в **переносимых** партнерских учетных записях останавливает последующее выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-148">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="ffdcf-149">Вам не требуется вручную отключать подписки Azure, поскольку они отключаются автоматически в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-149">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="ffdcf-150">Войдите в **Центр партнеров** с помощью учетной записи CSP **Переносимых** и перейдите к списку клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-150">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="ffdcf-151">Откройте клиента с подписками, которые необходимо отключить, и выберите первое предложение для отключения.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-151">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="ffdcf-152">**Приостановите** подписку и нажмите кнопку **отправить**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-152">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="ffdcf-153">**Примечание**Приостановка подписки гарантирует двойного выставления счетов не.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-153">**Note**Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="ffdcf-154">Теперь подписка отображается в списке как **приостановленная**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-154">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="ffdcf-155">Повторите эти действия для всех подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-155">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="ffdcf-156">Убедитесь, что для всех подписок отображается состояние **приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-156">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="ffdcf-157">Выберите следующего клиента в списке и повторите процедуру отключения всех подписок.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-157">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="ffdcf-158">Миграция Azure подписки с учетом использования</span><span class="sxs-lookup"><span data-stu-id="ffdcf-158">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="ffdcf-159">Обратите внимание, что подписки CSP Azure на основе использования не нужно переносить вручную, как подписки CSP Office 365.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-159">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="ffdcf-160">Служба поддержки Microsoft Azure может перенести подписки Azure, а также все развернутые службы или ресурсы из **переносимых** учетных записей CSP торговых посредников в **целевую** учетную запись CSP торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-160">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="ffdcf-161">Служба не прекращает работу во время переноса.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-161">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="ffdcf-162">Убедитесь, что клиенты, подписки Azure которых необходимо перенести, приняли соглашение для привязки к новой учетной записи CSP, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-162">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="ffdcf-163">Партнеры сообщают корпорации Майкрософт, какие учетные записи клиентов с подписками Azure готовы к миграции, и указывают названия компаний этих клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-163">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="ffdcf-164">Майкрософт переносит подписки Azure с учетом использования и уведомляет партнеров после завершения миграции.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-164">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="ffdcf-165">Партнеры подтверждают, что подписка Azure в **переносимых** учетных записях CSP торговых посредников теперь отображается как приостановленная в Центре партнеров в разделе подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-165">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="ffdcf-166">Партнеры подтверждают, что подписка Azure в разделе **целевой** учетной записи CSP торгового посредника теперь находится в состоянии **активно** в Центре партнеров в разделе подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-166">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="ffdcf-167">**Примечание**отключение подписок клиента не изменяет его внешний вид в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-167">**Note**Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="ffdcf-168">Сейчас нет возможности удалить клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-168">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="ffdcf-169">Партнерам следует избегать повторного добавления подписок к этим клиентам из **переносимой** учетной записи в будущем.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-169">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="ffdcf-170">Повторите эти действия для всех подписок всех клиентов, чтобы остановить выставление счетов за **переносимые** учетные записи.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-170">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="ffdcf-171">Партнеры получат последний счет с кредитом за неиспользованные дни между датой отмены и последним днем периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-171">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="ffdcf-172">После этого периода счета больше не будут выставляться.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-172">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="ffdcf-173">Примечания</span><span class="sxs-lookup"><span data-stu-id="ffdcf-173">Notes</span></span>

-   <span data-ttu-id="ffdcf-174">Отключение подписки в **переносимой** учетной записи CSP не влияет на службу клиента, если она была подготовлена на основе **целевой** учетной записи CSP до отключения.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-174">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="ffdcf-175">Клиент не сможет использовать подписки, а после их приостановки или отмены плата за них не взимается.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-175">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="ffdcf-176">Сейчас нет возможности полностью удалить клиента из списка клиентов.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-176">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="ffdcf-177">**Примечание**партнерам необходимо приостановить подписки в **Переносимой** партнерской учетной записи клиента в центре партнеров тот же день, они преобразованы в и настройка под учетной записью **Целевой** клиента партнера в центре партнеров, чтобы избежать двойного выставления счетов не происходит.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-177">**Note**Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ffdcf-178">Корпорация Майкрософт не поддерживает запросы кредитов из-за любого совпадения выставления счетов, вызванного неправильной настройкой **переносимых** подписок, которые следует приостановить.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-178">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="ffdcf-179">Упрощение миграции с помощью экспорта</span><span class="sxs-lookup"><span data-stu-id="ffdcf-179">Simplify migration using Export</span></span>

<span data-ttu-id="ffdcf-180">С помощью **функции экспорта** вы можете получить подписки, которые необходимо использовать в новой консолидированной структуре.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-180">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="ffdcf-181">Выберите **клиентов** в центре партнеров, чтобы просмотреть список клиентов в существующей структуре.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-181">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="ffdcf-182">Откройте имя нужного клиента.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-182">Open the desired customer name.</span></span>

3.  <span data-ttu-id="ffdcf-183">На странице **Подписки** щелкните **Экспорт подписок**, чтобы экспортировать данные подписок в файл Excel.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-183">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="ffdcf-184">Используйте этот список, чтобы повторного создать подписки в новом консолидированном клиенте.</span><span class="sxs-lookup"><span data-stu-id="ffdcf-184">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="ffdcf-185">Регистрация API</span><span class="sxs-lookup"><span data-stu-id="ffdcf-185">API registration</span></span>

<span data-ttu-id="ffdcf-186">Дополнительные сведения о регистрации API см. [на этой странице](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="ffdcf-186">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>


 

 



