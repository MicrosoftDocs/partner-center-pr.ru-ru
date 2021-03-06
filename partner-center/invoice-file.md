---
title: Общие сведения о выставлении счетов в центре партнеров
ms.topic: article
ms.date: 05/18/2020
description: Изучите поля в файле счета для выставления счетов в центре партнеров. Включены поля и определения для всех полей счета и одноразовых полей оплаты.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146618"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Общие сведения о полях счетов в центре партнеров

**Соответствующие роли**: глобальный администратор | Администратор управления пользователями | Администратор выставления счетов | Агент службы технической поддержки

Для понимания полей в файлах счетов центра партнеров можно использовать следующие таблицы.

## <a name="invoice-file-fields"></a>Поля файла накладной

В файлах накладных отображаются следующие поля.

| Поле | Определение |
| ----- | ---------- |
| Федеральный идентификационный номер работодателя США | Идентификационный номер правительственного работодателя (ФЕИН). Это ваш США Федеральный идентификационный номер налогоплательщика. |
| Номер клиента | Ваш номер клиента. |
| Получатель счета | Адрес, на который мы отправляем счет-фактуру. Вы можете изменить название и адрес Организации в профиле выставления счетов центра партнеров. |
| Оплата на основе лицензии | Фиксированная ежемесячная или ежегодная плата за приобретенные лицензии на основе использования, выставленная до службы. Это число является суммой всех расходов в столбце **промежуточных итогов** (столбец **T**) в файле согласования на основе лицензий. |
| Оплата на основе использования | Использование Azure. Сюда входят новые службы или приложения, включенные и используемые в течение расчетного периода. Это число является суммой всех расходов в столбце **PretaxCharges** (столбец **Z**) в файле сверки с учетом использования. |
| Скидки | Скидка, получаемая клиентом от обычной цены подписки. Это число отображается как *фиксированный объем*, а не как цена за единицу или лицензию. |
| Благодарности | Кредиты или корректировки изменений, внесенные в подписки (например, увеличение или уменьшение лицензии). |
| Промежуточный итог | Итог до вычета налогов, а также исключающих налоги сборов и кредитов. |
| Налог | Общий налог за текущие расходы, как Итого в разделе **сведений** , начиная со страницы 2 в счете. Это число — сумма всех выплат в столбце **таксамаунт** (столбец **AA**) в файле сверки с учетом использования, а также **налоговый** столбец (столбец **U**) в файле согласования на основе лицензий. |
| Другие кредиты | Кредиты без учета налогов. |
| Текущие платежи | Сумма оплаты за расчетный период в валюте выставления счетов. За эти расходы взимается Дата оплаты. |
| Инструкции по оплате | Описание способа оплаты счета на основе вашего региона. *При создании платежа всегда обязательно включайте номер счета.* |
| Номер счета-фактуры | Номер вашего счета-фактуры. |
| Расчетный период | Месячный период, ведущий к дате выставления счета. Это период, в течение которого службы на основе использования потребляются, а службы на основе лицензий выверяются на наличие корректировок кредита или изменений в количестве лицензий. |
| Дата выставления счета | Дата выставления счетов или Дата юбилея, на каждый месяц создается счет. |
| Условия оплаты | Срок платежа. Для единовременных покупок срок оплаты всегда составляет 60 дней. |
| Дата выполнения платежа | Дата, на которую должна быть получена оплата. |
| Клиентский номер заказа на покупку | Номер заказа на покупку. |
| Обслуживание клиентов | Адрес веб-сайта, на который можно получить доступ к службе поддержки клиентов. |
| Получатель службы | Адрес, по которому используется служба. (Это юридический адрес компании, связанный с компанией заглянув.) |

## <a name="one-time-charges-fields"></a>Поля оплаты за одноразовую оплату

Следующие поля применяются только к **одноразовым платам** в центре партнеров:

| Поле | Определение |
| ----- | ---------- |
| Дата | Дата покупки. |
| Описание: | Название продукта. |
| Количество | Количество приобретенных продуктов (например, резервирования). |
| Цена за единицу | Цена за продукт (например, резервирование). |
| Скидки | Все применимые скидки. |
| Сумма без налога | Подытог покупок перед налогами. |
| Налог с продаж | Сумма налога. |
| Итог | Общая сумма для оплаты. |
