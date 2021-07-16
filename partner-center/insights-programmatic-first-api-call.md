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
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Сделайте первый вызов API для доступа к данным аналитики Partner Insights

Список API-интерфейсов для доступа к данным аналитики Partner Insights см. в разделе [API для доступа к данным аналитики Partner Insights](insights-programmatic-analytics-available-api.md). прежде чем приступить к первому вызову API, убедитесь, что выполнены [предварительные требования](insights-programmatic-prerequisites.md) для программного доступа к данным аналитики Partner Аналитика.

## <a name="token-generation"></a>Создание маркера

перед вызовом любого из методов сначала необходимо получить маркер доступа Azure Active Directory (AAD). Необходимо передать маркер доступа Azure AD в заголовок авторизации каждого метода в API. После получения маркера доступа у вас будет 60 минут, чтобы использовать его до истечения срока действия. По истечении срока действия маркера можно обновить маркер и продолжить его использование для дальнейших вызовов API.

См. ниже пример запроса для создания маркера. Для создания маркера требуются три значения: `clientId`, `clientSecret` и `tenantId`. Параметр ресурса должен иметь значение `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Пример запроса

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

#### <a name="response-example"></a>Пример ответа

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

Дополнительные сведения о получении маркера Azure AD для приложения см. в статье [доступ к данным аналитики с помощью служб хранилища.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Программный вызов API

После получения маркера AAD, как описано в предыдущем разделе, выполните следующие действия, чтобы создать первый отчет программного доступа.

Данные можно скачать из следующих наборов данных (datasetName):

- кустомерсандтенантс
- сеатссубскриптионсандревенуе
- AzureUsage
- мслеарн
- оффицеусаже
- Профиль
- траинингкомплетионс
- динамиксусаже
- компетенцисуммарихистори
- повербиусаже
- емсусаже
- компетенципеформанцерекуиремент
- реселлерперформанце
- класагриментреневалспропенсити
- класазурепропенсити
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- теамсусажеворклоад
- теамсусажемитингсандкаллс

В следующем разделе мы рассмотрим примеры программного доступа `SubscriptionId` из набора данных динамиксусаже.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Шаг 1. вызов функции RESTFUL с помощью API получения наборов данных

Ответ API предоставляет имя набора данных, откуда можно скачать отчет. Для конкретного набора данных ответ API также предоставляет список выбираемых столбцов, которые можно использовать для настраиваемого шаблона отчета. Можно также ссылаться на [определения данных](insights-data-definitions.md) , чтобы получить имена столбцов.

#### <a name="request-example"></a>Пример запроса

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Пример ответа

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

### <a name="step-2-create-the-custom-query"></a>Шаг 2. Создание настраиваемого запроса

На этом шаге мы будем использовать SubscriptionId из набора данных Динамиксусаже, чтобы создать настраиваемый запрос для отчета, который нам нужен. Интервал времени по умолчанию, если он не указан в запросе, составляет 6 месяцев.

#### <a name="request-example"></a>Пример запроса

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

#### <a name="response-example"></a>Пример ответа

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

При успешном выполнении запроса генерируется `queryId`, необходимый для создания отчета.

### <a name="step-3-execute-test-query-api"></a>Шаг 3. Выполнение API пробного запроса

На этом шаге мы будем использовать API тестовых запросов для получения первых 100 строк для созданного запроса.

#### <a name="request-example"></a>Пример запроса

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Пример ответа

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

### <a name="step-4-create-the-report"></a>Шаг 4. Создание отчета

На этом шаге мы будем использовать ранее созданный QueryId для создания отчета.

#### <a name="request-example"></a>Пример запроса

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

#### <a name="response-example"></a>Пример ответа

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

При успешном выполнении генерируется `reportId`, необходимый для планирования скачивания отчета.

### <a name="step-5-execute-report-executions-api"></a>Шаг 5. Выполнение API Report Executions

На этом шаге мы будем использовать API выполнения отчетов для получения безопасного расположения (URL) отчета.

#### <a name="request-example"></a>Пример запроса

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Пример ответа

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

## <a name="next-steps"></a>Дальнейшие действия

- Испытайте интерфейсы API с помощью [URL-адреса API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) .