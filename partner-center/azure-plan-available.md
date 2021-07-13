---
title: Доступные службы Azure в Azure CSP
description: В этой статье рассматриваются службы Azure, которые доступны и не доступны в программе поставщика облачных решений Azure (CSP).
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: da97dded531b6792a4468d9be9b63367f818b352
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149746"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Доступные службы Azure в рамках программы поставщиков облачных решений (CSP) Azure

**Соответствующие роли**: агент по администрированию | администратор выставления счетов | глобальный администратор | агент службы технической поддержки | агент по продажам | администратор управления пользователями

## <a name="available-azure-services-in-azure-csp"></a>Доступные службы Azure в Azure CSP

В этой статье указаны службы Azure, которые доступны и недоступны в программе Azure "Поставщик облачных решений" (CSP). Здесь также объясняются моменты, связанные с доступностью службы в таких национальных облаках, как [Microsoft Azure для Германии](https://azure.microsoft.com/overview/clouds/germany/) и [Microsoft Azure для государственных организаций](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
> [Azure для Китая](https://www.azure.cn/) не поддерживается в программе Azure CSP.

## <a name="global-cloud"></a>Глобальное облако

Все службы на основе модели Azure Resource Manager доступны в программе CSP.  Службы не на основе модели Azure Resource Manager недоступны в программе CSP.  

## <a name="csp-specific-service-configurations"></a>Конфигурации служб, зависящих от CSP

Специальные конфигурации в CSP требуются для следующих служб:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Доменные службы Azure Active Directory](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Хранилище ключей](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Аналитика временных рядов Azure](https://azure.microsoft.com/services/time-series-insights/) — только пользователи из арендатора клиента могут получать доступ к данным в среде Аналитики временных рядов. Партнеры могут управлять средой Аналитики временных рядов клиента по умолчанию, но если им требуется доступ к данным в ней, они должны быть добавлены в арендатор клиента.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Теперь вы можете приобретать перечисленные ниже элементы в Visual Studio Marketplace, за исключением сторонних расширений.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Подписки Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Обучение в Xamarin University](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Чтобы вам было проще начать работу, мы предлагаем видео и документацию по [настройке, приобретению и администрированию Azure DevOps](/vsts/billing/csp/set-up-csp-customer) в CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Элементы Azure Marketplace в Azure CSP

Не все элементы Azure Marketplace сейчас доступны в подписках Azure CSP.

- Службы Azure на основе Microsoft: эти службы доступны. Ознакомьтесь с предыдущей таблицей и комментариями.

- Элементы с поддержкой BYOL: эти элементы доступны. Полный список элементов Azure Marketplace с поддержкой BYOL см. на [этой странице](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Сторонние элементы Azure Marketplace с оплатой по мере использования: эти элементы доступны, если поставщик опубликован в канале CSP. См. сведения о [продаже подписок на продукты Azure Marketplace](csp-commercial-marketplace-overview.md).

- Citrix XenApp Essentials: партнеры могут приобрести XenApp Essentials для клиентов в CSP. Сведения о распространении XenApp Essentials через канал поставщика облачных решений (Майкрософт) см. в [блоге Citrix](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

## <a name="national-clouds"></a>Национальные облака

В следующей таблице представлен регулярно обновляемый список доступных продуктов, служб и компонентов Azure для CSP в национальных облаках.

| Продукт, служба или компонент Azure | US Government | Германия |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  Виртуальные машины  |  X  |  X  |
|  Облачные службы  |    |    |
|  Масштабируемые наборы виртуальных машин  |  X  |  X  |
|  Функции  |    |    |
|  Служба контейнеров Azure  |    |    |
|  **Сетевое взаимодействие**  |    |    |
|  Azure DNS  |    |    |
|  Сеть доставки содержимого  |    |    |
|  Диспетчер трафика  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Виртуальная сеть  |  X  |  X  |
|  Подсистема балансировки нагрузки  |  X  |  X  |
|  VPN-шлюз  |  X  |  X  |
|  Шлюз приложений  |  X  |  X  |
|  Наблюдатель за сетями  |  X  |  X  |
|  **Хранилище**  |    |    |
|  Хранение  |  X  |  X  |
|  Резервное копирование  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Управляемые диски  |  X  |  X  |
|  **Интернет и мобильные устройства**  |    |    |
|  Служба приложений  |  X  |  X  |
|  Служба приложений в Linux  |    |  X  |
|  Управление API  |  X  |    |
|  Сеть доставки содержимого  |    |    |
|  Службы мультимедиа  |  X  |  X  |
|  Центры уведомлений  |  X  |  X  |
|  Поиск Azure  |    |    |
|  Компонент Logic Apps Службы приложений Azure  |    |    |
|  **Контейнеры**  |    |    |
|  Служба приложений  |  X  |  X  |
|  Служба приложений в Linux  |    |  X  |
|  Batch  |  X  |  X  |
|  Реестр контейнеров  |    |    |
|  Экземпляры контейнеров  |    |    |
|  Service Fabric  |  X  |  X  |
|  Служба контейнеров  |    |    |
|  **Базы данных**  |    |    |
|  База данных SQL  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  Хранилище данных SQL  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  База данных Azure для MySQL  |    |    |
|  База данных Azure для PostgreSQL  |    |    |
|  **Данные и аналитика**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Фабрика данных  |    |    |
|  Log Analytics  |  X  |    |
|  Каталог данных  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **Искусственный интеллект и Cognitive Services**  |    |    |
|  Машинное обучение  |    |  X  |
|  Служба Azure Bot  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch AI  |    |    |
|  **"Интернет вещей"**  |    |    |
|  Центр Интернета вещей  |  X  |  X  |
|  IoT Central  |    |    |
|  Машинное обучение  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Центры событий  |  X  |  X  |
|  Location Based Services  |    |    |
|  Центры уведомлений  |  X  |  X  |
|  Аналитика временных рядов  |    |    |
|  **Корпоративная интеграция**  |    |    |
|  StorSimple  |  X  |    |
|  Управление API  |    |    |
|  Сетка событий  |    |    |
|  Фабрика данных  |    |    |
|  Служебная шина  |  X  |  X  |
|  Каталог данных  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Компонент Logic Apps Службы приложений Azure  |    |    |
|  **Безопасность и идентификация**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Многофакторная идентификация  |    |    |
|  Доменные службы Azure Active Directory  |    |    |
|  Key Vault  |  X  |  X  |
|  Центр безопасности  |  X  |  X  |
|  **Средства разработчика**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Центр приложений Visual Studio  |    |    |
|  Xamarin University  |    |    |
|  **Мониторинг и управление**  |    |    |
|  Advisor  |    |    |
|  Резервное копирование  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Планировщик  |  X  |  X  |
|  Автоматизация  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Приложения, управляемые Azure  |    |    |
|  Миграция Azure  |    |    |
|  Группы управления  |    |  

## <a name="next-steps"></a>Дальнейшие действия

- [Узнайте](/azure/cloud-solution-provider/overview/partner-center-overview) о доступных возможностях Azure в Центре партнеров.

- [Создайте](/azure/cloud-solution-provider/customer-management/create-new-customer) первого клиента в Azure CSP и разверните службы Azure.
