---
title: Сделайте первый вызов API для доступа к данным аналитики Partner Insights
description: Примеры использования API для доступа к данным аналитики Partner Insights.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375867"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a><span data-ttu-id="8fac3-103">Сделайте первый вызов API для доступа к данным аналитики Partner Insights</span><span class="sxs-lookup"><span data-stu-id="8fac3-103">Make your first API call to access partner insights analytics data</span></span>

<span data-ttu-id="8fac3-104">Список API-интерфейсов для доступа к данным аналитики Partner Insights см. в разделе [API для доступа к данным аналитики Partner Insights](insights-programmatic-analytics-available-api.md).</span><span class="sxs-lookup"><span data-stu-id="8fac3-104">For a list of the APIs for accessing partner insights analytics data, see [APIs for accessing partner insights analytics data](insights-programmatic-analytics-available-api.md).</span></span> <span data-ttu-id="8fac3-105">прежде чем приступить к первому вызову API, убедитесь, что выполнены [предварительные требования](insights-programmatic-prerequisites.md) для программного доступа к данным аналитики Partner Аналитика.</span><span class="sxs-lookup"><span data-stu-id="8fac3-105">Before you make your first API call, make sure that you met the [pre-requisites](insights-programmatic-prerequisites.md) to programmatically access Partner Insights analytics data.</span></span>

## <a name="token-generation"></a><span data-ttu-id="8fac3-106">Создание маркера</span><span class="sxs-lookup"><span data-stu-id="8fac3-106">Token generation</span></span>

<span data-ttu-id="8fac3-107">перед вызовом любого из методов сначала необходимо получить маркер доступа Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="8fac3-107">Before calling any of the methods, you must first obtain an Azure Active Directory (AAD) access token.</span></span> <span data-ttu-id="8fac3-108">Необходимо передать маркер доступа Azure AD в заголовок авторизации каждого метода в API.</span><span class="sxs-lookup"><span data-stu-id="8fac3-108">You need to pass the Azure AD access token to the Authorization header of each method in the API.</span></span> <span data-ttu-id="8fac3-109">После получения маркера доступа у вас будет 60 минут, чтобы использовать его до истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="8fac3-109">After obtaining an access token, you have 60 minutes to use it before it expires.</span></span> <span data-ttu-id="8fac3-110">По истечении срока действия маркера можно обновить маркер и продолжить его использование для дальнейших вызовов API.</span><span class="sxs-lookup"><span data-stu-id="8fac3-110">After the token expires, you can refresh the token and can continue to use it for further calls to the API.</span></span>

<span data-ttu-id="8fac3-111">См. ниже пример запроса для создания маркера.</span><span class="sxs-lookup"><span data-stu-id="8fac3-111">Refer to a sample request below for generating a token.</span></span> <span data-ttu-id="8fac3-112">Для создания маркера требуются три значения: `clientId`, `clientSecret` и `tenantId`.</span><span class="sxs-lookup"><span data-stu-id="8fac3-112">The three values that are required to generate the token are `clientId`, `clientSecret`, and `tenantId`.</span></span> <span data-ttu-id="8fac3-113">Параметр ресурса должен иметь значение `https://api.partnercenter.microsoft.com`</span><span class="sxs-lookup"><span data-stu-id="8fac3-113">The resource parameter should be set to `https://api.partnercenter.microsoft.com`</span></span>

#### <a name="request-example"></a><span data-ttu-id="8fac3-114">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-114">Request example</span></span>

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a><span data-ttu-id="8fac3-115">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="8fac3-115">Response example</span></span>

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

<span data-ttu-id="8fac3-116">Дополнительные сведения о получении маркера Azure AD для приложения см. в статье [доступ к данным аналитики с помощью служб хранилища.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)</span><span class="sxs-lookup"><span data-stu-id="8fac3-116">For more information about how to obtain an Azure AD token for your application, see [Access analytics data using Store services.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)</span></span>

## <a name="programmatic-api-call"></a><span data-ttu-id="8fac3-117">Программный вызов API</span><span class="sxs-lookup"><span data-stu-id="8fac3-117">Programmatic API call</span></span>

<span data-ttu-id="8fac3-118">После получения маркера AAD, как описано в предыдущем разделе, выполните следующие действия, чтобы создать первый отчет программного доступа.</span><span class="sxs-lookup"><span data-stu-id="8fac3-118">After you obtain the AAD Token as described in the previous section, follow these steps to create your first programmatic access report.</span></span>

