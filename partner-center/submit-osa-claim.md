---
title: Создание связи с клиентом
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Создайте ассоциации клиентов с помощью модели заявок на утверждение партнеров (КПОР). Помогает управлять продажами, использованием, & поощрениями для клиентов Microsoft 365 и Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1fc528b0a00fab42d7ddfcf8dae79d1eae1e2967
ms.sourcegitcommit: b91119c587d37b4ed36dda00c2b0b1946beb3012
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/17/2020
ms.locfileid: "90714358"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="982be-104">Сопоставления клиентов с помощью утвержденной модели партнеров (КПОР) для Microsoft 365 и Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="982be-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="982be-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="982be-105">**Applies to**</span></span>

- <span data-ttu-id="982be-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="982be-106">Partner Center</span></span>

<span data-ttu-id="982be-107">**Соответствующие роли:**</span><span class="sxs-lookup"><span data-stu-id="982be-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="982be-108">Администратор программы поощрения</span><span class="sxs-lookup"><span data-stu-id="982be-108">Incentives admin</span></span>

<span data-ttu-id="982be-109">1 октября 2019 г. Корпорация Майкрософт приступила к использованию модели заявок для партнеров (КПОР) для управления связями с клиентами Microsoft 365 и Dynamics 365 в соответствии с рекомендациями по продаже интерактивных служб (OSA), использованием Интернет-служб (осу) Microsoft 365 и осу-Business.</span><span class="sxs-lookup"><span data-stu-id="982be-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="982be-110">Заявки на сопоставление с клиентами (КПОР) относятся только к продаже веб-служб (OSA), использованию интерактивных служб (осу) — Microsoft 365 и программам поощрения приложений осу-Business.</span><span class="sxs-lookup"><span data-stu-id="982be-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="982be-111">Если вы отправляете заявку на состановку для другой программы, например поставщика облачных решений, управляемого торгового посредника, размещения или поверхности, ознакомьтесь с разработкой заявок в совместных операциях, описанных здесь.</span><span class="sxs-lookup"><span data-stu-id="982be-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="982be-112">При отправке заявки корпорация Майкрософт проверяет его.</span><span class="sxs-lookup"><span data-stu-id="982be-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="982be-113">На этом этапе мы можем запросить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="982be-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="982be-114">Мы также будем уведомлять Клиента о запросе на сопоставление.</span><span class="sxs-lookup"><span data-stu-id="982be-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="982be-115">Клиенты могут отказаться от пяти рабочих дней. Если они не отказались от этого, связь с этим конкретным клиентом и рабочей нагрузкой будет официальной.</span><span class="sxs-lookup"><span data-stu-id="982be-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="982be-116">На этом этапе у вас будет доступ к данным об использовании клиента.</span><span class="sxs-lookup"><span data-stu-id="982be-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="982be-117">Для завершения утверждения потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="982be-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="982be-118">**Идентификатор MPN** сущности, которая делает утверждение</span><span class="sxs-lookup"><span data-stu-id="982be-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="982be-119">[Поиск](find-domain-name.md) в **доменном имени** клиента</span><span class="sxs-lookup"><span data-stu-id="982be-119">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="982be-120">**Идентификатор каталога** клиента или **идентификатор клиента** [найти](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="982be-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="982be-121">**Область решения**, например Business Applications или Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="982be-121">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="982be-122">**Действие** , которое вы выполнили, и тип заявки, которую вы хотите сделать, например "Предварительная продажа", "использование" или "доход"</span><span class="sxs-lookup"><span data-stu-id="982be-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="982be-123">**Имя контактного лица**, название и адрес электронной почты клиента</span><span class="sxs-lookup"><span data-stu-id="982be-123">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="982be-124">Для Dynamics 365 также необходимо **указать имя, название и** адрес электронной почты вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="982be-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="982be-125">**Имя контактного лица** и адрес электронной почты своей организации</span><span class="sxs-lookup"><span data-stu-id="982be-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="982be-126">Вы создадите **имя** для этого утверждения.</span><span class="sxs-lookup"><span data-stu-id="982be-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="982be-127">**Продукт (ы** ) или рабочие нагрузки, которые вы заказываете</span><span class="sxs-lookup"><span data-stu-id="982be-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="982be-128">**Подтверждение выполнения (ПОЕ)**, например заявление о работе, подписанное клиентом.</span><span class="sxs-lookup"><span data-stu-id="982be-128">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="982be-129">Вы также можете скачать шаблон ПОЕ для использования.</span><span class="sxs-lookup"><span data-stu-id="982be-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="982be-130">Для партнеров, которые заявляют только сопоставление доходов: **название продавца решения Dynamics**, **имя клиента**и **Название продукта или решения ISV**.</span><span class="sxs-lookup"><span data-stu-id="982be-130">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="982be-131">Следует также понимать следующие моменты.</span><span class="sxs-lookup"><span data-stu-id="982be-131">You should also understand the following points:</span></span>

- <span data-ttu-id="982be-132">Если у вас уже есть Microsoft 365 клиентов, вам потребуется повторно связать их с тем, что вы хотите продолжить получать осу поощрения с помощью этого процесса.</span><span class="sxs-lookup"><span data-stu-id="982be-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="982be-133">Если у вас есть существующие связи с Dynamics 365 или клиентами Power BI, эти связи останутся действительными до истечения срока действия подписок.</span><span class="sxs-lookup"><span data-stu-id="982be-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="982be-134">Клиент может иметь несколько партнеров, но каждая рабочая нагрузка (для осу-Microsoft 365) или подписка (для OSA-торгового и осу-Business Applications) может быть связана только с одним партнером.</span><span class="sxs-lookup"><span data-stu-id="982be-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="982be-135">Создание связи с клиентом</span><span class="sxs-lookup"><span data-stu-id="982be-135">Create a customer association</span></span>

1. <span data-ttu-id="982be-136">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="982be-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="982be-137">Перейдите на вкладку **поощрения** , выберите **Обзор**, а затем выберите **связи клиентов**.</span><span class="sxs-lookup"><span data-stu-id="982be-137">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="982be-138">В верхней части страницы ассоциации клиентов выберите **+ Сопоставление клиентов**.</span><span class="sxs-lookup"><span data-stu-id="982be-138">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="982be-139">Выберите **идентификатор MPN** расположения партнера, которое нужно связать с клиентом, а затем добавьте имя домена и идентификатор каталога этого клиента.</span><span class="sxs-lookup"><span data-stu-id="982be-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="982be-140">Найти</span><span class="sxs-lookup"><span data-stu-id="982be-140">Find this</span></span>](find-domain-name.md)

