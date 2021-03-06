---
title: Как подтвердить, что ваш клиент принял условия Клиентского соглашения Майкрософт для программы CSP
description: Прежде чем заказывать службы Майкрософт для клиентов, партнеры в рамках программы "Поставщик облачных решений" (CSP) должны подтвердить принятие условий Клиентского соглашения Майкрософт.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277017"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Как подтвердить, что ваш клиент принял условия Клиентского соглашения Майкрософт для программы CSP

**Соответствующие роли**: агент по администрированию | агент по продажам


Клиенты могут принять условия Клиентского соглашения Майкрософт двумя способами.

**Вариант 1** Утверждение принятия условий партнером. Партнер может подтвердить согласие клиента с помощью API, пакета SDK или панели мониторинга Центра партнеров.

**Вариант 2** Прямое принятие условий клиентом. У партнера есть возможность пригласить клиента с помощью URL-адреса для просмотра и принятия условий соглашения в Центре администрирования Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Получение шаблона Клиентского соглашения Майкрософт

Вы можете вручную скачать последнюю версию шаблона Клиентского соглашения Майкрософт [отсюда](https://aka.ms/customeragreement). Клиентские соглашения Майкрософт для разных стран могут отличаться. При запросе шаблона Клиентского соглашения Майкрософт обязательно выберите страну, в которой находится клиент.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Вариант 1. Подтверждение принятия клиентом условий соглашения в Центре партнеров

Партнеры с прямым выставлением счетов могут подтвердить принятие условий Клиентского соглашения Майкрософт в Центре партнеров для новых и уже имеющихся клиентов. Косвенные торговые посредники не могут утверждать принятие условий от имени своих клиентов и должны обращаться к своему непрямому поставщику, чтобы подтвердить согласие клиентов.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Подтверждение принятия условий соглашения новыми клиентами

При создании нового клиента в Центре партнеров выполните следующие действия, чтобы подтвердить принятие условий соглашения клиентом. Для выполнения этих действий необходимо быть агентом администрирования или агентом по продажам.

1. Выберите **Клиенты**, а затем — **Новый клиент**.

2. В разделе **Сведения об учетной записи** введите сведения о компании и ее основном контактном лице.

3. В разделе **Соглашение корпорации Майкрософт** установите флажок, чтобы подтвердить, что клиент принял условия Клиентского соглашения Майкрософт.

4. В разделе **Дата принятия условий соглашения** введите соответствующую дату. Здесь нельзя указать дату, которая еще не наступила.

5. Убедитесь, что отображаются правильные контактные данные основного контактного лица. Если это не так, выберите **Обновить** и введите точные сведения о лице, принявшем условия соглашения.

6. Выберите **Далее**, чтобы продолжить создание арендатора клиента.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Новый клиент":::.  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Подтвердите согласие клиента для существующих клиентов

Для выполнения этой процедуры вы должны быть агентом администрирования или агентом по продажам.

1. Выберите **Клиенты**. Найдите и выберите клиента.

2. Выберите **Сведения об учетной записи**.

3. В разделе **Клиентское соглашение Майкрософт** выберите **Обновить**.

4. Введите **Имя**, **Фамилию**, **Адрес электронной почты** и **Номер телефона** (необязательно) пользователя, принявшего условия соглашения. В разделе **Дата принятия условий соглашения** введите соответствующую дату. Здесь нельзя указать дату, которая еще не наступила.

5. Выберите **Сохранить** и продолжайте.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Существующий клиент":::.

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Получение подтверждения о принятии условий клиентом

Чтобы получить подтверждение того, что существующий клиент принял условия Клиентского соглашения Майкрософт, выполните описанные ниже действия. Для выполнения этой процедуры вы должны быть агентом администрирования или агентом по продажам.

1. Выберите **Клиенты**, а затем найдите и выберите необходимого клиента.

2. Выберите **Сведения об учетной записи**.

3. В разделе **Клиентское соглашение Майкрософт** просмотрите, было ли предоставлено этим клиентом подтверждение.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Подтверждение принятия клиентом условий использования API или пакета SDK Центра партнеров

Для подтверждения принятия клиентом условий Клиентского соглашения Майкрософт можно использовать API или пакет SDK Центра партнеров. Дополнительные сведения об этом API или пакете SDK:

- [Получение метаданных соглашения для Клиентского соглашения Майкрософт](/partner-center/develop/get-customer-agreement-metadata)

- [Подтверждение принятия клиентом условий Клиентского соглашения Майкрософт](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Получение подтверждения принятия клиентом условий клиентского соглашения Майкрософт](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Получение ссылки для скачивания шаблона клиентского соглашения Майкрософт](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Вариант 2. Принятие клиентом условий в центре администрирования Microsoft 365

Партнеры могут пригласить новых и существующих клиентов, отправив им соответствующий URL-адрес, чтобы они могли просмотреть и принять условия соглашения в центре администрирования Microsoft 365. В следующих разделах описывается, как:

- создать клиента и пригласить его для просмотра и принятия условий соглашения;

- пригласить нового клиента для просмотра и принятия условий взаимоотношений с торговым посредником и условий соглашения;

- пригласить имеющегося клиента для просмотра и принятия условий соглашения.

>[!NOTE]
> Вы можете использовать [пакет SDK или API Центра партнеров](/partner-center/develop/get-direct-sign-status-of-customer-agreement), чтобы получить состояние прямого принятия Клиентского соглашения Майкрософт.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Создание клиента и его приглашение для просмотра и принятия условий соглашения

Выполните следующие действия, чтобы создать учетные данные для клиента в Центре партнеров и пригласить его для просмотра и принятия условий Клиентского соглашения Майкрософт в центре администрирования Microsoft 365.

1. На вкладке **Клиенты** в Центре партнеров выберите **Добавить клиента**.

2. В разделе **Сведения об учетной записи** введите сведения о новом клиенте во всех обязательных полях, включая название компании клиента и основное контактное лицо.

3. В разделе **Клиентское соглашение** выберите элемент **Клиенту будет предложено принять Клиентское соглашение Майкрософт в Центре администрирования Microsoft 365**. Заполните все остальные обязательные поля на странице.

4. Выберите **Далее: отзыв** и выполните инструкции по созданию арендатора клиента. 

>[!NOTE] 
>Новые клиенты не смогут осуществить покупку, пока не примут условия Клиентского соглашения Майкрософт.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Создание нового клиента":::.

5. При переходе на страницу **Подтверждение** в процессе создания клиента сохраните учетные данные этого клиента. Позже эти учетные данные необходимо будет предоставить клиенту.

6. Вне Центра партнеров создайте и отправьте клиенту электронное сообщение с приглашением принять условия Клиентского соглашения Майкрософт в центре администрирования Microsoft 365. Обязательно добавьте в это электронное сообщение:

   - ссылку на этот [URL-адрес](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (требуется вход);

   - учетные данные клиента, которые вы сохранили на шаге 5.

7. Клиент получит приглашение от партнера по электронной почте и перейдет по предложенному [URL-адресу](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Он войдет в Центр администрирования Microsoft 365, используя предоставленные вами учетные данные.

9. Клиент установит флажок, чтобы принять условия Клиентского соглашения Майкрософт.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Приглашение нового клиента для просмотра и принятия условий взаимоотношений с торговым посредником и условий соглашения 

Чтобы пригласить нового клиента для просмотра и принятия условий взаимоотношений с торговым посредником и условий соглашения, выполните следующее. 

1. На вкладке **Клиенты** в Центре партнеров щелкните ссылку **Запросить установление взаимоотношений с торговым посредником**. 

2. Будет создан шаблон автоматического электронного сообщения, содержащего текст и ссылку с параметризованным URL-адресом для перехода в центр администрирования Microsoft 365.

3. Можно настроить автоматически создаваемый шаблон электронного сообщения, а затем выбрать **Скопировать в буфер обмена** или **Открыть в сообщении электронной почты**.

4. Используйте этот шаблон электронного сообщения, чтобы пригласить клиента для принятия запроса на установление **взаимосвязи с торговым посредником** и условий **Клиентского соглашения Майкрософт**. (Примечание. В электронное приглашение партнер должен также добавить URL-адрес, предоставляемый автоматически, и учетные данные клиента, которые были недавно созданы.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Создание взаимосвязи":::.

5. Клиент получит приглашение по электронной почте и щелкнет ссылку на параметризованный URL-адрес. 

6. Для входа в Центр администрирования Microsoft 365 он введет учетные данные, предоставленные вами в электронном сообщении.

7. Затем клиент установит флажок, чтобы принять условия **взаимосвязи с торговым посредником** и условия **Клиентского соглашения Майкрософт**. 

8. С помощью того же URL-адреса клиент может просмотреть объединенный список доступных деловых партнеров. Он может выбрать партнера для просмотра подробных сведений.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Принятие соглашения.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Приглашение имеющегося клиента для просмотра и принятия условий соглашения

Чтобы пригласить имеющегося клиента для просмотра и принятия условий Клиентского соглашения Майкрософт, выполните следующее. 

1. Создайте электронное сообщение, приглашающее клиента принять условия Клиентского соглашения Майкрософт, и добавьте в него соответствующий URL-адрес.

2. Клиент получит приглашение по электронной почте и щелкнет этот [URL-адрес](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Клиент введет свои учетные данные в Центре администрирования Microsoft 365.

4. Затем клиент установит флажок, чтобы принять условия Клиентского соглашения Майкрософт. 

5. С помощью того же URL-адреса он может просмотреть объединенный список доступных деловых партнеров. Он может выбрать партнера для просмотра подробных сведений.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Клиент":::.

>[!NOTE]
>В некоторых случаях у клиентов может отсутствовать возможность напрямую принять условия Клиентского соглашения Майкрософт. Чтобы узнать больше об этих ситуациях, прочтите представленный ниже раздел "Два сценария, в которых требуется утверждение от имени клиента".

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Два сценария, в которых требуется утверждение от имени клиента

Есть два сценария, в которых клиенты не могут напрямую принять условия Клиентского соглашения Майкрософт в Центре администрирования Microsoft 365.

**Сценарий 1.** Существующий клиент приобрел что-либо из следующего в рамках установленных партнерских отношений: предложения, программное обеспечение или подписки на него, зарезервированные экземпляры либо план Azure. Теперь клиент пытается осуществить новую покупку (это не относится к автоматическому продлению). Когда этот клиент щелкнет URL-адрес, он увидит сообщение "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement" (Обратитесь к своему партнеру, чтобы подтвердить согласие с условиями Клиентского соглашения Майкрософт).  

**Как это исправить** Необходимо утвердить принятие условий от имени клиента.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Снимок экрана со страницей Центра администрирования Microsoft 365 и предложением обратиться к партнеру, чтобы подтвердить принятие Клиентского соглашения Майкрософт.":::

**Сценарий 2** Существующий клиент приобрел что-либо из следующего: предложения, программное обеспечение и подписки на программное обеспечение, зарезервированные экземпляры, план Azure. Теперь клиент пытается осуществить новую покупку через нового партнера.

Когда этот клиент щелкнет ссылку на Центр администрирования Microsoft 365, чтобы принять условия сотрудничества с новым партнером и соглашения, он увидит сообщение "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement" (Обратитесь к своему партнеру, чтобы подтвердить согласие с условиями Клиентского соглашения Майкрософт).  

**Как это исправить** Необходимо утвердить принятие условий от имени клиента.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Подтверждение того, что клиент принял соглашение

Если вы пытаетесь создать новый заказ для существующего клиента, от которого еще не получено подтверждение принятия условий соглашения, вам будет предложено выполнить процедуру подтверждения. Выполните следующие действия.

1. Введите **Имя**, **Фамилию**, **Адрес электронной почты** и **Номер телефона** (необязательно) пользователя, принявшего условия соглашения.

2. В разделе **Дата принятия условий соглашения** введите соответствующую дату. Здесь нельзя указать дату, которая еще не наступила.

3. Выберите **Сохранить и продолжить**. 

## <a name="next-steps"></a>Дальнейшие действия

- [Проверка или обновление сведений в профиле компании](update-your-partner-profile.md)
- [Клиентские соглашения Майкрософт (по региону и языку)](Agreements.md)
