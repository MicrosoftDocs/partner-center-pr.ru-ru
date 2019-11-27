---
title: Создание связи с клиентом с помощью модели КПОР | Центр партнеров
ms.topic: article
ms.date: 10/29/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Создание связи с клиентом с помощью модели КПОР
author: LauraBrenner
ms.author: labrenne
keywords: заявки на поощрения, заявления о сопоставлении, фонды совместных операций, осу, OSA, ISV, выручка
ms.localizationpriority: medium
ms.openlocfilehash: a3515c0fff52c9083bbad6cd19f033a88ae2f38a
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384887"
---
# <a name="create-a-customer-association-using-the-cpor-model"></a><span data-ttu-id="76fe6-104">Создание связи с клиентом с помощью модели КПОР</span><span class="sxs-lookup"><span data-stu-id="76fe6-104">Create a customer association using the CPOR model</span></span>

<span data-ttu-id="76fe6-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="76fe6-105">**Applies to**</span></span>

-  <span data-ttu-id="76fe6-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="76fe6-106">Partner Center</span></span>


<span data-ttu-id="76fe6-107">1 октября 2019 г. Корпорация Майкрософт приступила к использованию модели "заявка партнера КПОР" для управления связями с клиентами Microsoft 365 и Dynamics 365 в соответствии с рекомендациями по интерактивным службам (OSA), использованием Интернет-служб (осу) — Microsoft 365 и осу — поощрения бизнес-приложений.</span><span class="sxs-lookup"><span data-stu-id="76fe6-107">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