<span data-ttu-id="8fac3-119">Данные можно скачать из следующих наборов данных (datasetName):</span><span class="sxs-lookup"><span data-stu-id="8fac3-119">Data can be downloaded from the following datasets (datasetName):</span></span>

- <span data-ttu-id="8fac3-120">кустомерсандтенантс</span><span class="sxs-lookup"><span data-stu-id="8fac3-120">CustomersAndTenants</span></span>
- <span data-ttu-id="8fac3-121">сеатссубскриптионсандревенуе</span><span class="sxs-lookup"><span data-stu-id="8fac3-121">SeatsSubscriptionsAndRevenue</span></span>
- <span data-ttu-id="8fac3-122">AzureUsage</span><span class="sxs-lookup"><span data-stu-id="8fac3-122">AzureUsage</span></span>
- <span data-ttu-id="8fac3-123">мслеарн</span><span class="sxs-lookup"><span data-stu-id="8fac3-123">MSLearn</span></span>
- <span data-ttu-id="8fac3-124">оффицеусаже</span><span class="sxs-lookup"><span data-stu-id="8fac3-124">OfficeUsage</span></span>
- <span data-ttu-id="8fac3-125">Профиль</span><span class="sxs-lookup"><span data-stu-id="8fac3-125">Profile</span></span>
- <span data-ttu-id="8fac3-126">траинингкомплетионс</span><span class="sxs-lookup"><span data-stu-id="8fac3-126">TrainingCompletions</span></span>
- <span data-ttu-id="8fac3-127">динамиксусаже</span><span class="sxs-lookup"><span data-stu-id="8fac3-127">DynamicsUsage</span></span>
- <span data-ttu-id="8fac3-128">компетенцисуммарихистори</span><span class="sxs-lookup"><span data-stu-id="8fac3-128">CompetencySummaryHistory</span></span>
- <span data-ttu-id="8fac3-129">повербиусаже</span><span class="sxs-lookup"><span data-stu-id="8fac3-129">PowerBIUsage</span></span>
- <span data-ttu-id="8fac3-130">емсусаже</span><span class="sxs-lookup"><span data-stu-id="8fac3-130">EMSUsage</span></span>
- <span data-ttu-id="8fac3-131">компетенципеформанцерекуиремент</span><span class="sxs-lookup"><span data-stu-id="8fac3-131">CompetencyPeformanceRequirement</span></span>
- <span data-ttu-id="8fac3-132">реселлерперформанце</span><span class="sxs-lookup"><span data-stu-id="8fac3-132">ResellerPerformance</span></span>
- <span data-ttu-id="8fac3-133">класагриментреневалспропенсити</span><span class="sxs-lookup"><span data-stu-id="8fac3-133">CLASAgreementRenewalsPropensity</span></span>
- <span data-ttu-id="8fac3-134">класазурепропенсити</span><span class="sxs-lookup"><span data-stu-id="8fac3-134">CLASAzurePropensity</span></span>
- <span data-ttu-id="8fac3-135">CLASD365Propensity</span><span class="sxs-lookup"><span data-stu-id="8fac3-135">CLASD365Propensity</span></span>
- <span data-ttu-id="8fac3-136">CLASM365Propensity</span><span class="sxs-lookup"><span data-stu-id="8fac3-136">CLASM365Propensity</span></span>
- <span data-ttu-id="8fac3-137">TeamsUsage3PApps</span><span class="sxs-lookup"><span data-stu-id="8fac3-137">TeamsUsage3PApps</span></span>
- <span data-ttu-id="8fac3-138">теамсусажеворклоад</span><span class="sxs-lookup"><span data-stu-id="8fac3-138">TeamsUsageWorkload</span></span>
- <span data-ttu-id="8fac3-139">теамсусажемитингсандкаллс</span><span class="sxs-lookup"><span data-stu-id="8fac3-139">TeamsUsageMeetingsAndCalls</span></span>

<span data-ttu-id="8fac3-140">В следующем разделе мы рассмотрим примеры программного доступа `SubscriptionId` из набора данных динамиксусаже.</span><span class="sxs-lookup"><span data-stu-id="8fac3-140">In the following section, we will see examples of how to programmatically access `SubscriptionId` from the DynamicsUsage dataset.</span></span>

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a><span data-ttu-id="8fac3-141">Шаг 1. вызов функции RESTFUL с помощью API получения наборов данных</span><span class="sxs-lookup"><span data-stu-id="8fac3-141">Step 1: Make a REST call using the get datasets API</span></span>

