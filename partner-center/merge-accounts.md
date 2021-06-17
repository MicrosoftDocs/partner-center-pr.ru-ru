---
title: Объединение учетной записи партнера с другой учетной записью партнера
description: Узнайте, как объединить учетную запись партнера с другой учетной записью партнера в центре партнеров — для компаний, которые являются активными партнерами Майкрософт в центре партнеров.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: bcef4c771d748b0e2fbeae8cf1daaf41d7f53b43
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276643"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="f26b9-103">Объединение учетной записи партнера с другой учетной записью партнера</span><span class="sxs-lookup"><span data-stu-id="f26b9-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="f26b9-104">**Соответствующие роли**: Администратор учетной записи</span><span class="sxs-lookup"><span data-stu-id="f26b9-104">**Appropriate roles**: Account admin</span></span>

<span data-ttu-id="f26b9-105">Две или более компаний, которые являются активными партнерами Майкрософт и имеют учетные записи в центре партнеров, могут объединить свои учетные записи.</span><span class="sxs-lookup"><span data-stu-id="f26b9-105">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="f26b9-106">Что происходит, когда два партнера объединяют учетные записи центра партнеров</span><span class="sxs-lookup"><span data-stu-id="f26b9-106">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="f26b9-107">Партнерская организация, инициирующая слияние, будет глобальной учетной записью партнера (PGA).</span><span class="sxs-lookup"><span data-stu-id="f26b9-107">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="f26b9-108">В компании, которая является приглашенной организацией, будет размещена Компания-инициатор.</span><span class="sxs-lookup"><span data-stu-id="f26b9-108">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="f26b9-109">Все расположения учетной записи слияния становятся расположениями под корпусом PGA.</span><span class="sxs-lookup"><span data-stu-id="f26b9-109">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="f26b9-110">После завершения слияния учетной записи вы увидите сведения об учетной записи, такие как местоположения и пользователи в профиле PGA.</span><span class="sxs-lookup"><span data-stu-id="f26b9-110">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="f26b9-111">Этот процесс нельзя отменить.</span><span class="sxs-lookup"><span data-stu-id="f26b9-111">You can't reverse this process.</span></span>

- <span data-ttu-id="f26b9-112">Все идентификаторы MPN для расположений сохраняются во время консолидации.</span><span class="sxs-lookup"><span data-stu-id="f26b9-112">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="f26b9-113">Роли пользователя переносятся.</span><span class="sxs-lookup"><span data-stu-id="f26b9-113">User's roles are brought over.</span></span> <span data-ttu-id="f26b9-114">Например, если пользователь был администратором поощрения для определенного местоположения, он по-прежнему будет иметь эту роль после слияния и сможет увидеть поощрения, которые они видели до слияния.</span><span class="sxs-lookup"><span data-stu-id="f26b9-114">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="f26b9-115">Клиенты Azure AD и учетные записи CSP не объединяются и не оказывают никакого влияния.</span><span class="sxs-lookup"><span data-stu-id="f26b9-115">Azure AD tenants and CSP accounts are not merged and have no effect.</span></span>

