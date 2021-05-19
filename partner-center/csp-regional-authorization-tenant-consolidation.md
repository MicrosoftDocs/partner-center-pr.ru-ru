---
title: Консолидация клиента региональной авторизации CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Соблюдайте эти инструкции, чтобы консолидировать клиентов для разных стран и регионов. Сюда входят действия по переносу учетных записей клиентов и клиентских подписок.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147587"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="6475a-104">Инструкции по консолидации клиента региональной авторизации CSP</span><span class="sxs-lookup"><span data-stu-id="6475a-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="6475a-105">Область **применения**: центр партнеров | Центр партнеров по Microsoft Cloud для государственных организаций США</span><span class="sxs-lookup"><span data-stu-id="6475a-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6475a-106">**Соответствующие роли**: глобальный администратор | Агент администратора</span><span class="sxs-lookup"><span data-stu-id="6475a-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="6475a-107">\[Некоторые сведения относятся к предварительно выпущенному продукту, который может быть значительно изменен перед коммерческой выпуском.</span><span class="sxs-lookup"><span data-stu-id="6475a-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="6475a-108">Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, относительно приведенных здесь сведений.\]</span><span class="sxs-lookup"><span data-stu-id="6475a-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="6475a-109">Вы можете консолидировать клиенты для вашего бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6475a-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="6475a-110">Соблюдайте эти инструкции, чтобы консолидировать клиентов для разных стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="6475a-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="6475a-111">Необходимо знать все подготовленные подписки и количество лицензий для каждого из клиентов в учетной записи, из которой выполняется переход.</span><span class="sxs-lookup"><span data-stu-id="6475a-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="6475a-112">Вы будете повторно подготавливаем те же самые подписки с теми же подсчетами лицензий в рамках новой Центральной учетной записи CSP в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="6475a-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="6475a-113">Используйте функцию экспорта, чтобы создать список клиентов для перемещения в централизованный клиент.</span><span class="sxs-lookup"><span data-stu-id="6475a-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="6475a-114">После завершения консолидации нельзя вернуться к предыдущему состоянию клиента.</span><span class="sxs-lookup"><span data-stu-id="6475a-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="6475a-115">Также может потребоваться действие клиента.</span><span class="sxs-lookup"><span data-stu-id="6475a-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="6475a-116">Подготовка к переносу</span><span class="sxs-lookup"><span data-stu-id="6475a-116">Prepare for migration</span></span>

- <span data-ttu-id="6475a-117">Войдите в **Центр партнеров**  , используя учетную запись **перехода** (ту, которая будет переходить на новую учетную запись), и ознакомьтесь со всеми клиентами и всеми службами, подготовленными для этих клиентов.</span><span class="sxs-lookup"><span data-stu-id="6475a-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="6475a-118">Выйти из этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6475a-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="6475a-119">Миграция учетных записей клиентов</span><span class="sxs-lookup"><span data-stu-id="6475a-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="6475a-120">Войдите в **Центр партнеров**  с помощью учетной записи **перехода** (новой) (той, в которую вы переходите заказчики).</span><span class="sxs-lookup"><span data-stu-id="6475a-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="6475a-121">Выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="6475a-121">Select **Customers**.</span></span>

3. <span data-ttu-id="6475a-122">Выберите **запросить связь через торгового посредника**.</span><span class="sxs-lookup"><span data-stu-id="6475a-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="6475a-123">Вы получите сообщение электронной почты по умолчанию для отправки клиентам.</span><span class="sxs-lookup"><span data-stu-id="6475a-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="6475a-124">Это сообщение содержит URL-адрес с уникальным для новой учетной записи Центра партнеров кодом организации.</span><span class="sxs-lookup"><span data-stu-id="6475a-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="6475a-125">**Действие клиента:** убедитесь, что каждый из активных клиентов, которого вы хотите перенести, перейдет по этому URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="6475a-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="6475a-126">При открытии URL-адреса клиента попросят войти на портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="6475a-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="6475a-127">Клиент выполняет вход с помощью того же кода организации, который используется для доступа к порталам администрирования Azure и Office 365.</span><span class="sxs-lookup"><span data-stu-id="6475a-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="6475a-128">После входа в систему глобального администратора для **учетной записи клиента** будет предложено отправить соглашение, предоставляющее права делегированного администратора новой учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="6475a-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="6475a-129">Если администратор соглашается, клиент устанавливает флажок и авторизует отношение.</span><span class="sxs-lookup"><span data-stu-id="6475a-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="6475a-130">Клиенты будут отображаться в списке клиентов партнера после отправки соглашения по одному.</span><span class="sxs-lookup"><span data-stu-id="6475a-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="6475a-131">Перенос подписок Office 365 и не связанных с Azure подписок с учетом использования</span><span class="sxs-lookup"><span data-stu-id="6475a-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="6475a-132">После подписи соглашения клиентом вы можете воссоздать их подписки в рамках централизованного клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="6475a-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="6475a-133">В **центре партнеров** выберите **Клиенты**.</span><span class="sxs-lookup"><span data-stu-id="6475a-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="6475a-134">Откройте название компании клиента, которого вы хотите перенести.</span><span class="sxs-lookup"><span data-stu-id="6475a-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="6475a-135">Выберите **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="6475a-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="6475a-136">Добавьте правильные подписки и подсчеты лицензий из каталога.</span><span class="sxs-lookup"><span data-stu-id="6475a-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="6475a-137">Проверьте сведения в партнерских учетных записях, **из которых осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="6475a-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="список клиентов":::

