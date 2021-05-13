---
title: Создание связи с клиентом
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Создайте ассоциации клиентов с помощью модели заявок на утверждение партнеров (КПОР). Помогает управлять продажами, использованием и поощрениями для клиентов Microsoft 365 & Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856106"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="e6b8a-104">Сопоставления клиентов с помощью утвержденной модели партнеров (КПОР) для Microsoft 365 и Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e6b8a-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="e6b8a-105">**Соответствующие роли**: администратор поощрения</span><span class="sxs-lookup"><span data-stu-id="e6b8a-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="e6b8a-106">1 октября 2019 г. Корпорация Майкрософт приступила к использованию модели "Заявка на утверждение партнера" (КПОР) для управления связями с клиентами Microsoft 365 и Dynamics 365 по отношению к продаже веб-служб (OSA), использованию Интернет-служб (осу) — Microsoft 365 и OSU-Business поощрения приложений.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="e6b8a-107">Заявки на сопоставление с клиентами (КПОР) относятся только к продаже веб-служб (OSA), использованию интерактивных служб (осу) — Microsoft 365 и OSU-Business программ стимулов для приложений.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="e6b8a-108">Если вы отправляете заявку на состановку для другой программы, например поставщика облачных решений, управляемого торгового посредника, размещения или поверхности, ознакомьтесь с разработкой заявок в совместных операциях, описанных здесь.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="e6b8a-109">При отправке заявки корпорация Майкрософт проверяет его.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="e6b8a-110">На этом этапе мы можем запросить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="e6b8a-111">Мы также будем уведомлять Клиента о запросе на сопоставление.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="e6b8a-112">Клиенты могут отказаться от пяти рабочих дней. Если они не отказались от этого, связь с этим конкретным клиентом и рабочей нагрузкой будет официальной.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="e6b8a-113">На этом этапе у вас будет доступ к данным об использовании клиента.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="e6b8a-114">Для завершения утверждения потребуются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="e6b8a-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="e6b8a-115">**Идентификатор MPN** сущности, которая делает утверждение</span><span class="sxs-lookup"><span data-stu-id="e6b8a-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="e6b8a-116">[Поиск](find-ids-and-domain-names.md) в **доменном имени** клиента</span><span class="sxs-lookup"><span data-stu-id="e6b8a-116">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="e6b8a-117">**Идентификатор каталога** клиента или **идентификатор клиента** [найти](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="e6b8a-117">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="e6b8a-118">**Область решения**, например Business Applications или Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e6b8a-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="e6b8a-119">**Действие** , которое вы выполнили, и тип заявки, которую вы хотите сделать, например "Предварительная продажа", "использование" или "доход"</span><span class="sxs-lookup"><span data-stu-id="e6b8a-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="e6b8a-120">**Имя контактного лица**, название и адрес электронной почты клиента</span><span class="sxs-lookup"><span data-stu-id="e6b8a-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="e6b8a-121">Для Dynamics 365 также необходимо **указать имя, название и** адрес электронной почты вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="e6b8a-122">**Имя контактного лица** и адрес электронной почты своей организации</span><span class="sxs-lookup"><span data-stu-id="e6b8a-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="e6b8a-123">Вы создадите **имя** для этого утверждения.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="e6b8a-124">**Продукт (ы** ) или рабочие нагрузки, которые вы заказываете</span><span class="sxs-lookup"><span data-stu-id="e6b8a-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="e6b8a-125">**Подтверждение выполнения (ПОЕ)**, например заявление о работе, подписанное клиентом.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="e6b8a-126">Вы также можете скачать шаблон ПОЕ для использования.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="e6b8a-127">Для партнеров, которые заявляют только сопоставление доходов: **название продавца решения Dynamics**, **имя клиента** и **Название продукта или решения ISV**.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="e6b8a-128">Следует также понимать следующие моменты.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-128">You should also understand the following points:</span></span>

- <span data-ttu-id="e6b8a-129">Если у вас уже есть Microsoft 365 клиентов, вам потребуется повторно связать их с тем, что вы хотите продолжить получать осу поощрения с помощью этого процесса.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="e6b8a-130">Если у вас есть существующие связи с Dynamics 365 или клиентами Power BI, эти связи останутся действительными до истечения срока действия подписок.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="e6b8a-131">У клиента может быть несколько партнеров, но каждая рабочая нагрузка (для OSU-Microsoft 365) или подписка (для OSA-Sell и OSU-Business приложений) может быть связана только с одним партнером.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="e6b8a-132">Создание связи с клиентом</span><span class="sxs-lookup"><span data-stu-id="e6b8a-132">Create a customer association</span></span>

1. <span data-ttu-id="e6b8a-133">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="e6b8a-133">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="e6b8a-134">Перейдите на вкладку **поощрения** , выберите **Обзор**, а затем выберите **связи клиентов**.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="e6b8a-135">В верхней части страницы ассоциации клиентов выберите **+ Сопоставление клиентов**.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="e6b8a-136">Выберите **идентификатор MPN** расположения партнера, которое нужно связать с клиентом, а затем добавьте имя домена и идентификатор каталога этого клиента.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="e6b8a-137">Найти</span><span class="sxs-lookup"><span data-stu-id="e6b8a-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="e6b8a-138">Выберите **Continue** (Продолжить).</span><span class="sxs-lookup"><span data-stu-id="e6b8a-138">Select **Continue**.</span></span>

6. <span data-ttu-id="e6b8a-139">Выберите **область решения** и **действие**.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="e6b8a-140">Если выбран вариант Business Applications, выберите **использование и (или) предварительные продажи** или **Ассоциация доходов**, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="e6b8a-141">Если вы выберете вариант сопоставления дохода, запрос на информацию будет отличаться от указанного ниже.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="e6b8a-142">Введите соответствующие сведения на странице **связать клиента** , а затем выберите **создать утверждение**.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="e6b8a-143">Выберите продукты, связанные с этой ассоциацией клиентов, а затем нажмите кнопку **продолжить**.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="e6b8a-144">Укажите контактные данные клиента и вашей организации.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="e6b8a-145">Все поля обязательные.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="e6b8a-146">Если ваш продукт является Dynamics 365, а у выбранного продукта несколько подписок для этого конкретного клиента, вам также потребуется ввести идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="e6b8a-147">Предоставьте свое подтверждение выполнения (ПОЕ).</span><span class="sxs-lookup"><span data-stu-id="e6b8a-147">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="e6b8a-148">Для этого можно перетащить документ в поле, перейти к сопроводительной документации или применить шаблон, щелкнув **Download template** (Скачать шаблон).</span><span class="sxs-lookup"><span data-stu-id="e6b8a-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="e6b8a-149">При желании добавьте и сохраните комментарии, а затем выберите **Submit claim** (Отправить заявку).</span><span class="sxs-lookup"><span data-stu-id="e6b8a-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="e6b8a-150">Мы отправим клиенту электронное письмо с запросом на утверждение связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="e6b8a-151">После отправки связи с клиентом вы не сможете изменить ее.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="e6b8a-152">Текущее состояние связи с клиентом отображается в поле **Status** (Состояние).</span><span class="sxs-lookup"><span data-stu-id="e6b8a-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="e6b8a-153">Щелкните **History** (Журнал), чтобы просмотреть историю состояний связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="e6b8a-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e6b8a-154">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e6b8a-154">Next steps</span></span>

- [<span data-ttu-id="e6b8a-155">Управление связями с клиентами</span><span class="sxs-lookup"><span data-stu-id="e6b8a-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)