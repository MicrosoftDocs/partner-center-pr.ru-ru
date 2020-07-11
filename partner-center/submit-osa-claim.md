---
title: Создание связи с клиентом с помощью модели КПОР
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Создание ассоциаций клиентов с помощью модели КПОР (заявка на утверждение партнера по записи). Помогает управлять продажами, использованием, & поощрениями для клиентов Microsoft 365 и Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
keywords: заявки на поощрения, заявления о сопоставлении, фонды совместных операций, осу, OSA, ISV, выручка
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ded3850ea03626cd25571746cc9aa32231bd14bc
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265069"
---
# <a name="create-a-customer-association-via-the-cpor-model--use-for-microsoft-365-and-dynamics-365-customers"></a><span data-ttu-id="d4800-105">Создание связи с клиентом с помощью модели КПОР — используется для клиентов Microsoft 365 и Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d4800-105">Create a customer association via the CPOR model – use for Microsoft 365 and Dynamics 365 customers</span></span>

<span data-ttu-id="d4800-106">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="d4800-106">**Applies to**</span></span>

- <span data-ttu-id="d4800-107">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="d4800-107">Partner Center</span></span>

<span data-ttu-id="d4800-108">1 октября 2019 г. Корпорация Майкрософт приступила к использованию модели заявок для партнеров (КПОР) для управления связями с клиентами Microsoft 365 и Dynamics 365 в соответствии с рекомендациями по продаже интерактивных служб (OSA), использованием Интернет-служб (осу) Microsoft 365 и осу-Business.</span><span class="sxs-lookup"><span data-stu-id="d4800-108">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

<span data-ttu-id="d4800-109">При отправке заявки корпорация Майкрософт проверяет его.</span><span class="sxs-lookup"><span data-stu-id="d4800-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="d4800-110">На этом этапе мы можем запросить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="d4800-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="d4800-111">Мы также будем уведомлять Клиента о запросе на сопоставление.</span><span class="sxs-lookup"><span data-stu-id="d4800-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="d4800-112">Клиенты могут отказаться от пяти рабочих дней. Если они не отказались от этого, связь с этим конкретным клиентом и рабочей нагрузкой будет официальной.</span><span class="sxs-lookup"><span data-stu-id="d4800-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="d4800-113">На этом этапе у вас будет доступ к данным об использовании клиента.</span><span class="sxs-lookup"><span data-stu-id="d4800-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="d4800-114">Для завершения утверждения потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="d4800-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="d4800-115">**Идентификатор MPN** сущности, которая делает утверждение</span><span class="sxs-lookup"><span data-stu-id="d4800-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="d4800-116">[Поиск](https://docs.microsoft.com/partner-center/find-customer-domain-name) в **доменном имени** клиента</span><span class="sxs-lookup"><span data-stu-id="d4800-116">Customer's **domain name** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="d4800-117">**Идентификатор каталога** клиента или **идентификатор клиента** [найти](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span><span class="sxs-lookup"><span data-stu-id="d4800-117">Customer's **Directory ID** or **Tenant ID** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="d4800-118">**Область решения**, например Business Applications или Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d4800-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="d4800-119">**Действие** , которое вы выполнили, и тип заявки, которую вы хотите сделать, например "Предварительная продажа", "использование" или "доход"</span><span class="sxs-lookup"><span data-stu-id="d4800-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="d4800-120">**Имя контактного лица**, название и адрес электронной почты клиента</span><span class="sxs-lookup"><span data-stu-id="d4800-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="d4800-121">Для Dynamics 365 также необходимо **указать имя, название и** адрес электронной почты вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="d4800-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="d4800-122">**Имя контактного лица** и адрес электронной почты своей организации</span><span class="sxs-lookup"><span data-stu-id="d4800-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="d4800-123">Вы создадите **имя** для этого утверждения.</span><span class="sxs-lookup"><span data-stu-id="d4800-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="d4800-124">**Продукт (ы** ) или рабочие нагрузки, которые вы заказываете</span><span class="sxs-lookup"><span data-stu-id="d4800-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="d4800-125">**Подтверждение выполнения (ПОЕ)**, например заявление о работе, подписанное клиентом.</span><span class="sxs-lookup"><span data-stu-id="d4800-125">**Proof of execution (POE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="d4800-126">Вы также можете скачать шаблон ПОЕ для использования.</span><span class="sxs-lookup"><span data-stu-id="d4800-126">You can also download a POE template to use.</span></span>

- <span data-ttu-id="d4800-127">Для партнеров, которые заявляют только сопоставление доходов: **название продавца решения Dynamics**, **имя клиента**и **Название продукта или решения ISV**.</span><span class="sxs-lookup"><span data-stu-id="d4800-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="d4800-128">Следует также понимать следующие моменты.</span><span class="sxs-lookup"><span data-stu-id="d4800-128">You should also understand the following points:</span></span>

