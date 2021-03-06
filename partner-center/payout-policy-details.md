---
title: Расписания и процессы выплат
description: Сведения о выплатах и транзакциях, таких как расписания оплаты и процессы рекаупмент для Azure Marketplace и других транзакций.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: bcecd4c31d80a4130331c652491e7951af180c67
ms.sourcegitcommit: f1255fb65eac6ee2e0ff0cb95cc16a02dc57fc1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "110582429"
---
# <a name="payout-schedules-and-processes"></a>Расписания и процессы выплат

**Соответствующие роли**: Администратор учетной записи | Глобальный администратор

В этой статье рассматривается график оплаты корпорации Майкрософт, где можно найти состояние выплаты и процесс неуплаты клиента.

## <a name="payment-schedules"></a>Расписания оплаты

В следующих разделах описывается процесс выплат для **Соглашение Enterprise** , а **также для соглашений клиента Майкрософт или** для транзакций CSP.

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Транзакции, когда у клиента есть Соглашение Enterprise

Когда клиент приобретает продукт из Microsoft AppSource или Azure Marketplace с использованием существующих Соглашение Enterprise Майкрософт для транзакций, мы будем выставлять выплаты в следующем цикле выплаты 30-дневного счета клиента. Транзакции, в которых клиент использует кредитную карту, имеют 30-дневный период времени до выплаты.

