---
title: Отчет о соблюдении требований к безопасности
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как проверить соблюдение требований к безопасности с помощью соответствующего отчета и отчета об MFA в Центре партнеров
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: a429706848a469aace2704d4eaf3d57898ae578f
ms.sourcegitcommit: d96ad93449da4c914becfffab167cdc1aa165ada
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "112915632"
---
# <a name="security-requirements-status-report"></a>Отчет о соблюдении требований к безопасности

**Соответствующие роли**: администратор CPV | глобальный администратор

В этой статье рассказывается об отчете о соблюдении требований к безопасности в Центре партнеров. Этот отчет предоставляет метрики соответствия с [требованиями к безопасности для партнеров](partner-security-requirements.md) по прохождению многофакторной проверки подлинности (MFA) пользователями в вашем арендаторе партнера.

Чтобы получить доступ к отчету в [Центре партнеров](https://partner.microsoft.com/dashboard), последовательно выберите элементы **Параметры** > **Параметры учетной записи** > **Состояние требований безопасности**. Этот отчет обновляется ежедневно и включает данные о входе за последние семь дней.

>[!NOTE]
>Отчет о соблюдении требований к безопасности доступен только в Центре партнеров. Он недоступен в Microsoft Cloud for US Government и Microsoft Cloud Germany. Мы настоятельно рекомендуем всем партнерам, осуществляющим операции через национальное облако (для государственных организаций США и для Германии), немедленно внедрить эти новые требования к безопасности. Но эти партнеры сейчас не обязаны обеспечивать соответствие новым требованиям к безопасности. Корпорация Майкрософт предоставит дополнительные сведения о применении этих требований к безопасности для национальных облаков в будущем.

## <a name="security-status-metrics"></a>Метрики состояния безопасности

В отчете о соблюдении требований к безопасности представлены полезные сведения о реализации MFA у партнеров.Кроме того, отчет содержит метрики конфигурации MFA и сведения о действиях с арендаторами партнеров в Центре партнеров. В следующих разделах подробно описаны эти метрики.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Конфигурация MFA в арендаторе клиента

Метрика **Доля включенных учетных записей пользователей с принудительным применением MFA с использованием приведенных здесь вариантов:** отображает данные о доле включенных учетных записей пользователей в арендаторе клиента, для которых принудительно применяется MFA. Для обеспечения соответствия вы можете использовать один из таких [вариантов MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Эти данные сохраняются и формируются в отчет ежедневно. Например:

- Contoso — это партнер CSP с 110 учетными записями пользователей в клиенте, 10 из которых отключены. 
- Из 100 оставшихся учетных записей пользователей в 90 применяется один из указанных [вариантов MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Поэтому метрика показывает значение 90 %. 

### <a name="partner-center-requests-with-mfa"></a>Запросы с MFA к Центру партнеров

Каждый раз, когда ваши сотрудники входят в Центр партнеров для работы или используют интерфейсы API для получения или отправки данных через Центр партнеров, их состояние безопасности проверяется и отслеживается. Кроме того, отслеживание состояния безопасности охватывает ваши приложения и все приложения поставщиков панелей управления. Эти данные отображаются в метриках в разделе **Процент запросов к Центру партнеров с использованием MFA**. Сведения приводятся за последние семь дней.

#### <a name="dashboard-mfa-verification"></a>Проверка с MFA на панели мониторинга

Метрика **Использование портала Центра партнеров** связана с действиями на панели мониторинга Центра партнеров. Она измеряет процент операций, выполненных пользователями, которые прошли проверку MFA. Например:

- Contoso — это партнер CSP с двумя агентами-администраторами, Джейн и Джоном.
- В первый день Джейн вошла на Панель мониторинга Центра партнеров без проверки MFA и выполнила три операции.
- На второй день Джон вошел на Панель мониторинга Центра партнеров без проверки MFA и выполнил пять операций.
- На третий день Джейн вошла на Панель мониторинга Центра партнеров, пройдя проверку MFA, и выполнила две операции.
- Ни один из агентов не выполнял никаких операций в течение оставшихся четырех дней.
- Из 10 операций, выполненных в течение семи дней, только две были выполнены с проверкой MFA. Поэтому метрика показывает значение 20 %.

Ознакомьтесь с файлом **запросов портала без MFA**, чтобы понять, какой пользователь вошел на Панель мониторинга Центра партнеров без проверки MFA, и получить сведения о последнем посещении в окне отчетности.

#### <a name="appuser-mfa-verification"></a>Проверка с MFA для приложений и пользователей

Метрика **Использование API или пакета SDK** связана с аутентификацией приложений и пользователей с помощью запросов API Центра партнеров. Она измеряет процент запросов к API, выполненных с помощью маркера доступа с утверждением MFA. Например:

- Компания Fabrikam является партнером CSP и использует приложение CSP, которое сочетает методы проверки подлинности приложения и пользователя и проверки подлинности только приложения.
- В первый день приложение отправило три запроса API, снабженных маркером доступа, который получен с использованием метода проверки подлинности приложения и пользователя без проверки MFA.
- На второй день приложение отправило пять запросов API, снабженных маркером доступа, который получен с использованием метода проверки подлинности только приложения.
- На третий день приложение отправило два запроса API, снабженных маркером доступа, который получен с использованием метода проверки подлинности приложения и пользователя с проверкой MFA.
- Ни один из агентов не выполнял никаких операций в течение оставшихся четырех дней.
- Отправленные на второй день пять запросов к API, снабженных маркером доступа, который получен с использованием метода проверки подлинности только приложения, не учитываются в метрике, так как они не использовали учетные данные пользователя. Две из оставшихся пяти операций снабжены маркером доступа, полученным с использованием проверки MFA. Поэтому метрика показывает значение 40 %.

Если вы хотите понять, какие действия приложения и пользователя привели к тому, что метрики не показывают 100 %, просмотрите следующие файлы:

- **Сводка по запросам API**, чтобы получить сведения об общем состоянии MFA по приложению.
- **Все запросы API**, чтобы получить сведения о каждом запросе API, выполненном пользователями вашего клиента. Для оптимальной загрузки результат будет содержать не более 10 000 последних запросов.

## <a name="actions-for-mfa-status-below-100"></a>Действия для состояния MFA со значением менее 100 %

У некоторых партнеров, которые реализовали MFA, метрики отчета могут сообщать о значении менее 100 %. Чтобы понять, почему это так, следует учесть некоторые факторы.

> [!NOTE]
> Вам нужно будет обратиться к кому-нибудь в вашей организации, кто знаком с управлением удостоверениями и реализацией MFA для вашего арендатора партнера.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Реализованная проверка MFA для арендатора партнера

Для обеспечения соответствия вы должны реализовать MFA для арендатора партнера. Сведения о реализации MFA см. в статье [Требования к безопасности для партнеров, использующих Центр партнеров или API-интерфейсы Центра партнеров](partner-security-requirements.md).

>[!NOTE]
> Метрики MFA вычисляются ежедневно с учетом операций, выполненных за последние семь дней. Если вы только недавно завершили реализацию MFA для арендатора партнера, метрики могут не показывать значение 100 %.

### <a name="verify-mfa-on-all-user-accounts"></a>Проверка MFA для всех учетных записей пользователей

Определите, охватывает ли текущая реализация MFA все учетные записи пользователей или только некоторые из них. Некоторые решения MFA основаны на политиках и поддерживают исключение пользователей, а другие могут требовать явного включения MFA для каждого пользователя по отдельности. Убедитесь, что ни один пользователь не исключен из текущей реализации MFA. Любая учетная запись пользователя, которая исключена, но используется для входа в Центр партнеров и выполнения каких-либо действий, связанных с CSP, CPV или консультантом, может быть причиной того, что метрики не показывают значение 100 %.

### <a name="review-your-mfa-conditions"></a>Проверка условий MFA

Определите, применяется ли MFA в вашей текущей реализации только в конкретных условиях. Некоторые решения MFA обеспечивают гибкость, позволяя применять MFA при соблюдении определенных условий. Например, пользователь подключается с неизвестного устройства или из неизвестного расположения. Пользователь, которому разрешено использовать MFA, но это не является обязательным при доступе к Центру партнеров, может быть причиной того, что метрики не показывают 100 %.

>[!NOTE]
>Важное примечание для партнеров, которые внедрили MFA с помощью средств безопасности Azure AD по умолчанию. Для учетных записей пользователей без прав администратора будет применяться многофакторная проверка подлинности с учетом риска. Пользователям будет предлагаться пройти MFA только при попытках входа с риском (к примеру, пользователь выполняет вход из другого расположения). Кроме того, пользователям предоставляется 14 дней на регистрацию для использования MFA. Пользователи, которые не выполнили регистрацию для использования MFA, не будут получать запросы защиты MFA в течение 14-дневного периода. Поэтому предполагается, что метрики не будут показывать 100 % для партнеров, которые реализовали MFA с помощью средств безопасности Azure AD о умолчанию.

### <a name="review-third-party-mfa-configurations"></a>Проверка сторонних конфигураций MFA

Если вы используете стороннее решение MFA, определите, как вы интегрируете его с Azure AD. Как правило, существуют два метода, включая федерацию и пользовательские элементы управления.

* **Федерация удостоверений**. Когда Azure AD получает запрос на аутентификацию, Azure AD перенаправляет пользователя к федеративному поставщику удостоверений для выполнения аутентификации. После успешной аутентификации федеративный поставщик удостоверений перенаправляет пользователя обратно в Azure AD, снабдив его маркером SAML. Чтобы система Azure AD могла убедиться, что пользователь прошел проверку MFA при аутентификации в федеративном поставщике удостоверений, маркер SAML должен содержать утверждение *authenticationmethodsreferences* (со значением *multipleauthn*). Проверьте, поддерживает ли федеративный поставщик удостоверений выдачу такого утверждения. Если это так, проверьте, настроен ли для этого федеративный поставщик удостоверений. Если утверждение отсутствует, Azure AD (и, следовательно, Центр партнеров) не узнает, что пользователь прошел проверку MFA, и поэтому метрика может не показывать 100 %.

* **Пользовательский элемент управления**. Пользовательский элемент управления Azure AD невозможно использовать, чтобы определить, прошел ли пользователь проверку MFA с помощью стороннего решения MFA. В результате все пользователи, которые прошли проверку MFA с помощью пользовательского элемента управления, всегда будут отображаться в Azure AD (и, следовательно, в Центре партнеров) как пользователи, не прошедшие проверку MFA. При интеграции с Azure AD рекомендуется перейти на использование федерации удостоверений вместо пользовательского элемента управления, когда это возможно.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Определение пользователей, которые вошли в Центр партнеров без MFA

Может быть полезно определить, какие пользователи входят в Центр партнеров без проверки MFA, и проверить их в соответствии с текущей реализацией MFA. Вы можете использовать [отчет о входе в Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins), чтобы узнать, проходил ли пользователь проверку MFA. Отчет о входе в Azure AD сейчас доступен только партнерам, подписавшимся на Azure AD Premium или любой номер SKU Office 365, который включает в себя Azure AD Premium (например, EMS).

## <a name="next-steps"></a>Дальнейшие действия

- [Сообщество группы рекомендаций по безопасности для Центра партнеров](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Требования к безопасности для партнеров](partner-security-requirements.md)
- [Часто задаваемые вопросы о требованиях к безопасности для партнеров](partner-security-requirements-faq.yml)
