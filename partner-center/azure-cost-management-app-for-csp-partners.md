---
title: Azure Cost Management от Cloudyn для партнеров CSP | Центр партнеров
ms.topic: article
ms.date: 10/29/2018
description: Для использования Azure Cost Management от Cloudyn требуется предоставленный доступ к API Центра партнеров.
author: Janet
ms.author: janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 32112dd8ba23d371eda554d86cf166562779a1d1
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796097"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Приложение Azure Cost Management для партнеров Azure CSP  

**Область применения**

-  Центр партнеров

[Дополнительная информация об Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Перед началом работы
До начала использования Azure Cost Management убедитесь, что соблюдаются следующие требования:

- Вы являетесь партнером и участвуете в программе для поставщиков облачных решений (CSP).
- Вы можете создать веб-приложение на основе API Центра партнеров.

## <a name="overview"></a>Обзор

Azure Cost Management от Cloudyn— это веб-приложение, позволяющее отслеживать и контролировать объем и стоимость использования Azure вашими клиентами. Приложение доступно через API Центра партнеров.

## <a name="register-your-web-app-in-the-partner-center"></a>Регистрация своего веб-приложения в Центре партнеров
При регистрации веб-приложения Azure Active Directory в Центре партнеров вы предоставляете доступ к API Центра партнеров. 
1.  Войдите в [Центр партнеров](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) с помощью [учетной записи глобального администратора или агента администратора](create-user-accounts-and-set-permissions.md).
2.  В **Центре партнеров**, выберите **Параметры учетной записи** &gt; **[Управление приложениями](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  В разделе **Веб-приложение** щелкните **Добавить новое веб-приложение**.
<br> **Примечание**. Если ранее вы уже создали веб-приложение, шаг 3 можно пропустить.
4.  Копируйте и сохраните GUID **ИД коммерции** и GUID **ИД приложения** вашего веб-приложения. Для использования бесплатной пробной версии приложения Azure Cost Management на 30 дней потребуются оба идентификатора.

## <a name="add-a-secret-key-to-your-app"></a>Добавление секретного ключа в приложение
1.  В раскрывающемся меню рядом с кнопкой **Добавить ключ** выберите период: 1 или 2 года.
2.  Нажмите кнопку **Добавить ключ**. 
3.  Копируйте и сохраните значение секретного ключа. Это необходимо для получения бесплатной пробной версии на 30 дней.<br>
> [!NOTE]  
> Секретные ключи приложения напоминают пароли с более длительным сроком действия. Сохраните значение ключа в безопасном расположении для будущего использования.

## <a name="next-steps"></a>Дальнейшие действия
Запустите [бесплатную пробную версию на 30 дней](https://go.microsoft.com/fwlink/?linkid=857895).
Для запуска пробной версии потребуются следующие сведения:
- Учетные данные для входа в Центр партнеров
- GUID "ИД коммерции"
- GUID "ИД приложения"
- Значение секретного ключа приложения