- <span data-ttu-id="d4800-129">Если у вас уже есть Microsoft 365 клиентов, вам потребуется повторно связать их с тем, что вы хотите продолжить получать осу поощрения с помощью этого процесса.</span><span class="sxs-lookup"><span data-stu-id="d4800-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="d4800-130">Если у вас есть существующие связи с Dynamics 365 или клиентами Power BI, эти связи останутся действительными до истечения срока действия подписок.</span><span class="sxs-lookup"><span data-stu-id="d4800-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="d4800-131">Клиент может иметь несколько партнеров, но каждая рабочая нагрузка (для осу-Microsoft 365) или подписка (для OSA-торгового и осу-Business Applications) может быть связана только с одним партнером.</span><span class="sxs-lookup"><span data-stu-id="d4800-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="d4800-132">Создание связи с клиентом</span><span class="sxs-lookup"><span data-stu-id="d4800-132">Create a customer association</span></span>

1. <span data-ttu-id="d4800-133">На панели мониторинга центра партнеров в разделе **поощрения**выберите **Обзор**, а затем выберите **связи клиентов**.</span><span class="sxs-lookup"><span data-stu-id="d4800-133">In the Partner Center dashboard, under **Incentives**, select **Overview**, and then select **Customer associations**.</span></span> 

2. <span data-ttu-id="d4800-134">В верхней части страницы ассоциации клиентов выберите **+ Сопоставление клиентов**.</span><span class="sxs-lookup"><span data-stu-id="d4800-134">At the top of the Customer associations page, select **+ Customer association**.</span></span>

3. <span data-ttu-id="d4800-135">Выберите **идентификатор MPN** для партнера, который должен быть связан с клиентом, а затем добавьте доменное имя и идентификатор каталога клиента.</span><span class="sxs-lookup"><span data-stu-id="d4800-135">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="d4800-136">Где это?</span><span class="sxs-lookup"><span data-stu-id="d4800-136">Where are these?</span></span>](https://docs.microsoft.com/partner-center/find-customer-domain-name)

4. <span data-ttu-id="d4800-137">Выберите **Continue** (Продолжить).</span><span class="sxs-lookup"><span data-stu-id="d4800-137">Select **Continue**.</span></span>

5. <span data-ttu-id="d4800-138">Выберите **область решения** и **действие**.</span><span class="sxs-lookup"><span data-stu-id="d4800-138">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="d4800-139">Если выбран вариант Business Applications, выберите **использование и (или) предварительные продажи**или **Ассоциация доходов**, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="d4800-139">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 

   ><span data-ttu-id="d4800-140">При выборе предложения "выручка" будет предложено немного отличить информацию, указанную ниже.</span><span class="sxs-lookup"><span data-stu-id="d4800-140">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

6. <span data-ttu-id="d4800-141">Введите соответствующие сведения на странице **связать клиента** , а затем выберите **создать утверждение**.</span><span class="sxs-lookup"><span data-stu-id="d4800-141">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

7. <span data-ttu-id="d4800-142">Выберите продукты, связанные с этой ассоциацией клиентов, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="d4800-142">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

8. <span data-ttu-id="d4800-143">Заполните контактные данные клиента и контактные данные вашей организации.</span><span class="sxs-lookup"><span data-stu-id="d4800-143">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="d4800-144">Все поля обязательные.</span><span class="sxs-lookup"><span data-stu-id="d4800-144">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="d4800-145">Если ваш продукт является Dynamics 365, а у выбранного продукта несколько подписок для этого конкретного клиента, вам также потребуется ввести идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="d4800-145">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

9. <span data-ttu-id="d4800-146">Предоставьте свое подтверждение выполнения (ПОЕ).</span><span class="sxs-lookup"><span data-stu-id="d4800-146">Supply your proof of execution (POE).</span></span> <span data-ttu-id="d4800-147">Можно перетащить его в поле, перейти к собственной вспомогательной документации или использовать шаблон, выбрав **загрузить шаблон**.</span><span class="sxs-lookup"><span data-stu-id="d4800-147">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

10. <span data-ttu-id="d4800-148">При желании добавьте и сохраните комментарии, а затем выберите **отправить утверждение**.</span><span class="sxs-lookup"><span data-stu-id="d4800-148">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="d4800-149">Мы отправим клиенту сообщение электронной почты, запрашивающее утверждение связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="d4800-149">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="d4800-150">После отправки связи с клиентом вы не сможете изменить ее.</span><span class="sxs-lookup"><span data-stu-id="d4800-150">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="d4800-151">Состояние сопоставления с клиентом отображается в поле **состояние** .</span><span class="sxs-lookup"><span data-stu-id="d4800-151">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="d4800-152">Выберите **Журнал** , чтобы просмотреть историю сопоставления клиента.</span><span class="sxs-lookup"><span data-stu-id="d4800-152">Select **History** to view the history of a customer association.</span></span>