6. <span data-ttu-id="6475a-139">Выберите **Отправить.**</span><span class="sxs-lookup"><span data-stu-id="6475a-139">Select **Submit.**</span></span>

   <span data-ttu-id="6475a-140">Службы теперь предоставляются клиенту из партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="6475a-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="6475a-141">Повторите эти действия, чтобы перенести подписки для всех других клиентов.</span><span class="sxs-lookup"><span data-stu-id="6475a-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="6475a-142">Перед переходом к следующему разделу убедитесь, что все подписки клиентов в партнерских учетных записях, **из которых осуществляется перенос**, повторно подготовлены в партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="6475a-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="6475a-143">Партнеры должны приостановить подписки на **Переход от** учетной записи клиента партнера в центре партнеров на тот же день, когда эти подписки будут перенесены и настроены в рамках **перехода на** учетную запись клиента партнера в центре партнеров, чтобы не происходило двойное выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="6475a-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="6475a-144">Запросы в службу поддержки будут отвергнуты для кредитов из-за перекрытия при выставлении счетов, которое происходит после неправильного отключения **перехода от** подписок.</span><span class="sxs-lookup"><span data-stu-id="6475a-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="6475a-145">Отключение подписок Office 365 в переносимой партнерской учетной записи</span><span class="sxs-lookup"><span data-stu-id="6475a-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="6475a-146">Отключение подписки CSP в **переносимых** партнерских учетных записях останавливает последующее выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="6475a-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="6475a-147">Вам не нужно вручную отключать подписки Azure, так как подписки Azure автоматически отключаются в процессе миграции.</span><span class="sxs-lookup"><span data-stu-id="6475a-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="6475a-148">Войдите в **Центр партнеров** с помощью **перехода из** учетной записи CSP и перейдите к списку клиентов.</span><span class="sxs-lookup"><span data-stu-id="6475a-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="6475a-149">Откройте клиента с подписками, которые необходимо отключить, и выберите первое предложение для отключения.</span><span class="sxs-lookup"><span data-stu-id="6475a-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="6475a-150">Установите для подписки значение **приостановлено** и нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="6475a-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="6475a-151">Приостановка подписки обеспечивает наличие двойного счета.</span><span class="sxs-lookup"><span data-stu-id="6475a-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="6475a-152">Подписка отображается как **приостановленная** в списке подписок.</span><span class="sxs-lookup"><span data-stu-id="6475a-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="6475a-153">Повторите эти действия для всех подписок клиента.</span><span class="sxs-lookup"><span data-stu-id="6475a-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="6475a-154">Убедитесь, что для всех подписок отображается состояние **приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="6475a-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="6475a-155">Выберите следующего клиента в списке и повторите процедуру отключения всех подписок.</span><span class="sxs-lookup"><span data-stu-id="6475a-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="6475a-156">Миграция Azure подписки с учетом использования</span><span class="sxs-lookup"><span data-stu-id="6475a-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="6475a-157">В отличие от подписок CSP для Office 365, в Azure не требуется ручная миграция подписок CSP на основе использования.</span><span class="sxs-lookup"><span data-stu-id="6475a-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="6475a-158">Microsoft Azure поддержка перенесет подписки Azure и все развернутые службы или ресурсы из учетных записей торгового посредника CSP в **Переход на** учетную запись торгового посредника **CSP.**</span><span class="sxs-lookup"><span data-stu-id="6475a-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="6475a-159">Служба не прекращает работу во время переноса.</span><span class="sxs-lookup"><span data-stu-id="6475a-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="6475a-160">Убедитесь, что все учетные записи клиентов, которые будут перенесены с помощью подписок Azure, приняли соглашение о том, что оно будет связано с новым **переходом к** учетной записи CSP.</span><span class="sxs-lookup"><span data-stu-id="6475a-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="6475a-161">Вы получите уведомление корпорации Майкрософт о том, какие учетные записи клиентов готовы к миграции, и укажите названия компаний клиентов.</span><span class="sxs-lookup"><span data-stu-id="6475a-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="6475a-162">Корпорация Майкрософт перенесет подписки на основе использования Azure и уведомляет вас о завершении миграции.</span><span class="sxs-lookup"><span data-stu-id="6475a-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="6475a-163">Необходимо подтвердить, что подписка Azure в рамках **перехода от** учетной записи торгового посредника CSP теперь помечена как " **приостановлено** " в центре партнеров в разделе "подписки клиентов".</span><span class="sxs-lookup"><span data-stu-id="6475a-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="6475a-164">Убедитесь, что подписка Azure в учетной записи торгового посредника " **Переход к** CSP" теперь показывает состояние " **активно** " в центре партнеров в разделе "подписки клиентов".</span><span class="sxs-lookup"><span data-stu-id="6475a-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="6475a-165">Отключение подписок в клиенте не влияет на внешний вид клиента в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="6475a-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="6475a-166">Сейчас нет возможности удалить клиентов из списка.</span><span class="sxs-lookup"><span data-stu-id="6475a-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="6475a-167">Партнерам следует избегать повторного добавления подписок к этим клиентам из **переносимой** учетной записи в будущем.</span><span class="sxs-lookup"><span data-stu-id="6475a-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="6475a-168">Повторите эти действия для всех подписок всех клиентов, чтобы остановить выставление счетов за **переносимые** учетные записи.</span><span class="sxs-lookup"><span data-stu-id="6475a-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="6475a-169">Партнеры получат последний счет с кредитом за неиспользованные дни между датой отмены и последним днем периода выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="6475a-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="6475a-170">После этого периода счета больше не будут выставляться.</span><span class="sxs-lookup"><span data-stu-id="6475a-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="6475a-171">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="6475a-171">Additional information</span></span>

