---
title: Управление лицензированием в предложениях Marketplace
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как настроить и администрировать лицензирование для предложений коммерческих партнеров ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284880"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="a3bfb-103">Управление лицензированием в предложениях Marketplace</span><span class="sxs-lookup"><span data-stu-id="a3bfb-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="a3bfb-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="a3bfb-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a3bfb-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a3bfb-105">Global admin</span></span>
- <span data-ttu-id="a3bfb-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="a3bfb-106">Account admin</span></span>

<span data-ttu-id="a3bfb-107">В этой статье описано, как настроить предложение в центре партнеров, сделать его доступным в Microsoft AppSource, а затем управлять лицензиями для этого предложения.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="a3bfb-108">Возможности в этой статье в настоящее время доступны в общедоступной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="a3bfb-109">Перед началом</span><span class="sxs-lookup"><span data-stu-id="a3bfb-109">Before you begin</span></span>

<span data-ttu-id="a3bfb-110">Прежде чем начать этот процесс, вы должны ознакомиться со сведениями ниже.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="a3bfb-111">Ознакомьтесь с документацией Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="a3bfb-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="a3bfb-112">Приведенные ниже статьи содержат сведения, которые необходимо изучить перед продолжением.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="a3bfb-113">Создание предложения Dynamics 365 for Customer Engagement & PowerApps</span><span class="sxs-lookup"><span data-stu-id="a3bfb-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="a3bfb-114">Создание коммерческой учетной записи Marketplace в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="a3bfb-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="a3bfb-115">Создание идентификатора предложения</span><span class="sxs-lookup"><span data-stu-id="a3bfb-115">Create your Offer ID</span></span>

<span data-ttu-id="a3bfb-116">В приведенных ниже процедурах вам будет предложено ввести идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="a3bfb-117">Потратьте некоторое время на получение подходящего идентификатора предложения, учитывая следующие моменты:</span><span class="sxs-lookup"><span data-stu-id="a3bfb-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="a3bfb-118">Идентификатор отображается для клиентов в веб-адресе предложения на Marketplace, а также, если применимо, шаблонов Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="a3bfb-119">Длина идентификатора предложения в сочетании с ИДЕНТИФИКАТОРом издателя не должна превышать 40 символов.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="a3bfb-120">Вы можете использовать только строчные буквы и цифры.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="a3bfb-121">Идентификатор предложения может включать дефисы и символы подчеркивания, но не пробелы.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="a3bfb-122">Например, если идентификатор издателя — тестпублишерид и вы вводите Test-предложение-1, веб-адрес предложения будет иметь значение https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="a3bfb-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="a3bfb-123">Этот идентификатор нельзя изменить после нажатия **создать**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="a3bfb-124">Создание псевдонима предложения</span><span class="sxs-lookup"><span data-stu-id="a3bfb-124">Create your Offer alias</span></span>

<span data-ttu-id="a3bfb-125">Псевдоним предложения — это имя, используемое для предложения в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="a3bfb-126">Вам также потребуется соответствующий псевдоним предложения, который следует правилам, приведенным ниже.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="a3bfb-127">Это имя не используется в Marketplace и отличается от имени предложения и других значений, отображаемых для клиентов.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="a3bfb-128">Это имя нельзя изменить после нажатия создать.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="a3bfb-129">Создайте предложение</span><span class="sxs-lookup"><span data-stu-id="a3bfb-129">Create your offer</span></span>

