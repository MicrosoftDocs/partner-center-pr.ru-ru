---
title: Образец приложения
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Используйте пример приложения, чтобы создать собственное приложение для программного доступа к данным Partner Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375855"
---
# <a name="sample-application"></a>Образец приложения

Примеры приложений создаются на языках C# и JAVA и доступны на [GitHub](https://github.com/partneranalytics)

- [Пример приложения C#](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Пример приложения JAVA](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Можно использовать пример приложения, чтобы создать собственное приложение на любом языке.

Пример приложения достигает следующих целей:

- создает маркер Azure Active Directory (Azure AD).
- Получение доступных наборов данных.
- Создает определяемые пользователем запросы.
- Получает определяемые пользователем и системные запросы.
- Планирование отчетов.

Пример приложения не охватывает метод вызова API для других функций. Однако процесс вызова других API-интерфейсов остается таким же, как описано выше.

## <a name="how-to-run-the-application"></a>Запуск приложения

- Выполните клонирование репозитория в локальную систему с помощью следующей команды:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> дополнительные инструкции см. в файле программатицекспортсамплеаппмпн/README. md в [репозитории](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub.

- Чтобы быстро запустить приложение, обновите идентификатор клиента и секрет клиента в **appsettings.Development.jsна**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Иллюстрация разработки AppSetting в формате JSON":::

При запуске приложения запускается локальный веб-сервер, и открывается страница (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Иллюстрация пользовательского интерфейса примера приложения":::

На этой странице будут выполняться вызовы API к веб-серверу, работающему на локальном компьютере, который, в свою очередь, выполняет фактические вызовы API программного доступа.

## <a name="code-snippets"></a>Фрагменты кода

Базовая структура кода C# для выполнения вызовов API программного доступа имеет следующий вызов:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Иллюстрация фрагмента кода":::

## <a name="next-steps"></a>Дальнейшие действия

[Интерфейсы API для доступа к данным аналитики Partner Insights](insights-programmatic-analytics-available-api.md)
