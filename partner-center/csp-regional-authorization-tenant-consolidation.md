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
ms.openlocfilehash: 695f8298e13680532b63ec24a27d56984bd59c89
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995888"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="7d406-104">Консолидация клиента региональной авторизации CSP</span><span class="sxs-lookup"><span data-stu-id="7d406-104">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="7d406-105">Относится к:</span><span class="sxs-lookup"><span data-stu-id="7d406-105">Applies to</span></span>**

-  <span data-ttu-id="7d406-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="7d406-106">Partner Center</span></span>
-  <span data-ttu-id="7d406-107">Центр партнеров для Microsoft Cloud для правительства США</span><span class="sxs-lookup"><span data-stu-id="7d406-107">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="7d406-108">\[Некоторые сведения относятся к предварительным версиям продуктов, в которые перед коммерческим выпуском могут быть внесены существенные изменения.</span><span class="sxs-lookup"><span data-stu-id="7d406-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="7d406-109">Корпорация Майкрософт не дает никаких гарантий, прямых или косвенных, в отношении указанной здесь информации.\]</span><span class="sxs-lookup"><span data-stu-id="7d406-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="7d406-110">Соблюдайте эти инструкции, чтобы консолидировать клиентов для разных стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="7d406-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="7d406-111">**Примечание**. Необходимо учитывать все подписки и число пользователей для ваших клиентов, подготовленных на основе переходных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7d406-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="7d406-112">Вы будете снова настраивать те же самые подписки с тем же числом пользователей в новой учетной записи центрального CSP в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="7d406-112">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="7d406-113">Используйте функцию экспорта, чтобы создать список клиентов для перемещения в централизованный клиент.</span><span class="sxs-lookup"><span data-stu-id="7d406-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="7d406-114">Партнеры решают консолидировать своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="7d406-115">После завершения консолидация партнеры не смогут вернуться в предыдущее состояние.</span><span class="sxs-lookup"><span data-stu-id="7d406-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="7d406-116">Обратите внимание, что также может потребоваться действие клиента.</span><span class="sxs-lookup"><span data-stu-id="7d406-116">Note that customer action may also be required.</span></span>



## <a name="prepare-for-migration"></a><span data-ttu-id="7d406-117">Подготовка к миграции</span><span class="sxs-lookup"><span data-stu-id="7d406-117">Prepare for migration</span></span>


-   <span data-ttu-id="7d406-118">Войдите **Центр партнеров** с **переходной** (существующей) учетной записью (с той вы перейдете на основную) и запишите всех клиентов и все службы, настроенные для них.</span><span class="sxs-lookup"><span data-stu-id="7d406-118">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![список региональные клиентов](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="7d406-120">Миграция учетных записей клиентов</span><span class="sxs-lookup"><span data-stu-id="7d406-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="7d406-121">Войдите **Центр партнеров** с **переходной** (новое) учетной записью (то, что вы осуществляете переход) и перейдите к списку пользователей от **клиентов**.</span><span class="sxs-lookup"><span data-stu-id="7d406-121">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="7d406-122">Выберите клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-122">Select Customers.</span></span>

3.  <span data-ttu-id="7d406-123">Нажмите кнопку **Запросить установление взаимоотношений с торговым посредником**.</span><span class="sxs-lookup"><span data-stu-id="7d406-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="7d406-124">Вы увидите сообщение по умолчанию для ваших клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="7d406-125">Это сообщение содержит URL-адрес с уникальным для новой учетной записи Центра партнеров кодом организации.</span><span class="sxs-lookup"><span data-stu-id="7d406-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="7d406-126">**Действие клиента:** убедитесь, что каждый из активных клиентов, которого вы хотите перенести, перейдет по этому URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="7d406-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="7d406-127">При открытии URL-адреса клиента попросят войти на портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d406-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="7d406-128">Клиент выполняет вход с помощью того же кода организации, который используется для доступа к порталам администрирования Azure и Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d406-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="7d406-129">После входа в систему глобальному администратору учетной записи клиента предлагается отправить соглашение, чтобы предоставить права делегированного администратора новой учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="7d406-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="7d406-130">Если администратор соглашается, клиент устанавливает флажок и авторизует отношение.</span><span class="sxs-lookup"><span data-stu-id="7d406-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="7d406-131">Клиенты появятся в списке клиентов партнера после отправки соглашения один за одним.</span><span class="sxs-lookup"><span data-stu-id="7d406-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="7d406-132">Перенос подписок Office 365 и не связанных с Azure подписок с учетом использования</span><span class="sxs-lookup"><span data-stu-id="7d406-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="7d406-133">После подписи соглашения клиентом вы можете воссоздать их подписки в рамках централизованного клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="7d406-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="7d406-134">Выберите **клиентов**из **Центра партнеров** .</span><span class="sxs-lookup"><span data-stu-id="7d406-134">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="7d406-135">Откройте название компании клиента, которого вы хотите перенести.</span><span class="sxs-lookup"><span data-stu-id="7d406-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="7d406-136">Нажмите кнопку **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="7d406-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="7d406-137">Добавьте нужные подписки и число пользователей из каталога.</span><span class="sxs-lookup"><span data-stu-id="7d406-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="7d406-138">Проверьте сведения в партнерских учетных записях, **из которых осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="7d406-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

![список клиентов](images/regionalcustomer2.png)

6.  <span data-ttu-id="7d406-140">Нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="7d406-140">Click **Submit.**</span></span>

<span data-ttu-id="7d406-141">Службы теперь предоставляются клиенту из партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="7d406-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="7d406-142">Повторите эти действия, чтобы перенести подписки для всех других клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="7d406-143">Перед переходом к следующему разделу убедитесь, что все подписки клиентов в партнерских учетных записях, **из которых осуществляется перенос**, повторно подготовлены в партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="7d406-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="7d406-144">**Примечание**. Партнерам необходимо приостановить подписки в учетной записи клиента, **из которых осуществляется перенос**, в Центре партнеров в тот же день, в который они переносятся, и настроить их в учетной записи, **в которую осуществляется перенос** в Центре партнеров, чтобы избежать двойного выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7d406-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="7d406-145">Запросы поддержки будут отклонены из-за любого совпадения выставления счетов, вызванного неправильной настройкой **переносимых** подписок, которые следует отключить.</span><span class="sxs-lookup"><span data-stu-id="7d406-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="7d406-146">Отключение подписок Office 365 в переносимой партнерской учетной записи</span><span class="sxs-lookup"><span data-stu-id="7d406-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="7d406-147">Отключение подписки CSP в **переносимых** партнерских учетных записях останавливает последующее выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="7d406-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="7d406-148">Вам не требуется вручную отключать подписки Azure, поскольку они отключаются автоматически в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="7d406-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="7d406-149">Войдите в **Центр партнеров** с помощью учетной записи CSP **Переносимых** и перейдите к списку клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-149">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="7d406-150">Откройте клиента с подписками, которые необходимо отключить, и выберите первое предложение для отключения.</span><span class="sxs-lookup"><span data-stu-id="7d406-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="7d406-151">**Приостановите** подписку и нажмите кнопку **отправить**.</span><span class="sxs-lookup"><span data-stu-id="7d406-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

 >[! **Примечание**]<span data-ttu-id="7d406-152"> Приостановка подписки гарантирует, что двойного выставления счетов не происходит.</span><span class="sxs-lookup"><span data-stu-id="7d406-152"> Suspending the subscription ensures double billing does not occur.</span></span>



~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  <span data-ttu-id="7d406-153">Повторите эти действия для всех подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="7d406-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="7d406-154">Убедитесь, что для всех подписок отображается состояние **приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="7d406-154">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="7d406-155">Выберите следующего клиента в списке и повторите процедуру отключения всех подписок.</span><span class="sxs-lookup"><span data-stu-id="7d406-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="7d406-156">Миграция Azure подписки с учетом использования</span><span class="sxs-lookup"><span data-stu-id="7d406-156">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="7d406-157">Обратите внимание, что подписки CSP Azure на основе использования не нужно переносить вручную, как подписки CSP Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d406-157">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="7d406-158">Служба поддержки Microsoft Azure может перенести подписки Azure, а также все развернутые службы или ресурсы из **переносимых** учетных записей CSP торговых посредников в **целевую** учетную запись CSP торгового посредника.</span><span class="sxs-lookup"><span data-stu-id="7d406-158">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="7d406-159">Служба не прекращает работу во время переноса.</span><span class="sxs-lookup"><span data-stu-id="7d406-159">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="7d406-160">Убедитесь, что клиенты, подписки Azure которых необходимо перенести, приняли соглашение для привязки к новой учетной записи CSP, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="7d406-160">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="7d406-161">Партнеры сообщают корпорации Майкрософт, какие учетные записи клиентов с подписками Azure готовы к миграции, и указывают названия компаний этих клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-161">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="7d406-162">Майкрософт переносит подписки Azure с учетом использования и уведомляет партнеров после завершения миграции.</span><span class="sxs-lookup"><span data-stu-id="7d406-162">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="7d406-163">Партнеры подтверждают, что подписка Azure в **переносимых** учетных записях CSP торговых посредников теперь отображается как приостановленная в Центре партнеров в разделе подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="7d406-163">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="7d406-164">Партнеры подтверждают, что подписка Azure в разделе **целевой** учетной записи CSP торгового посредника теперь находится в состоянии **активно** в Центре партнеров в разделе подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="7d406-164">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

>[! **Примечание**]<span data-ttu-id="7d406-165"> Отключение подписок клиента не изменяет его внешний вид в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-165"> Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="7d406-166">Сейчас нет возможности удалить клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="7d406-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="7d406-167">Партнерам следует избегать повторного добавления подписок к этим клиентам из **переносимой** учетной записи в будущем.</span><span class="sxs-lookup"><span data-stu-id="7d406-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>



6.  <span data-ttu-id="7d406-168">Повторите эти действия для всех подписок всех клиентов, чтобы остановить выставление счетов за **переносимые** учетные записи.</span><span class="sxs-lookup"><span data-stu-id="7d406-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="7d406-169">Партнеры получат последний счет с кредитом за неиспользованные дни между датой отмены и последним днем периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7d406-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="7d406-170">После этого периода счета больше не будут выставляться.</span><span class="sxs-lookup"><span data-stu-id="7d406-170">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="7d406-171">Примечания</span><span class="sxs-lookup"><span data-stu-id="7d406-171">Notes</span></span>

-   <span data-ttu-id="7d406-172">Отключение подписки в **переносимой** учетной записи CSP не влияет на службу клиента, если она была подготовлена на основе **целевой** учетной записи CSP до отключения.</span><span class="sxs-lookup"><span data-stu-id="7d406-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="7d406-173">Клиент не сможет использовать подписки, а после их приостановки или отмены плата за них не взимается.</span><span class="sxs-lookup"><span data-stu-id="7d406-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="7d406-174">Сейчас нет возможности полностью удалить клиента из списка клиентов.</span><span class="sxs-lookup"><span data-stu-id="7d406-174">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="7d406-175">**Примечание**. Партнерам необходимо приостановить подписки в учетной записи клиента, **из которых осуществляется перенос**, в Центре партнеров в тот же день, в который они переносятся, и настроить их в учетной записи, **в которую осуществляется перенос** в Центре партнеров, чтобы избежать двойного выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="7d406-175">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="7d406-176">Корпорация Майкрософт не поддерживает запросы кредитов из-за любого совпадения выставления счетов, вызванного неправильной настройкой **переносимых** подписок, которые следует приостановить.</span><span class="sxs-lookup"><span data-stu-id="7d406-176">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>



### <a name="simplify-migration-using-export"></a><span data-ttu-id="7d406-177">Упрощение миграции с помощью экспорта</span><span class="sxs-lookup"><span data-stu-id="7d406-177">Simplify migration using Export</span></span>

<span data-ttu-id="7d406-178">С помощью **функции экспорта** вы можете получить подписки, которые необходимо использовать в новой консолидированной структуре.</span><span class="sxs-lookup"><span data-stu-id="7d406-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="7d406-179">Выберите **клиентов** в центре партнеров, чтобы просмотреть список клиентов в существующей структуре.</span><span class="sxs-lookup"><span data-stu-id="7d406-179">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="7d406-180">Откройте имя нужного клиента.</span><span class="sxs-lookup"><span data-stu-id="7d406-180">Open the desired customer name.</span></span>

3.  <span data-ttu-id="7d406-181">На странице **Подписки** щелкните **Экспорт подписок**, чтобы экспортировать данные подписок в файл Excel.</span><span class="sxs-lookup"><span data-stu-id="7d406-181">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="7d406-182">Используйте этот список, чтобы повторного создать подписки в новом консолидированном клиенте.</span><span class="sxs-lookup"><span data-stu-id="7d406-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="7d406-183">Регистрация API</span><span class="sxs-lookup"><span data-stu-id="7d406-183">API registration</span></span>

<span data-ttu-id="7d406-184">Дополнительные сведения о регистрации API см. [на этой странице](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="7d406-184">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>








