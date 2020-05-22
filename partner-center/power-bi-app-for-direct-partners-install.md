---
title: Установка аналитики центра партнеров для Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Выполните действия, описанные в этой статье, чтобы установить и просмотреть приложение аналитики центра партнеров для Power BI (для прямых партнеров в CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e8a8558bad11f641737507f4d76405e9825df516
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795875"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Установить и ознакомиться с приложением "Аналитика Центра партнеров для Microsoft Power BI"

**Относится к**

- Центр партнеров

**Соответствующие роли**
-   Глобальный администратор
-   администратор пользователей.
-   Агент по продажам
-   Агент по администрированию

## <a name="before-you-begin"></a>Подготовка к работе

Выберите приложение, которое наиболее релевантно для вашего бизнеса, в следующем списке доступных Power BI приложений:
- [Прямой партнер](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [Косвенный партнер](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [Непрямой Торговый посредник](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

Перед установкой предварительной версии приложения "Аналитика Центра партнеров" убедитесь, что соблюдены следующие требования.

- Выберите нужное приложение Power BI для вашего бизнеса.

- У вас есть активная подписка на Microsoft Power BI Professional или Microsoft Power BI Premium.

- Вы можете войти в Power BI.

- Вы можете войти в систему в качестве глобального администратора, агента администратора или администратора выставления счетов в [клиенте Azure Active Directory (Azure AD) вашей компании](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Установка приложения

1. Начните [процесс установки](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).

2. В разделе **Уже есть учетная запись?** выберите **Вход**. 

3. На следующей странице введите имя пользователя и пароль Power BI, а затем выберите **Вход**. 

4. На всплывающем окне **Подключение к аналитике центра партнеров** убедитесь, что для **метода проверки подлинности** задано значение **oAuth2** , или выберите **oAuth2** из списка, если это не так. 

> [!NOTE]  
>  Для отображение окна может потребоваться несколько минут.

5. На странице **соединителя аналитики центра партнеров** выполните вход с помощью глобального администратора, агента администратора или учетных данных администратора выставления счетов для клиента Azure AD Организации, а затем выберите **Вход**.
 
6. Когда появится запрос доступа, нажмите кнопку **Принять**. 

После подключения служба аналитики Центра партнеров к Power BI начнется загрузка данных. Это может занять до 10 минут в зависимости от объема данных. 

После завершения загрузки данных вы можете приступить к использованию информационной панели и отчетов приложения "Аналитика Центра партнеров" в Power BI.

## <a name="next-steps"></a>Дальнейшие действия

[Просматривайте бизнес-данные с помощью приложения "Аналитика Центра партнеров для Microsoft Power BI"](power-bi-app-for-direct-partners-use.md)
