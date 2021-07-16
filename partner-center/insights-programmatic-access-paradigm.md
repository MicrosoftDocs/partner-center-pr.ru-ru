---
title: парадигма программного доступа к данным Аналитика
description: Общие сведения о высокоуровневом потоке шаблона вызова API для программной аналитики. Также рассматриваются API-интерфейсы для доступа к отчетам аналитики Partner Insights.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375888"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="bb81c-104">Парадигма программного доступа</span><span class="sxs-lookup"><span data-stu-id="bb81c-104">Programmatic access paradigm</span></span>

<span data-ttu-id="bb81c-105">На этой схеме показан шаблон вызова API, используемый для создания нового шаблона отчета, планирования пользовательского отчета и получения данных об ошибках.</span><span class="sxs-lookup"><span data-stu-id="bb81c-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Поток высокого уровня":::
<span data-ttu-id="bb81c-107">***Рис. 1. поток высокого уровня в шаблоне вызова API***</span><span class="sxs-lookup"><span data-stu-id="bb81c-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="bb81c-108">Этот список содержит дополнительные сведения о рис. 1.</span><span class="sxs-lookup"><span data-stu-id="bb81c-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="bb81c-109">Клиентское приложение может определить схему или шаблон пользовательского отчета, вызвав [API создания запроса отчета](#create-report-query-api).</span><span class="sxs-lookup"><span data-stu-id="bb81c-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="bb81c-110">Кроме того, можно выбрать шаблон отчета (QueryId) из примеров библиотеки шаблонов отчетов, перечисленных [здесь.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="bb81c-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="bb81c-111">При успешном выполнении API создания запросов отчета возвращает QueryId.</span><span class="sxs-lookup"><span data-stu-id="bb81c-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="bb81c-112">Затем клиентскому приложению необходимо вызвать [API создания отчета](#create-report-api) с помощью QueryId вместе с датой начала отчета, интервалом повтора, повторением и необязательным URI обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="bb81c-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="bb81c-113">При успешном выполнении [API создания отчета](#create-report-api) возвращает идентификатор reportID.</span><span class="sxs-lookup"><span data-stu-id="bb81c-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="bb81c-114">Клиентское приложение получает уведомления по URL-адресу обратного вызова, как только данные отчета готовы к скачиванию.</span><span class="sxs-lookup"><span data-stu-id="bb81c-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="bb81c-115">Затем клиентское приложение использует [API получения отчетов для выполнения](#get-report-execution-api) запроса состояния отчета с идентификатором отчета и диапазоном дат.</span><span class="sxs-lookup"><span data-stu-id="bb81c-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="bb81c-116">При успешном выполнении возвращается ссылка на скачивание отчета, после чего приложение может инициировать скачивание данных.</span><span class="sxs-lookup"><span data-stu-id="bb81c-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="bb81c-117">Спецификация языка запросов отчетов</span><span class="sxs-lookup"><span data-stu-id="bb81c-117">Report query language specification</span></span>

<span data-ttu-id="bb81c-118">В то время как мы предоставляем [системные запросы](insights-programmatic-system-queries.md) , которые можно использовать для создания отчетов, можно также создавать собственные запросы на основе бизнес-потребностей.</span><span class="sxs-lookup"><span data-stu-id="bb81c-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="bb81c-119">Дополнительные сведения о пользовательских запросах см. в разделе [Спецификация настраиваемого запроса](insights-programmatic-custom-query.md).</span><span class="sxs-lookup"><span data-stu-id="bb81c-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="bb81c-120">API создания запросов отчетов</span><span class="sxs-lookup"><span data-stu-id="bb81c-120">Create report query API</span></span>

<span data-ttu-id="bb81c-121">API помогает создавать пользовательские запросы, определяющие набор данных, из которого должны быть экспортированы столбцы и метрики.</span><span class="sxs-lookup"><span data-stu-id="bb81c-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="bb81c-122">Он позволяет гибко создавать шаблоны отчетов с учетом потребностей организации.</span><span class="sxs-lookup"><span data-stu-id="bb81c-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="bb81c-123">Вы также можете использовать [системные запросы](insights-programmatic-system-queries.md), которые предоставляем мы.</span><span class="sxs-lookup"><span data-stu-id="bb81c-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="bb81c-124">Если пользовательские шаблоны отчетов не нужны, можно вызвать [API Create Report](#create-report-api) напрямую с помощью куеридс системных запросов.</span><span class="sxs-lookup"><span data-stu-id="bb81c-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="bb81c-125">В следующем примере показано, как создать настраиваемый запрос для получения 10 лучших клиентов по доходу за прошлый месяц.</span><span class="sxs-lookup"><span data-stu-id="bb81c-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="bb81c-126">Синтаксис запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-126">Request syntax</span></span>

|    <span data-ttu-id="bb81c-127">Метод</span><span class="sxs-lookup"><span data-stu-id="bb81c-127">Method</span></span>     |    <span data-ttu-id="bb81c-128">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="bb81c-129">POST</span><span class="sxs-lookup"><span data-stu-id="bb81c-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="bb81c-130">Заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-130">Request header</span></span>

|    <span data-ttu-id="bb81c-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb81c-131">Header</span></span>     |    <span data-ttu-id="bb81c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="bb81c-132">Type</span></span>     |    <span data-ttu-id="bb81c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="bb81c-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb81c-134">Authorization</span></span>     |    <span data-ttu-id="bb81c-135">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-135">string</span></span> |<span data-ttu-id="bb81c-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb81c-136">Required.</span></span> <span data-ttu-id="bb81c-137">Маркер доступа Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bb81c-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="bb81c-138">Формат:  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="bb81c-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="bb81c-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb81c-139">Content-Type</span></span>     |<span data-ttu-id="bb81c-140">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="bb81c-141">Параметр пути</span><span class="sxs-lookup"><span data-stu-id="bb81c-141">Path parameter</span></span>

<span data-ttu-id="bb81c-142">None</span><span class="sxs-lookup"><span data-stu-id="bb81c-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="bb81c-143">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-143">Query parameter</span></span>

<span data-ttu-id="bb81c-144">None</span><span class="sxs-lookup"><span data-stu-id="bb81c-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="bb81c-145">Пример полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="bb81c-146">Глоссарий</span><span class="sxs-lookup"><span data-stu-id="bb81c-146">Glossary</span></span>

<span data-ttu-id="bb81c-147">В этой таблице приводятся основные определения элементов в полезных данных запроса.</span><span class="sxs-lookup"><span data-stu-id="bb81c-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="bb81c-148">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb81c-148">Parameter</span></span>|    <span data-ttu-id="bb81c-149">Обязательно</span><span class="sxs-lookup"><span data-stu-id="bb81c-149">Required</span></span>     |    <span data-ttu-id="bb81c-150">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-150">Description</span></span>     |    <span data-ttu-id="bb81c-151">Допустимые значения</span><span class="sxs-lookup"><span data-stu-id="bb81c-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="bb81c-152">Имя</span><span class="sxs-lookup"><span data-stu-id="bb81c-152">Name</span></span> |    <span data-ttu-id="bb81c-153">Да</span><span class="sxs-lookup"><span data-stu-id="bb81c-153">Yes</span></span>     |    <span data-ttu-id="bb81c-154">Понятное имя запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-154">Friendly name of the query</span></span>     |    <span data-ttu-id="bb81c-155">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-155">string</span></span>     |
|    <span data-ttu-id="bb81c-156">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-156">Description</span></span>     |    <span data-ttu-id="bb81c-157">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-157">No</span></span>     |    <span data-ttu-id="bb81c-158">Описание данных, возвращаемых запросом</span><span class="sxs-lookup"><span data-stu-id="bb81c-158">Description of what the query returns</span></span>     |    <span data-ttu-id="bb81c-159">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-159">string</span></span>     |
|    <span data-ttu-id="bb81c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb81c-160">Query</span></span>     |    <span data-ttu-id="bb81c-161">Да</span><span class="sxs-lookup"><span data-stu-id="bb81c-161">Yes</span></span>     |    <span data-ttu-id="bb81c-162">Строка запроса отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-162">Report query string</span></span>     |    <span data-ttu-id="bb81c-163">Тип данных: строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-163">Data type: string</span></span> <br> <span data-ttu-id="bb81c-164">[Пользовательский запрос](insights-programmatic-custom-query.md) с учетом потребностей организации</span><span class="sxs-lookup"><span data-stu-id="bb81c-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="bb81c-165">Примеры [запросов см.](insights-programmatic-sample-queries.md) в примерах пользовательских запросов.</span><span class="sxs-lookup"><span data-stu-id="bb81c-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="bb81c-166">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="bb81c-166">Sample response</span></span>

<span data-ttu-id="bb81c-167">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="bb81c-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="bb81c-168">Коды ответов: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="bb81c-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="bb81c-169">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="bb81c-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="bb81c-170">Глоссарий</span><span class="sxs-lookup"><span data-stu-id="bb81c-170">Glossary</span></span>

<span data-ttu-id="bb81c-171">В этой таблице приводятся основные определения элементов в полезных данных запроса.</span><span class="sxs-lookup"><span data-stu-id="bb81c-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="bb81c-172">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb81c-172">Parameter</span></span>     |    <span data-ttu-id="bb81c-173">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="bb81c-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="bb81c-174">QueryId</span></span>     |    <span data-ttu-id="bb81c-175">Универсальный уникальный идентификатор (UUID) созданного запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="bb81c-176">Имя</span><span class="sxs-lookup"><span data-stu-id="bb81c-176">Name</span></span>     |    <span data-ttu-id="bb81c-177">Понятное имя, присвоенное запросу в полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="bb81c-178">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-178">Description</span></span>     |    <span data-ttu-id="bb81c-179">Описание, заданное при создании запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="bb81c-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb81c-180">Query</span></span>     |    <span data-ttu-id="bb81c-181">Запрос отчета, передаваемый как входные данные при создании запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="bb81c-182">Тип</span><span class="sxs-lookup"><span data-stu-id="bb81c-182">Type</span></span>     |    <span data-ttu-id="bb81c-183">Установите значение `userDefined`</span><span class="sxs-lookup"><span data-stu-id="bb81c-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="bb81c-184">Пользователь</span><span class="sxs-lookup"><span data-stu-id="bb81c-184">User</span></span>     |    <span data-ttu-id="bb81c-185">Идентификатор пользователя, используемый для создания запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="bb81c-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="bb81c-186">CreatedTime</span></span>     |    <span data-ttu-id="bb81c-187">Время создания запроса в формате UTC: гггг-мм-ddTчч: мм: ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bb81c-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bb81c-188">TotalCount</span></span>     |    <span data-ttu-id="bb81c-189">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="bb81c-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="bb81c-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="bb81c-190">StatusCode</span></span>     |    <span data-ttu-id="bb81c-191">Код результата</span><span class="sxs-lookup"><span data-stu-id="bb81c-191">Result Code</span></span> <br> <span data-ttu-id="bb81c-192">Возможные значения — 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="bb81c-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="bb81c-193">message</span><span class="sxs-lookup"><span data-stu-id="bb81c-193">message</span></span>     |    <span data-ttu-id="bb81c-194">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="bb81c-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="bb81c-195">API создания отчетов</span><span class="sxs-lookup"><span data-stu-id="bb81c-195">Create report API</span></span>

<span data-ttu-id="bb81c-196">При успешном создании пользовательского шаблона отчета и получении QueryID в ответе на [запрос создания отчета](#create-report-query-api) этот API можно вызвать, чтобы запланировать выполнение запроса с регулярными интервалами.</span><span class="sxs-lookup"><span data-stu-id="bb81c-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="bb81c-197">Вы можете настроить частоту и расписание доставки отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="bb81c-198">Для предоставляемых нами системных запросов API создания отчетов также можно вызывать с помощью [QueryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="bb81c-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="bb81c-199">URL-адрес обратного вызова</span><span class="sxs-lookup"><span data-stu-id="bb81c-199">Callback URL</span></span>

<span data-ttu-id="bb81c-200">API создания отчета принимает URL-адрес обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="bb81c-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="bb81c-201">Этот URL-адрес будет вызываться после успешного создания отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="bb81c-202">URL-адрес обратного вызова должен иметь открытый доступ.</span><span class="sxs-lookup"><span data-stu-id="bb81c-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="bb81c-203">Кроме URL-адреса, можно также предоставить метод обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="bb81c-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="bb81c-204">Метод обратного вызова может иметь только значение "GET" или "POST".</span><span class="sxs-lookup"><span data-stu-id="bb81c-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="bb81c-205">Метод по умолчанию, если значение не передается "POST".</span><span class="sxs-lookup"><span data-stu-id="bb81c-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="bb81c-206">Идентификатор reportID, который завершил создание, всегда будет передаваться обратно во время обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="bb81c-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="bb81c-207">Обратный вызов: если передан URL-адрес `https://www.contosso.com/callback` , то вызываемый URL-адрес обратной передачи будет `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="bb81c-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="bb81c-208">ПОЛУЧИТЬ обратный вызов: если передан URL-адрес `https://www.contosso.com/callback` , то вызываемый URL-адрес обратной передачи будет `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="bb81c-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="bb81c-209">Отчеты Ексекутенов</span><span class="sxs-lookup"><span data-stu-id="bb81c-209">ExecuteNow reports</span></span>

<span data-ttu-id="bb81c-210">Существует возможность создания отчета без планирования.</span><span class="sxs-lookup"><span data-stu-id="bb81c-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="bb81c-211">Полезные данные API создания отчета могут принимать параметр `ExecuteNow` , который будет помещать отчет в очередь для создания, как только будет вызван API.</span><span class="sxs-lookup"><span data-stu-id="bb81c-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="bb81c-212">Если `ExecuteNow` для задано значение true, поля: `StartTime` , `RecurrenceCount` , `RecurrenceInterval` не учитываются, так как эти отчеты не запланированы.</span><span class="sxs-lookup"><span data-stu-id="bb81c-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="bb81c-213">При значении true можно передавать два дополнительных поля `ExecuteNow` , `QueryStartTime` и `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="bb81c-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="bb81c-214">Эти два поля будут переопределять `TIMESPAN` поле в запросе.</span><span class="sxs-lookup"><span data-stu-id="bb81c-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="bb81c-215">Эти поля не применяются к запланированным отчетам, так как данные будут непрерывно созданы в течение фиксированного периода времени, который не изменяется.</span><span class="sxs-lookup"><span data-stu-id="bb81c-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="bb81c-216">Синтаксис запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-216">Request syntax</span></span>

|    <span data-ttu-id="bb81c-217">Метод</span><span class="sxs-lookup"><span data-stu-id="bb81c-217">Method</span></span>     |    <span data-ttu-id="bb81c-218">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="bb81c-219">POST</span><span class="sxs-lookup"><span data-stu-id="bb81c-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="bb81c-220">Заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-220">Request header</span></span>

|    <span data-ttu-id="bb81c-221">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb81c-221">Header</span></span>     |    <span data-ttu-id="bb81c-222">Тип</span><span class="sxs-lookup"><span data-stu-id="bb81c-222">Type</span></span>     |    <span data-ttu-id="bb81c-223">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="bb81c-224">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb81c-224">Authorization</span></span>     |    <span data-ttu-id="bb81c-225">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-225">string</span></span> |<span data-ttu-id="bb81c-226">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb81c-226">Required.</span></span> <span data-ttu-id="bb81c-227">Маркер доступа Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bb81c-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="bb81c-228">Формат:  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="bb81c-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="bb81c-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb81c-229">Content-Type</span></span>     |<span data-ttu-id="bb81c-230">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="bb81c-231">Параметр пути</span><span class="sxs-lookup"><span data-stu-id="bb81c-231">Path Parameter</span></span>

<span data-ttu-id="bb81c-232">None</span><span class="sxs-lookup"><span data-stu-id="bb81c-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="bb81c-233">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-233">Query Parameter</span></span>

<span data-ttu-id="bb81c-234">None</span><span class="sxs-lookup"><span data-stu-id="bb81c-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="bb81c-235">Пример полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="bb81c-236">Глоссарий</span><span class="sxs-lookup"><span data-stu-id="bb81c-236">Glossary</span></span>

<span data-ttu-id="bb81c-237">Основные определения элементов в полезных данных запроса приведены ниже.</span><span class="sxs-lookup"><span data-stu-id="bb81c-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="bb81c-238">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb81c-238">Parameter</span></span>     |    <span data-ttu-id="bb81c-239">Обязательно</span><span class="sxs-lookup"><span data-stu-id="bb81c-239">Required</span></span>     |    <span data-ttu-id="bb81c-240">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-240">Description</span></span>     |    <span data-ttu-id="bb81c-241">Допустимые значения</span><span class="sxs-lookup"><span data-stu-id="bb81c-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="bb81c-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="bb81c-242">ReportName</span></span>     |    <span data-ttu-id="bb81c-243">Да</span><span class="sxs-lookup"><span data-stu-id="bb81c-243">Yes</span></span>     |    <span data-ttu-id="bb81c-244">Имя, назначаемое отчету</span><span class="sxs-lookup"><span data-stu-id="bb81c-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="bb81c-245">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-245">string</span></span>     |
|    <span data-ttu-id="bb81c-246">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-246">Description</span></span>     |    <span data-ttu-id="bb81c-247">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-247">No</span></span>     |    <span data-ttu-id="bb81c-248">Описание созданного отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-248">Description of the created report</span></span>     |    <span data-ttu-id="bb81c-249">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-249">string</span></span>     |
|    <span data-ttu-id="bb81c-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="bb81c-250">QueryId</span></span>     |    <span data-ttu-id="bb81c-251">Да</span><span class="sxs-lookup"><span data-stu-id="bb81c-251">Yes</span></span>     |    <span data-ttu-id="bb81c-252">Идентификатор запроса отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-252">Report query ID</span></span>     |    <span data-ttu-id="bb81c-253">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-253">string</span></span>     |
|    <span data-ttu-id="bb81c-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="bb81c-254">StartTime</span></span>     |    <span data-ttu-id="bb81c-255">Да</span><span class="sxs-lookup"><span data-stu-id="bb81c-255">Yes</span></span>     |    <span data-ttu-id="bb81c-256">Метка времени в формате UTC, после которой начнется создание отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="bb81c-257">Требуемый формат: гггг-мм-ддTчч:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="bb81c-258">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-258">string</span></span>     |
|    <span data-ttu-id="bb81c-259">ексекутенов</span><span class="sxs-lookup"><span data-stu-id="bb81c-259">ExecuteNow</span></span>     |    <span data-ttu-id="bb81c-260">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-260">No</span></span>     |    <span data-ttu-id="bb81c-261">Этот параметр следует использовать для создания отчета, который будет выполняться только один раз.</span><span class="sxs-lookup"><span data-stu-id="bb81c-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="bb81c-262">`StartTime``RecurrenceInterval`и `RecurrenceCount` не учитываются, если задано значение true.</span><span class="sxs-lookup"><span data-stu-id="bb81c-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="bb81c-263">Отчет немедленно выполняется в асинхронном режиме</span><span class="sxs-lookup"><span data-stu-id="bb81c-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="bb81c-264">true/false</span><span class="sxs-lookup"><span data-stu-id="bb81c-264">true/false</span></span>     |
|    <span data-ttu-id="bb81c-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="bb81c-265">QueryStartTime</span></span>     |    <span data-ttu-id="bb81c-266">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-266">No</span></span>     |    <span data-ttu-id="bb81c-267">Дополнительно указывает время начала для запроса на извлечение данных.</span><span class="sxs-lookup"><span data-stu-id="bb81c-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="bb81c-268">Этот параметр применим только для одного отчета о выполнении, для которого `ExecuteNow` задано значение true.</span><span class="sxs-lookup"><span data-stu-id="bb81c-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="bb81c-269">Установка этого параметра переопределяет значения `TIMESPAN` , заданные в запросе.</span><span class="sxs-lookup"><span data-stu-id="bb81c-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="bb81c-270">Требуемый формат: гггг-мм-ддTчч:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="bb81c-271">Отметка времени в виде строки</span><span class="sxs-lookup"><span data-stu-id="bb81c-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="bb81c-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="bb81c-272">QueryEndTime</span></span>     |    <span data-ttu-id="bb81c-273">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-273">No</span></span>     |    <span data-ttu-id="bb81c-274">Дополнительно указывает время окончания для запроса на извлечение данных.</span><span class="sxs-lookup"><span data-stu-id="bb81c-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="bb81c-275">Этот параметр применим только для одного отчета о выполнении, для которого `ExecuteNow` задано значение true.</span><span class="sxs-lookup"><span data-stu-id="bb81c-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="bb81c-276">Установка этого параметра переопределяет значения `TIMESPAN` , заданные в запросе.</span><span class="sxs-lookup"><span data-stu-id="bb81c-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="bb81c-277">Требуемый формат: гггг-мм-ддTчч:мм:ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="bb81c-278">Отметка времени в виде строки</span><span class="sxs-lookup"><span data-stu-id="bb81c-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="bb81c-279">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="bb81c-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="bb81c-280">Да</span><span class="sxs-lookup"><span data-stu-id="bb81c-280">Yes</span></span>     |    <span data-ttu-id="bb81c-281">Периодичность создания отчета в часах.</span><span class="sxs-lookup"><span data-stu-id="bb81c-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="bb81c-282">Минимальное значение равно 4, а максимальное значение — 2160.</span><span class="sxs-lookup"><span data-stu-id="bb81c-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="bb81c-283">Целое число</span><span class="sxs-lookup"><span data-stu-id="bb81c-283">integer</span></span>     |
|    <span data-ttu-id="bb81c-284">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="bb81c-284">RecurrenceCount</span></span>     |    <span data-ttu-id="bb81c-285">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-285">No</span></span>     |    <span data-ttu-id="bb81c-286">Число создаваемых отчетов.</span><span class="sxs-lookup"><span data-stu-id="bb81c-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="bb81c-287">Целое число</span><span class="sxs-lookup"><span data-stu-id="bb81c-287">integer</span></span>     |
|    <span data-ttu-id="bb81c-288">Формат</span><span class="sxs-lookup"><span data-stu-id="bb81c-288">Format</span></span>     |    <span data-ttu-id="bb81c-289">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-289">No</span></span>     |    <span data-ttu-id="bb81c-290">Формат экспортируемого файла.</span><span class="sxs-lookup"><span data-stu-id="bb81c-290">File format of the exported file.</span></span> <br> <span data-ttu-id="bb81c-291">Значение по умолчанию — CSV.</span><span class="sxs-lookup"><span data-stu-id="bb81c-291">Default is CSV.</span></span>    |    <span data-ttu-id="bb81c-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="bb81c-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="bb81c-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="bb81c-293">CallbackUrl</span></span>     |    <span data-ttu-id="bb81c-294">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-294">No</span></span>     |    <span data-ttu-id="bb81c-295">Общедоступный URL-адрес, который можно дополнительно настроить в качестве назначения обратного вызова</span><span class="sxs-lookup"><span data-stu-id="bb81c-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="bb81c-296">Строка (URL-адрес HTTP)</span><span class="sxs-lookup"><span data-stu-id="bb81c-296">String (http URL)</span></span>     |
|    <span data-ttu-id="bb81c-297">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="bb81c-297">CallbackMethod</span></span>     |    <span data-ttu-id="bb81c-298">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-298">No</span></span>     |    <span data-ttu-id="bb81c-299">Метод, используемый для обратного вызова</span><span class="sxs-lookup"><span data-stu-id="bb81c-299">The method to be used for callback</span></span>     |    <span data-ttu-id="bb81c-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="bb81c-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="bb81c-301">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="bb81c-301">Sample response</span></span>

<span data-ttu-id="bb81c-302">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="bb81c-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="bb81c-303">Коды ответов: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="bb81c-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="bb81c-304">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="bb81c-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a><span data-ttu-id="bb81c-305">Глоссарий</span><span class="sxs-lookup"><span data-stu-id="bb81c-305">Glossary</span></span>

<span data-ttu-id="bb81c-306">Основные определения элементов в ответе представлены ниже:</span><span class="sxs-lookup"><span data-stu-id="bb81c-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="bb81c-307">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb81c-307">Parameter</span></span>     |    <span data-ttu-id="bb81c-308">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="bb81c-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="bb81c-309">ReportId</span></span>     |    <span data-ttu-id="bb81c-310">Универсальный уникальный идентификатор (UUID) созданного отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="bb81c-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="bb81c-311">ReportName</span></span>     |    <span data-ttu-id="bb81c-312">Имя, присвоенное отчету в полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="bb81c-313">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-313">Description</span></span>     |    <span data-ttu-id="bb81c-314">Описание, заданное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="bb81c-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="bb81c-315">QueryId</span></span>     |    <span data-ttu-id="bb81c-316">Идентификатор запроса, переданный во время создания отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="bb81c-317">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb81c-317">Query</span></span>     |    <span data-ttu-id="bb81c-318">Текст запроса, который будет выполнен для этого отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="bb81c-319">Пользователь</span><span class="sxs-lookup"><span data-stu-id="bb81c-319">User</span></span>     |    <span data-ttu-id="bb81c-320">Идентификатор пользователя, используемый для создания отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="bb81c-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="bb81c-321">CreatedTime</span></span>     |    <span data-ttu-id="bb81c-322">Время создания отчета в формате UTC: гггг-мм-ddTчч: мм: ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bb81c-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="bb81c-323">ModifiedTime</span></span>     |    <span data-ttu-id="bb81c-324">Время последнего изменения отчета в формате UTC: гггг-мм-ddTчч: мм: ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bb81c-325">ексекутенов</span><span class="sxs-lookup"><span data-stu-id="bb81c-325">ExecuteNow</span></span>     |    <span data-ttu-id="bb81c-326">`ExecuteNow` флаг, установленный на момент создания отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="bb81c-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="bb81c-327">StartTime</span></span>     |    <span data-ttu-id="bb81c-328">Время начала выполнения отчета в формате UTC: гггг-мм-ddTчч: мм: ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="bb81c-329">репортстатус</span><span class="sxs-lookup"><span data-stu-id="bb81c-329">ReportStatus</span></span>     |    <span data-ttu-id="bb81c-330">Состояние выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-330">Status of the report execution.</span></span> <span data-ttu-id="bb81c-331">Возможные значения: `Paused` , `Active` и. `Inactive`</span><span class="sxs-lookup"><span data-stu-id="bb81c-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="bb81c-332">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="bb81c-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="bb81c-333">Интервал повторения, указанный при создании отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="bb81c-334">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="bb81c-334">RecurrenceCount</span></span>     |    <span data-ttu-id="bb81c-335">Число повторений, указанное при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="bb81c-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="bb81c-336">CallbackUrl</span></span>     |    <span data-ttu-id="bb81c-337">URL-адрес обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="bb81c-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="bb81c-338">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="bb81c-338">CallbackMethod</span></span>     |    <span data-ttu-id="bb81c-339">Метод обратного вызова, указанный в запросе</span><span class="sxs-lookup"><span data-stu-id="bb81c-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="bb81c-340">Формат</span><span class="sxs-lookup"><span data-stu-id="bb81c-340">Format</span></span>     |    <span data-ttu-id="bb81c-341">Формат файлов отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-341">Format of the report files.</span></span> <span data-ttu-id="bb81c-342">Возможные значения: `CSV` или `TSV` .</span><span class="sxs-lookup"><span data-stu-id="bb81c-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="bb81c-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bb81c-343">TotalCount</span></span>     |    <span data-ttu-id="bb81c-344">Число записей в массиве значений</span><span class="sxs-lookup"><span data-stu-id="bb81c-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="bb81c-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="bb81c-345">StatusCode</span></span>     |    <span data-ttu-id="bb81c-346">Код результата</span><span class="sxs-lookup"><span data-stu-id="bb81c-346">Result Code</span></span>     |
|    <span data-ttu-id="bb81c-347">message</span><span class="sxs-lookup"><span data-stu-id="bb81c-347">message</span></span>     |    <span data-ttu-id="bb81c-348">Возможные значения: 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="bb81c-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="bb81c-349">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="bb81c-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="bb81c-350">Получение API выполнения отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-350">Get report execution API</span></span>

<span data-ttu-id="bb81c-351">Этот метод можно использовать для запроса состояния выполнения отчета с помощью идентификатор reportID, полученной из [API создания отчета](#create-report-api).</span><span class="sxs-lookup"><span data-stu-id="bb81c-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="bb81c-352">Если отчет готов к скачиванию, метод возвращает ссылку для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="bb81c-353">В противном случае метод возвращает состояние.</span><span class="sxs-lookup"><span data-stu-id="bb81c-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="bb81c-354">Этот API также можно использовать для получения всех выполнений определенного отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="bb81c-355">Этот API имеет параметры запроса по умолчанию, заданные для `executionStatus=Completed` и `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="bb81c-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="bb81c-356">В связи с этим вызов API до первого успешного выполнения отчета возвращает 404.</span><span class="sxs-lookup"><span data-stu-id="bb81c-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="bb81c-357">Для получения ожидающих выполнений можно использовать параметр `executionStatus=Pending`.</span><span class="sxs-lookup"><span data-stu-id="bb81c-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="bb81c-358">Синтаксис запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-358">Request syntax</span></span>

|    <span data-ttu-id="bb81c-359">Метод</span><span class="sxs-lookup"><span data-stu-id="bb81c-359">Method</span></span>     |    <span data-ttu-id="bb81c-360">Универсальный код ресурса (URI) запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="bb81c-361">GET</span><span class="sxs-lookup"><span data-stu-id="bb81c-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="bb81c-362">Заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-362">Request header</span></span>

|    <span data-ttu-id="bb81c-363">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb81c-363">Header</span></span>     |    <span data-ttu-id="bb81c-364">Тип</span><span class="sxs-lookup"><span data-stu-id="bb81c-364">Type</span></span>     |    <span data-ttu-id="bb81c-365">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="bb81c-366">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb81c-366">Authorization</span></span>     |    <span data-ttu-id="bb81c-367">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-367">string</span></span> |<span data-ttu-id="bb81c-368">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb81c-368">Required.</span></span> <span data-ttu-id="bb81c-369">Маркер доступа Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bb81c-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="bb81c-370">Формат:  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="bb81c-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="bb81c-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb81c-371">Content-Type</span></span>     |<span data-ttu-id="bb81c-372">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="bb81c-373">Параметр пути</span><span class="sxs-lookup"><span data-stu-id="bb81c-373">Path parameter</span></span>

|    <span data-ttu-id="bb81c-374">имени параметра</span><span class="sxs-lookup"><span data-stu-id="bb81c-374">Parameter Name</span></span>    |    <span data-ttu-id="bb81c-375">Обязательно</span><span class="sxs-lookup"><span data-stu-id="bb81c-375">Required</span></span>    |    <span data-ttu-id="bb81c-376">Тип</span><span class="sxs-lookup"><span data-stu-id="bb81c-376">Type</span></span>    |    <span data-ttu-id="bb81c-377">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="bb81c-378">reportId</span><span class="sxs-lookup"><span data-stu-id="bb81c-378">reportId</span></span>    |    <span data-ttu-id="bb81c-379">Да</span><span class="sxs-lookup"><span data-stu-id="bb81c-379">Yes</span></span>    |    <span data-ttu-id="bb81c-380">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-380">string</span></span>    |    <span data-ttu-id="bb81c-381">Фильтр для получения сведений о выполнении только отчетов с идентификатор reportID, указанными в этом аргументе.</span><span class="sxs-lookup"><span data-stu-id="bb81c-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="bb81c-382">Несколько Репортидс можно указать, разделив их точкой с запятой ";".</span><span class="sxs-lookup"><span data-stu-id="bb81c-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="bb81c-383">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-383">Query parameter</span></span>

|    <span data-ttu-id="bb81c-384">имени параметра</span><span class="sxs-lookup"><span data-stu-id="bb81c-384">Parameter Name</span></span>    |    <span data-ttu-id="bb81c-385">Обязательно</span><span class="sxs-lookup"><span data-stu-id="bb81c-385">Required</span></span>    |    <span data-ttu-id="bb81c-386">Тип</span><span class="sxs-lookup"><span data-stu-id="bb81c-386">Type</span></span>    |    <span data-ttu-id="bb81c-387">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="bb81c-388">executionId</span><span class="sxs-lookup"><span data-stu-id="bb81c-388">executionId</span></span>    |    <span data-ttu-id="bb81c-389">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-389">No</span></span>    |    <span data-ttu-id="bb81c-390">строка</span><span class="sxs-lookup"><span data-stu-id="bb81c-390">string</span></span>    |    <span data-ttu-id="bb81c-391">Фильтр для получения сведений только об отчетах с executionId, указанными в этом аргументе.</span><span class="sxs-lookup"><span data-stu-id="bb81c-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="bb81c-392">Несколько Ексекутионидс можно указать, разделив их точкой с запятой ";".</span><span class="sxs-lookup"><span data-stu-id="bb81c-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="bb81c-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="bb81c-393">executionStatus</span></span>    |    <span data-ttu-id="bb81c-394">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-394">No</span></span>    |    <span data-ttu-id="bb81c-395">Строка или перечисление</span><span class="sxs-lookup"><span data-stu-id="bb81c-395">String/enum</span></span>    |    <span data-ttu-id="bb81c-396">Фильтр для получения сведений только об отчетах с Ексекутионстатус, указанными в этом аргументе.</span><span class="sxs-lookup"><span data-stu-id="bb81c-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="bb81c-397">Допустимые значения: `Pending` , `Running` `Paused` и `Completed` .</span><span class="sxs-lookup"><span data-stu-id="bb81c-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="bb81c-398">Значение по умолчанию — `Completed`.</span><span class="sxs-lookup"><span data-stu-id="bb81c-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="bb81c-399">Можно указать несколько состояний, разделяя их точкой с запятой ";".</span><span class="sxs-lookup"><span data-stu-id="bb81c-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="bb81c-400">жетлатестексекутион</span><span class="sxs-lookup"><span data-stu-id="bb81c-400">getLatestExecution</span></span>    |    <span data-ttu-id="bb81c-401">Нет</span><span class="sxs-lookup"><span data-stu-id="bb81c-401">No</span></span>    |    <span data-ttu-id="bb81c-402">Логическое</span><span class="sxs-lookup"><span data-stu-id="bb81c-402">boolean</span></span>    |    <span data-ttu-id="bb81c-403">API возвратит сведения о последнем выполнении.</span><span class="sxs-lookup"><span data-stu-id="bb81c-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="bb81c-404">По умолчанию этот параметр имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="bb81c-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="bb81c-405">Если вы решили передать значение этого параметра как false, API возвратит последние 90 дней выполнения.</span><span class="sxs-lookup"><span data-stu-id="bb81c-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="bb81c-406">Пример полезных данных запроса</span><span class="sxs-lookup"><span data-stu-id="bb81c-406">Sample Request Payload</span></span>

<span data-ttu-id="bb81c-407">None</span><span class="sxs-lookup"><span data-stu-id="bb81c-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="bb81c-408">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="bb81c-408">Sample Response</span></span>

<span data-ttu-id="bb81c-409">Полезные данные ответа имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="bb81c-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="bb81c-410">Коды ответов: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="bb81c-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="bb81c-411">Пример полезных данных ответа:</span><span class="sxs-lookup"><span data-stu-id="bb81c-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="bb81c-412">После выполнения отчета отобразится состояние выполнения `Completed`.</span><span class="sxs-lookup"><span data-stu-id="bb81c-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="bb81c-413">Вы можете скачать отчет по URL-адресу, указанному в параметре `reportAccessSecureLink`.</span><span class="sxs-lookup"><span data-stu-id="bb81c-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="bb81c-414">Глоссарий</span><span class="sxs-lookup"><span data-stu-id="bb81c-414">Glossary</span></span>

<span data-ttu-id="bb81c-415">Основные определения элементов в ответе.</span><span class="sxs-lookup"><span data-stu-id="bb81c-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="bb81c-416">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb81c-416">Parameter</span></span>    |    <span data-ttu-id="bb81c-417">Описание</span><span class="sxs-lookup"><span data-stu-id="bb81c-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="bb81c-418">ExecutionID</span><span class="sxs-lookup"><span data-stu-id="bb81c-418">ExecutionId</span></span>    |    <span data-ttu-id="bb81c-419">Универсальный уникальный идентификатор (UUID) экземпляра выполнения</span><span class="sxs-lookup"><span data-stu-id="bb81c-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="bb81c-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="bb81c-420">ReportId</span></span>    |    <span data-ttu-id="bb81c-421">Идентификатор отчета, связанный с экземпляром выполнения</span><span class="sxs-lookup"><span data-stu-id="bb81c-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="bb81c-422">рекурренцеинтервал</span><span class="sxs-lookup"><span data-stu-id="bb81c-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="bb81c-423">Интервал повторения, указанный при создании отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="bb81c-424">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="bb81c-424">RecurrenceCount</span></span>    |    <span data-ttu-id="bb81c-425">Число повторений, указанное при создании отчета</span><span class="sxs-lookup"><span data-stu-id="bb81c-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="bb81c-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="bb81c-426">CallbackUrl</span></span>    |    <span data-ttu-id="bb81c-427">URL-адрес обратного вызова, связанный с экземпляром выполнения</span><span class="sxs-lookup"><span data-stu-id="bb81c-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="bb81c-428">каллбаккмесод</span><span class="sxs-lookup"><span data-stu-id="bb81c-428">CallbackMethod</span></span>    |    <span data-ttu-id="bb81c-429">Метод обратного вызова, связанный с экземпляром выполнения</span><span class="sxs-lookup"><span data-stu-id="bb81c-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="bb81c-430">Формат</span><span class="sxs-lookup"><span data-stu-id="bb81c-430">Format</span></span>    |    <span data-ttu-id="bb81c-431">Формат созданного файла по завершении выполнения</span><span class="sxs-lookup"><span data-stu-id="bb81c-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="bb81c-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="bb81c-432">ExecutionStatus</span></span>    |    <span data-ttu-id="bb81c-433">Состояние экземпляра выполнения отчета.</span><span class="sxs-lookup"><span data-stu-id="bb81c-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="bb81c-434">Допустимые значения: `Pending`, `Running`, `Paused` и `Completed`</span><span class="sxs-lookup"><span data-stu-id="bb81c-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="bb81c-435">репортакцесссекурелинк</span><span class="sxs-lookup"><span data-stu-id="bb81c-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="bb81c-436">Ссылка для безопасного доступа к отчету</span><span class="sxs-lookup"><span data-stu-id="bb81c-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="bb81c-437">репортекспиритиме</span><span class="sxs-lookup"><span data-stu-id="bb81c-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="bb81c-438">Время, при наступлении которого истекает срок действия ссылки на отчет, в формате UTC: гггг-мм-ddTчч: мм: ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="bb81c-439">репортженератедтиме</span><span class="sxs-lookup"><span data-stu-id="bb81c-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="bb81c-440">Время создания отчета в формате UTC: гггг-мм-ddTHH: мм: ссZ</span><span class="sxs-lookup"><span data-stu-id="bb81c-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="bb81c-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bb81c-441">TotalCount</span></span>    |    <span data-ttu-id="bb81c-442">Количество наборов данных в массиве Value</span><span class="sxs-lookup"><span data-stu-id="bb81c-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="bb81c-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="bb81c-443">StatusCode</span></span>    |    <span data-ttu-id="bb81c-444">Код результата</span><span class="sxs-lookup"><span data-stu-id="bb81c-444">Result Code</span></span> <br> <span data-ttu-id="bb81c-445">Возможные значения: 200, 400, 401, 403, 404 и 500</span><span class="sxs-lookup"><span data-stu-id="bb81c-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="bb81c-446">message</span><span class="sxs-lookup"><span data-stu-id="bb81c-446">message</span></span>    |    <span data-ttu-id="bb81c-447">Сообщение о состоянии из выполнения API</span><span class="sxs-lookup"><span data-stu-id="bb81c-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="bb81c-448">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="bb81c-448">Next steps</span></span>

- <span data-ttu-id="bb81c-449">Испытайте интерфейсы API с помощью [URL-адреса API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) .</span><span class="sxs-lookup"><span data-stu-id="bb81c-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="bb81c-450">Выполнение первого вызова API</span><span class="sxs-lookup"><span data-stu-id="bb81c-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)