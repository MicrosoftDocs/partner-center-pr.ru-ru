---
title: Устранение проблем с соединителями рефералов при совместных продажах
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Часто задаваемые вопросы об устранении неполадок соединителей совместных продаж.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 312ff9155ab4c2d84fb38bb6ccd093505e628832
ms.sourcegitcommit: df7643f3b7978e164e419e447a4dc3c163cb3bd2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2020
ms.locfileid: "91844658"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="1c798-103">Устранение проблем с соединителями рефералов при совместных продажах</span><span class="sxs-lookup"><span data-stu-id="1c798-103">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="1c798-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="1c798-104">**Applies to:**</span></span>

- <span data-ttu-id="1c798-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="1c798-105">Partner Center</span></span>
- <span data-ttu-id="1c798-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="1c798-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="1c798-107">SalesForce CRM</span><span class="sxs-lookup"><span data-stu-id="1c798-107">Salesforce CRM</span></span>

<span data-ttu-id="1c798-108">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="1c798-108">**Appropriate roles**</span></span>

- <span data-ttu-id="1c798-109">Администратор авторов</span><span class="sxs-lookup"><span data-stu-id="1c798-109">Referrals admin</span></span>
- <span data-ttu-id="1c798-110">Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="1c798-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="1c798-111">Вопросы и ответы о предварительных требованиях</span><span class="sxs-lookup"><span data-stu-id="1c798-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="1c798-112">Можно ли использовать для вашей среды решение соединителей для совместных продаж?</span><span class="sxs-lookup"><span data-stu-id="1c798-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="1c798-113">Если вы используете тестовую или промежуточную среду, вы можете выбрать пробную версию решения.</span><span class="sxs-lookup"><span data-stu-id="1c798-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="1c798-114">Платная версия соединителей доступна в AppSource за 15 долларов США в месяц.</span><span class="sxs-lookup"><span data-stu-id="1c798-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="1c798-115">С платным подключением вы будете получать вызовы API 10000 в день.</span><span class="sxs-lookup"><span data-stu-id="1c798-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="1c798-116">Соединители являются оболочками на основе API-интерфейсов ссылок центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="1c798-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="1c798-117">Каждый раз, когда решения соединителя выполняются для событий **создания** или **обновления** на стороне центра партнеров или CRM, выполняется вызов API.</span><span class="sxs-lookup"><span data-stu-id="1c798-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="1c798-118">Какую роль необходимо создать в среде CRM?</span><span class="sxs-lookup"><span data-stu-id="1c798-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="1c798-119">Пользователи, являющиеся системными администраторами или настройщиками системы, могут применять изменения для всех.</span><span class="sxs-lookup"><span data-stu-id="1c798-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="1c798-120">Однако все пользователи приложений могут персонализировать систему и даже использовать некоторые настройки совместно с другими пользователями.</span><span class="sxs-lookup"><span data-stu-id="1c798-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="1c798-121">Требуются ли партнерским продавцов специальные роли для работы в центре партнеров?</span><span class="sxs-lookup"><span data-stu-id="1c798-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="1c798-122">Партнеру продавцов должна быть назначена роль "Администратор ссылок".</span><span class="sxs-lookup"><span data-stu-id="1c798-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="1c798-123">Дополнительные сведения см. в следующих [обзоре разрешений) (Create-User-Accounts-and-Set-Permissions).</span><span class="sxs-lookup"><span data-stu-id="1c798-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="1c798-124">Какие поля необходимо настроить в среде CRM первыми?</span><span class="sxs-lookup"><span data-stu-id="1c798-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="1c798-125">• Убедитесь, что Ваша валюта подходит для вашего расположения и правильно находится в среде CRM.</span><span class="sxs-lookup"><span data-stu-id="1c798-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="1c798-126">• Группа продаж должна быть указана в среде CRM в качестве пользователей CRM.</span><span class="sxs-lookup"><span data-stu-id="1c798-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="1c798-127">Какие предварительные требования необходимы для создания среды Power автоматизиру?</span><span class="sxs-lookup"><span data-stu-id="1c798-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="1c798-128">Чтобы использовать среду Power автоматизиру, вам потребуется:</span><span class="sxs-lookup"><span data-stu-id="1c798-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="1c798-129">Требуется лицензия Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="1c798-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="1c798-130">Требуется не менее 1 ГБ хранилища.</span><span class="sxs-lookup"><span data-stu-id="1c798-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="1c798-131">Нужна ли вам подписка Dynamics 365 для использования решения соединителей Salesforce?</span><span class="sxs-lookup"><span data-stu-id="1c798-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="1c798-132">Решение соединителя Salesforce имеет тип "Dynamics Flow", поддерживающий синхронизацию с другими системами CRM.</span><span class="sxs-lookup"><span data-stu-id="1c798-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="1c798-133">Для решения не требуется наличие экземпляра Dynamics 365 или подписки.</span><span class="sxs-lookup"><span data-stu-id="1c798-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="1c798-134">При установке решения Salesforce может появиться раскрывающийся список с существующей средой для работы с компакт-дисков в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="1c798-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="1c798-135">Необходимо выбрать эту среду.</span><span class="sxs-lookup"><span data-stu-id="1c798-135">You need to select that environment.</span></span> <span data-ttu-id="1c798-136">Кроме того, если возникает ошибка "не удалось найти организацию Dynamics 365, подключенную к пользователю, выполнившего вход", необходимо создать новую среду для соединителя.</span><span class="sxs-lookup"><span data-stu-id="1c798-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="1c798-137">Вопросы и ответы о конфигурации</span><span class="sxs-lookup"><span data-stu-id="1c798-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="1c798-138">Что делать, если при активации последовательностей в платформе Power автоматизировать произошла следующая ошибка?</span><span class="sxs-lookup"><span data-stu-id="1c798-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="1c798-139">Ошибка: запрос к Azure Resource Manager завершился с ошибкой: "{" Error ": {" Code ":" Воркфловтригжернотфаунд "," Message ":" не удалось найти рабочий процесс "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" триггер "Manual". "}}".</span><span class="sxs-lookup"><span data-stu-id="1c798-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="1c798-140">Выполните следующие действия по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="1c798-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="1c798-141">Удалите подключение к компакт-дискам, а затем Воссоздайте подключения к компакт-дискам.</span><span class="sxs-lookup"><span data-stu-id="1c798-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="1c798-142">Включение и отключение дочернего потока</span><span class="sxs-lookup"><span data-stu-id="1c798-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="1c798-143">Удалите решение, а затем переустановите решение.</span><span class="sxs-lookup"><span data-stu-id="1c798-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="1c798-144">Что делать, если во время добавления соединителя центра партнеров в платформу Power автоматизиру, вы сталкиваетесь с ошибкой входа?</span><span class="sxs-lookup"><span data-stu-id="1c798-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Сообщение об ошибке, запрашивающее вход":::

