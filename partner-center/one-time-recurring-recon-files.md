---
title: One-time and recurring reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand one-time and recurring reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389682"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>One-time and recurring reconciliation files

Область применения

- Центр партнеров
- Центр партнеров для Microsoft Cloud for US Government

This topic explains how to read one-time and recurring reconciliation files in Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Fields in one-time and recurring reconciliation files

| Column | Описание |
| ------ | ----------- |
| PartnerId | Unique Azure Active Directory (Azure AD) tenant identifier for a specific billing entity, in GUID format. Not required for reconciliation. Одинаково во всех строках. |
| Customer Id | Unique Azure AD tenant identifier, in GUID format. Identifies the customer. |
| Customer Name (Имя клиента) | Customer's organization name, as reported in Partner Center. |
| CustomerDomainName | Customer's domain name. Это поле может быть пустым до второго цикла выставления счетов. *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* |
| Customer Country | Страна, в которой находится клиент. |
| Номер счета | Номер счета-фактуры, содержащего указанную транзакцию. |
| MpnId | MPN identifier of the CSP partner. |
| Reseller MpnId | MPN identifier of the reseller of record for the subscription. |
| Идентификатор заказа | Unique identifier for an order in the Microsoft commerce platform. Not used for reconciliation. |
| Дата заказа | Дата размещения заказа. |
| ProductID | The identifier for the product. |
| SkuId | The identifier for a particular SKU (stock-keeping unit). |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | Название для определенного номера SKU. |
| название продукта; | Название продукта. |
| PublisherName | The name of the product's publisher.
| PublisherID | Unique identifier for a particular publisher. |
| Subscription Description | Friendly name of a subscription. |
| Код подписки | Unique identifier for a subscription in the Microsoft commerce platform. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | Дата начала взимания оплаты. Временем всегда является начало дня, 0:00. |
| ChargeEndDate | День завершения взимания оплаты. Временем всегда является конец дня, 23:59. |
| Term and Billingcycle | The term length and billing cycle for the purchase (for example, *1 Year, Monthly*). |
| Тип оплаты | Тип оплаты или корректировки. |
| Цена за единицу | The unit price as published in the price list at the time of purchase. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Effective Unit Price | The unit price after adjustments have been made. |
| Количество | Number of units. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Unit type | The type of unit being purchased. |
| DiscountDetails | An explanation of any applicable discount. |
| Sub Total | Сумма до налога. Checks if your subtotal matches your expected total, in case of a discount. |
| Tax Total | Tax amount charge. Based on your market's tax rules and specific circumstances. |
| Total (Всего) | Цена после налогов. Проверьте, вычтены ли с вас налоги в накладной. |
| Валюта | Тип валюты. Каждый объект выставления счетов имеет только одну валюту. Make sure this matches your first invoice and check again after any major billing platform updates. |
| AlternateID | An alternative identifier to an **Order ID**. |
