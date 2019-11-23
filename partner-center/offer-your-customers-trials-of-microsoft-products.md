---
title: Предлагайте клиентам пробные версии продуктов Майкрософт | Центр партнеров
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ваши клиенты могут ознакомиться с продуктами Майкрософт, доступными по подписке, в течение 30 дней. You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384829"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Предложение клиентам пробных версий продуктов Майкрософт

Область применения

- Центр партнеров

Чтобы продемонстрировать клиентам новые продукты Майкрософт, рекомендуется предлагать 30-дневные бесплатные пробные версии. Процесс регистрации для получения пробной версии продукта из каталога аналогичен процессу регистрации во многих других веб-службах. Предложение доступно для всех партнеров.

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. Например, они могут получить одну бесплатную пробную версию для Office 365 бизнес премиум и одну для Office 365 E3. However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

Бесплатные пробные версии будут доступны для следующих продуктов:

- Office 365 бизнес премиум
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility & Security E5
- План 1 Dynamics 365 Enterprise Customer Engagement
- Dynamics 365 for Financials
- Microsoft 365 бизнес

Мы предоставляем бесплатные пробные версии для этих продуктов, поскольку они являются наиболее полными и популярными бизнес-предложениями. В будущем мы можем добавить другие предложения для бесплатных пробных версий.

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. В подразделе **Периодичность выставления счетов** в каталоге щелкните **Пробная версия**. При этом отобразятся только бесплатные пробные версии, а платные предложения будут скрыты. Пробные версии отобразятся на вкладке **Пробные версии** в каталоге.
3. Выберите бесплатную пробную версию, которую вы хотите предложить, а затем нажмите **Отправить**. Срок действия всех пробных версий составляет 30 дней, в течение которых счет выставлен не будет. Также пробную версию можно преобразовать в платную подписку в любой момент пробного периода.

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. Перейдите на страницу подписки клиента и выберите бесплатную пробную версию.
2. Выберите **Преобразование пробной версии в платную подписку**.
3. Введите требуемое количество лицензий и периодичность выставления счетов, а затем нажмите **Применить**.
4. Выставление счетов за платную подписку начинается с даты преобразования и подписка автоматически продляется через 12 месяцев с даты преобразования. 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [Преобразование пробной подписки в платную](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Получение списка предложений для преобразования пробных версий](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. Рекомендуется регулярно отслеживать эти даты, чтобы выполнить соответствующие действия, когда клиентам понадобится принять решение.

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>Выставление счетов

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. Если бесплатная пробная версия была преобразована в платное предложение с ежегодным выставлением счетов, подписка будет продлена через 12 месяцев с даты преобразования. Если бесплатная пробная версия была преобразована в платное предложение с ежемесячным выставлением счетов, подписка будет продлена через 12 месяцев с даты выставления счетов, следующей за датой преобразования.

### <a name="invoices"></a>Счета

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>Программа поощрения

Free trials do not have an impact on incentives.

## <a name="support"></a>Поддержка

For support on free trials, submit a service request through Partner Center.
