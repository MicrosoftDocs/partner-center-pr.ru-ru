---
title: Приступая к переходу на план Azure
description: Все, что нужно знать вам и вашим клиентам о плане Azure с оплатой по мере использования, включая первые шаги, меры безопасности и как приступить к работе.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 58feabdefb02660559c69f61190070310768b947
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149661"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Начало перехода на тарифы с оплатой по мере использования для плана Azure

**Соответствующие роли**: агент по администрированию | агент по продажам


Корпорация Майкрософт представила новую коммерческую модель в Центре партнеров.  Благодаря этой новой модели партнеры смогут предлагать службы Azure по тарифам с оплатой по мере использования клиентам, подписавшим клиентский договор с Майкрософт.

Этот план упрощает процесс приобретения — в одном плане Azure может быть несколько подписок Azure. Вам больше не нужно отправлять отдельный заказ для каждой подписки Azure. И в этой новой коммерческой модели для Azure мы руководствовались принципом единых глобальных цен, что позволит партнерам CSP предлагать решения Azure по опубликованным ценам.

Потребности клиентов в цифровом преобразовании требуют от партнеров новых навыков. Многие клиенты ищут партнеров, предоставляющих услуги, которые не ограничиваются непосредственно переходом, чтобы облегчить миграцию в облако и эффективно использовать службы Azure. Партнеры корпорации Майкрософт играют важную роль на всех этапах жизненного цикла клиента. Партнерские услуги по сути являются непрерывными и включают мониторинг инфраструктуры Azure, управление политиками и общее управление, установку и настройку конфигурации, техническую поддержку и многое другое. Для использования этих служб требуется, чтобы партнер был тесно знаком со средой Azure клиента и имел возможность непрерывного и полноценного управления базовыми ресурсами, которыми клиент управляет. Партнеры по выставлению счетов, предоставляющие услуги круглосуточного управления облачными операциями, будут иметь право на получение **партнерских баллов за управляемые ими службы**.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Убедитесь, что ваши клиенты подписали клиентский договор с Майкрософт

С 1 октября 2019 г. доступно Клиентское соглашение Майкрософт — бессрочное соглашение, которое упрощает и оптимизирует приобретение за счет полностью цифрового процесса. Все клиенты, желающие воспользоваться преимуществами новой коммерческой модели в CSP для Azure, должны подписать клиентский договор с Майкрософт.

Партнеры, которые хотят совершать транзакции в рамках нового плана Azure и создавать новые заказы, должны подтвердить принятие клиентом Клиентского соглашения Майкрософт, используя панель мониторинга Центра партнеров и API в рабочей среде.

1 февраля 2020 г. существующее соглашение об использовании Microsoft Cloud перестанет использоваться в программе CSP. С этой даты для всех других предложений, включая Microsoft 365, Dynamics 365 и существующие предложения Azure, будет требоваться подтверждение партнера о принятии клиентом нового Клиентского соглашения Майкрософт. Партнеры, участвующие в программе CSP, не смогут создать новый заказ для клиента без подтверждения принятия Клиентского соглашения Майкрософт.

Полные сведения представлены в разделе [Подтверждение принятия клиентом условий клиентского соглашения Майкрософт](confirm-customer-agreement.md).

## <a name="security-and-access-control-practices"></a>Методики обеспечения безопасности и контроля доступа

В целях защиты партнеров и клиентов мы вводим набор обязательных требований к безопасности для консультантов, поставщиков панелей управления и партнеров, участвующих в программе поставщиков облачных решений.

Партнеры, которые не выполнят обязательные требования к безопасности, не смогут осуществлять транзакции в программе для поставщиков облачных решений или управлять клиентами, используя делегированные права администратора, после соблюдения этих требований. В настоящее время мы устанавливаем дату технического применения этих требований, а после уведомим партнеров о ней, предоставив подробные сведения.

## <a name="actions-to-take-to-implement-mfa"></a>Действия, выполняемые для реализации MFA

Учитывая высокий уровень привилегии партнеров, мы должны обеспечить для каждого пользователя появление запроса MFA при выполнении каждой отдельной проверки подлинности. Это можно сделать одним из следующих способов.

- Можно реализовать Azure AD Premium и применить многофакторную проверку подлинности для каждого пользователя.
- Можно реализовать [параметры безопасности Azure AD по умолчанию](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).
- Реализация стороннего решения и обеспечение применения MFA для каждого пользователя.

Начиная с 1 августа 2019 года все партнеры обязаны применять в своем арендаторе многофакторную проверку подлинности для всех пользователей, включая учетные записи служб. Подробные сведения об этих требованиях к безопасности можно найти в разделе [Требования к безопасности для партнеров](partner-security-requirements.md).

Корпорация Майкрософт рекомендует партнерам осмотрительно использовать RBAC, следуя рекомендациям раздела [Что такое Azure AD Privileged Identity Management?](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="read-more-about-the-azure-plan"></a>Прочитайте больше о плане Azure:

- [Приобретение плана Azure](purchase-azure-plan.md)

- [Сравнение предложений Azure](compare-azure-offers.md)

- [Общие сведения о партнерских баллах](partner-earned-credit.md)

- Формулы расчета партнерских баллов (PEC), а также роли и разрешения, дающие право на получение этих баллов, указаны в прейскуранте на Панели мониторинга Центра партнеров (требуется вход).

## <a name="next-steps"></a>Дальнейшие действия 

- [Как вычисляются и выплачиваются партнерские баллы](partner-earned-credit-explanation.md)
- [Прейскурант для новой коммерческой модели Azure в CSP](azure-plan-price-list.md)
- [Перевод клиентов на план Azure](azure-plan-transition.md)
- [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md)
- [Полный список стран и регионов, в которых доступен план Azure](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)