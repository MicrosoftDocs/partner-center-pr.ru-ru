---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="5b4b9-103">CSP regional authorization tenant consolidation</span><span class="sxs-lookup"><span data-stu-id="5b4b9-103">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="5b4b9-104">Applies to</span><span class="sxs-lookup"><span data-stu-id="5b4b9-104">Applies to</span></span>**

-  <span data-ttu-id="5b4b9-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="5b4b9-105">Partner Center</span></span>
-  <span data-ttu-id="5b4b9-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="5b4b9-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="5b4b9-107">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="5b4b9-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="5b4b9-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="5b4b9-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span><span class="sxs-lookup"><span data-stu-id="5b4b9-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="5b4b9-110">Use these instructions to consolidate tenants for different country/regions.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="5b4b9-111">**Примечание**. Необходимо учитывать все подписки и число пользователей для ваших клиентов, подготовленных на основе переходных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="5b4b9-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="5b4b9-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="5b4b9-114">Partners choose to consolidate their tenants.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="5b4b9-115">Once consolidation is complete, Partners cannot revert to their previous state.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="5b4b9-116">Note that customer action is also be required.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-116">Note that customer action is also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="5b4b9-117">Prepare for migration</span><span class="sxs-lookup"><span data-stu-id="5b4b9-117">Prepare for migration</span></span>


-   <span data-ttu-id="5b4b9-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span></span>

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="5b4b9-120">Migrate customer accounts</span><span class="sxs-lookup"><span data-stu-id="5b4b9-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="5b4b9-121">Войдите на страницу <https://partnercenter.microsoft.com> с переходной (новой) учетной записью и перейдите к списку клиентов на информационной панели Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-121">Log on to <https://partnercenter.microsoft.com> with the Transitioning (new) account and navigate to the Customers list from the Partner Center dashboard.</span></span>

2.  <span data-ttu-id="5b4b9-122">Select Customer.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-122">Select Customer.</span></span>

3.  <span data-ttu-id="5b4b9-123">Нажмите кнопку **Запросить установление взаимоотношений с торговым посредником**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="5b4b9-124">You are presented with a default email message to present to your customers.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="5b4b9-125">This message contains a URL with the org ID unique to your new Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="5b4b9-126">**Действие клиента:** убедитесь, что каждый из активных клиентов, которого вы хотите перенести, перейдет по этому URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="5b4b9-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="5b4b9-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="5b4b9-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="5b4b9-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="5b4b9-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="5b4b9-132">Migrating Office 365 and non-Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="5b4b9-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="5b4b9-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="5b4b9-134">На информационной панели в Центре партнеров щелкните **Клиенты** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-134">On the Partner Center Dashboard click on **Customers** in the left navigation</span></span>

3.  <span data-ttu-id="5b4b9-135">Open the company name for the customer you want to migrate.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="5b4b9-136">Нажмите кнопку **Добавить подписку**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="5b4b9-137">Add the correct subscriptions and seat counts from the catalog.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="5b4b9-138">Проверьте сведения в партнерских учетных записях, **из которых осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  <span data-ttu-id="5b4b9-140">Нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-140">Click **Submit.**</span></span>

<span data-ttu-id="5b4b9-141">Службы теперь предоставляются клиенту из партнерской учетной записи, **в которую осуществляется перенос**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="5b4b9-142">Repeat these steps to migrate subscriptions for all additional customers.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="5b4b9-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="5b4b9-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="5b4b9-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="5b4b9-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span><span class="sxs-lookup"><span data-stu-id="5b4b9-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="5b4b9-147">Отключение подписки CSP в **переносимых** партнерских учетных записях останавливает последующее выставление счетов.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="5b4b9-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="5b4b9-149">Войдите на веб-сайт <https://partnercenter.microsoft.com> с **переносимой** учетной записью CSP и перейдите в список клиентов.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-149">Log on to <https://partnercenter.microsoft.com> with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="5b4b9-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="5b4b9-151">**Приостановите** подписку и нажмите кнопку **отправить**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="5b4b9-152">**Примечание**. Приостановка подписки гарантирует отсутствие двойного выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-152">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="5b4b9-153">Теперь подписка отображается в списке как **приостановленная**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-153">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="5b4b9-154">Repeat these steps for all subscriptions under the customer.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-154">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="5b4b9-155">Убедитесь, что для всех подписок отображается состояние **приостановлено**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-155">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="5b4b9-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="5b4b9-157">Migrating Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="5b4b9-157">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="5b4b9-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="5b4b9-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="5b4b9-160">There will be no disruption of service to the customer during this transition.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-160">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="5b4b9-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="5b4b9-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="5b4b9-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="5b4b9-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="5b4b9-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="5b4b9-166">**Примечание**. Отключение подписок клиента не изменяет его внешний вид в списке клиентов.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-166">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="5b4b9-167">There is currently no option to remove customers from the list.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-167">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="5b4b9-168">Партнерам следует избегать повторного добавления подписок к этим клиентам из **переносимой** учетной записи в будущем.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-168">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="5b4b9-169">Повторите эти действия для всех подписок всех клиентов, чтобы остановить выставление счетов за **переносимые** учетные записи.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-169">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="5b4b9-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="5b4b9-171">No future invoices will generate after that final billing period.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-171">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="5b4b9-172">Notes</span><span class="sxs-lookup"><span data-stu-id="5b4b9-172">Notes</span></span>

