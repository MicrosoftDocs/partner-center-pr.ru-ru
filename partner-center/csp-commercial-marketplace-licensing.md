---
title: Управление лицензированием в предложениях Marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как настроить и администрировать лицензирование для предложений коммерческих партнеров ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328021"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="1a114-103">Управление лицензированием в предложениях Marketplace</span><span class="sxs-lookup"><span data-stu-id="1a114-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="1a114-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="1a114-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1a114-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1a114-105">Global admin</span></span>
- <span data-ttu-id="1a114-106">Администратор учетных записей</span><span class="sxs-lookup"><span data-stu-id="1a114-106">Account admin</span></span>

<span data-ttu-id="1a114-107">В этой статье описано, как настроить предложение в центре партнеров, сделать его доступным в Microsoft AppSource, а затем управлять лицензиями для этого предложения.</span><span class="sxs-lookup"><span data-stu-id="1a114-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="1a114-108">Возможности в этой статье в настоящее время доступны в общедоступной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="1a114-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="1a114-109">Подготовка к работе</span><span class="sxs-lookup"><span data-stu-id="1a114-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="1a114-110">Основы коммерческого рынка</span><span class="sxs-lookup"><span data-stu-id="1a114-110">Commercial marketplace basics</span></span>

<span data-ttu-id="1a114-111">Прежде чем начать этот процесс, вы должны ознакомиться с основами коммерческого рынка.</span><span class="sxs-lookup"><span data-stu-id="1a114-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="1a114-112">Статьи, приведенные в таблице ниже, помогут вам приступить к работе.</span><span class="sxs-lookup"><span data-stu-id="1a114-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="1a114-113">Раздел</span><span class="sxs-lookup"><span data-stu-id="1a114-113">Topic</span></span>  | <span data-ttu-id="1a114-114">Статья</span><span class="sxs-lookup"><span data-stu-id="1a114-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="1a114-115">Планы коммерческого рынка</span><span class="sxs-lookup"><span data-stu-id="1a114-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="1a114-116">Планы и цены на коммерческие предложения Marketplace</span><span class="sxs-lookup"><span data-stu-id="1a114-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="1a114-117">Предложения коммерческих рынков</span><span class="sxs-lookup"><span data-stu-id="1a114-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="1a114-118">Типы списков</span><span class="sxs-lookup"><span data-stu-id="1a114-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="1a114-119">Коммерческие учетные записи Marketplace</span><span class="sxs-lookup"><span data-stu-id="1a114-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="1a114-120">Создание коммерческой учетной записи Marketplace в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="1a114-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="1a114-121">Определение идентификатора предложения</span><span class="sxs-lookup"><span data-stu-id="1a114-121">Determine your Offer ID</span></span>

