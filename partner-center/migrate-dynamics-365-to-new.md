---
title: Перенос Dynamics 365 Business Edition предоставляет до более новых версий | Центр партнеров
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 Business Edition подписки больше не могут быть обновлены.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 предлагает, обновить предложения, новые номера SKU Dynamics 365
ms.openlocfilehash: ca1823c4055e2d89edc5c49e900a1c255a94f59a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584627"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Перенос предложений с выпуском Dynamics 365 Business в более новые версии 

**Применяется к**

- Центр партнеров

Действующие клиенты 1 января 2019 г., с подписками Dynamics 365 Business Edition больше не можете продлить в эти устаревшие предложения; существующие подписки не будут автоматически продлеваться истечении их срока действия. На странице сведений о подписке состояние подписки изменится на «Истекает [дата]» из «Автоматически обновляет [дата]».

Чтобы обеспечить непрерывность для клиентов, должно перейти с истекающим сроком действия подписки на поддерживаемый параметр, перечисленных ниже. Мы рекомендуем переводить клиентов на новые подписки до ежегодной даты завершения подписки, чтобы не допускать перерывов в предоставлении службы клиентам.

Если вы используете API (CREST или центра партнеров), можно найти подписки, срок действия которых истекает, оценивая дату окончания подписки, а также автоматического обновления = False свойство. Рассматриваемый подписки будет указано значение auto продлить = False на 1 января 2019 г. Перевести клиентов на новый план можно в любое время. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Бизнес-версии Dynamics 365 выводится из эксплуатации

- Dynamics 365 для Finance and Operations, выпуск для бизнеса
- Dynamics 365 for Team Members Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - новых предложениях Dynamics 365 Business Edition

С помощью новых предложениях Dynamics Business Central клиентам можно подключиться их Финансы, продажи, службы и операции для оптимизации бизнес-процессов, повысить качество взаимодействия с клиентами и принимать более взвешенные решения. Dynamics 365 Business Central облачных и доступны только участники программы поставщика облачных решений (CSP).
Dynamics 365, зарегистрированные для получения цены со скидкой перехода на новый Business Central пользователям Business Edition предоставляет до 30 июня 2020 г.

## <a name="transition-customers-to-new-product-plans"></a>Перевод клиентов на новые планы продуктов

 Переход клиентов с удалено номера SKU на более новые необходимо выполнить следующие действия в указанном порядке:

- Приобретение новой подписки
- Переназначение текущих пользовательских лицензий
- Отмена старой подписки

## <a name="purchase-the-new-plan-for-your-customer"></a>Приобретите новый план для вашего клиента

1. Выберите **клиентов** (левая панель), а затем выберите клиента, которую требуется переместить в новую подписку.
2. Выберите **добавить подписку**.
3. Выберите из каталога подписку, которую требуется приобрести (в данном случае — одно из указанных выше предложений), введите количество лицензий и выберите **Отправить**. 

Теперь у вашего клиента будут старой подписки и новое. Следующий шаг — переназначать лицензии для пользователей клиента.

1. Выберите **клиентов** (левая панель), а затем выберите клиента вы переходите.
2. Выберите **Пользователи и лицензии**.
3. Чтобы переназначить лицензию пользователю, выберите пользователя, а затем выберите **Управление лицензиями**. 
4. На **Управление лицензиями** странице снимите Dynamics 365 for Sales / плана Customer Engagement из Basic (Полное предложение), лицензии "флажок" и выберите новый план службы для клиента на перенос подписки. 
5. Выберите **Отправить**. Это будет сделать для каждого пользователя, которому требуется новая лицензия. 

После перемещения лицензий в новую подписку можно отменить старой подписки. 

1. Выберите **клиентов** (левая панель), а затем выберите клиента вы переходите.
2. На странице сведений подписки присвоено старой подписки **Suspended** и выберите **отправить**.

Приостановлена старой подписки, а новая подписка активна. Приостановленная подписка будет автоматически отозвана через 120 дней. Клиент будет взиматься без дополнительных затрат для старой подписки.