-   <span data-ttu-id="5b4b9-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="5b4b9-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="5b4b9-175">There is currently no way to remove a customer from the Customers list completely.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-175">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="5b4b9-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="5b4b9-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="5b4b9-178">Simplify migration using Export</span><span class="sxs-lookup"><span data-stu-id="5b4b9-178">Simplify migration using Export</span></span>

<span data-ttu-id="5b4b9-179">С помощью **функции экспорта** вы можете получить подписки, которые необходимо использовать в новой консолидированной структуре.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-179">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="5b4b9-180">Щелкните **Клиенты** на информационной панели, чтобы просмотреть список клиентов в существующей структуре.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-180">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="5b4b9-181">Open the desired customer name.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-181">Open the desired customer name.</span></span>

3.  <span data-ttu-id="5b4b9-182">На странице **Подписки** щелкните **Экспорт подписок**, чтобы экспортировать данные подписок в файл Excel.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-182">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="5b4b9-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="5b4b9-184">API registration</span><span class="sxs-lookup"><span data-stu-id="5b4b9-184">API registration</span></span>

<span data-ttu-id="5b4b9-185">Дополнительные сведения о регистрации API см. [на этой странице](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="5b4b9-185">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="partner-center-activity-log"></a><span data-ttu-id="5b4b9-186">Partner Center Activity log</span><span class="sxs-lookup"><span data-stu-id="5b4b9-186">Partner Center Activity log</span></span>


<span data-ttu-id="5b4b9-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span></span> <span data-ttu-id="5b4b9-188">This helps partners track changes on a customer tenant.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-188">This helps partners track changes on a customer tenant.</span></span>

**<span data-ttu-id="5b4b9-189">View the Activity log</span><span class="sxs-lookup"><span data-stu-id="5b4b9-189">View the Activity log</span></span>**

1.  <span data-ttu-id="5b4b9-190">На информационной панели в Центре партнеров щелкните ссылку **Журнал действий**.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-190">From the Partner Center Dashboard, click the **Activity Log** link.</span></span>
2.  <span data-ttu-id="5b4b9-191">На странице **Журнал действий** просмотрите изменения, внесенные в учетные записи клиентов.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-191">On the **Activity Log** page, view the changes made to customer accounts.</span></span> <span data-ttu-id="5b4b9-192">Чтобы отфильтровать журнал действий по дате, выберите **начальную** и **конечную** дату для сужения выбранных записей в журнале.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-192">To filter the Activity log by date, pick **from** and **to** dates to narrow the selected records in the log.</span></span> <span data-ttu-id="5b4b9-193">Для фильтрации по клиенту в **журнале действий** используйте поле поиска.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-193">To filter by customer in the **Activity log**, use the search box.</span></span>

**<span data-ttu-id="5b4b9-194">Export the Activity log</span><span class="sxs-lookup"><span data-stu-id="5b4b9-194">Export the Activity log</span></span>**

-   <span data-ttu-id="5b4b9-195">Нажмите кнопку **Экспорт журнала**, чтобы экспортировать данные журнала действий в CSV-файл.</span><span class="sxs-lookup"><span data-stu-id="5b4b9-195">Click **Export log** to export your Activity log data to a CSV file.</span></span>

    <span data-ttu-id="5b4b9-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span><span class="sxs-lookup"><span data-stu-id="5b4b9-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span></span>

 

 



