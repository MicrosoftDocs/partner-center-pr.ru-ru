---
title: Поля для CSV-файла для импорта нескольких пользователей для учетной записи клиента
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Чтобы добавить нескольких пользователей в учетную запись клиента, создайте файл значений с разделителями-запятыми (CSV) с соответствующими полями.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150987"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Добавление нескольких пользователей в учетную запись клиента путем создания CSV-файла

**Соответствующие роли** — глобальный администратор.

Одновременное добавление нескольких пользователей в учетную запись клиента путем отправки файла данных в формате файла с разделителями-запятыми (CSV) в центр партнеров. Вы можете скачать образец файла данных из центра партнеров, а затем изменить его для использования или создать новый файл данных, используя модель данных, определенную ниже.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Требования к файлу данных

Чтобы добавить нескольких пользователей в учетную запись клиента с помощью процесса групповой отправки, необходимо выполнить следующие требования.

- у вас должны быть разрешения глобального администратора для учетной записи клиента;
- у каждого пользователя должен быть уникальный электронный адрес в почтовом домене пользователя;
- одновременно можно передавать до 100 записей. Если вам необходимо добавить более 100 пользователей, создайте и загрузите дополнительные файлы данных;
- все пользователи должны быть в одном географическом **регионе**;
- вводите только данные, описанные ниже. Лишние данные приведут к ошибке отправки.

Введите следующие данные в файле данных:

| **Имя столбца** | **Описание**  | **Ограничения**  |
|:-------- |:------  |:----- |
| Имя  | Имя пользователя (необязательное поле)  | Не более 50 знаков  |
| Фамилия  | Фамилия пользователя (обязательное поле)  | Не более 50 знаков  |
| Отображаемое имя    | Имя, отображаемое в центре партнеров (обязательное поле)                            | Не более 50 знаков                         |
| Email   | Рабочий адрес электронной почты пользователя в клиентской компании (обязательное поле)           | Каждый пользователь должен иметь уникальный адрес электронной почты. |
| Обновление состояния   | Используется для указания, успешно ли создана новая запись пользователя | \*\*Оставить пустым\*\*                        |

## <a name="next-steps"></a>Следующие шаги

- [Как добавить нескольких пользователей для клиента](adding-multiple-users-to-a-customer-account.md)