- <span data-ttu-id="f26b9-116">Опубликованные предложения и данные конвейера совместной продажи, связанные с обеими компаниями, сохраняются.</span><span class="sxs-lookup"><span data-stu-id="f26b9-116">Published offers and Co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="f26b9-117">Представление Объединенных учетных записей</span><span class="sxs-lookup"><span data-stu-id="f26b9-117">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Слияние учетных записей.":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="f26b9-119">Что следует делать, если вы приглашены на слияние учетной записи центра партнеров с другой учетной записью центра партнеров</span><span class="sxs-lookup"><span data-stu-id="f26b9-119">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="f26b9-120">Если вы решили принять приглашение для слияния учетных записей: · ИДЕНТИФИКАТОРы и расположения MPN будут объединены в PGA учетной записи партнера, которая вас пригласила.</span><span class="sxs-lookup"><span data-stu-id="f26b9-120">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="f26b9-121">Ваши пользователи будут переведены в Объединенную учетную запись со своими ролями без изменений.</span><span class="sxs-lookup"><span data-stu-id="f26b9-121">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="f26b9-122">Существующие преимущества и компетенции будут сохранены для обеих компаний после слияния до продления.</span><span class="sxs-lookup"><span data-stu-id="f26b9-122">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="f26b9-123">При продлении учетные записи будут рассматриваться как одна компания и будут применяться стандартные правила продления.</span><span class="sxs-lookup"><span data-stu-id="f26b9-123">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="f26b9-124">Общие сведения о влиянии на программы и преимущества при выборе партнеров для слияния учетных записей</span><span class="sxs-lookup"><span data-stu-id="f26b9-124">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="f26b9-125">Все существующие компетенции (Gold/серебро), покупки (например, Microsoft Action Pack) и связанные с ними преимущества сохраняются во время консолидации.</span><span class="sxs-lookup"><span data-stu-id="f26b9-125">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="f26b9-126">Если обе компании имеют одну и ту же компетенцию, но одна из них — золото, а другая серебряная, то будет выделена компетенция с самым высоким уровнем квалификации, а у партнеров будет один набор преимуществ для этой компетенции и один набор из Gold выгод для этого сертификата до следующего продления.</span><span class="sxs-lookup"><span data-stu-id="f26b9-126">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="f26b9-127">Самая высокая Дата юбилея Microsoft Action Pack будет храниться после слияния.</span><span class="sxs-lookup"><span data-stu-id="f26b9-127">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="f26b9-128">Например, если дата юбилея для компании 1 — Июнь 2020 для Action Pack продления, а Дата юбилея Action Pack продления для компании 2 — Октябрь 2020, корпорация Майкрософт будет использовать в качестве новой даты выпуска за Октябрь 2020 дату, выпущенную в октябре.</span><span class="sxs-lookup"><span data-stu-id="f26b9-128">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="f26b9-129">Во время слияния учетных записей и до следующего продления каждая учетная запись будет хранить свои Action Pack и (или) компетенции.</span><span class="sxs-lookup"><span data-stu-id="f26b9-129">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="f26b9-130">При продлении применяются стандартные Action Pack и правила обновления компетенций.</span><span class="sxs-lookup"><span data-stu-id="f26b9-130">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="f26b9-131">После продления вы можете воспользоваться преимуществами, предоставляемыми при достижении компетенции и Action Pack для глобальной учетной записи партнера партнерской компании.</span><span class="sxs-lookup"><span data-stu-id="f26b9-131">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="f26b9-132">Microsoft Action Pack: компания-партнер может приобрести одну Action Pack для глобальной учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="f26b9-132">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="f26b9-133">Компетенция: Партнерская компания получит один пакет основных преимуществ, который связан с максимальным достижением, а также преимущества, относящиеся к компетенции, которые партнер может использовать в глобальной учетной записи партнера.</span><span class="sxs-lookup"><span data-stu-id="f26b9-133">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="f26b9-134">Все преимущества распространяются в соответствии с [руководством по использованию Microsoft Partner Networkных преимуществ](https://aka.ms/partner-benefits-use-guide).</span><span class="sxs-lookup"><span data-stu-id="f26b9-134">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="f26b9-135">Например: активированный токен O365 E3 работает в течение 12 месяцев после активации.</span><span class="sxs-lookup"><span data-stu-id="f26b9-135">For example: an activated O365 E3 token is functional for 12 months after activation.</span></span> <span data-ttu-id="f26b9-136">После активации маркера для лицензий в клиенте эти лицензии нельзя переместить в другой клиент.</span><span class="sxs-lookup"><span data-stu-id="f26b9-136">Once a token has been activated for licenses on a tenant, those licenses may not be moved to another tenant.</span></span>