<span data-ttu-id="1c798-146">Выполните следующие действия по устранению неполадок:</span><span class="sxs-lookup"><span data-stu-id="1c798-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="1c798-147">Используйте учетные данные центра партнеров, чтобы войти в среду потока один раз (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="1c798-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="1c798-148">Что делать, если вы получаете следующую ошибку при активации центра партнеров в CRM Flow на платформе Power автоматизиру?</span><span class="sxs-lookup"><span data-stu-id="1c798-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Сообщение об ошибке, запрашивающее вход":::

<span data-ttu-id="1c798-150">Выполните следующие действия по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="1c798-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="1c798-151">Прежде чем активировать центр партнеров до CRM Flow, активируйте следующие два дочерних потока.</span><span class="sxs-lookup"><span data-stu-id="1c798-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="1c798-152">Центр партнеров в CRM — вспомогательный (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="1c798-153">Центр партнеров обновления справочных данных по Microsoft CRM (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="1c798-154">Что делать, если вы не можете добавить подключения к потоку при попытке изменить последовательность?</span><span class="sxs-lookup"><span data-stu-id="1c798-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="1c798-155">Вы добавляете подключения к потоку во время выполнения последовательности и добавляете их в каждый поток по отдельности.</span><span class="sxs-lookup"><span data-stu-id="1c798-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="1c798-156">Если диалоговое окно для добавления подключений не открывается автоматически при редактировании потока, то можно изменить каждый из шагов и подзадач каждого потока по отдельности.</span><span class="sxs-lookup"><span data-stu-id="1c798-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="1c798-157">Выберите каждый поток и измените их по отдельности.</span><span class="sxs-lookup"><span data-stu-id="1c798-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="1c798-158">Развернуть все шаги в последовательности</span><span class="sxs-lookup"><span data-stu-id="1c798-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Сообщение об ошибке, запрашивающее вход":::

- <span data-ttu-id="1c798-160">Выберите шаги, на которых отображается значок предупреждения, предлагающий связать подключения и добавить подключения.</span><span class="sxs-lookup"><span data-stu-id="1c798-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Сообщение об ошибке, запрашивающее вход":::


5. <span data-ttu-id="1c798-162">Что делать, если в решении "соединители для совместной продажи" не включены потоки?</span><span class="sxs-lookup"><span data-stu-id="1c798-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="1c798-163">A.</span><span class="sxs-lookup"><span data-stu-id="1c798-163">A.</span></span> <span data-ttu-id="1c798-164">В Power Автоматизация необходимо изменить последовательности в следующем порядке и обновить их для использования правильных подключений:</span><span class="sxs-lookup"><span data-stu-id="1c798-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="1c798-165">Регистрация веб-перехватчика центра партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="1c798-166">Создание ссылки на совместную продажу — Salesforce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1c798-167">Центр партнеров обновления справочных обновлений в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1c798-168">Центр партнеров в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1c798-169">SalesForce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1c798-170">Возможность Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1c798-171">Решения Майкрософт для Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="1c798-172">Б.</span><span class="sxs-lookup"><span data-stu-id="1c798-172">B.</span></span> <span data-ttu-id="1c798-173">Для каждого потока выберите параметр **выполнять только пользователей** .</span><span class="sxs-lookup"><span data-stu-id="1c798-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="1c798-174">Выберите **использовать соединение** вместо **предоставленного пользователем только для запуска**.</span><span class="sxs-lookup"><span data-stu-id="1c798-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Сообщение об ошибке, запрашивающее вход":::


<span data-ttu-id="1c798-176">В.</span><span class="sxs-lookup"><span data-stu-id="1c798-176">C.</span></span> <span data-ttu-id="1c798-177">Активируйте указанные ниже потоки.</span><span class="sxs-lookup"><span data-stu-id="1c798-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="1c798-178">Центр партнеров обновления справочных обновлений в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="1c798-179">SalesForce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1c798-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="1c798-180">Г.</span><span class="sxs-lookup"><span data-stu-id="1c798-180">D.</span></span> <span data-ttu-id="1c798-181">Активируйте все оставшиеся потоки.</span><span class="sxs-lookup"><span data-stu-id="1c798-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="1c798-182">Д.</span><span class="sxs-lookup"><span data-stu-id="1c798-182">E.</span></span> <span data-ttu-id="1c798-183">На странице Регистрация веб-перехватчика центра партнеров в потоке выберите **выполнить**.</span><span class="sxs-lookup"><span data-stu-id="1c798-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="1c798-184">Укажите **URL-адрес HTTP** от первого действия в **центре партнеров до потока Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="1c798-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="1c798-185">Выберите все четыре параметра в разделе регистрируемые **события** и выберите **Да** для перезаписи.</span><span class="sxs-lookup"><span data-stu-id="1c798-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="1c798-186">Вопросы и ответы о запуске и обслуживании</span><span class="sxs-lookup"><span data-stu-id="1c798-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="1c798-187">Как устранить неполадки в случае сбоев при выполнении потока Power автоматизиру?</span><span class="sxs-lookup"><span data-stu-id="1c798-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="1c798-188">Сведения о том, как обеспечить выполнение потоков Power автоматизиру в соответствии с ожиданиями и устранить ошибки во время выполнения, см. в статье [Устранение сбоев потока](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="1c798-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="1c798-189">Что делать, если вы видите ссылки, которые не были правильно синхронизированы в центре партнеров или в среде CRM?</span><span class="sxs-lookup"><span data-stu-id="1c798-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="1c798-190">Чтобы определить состояние синхронизации ссылок, выберите **Аудит**.</span><span class="sxs-lookup"><span data-stu-id="1c798-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Сообщение об ошибке, запрашивающее вход":::

<span data-ttu-id="1c798-192">Убедитесь, что выполняются следующие условия.</span><span class="sxs-lookup"><span data-stu-id="1c798-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="1c798-193">Идентификатор решения предоставляется в составе возможности.</span><span class="sxs-lookup"><span data-stu-id="1c798-193">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="1c798-194">Требуется указать двухбуквенный код страны.</span><span class="sxs-lookup"><span data-stu-id="1c798-194">Two letter country code is required.</span></span>

- <span data-ttu-id="1c798-195">Если для возможности выбрана Справка Майкрософт, требуются контактные данные клиента.</span><span class="sxs-lookup"><span data-stu-id="1c798-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="1c798-196">Как убедиться, что ссылка будет синхронизироваться двунаправленно?</span><span class="sxs-lookup"><span data-stu-id="1c798-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="1c798-197">Выполните следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="1c798-197">Do the following steps:</span></span>

- <span data-ttu-id="1c798-198">Партнер продавцов должен убедиться, что у них включена функция **синхронизации с центром партнеров** в разделе CRM.</span><span class="sxs-lookup"><span data-stu-id="1c798-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Сообщение об ошибке, запрашивающее вход":::

- <span data-ttu-id="1c798-200">Продавцов необходимо предоставить доход и дату закрытия, когда уточняется интерес.</span><span class="sxs-lookup"><span data-stu-id="1c798-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="1c798-201">Если идентификатор CRM указан на этапе **создания** или **обновления** возможности совместной продажи, но Потенциальная сделка с этим идентификатором не найдена в CRM, то обновление или создание будет проигнорировано.</span><span class="sxs-lookup"><span data-stu-id="1c798-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="1c798-202">Убедитесь, что поле ссылочная Валюта настроено в среде Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1c798-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="1c798-203">Что делать, если соединитель отключается и вы пропустили синхронизацию ссылок.</span><span class="sxs-lookup"><span data-stu-id="1c798-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="1c798-204">Ниже приведены некоторые варианты, которые можно испытать.</span><span class="sxs-lookup"><span data-stu-id="1c798-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="1c798-205">Проверьте, истек ли срок действия имени пользователя или пароля для пользователя центра партнеров с ролями администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="1c798-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="1c798-206">Можно вернуться к несинхронизированной возможности, внести незначительное обновление и проверить, синхронизирована ли ссылка.</span><span class="sxs-lookup"><span data-stu-id="1c798-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="1c798-207">Если потоки запущены и завершились сбоем, выберите последовательность и повторно отправьте выполнение, которое завершилось сбоем.</span><span class="sxs-lookup"><span data-stu-id="1c798-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="1c798-208">Что делать при возникновении ошибок отказа в доступе?</span><span class="sxs-lookup"><span data-stu-id="1c798-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="1c798-209">Убедитесь, что соответствующие роли существуют.</span><span class="sxs-lookup"><span data-stu-id="1c798-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="1c798-210">Роль администратора ссылок для продавца центра партнеров</span><span class="sxs-lookup"><span data-stu-id="1c798-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="1c798-211">Системный администратор или роль System настройщика в экземпляре CRM</span><span class="sxs-lookup"><span data-stu-id="1c798-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="1c798-212">Убедитесь, что пользователь учетной записи потока Power автоматизиру входит в систему https://flow.microsoft.com по крайней мере один раз</span><span class="sxs-lookup"><span data-stu-id="1c798-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="1c798-213">Если вы видите, что **код страны для учетной записи клиента** отсутствует при создании возможности совместной продажи, что делать?</span><span class="sxs-lookup"><span data-stu-id="1c798-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="1c798-214">Вам потребуется добавить двухбуквенный код страны ISO в учетную запись клиента в CRM.</span><span class="sxs-lookup"><span data-stu-id="1c798-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="1c798-215">Что делать, если вы видите сообщение об ошибке, когда **требуется идентификатор решения** при создании возможности совместной продажи?</span><span class="sxs-lookup"><span data-stu-id="1c798-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="1c798-216">Чтобы создать ссылку на совместную продажу, вам потребуется решение, готовое к совместной продаже корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1c798-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="1c798-217">Что делать, если вы видите возможности совместной продажи, созданные в центре партнеров, которые не синхронизированы с CRM, несмотря на отсутствие ошибок в потоках:</span><span class="sxs-lookup"><span data-stu-id="1c798-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="1c798-218">Выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="1c798-218">Do the following:</span></span>

- <span data-ttu-id="1c798-219">После создания новой сделки по совместной работе в центре партнеров проверьте, вызывается ли в центре партнеров протокол Dynamics 365 (он может быть вызван несколько раз).</span><span class="sxs-lookup"><span data-stu-id="1c798-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="1c798-220">Если поток вызывается, проверьте все вызванные потоки и укажите выполнение потока, которое обновит CRM.</span><span class="sxs-lookup"><span data-stu-id="1c798-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="1c798-221">Вы можете выполнить действия и проверить, не обновлялось ли приложение в CRM или возникла проблема.</span><span class="sxs-lookup"><span data-stu-id="1c798-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="1c798-222">Ознакомьтесь с *новыми сделками*\* в центре партнеров, чтобы узнать, заполнен ли он идентификатором CRM.</span><span class="sxs-lookup"><span data-stu-id="1c798-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="1c798-223">Убедитесь, что сделка не была случайно закрыта как "выигран" или "потеряна" в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="1c798-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1c798-224">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1c798-224">Next steps</span></span>

- [<span data-ttu-id="1c798-225">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="1c798-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="1c798-226">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="1c798-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)