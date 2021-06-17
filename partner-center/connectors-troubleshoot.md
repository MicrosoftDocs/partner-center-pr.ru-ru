---
title: Устранение проблем с соединителями рефералов при совместных продажах
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ознакомьтесь с ответами на распространенные вопросы об использовании соединителей совместной продажи. Сведения об устранении неполадок соединителей совместных продаж см. в этой статье.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276941"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="6751b-104">Устранение проблем с соединителями рефералов при совместных продажах</span><span class="sxs-lookup"><span data-stu-id="6751b-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="6751b-105">**Применимо к**: Dynamics 365 CRM | SalesForce CRM</span><span class="sxs-lookup"><span data-stu-id="6751b-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="6751b-106">**Соответствующие роли**: администратор ссылок | Системный администратор или Настройщик системы в CRM</span><span class="sxs-lookup"><span data-stu-id="6751b-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="6751b-107">Вопросы и ответы о предварительных требованиях</span><span class="sxs-lookup"><span data-stu-id="6751b-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="6751b-108">Можно ли использовать для вашей среды решение соединителей для совместных продаж?</span><span class="sxs-lookup"><span data-stu-id="6751b-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="6751b-109">Если вы используете тестовую или промежуточную среду, вы можете выбрать пробную версию решения.</span><span class="sxs-lookup"><span data-stu-id="6751b-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="6751b-110">Платная версия соединителей доступна в AppSource за 15 долларов США в месяц.</span><span class="sxs-lookup"><span data-stu-id="6751b-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="6751b-111">С платным подключением вы будете получать вызовы API 10000 в день.</span><span class="sxs-lookup"><span data-stu-id="6751b-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="6751b-112">Соединители являются оболочками на основе API-интерфейсов ссылок центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="6751b-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="6751b-113">Каждый раз, когда решения соединителя выполняются для событий **создания** или **обновления** на стороне центра партнеров или CRM, выполняется вызов API.</span><span class="sxs-lookup"><span data-stu-id="6751b-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="6751b-114">Какую роль необходимо создать в среде CRM?</span><span class="sxs-lookup"><span data-stu-id="6751b-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="6751b-115">Пользователи, являющиеся системными администраторами или настройщиками системы, могут применять изменения для всех.</span><span class="sxs-lookup"><span data-stu-id="6751b-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="6751b-116">Однако все пользователи приложений могут персонализировать систему и даже использовать некоторые настройки совместно с другими пользователями.</span><span class="sxs-lookup"><span data-stu-id="6751b-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="6751b-117">Требуются ли партнерским продавцов специальные роли для работы в центре партнеров?</span><span class="sxs-lookup"><span data-stu-id="6751b-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="6751b-118">Партнеру продавцов должна быть назначена роль "Администратор ссылок".</span><span class="sxs-lookup"><span data-stu-id="6751b-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="6751b-119">Дополнительные сведения см. в разделе [Общие сведения о разрешениях](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="6751b-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="6751b-120">Какие поля необходимо настроить в среде CRM первыми?</span><span class="sxs-lookup"><span data-stu-id="6751b-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="6751b-121">• Убедитесь, что Ваша валюта подходит для вашего расположения и правильно находится в среде CRM.</span><span class="sxs-lookup"><span data-stu-id="6751b-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="6751b-122">• Группа продаж должна быть указана в среде CRM в качестве пользователей CRM.</span><span class="sxs-lookup"><span data-stu-id="6751b-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="6751b-123">Какие предварительные требования необходимы для создания среды Power автоматизиру?</span><span class="sxs-lookup"><span data-stu-id="6751b-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="6751b-124">Чтобы использовать среду Power автоматизиру, вам потребуется:</span><span class="sxs-lookup"><span data-stu-id="6751b-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="6751b-125">Требуется лицензия Power автоматизиру.</span><span class="sxs-lookup"><span data-stu-id="6751b-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="6751b-126">Требуется не менее 1 ГБ хранилища.</span><span class="sxs-lookup"><span data-stu-id="6751b-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="6751b-127">Нужна ли вам подписка Dynamics 365 для использования решения соединителей Salesforce?</span><span class="sxs-lookup"><span data-stu-id="6751b-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="6751b-128">Решение соединителя Salesforce имеет тип "Dynamics Flow", поддерживающий синхронизацию с другими системами CRM.</span><span class="sxs-lookup"><span data-stu-id="6751b-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="6751b-129">Для решения не требуется наличие экземпляра Dynamics 365 или подписки.</span><span class="sxs-lookup"><span data-stu-id="6751b-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="6751b-130">При установке решения Salesforce может появиться раскрывающийся список с существующей средой для работы с компакт-дисков в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="6751b-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="6751b-131">Необходимо выбрать эту среду.</span><span class="sxs-lookup"><span data-stu-id="6751b-131">You need to select that environment.</span></span> <span data-ttu-id="6751b-132">Кроме того, если возникает ошибка "не удалось найти организацию Dynamics 365, подключенную к пользователю, выполнившего вход", необходимо создать новую среду для соединителя.</span><span class="sxs-lookup"><span data-stu-id="6751b-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="6751b-133">Вопросы и ответы о конфигурации</span><span class="sxs-lookup"><span data-stu-id="6751b-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="6751b-134">Что делать, если при активации последовательностей в платформе Power автоматизировать произошла следующая ошибка?</span><span class="sxs-lookup"><span data-stu-id="6751b-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="6751b-135">Ошибка: запрос к Azure Resource Manager завершился с ошибкой: "{" Error ": {" Code ":" Воркфловтригжернотфаунд "," Message ":" не удалось найти рабочий процесс "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" триггер "Manual". "}}".</span><span class="sxs-lookup"><span data-stu-id="6751b-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="6751b-136">Выполните следующие действия по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="6751b-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="6751b-137">Удалите подключение к компакт-дискам, а затем Воссоздайте подключения к компакт-дискам.</span><span class="sxs-lookup"><span data-stu-id="6751b-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="6751b-138">Включение и отключение дочернего потока</span><span class="sxs-lookup"><span data-stu-id="6751b-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="6751b-139">Удалите решение, а затем переустановите решение.</span><span class="sxs-lookup"><span data-stu-id="6751b-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="6751b-140">Что делать, если во время добавления соединителя центра партнеров в платформу Power автоматизиру, вы сталкиваетесь с ошибкой входа?</span><span class="sxs-lookup"><span data-stu-id="6751b-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Сообщение об ошибке, обязательное для входа.":::

<span data-ttu-id="6751b-142">Выполните следующие действия по устранению неполадок:</span><span class="sxs-lookup"><span data-stu-id="6751b-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="6751b-143">Используйте учетные данные центра партнеров, чтобы войти в среду потока один раз (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="6751b-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="6751b-144">Что делать, если вы получаете следующую ошибку при активации центра партнеров в CRM Flow на платформе Power автоматизиру?</span><span class="sxs-lookup"><span data-stu-id="6751b-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Сообщение об ошибке, запрашивающее обновления.":::

<span data-ttu-id="6751b-146">Выполните следующие действия по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="6751b-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="6751b-147">Прежде чем активировать центр партнеров до CRM Flow, активируйте следующие два дочерних потока.</span><span class="sxs-lookup"><span data-stu-id="6751b-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="6751b-148">Центр партнеров в CRM — вспомогательный (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="6751b-149">Центр партнеров обновления справочных данных по Microsoft CRM (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="6751b-150">Что делать, если вы не можете добавить подключения к потоку при попытке изменить последовательность?</span><span class="sxs-lookup"><span data-stu-id="6751b-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="6751b-151">Вы добавляете подключения к потоку во время выполнения последовательности и добавляете их в каждый поток по отдельности.</span><span class="sxs-lookup"><span data-stu-id="6751b-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="6751b-152">Если диалоговое окно для добавления подключений не открывается автоматически при редактировании потока, то можно изменить каждый из шагов и подзадач каждого потока по отдельности.</span><span class="sxs-lookup"><span data-stu-id="6751b-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="6751b-153">Выберите каждый поток и измените их по отдельности.</span><span class="sxs-lookup"><span data-stu-id="6751b-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="6751b-154">Развернуть все шаги в последовательности</span><span class="sxs-lookup"><span data-stu-id="6751b-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Шаги, требующие подключения.":::

- <span data-ttu-id="6751b-156">Выберите шаги, на которых отображается значок предупреждения, предлагающий связать подключения и добавить подключения.</span><span class="sxs-lookup"><span data-stu-id="6751b-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Пошаговое изменение последовательности.":::


5. <span data-ttu-id="6751b-158">Что делать, если в решении "соединители для совместной продажи" не включены потоки?</span><span class="sxs-lookup"><span data-stu-id="6751b-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="6751b-159">A.</span><span class="sxs-lookup"><span data-stu-id="6751b-159">A.</span></span> <span data-ttu-id="6751b-160">В Power Автоматизация необходимо изменить последовательности в следующем порядке и обновить их для использования правильных подключений:</span><span class="sxs-lookup"><span data-stu-id="6751b-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="6751b-161">Регистрация веб-перехватчика центра партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="6751b-162">Создание ссылки на совместную продажу — Salesforce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6751b-163">Центр партнеров обновления справочных обновлений в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="6751b-164">Центр партнеров в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="6751b-165">SalesForce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6751b-166">Возможность Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6751b-167">Решения Майкрософт для Salesforce в центре партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="6751b-168">Б.</span><span class="sxs-lookup"><span data-stu-id="6751b-168">B.</span></span> <span data-ttu-id="6751b-169">Для каждого потока выберите параметр **выполнять только пользователей** .</span><span class="sxs-lookup"><span data-stu-id="6751b-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="6751b-170">Выберите **использовать соединение** вместо **предоставленного пользователем только для запуска**.</span><span class="sxs-lookup"><span data-stu-id="6751b-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Для активации последовательности.":::


<span data-ttu-id="6751b-172">В.</span><span class="sxs-lookup"><span data-stu-id="6751b-172">C.</span></span> <span data-ttu-id="6751b-173">Активируйте указанные ниже потоки.</span><span class="sxs-lookup"><span data-stu-id="6751b-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="6751b-174">Центр партнеров обновления справочных обновлений в Salesforce (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="6751b-175">SalesForce в центр партнеров (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6751b-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="6751b-176">Г.</span><span class="sxs-lookup"><span data-stu-id="6751b-176">D.</span></span> <span data-ttu-id="6751b-177">Активируйте все оставшиеся потоки.</span><span class="sxs-lookup"><span data-stu-id="6751b-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="6751b-178">Д.</span><span class="sxs-lookup"><span data-stu-id="6751b-178">E.</span></span> <span data-ttu-id="6751b-179">На странице Регистрация веб-перехватчика центра партнеров в потоке выберите **выполнить**.</span><span class="sxs-lookup"><span data-stu-id="6751b-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="6751b-180">Укажите **URL-адрес HTTP** от первого действия в **центре партнеров до потока Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="6751b-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="6751b-181">Выберите все четыре параметра в разделе регистрируемые **события** и выберите **Да** для перезаписи.</span><span class="sxs-lookup"><span data-stu-id="6751b-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="6751b-182">Вопросы и ответы о запуске и обслуживании</span><span class="sxs-lookup"><span data-stu-id="6751b-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="6751b-183">Как устранить неполадки во время выполнения потока Power автоматизиру?</span><span class="sxs-lookup"><span data-stu-id="6751b-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="6751b-184">Сведения о том, как обеспечить выполнение потоков Power автоматизиру в соответствии с ожиданиями и устранить ошибки во время выполнения, см. в статье [Устранение сбоев потока](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="6751b-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="6751b-185">Что делать, если вы видите ссылки, которые не были правильно синхронизированы в центре партнеров или в среде CRM?</span><span class="sxs-lookup"><span data-stu-id="6751b-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="6751b-186">Чтобы определить состояние синхронизации ссылок, выберите **Аудит**.</span><span class="sxs-lookup"><span data-stu-id="6751b-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Как синхронизировать ссылки.":::

<span data-ttu-id="6751b-188">Убедитесь, что выполняются следующие условия.</span><span class="sxs-lookup"><span data-stu-id="6751b-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="6751b-189">ИДЕНТИФИКАТОР решения предоставляется в составе возможности.</span><span class="sxs-lookup"><span data-stu-id="6751b-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="6751b-190">Требуется указать двухбуквенный код страны.</span><span class="sxs-lookup"><span data-stu-id="6751b-190">Two letter country code is required.</span></span>

- <span data-ttu-id="6751b-191">Если для возможности выбрана Справка Майкрософт, требуются контактные данные клиента.</span><span class="sxs-lookup"><span data-stu-id="6751b-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="6751b-192">Как убедиться, что ссылка будет синхронизироваться двунаправленно?</span><span class="sxs-lookup"><span data-stu-id="6751b-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="6751b-193">Выполните следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="6751b-193">Do the following steps:</span></span>

- <span data-ttu-id="6751b-194">Партнер продавцов должен убедиться, что у них включена функция **синхронизации с центром партнеров** в разделе CRM.</span><span class="sxs-lookup"><span data-stu-id="6751b-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Убедитесь, что вы включили синхронизацию.":::

- <span data-ttu-id="6751b-196">Продавцов необходимо предоставить доход и дату закрытия, когда уточняется интерес.</span><span class="sxs-lookup"><span data-stu-id="6751b-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="6751b-197">Если идентификатор CRM указан на этапе **создания** или **обновления** возможности совместной продажи, но Потенциальная сделка с этим идентификатором не найдена в CRM, то обновление или создание будет проигнорировано.</span><span class="sxs-lookup"><span data-stu-id="6751b-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="6751b-198">Убедитесь, что поле ссылочная Валюта настроено в среде Salesforce.</span><span class="sxs-lookup"><span data-stu-id="6751b-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="6751b-199">Что делать, если соединитель отключается и вы пропустили синхронизацию ссылок?</span><span class="sxs-lookup"><span data-stu-id="6751b-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="6751b-200">Ниже приведены некоторые варианты, которые можно испытать.</span><span class="sxs-lookup"><span data-stu-id="6751b-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="6751b-201">Проверьте, истек ли срок действия имени пользователя или пароля для пользователя центра партнеров с ролями администратора ссылок.</span><span class="sxs-lookup"><span data-stu-id="6751b-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="6751b-202">Можно вернуться к несинхронизированной возможности, внести незначительное обновление и проверить, синхронизирована ли ссылка.</span><span class="sxs-lookup"><span data-stu-id="6751b-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="6751b-203">Если потоки запущены и завершились сбоем, выберите последовательность и повторно отправьте выполнение, которое завершилось сбоем.</span><span class="sxs-lookup"><span data-stu-id="6751b-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="6751b-204">Что делать при возникновении ошибок отказа в доступе?</span><span class="sxs-lookup"><span data-stu-id="6751b-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="6751b-205">Убедитесь, что соответствующие роли существуют.</span><span class="sxs-lookup"><span data-stu-id="6751b-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="6751b-206">Роль администратора ссылок для продавца центра партнеров</span><span class="sxs-lookup"><span data-stu-id="6751b-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="6751b-207">Системный администратор или роль System настройщика в экземпляре CRM</span><span class="sxs-lookup"><span data-stu-id="6751b-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="6751b-208">Убедитесь, что пользователь учетной записи потока Power автоматизиру входит в систему https://flow.microsoft.com по крайней мере один раз</span><span class="sxs-lookup"><span data-stu-id="6751b-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="6751b-209">Если вы видите, что **код страны для учетной записи клиента** отсутствует при создании возможности совместной продажи, что делать?</span><span class="sxs-lookup"><span data-stu-id="6751b-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="6751b-210">Вам потребуется добавить двухбуквенный код страны ISO в учетную запись клиента в CRM.</span><span class="sxs-lookup"><span data-stu-id="6751b-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="6751b-211">Что делать, если вы видите сообщение об ошибке, когда **требуется идентификатор решения** при создании возможности совместной продажи?</span><span class="sxs-lookup"><span data-stu-id="6751b-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="6751b-212">Чтобы создать ссылку на совместную продажу, вам потребуется решение, готовое к совместной продаже корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6751b-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="6751b-213">Что делать, если вы видите возможности совместной продажи, созданные в центре партнеров, которые не синхронизированы с CRM, несмотря на отсутствие ошибок в потоках?</span><span class="sxs-lookup"><span data-stu-id="6751b-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="6751b-214">Выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6751b-214">Do the following:</span></span>

- <span data-ttu-id="6751b-215">После создания новой сделки по совместной работе в центре партнеров проверьте, вызывается ли в центре партнеров протокол Dynamics 365 (он может быть вызван несколько раз).</span><span class="sxs-lookup"><span data-stu-id="6751b-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="6751b-216">Если поток вызывается, проверьте все вызванные потоки и укажите выполнение потока, которое будет обновлять CRM.</span><span class="sxs-lookup"><span data-stu-id="6751b-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="6751b-217">Вы можете выполнить действия и проверить, не обновлялось ли приложение в CRM или возникла проблема.</span><span class="sxs-lookup"><span data-stu-id="6751b-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="6751b-218">Ознакомьтесь с **новой разделом** в центре партнеров, чтобы узнать, заполнен ли он идентификатором CRM.</span><span class="sxs-lookup"><span data-stu-id="6751b-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="6751b-219">Убедитесь, что сделка не была случайно закрыта как **выигранная** или **потеряна** в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="6751b-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6751b-220">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="6751b-220">Next steps</span></span>

- [<span data-ttu-id="6751b-221">Управление потенциальными клиентами</span><span class="sxs-lookup"><span data-stu-id="6751b-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="6751b-222">Управление возможностями совместной продажи</span><span class="sxs-lookup"><span data-stu-id="6751b-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