<span data-ttu-id="a3bfb-130">Первым шагом в процессе лицензирования является создание предложения коммерческого рынка.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="a3bfb-131">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="a3bfb-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="a3bfb-132">В меню навигации слева выберите **коммерческие рынки/обзор**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="a3bfb-133">В верхней части страницы обзора выберите **новое предложение**, а затем выберите **Dynamics 365 для участия клиента & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="a3bfb-134">Введите **идентификатор предложения** и **псевдоним предложения** , созданные ранее.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="a3bfb-135">Выберите **Создать**, чтобы создать предложение и продолжить.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="a3bfb-136">Выберите параметры лицензирования.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="a3bfb-137">Чтобы включить управление лицензиями для вашего предложения, выберите **включить управление лицензиями приложений в Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="a3bfb-138">Это одноразовый параметр, и его нельзя изменить после публикации предложения.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="a3bfb-139">Вы также можете разрешить клиентам запускать базовые функции вашего приложения без лицензии и запускать функции Premium после приобретения лицензии.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="a3bfb-140">Для этого выберите **Разрешить клиентам устанавливать приложение, даже если лицензии не назначены**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="a3bfb-141">Если вы не хотите, чтобы предложение включало Управление лицензиями, выберите **получить сейчас (бесплатно)**, **Бесплатная пробная версия** или **свяжитесь со мной**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="a3bfb-142">Создание плана</span><span class="sxs-lookup"><span data-stu-id="a3bfb-142">Create your plan</span></span>