Плата часто возникает до того, как корпорация Майкрософт собирает платеж от клиента. Действия, которые мы принимаем, если клиент не оплачивает Майкрософт, но уже выдавали [оплату](#process-for-customer-non-payment) , см. ниже.

| Событие | Описание | Видимость отчетов | Временных |
| --- | --- | --- | --- |
| Использование или месяц транзакции | Клиент использует или покупает службу. | Панель мониторинга " [Использование](/azure/marketplace/partner-center-portal/usage-dashboard) " или " [заказ](/azure/marketplace/partner-center-portal/orders-dashboard) " | **Месяц 1** |
| Корпорация Майкрософт вычисляет сумму выставления счетов | Определение общего использования, всего транзакций | Панель мониторинга " [Использование](/azure/marketplace/partner-center-portal/usage-dashboard) " или " [заказ](/azure/marketplace/partner-center-portal/orders-dashboard) " | **Месяц 2** |
| Выплата опубликована | Определение тарифных выплат и доходов на выплаты | Помечается как необработанный в журнале транзакций в [отчете о выплатах](payout-statement.md) | **Месяц 3 (1-я неделя)** |
| Подготовить выплата | Доходы подготавливаются для ежемесячного платежа | Помечается как предстоящий в журнале транзакций в [отчете о выплатах](payout-statement.md) | **Месяц 3 (1-я неделя)** |
| **Выплата отправлена** | **Платеж отправляется издателю** | **Помечается как отправленный в журнале транзакций и в разделе выплат [оператора выплаты](payout-statement.md)** | **Месяц 3 (не позднее 15)** |
| Счет оплачивается клиентом | Корпорация Майкрософт собирает платеж от клиента | Без изменения. | **Месяц с 4 по 12** |
|

\* Дата вывыплаты в стандартном Тихоокеанском времени (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Временная шкала платежей для клиентов с соглашением Enterprise.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Транзакции, когда клиент имеет соглашение с клиентами Майкрософт или CSP

Все покупки с кредитной картой или ежемесячным счетом имеют 30-дневный период, чтобы обеспечить сбор фондов от клиента.

| Событие | Описание | Видимость отчетов | Временных |
| --- | --- | --- | --- |
| Использование или месяц транзакции | Клиент использует или покупает службу. | Панель мониторинга " [Использование](/azure/marketplace/partner-center-portal/usage-dashboard) " или " [заказ](/azure/marketplace/partner-center-portal/orders-dashboard) " | **Месяц 1** |
| Счет оплачивается клиентом | Определение общего использования, общего значения транзакции и счета за оплату клиента | Панель мониторинга " [Использование](/azure/marketplace/partner-center-portal/usage-dashboard) " или " [заказ](/azure/marketplace/partner-center-portal/orders-dashboard) " | **Месяц 2** |
| Выплата опубликована | Определение тарифных выплат и доходов на выплаты | Помечается как необработанный в журнале транзакций в [отчете о выплатах](payout-statement.md) | **Месяц 2** |
| 30-дневный период удержания | Обеспечение сбора фондов, возможных гибких и денежных запросов | Помечается как необработанный в журнале транзакций в [отчете о выплатах](payout-statement.md) | **Месяц 3** |
| Подготовить выплата | Доходы подготавливаются для ежемесячного платежа | Помечается как предстоящий в журнале транзакций в [отчете о выплатах](payout-statement.md) | **Месяц 4 (1-я неделя)** |
| **Выплата отправлена** | **Платеж отправляется издателю** | **Помечается как отправленный в журнале транзакций и в разделе выплат [оператора выплаты](payout-statement.md)** | **Месяц 4 (не позднее 15)** |
|

\* Дата вывыплаты в стандартном Тихоокеанском времени (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Временная шкала платежей для клиентов кредитных карт и счетов.":::

## <a name="process-for-customer-non-payment"></a>Процесс неуплаты клиента

В редких случаях корпорация Майкрософт не может получать платежи от клиентов на приобретение коммерческих рынков. Когда клиент не оплачивается корпорацией Майкрософт в соответствии с графиком выставления счетов, мы начнем процесс сбора. Этот процесс занимает примерно четыре месяца и включает постоянное взаимодействие с Майкрософт. Если оплата не получена по окончании этого процесса, Майкрософт выводит средства в виде несобранных средств.

В соответствии с описанным здесь процессом выплаты Корпорация Майкрософт могла уже платить средства издателям (вы), которые в итоге будут недоступными. Поэтому у нас есть процесс сверки этих сумм.

Корпорация Майкрософт будет рекауп любые выплаты, уже оплаченные Вами, используя один из следующих методов: (1) корпорация Майкрософт может вычесть неоплаченные суммы из будущих выплат; Например, если в выплатах $1 000 недоступна и списана сумма, будущие выплаты будут удерживаться до тех пор, пока $1 000 не будет восстановлена или (2) корпорация Майкрософт может запросить возмещения или издателей по накладным для любых несобранных сумм.

Пример имеет следующее расписание:

| Событие | Приблизительная дата * | Видимость партнера |
| --- | --- | --- |
| Пример даты вывыплаты | 10/15/2020 | Помечаются как **Отправленные** в журнале транзакций и в разделе "платежи" на панели мониторинга выплата |
| <font color="red">Если клиент не оплачивает Майкрософт</font> | 12/2/2020 – 12/5/2020 | Без изменений, как и выше |
| Клиент получает сообщение о первой поздней оплате | 12/6/2020 | Нет |
| Клиент получает обычные сообщения электронной почты по возрастанию срочности | 12/7/2020 – 1/31/2021 | Нет |
| Скорее всего, издатель получает уведомления о списании. | 1/7/2021 | - |
| Клиент получает уведомление об увольнении | 2/1/2021 | Нет |
| Завершение процесса сбора/фонды списаны | 2/15/2021 | Уведомление по электронной почте, отправленное издателю, что средства были списаны. |
| Выплата вычитается | 01.03.2021 | Издатель увидит отрицательную транзакцию в заявлении о выплатах центра партнеров |
| Выплата удержана | 3/15/2021 | Будущие выплаты выводятся в заявлении о выплатах центра партнеров. Издатель не сможет получить оплату, пока баланс больше не будет отрицательным.  |
|||

\* Дата вывыплаты в стандартном Тихоокеанском времени (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Число дней, на которое платежи попадают в счет выплата

Мы, как правило, отправляют оплату за определенный месяц на 15-й день этого месяца, но для оплаты вашей учетной записи потребуется еще одно время. Количество дней зависит от способа оплаты, используемого для вашей учетной записи, как описано ниже.

> [!NOTE]
> Указанные ниже дни являются приблизительными. любой платеж может занять больше или меньше времени для достижения вашей учетной записи.

| Способ оплаты     | Количество дней до поступления на счет для выплат     |
|--------------------|--------------------------------------------|
| PayPal             | 1 рабочий день                             |
| ACH/SEPA           | 2–3 рабочих дня                          |
| Банковский перевод      | 7–10 рабочих дней                         |
|

## <a name="next-steps"></a>Дальнейшие действия

- [Сведения о налогах](tax-details-marketplace.md)
