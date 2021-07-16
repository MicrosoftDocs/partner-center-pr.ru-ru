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
# <a name="sample-application"></a><span data-ttu-id="420fd-103">Образец приложения</span><span class="sxs-lookup"><span data-stu-id="420fd-103">Sample Application</span></span>

<span data-ttu-id="420fd-104">Примеры приложений создаются на языках C# и JAVA и доступны на [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="420fd-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="420fd-105">Пример приложения C#</span><span class="sxs-lookup"><span data-stu-id="420fd-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="420fd-106">Пример приложения JAVA</span><span class="sxs-lookup"><span data-stu-id="420fd-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="420fd-107">Можно использовать пример приложения, чтобы создать собственное приложение на любом языке.</span><span class="sxs-lookup"><span data-stu-id="420fd-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="420fd-108">Пример приложения достигает следующих целей:</span><span class="sxs-lookup"><span data-stu-id="420fd-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="420fd-109">создает маркер Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="420fd-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="420fd-110">Получение доступных наборов данных.</span><span class="sxs-lookup"><span data-stu-id="420fd-110">Gets available datasets.</span></span>
- <span data-ttu-id="420fd-111">Создает определяемые пользователем запросы.</span><span class="sxs-lookup"><span data-stu-id="420fd-111">Creates user defined queries.</span></span>
- <span data-ttu-id="420fd-112">Получает определяемые пользователем и системные запросы.</span><span class="sxs-lookup"><span data-stu-id="420fd-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="420fd-113">Планирование отчетов.</span><span class="sxs-lookup"><span data-stu-id="420fd-113">Schedules a report.</span></span>

<span data-ttu-id="420fd-114">Пример приложения не охватывает метод вызова API для других функций.</span><span class="sxs-lookup"><span data-stu-id="420fd-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="420fd-115">Однако процесс вызова других API-интерфейсов остается таким же, как описано выше.</span><span class="sxs-lookup"><span data-stu-id="420fd-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="420fd-116">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="420fd-116">How to run the application</span></span>

- <span data-ttu-id="420fd-117">Выполните клонирование репозитория в локальную систему с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="420fd-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="420fd-118">дополнительные инструкции см. в файле программатицекспортсамплеаппмпн/README. md в [репозитории](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub.</span><span class="sxs-lookup"><span data-stu-id="420fd-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="420fd-119">Чтобы быстро запустить приложение, обновите идентификатор клиента и секрет клиента в **appsettings.Development.jsна**</span><span class="sxs-lookup"><span data-stu-id="420fd-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Иллюстрация разработки AppSetting в формате JSON":::

<span data-ttu-id="420fd-121">При запуске приложения запускается локальный веб-сервер, и открывается страница (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span><span class="sxs-lookup"><span data-stu-id="420fd-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Иллюстрация пользовательского интерфейса примера приложения":::

<span data-ttu-id="420fd-123">На этой странице будут выполняться вызовы API к веб-серверу, работающему на локальном компьютере, который, в свою очередь, выполняет фактические вызовы API программного доступа.</span><span class="sxs-lookup"><span data-stu-id="420fd-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="420fd-124">Фрагменты кода</span><span class="sxs-lookup"><span data-stu-id="420fd-124">Code Snippets</span></span>

<span data-ttu-id="420fd-125">Базовая структура кода C# для выполнения вызовов API программного доступа имеет следующий вызов:</span><span class="sxs-lookup"><span data-stu-id="420fd-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Иллюстрация фрагмента кода":::

## <a name="next-steps"></a><span data-ttu-id="420fd-127">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="420fd-127">Next steps</span></span>

[<span data-ttu-id="420fd-128">Интерфейсы API для доступа к данным аналитики Partner Insights</span><span class="sxs-lookup"><span data-stu-id="420fd-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