<span data-ttu-id="a3bfb-143">На этих шагах вы определите план или планы, которые вы хотите включить для вашего предложения.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="a3bfb-144">В меню навигации слева выберите пункт **Общие сведения о плане**, а затем выберите **создать новый план**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="a3bfb-145">Введите **идентификатор плана** и **имя плана**, а затем щелкните **создать**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="a3bfb-146">На странице « **список планов** » введите **Описание плана**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="a3bfb-147">Чтобы сохранить описание и завершить работу позже, выберите **Сохранить черновик**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="a3bfb-148">По завершении выберите **проверить и опубликовать**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="a3bfb-149">Теперь сведения о плане будут отображаться в appsource.microsoft.com в разделе "список предложений" (раздел "планы").</span><span class="sxs-lookup"><span data-stu-id="a3bfb-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="a3bfb-150">После создания всех планов для этого предложения необходимо скопировать идентификатор службы каждого плана.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="a3bfb-151">Выберите **Общие сведения о плане** в верхней части страницы "план".</span><span class="sxs-lookup"><span data-stu-id="a3bfb-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="a3bfb-152">Скопируйте идентификатор службы для каждого плана в надежное расположение.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="a3bfb-153">Добавление идентификаторов служб в решение</span><span class="sxs-lookup"><span data-stu-id="a3bfb-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="a3bfb-154">Следующим шагом является обновление решения путем добавления идентификаторов службы для каждого скопированного плана.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="a3bfb-155">Рекомендации по этому см. в статье [Создание пакета AppSource для решения](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="a3bfb-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="a3bfb-156">Отправка пакета и публикация предложения</span><span class="sxs-lookup"><span data-stu-id="a3bfb-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="a3bfb-157">В области навигации слева выберите **коммерческое Marketplace**, а затем выберите пункт **Техническая конфигурация**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="a3bfb-158">В разделе **Базовая модель лицензии** выберите **пользователь**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="a3bfb-159">В разделе **пакет CRM** введите URL-адрес расположения пакета.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="a3bfb-160">Используйте другие вкладки в левой области навигации, чтобы ввести другие необходимые сведения.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="a3bfb-161">Когда все будет готово, выберите **проверить и опубликовать**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="a3bfb-162">После публикации предложения мы будем просматривать и проверять сведения.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="a3bfb-163">При возникновении проблем с этим процессом мы отправим вам уведомление.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="a3bfb-164">Когда все проблемы будут устранены, вы получите уведомление о том, что ваше предложение доступно в AppSource.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="a3bfb-165">На этом этапе вы можете сделать это прямо сейчас.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="a3bfb-166">Сделайте свое предложение активным в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="a3bfb-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="a3bfb-167">Приведенная ниже процедура поможет вам выполнить процедуру создания предложения в AppSource.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="a3bfb-168">Дополнительные сведения об этом процессе см. в разделе Общие сведения о [параметрах перечисления](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="a3bfb-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="a3bfb-169">После публикации предложения оно займет 4-6 часов.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="a3bfb-170">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="a3bfb-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="a3bfb-171">В меню навигации слева выберите **коммерческие рынки/обзор**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="a3bfb-172">На странице **Обзор** найдите предложение, которое вы ищете.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="a3bfb-173">Готовые к публикации предложения будут иметь состояние **предварительной** версии.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="a3bfb-174">Выберите предложение.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-174">Select the offer.</span></span>
4. <span data-ttu-id="a3bfb-175">На странице **Обзор предложения** выберите **Go Live**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="a3bfb-176">Предложение будет находиться в течение 4-6 часов.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="a3bfb-177">Чтобы просмотреть список предложений на AppSource, щелкните ссылку **AppSource** в нижней части страницы " **Обзор предложения** ".</span><span class="sxs-lookup"><span data-stu-id="a3bfb-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="a3bfb-178">**Для предложений с поддержкой лицензий**. Если для вашего предложения требуется проверка лицензии, пользователи смогут ввести только его, щелкнув " **связаться со мной**", чтобы вы могли взаимодействовать с ними.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="a3bfb-179">**Для предложений с поддержкой лицензий с возможностью бесплатной установки**: Если для вашего предложения не требуется проверка лицензии, пользователи с правами администратора увидят кнопку **получить сейчас** , а также связаться со **мной**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="a3bfb-180">Пользователи, желающие опробовать бесплатную установку, должны щелкнуть " **получить сейчас**", что позволит им установить предложение в центре администрирования Power Platform.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="a3bfb-181">Пользователи по-прежнему могут использовать **связь со мной** , если у них есть вопросы или они хотят выполнить обновление до платного плана.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="a3bfb-182">Регистрация беспроблемных подключений ISV в Деалрег</span><span class="sxs-lookup"><span data-stu-id="a3bfb-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="a3bfb-183">Следующим шагом является регистрация вашей сделки.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-183">The next step is to register your deal.</span></span> <span data-ttu-id="a3bfb-184">Дополнительные сведения см. в разделе [регистрация сделок](https://docs.microsoft.com/partner-center/register-deals).</span><span class="sxs-lookup"><span data-stu-id="a3bfb-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="a3bfb-185">Пригласить клиента</span><span class="sxs-lookup"><span data-stu-id="a3bfb-185">Invite the customer</span></span>

<span data-ttu-id="a3bfb-186">Используйте следующую процедуру, чтобы пригласить клиента принять участие в этой сделки.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="a3bfb-187">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="a3bfb-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="a3bfb-188">В меню навигации слева выберите **коммерческие рынки/обзор**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="a3bfb-189">Отфильтруйте **Отправленные** сделки, выберите вкладку **выполняется** , а затем выберите нужную сделку.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="a3bfb-190">На странице Обзор для этой сделки выберите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="a3bfb-191">В окне **Управление лицензиями** выберите клиента в раскрывающемся списке **сведения о клиенте** .</span><span class="sxs-lookup"><span data-stu-id="a3bfb-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="a3bfb-192">Если связь с клиентом еще не существует, выберите **+ пригласить нового клиента в согласие**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="a3bfb-193">Скопируйте отображаемую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="a3bfb-194">Отправьте эту ссылку администратору выставления счетов клиента или глобальному администратору по электронной почте и используйте эту ссылку для доступа к admin.microsoft.com и принятия и авторизации установленной связи.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a3bfb-195">Связь не будет установлена до тех пор, пока клиент не выполнит этот шаг.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="a3bfb-196">Активация, управление и удаление лицензий</span><span class="sxs-lookup"><span data-stu-id="a3bfb-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="a3bfb-197">После установки клиента можно приступить к добавлению планов из предложения и назначению лицензий каждому плану.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="a3bfb-198">В окне Manage Licenses (Управление лицензиями) выберите **+ Добавить план**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="a3bfb-199">Заполните поля **планы для этого решения** и **числа лицензий** , а затем выберите **Обновить лицензии**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="a3bfb-200">Лицензии будут доступны по адресу admin.microsoft.com, чтобы клиенты могли управлять и назначать сотрудников.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="a3bfb-201">Чтобы изменить число лицензий для существующего плана, введите новое значение в поле **число лицензий** и выберите **Обновить лицензии**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="a3bfb-202">Чтобы отключить или удалить лицензии для сделки, выберите значок корзины в поле **действия** , а затем выберите **Обновить лицензии**.</span><span class="sxs-lookup"><span data-stu-id="a3bfb-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>