5. <span data-ttu-id="982be-141">Выберите **Continue** (Продолжить).</span><span class="sxs-lookup"><span data-stu-id="982be-141">Select **Continue**.</span></span>

6. <span data-ttu-id="982be-142">Выберите **область решения** и **действие**.</span><span class="sxs-lookup"><span data-stu-id="982be-142">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="982be-143">Если выбран вариант Business Applications, выберите **использование и (или) предварительные продажи**или **Ассоциация доходов**, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="982be-143">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="982be-144">Если вы выберете вариант сопоставления дохода, запрос на информацию будет отличаться от указанного ниже.</span><span class="sxs-lookup"><span data-stu-id="982be-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="982be-145">Введите соответствующие сведения на странице **связать клиента** , а затем выберите **создать утверждение**.</span><span class="sxs-lookup"><span data-stu-id="982be-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="982be-146">Выберите продукты, связанные с этой ассоциацией клиентов, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="982be-146">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="982be-147">Укажите контактные данные клиента и вашей организации.</span><span class="sxs-lookup"><span data-stu-id="982be-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="982be-148">Все поля обязательные.</span><span class="sxs-lookup"><span data-stu-id="982be-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="982be-149">Если ваш продукт является Dynamics 365, а у выбранного продукта несколько подписок для этого конкретного клиента, вам также потребуется ввести идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="982be-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="982be-150">Предоставьте свое подтверждение выполнения (ПОЕ).</span><span class="sxs-lookup"><span data-stu-id="982be-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="982be-151">Для этого можно перетащить документ в поле, перейти к сопроводительной документации или применить шаблон, щелкнув **Download template** (Скачать шаблон).</span><span class="sxs-lookup"><span data-stu-id="982be-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="982be-152">При желании добавьте и сохраните комментарии, а затем выберите **Submit claim** (Отправить заявку).</span><span class="sxs-lookup"><span data-stu-id="982be-152">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="982be-153">Мы отправим клиенту электронное письмо с запросом на утверждение связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="982be-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="982be-154">После отправки связи с клиентом вы не сможете изменить ее.</span><span class="sxs-lookup"><span data-stu-id="982be-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="982be-155">Текущее состояние связи с клиентом отображается в поле **Status** (Состояние).</span><span class="sxs-lookup"><span data-stu-id="982be-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="982be-156">Щелкните **History** (Журнал), чтобы просмотреть историю состояний связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="982be-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="982be-157">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="982be-157">Next steps</span></span>

- [<span data-ttu-id="982be-158">Управление связями с клиентами</span><span class="sxs-lookup"><span data-stu-id="982be-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)