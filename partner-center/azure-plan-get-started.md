---
title: Приступая к переходу на план Azure | Центр партнеров
ms.topic: article
ms.date: 10/15/2019
description: ''
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: eb46255403297539c17145b82ecf096699abe390
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171269"
---
# <a name="move-to-azure-plan---get-started"></a>Приступая к переходу на план Azure

Корпорация Майкрософт представила новую коммерческую модель в CSP для партнеров Azure, которые подписали соглашение с партнером Майкрософт. Благодаря этой новой модели партнеры смогут предлагать службы Azure по тарифам с оплатой по мере использования клиентам, подписавшим клиентский договор с Майкрософт. 

Этот план упрощает процесс приобретения — в одном плане Azure может быть несколько подписок Azure. Вам больше не нужно отправлять отдельный заказ для каждой подписки Azure. И в этой новой коммерческой модели для Azure мы руководствовались принципом единых глобальных цен, что позволит партнерам CSP предлагать решения Azure по опубликованным ценам. 

Потребности клиентов в цифровом преобразовании требуют от партнеров новых навыков. Многие клиенты ищут партнеров, предоставляющих услуги, которые не ограничиваются непосредственно переходом, чтобы облегчить миграцию в облако и эффективно использовать службы Azure. Партнеры корпорации Майкрософт играют важную роль на всех этапах жизненного цикла клиента. Эти службы для партнеров являются оперативными: это мониторинг инфраструктуры Azure, управление политиками и общее управление, общая и точная настройка, техническая поддержка, а также множество других служб. Для использования этих служб требуется, чтобы партнер был тесно знаком со средой Azure клиента и имел возможность непрерывного и полноценного управления базовыми ресурсами, которыми клиент управляет. Партнеры по выставлению счетов, предоставляющие услуги круглосуточного управления облачными операциями, будут иметь право на получение **партнерских баллов за управляемые ими службы**.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Убедитесь, что ваши клиенты подписали клиентский договор с Майкрософт

С 1 октября 2019 года клиентский договор с Майкрософт (бессрочное соглашение, которое упрощает и оптимизирует приобретение за счет полностью цифрового процесса) можно заключать с помощью цифровой подписи. Все клиенты, желающие воспользоваться преимуществами новой коммерческой модели в CSP для Azure, должны подписать клиентский договор с Майкрософт.

Полные сведения представлены в разделе [Подтверждение принятия клиентом условий клиентского соглашения Майкрософт](confirm-customer-agreement.md).

## <a name="security-and-access-control-practices"></a>Методики обеспечения безопасности и контроля доступа

В целях обеспечения защиты для партнеров и клиентов мы вводим набор обязательных требований к безопасности для консультантов, поставщиков панели управления и партнеров, участвующих в программе для поставщиков облачных решений. 

Партнеры, которые не выполнят обязательные требования к безопасности, не смогут осуществлять транзакции в программе для поставщиков облачных решений или управлять клиентами, используя делегированные права администратора, после соблюдения этих требований. В настоящее время мы устанавливаем дату технического применения этих требований, а после уведомим партнеров о ней, предоставив подробные сведения. 

## <a name="actions-to-take-to-implement-mfa"></a>Действия, выполняемые для реализации MFA 

Учитывая высокий уровень привилегии партнеров, мы должны обеспечить для каждого пользователя появление запроса MFA при выполнении каждой отдельной проверки подлинности. Это можно сделать одним из следующих способов.

- Можно реализовать Azure AD Premium и применить многофакторную проверку подлинности для каждого пользователя. 
- Можно реализовать базовые политики защиты. 
- Реализация стороннего решения и обеспечение применения MFA для каждого пользователя. 

Начиная с 1 августа 2019 года все партнеры обязаны применять в своем арендаторе многофакторную проверку подлинности для всех пользователей, включая учетные записи служб. Подробные сведения об этих требованиях к безопасности можно найти в разделе [Требования к безопасности для партнеров](https://docs.microsoft.com/partner-center/partner-security-requirements). 

Корпорация Майкрософт рекомендует партнерам осмотрительно использовать RBAC, следуя рекомендациям раздела [Что такое Azure AD Privileged Identity Management?](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure ) 

## <a name="read-more-about-the-azure-plan"></a>Прочитайте больше о плане Azure:

- [Приобретение плана Azure](purchase-azure-plan.md)

- [Сравнение предложений Azure](compare-azure-offers.md)

- [Общие сведения о партнерских баллах](partner-earned-credit.md)

- Формулы расчета партнерских баллов (PEC), а также роли и разрешения, дающие право на получение этих баллов, указаны в прейскуранте на Панели мониторинга Центра партнеров (требуется вход).

- [Как вычисляются и выплачиваются партнерские баллы](partner-earned-credit-explanation.md)

- [Прейскурант для новой коммерческой модели Azure в CSP](azure-plan-price-list.md)

- [Перевод клиентов на план Azure](azure-plan-transition.md)

- [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md)

- [Полный список стран и регионов, в которых доступен план Azure](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)

 


