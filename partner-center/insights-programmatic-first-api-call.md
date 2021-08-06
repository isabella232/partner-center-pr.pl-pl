---
title: Pierwsze wywołanie interfejsu API w celu uzyskania dostępu do danych analitycznych szczegółowych informacji partnerów
description: Przykłady, na których można dowiedzieć się, jak korzystać z interfejsu API w celu uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 76fb1b113a44e195114d67d79f192b3c2dce1071b7502f01af20387f69d62a8f
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697469"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Pierwsze wywołanie interfejsu API w celu uzyskania dostępu do danych analitycznych szczegółowych informacji partnerów

Aby uzyskać listę interfejsów API na temat uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów, zobacz Interfejsy API służące do uzyskiwania dostępu do danych analitycznych [szczegółowych informacji partnerów.](insights-programmatic-analytics-available-api.md) Przed pierwszym wywołaniem interfejsu API upewnij [](insights-programmatic-prerequisites.md) się, że spełniliśmy wymagania wstępne programowego uzyskiwania dostępu do danych analitycznych Szczegółowe informacje partnerów.

## <a name="token-generation"></a>Generowanie tokenu

Przed wywołaniem dowolnej z metod należy najpierw uzyskać token Azure Active Directory (AAD). Należy przekazać token dostępu usługi Azure AD do nagłówka Autoryzacja każdej metody w interfejsie API. Po uzyskaniu tokenu dostępu masz 60 minut na jego użycie przed wygaśnięciem. Po wygaśnięciu tokenu możesz odświeżyć token i nadal używać go do dalszych wywołań interfejsu API.

Zapoznaj się z poniższym przykładowym żądaniem generowania tokenu. Trzy wartości wymagane do wygenerowania tokenu to `clientId` , `clientSecret` i `tenantId` . Parametr zasobu powinien być ustawiony na `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Przykład żądania

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

#### <a name="response-example"></a>Przykład odpowiedzi

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

Aby uzyskać więcej informacji na temat sposobu uzyskiwania tokenu usługi Azure AD dla aplikacji, zobacz [Access analytics data using Store services (Uzyskiwanie](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token) dostępu do danych analitycznych przy użyciu usług Store Services).

## <a name="programmatic-api-call"></a>Programowe wywołanie interfejsu API

Po uzyskaniu tokenu usługi AAD zgodnie z opisem w poprzedniej sekcji wykonaj następujące kroki, aby utworzyć pierwszy programowy raport dostępu.

Dane można pobrać z następujących zestawów danych (datasetName):

- CustomersAndTenants
- MiejscaSubskrypcje IRavenue
- AzureUsage
- MsLearn
- OfficeUsage
- Profil
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetencyPeformanceRequirement
- ResellerPerformance (ResellerPerformance)
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

W poniższej sekcji przedstawiono przykłady programowego uzyskiwania dostępu z `SubscriptionId` zestawu danych DynamicsUsage.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Krok 1. Wywołanie REST przy użyciu interfejsu API pobierz zestawy danych

Odpowiedź interfejsu API zawiera nazwę zestawu danych, z którego można pobrać raport. W przypadku określonego zestawu danych odpowiedź interfejsu API zawiera również listę poszczególnych kolumn, których można użyć dla niestandardowego szablonu raportu. Możesz również odwołać się do [definicji danych,](insights-data-definitions.md) aby uzyskać nazwy kolumn.

#### <a name="request-example"></a>Przykład żądania

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Przykład odpowiedzi

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

### <a name="step-2-create-the-custom-query"></a>Krok 2. Tworzenie zapytania niestandardowego

W tym kroku użyjemy właściwości SubscriptionId z zestawu danych DynamicsUsage, aby utworzyć zapytanie niestandardowe dla raportu, którego potrzebujemy. Domyślny limit czasu, jeśli nie zostanie określony w zapytaniu, wynosi 6 miesięcy.

#### <a name="request-example"></a>Przykład żądania

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

#### <a name="response-example"></a>Przykład odpowiedzi

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

Po pomyślnym wykonaniu zapytania generowany jest kod , `queryId` który musi zostać użyty do wygenerowania raportu.

### <a name="step-3-execute-test-query-api"></a>Krok 3. Wykonywanie interfejsu API zapytania testowego

W tym kroku użyjemy interfejsu API zapytania testowego, aby uzyskać 100 górnych wierszy dla utworzonego zapytania.

#### <a name="request-example"></a>Przykład żądania

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Przykład odpowiedzi

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

### <a name="step-4-create-the-report"></a>Krok 4. Tworzenie raportu

W tym kroku użyjemy wcześniej wygenerowanego queryid do utworzenia raportu.

#### <a name="request-example"></a>Przykład żądania

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

#### <a name="response-example"></a>Przykład odpowiedzi

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

Po pomyślnym wykonaniu generowany jest plik , który musi zostać użyty `reportId` do zaplanowania pobrania raportu.

### <a name="step-5-execute-report-executions-api"></a>Krok 5. Wykonywanie interfejsu API wykonywania raportów

W tym kroku użyjemy interfejsu API wykonywania raportów, aby uzyskać bezpieczną lokalizację (adres URL) raportu.

#### <a name="request-example"></a>Przykład żądania

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Przykład odpowiedzi

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

## <a name="next-steps"></a>Następne kroki

- Wypróbuj interfejsy API za pomocą adresu [URL interfejsu API swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)