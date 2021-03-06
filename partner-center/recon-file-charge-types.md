---
title: Типы расходов в файле выверки
ms.topic: article
ms.date: 06/05/2020
description: Узнайте о типах начислений (например, на основе лицензий, на основе использования и одноразовых), кредиты и скидках в файлах сверки центра партнеров.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989780"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Изучите различные типы оплаты в файлах сверки центра партнеров

**Область применения**: Центр партнеров | Центр партнеров для Microsoft Cloud for US Government

**Соответствующие роли**: агент по администрированию | глобальный администратор

В этой статье описываются сопоставления между разделом счета и связанными типами оплаты, которые могут находиться в файле сверки. В счете представлена сводка по расходам. Файл сверки содержит подробную разбивку транзакций по строкам, включая типы начислений. Дополнительные сведения о файлах сверки см. [в разделе Использование файлов сверки](use-the-reconciliation-files.md).

[Файлы согласованности на основе использования](usage-based-recon-files.md) и [файлы сверки на основе лицензий](license-based-recon-files.md) содержат только связанные с использованием транзакции и расходы (потребленные единицы и связанные с ней расходы).

> [!NOTE]
> Одноразовые кредиты, скидки или возмещения, которые отображаются в счете в качестве **корректировок** , не отображаются в файле сверки.

## <a name="map-charge-types-to-invoice-charges"></a>Сопоставьте типы расходов с накладными расходами

Для сбора сумм оплаты между счетом и файлом сверки используйте параметры фильтра в Microsoft Excel. Фильтрация по типам оплаты в файле сверки для сопоставления расходов по счету с набором разбивки на счет для файла сверки.

## <a name="license-based-charges"></a>Оплата на основе лицензии

Чтобы связать эти расходы на основе лицензий с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.

| Описание платы (столбец Чаржетипе в файле сверки) | Объяснение затрат |
| ------------------------------------------------------------- | ------------------ |
| Сбор за активацию | Сумма, выплаченная клиенту при использовании подписки после покупки. |
| Сбор за отмену | Распределенные расходы, которые были возвращены клиенту при изменении связанных с ним лицензий. |
| Отмена пропорционального распределения экземпляра | Распределенные платежи отменяются, когда у клиента с месячной подпиской есть приостановленная подписка, а связанные с ней лицензии изменяются в тот же месяц. |
| Оплата цикла | Периодическая оплата за подписку. |
| Пропорциональное распределение экземпляра цикла | При изменении связанных лицензий взимается плата за распределенные платежи от клиента. |
| Пропорциональные сборы при отмене | Пропорциональное возмещение за неиспользуемую часть службы при отмене. |
| Пропорциональное количество выплат при преобразовании из текущего предложения | Плата распределяется пропорционально после преобразования текущей ежемесячной подписки в годовую. |
| Пропорциональное количество выплат при преобразовании в новое предложение | Плата распределяется пропорционально после преобразования месячной подписки в новую годовую подписку. |
| Пропорциональные сборы при покупке | Тип оплаты для подписки при использовании ежемесячного или годового счета. |
| Пропорциональные сборы при обновлении | Пропорциональное вознаграждение при обновлении подписки. |
| Плата за обновление | Платеж за обновление подписки |
| Пропорциональные сборы при активации | Пропорциональное количество выплат с активации до окончания расчетного периода. |

## <a name="one-time-charges"></a>Оплата за один раз

Чтобы связать эти одноразовые платежи с накладной, Вычислите сумму столбца **Amount** из файла, основанного на лицензии.

| Описание платы (столбец Чаржетипе в файле сверки) | Объяснение затрат |
| ------------------------------------------------------------- | ------------------ |
| new | Используется при создании новой покупки. |
| Продление | Используется при продлении подписки после окончания срока. |
| addQuantity | Используется как для возврата первоначальной покупки, так и для нового количества после увеличения. |
| removeQuantity | Используется как для возврата первоначальной покупки, так и для нового количества после уменьшения. |
| канцелиммедиате | Используется при отмене подписки. |
| convert | Используется при обновлении лицензии. |
| кустомеркредит | Используется при указании кредитов (например, Azure, SLA и т. д.) для транзакции. |

## <a name="usage-charges"></a>Плата за использование

Чтобы сопоставлять расходы на использование с накладной, вычислите столбец **PretaxCharges** из файла на основе использования.

| Описание платы (столбец Чаржетипе в файле сверки) | Объяснение затрат |
| ------------------------------------------------------------- | ------------------ |
| Плата за использование Assess при отмене | Плата за пользование при аннулировании за неоплачиваемое использование в течение текущего платежного периода. |
| Плата за использование Assess для текущего цикла | Плата за пользование для текущего периода выставления счетов. |

### <a name="credits"></a>Благодарности

Чтобы связать эти кредиты с накладной:

- Вычислите сумму **тоталфоркустомер** из файла, основанного на лицензии.
- Вычислите сумму столбца **PostTaxTotal** из файла на основе использования.

| Описание платы (столбец Чаржетипе в файле сверки) | Объяснение затрат |
| ------------------------------------------------------------- | ------------------ |
| Смещение позиции строки | Частичное или полное возмещение за позицию в строке (с налогом). |

### <a name="usage-based-discounts"></a>Скидки на основе использования

Чтобы связать скидки на основе использования с накладной, суммируйте столбец **PretaxCharges** из файла, основанного на использовании.

| Описание платы (столбец Чаржетипе в файле сверки) | Объяснение затрат |
| ------------------------------------------------------------- | ------------------ |
| Скидка при активации | Скидка, применяемая при активации подписки. |
| Скидка на цикл | Скидка, действующая на периодические платежи. |
| Скидка при возобновлении | Скидка, применяемая при продлении подписки. |
| Скидка при отмене | Плата, которая взимается при отмене скидок. |

### <a name="license-based-discounts"></a>Скидки на основе лицензии

Чтобы сопоставлять скидки на основе лицензий с накладной, суммируйте столбец **тоталосердискаунт** из файла, основанного на лицензии.

*Скидки на основе лицензий могут применяться к нескольким типам оплаты.*
