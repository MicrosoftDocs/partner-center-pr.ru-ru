---
title: Перенос подписки Azure на другого партнера
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как изменить партнера программы поставщика облачных решений, связанного с подписками Azure клиента.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856072"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Сведения о передаче клиентской подписки Azure другому партнеру

Область **применения**: центр партнеров | Центр партнеров по Microsoft Cloud для государственных организаций США

**Соответствующие роли**: глобальный администратор

В этой статье описывается, как клиент может переключить свои Microsoft Azureные службы с одного поставщика облачных решений (CSP) на другой.

Чтобы переключить службы Azure или подписки клиента на другого партнера, выполните эти действия вручную. И партнер, и клиент должны выполнить эти действия.

>[!Note]  
>Сейчас только прямые или косвенные поставщики могут передавать подписки.
>Вы не можете изменить партнеров для подписок поставщиков облачных решений, связанных с планами Azure, Office 365, Enterprise Mobility Suite или подписками Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Переключение партнеров для подписок Azure

1. Для передачи подписки Azure новому партнеру клиент должен инициировать процесс и обратиться к текущему зарегистрированному партнеру в письменном виде.

   >[!Note]
   > Создание заявки на обслуживание, инициирующей процесс передачи, входит в обязанности текущего партнера. Microsoft не может вмешиваться в процесс от имени клиента или нового партнера. Клиент должен тщательно спланировать взаимодействие с текущим партнером, чтобы переход прошел без проблем.

2. Участнику подписки необходимо выполнить следующие задачи:

   Создать запрос в службу поддержки Azure в Центре партнеров, чтобы запросить форму передачи подписки:

   1. В меню Центр партнеров выберите **Клиенты**, выберите клиента в списке, а затем — **Управление службами**.

   2. В разделе **Запросы в службу поддержки** выберите раскрывающееся меню **Новый запрос** и нажмите **Microsoft Azure**.
   
   3. В [портал Azure](https://portal.azure.com)выберите **новый запрос в службу поддержки**.
   
   4. На шаге 1 выберите **Управление подписками** в качестве типа проблемы, укажите идентификатор нужной подписки и выберите **Поставщик облачных решений** в качестве плана поддержки.
   
   5. На шаге 2 выберите **C — минимальные последствия** и в качестве типа проблемы выберите **другие общие вопросы** .
   
   6. Скачайте [форму передачи подписки CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. Партнер для подписки: заполните [форму передачи подписки CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), подпишите ее и отправьте клиенту. 

   Чтобы заполнить форму, вам потребуются следующее сведения:

   - Контактные данные и идентификатор Майкрософт текущего партнера. В меню Центра партнеров выберите **Параметры учетной записи** &gt; **Профиль организации** и используйте **идентификатор Майкрософт**, **название организации** и **адрес**, указанные здесь.

   - Идентификатор Майкрософт клиента. В меню Центра партнеров выберите **Клиенты**, а затем разверните раздел описания клиента, чтобы узнать **идентификатор Майкрософт**.

   - Идентификатор передаваемой подписки. В развернутом описании клиента выберите **Смотреть подписки**, а затем разверните выбранную подписку, чтобы просмотреть ее **идентификатор**.

   >[!Note]
   >Передача подписки приводит к появлению у нее двух идентификаторов, которые будут отображаться на странице **Редактирование подписки** передаваемой подписки: **1**- ИД подписки в Центре партнеров используется для выставления счетов. **2** — исходный ИД подписки Azure сохраняется и будет отображаться в Центре партнеров, а также на портале управления Azure. Этот идентификатор будет отображаться в файле выверки.  **При регистрации запросов в службу поддержки необходимо использовать оба идентификатора.**

4. Клиент и новый партнер для подписки:

   Изучите форму, введите информацию о новом партнере и подпишите ее. Убедитесь, что нового клиента есть действующее соглашение. Отправьте форму текущему зарегистрированному партнеру.

   *Важно!* если у нового партнера CSP нет связи с клиентом, он должен установить его до передачи подписки. [Сведения о том, как это сделать, можно найти здесь](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Новый партнер CSP и клиент клиента должны быть в одной стране. 

5. Текущий партнер:

   Убедитесь, что в форме есть контактные данные для обоих администраторов партнеров. Служба поддержки Майкрософт свяжется с обоими администраторами для проверки перемещения. Убедитесь, что у вас есть все три подписи. Затем используйте параметр **отправить файл** , чтобы присоединить завершенную форму к существующему запросу на обслуживание. Инженер службы поддержки Майкрософт вернет вас в течение восьми рабочих часов, чтобы проверить получение и завершение.

6. Новый партнер:

   Обновите параметры подписки Azure, чтобы удалить старого партнера из учетной записи. Чтобы узнать, какие назначения ролей подготавливаются, запустите два командлеты PowerShell.

   - Добавьте нового партнера как торгового посредника в учетной записи:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > **Идентификатор** клиента клиента отображается в центре партнеров в качестве **идентификатора Майкрософт** клиента. Чтобы найти идентификатор Майкрософт (идентификатор клиента) для конкретного клиента, войдите на [панель мониторинга](https://partner.microsoft.com/dashboard)центра партнеров. Затем в меню выберите **Клиенты** . В списке щелкните клиент. Щелкните стрелку вниз, чтобы развернуть список клиента. Вы увидите сведения о *доменном имени* клиента и **идентификаторе Майкрософт** клиента. Используйте 16-значный **идентификатор Майкрософт** в PowerShell командлет.

   - Просмотрите роли в учетной записи, в том числе для предыдущих партнеров CSP:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Удалить устаревшие разрешения на доступ:

   - В меню Центра партнеров выберите **Клиенты**.
   - В списке щелкните клиент. Выберите (дважды щелкните) название организации. Это действие открывает страницу клиентские **подписки** .
   - В меню сведения о клиенте выберите **Управление службами**.
   - В разделе **Microsoft Azure** выберите ссылку для перехода к **портал управления Microsoft Azure**.

## <a name="next-steps"></a>Дальнейшие действия

- Скачайте [форму передачи подписки CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Узнайте о [поддержке нескольких партнеров](multipartner.md).

- [Поддержка нескольких партнеров](multipartner.md).
- [Поддержка нескольких каналов](multichannel.md).
- [Перенос подписок Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)