- <span data-ttu-id="f26b9-137">Связи ИДЕНТИФИКАТОРов MCP для обеих компаний будут сохранены и сопоставлены с ИДЕНТИФИКАТОРом MPN (PGA).</span><span class="sxs-lookup"><span data-stu-id="f26b9-137">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="f26b9-138">Предложения "переход на рынок" и "технические преимущества" предлагаются в качестве преимущества ключевого обеспечения компетенции.</span><span class="sxs-lookup"><span data-stu-id="f26b9-138">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="f26b9-139">После слияния рекомендуется проверить банковские и налоговые данные, чтобы обеспечить точность.</span><span class="sxs-lookup"><span data-stu-id="f26b9-139">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="f26b9-140">Если ваша компания входит в программу MSP эксперта по Azure, преимущества сохраняются до продления.</span><span class="sxs-lookup"><span data-stu-id="f26b9-140">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="f26b9-141">Если ваша компания послужила расширенными специализациями, они сохраняются в обеих учетных записях.</span><span class="sxs-lookup"><span data-stu-id="f26b9-141">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="f26b9-142">Все ваучеры по программе Software Assurance сохраняются в обеих учетных записях.</span><span class="sxs-lookup"><span data-stu-id="f26b9-142">Any software assurance vouchers are retained across both accounts.</span></span> 

- <span data-ttu-id="f26b9-143">Связь DPOR или PAL не действует.</span><span class="sxs-lookup"><span data-stu-id="f26b9-143">There is no effect to DPOR or PAL association.</span></span> <span data-ttu-id="f26b9-144">Все связанные вклады доходов начнут передаваться в глобальную учетную запись партнера</span><span class="sxs-lookup"><span data-stu-id="f26b9-144">Any associated revenue contributions will begin to flow into the new Partner Global Account</span></span>

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="f26b9-145">Пригласите компании, чтобы объединить учетную запись центра партнеров с учетной записью центра партнеров</span><span class="sxs-lookup"><span data-stu-id="f26b9-145">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="f26b9-146">Чтобы выполнить слияние учетной записи, необходимо быть **администратором учетной записи** для вашей компании.</span><span class="sxs-lookup"><span data-stu-id="f26b9-146">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="f26b9-147">Выберите **Параметры** на панели мониторинга центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="f26b9-147">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="f26b9-148">Выберите **Объединение учетных записей**.</span><span class="sxs-lookup"><span data-stu-id="f26b9-148">Select **Account merge**.</span></span>

3. <span data-ttu-id="f26b9-149">Добавьте идентификатор MPN, расположенный в **профиле партнера** учетной записи, который вы хотите пригласить для объединения с вами.</span><span class="sxs-lookup"><span data-stu-id="f26b9-149">Add the MPN ID located in the **Partner profile** of the account that you want to invite to merge with you.</span></span> <span data-ttu-id="f26b9-150">Необходимо использовать глобальный идентификатор MPN партнера.</span><span class="sxs-lookup"><span data-stu-id="f26b9-150">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="f26b9-151">Нельзя использовать MPN location ID.</span><span class="sxs-lookup"><span data-stu-id="f26b9-151">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="f26b9-152">При выборе **слияния** в компанию-партнер отправляется приглашение.</span><span class="sxs-lookup"><span data-stu-id="f26b9-152">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="f26b9-153">Принимая запрос, вы можете начать слияние учетных записей в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="f26b9-153">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="f26b9-154">Если компания отклоняет Ваш запрос на слияние учетных записей, они могут объяснить, почему они отклонили запрос.</span><span class="sxs-lookup"><span data-stu-id="f26b9-154">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="f26b9-155">Список всех слияний учетных записей доступен в разделе **Журнал слияния**.</span><span class="sxs-lookup"><span data-stu-id="f26b9-155">A list of all your account merges is available to you under **Merge history**.</span></span>
 
### <a name="example-of-two-companies-merging-accounts"></a><span data-ttu-id="f26b9-156">Пример двух компаний, объединяющих учетные записи</span><span class="sxs-lookup"><span data-stu-id="f26b9-156">Example of two companies merging accounts</span></span>

