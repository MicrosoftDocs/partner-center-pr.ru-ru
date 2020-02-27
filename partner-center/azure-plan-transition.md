---
title: Перевод клиентов на план Azure | Центр партнеров
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как перевести своих клиентов на план Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567240"
---
# <a name="transition-your-customers-to-azure-plan"></a>Перевод клиентов на план Azure

**Соответствующие роли**

- Агент по администрированию
- Администратор выставления счетов
- Глобальный администратор
- Агент службы технической поддержки
- Агент по продажам
- Администратор управления пользователями

Косвенные поставщики и партнеры с правом на прямое выставление счетов могут перейти на новую коммерческую модель, доступную в программе для поставщиков облачных решений (CSP) от Майкрософт для Azure. (Косвенные торговые посредники должны обращаться к своим косвенным поставщикам.) Клиентам будет проще покупать облачные службы у партнеров, торговых посредников Майкрософт или непосредственно в Интернете.

Возможность перехода предназначена только для клиентов, которые переходят на новую коммерческую модель для Azure и подписали клиентский договор с Майкрософт, а не для других предложений в CSP, таких как Office 365 или Dynamics 365.

## <a name="available-azure-services-in-azure-csp"></a>Доступные службы Azure в Azure CSP

В этом разделе описаны службы Azure, которые доступны и недоступны в программе поставщиков облачных решений Azure (CSP). Здесь также объясняются моменты, связанные с доступностью службы в таких национальных облаках, как [Microsoft Azure для Германии](https://azure.microsoft.com/overview/clouds/germany/) и [Microsoft Azure для государственных организаций](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
>[Azure для Китая]( https://www.azure.cn/) не поддерживается в программе Azure CSP.

### <a name="global-cloud"></a>Глобальное облако 

Все службы на основе модели Azure Resource Manager доступны в программе CSP.  Службы не на основе модели Azure Resource Manager недоступны в программе CSP.  

### <a name="csp-specific-service-configurations"></a>Конфигурации служб, зависящих от CSP

Специальные конфигурации в CSP требуются для следующих служб:

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Доменные службы Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Хранилище ключей](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Аналитика временных рядов Azure](https://azure.microsoft.com/services/time-series-insights/) — только пользователи из арендатора клиента могут получать доступ к данным в среде Аналитики временных рядов. Партнеры могут управлять средой Аналитики временных рядов клиента по умолчанию, но если им требуется доступ к данным в ней, они должны быть добавлены в арендатор клиента. 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Теперь вы можете приобретать перечисленные ниже элементы в Visual Studio Marketplace, за исключением сторонних расширений.

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Подписки Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Обучение в Xamarin University](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Чтобы вам было проще начать работу, мы предлагаем видео и документацию по [настройке, приобретению и администрированию Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) в CSP.

### <a name="azure-marketplace-items-in-azure-csp"></a>Элементы Azure Marketplace в Azure CSP

Не все элементы Azure Marketplace сейчас доступны в подписках Azure CSP.

- Службы Azure на основе Microsoft: эти службы доступны. Ознакомьтесь с предыдущей таблицей и комментариями.

- Элементы с поддержкой BYOL: эти элементы доступны. Полный список элементов Azure Marketplace с поддержкой BYOL см. на [этой странице](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Сторонние элементы Azure Marketplace с оплатой по мере использования: эти элементы доступны, если поставщик опубликован в канале CSP. См. сведения о [продаже подписок на продукты Azure Marketplace](https://aka.ms/marketplaceincsp).   

- Citrix XenApp Essentials: партнеры могут приобрести XenApp Essentials для клиентов в CSP. Сведения о распространении XenApp Essentials через канал поставщика облачных решений (Майкрософт) см. в [блоге Citrix](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

### <a name="national-clouds"></a>Национальные облака 
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

### <a name="next-steps"></a>Дальнейшие действия

- [Узнайте](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) о доступных возможностях Azure в Центре партнеров.

- [Создайте](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) первого клиента в Azure CSP и разверните службы Azure.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Переход с существующих предложений CSP на план Azure

Вы можете перевести клиента с существующих предложений Azure для CSP на службы Azure, доступные в плане Azure в новой коммерческой модели в программе CSP, перейдя в Центр партнеров. Для этого партнер и клиент должны установить взаимоотношения торговых посредников через Центр партнеров, а клиент должен подписать Клиентское соглашение Майкрософт.

### <a name="select-transition-to-azure-plan"></a>Выбор перехода в план Azure

1. Выберите план Azure для клиента.

2. Щелкните **Перевод выставления счетов в план Azure**.

![Переход](images/azure/transition1.png)

3. Выберите **Продолжить**.

![Переход](images/azure/transition2.png)

Ваш клиент будет переведен на план Azure автоматически.

**Рабочий процесс перехода автоматизирует необходимые шаги**:

- покупка планов Azure;
- один план на клиента в сценариях прямого партнера CSP;  
- один план для торгового посредника.  

Например, партнер приобрел два предложения Microsoft Azure и включил в покупку два отдельных заказа на поставку. В этом случае рабочий процесс перехода приобретет два плана Azure (по одному на торгового посредника) и автоматически сопоставит подписки Azure с этими планами Azure.  

**Сопоставление подписки Azure с планом Azure**

После приобретения планов Azure наша система сопоставит с ними существующие подписки Azure. Ход выполнения можно просмотреть на портале Azure, а также в Центре партнеров. 

4. Вернитесь на страницу **Подписки** клиента в Центре партнеров, чтобы обновить лимит бюджета в местной валюте. 

![Переход](images/azure/transition3.png)

>[!NOTE]
>Бюджет, заданный в Центре партнеров, не переносится на портал Azure. Вы также должны настроить бюджет и оповещение на портале Azure.

После перехода на план Azure вы больше не сможете покупать подписки Azure для этого клиента. Подписки можно будет создавать в плане Azure на портале Azure.

>[!NOTE]
> Плата за все подписки Azure, приобретенные с использованием RBAC в плане Azure, будет взиматься в местной валюте. Курсы валют не будут использоваться.

### <a name="track-your-transition-details"></a>Отслеживание сведений о переходе

Процесс перехода можно наблюдать на портале Azure и в Центре партнеров.

![Отображение сведений](images/azure/details1.png)

**Влияние на выставление счетов для партнеров**

Перевод клиента с существующего предложения CSP для Azure влияет на выставление счетов следующим образом.

- Вам будет выставлен счет по имеющимся предложениям CSP за все использование до момента перехода с исходной подписки CSP для Azure.

- Если у вас есть права доступа администратора к существующей подписке CSP, то после переноса этой подписки ваш доступ сохранится.

Чтобы перевести прямые Соглашения Enterprise для CSP и серверные и облачные регистрации на службы Azure, ознакомьтесь с [управлением выставлением счетов по подпискам Azure для соглашения с партнером Майкрософт](https://docs.microsoft.com/azure/billing/mpa-request-ownership).

**Журнал аудита**.

Чтобы согласовать выставление счетов, просмотрите журнал подписок "Microsoft Azure" (0145P) на странице **Подписки**. 

Подписка "Microsoft Azure" (0145P) состоит из двух частей:
1. коммерческая подписка; 
2. подписка Azure (права).

По завершении перехода подписка Azure перемещается в новый план Azure, а действие коммерческой подписки приостанавливается, поэтому в дальнейшем данные о ее использовании не отображаются.  

>Примечание. Если подписка Microsoft Azure (0145P) приобретена в рамках CSP, то коммерческая подписка и подписка Azure (права) имеют одинаковое значение. Значения могут отличаться только в случае изменения или перемещения владельца выставления счетов. 

**Проблемы перехода**

Во время перехода мы не ожидаем каких-либо проблем. При возникновении каких-либо проблем мы сообщим вам об этом в самом рабочем процессе перехода. Это не нарушит работу Azure.  

## <a name="next-steps"></a>Дальнейшие действия

- [Управление подписками и ресурсами в плане Azure](azure-plan-manage.md)

- [Общие сведения о партнерских баллах](partner-earned-credit.md)



