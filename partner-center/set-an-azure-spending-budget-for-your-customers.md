---
title: Установка расходного бюджета Azure для клиентов
ms.topic: how-to
ms.date: 03/17/2021
description: Узнайте, как устанавливать или удалять месячные бюджеты расходов на Azure для клиентов, а также просматривать данные о расходах Azure и задавать уведомления, связанные с бюджетом.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855358"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Установка, проверка и удаление ежемесячных бюджетных расходов Azure для клиентов в центре партнеров

**Соответствующие роли**: Агент администрирования

Вы можете [задать ежемесячный бюджет расходов на Azure для клиентов](#set-azure-spending-budget) в центре партнеров. Это помогает Вашим клиентам управлять расходами на Azure. Этот параметр позволяет сравнить расходы на Azure с бюджетом в течение месяца. Кроме того, он позволяет клиентам вычислять затраты на Azure, чтобы их месячный счет не превышал ожидаемый объем.

> [!NOTE]  
> Эта функция недоступна в "песочнице" или "тестирование" в рабочей учетной записи (TIP).

После того как вы [настроили бюджет расходов Azure для ваших клиентов](#set-azure-spending-budget), вы также можете просматривать сведения об использовании клиентов следующими способами. Эти параметры могут помочь вам выявить неправильно настроенные службы или необычные тенденции, которые могут предложить мошенничество. Затем вы можете работать с клиентами для выяснения основной причины и управления затратами. При необходимости можно также [изменить бюджет клиента](#set-azure-spending-budget) на более высокий.

- [Проверка текущих расходов Azure](#check-current-azure-spending)

- [Включить уведомления по электронной почте, когда расходы клиента приближается к лимиту бюджета](#notifications-for-budget-limits)

- [Просмотр детализированных затрат по службе для подписок на основе использования](#itemized-costs-by-service)

Вы также можете [Удалить бюджет расходов Azure](#remove-azure-spending-budget) для клиентов в любое время.

## <a name="azure-spending-data"></a>Данные о расходах Azure

Данные о расходах Azure — это *Оценка* , и *фактические суммы счетов могут отличаться*. Значение данных *не отражает* налоги, кредиты, корректировки и другие расходы, которые могут быть применены.

Данные о расходах *обновляются раз в день*. Ваши клиенты могут по-прежнему использовать и заставлять счета за использование служб и ресурсов Azure, если не изменить параметры учетной записи в портал Azure.

## <a name="set-azure-spending-budget"></a>Настройка бюджета расходов Azure

Вы можете *задать ежемесячный бюджет расходов на Azure* для нескольких клиентов в центре партнеров:

1. Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).

2. В меню слева в разделе **CSP** выберите **затраты на Azure**.

3. На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** выберите клиентов, для которых требуется задать бюджет.

4. Введите значение для **месячного бюджета**.

5. Нажмите кнопку **Применить** , чтобы сохранить изменения.

Вы также можете *задать бюджет для отдельного клиента* в параметрах подписки:

1. Войдите на панель мониторинга Центра партнеров.

2. В меню слева в разделе **CSP** выберите **Customers (клиенты**).

3. На странице **Клиенты** выберите **название компании** клиента.

4. На странице **подписки** клиента в разделе **Подписка на основе использования** выберите **изменить бюджет**.

5. Введите значение для бюджета.

6. Нажмите кнопку **Применить** , чтобы сохранить изменения.

## <a name="remove-azure-spending-budget"></a>Удаление бюджета расходов Azure

Вы можете *Удалить месячный бюджет расходов на Azure* для ваших клиентов в центре партнеров:

1. Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).

2. В меню слева в разделе **CSP** выберите **затраты на Azure**.

3. На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** выберите клиентов, бюджет которых необходимо удалить.

4. Выберите **Удалить бюджет**.

## <a name="check-current-azure-spending"></a>Проверка текущих расходов Azure

Вы можете в любое время *отслеживанию текущих затрат Azure и ежемесячных бюджетов клиентов* :

1. Войдите на [панель мониторинга Центра партнеров](https://partner.microsoft.com/dashboard/).

2. В меню слева в разделе **CSP** выберите **затраты на Azure**.

3. На странице " **расходы Azure** " в разделе **Клиенты с подпиской Microsoft Azure** вы можете просмотреть обзор месячных бюджетов клиентов, оценки текущих расходов и процент использования бюджета.

## <a name="notifications-for-budget-limits"></a>Уведомления об ограничениях бюджета

Вы можете *включить уведомления по электронной почте* , когда месячные затраты клиента приближается к лимиту бюджета. При включении этого параметра вы получите уведомления, когда клиенты будут использовать 80% или больше ежемесячного бюджета. Этот параметр позволяет следить за счетом Azure. Настройка уведомлений по электронной почте:

1. Войдите в Центр партнеров.

2. Перейдите в меню **Параметры**.

3. Выберите **Мои предпочтения**.

4. Если вы этого не сделали, настройте предпочтительный адрес электронной почты.

5. Настройте предпочтительный язык для уведомления.

6. Выберите вкладку **CSP** в разделе **Параметры уведомления** .

7. Установите флажок Электронная почта для уведомления **Azure о расходах** и **Сохраните**.


## <a name="itemized-costs-by-service"></a>Детализированные затраты по службам

Можно *Просмотреть детализированные затраты (и предполагаемое использование) службой для подписок на основе использования*:

1. Войдите в Центр партнеров.

2. В меню слева в разделе **CSP** выберите **Customers (клиенты**).

3. На странице **Клиенты** выберите **название компании** клиента.

4. На странице **подписки** клиента в разделе **подписки на основе использования** выберите имя **подписки**.

5. На странице подписки можно просматривать **детализированные затраты** по службам и **оценивать использование** за текущий месяц.


## <a name="next-steps"></a>Дальнейшие действия

- [Новый интерфейс для коммерческих приложений в CSP. Выставление счетов в Azure](azure-plan-billing.md)