<span data-ttu-id="1a114-122">В приведенных ниже процедурах вам будет предложено ввести идентификатор предложения.</span><span class="sxs-lookup"><span data-stu-id="1a114-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="1a114-123">Потратьте некоторое время на получение подходящего идентификатора предложения, учитывая следующие моменты:</span><span class="sxs-lookup"><span data-stu-id="1a114-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="1a114-124">Идентификатор отображается для клиентов в веб-адресе предложения на Marketplace, а также, если применимо, шаблонов Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="1a114-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="1a114-125">Длина идентификатора предложения в сочетании с ИДЕНТИФИКАТОРом издателя не должна превышать 40 символов.</span><span class="sxs-lookup"><span data-stu-id="1a114-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="1a114-126">Вы можете использовать только строчные буквы и цифры.</span><span class="sxs-lookup"><span data-stu-id="1a114-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="1a114-127">Идентификатор предложения может включать дефисы и символы подчеркивания, но не пробелы.</span><span class="sxs-lookup"><span data-stu-id="1a114-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="1a114-128">Например, если `testpublisherid` вы вводите идентификатор издателя `test-offer-1` , веб-адрес предложения будет иметь значение `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="1a114-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="1a114-129">Этот идентификатор нельзя изменить после нажатия **создать**.</span><span class="sxs-lookup"><span data-stu-id="1a114-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="1a114-130">Определение псевдонима предложения</span><span class="sxs-lookup"><span data-stu-id="1a114-130">Determine your Offer alias</span></span>

<span data-ttu-id="1a114-131">Псевдоним предложения — это имя, используемое для предложения в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="1a114-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="1a114-132">Вам также потребуется соответствующий псевдоним предложения, который следует правилам, приведенным ниже.</span><span class="sxs-lookup"><span data-stu-id="1a114-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="1a114-133">Это имя не используется в Marketplace и отличается от имени предложения и других значений, отображаемых для клиентов.</span><span class="sxs-lookup"><span data-stu-id="1a114-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="1a114-134">Это имя нельзя изменить после нажатия создать.</span><span class="sxs-lookup"><span data-stu-id="1a114-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="1a114-135">Создайте предложение</span><span class="sxs-lookup"><span data-stu-id="1a114-135">Create your offer</span></span>

<span data-ttu-id="1a114-136">Первым шагом в процессе лицензирования является создание предложения коммерческого рынка.</span><span class="sxs-lookup"><span data-stu-id="1a114-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="1a114-137">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1a114-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1a114-138">В меню навигации слева выберите **коммерческие рынки/обзор**.</span><span class="sxs-lookup"><span data-stu-id="1a114-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="1a114-139">В верхней части страницы обзора выберите **новое предложение**, а затем выберите **Dynamics 365 для участия клиента & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="1a114-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="1a114-140">Введите **идентификатор предложения** и **псевдоним предложения** , созданные ранее.</span><span class="sxs-lookup"><span data-stu-id="1a114-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="1a114-141">Выберите **Создать**, чтобы создать предложение и продолжить.</span><span class="sxs-lookup"><span data-stu-id="1a114-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="1a114-142">Выберите параметры лицензирования.</span><span class="sxs-lookup"><span data-stu-id="1a114-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="1a114-143">Чтобы включить управление лицензиями для вашего предложения, выберите **включить управление лицензиями приложений в Майкрософт**.</span><span class="sxs-lookup"><span data-stu-id="1a114-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="1a114-144">Это одноразовый параметр, и его нельзя изменить после публикации предложения.</span><span class="sxs-lookup"><span data-stu-id="1a114-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="1a114-145">Вы также можете разрешить клиентам запускать базовые функции вашего приложения без лицензии и запускать функции Premium после приобретения лицензии.</span><span class="sxs-lookup"><span data-stu-id="1a114-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="1a114-146">Для этого выберите **Разрешить клиентам устанавливать приложение, даже если лицензии не назначены**.</span><span class="sxs-lookup"><span data-stu-id="1a114-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="1a114-147">Если вы не хотите, чтобы предложение включало Управление лицензиями, выберите **получить сейчас (бесплатно)**, **Бесплатная пробная версия** или **свяжитесь со мной**.</span><span class="sxs-lookup"><span data-stu-id="1a114-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="1a114-148">Создание плана</span><span class="sxs-lookup"><span data-stu-id="1a114-148">Create your plan</span></span>

<span data-ttu-id="1a114-149">На этих шагах вы определите план или планы, которые вы хотите включить для вашего предложения.</span><span class="sxs-lookup"><span data-stu-id="1a114-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="1a114-150">В меню навигации слева выберите пункт **Общие сведения о плане**, а затем выберите **создать новый план**.</span><span class="sxs-lookup"><span data-stu-id="1a114-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="1a114-151">Введите **идентификатор плана** и **имя плана**, а затем щелкните **создать**.</span><span class="sxs-lookup"><span data-stu-id="1a114-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="1a114-152">На странице « **список планов** » введите **Описание плана**.</span><span class="sxs-lookup"><span data-stu-id="1a114-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="1a114-153">Чтобы сохранить описание и завершить работу позже, выберите **Сохранить черновик**.</span><span class="sxs-lookup"><span data-stu-id="1a114-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="1a114-154">По завершении выберите **проверить и опубликовать**.</span><span class="sxs-lookup"><span data-stu-id="1a114-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="1a114-155">Теперь сведения о плане будут отображаться в appsource.microsoft.com в разделе "список предложений" (раздел "планы").</span><span class="sxs-lookup"><span data-stu-id="1a114-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="1a114-156">После создания всех планов для этого предложения необходимо скопировать идентификатор службы каждого плана.</span><span class="sxs-lookup"><span data-stu-id="1a114-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="1a114-157">Выберите **Общие сведения о плане** в верхней части страницы "план".</span><span class="sxs-lookup"><span data-stu-id="1a114-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="1a114-158">Скопируйте идентификатор службы для каждого плана в надежное расположение.</span><span class="sxs-lookup"><span data-stu-id="1a114-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="1a114-159">Добавление идентификаторов служб в решение</span><span class="sxs-lookup"><span data-stu-id="1a114-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="1a114-160">Следующим шагом является обновление решения путем добавления идентификаторов службы для каждого скопированного плана.</span><span class="sxs-lookup"><span data-stu-id="1a114-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="1a114-161">Рекомендации по этому см. в статье [Создание пакета AppSource для решения](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span><span class="sxs-lookup"><span data-stu-id="1a114-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="1a114-162">Отправка пакета и публикация предложения</span><span class="sxs-lookup"><span data-stu-id="1a114-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="1a114-163">В области навигации слева выберите **коммерческое Marketplace**, а затем выберите пункт **Техническая конфигурация**.</span><span class="sxs-lookup"><span data-stu-id="1a114-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="1a114-164">В разделе **Базовая модель лицензии** выберите **пользователь**.</span><span class="sxs-lookup"><span data-stu-id="1a114-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="1a114-165">В разделе **пакет CRM** введите URL-адрес расположения пакета.</span><span class="sxs-lookup"><span data-stu-id="1a114-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="1a114-166">Используйте другие вкладки в левой области навигации, чтобы ввести другие необходимые сведения.</span><span class="sxs-lookup"><span data-stu-id="1a114-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="1a114-167">Когда все будет готово, выберите **проверить и опубликовать**.</span><span class="sxs-lookup"><span data-stu-id="1a114-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="1a114-168">После публикации предложения мы будем просматривать и проверять сведения.</span><span class="sxs-lookup"><span data-stu-id="1a114-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="1a114-169">При возникновении проблем с этим процессом мы отправим вам уведомление.</span><span class="sxs-lookup"><span data-stu-id="1a114-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="1a114-170">Когда все проблемы будут устранены, вы получите уведомление о том, что ваше предложение доступно в AppSource.</span><span class="sxs-lookup"><span data-stu-id="1a114-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="1a114-171">На этом этапе вы можете сделать это прямо сейчас.</span><span class="sxs-lookup"><span data-stu-id="1a114-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="1a114-172">Сделайте свое предложение активным в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="1a114-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="1a114-173">Приведенная ниже процедура поможет вам выполнить процедуру создания предложения в AppSource.</span><span class="sxs-lookup"><span data-stu-id="1a114-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="1a114-174">Дополнительные сведения об этом процессе см. в разделе Общие сведения о [параметрах перечисления](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="1a114-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="1a114-175">После публикации предложения оно займет 4-6 часов.</span><span class="sxs-lookup"><span data-stu-id="1a114-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="1a114-176">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1a114-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1a114-177">В меню навигации слева выберите **коммерческие рынки/обзор**.</span><span class="sxs-lookup"><span data-stu-id="1a114-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="1a114-178">На странице **Обзор** найдите предложение, которое вы ищете.</span><span class="sxs-lookup"><span data-stu-id="1a114-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="1a114-179">Готовые к публикации предложения будут иметь состояние **предварительной** версии.</span><span class="sxs-lookup"><span data-stu-id="1a114-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="1a114-180">Выберите предложение.</span><span class="sxs-lookup"><span data-stu-id="1a114-180">Select the offer.</span></span>
4. <span data-ttu-id="1a114-181">На странице **Обзор предложения** выберите **Go Live**.</span><span class="sxs-lookup"><span data-stu-id="1a114-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="1a114-182">Предложение будет находиться в течение 4-6 часов.</span><span class="sxs-lookup"><span data-stu-id="1a114-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="1a114-183">Чтобы просмотреть список предложений на AppSource, щелкните ссылку **AppSource** в нижней части страницы " **Обзор предложения** ".</span><span class="sxs-lookup"><span data-stu-id="1a114-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="1a114-184">**Для предложений с поддержкой лицензий**. Если для вашего предложения требуется проверка лицензии, пользователи смогут ввести только его, щелкнув " **связаться со мной**", чтобы вы могли взаимодействовать с ними.</span><span class="sxs-lookup"><span data-stu-id="1a114-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="1a114-185">**Для предложений с поддержкой лицензий с возможностью бесплатной установки**: Если для вашего предложения не требуется проверка лицензии, пользователи с правами администратора увидят кнопку **получить сейчас** , а также связаться со **мной**.</span><span class="sxs-lookup"><span data-stu-id="1a114-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="1a114-186">Пользователи, желающие опробовать бесплатную установку, должны щелкнуть " **получить сейчас**", что позволит им установить предложение в центре администрирования Power Platform.</span><span class="sxs-lookup"><span data-stu-id="1a114-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="1a114-187">Пользователи по-прежнему могут использовать **связь со мной** , если у них есть вопросы или они хотят выполнить обновление до платного плана.</span><span class="sxs-lookup"><span data-stu-id="1a114-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="1a114-188">Регистрация беспроблемного подключения ISV в регистрации сделки</span><span class="sxs-lookup"><span data-stu-id="1a114-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="1a114-189">Прежде чем назначать лицензии клиенту, каждая продажа должна быть зарегистрирована в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="1a114-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="1a114-190">Дополнительные сведения см. в разделе [регистрация сделок](register-deals.md).</span><span class="sxs-lookup"><span data-stu-id="1a114-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="1a114-191">Пригласить клиента</span><span class="sxs-lookup"><span data-stu-id="1a114-191">Invite the customer</span></span>

<span data-ttu-id="1a114-192">Используйте следующую процедуру, чтобы пригласить клиента принять участие в этой сделки.</span><span class="sxs-lookup"><span data-stu-id="1a114-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="1a114-193">Войдите в [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1a114-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1a114-194">В меню навигации слева выберите **коммерческие рынки/обзор**.</span><span class="sxs-lookup"><span data-stu-id="1a114-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="1a114-195">В меню навигации слева выберите **ссылки**, а затем щелкните **Регистрация сделки**.</span><span class="sxs-lookup"><span data-stu-id="1a114-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="1a114-196">Отфильтруйте **Отправленные** сделки, выберите вкладку **выполняется** , а затем выберите нужную сделку.</span><span class="sxs-lookup"><span data-stu-id="1a114-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="1a114-197">На странице Обзор для этой сделки выберите **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="1a114-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="1a114-198">В окне **Управление лицензиями** выберите клиента в раскрывающемся списке **сведения о клиенте** .</span><span class="sxs-lookup"><span data-stu-id="1a114-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="1a114-199">Если связь с клиентом еще не существует, выберите **+ пригласить нового клиента в согласие**.</span><span class="sxs-lookup"><span data-stu-id="1a114-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="1a114-200">Скопируйте отображаемую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1a114-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="1a114-201">Отправьте эту ссылку администратору выставления счетов клиента или глобальному администратору по электронной почте и используйте эту ссылку для доступа к admin.microsoft.com и принятия и авторизации установленной связи.</span><span class="sxs-lookup"><span data-stu-id="1a114-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="1a114-202">Связь не будет установлена до тех пор, пока клиент не выполнит этот шаг.</span><span class="sxs-lookup"><span data-stu-id="1a114-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="1a114-203">Активация, управление и удаление лицензий</span><span class="sxs-lookup"><span data-stu-id="1a114-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="1a114-204">После того, как ваш клиент попытается получить связь с вами, можно приступить к добавлению планов из вашего предложения и назначению лицензий каждому плану.</span><span class="sxs-lookup"><span data-stu-id="1a114-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="1a114-205">В окне Manage Licenses (Управление лицензиями) выберите **+ Добавить план**.</span><span class="sxs-lookup"><span data-stu-id="1a114-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="1a114-206">Заполните поля **планы для этого решения** и **числа лицензий** , а затем выберите **Обновить лицензии**.</span><span class="sxs-lookup"><span data-stu-id="1a114-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="1a114-207">Лицензии будут доступны по адресу admin.microsoft.com, чтобы клиенты могли управлять и назначать сотрудников.</span><span class="sxs-lookup"><span data-stu-id="1a114-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="1a114-208">Чтобы изменить число лицензий для существующего плана, введите новое значение в поле **число лицензий** и выберите **Обновить лицензии**.</span><span class="sxs-lookup"><span data-stu-id="1a114-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="1a114-209">Чтобы отключить или удалить лицензии для сделки, выберите значок корзины в поле **действия** , а затем выберите **Обновить лицензии**.</span><span class="sxs-lookup"><span data-stu-id="1a114-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1a114-210">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1a114-210">Next steps</span></span>

[<span data-ttu-id="1a114-211">Ресурсы по лицензированию</span><span class="sxs-lookup"><span data-stu-id="1a114-211">Licensing resources</span></span>](support-resources-licensing.md)