1. <span data-ttu-id="f26b9-157">Компания Contoso, Ltd. имеет</span><span class="sxs-lookup"><span data-stu-id="f26b9-157">Contoso, Ltd. has</span></span> 

    <span data-ttu-id="f26b9-158">а.</span><span class="sxs-lookup"><span data-stu-id="f26b9-158">a.</span></span> <span data-ttu-id="f26b9-159">[глобальный идентификатор MPN 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) и одно подчиненное [Расположение MPN с идентификаторами 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span><span class="sxs-lookup"><span data-stu-id="f26b9-159">a [global MPN ID of 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) and one subordinate [location MPN IDs of 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span></span>
  
    <span data-ttu-id="f26b9-160">b.</span><span class="sxs-lookup"><span data-stu-id="f26b9-160">b.</span></span> <span data-ttu-id="f26b9-161">Клиент Azure AD = @contoso.com</span><span class="sxs-lookup"><span data-stu-id="f26b9-161">an Azure AD tenant = @contoso.com</span></span>
 
    <span data-ttu-id="f26b9-162">c.</span><span class="sxs-lookup"><span data-stu-id="f26b9-162">c.</span></span> <span data-ttu-id="f26b9-163">компетенция Gold с истекшим сроком действия 1 октября 2020 г.</span><span class="sxs-lookup"><span data-stu-id="f26b9-163">a gold competency that expires October 1, 2020</span></span>
2. <span data-ttu-id="f26b9-164">Компания Fabrikam, Inc.</span><span class="sxs-lookup"><span data-stu-id="f26b9-164">Fabrikam, Inc. has</span></span>
 
    <span data-ttu-id="f26b9-165">а.</span><span class="sxs-lookup"><span data-stu-id="f26b9-165">a.</span></span>  <span data-ttu-id="f26b9-166">Глобальный идентификатор MPN, 3333333 и два подчиненных расположения MPN с идентификаторами 4444444 и 5555555.</span><span class="sxs-lookup"><span data-stu-id="f26b9-166">a global MPN ID of 3333333 and two subordinate location MPN IDs of 4444444 and 5555555</span></span>

    <span data-ttu-id="f26b9-167">b.</span><span class="sxs-lookup"><span data-stu-id="f26b9-167">b.</span></span>  <span data-ttu-id="f26b9-168">Клиент Azure AD = @fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="f26b9-168">an Azure AD tenant = @fabrikam.com</span></span>

    <span data-ttu-id="f26b9-169">c.</span><span class="sxs-lookup"><span data-stu-id="f26b9-169">c.</span></span>  <span data-ttu-id="f26b9-170">две категории компетенции Gold с истекшим сроком 1 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="f26b9-170">two gold competencies that expire December 1, 2020</span></span>
3.  <span data-ttu-id="f26b9-171">Компания Contoso покупает Fabrikam и перейдет [сюда](https://partner.microsoft.com/dashboard/account/merger) , чтобы начать запрос на слияние.</span><span class="sxs-lookup"><span data-stu-id="f26b9-171">Contoso buys Fabrikam and goes [here](https://partner.microsoft.com/dashboard/account/merger) to initiate a merge request.</span></span>
4.  <span data-ttu-id="f26b9-172">Fabrikam входит в центр партнеров и переходит на ту же страницу, что и Contoso #3, чтобы утвердить запрос contoso.</span><span class="sxs-lookup"><span data-stu-id="f26b9-172">Fabrikam signs into Partner Center and goes to the same page as Contoso did in step #3, to approve Contoso’s request.</span></span>
5.  <span data-ttu-id="f26b9-173">Contoso проверяет сведения о слиянии на этой же странице и предоставляет подтверждение для продолжения слияния учетных записей.</span><span class="sxs-lookup"><span data-stu-id="f26b9-173">Contoso reviews the details of the merge on that same page and provides confirmation to proceed with the account merger.</span></span>
6.  <span data-ttu-id="f26b9-174">После слияния учетная запись компании будет отображаться следующим образом:</span><span class="sxs-lookup"><span data-stu-id="f26b9-174">After the merger, the company account will display as:</span></span>

    <span data-ttu-id="f26b9-175">а.</span><span class="sxs-lookup"><span data-stu-id="f26b9-175">a.</span></span>  <span data-ttu-id="f26b9-176">Компания Contoso с глобальным ИДЕНТИФИКАТОРом MPN 1111111 и 4 подчиненного расположения MPN идентификаторы 2222222, 3333333, 4444444 и 5555555.</span><span class="sxs-lookup"><span data-stu-id="f26b9-176">A company named Contoso with a global MPN ID of 1111111 and 4 subordinate location MPN IDs of 2222222, 3333333, 4444444, and 5555555</span></span>
    
    <span data-ttu-id="f26b9-177">b.</span><span class="sxs-lookup"><span data-stu-id="f26b9-177">b.</span></span>  <span data-ttu-id="f26b9-178">У него будут два клиента Azure AD ( @contoso.com + @fabrikam.com ), которые имеют доступ к одной и той же учетной записи центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="f26b9-178">It will have two Azure AD tenants (@contoso.com + @fabrikam.com) that have access to the same Partner Center account</span></span>
    
    <span data-ttu-id="f26b9-179">c.</span><span class="sxs-lookup"><span data-stu-id="f26b9-179">c.</span></span>  <span data-ttu-id="f26b9-180">У него будет два пакета компетенции, срок действия которого истекает 1 октября 2020, а другой — 1 декабря 2020.</span><span class="sxs-lookup"><span data-stu-id="f26b9-180">It will have two competency benefits packages, one that expires October 1, 2020 and another that expires December 1, 2020.</span></span> <span data-ttu-id="f26b9-181">Они смогут продлить один пакет преимуществ для компетенции 1 декабря 2020.</span><span class="sxs-lookup"><span data-stu-id="f26b9-181">They'll be able to renew as a single competency benefits package on December 1, 2020.</span></span> <span data-ttu-id="f26b9-182">При продлении Contoso сохранит все три компетенции, несмотря на то, что они могут поддерживать только один пакет преимуществ.</span><span class="sxs-lookup"><span data-stu-id="f26b9-182">When they renew, Contoso will retain all three competencies even though they can only maintain a single benefits package.</span></span>
    
7.  <span data-ttu-id="f26b9-183">Администраторы Contoso продолжат управление ролями центра партнеров для @contoso.com пользователей.</span><span class="sxs-lookup"><span data-stu-id="f26b9-183">Contoso’s admins will continue to manage Partner Center roles for @contoso.com’s users.</span></span> <span data-ttu-id="f26b9-184">Администраторы Fabrikam продолжат управление ролями центра партнеров для @fabrikam.com пользователей.</span><span class="sxs-lookup"><span data-stu-id="f26b9-184">Fabrikam’s admins will continue to manage Partner Center roles for @fabrikam.com’s users.</span></span> <span data-ttu-id="f26b9-185">Администраторы Contoso могут администрировать пользователей Fabrikam только в том случае, если они приглашены в качестве гостя в клиент Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="f26b9-185">Contoso’s admins can only administer Fabrikam’s users if they are invited as a guest into Fabrikam’s tenant.</span></span>
8.  <span data-ttu-id="f26b9-186">Компания Contoso решила проигнорировать @fabrikam.com клиент и повторно выдать новые @contoso.com учетные данные сотрудников Fabrikam с новыми ролями и разрешениями.</span><span class="sxs-lookup"><span data-stu-id="f26b9-186">Contoso could decide to ignore the @fabrikam.com tenant, and reissue the Fabrikam employees new @contoso.com credentials with new roles and permissions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f26b9-187">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f26b9-187">Next steps</span></span>

- [<span data-ttu-id="f26b9-188">Назначение пользователям ролей и разрешений</span><span class="sxs-lookup"><span data-stu-id="f26b9-188">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="f26b9-189">Проверка информации профиля партнера</span><span class="sxs-lookup"><span data-stu-id="f26b9-189">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="f26b9-190">Добавьте общие службы партнеров Azure, чтобы партнеры могли покупать подписки Azure для их собственного использования.</span><span class="sxs-lookup"><span data-stu-id="f26b9-190">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
