---
title: Поиск количества рабочих столов и уровня сбора
ms.topic: how-to
ms.date: 02/18/2021
description: Узнайте, как использовать платформу поощрения каналов (микросхемы) для поиска количества настольных компьютеров и сведений об уровне сбора для соглашения.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276948"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Определение количества рабочих столов и ставки для соглашения

**Соответствующие роли**: основной контакт или администратор программы

Вы можете войти в [Explore.MS](https://www.explore.ms/) , чтобы ознакомиться с соглашением, или скачать файл, предоставляющий сведения о соглашении для количества настольных компьютеров и уровня сбора.

## <a name="to-locate-the-information"></a>Определение местонахождения информации

### <a name="method-1--explorems"></a>Метод 1 — Explore.ms

1. Откройте [Explore.MS](https://www.explore.ms/) в Internet Explorer. 

>[!Note]
>Эта функция не может быть выполнена в Google Chrome или Microsoft ребра.

2. Войдите в систему, используя рабочую или учебную учетную запись или Live ID.  

3. В поле **отчеты** выберите **соглашения**.

4. На полученной странице введите номер соглашения в поле **поиска** , а затем выберите **выбрать/упорядочить столбцы**.

5. Во всплывающем окне в списке Доступные столбцы выберите значение **соглашение настольных компьютеров** и нажмите кнопку со стрелкой вправо, чтобы добавить столбец. Щелкните **ОК**.

6. Выберите **Поиск.**

7. На открывшемся экране прокрутите результаты, чтобы найти столбец **соглашения о количестве настольных компьютеров** . 

8. Используйте число настольных компьютеров, чтобы определить уровень сбора на основе таблицы тарифов ниже.  

| Уровень сбора | Число рабочих столов |
| ------ | :-----------: |
|  A | 0 – 2 399    |
|  B | 2 400 – 5 999    |
|  C | 6 000 – 14 999    |
|  D | 15000 +   |

>[!NOTE]
>Корпоративные уровни поощрения основаны на количестве настольных компьютеров или пользователей (в зависимости от того, какое значение выше) в коммерческих и общественных регистрациях (PS). Для регистраций без физического сопоставленного рабочего стола или числа пользователей корпорация Майкрософт применяет инвентаризацию настольных компьютеров на основе числа настольных компьютеров или числа пользователей соответствующих EA. <br><br>Если сопутствующий атрибут EA отсутствует, то уровень сбора зависит от уровня цен на регистрацию. Ценовую категорию сделки также можно просмотреть на [www.Explore.MS](https://www.explore.ms/). <br><br>При наличии нескольких уровней и (или) цен для существующих EA/EAS Корпорация Майкрософт оплачивает стимул на наивысшей назначенной цене или на уровне пула, при этом уровень A является самым низким, а уровень D — самым высоким.

#### <a name="pool-and-pricing-levels"></a>Уровни пула и ценообразования

После поиска номера соглашения в explore.ms с помощью описанных выше действий выберите номер соглашения. Откроется страница сведений о соглашении, в которой будут отображаться сводка и **предложения** **соглашения** . В разделе предложения содержатся ценовые уровни.

## <a name="method-2---chip"></a>Метод 2. микросхема

1. Войдите в микросхему и выберите LSP стимул.

2. На странице **Сводка платежного платежа** выберите отчетный месяц, который требуется просмотреть, а затем в раскрывающемся списке в разделе **Экспорт в Excel** выберите **сведения о вычислении** .

:::image type="content" source="images/chip/chiplocate.png" alt-text="Находите сведения о программе.":::

3. Начнется экспорт, и вы сможете открыть файл или сохранить или сохранить как в место назначения.

4. Когда отчет открыт, перейдите на вкладку **детаилрепорт-Flatfile** в левом нижнем углу экрана:

:::image type="content" source="images/chip/flatfile.png" alt-text="Загрузка неструктурированного файла.":::

Теперь можно выполнить поиск номера соглашения, которое вы ищете в столбце J. Кроме того, вы найдете назначенное число настольных компьютеров в столбце R с меткой Agreement_DesktopCount. Вы также можете подтвердить уровень сбора для этого соглашения в столбце "AI" с меткой "уровень".

## <a name="next-steps"></a>Дальнейшие действия

- [Устранение проблем с доступом к микросхемам](chip-access-trouble.md)