- <span data-ttu-id="6475a-172">Отключение подписки от **перехода от** учетной записи CSP не влияет на службу клиента, пока служба была подготовлена из **перехода на** учетную запись CSP перед отключением подписки.</span><span class="sxs-lookup"><span data-stu-id="6475a-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="6475a-173">Клиенты не могут использовать подписки и не создают оплату при приостановке или отмене.</span><span class="sxs-lookup"><span data-stu-id="6475a-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="6475a-174">В настоящее время нет возможности полностью удалить клиента из списка **клиентов** .</span><span class="sxs-lookup"><span data-stu-id="6475a-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="6475a-175">Партнеры должны приостанавливать подписки на **Переход от** учетной записи клиента партнера в центре партнеров на тот же день, когда эти подписки переходят в и настроены в рамках **перехода на** учет, чтобы гарантировать, что двойная оплата не будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="6475a-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="6475a-176">Корпорация Майкрософт не будет поддерживать запросы на кредиты в связи с перекрытием при выставлении счетов, которое происходит из-за неправильной настройки **перехода от** подписок на приостановленные.</span><span class="sxs-lookup"><span data-stu-id="6475a-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="6475a-177">Упрощение миграции с помощью экспорта</span><span class="sxs-lookup"><span data-stu-id="6475a-177">Simplify migration using Export</span></span>

<span data-ttu-id="6475a-178">С помощью **функции экспорта** вы можете получить подписки, которые необходимо использовать в новой консолидированной структуре.</span><span class="sxs-lookup"><span data-stu-id="6475a-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="6475a-179">Выберите **Клиенты** в центре партнеров, чтобы просмотреть список клиентов.</span><span class="sxs-lookup"><span data-stu-id="6475a-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="6475a-180">Откройте имя нужного клиента.</span><span class="sxs-lookup"><span data-stu-id="6475a-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="6475a-181">На странице **подписки** выберите **Экспорт подписок** для экспорта сведений о подписках в файл Excel.</span><span class="sxs-lookup"><span data-stu-id="6475a-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="6475a-182">Используйте этот список, чтобы повторного создать подписки в новом консолидированном клиенте.</span><span class="sxs-lookup"><span data-stu-id="6475a-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="6475a-183">Регистрация API</span><span class="sxs-lookup"><span data-stu-id="6475a-183">API registration</span></span>

<span data-ttu-id="6475a-184">Дополнительные сведения о регистрации API см. [в статье Настройка доступа через API в центре партнеров](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="6475a-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6475a-185">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="6475a-185">Next steps</span></span>

- [<span data-ttu-id="6475a-186">Региональные рынки и валюты поставщика облачных решений, где можно продать предложения CSP</span><span class="sxs-lookup"><span data-stu-id="6475a-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