<span data-ttu-id="8fac3-142">Ответ API предоставляет имя набора данных, откуда можно скачать отчет.</span><span class="sxs-lookup"><span data-stu-id="8fac3-142">The API response provides the dataset name from where you can download the report.</span></span> <span data-ttu-id="8fac3-143">Для конкретного набора данных ответ API также предоставляет список выбираемых столбцов, которые можно использовать для настраиваемого шаблона отчета.</span><span class="sxs-lookup"><span data-stu-id="8fac3-143">For the specific dataset, the API response also provides the list of selectable columns that can be used for your custom report template.</span></span> <span data-ttu-id="8fac3-144">Можно также ссылаться на [определения данных](insights-data-definitions.md) , чтобы получить имена столбцов.</span><span class="sxs-lookup"><span data-stu-id="8fac3-144">You can also refer to the [Data Definitions](insights-data-definitions.md) to get the names of the columns.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8fac3-145">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-145">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="8fac3-146">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="8fac3-146">Response example</span></span>

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a><span data-ttu-id="8fac3-147">Шаг 2. Создание настраиваемого запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-147">Step 2: Create the Custom Query</span></span>

<span data-ttu-id="8fac3-148">На этом шаге мы будем использовать SubscriptionId из набора данных Динамиксусаже, чтобы создать настраиваемый запрос для отчета, который нам нужен.</span><span class="sxs-lookup"><span data-stu-id="8fac3-148">In this step, we will use SubscriptionId from the DynamicsUsage dataset to create a custom query for the report we want.</span></span> <span data-ttu-id="8fac3-149">Интервал времени по умолчанию, если он не указан в запросе, составляет 6 месяцев.</span><span class="sxs-lookup"><span data-stu-id="8fac3-149">The default timespan if not specified in the query is 6 months.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8fac3-150">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-150">Request example</span></span>

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a><span data-ttu-id="8fac3-151">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="8fac3-151">Response example</span></span>

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="8fac3-152">При успешном выполнении запроса генерируется `queryId`, необходимый для создания отчета.</span><span class="sxs-lookup"><span data-stu-id="8fac3-152">On successful execution of the query, a `queryId` is generated that needs to be used to generate the report.</span></span>

### <a name="step-3-execute-test-query-api"></a><span data-ttu-id="8fac3-153">Шаг 3. Выполнение API пробного запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-153">Step 3: Execute test query API</span></span>

<span data-ttu-id="8fac3-154">На этом шаге мы будем использовать API тестовых запросов для получения первых 100 строк для созданного запроса.</span><span class="sxs-lookup"><span data-stu-id="8fac3-154">In this step, we will use the test query API to get the top 100 rows for the query that was created.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8fac3-155">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-155">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="8fac3-156">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="8fac3-156">Response example</span></span>

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a><span data-ttu-id="8fac3-157">Шаг 4. Создание отчета</span><span class="sxs-lookup"><span data-stu-id="8fac3-157">Step 4: Create the report</span></span>

<span data-ttu-id="8fac3-158">На этом шаге мы будем использовать ранее созданный QueryId для создания отчета.</span><span class="sxs-lookup"><span data-stu-id="8fac3-158">In this step, we will use the previously generated QueryId to create the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8fac3-159">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-159">Request example</span></span>

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a><span data-ttu-id="8fac3-160">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="8fac3-160">Response example</span></span>

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
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

<span data-ttu-id="8fac3-161">При успешном выполнении генерируется `reportId`, необходимый для планирования скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8fac3-161">On successful execution, a `reportId` is generated that needs to be used to schedule a download of the report.</span></span>

### <a name="step-5-execute-report-executions-api"></a><span data-ttu-id="8fac3-162">Шаг 5. Выполнение API Report Executions</span><span class="sxs-lookup"><span data-stu-id="8fac3-162">Step 5: Execute Report Executions API</span></span>

<span data-ttu-id="8fac3-163">На этом шаге мы будем использовать API выполнения отчетов для получения безопасного расположения (URL) отчета.</span><span class="sxs-lookup"><span data-stu-id="8fac3-163">In this step, we will use the Report Executions API to get the secure location (URL) of the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8fac3-164">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="8fac3-164">Request example</span></span>

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a><span data-ttu-id="8fac3-165">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="8fac3-165">Response example</span></span>

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a><span data-ttu-id="8fac3-166">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8fac3-166">Next steps</span></span>

- <span data-ttu-id="8fac3-167">Испытайте интерфейсы API с помощью [URL-адреса API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) .</span><span class="sxs-lookup"><span data-stu-id="8fac3-167">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>