<span data-ttu-id="76fe6-108">При отправке заявки корпорация Майкрософт проверяет его.</span><span class="sxs-lookup"><span data-stu-id="76fe6-108">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="76fe6-109">На этом этапе мы можем запросить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="76fe6-109">We may ask you for more information at this point.</span></span> <span data-ttu-id="76fe6-110">Мы также будем уведомлять Клиента о запросе на сопоставление.</span><span class="sxs-lookup"><span data-stu-id="76fe6-110">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="76fe6-111">Клиенты могут отказаться от пяти рабочих дней. Если они не отказались от этого, связь с этим конкретным клиентом и рабочей нагрузкой будет официальной.</span><span class="sxs-lookup"><span data-stu-id="76fe6-111">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="76fe6-112">На этом этапе у вас будет доступ к данным об использовании клиента.</span><span class="sxs-lookup"><span data-stu-id="76fe6-112">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="76fe6-113">Для завершения утверждения потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="76fe6-113">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="76fe6-114">**Идентификатор MPN** сущности, которая делает утверждение</span><span class="sxs-lookup"><span data-stu-id="76fe6-114">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="76fe6-115">[Поиск](https://docs.microsoft.com/partner-center/find-customer-domain-name) в **доменном имени** клиента</span><span class="sxs-lookup"><span data-stu-id="76fe6-115">Customer's **domain name** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="76fe6-116">**Идентификатор каталога** клиента или **идентификатор клиента** [найти](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span><span class="sxs-lookup"><span data-stu-id="76fe6-116">Customer's **Directory ID** or **Tenant ID** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="76fe6-117">**Область решения**, например Business Applications или Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="76fe6-117">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="76fe6-118">**Действие** , которое вы выполнили, и тип заявки, которую вы хотите сделать, например "Предварительная продажа", "использование" или "доход"</span><span class="sxs-lookup"><span data-stu-id="76fe6-118">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="76fe6-119">**Имя контактного лица**, название и адрес электронной почты клиента</span><span class="sxs-lookup"><span data-stu-id="76fe6-119">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="76fe6-120">Для Dynamics 365 также необходимо **указать имя, название и** адрес электронной почты вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="76fe6-120">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="76fe6-121">**Имя контактного лица** и адрес электронной почты своей организации</span><span class="sxs-lookup"><span data-stu-id="76fe6-121">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="76fe6-122">Вы создадите **имя** для этого утверждения.</span><span class="sxs-lookup"><span data-stu-id="76fe6-122">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="76fe6-123">**Продукт (ы** ) или рабочие нагрузки, которые вы заказываете</span><span class="sxs-lookup"><span data-stu-id="76fe6-123">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="76fe6-124">**Подтверждение выполнения (ПОЕ)** , например заявление о работе, подписанное клиентом.</span><span class="sxs-lookup"><span data-stu-id="76fe6-124">**Proof of execution (POE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="76fe6-125">Вы также можете скачать шаблон ПОЕ для использования.</span><span class="sxs-lookup"><span data-stu-id="76fe6-125">You can also download a POE template to use.</span></span>

- <span data-ttu-id="76fe6-126">Для партнеров, которые заявляют только сопоставление доходов: **название продавца решения Dynamics**, **имя клиента**и **Название продукта или решения ISV**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-126">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="76fe6-127">Следует также понимать следующие моменты.</span><span class="sxs-lookup"><span data-stu-id="76fe6-127">You should also understand the following points:</span></span>
- <span data-ttu-id="76fe6-128">Если у вас уже есть Microsoft 365 клиентов, вам потребуется повторно связать их с тем, что вы хотите продолжить получать осу поощрения с помощью этого процесса.</span><span class="sxs-lookup"><span data-stu-id="76fe6-128">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>
- <span data-ttu-id="76fe6-129">Если у вас есть существующие связи с Dynamics 365 или клиентами Power BI, эти связи останутся действительными до истечения срока действия подписок.</span><span class="sxs-lookup"><span data-stu-id="76fe6-129">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>
- <span data-ttu-id="76fe6-130">Клиент может иметь несколько партнеров, но каждая рабочая нагрузка (для осу-Microsoft 365) или подписка (для OSA-торгового и осу-Business Applications) может быть связана только с одним партнером.</span><span class="sxs-lookup"><span data-stu-id="76fe6-130">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="76fe6-131">Создание связи с клиентом</span><span class="sxs-lookup"><span data-stu-id="76fe6-131">Create a customer association</span></span>
1.  <span data-ttu-id="76fe6-132">На панели мониторинга центра партнеров в разделе **поощрения**выберите **Обзор**, а затем выберите **связи клиентов**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-132">In the Partner Center dashboard, under **Incentives**, select **Overview**, and then select **Customer associations**.</span></span> 

2.  <span data-ttu-id="76fe6-133">В верхней части страницы ассоциации клиентов выберите **+ Сопоставление клиентов**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-133">At the top of the Customer associations page, select **+ Customer association**.</span></span>

3.  <span data-ttu-id="76fe6-134">Выберите **идентификатор MPN** для партнера, который должен быть связан с клиентом, а затем добавьте доменное имя и идентификатор каталога клиента.</span><span class="sxs-lookup"><span data-stu-id="76fe6-134">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="76fe6-135">Где это?</span><span class="sxs-lookup"><span data-stu-id="76fe6-135">Where are these?</span></span>](https://docs.microsoft.com/partner-center/find-customer-domain-name)

<span data-ttu-id="76fe6-136">Выберите пункт **Продолжить**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-136">Select **Continue**.</span></span>

4.  <span data-ttu-id="76fe6-137">Выберите **область решения** и **действие**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-137">Select the **Solution area** and **Activity**.</span></span> 

>[!Note]

><span data-ttu-id="76fe6-138">Если выбран вариант Business Applications, выберите **использование и (или) предварительные продажи**или **Ассоциация доходов**, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-138">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 

><span data-ttu-id="76fe6-139">При выборе предложения "выручка" будет предложено немного отличить информацию, указанную ниже.</span><span class="sxs-lookup"><span data-stu-id="76fe6-139">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span> 

5.  <span data-ttu-id="76fe6-140">Введите соответствующие сведения на странице **связать клиента** , а затем выберите **создать утверждение**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-140">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

6.  <span data-ttu-id="76fe6-141">Выберите продукты, связанные с этой ассоциацией клиентов, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-141">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

7.  <span data-ttu-id="76fe6-142">Заполните контактные данные клиента и контактные данные вашей организации.</span><span class="sxs-lookup"><span data-stu-id="76fe6-142">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="76fe6-143">Все поля являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="76fe6-143">All fields are required.</span></span> 

>[!Note]

<span data-ttu-id="76fe6-144">Если ваш продукт является Dynamics 365, а у выбранного продукта несколько подписок для этого конкретного клиента, вам также потребуется ввести идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="76fe6-144">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

8.  <span data-ttu-id="76fe6-145">Предоставьте свое подтверждение выполнения (ПОЕ).</span><span class="sxs-lookup"><span data-stu-id="76fe6-145">Supply your proof of execution (POE).</span></span> <span data-ttu-id="76fe6-146">Можно перетащить его в поле, перейти к собственной вспомогательной документации или использовать шаблон, выбрав **загрузить шаблон**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-146">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

9.  <span data-ttu-id="76fe6-147">При желании добавьте и сохраните комментарии, а затем выберите **отправить утверждение**.</span><span class="sxs-lookup"><span data-stu-id="76fe6-147">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="76fe6-148">Мы отправим клиенту сообщение электронной почты, запрашивающее утверждение связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="76fe6-148">We'll send an email to the customer requesting approval of your customer association.</span></span> 

>[!NOTE]

><span data-ttu-id="76fe6-149">После отправки связи с клиентом вы не сможете изменить ее.</span><span class="sxs-lookup"><span data-stu-id="76fe6-149">Once you submit your customer association, you can't edit it.</span></span> 

<span data-ttu-id="76fe6-150">Состояние сопоставления с клиентом отображается в поле **состояние** .</span><span class="sxs-lookup"><span data-stu-id="76fe6-150">The status of your customer association appears in the **Status** field.</span></span> 

<span data-ttu-id="76fe6-151">Выберите **Журнал** , чтобы просмотреть историю сопоставления клиента.</span><span class="sxs-lookup"><span data-stu-id="76fe6-151">Select **History** to view the history of a customer association.</span></span>
