---
title: Влияние налоговых политик на Выдача для Azure Marketplace
description: Узнайте, как налоговые политики влияют на выплата в Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 3630824c839ccd9f54f3e8e5199a573b5824bb91
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2021
ms.locfileid: "101758498"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Влияние налоговых политик на Выдача для Azure Marketplace

**Соответствующие роли**
-    Глобальный администратор
-    администратор пользователей.
-    Агент по администрированию

## <a name="introduction"></a>Введение

В коммерческом магазине Майкрософт есть глобальный доступ. Транзакции происходят по границам, и в зависимости от того, где находятся независимые поставщики программного обеспечения и клиента, налоговые последствия могут различаться. Microsoft AppSource и Azure Marketplace используют сведения о профиле налогов центра партнеров для определения страны ISV. Чтобы определить страну клиента, следует либо использовать сведения о выставлении счетов клиента, либо, если клиент входит в ЕС, мы используем два разных фрагмента информации.

Чтобы лучше разобраться в следующих сценариях, см. таблицу [сведения о налогах](tax-details-marketplace.md) , в которой показано, собирает ли корпорация Майкрософт налоги от имени издателя или если ответственность принадлежит к издателю.

> [!NOTE]
> Все примеры значений продаж и налоговых процентов в этом разделе предназначены только для наглядности, а не для точных иллюстраций.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Издатель взаимодействует в стране налога, управляемой корпорацией Майкрософт

**Сценарий A** — транзакции, которые выполняются между издателем и клиентом в [стране налога, управляемом корпорацией Майкрософт](tax-details-marketplace.md#microsoft-managed-countries). Эти транзакции будут иметь применимый налог, добавленный во время продажи, и корпорация Майкрософт отправит этот налог в соответствующую страну. Налоги не будут удержаны из расчета выплат, а Расчет выплат не является налоговым.

См. [сценарий г](#foreign-publisher-transacts-with-us-customer) для транзакций между издателем, ОТЛИЧНЫМ от США, и клиентом США.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты а.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Издатель взаимодействует в стране налога, управляемой корпорацией Майкрософт, где плата Marketplace является налогооблагаемой службой

**Сценарий б** . транзакции, выполняемые между издателем на основе США (как определено в сведениях о почтовом профиле центра партнеров) к клиенту в стране налога, управляемом корпорацией Майкрософт, в которой страна накладывает налог на плату Marketplace (налогооблагаемая служба). В этом сценарии налог на услугу оплаты магазина вычитается из выплаты издателя.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты б.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Издатель взаимодействует в стране налога, управляемой издателем

**Сценарий C** — транзакции, которые выполняются между издателем и клиентом в налоговой стране, управляемой издателем, которая не накладывает на клиентов подоходный налог. Клиенты платят без налогов на момент продажи, и это обязательства издателя по оплате всех применимых налогов.

Дополнительные сведения о ценах, относящихся к конкретной стране (например, для смещения предстоящего налогообложения), см. в статье [планы и цены на коммерческие предложения Marketplace](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Внешний издатель взаимодействует с клиентами США

**Сценарий г** . все иностранные издатели (как определено в сведениях о почтовом профиле центра партнеров) в странах без соглашения США (см. [сценарий E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) принятие продажи клиенту на основе США (как определено в адресе учетной записи клиента). Для государственных организаций США требуется, чтобы от имени издателя был удержан налог от корпорации Майкрософт. Налог, удержанный от выплаты к издателю, вычисляется на основе цены предложения.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты г.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Внешний издатель с договором взаимодействует с клиентом США

**Сценарий E** . все иностранные издатели (как определено в сведениях о почтовом профиле центра партнеров) в странах с договором США о продажах клиенту на основе США (как определено по адресу учетной записи клиента). Для государственных организаций США не требуется удержание налога от корпорации Майкрософт от имени издателя.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Иностранный издатель продает клиенту, зарегистрированному в ЕС, в стране, управляемой Майкрософт (за пределами Ирландии)

**Сценарий F** — все транзакции между внешними издателями и зарегистрированными в ЕС клиентами (за пределами Ирландии) в стране Microsoft-Managed. Клиент не оплачивает налоги по продажам.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Иностранный издатель продает клиенту, зарегистрированному в ЕС, в стране, управляемой корпорацией Майкрософт (в Ирландии).

**Сценарий G** — все транзакции между внешними издателями и зарегистрированными клиентами ЕС (в Ирландии) в Microsoft-Managed стране. Клиент оплачивает ирландский НДС, и корпорация Майкрософт оплачивает этот налог на правительство государственных организаций.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Показывает рабочий процесс для сценария процесса вывыплаты G.":::

## <a name="next-steps"></a>Дальнейшие действия

- [Издатель: вопросы и ответы](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)
- [Инструкции по созданию платежных и налоговых профилей](https://docs.microsoft.com/partner-center/set-up-your-payout-account?context=/azure/marketplace/context/context#create-a-payment-profile)