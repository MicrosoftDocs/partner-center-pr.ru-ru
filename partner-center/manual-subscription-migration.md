---
title: Перенос данных о Dynamics 365 и план взаимодействия клиента с Basic (полное предложений) до более новых версий | Центр партнеров
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement план из подписок Basic (полное предлагает) могут не обновляться.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 предлагает, обновить предложения, новые номера SKU Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134404"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Перенос Dynamics 365 и плана Customer Engagement с "Базового" уровня (соответствующие предложения) в более новые версии

**Применяется к**

-  Центр партнеров

Действующие клиенты 1 января 2019 г., с помощью Dynamics 365 for Sales / Customer Engagement план из подписок Basic (полное предлагает) больше не можете продлить эти устаревшие предложения; существующие подписки не будут автоматически продлеваться истечении их срока действия. На странице сведений о подписке состояние подписки изменится на «Истекает [дата]» из «Автоматически обновляет [дата]». 


Чтобы обеспечить непрерывность для клиентов, должно перейти с истекающим сроком действия подписки на поддерживаемый параметр, перечисленных ниже. Мы рекомендуем переводить клиентов на новые подписки до ежегодной даты завершения подписки, чтобы не допускать перерывов в предоставлении службы клиентам.

Если вы используете API (CREST или центра партнеров), можно найти подписки, срок действия которых истекает, оценивая дату окончания подписки, а также автоматического обновления = False свойство. Рассматриваемый подписки будет указано значение auto продлить = False на 1 января 2019 г. Перевести клиентов на новый план можно в любое время. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 предлагает выводится из эксплуатации

- Dynamics 365 для Sales Enterprise Edition CRMOL Basic (Полное предложение)
- Dynamics 365 для Basic CRMOL Sales Enterprise Edition (Полное предложение) для преподавателей
- Dynamics 365 для Basic CRMOL Sales Enterprise Edition (Полное предложение) для учащихся
- Dynamics 365 для Sales Enterprise Edition (для государственных организаций) CRMOL Basic (Полное предложение)
- Dynamics 365 for Sales Enterprise Edition с SA для Basic CRM (Полное предложение)
- Dynamics 365 for Sales Enterprise Edition с SA для Basic CRM (Полное предложение) для преподавателей
- Dynamics 365 for Sales Enterprise Edition с SA для Basic CRM (Полное предложение) для учащихся
- Dynamics 365 for Sales Enterprise Edition (для государственных организаций) из SA для Basic CRM (Полное предложение)
- Dynamics 365 для надстройки Sales Enterprise Edition для Basic CRM (Полное предложение)
- Dynamics 365 для надстройки Sales Enterprise Edition для Basic CRM (Полное предложение) для преподавателей
- Dynamics 365 для надстройки Sales Enterprise Edition для Basic CRM (Полное предложение) для учащихся
- Dynamics 365 для Sales Enterprise Edition (для государственных организаций) надстройками для Basic CRM (Полное предложение)
- Dynamics 365 Customer Engagement плана Enterprise Edition Basic CRMOL (Полное предложение)
- Dynamics 365 Customer Engagement плана Enterprise Edition (для государственных организаций) Basic CRMOL (Полное предложение)
- Dynamics 365 Customer Engagement плана Enterprise Edition CRMOL Basic (Полное предложение) для учащихся
- Dynamics 365 Customer Engagement плана Enterprise Edition CRMOL Basic (Полное предложение) для преподавателей
- Dynamics 365 Customer Engagement Plan Enterprise Edition с SA для Basic CRM (Полное предложение)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (для государственных организаций) из SA для Basic CRM (Полное предложение)
- Dynamics 365 Customer Engagement Plan Enterprise Edition с SA для Basic CRM (Полное предложение) для учащихся
- Dynamics 365 Customer Engagement Plan Enterprise Edition с SA для Basic CRM (Полное предложение) для преподавателей
- Dynamics 365 Customer Engagement плана Enterprise Edition надстройку для Basic CRM (Полное предложение)
- Dynamics 365 Customer Engagement Enterprise Edition (для государственных организаций) надстройки плана для Basic CRM (Полное предложение)
- Dynamics 365 Customer Engagement плана Enterprise Edition надстройку для Basic CRM (Полное предложение) для учащихся
- Dynamics 365 Customer Engagement плана Enterprise Edition надстройку для Basic CRM (Полное предложение) для преподавателей



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / Customer Engagement плана Basic (полное предлагает) замены планы

**Устаревшие предложения**   

- Dynamics 365 for Sales из CRM Basic или CRMOL Basic (Полное предложение)
- Плана Dynamics 365 Customer Engagement, из CRM Basic или CRMOL Basic (Полное предложение)

**Параметры замены**
- Dynamics 365 for Sales Professional (НОВОЕ)
- Dynamics 365 for Sales Professional (НОВОЕ)
- Dynamics 365 for Customer Service
- Плана Dynamics 365 Customer Engagement или
- Члены команды Dynamics 365



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
 

 



