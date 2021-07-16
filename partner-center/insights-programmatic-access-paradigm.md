---
title: Paradygmat dostępu programowego dla Szczegółowe informacje danych
description: Opis przepływu wysokiego poziomu wzorca wywołań interfejsu API dla analizy programowej. Interfejsy API służące do uzyskiwania dostępu do raportów analizy szczegółowych informacji partnerów są również objęte analizą.
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
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376982"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="85053-104">Paradygmat dostępu programowego</span><span class="sxs-lookup"><span data-stu-id="85053-104">Programmatic access paradigm</span></span>

<span data-ttu-id="85053-105">Na tym diagramie przedstawiono wzorzec wywołania interfejsu API używany do tworzenia nowego szablonu raportu, planowania raportu niestandardowego i pobierania danych błędów.</span><span class="sxs-lookup"><span data-stu-id="85053-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Przepływ wysokiego poziomu":::
<span data-ttu-id="85053-107">***Rysunek 1. Przepływ wysokiego poziomu wzorca wywołań interfejsu API***</span><span class="sxs-lookup"><span data-stu-id="85053-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="85053-108">Ta lista zawiera więcej szczegółów na temat rysunku 1.</span><span class="sxs-lookup"><span data-stu-id="85053-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="85053-109">Aplikacja kliencza może zdefiniować niestandardowy schemat/szablon raportu, wywołując [interfejs API tworzenia zapytania raportu.](#create-report-query-api)</span><span class="sxs-lookup"><span data-stu-id="85053-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="85053-110">Alternatywnie możesz wybrać szablon raportu (QueryId) z przykładów biblioteki szablonów raportów wymienionych [tutaj.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="85053-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="85053-111">W przypadku powodzenia interfejs API tworzenia zapytania raportu zwraca wartość QueryId.</span><span class="sxs-lookup"><span data-stu-id="85053-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="85053-112">Następnie aplikacja klienjąca musi wywołać interfejs [API](#create-report-api) tworzenia raportu przy użyciu parametru QueryId wraz z datą rozpoczęcia raportu, interwałem powtórzeń, cyklem i opcjonalnym URI wywołania zwrotnego.</span><span class="sxs-lookup"><span data-stu-id="85053-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="85053-113">W przypadku powodzenia interfejs [API tworzenia raportu](#create-report-api) zwraca wartość ReportId.</span><span class="sxs-lookup"><span data-stu-id="85053-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="85053-114">Aplikacja klienjąca jest powiadamiana pod adresem URL wywołania zwrotnego, gdy tylko dane raportu będą gotowe do pobrania.</span><span class="sxs-lookup"><span data-stu-id="85053-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="85053-115">Następnie aplikacja kliency używa interfejsu API get [report executions do](#get-report-execution-api) wykonywania zapytań o stan raportu przy użyciu identyfikatora raportu i zakresu dat.</span><span class="sxs-lookup"><span data-stu-id="85053-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="85053-116">W przypadku powodzenia jest zwracany link pobierania raportu, a aplikacja może zainicjować pobieranie danych.</span><span class="sxs-lookup"><span data-stu-id="85053-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="85053-117">Specyfikacja języka zapytań raportów</span><span class="sxs-lookup"><span data-stu-id="85053-117">Report query language specification</span></span>

<span data-ttu-id="85053-118">Chociaż zapewniamy zapytania [systemowe, których](insights-programmatic-system-queries.md) można używać do tworzenia raportów, możesz również tworzyć własne zapytania w zależności od potrzeb biznesowych.</span><span class="sxs-lookup"><span data-stu-id="85053-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="85053-119">Aby dowiedzieć się więcej na temat zapytań niestandardowych, zobacz [Custom Query Specification](insights-programmatic-custom-query.md).</span><span class="sxs-lookup"><span data-stu-id="85053-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="85053-120">Tworzenie interfejsu API zapytań raportu</span><span class="sxs-lookup"><span data-stu-id="85053-120">Create report query API</span></span>

<span data-ttu-id="85053-121">Interfejs API pomaga tworzyć zapytania niestandardowe definiujące zestaw danych, z którego należy wyeksportować kolumny i metryki.</span><span class="sxs-lookup"><span data-stu-id="85053-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="85053-122">Interfejs API zapewnia elastyczność tworzenia nowego szablonu raportowania w zależności od potrzeb biznesowych.</span><span class="sxs-lookup"><span data-stu-id="85053-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="85053-123">Możesz również użyć zapytań [systemowych, które](insights-programmatic-system-queries.md) udostępniliśmy.</span><span class="sxs-lookup"><span data-stu-id="85053-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="85053-124">Gdy niestandardowe szablony raportów nie są potrzebne, można wywołać interfejs [API](#create-report-api) tworzenia raportów bezpośrednio przy użyciu podanych zapytań systemowych QueryId.</span><span class="sxs-lookup"><span data-stu-id="85053-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="85053-125">W poniższym przykładzie pokazano, jak utworzyć zapytanie niestandardowe, aby uzyskać 10 klientów z najlepszymi przychodami w ostatnim miesiącu.</span><span class="sxs-lookup"><span data-stu-id="85053-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="85053-126">Składnia żądania</span><span class="sxs-lookup"><span data-stu-id="85053-126">Request syntax</span></span>

|    <span data-ttu-id="85053-127">Metoda</span><span class="sxs-lookup"><span data-stu-id="85053-127">Method</span></span>     |    <span data-ttu-id="85053-128">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="85053-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="85053-129">POST</span><span class="sxs-lookup"><span data-stu-id="85053-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="85053-130">Nagłówek żądania</span><span class="sxs-lookup"><span data-stu-id="85053-130">Request header</span></span>

|    <span data-ttu-id="85053-131">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="85053-131">Header</span></span>     |    <span data-ttu-id="85053-132">Typ</span><span class="sxs-lookup"><span data-stu-id="85053-132">Type</span></span>     |    <span data-ttu-id="85053-133">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="85053-134">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="85053-134">Authorization</span></span>     |    <span data-ttu-id="85053-135">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-135">string</span></span> |<span data-ttu-id="85053-136">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="85053-136">Required.</span></span> <span data-ttu-id="85053-137">Token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="85053-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="85053-138">Format to  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="85053-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="85053-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85053-139">Content-Type</span></span>     |<span data-ttu-id="85053-140">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="85053-141">Parametr ścieżki</span><span class="sxs-lookup"><span data-stu-id="85053-141">Path parameter</span></span>

<span data-ttu-id="85053-142">Brak</span><span class="sxs-lookup"><span data-stu-id="85053-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="85053-143">Parametr zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-143">Query parameter</span></span>

<span data-ttu-id="85053-144">Brak</span><span class="sxs-lookup"><span data-stu-id="85053-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="85053-145">Ładunek przykładowego żądania</span><span class="sxs-lookup"><span data-stu-id="85053-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="85053-146">Słownik</span><span class="sxs-lookup"><span data-stu-id="85053-146">Glossary</span></span>

<span data-ttu-id="85053-147">Ta tabela zawiera kluczowe definicje elementów w ładunku żądania.</span><span class="sxs-lookup"><span data-stu-id="85053-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="85053-148">Parametr</span><span class="sxs-lookup"><span data-stu-id="85053-148">Parameter</span></span>|    <span data-ttu-id="85053-149">Wymagane</span><span class="sxs-lookup"><span data-stu-id="85053-149">Required</span></span>     |    <span data-ttu-id="85053-150">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-150">Description</span></span>     |    <span data-ttu-id="85053-151">Dozwolone wartości</span><span class="sxs-lookup"><span data-stu-id="85053-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="85053-152">Nazwa</span><span class="sxs-lookup"><span data-stu-id="85053-152">Name</span></span> |    <span data-ttu-id="85053-153">Yes</span><span class="sxs-lookup"><span data-stu-id="85053-153">Yes</span></span>     |    <span data-ttu-id="85053-154">Przyjazna nazwa zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-154">Friendly name of the query</span></span>     |    <span data-ttu-id="85053-155">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-155">string</span></span>     |
|    <span data-ttu-id="85053-156">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-156">Description</span></span>     |    <span data-ttu-id="85053-157">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-157">No</span></span>     |    <span data-ttu-id="85053-158">Opis danych zwracanych przez zapytanie</span><span class="sxs-lookup"><span data-stu-id="85053-158">Description of what the query returns</span></span>     |    <span data-ttu-id="85053-159">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-159">string</span></span>     |
|    <span data-ttu-id="85053-160">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="85053-160">Query</span></span>     |    <span data-ttu-id="85053-161">Yes</span><span class="sxs-lookup"><span data-stu-id="85053-161">Yes</span></span>     |    <span data-ttu-id="85053-162">Ciąg zapytania raportu</span><span class="sxs-lookup"><span data-stu-id="85053-162">Report query string</span></span>     |    <span data-ttu-id="85053-163">Typ danych: ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-163">Data type: string</span></span> <br> <span data-ttu-id="85053-164">[Zapytanie niestandardowe oparte](insights-programmatic-custom-query.md) na potrzebach biznesowych</span><span class="sxs-lookup"><span data-stu-id="85053-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="85053-165">Aby uzyskać przykłady zapytań niestandardowych, [zobacz Przykłady przykładowych zapytań.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="85053-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="85053-166">Przykładowa odpowiedź</span><span class="sxs-lookup"><span data-stu-id="85053-166">Sample response</span></span>

<span data-ttu-id="85053-167">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="85053-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="85053-168">Kody odpowiedzi: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="85053-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="85053-169">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="85053-169">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="85053-170">Słownik</span><span class="sxs-lookup"><span data-stu-id="85053-170">Glossary</span></span>

<span data-ttu-id="85053-171">Ta tabela zawiera kluczowe definicje elementów w ładunku żądania.</span><span class="sxs-lookup"><span data-stu-id="85053-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="85053-172">Parametr</span><span class="sxs-lookup"><span data-stu-id="85053-172">Parameter</span></span>     |    <span data-ttu-id="85053-173">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="85053-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="85053-174">QueryId</span></span>     |    <span data-ttu-id="85053-175">Unikatowy identyfikator (UUID) utworzonego zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="85053-176">Nazwa</span><span class="sxs-lookup"><span data-stu-id="85053-176">Name</span></span>     |    <span data-ttu-id="85053-177">Przyjazna nazwa nadana zapytaniu w ładunku żądania</span><span class="sxs-lookup"><span data-stu-id="85053-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="85053-178">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-178">Description</span></span>     |    <span data-ttu-id="85053-179">Opis podany podczas tworzenia zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="85053-180">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="85053-180">Query</span></span>     |    <span data-ttu-id="85053-181">Zapytanie raportu przekazane jako dane wejściowe podczas tworzenia zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="85053-182">Typ</span><span class="sxs-lookup"><span data-stu-id="85053-182">Type</span></span>     |    <span data-ttu-id="85053-183">Ustaw wartość `userDefined`</span><span class="sxs-lookup"><span data-stu-id="85053-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="85053-184">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="85053-184">User</span></span>     |    <span data-ttu-id="85053-185">Identyfikator użytkownika użyty do utworzenia zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="85053-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="85053-186">CreatedTime</span></span>     |    <span data-ttu-id="85053-187">Czas UTC utworzenia zapytania w tym formacie: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="85053-188">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="85053-188">TotalCount</span></span>     |    <span data-ttu-id="85053-189">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="85053-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="85053-190">Statuscode</span><span class="sxs-lookup"><span data-stu-id="85053-190">StatusCode</span></span>     |    <span data-ttu-id="85053-191">Kod wyniku</span><span class="sxs-lookup"><span data-stu-id="85053-191">Result Code</span></span> <br> <span data-ttu-id="85053-192">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="85053-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="85053-193">message</span><span class="sxs-lookup"><span data-stu-id="85053-193">message</span></span>     |    <span data-ttu-id="85053-194">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="85053-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="85053-195">Tworzenie interfejsu API raportu</span><span class="sxs-lookup"><span data-stu-id="85053-195">Create report API</span></span>

<span data-ttu-id="85053-196">Po pomyślnym utworzeniu niestandardowego szablonu raportu i [](#create-report-query-api) otrzymaniu pola QueryID w ramach odpowiedzi na zapytanie dotyczące tworzenia raportu ten interfejs API może zostać wywołany w celu zaplanowania wykonywania zapytania w regularnych odstępach czasu.</span><span class="sxs-lookup"><span data-stu-id="85053-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="85053-197">Można ustawić częstotliwość i harmonogram dostarczenia raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="85053-198">W przypadku zapytań systemowych, które zapewniamy, interfejs API tworzenia raportu może być również wywoływany za pomocą [queryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="85053-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="85053-199">Adres URL wywołania zwrotnego</span><span class="sxs-lookup"><span data-stu-id="85053-199">Callback URL</span></span>

<span data-ttu-id="85053-200">Interfejs API tworzenia raportu akceptuje adres URL wywołania zwrotnego.</span><span class="sxs-lookup"><span data-stu-id="85053-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="85053-201">Ten adres URL zostanie wywołany po pomyślnym generowaniu raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="85053-202">Adres URL wywołania zwrotnego powinien być publicznie dostępny.</span><span class="sxs-lookup"><span data-stu-id="85053-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="85053-203">Oprócz adresu URL można również określić metodę wywołania zwrotnego.</span><span class="sxs-lookup"><span data-stu-id="85053-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="85053-204">Metodą wywołania zwrotnego może być tylko "GET" lub "POST".</span><span class="sxs-lookup"><span data-stu-id="85053-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="85053-205">Metoda domyślna, jeśli nie zostanie przekazana żadna wartość, to "POST".</span><span class="sxs-lookup"><span data-stu-id="85053-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="85053-206">ReportId, który zakończył generowanie zawsze będzie przekazywany z powrotem podczas wywołania zwrotnego.</span><span class="sxs-lookup"><span data-stu-id="85053-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="85053-207">Wywołanie zwrotne POST: Jeśli przekazany adres URL to `https://www.contosso.com/callback` , wywołany zwrotny adres URL to . `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="85053-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="85053-208">Wywołanie zwrotne GET: Jeśli przekazany adres URL to `https://www.contosso.com/callback` , wywołany zwrotny adres URL to . `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="85053-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="85053-209">Raporty executeNow</span><span class="sxs-lookup"><span data-stu-id="85053-209">ExecuteNow reports</span></span>

<span data-ttu-id="85053-210">Istnieje aprowizowanie do generowania raportu bez planowania.</span><span class="sxs-lookup"><span data-stu-id="85053-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="85053-211">Ładunek interfejsu API tworzenia raportu może akceptować parametr , który będzie kolejkować raport do wygenerowania zaraz po `ExecuteNow` wywołaniu interfejsu API.</span><span class="sxs-lookup"><span data-stu-id="85053-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="85053-212">W `ExecuteNow` przypadku ustawienia wartości true pola , , są `StartTime` ignorowane, ponieważ te `RecurrenceCount` `RecurrenceInterval` raporty nie są zaplanowane.</span><span class="sxs-lookup"><span data-stu-id="85053-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="85053-213">Dwa dodatkowe pola mogą być przekazywane, gdy `ExecuteNow` ma wartość true, `QueryStartTime` i `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="85053-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="85053-214">Te dwa pola `TIMESPAN` zastąpią pole w zapytaniu.</span><span class="sxs-lookup"><span data-stu-id="85053-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="85053-215">Te pola nie mają zastosowania do zaplanowanych raportów, ponieważ dane będą generowane w sposób ciągły przez ustalony czas, który nie zmienia się.</span><span class="sxs-lookup"><span data-stu-id="85053-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="85053-216">Składnia żądania</span><span class="sxs-lookup"><span data-stu-id="85053-216">Request syntax</span></span>

|    <span data-ttu-id="85053-217">Metoda</span><span class="sxs-lookup"><span data-stu-id="85053-217">Method</span></span>     |    <span data-ttu-id="85053-218">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="85053-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="85053-219">POST</span><span class="sxs-lookup"><span data-stu-id="85053-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="85053-220">Nagłówek żądania</span><span class="sxs-lookup"><span data-stu-id="85053-220">Request header</span></span>

|    <span data-ttu-id="85053-221">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="85053-221">Header</span></span>     |    <span data-ttu-id="85053-222">Typ</span><span class="sxs-lookup"><span data-stu-id="85053-222">Type</span></span>     |    <span data-ttu-id="85053-223">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="85053-224">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="85053-224">Authorization</span></span>     |    <span data-ttu-id="85053-225">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-225">string</span></span> |<span data-ttu-id="85053-226">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="85053-226">Required.</span></span> <span data-ttu-id="85053-227">Token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="85053-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="85053-228">Format to  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="85053-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="85053-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85053-229">Content-Type</span></span>     |<span data-ttu-id="85053-230">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="85053-231">Parametr ścieżki</span><span class="sxs-lookup"><span data-stu-id="85053-231">Path Parameter</span></span>

<span data-ttu-id="85053-232">Brak</span><span class="sxs-lookup"><span data-stu-id="85053-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="85053-233">Parametr zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-233">Query Parameter</span></span>

<span data-ttu-id="85053-234">Brak</span><span class="sxs-lookup"><span data-stu-id="85053-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="85053-235">Ładunek przykładowego żądania</span><span class="sxs-lookup"><span data-stu-id="85053-235">Sample request payload</span></span>

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

### <a name="glossary"></a><span data-ttu-id="85053-236">Słownik</span><span class="sxs-lookup"><span data-stu-id="85053-236">Glossary</span></span>

<span data-ttu-id="85053-237">Poniżej przedstawiono kluczowe definicje elementów w ładunku żądania:</span><span class="sxs-lookup"><span data-stu-id="85053-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="85053-238">Parametr</span><span class="sxs-lookup"><span data-stu-id="85053-238">Parameter</span></span>     |    <span data-ttu-id="85053-239">Wymagane</span><span class="sxs-lookup"><span data-stu-id="85053-239">Required</span></span>     |    <span data-ttu-id="85053-240">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-240">Description</span></span>     |    <span data-ttu-id="85053-241">Dozwolone wartości</span><span class="sxs-lookup"><span data-stu-id="85053-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="85053-242">Reportname</span><span class="sxs-lookup"><span data-stu-id="85053-242">ReportName</span></span>     |    <span data-ttu-id="85053-243">Yes</span><span class="sxs-lookup"><span data-stu-id="85053-243">Yes</span></span>     |    <span data-ttu-id="85053-244">Nazwa, która ma zostać przypisana do raportu</span><span class="sxs-lookup"><span data-stu-id="85053-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="85053-245">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-245">string</span></span>     |
|    <span data-ttu-id="85053-246">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-246">Description</span></span>     |    <span data-ttu-id="85053-247">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-247">No</span></span>     |    <span data-ttu-id="85053-248">Opis utworzonego raportu</span><span class="sxs-lookup"><span data-stu-id="85053-248">Description of the created report</span></span>     |    <span data-ttu-id="85053-249">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-249">string</span></span>     |
|    <span data-ttu-id="85053-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="85053-250">QueryId</span></span>     |    <span data-ttu-id="85053-251">Yes</span><span class="sxs-lookup"><span data-stu-id="85053-251">Yes</span></span>     |    <span data-ttu-id="85053-252">Identyfikator zapytania raportu</span><span class="sxs-lookup"><span data-stu-id="85053-252">Report query ID</span></span>     |    <span data-ttu-id="85053-253">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-253">string</span></span>     |
|    <span data-ttu-id="85053-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="85053-254">StartTime</span></span>     |    <span data-ttu-id="85053-255">Yes</span><span class="sxs-lookup"><span data-stu-id="85053-255">Yes</span></span>     |    <span data-ttu-id="85053-256">Znacznik czasu UTC, od którego rozpocznie się generowanie raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="85053-257">Format powinien być: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="85053-258">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-258">string</span></span>     |
|    <span data-ttu-id="85053-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="85053-259">ExecuteNow</span></span>     |    <span data-ttu-id="85053-260">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-260">No</span></span>     |    <span data-ttu-id="85053-261">Ten parametr powinien służyć do tworzenia raportu, który zostanie wykonany tylko raz.</span><span class="sxs-lookup"><span data-stu-id="85053-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="85053-262">`StartTime`, `RecurrenceInterval` i `RecurrenceCount` są ignorowane, jeśli jest ustawiona na wartość true.</span><span class="sxs-lookup"><span data-stu-id="85053-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="85053-263">Raport jest wykonywany natychmiast w sposób asynchroniczny</span><span class="sxs-lookup"><span data-stu-id="85053-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="85053-264">true/false</span><span class="sxs-lookup"><span data-stu-id="85053-264">true/false</span></span>     |
|    <span data-ttu-id="85053-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="85053-265">QueryStartTime</span></span>     |    <span data-ttu-id="85053-266">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-266">No</span></span>     |    <span data-ttu-id="85053-267">Opcjonalnie określa czas rozpoczęcia zapytania wyodrębniania danych.</span><span class="sxs-lookup"><span data-stu-id="85053-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="85053-268">Ten parametr ma zastosowanie tylko w przypadku raportu wykonania raz, dla których `ExecuteNow` ustawiono wartość true.</span><span class="sxs-lookup"><span data-stu-id="85053-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="85053-269">Ustawienie zastąpień tego `TIMESPAN` parametru podanych w zapytaniu.</span><span class="sxs-lookup"><span data-stu-id="85053-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="85053-270">Format powinien być yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="85053-271">Sygnatura czasowa jako ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="85053-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="85053-272">QueryEndTime</span></span>     |    <span data-ttu-id="85053-273">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-273">No</span></span>     |    <span data-ttu-id="85053-274">Opcjonalnie określa czas zakończenia zapytania wyodrębniania danych.</span><span class="sxs-lookup"><span data-stu-id="85053-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="85053-275">Ten parametr ma zastosowanie tylko w przypadku raportu wykonania raz, dla których `ExecuteNow` ustawiono wartość true.</span><span class="sxs-lookup"><span data-stu-id="85053-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="85053-276">Ustawienie zastąpień tego `TIMESPAN` parametru podanych w zapytaniu.</span><span class="sxs-lookup"><span data-stu-id="85053-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="85053-277">Format powinien być yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="85053-278">Sygnatura czasowa jako ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="85053-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="85053-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="85053-280">Yes</span><span class="sxs-lookup"><span data-stu-id="85053-280">Yes</span></span>     |    <span data-ttu-id="85053-281">Częstotliwość w godzinach, z jaką raport powinien zostać wygenerowany.</span><span class="sxs-lookup"><span data-stu-id="85053-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="85053-282">Wartość minimalna to 4, a wartość maksymalna to 2160.</span><span class="sxs-lookup"><span data-stu-id="85053-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="85053-283">liczba całkowita</span><span class="sxs-lookup"><span data-stu-id="85053-283">integer</span></span>     |
|    <span data-ttu-id="85053-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="85053-284">RecurrenceCount</span></span>     |    <span data-ttu-id="85053-285">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-285">No</span></span>     |    <span data-ttu-id="85053-286">Liczba raportów do wygenerowania.</span><span class="sxs-lookup"><span data-stu-id="85053-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="85053-287">liczba całkowita</span><span class="sxs-lookup"><span data-stu-id="85053-287">integer</span></span>     |
|    <span data-ttu-id="85053-288">Format</span><span class="sxs-lookup"><span data-stu-id="85053-288">Format</span></span>     |    <span data-ttu-id="85053-289">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-289">No</span></span>     |    <span data-ttu-id="85053-290">Format wyeksportowanego pliku.</span><span class="sxs-lookup"><span data-stu-id="85053-290">File format of the exported file.</span></span> <br> <span data-ttu-id="85053-291">Wartość domyślna to CSV.</span><span class="sxs-lookup"><span data-stu-id="85053-291">Default is CSV.</span></span>    |    <span data-ttu-id="85053-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="85053-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="85053-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="85053-293">CallbackUrl</span></span>     |    <span data-ttu-id="85053-294">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-294">No</span></span>     |    <span data-ttu-id="85053-295">Publicznie dostępny adres URL, który można opcjonalnie skonfigurować jako miejsce docelowe wywołania zwrotnego</span><span class="sxs-lookup"><span data-stu-id="85053-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="85053-296">Ciąg (adres URL HTTP)</span><span class="sxs-lookup"><span data-stu-id="85053-296">String (http URL)</span></span>     |
|    <span data-ttu-id="85053-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="85053-297">CallbackMethod</span></span>     |    <span data-ttu-id="85053-298">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-298">No</span></span>     |    <span data-ttu-id="85053-299">Metoda, która ma być używana do wywołania zwrotnego</span><span class="sxs-lookup"><span data-stu-id="85053-299">The method to be used for callback</span></span>     |    <span data-ttu-id="85053-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="85053-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="85053-301">Przykładowa odpowiedź</span><span class="sxs-lookup"><span data-stu-id="85053-301">Sample response</span></span>

<span data-ttu-id="85053-302">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="85053-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="85053-303">Kody odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="85053-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="85053-304">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="85053-304">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="85053-305">Słownik</span><span class="sxs-lookup"><span data-stu-id="85053-305">Glossary</span></span>

<span data-ttu-id="85053-306">Poniżej przedstawiono kluczowe definicje elementów w odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="85053-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="85053-307">Parametr</span><span class="sxs-lookup"><span data-stu-id="85053-307">Parameter</span></span>     |    <span data-ttu-id="85053-308">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="85053-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="85053-309">ReportId</span></span>     |    <span data-ttu-id="85053-310">Uniwersalnie unikatowy identyfikator (UUID) utworzonego raportu</span><span class="sxs-lookup"><span data-stu-id="85053-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="85053-311">Reportname</span><span class="sxs-lookup"><span data-stu-id="85053-311">ReportName</span></span>     |    <span data-ttu-id="85053-312">Nazwa nadana raportowi w ładunku żądania</span><span class="sxs-lookup"><span data-stu-id="85053-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="85053-313">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-313">Description</span></span>     |    <span data-ttu-id="85053-314">Opis podany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="85053-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="85053-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="85053-315">QueryId</span></span>     |    <span data-ttu-id="85053-316">Identyfikator zapytania przekazany w momencie utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="85053-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="85053-317">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="85053-317">Query</span></span>     |    <span data-ttu-id="85053-318">Tekst zapytania, który zostanie wykonany dla tego raportu</span><span class="sxs-lookup"><span data-stu-id="85053-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="85053-319">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="85053-319">User</span></span>     |    <span data-ttu-id="85053-320">Identyfikator użytkownika użyty do utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="85053-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="85053-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="85053-321">CreatedTime</span></span>     |    <span data-ttu-id="85053-322">Czas UTC utworzenia raportu w tym formacie: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="85053-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="85053-323">ModifiedTime</span></span>     |    <span data-ttu-id="85053-324">Czas UTC ostatniej modyfikacji raportu w tym formacie: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="85053-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="85053-325">ExecuteNow</span></span>     |    <span data-ttu-id="85053-326">`ExecuteNow` flaga ustawiona w czasie tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="85053-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="85053-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="85053-327">StartTime</span></span>     |    <span data-ttu-id="85053-328">Czas UTC rozpoczęcia wykonywania raportu w tym formacie: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="85053-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="85053-329">ReportStatus</span></span>     |    <span data-ttu-id="85053-330">Stan wykonania raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-330">Status of the report execution.</span></span> <span data-ttu-id="85053-331">Możliwe wartości to `Paused` , `Active` i `Inactive`</span><span class="sxs-lookup"><span data-stu-id="85053-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="85053-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="85053-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="85053-333">Interwał cyklu zapewniany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="85053-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="85053-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="85053-334">RecurrenceCount</span></span>     |    <span data-ttu-id="85053-335">Liczba cyklów zapewniana podczas tworzenia raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="85053-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="85053-336">CallbackUrl</span></span>     |    <span data-ttu-id="85053-337">Adres URL wywołania zwrotnego podany w żądaniu</span><span class="sxs-lookup"><span data-stu-id="85053-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="85053-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="85053-338">CallbackMethod</span></span>     |    <span data-ttu-id="85053-339">Metoda wywołania zwrotnego dostarczana w żądaniu</span><span class="sxs-lookup"><span data-stu-id="85053-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="85053-340">Format</span><span class="sxs-lookup"><span data-stu-id="85053-340">Format</span></span>     |    <span data-ttu-id="85053-341">Format plików raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-341">Format of the report files.</span></span> <span data-ttu-id="85053-342">Możliwe wartości to `CSV` lub `TSV` .</span><span class="sxs-lookup"><span data-stu-id="85053-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="85053-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="85053-343">TotalCount</span></span>     |    <span data-ttu-id="85053-344">Liczba rekordów w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="85053-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="85053-345">Statuscode</span><span class="sxs-lookup"><span data-stu-id="85053-345">StatusCode</span></span>     |    <span data-ttu-id="85053-346">Kod wyniku</span><span class="sxs-lookup"><span data-stu-id="85053-346">Result Code</span></span>     |
|    <span data-ttu-id="85053-347">message</span><span class="sxs-lookup"><span data-stu-id="85053-347">message</span></span>     |    <span data-ttu-id="85053-348">Możliwe wartości to 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="85053-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="85053-349">Komunikat o stanie z wykonywania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="85053-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="85053-350">Uzyskiwanie interfejsu API wykonywania raportu</span><span class="sxs-lookup"><span data-stu-id="85053-350">Get report execution API</span></span>

<span data-ttu-id="85053-351">Ta metoda umożliwia wykonywanie zapytań o stan wykonania raportu przy użyciu raportu otrzymywanego z interfejsu [API tworzenia raportu.](#create-report-api)</span><span class="sxs-lookup"><span data-stu-id="85053-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="85053-352">Metoda zwraca link pobierania raportu, jeśli raport jest gotowy do pobrania.</span><span class="sxs-lookup"><span data-stu-id="85053-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="85053-353">W przeciwnym razie metoda zwraca stan.</span><span class="sxs-lookup"><span data-stu-id="85053-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="85053-354">Ten interfejs API umożliwia również uzyskiwanie wszystkich wykonań, które miały miejsce dla danego raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="85053-355">Ten interfejs API ma domyślne parametry zapytania ustawione dla `executionStatus=Completed` i `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="85053-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="85053-356">W związku z tym wywołanie interfejsu API przed pierwszym pomyślnym wykonaniem raportu zwróci kod 404.</span><span class="sxs-lookup"><span data-stu-id="85053-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="85053-357">Oczekujące wykonania można uzyskać, ustawiając . `executionStatus=Pending`</span><span class="sxs-lookup"><span data-stu-id="85053-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="85053-358">Składnia żądania</span><span class="sxs-lookup"><span data-stu-id="85053-358">Request syntax</span></span>

|    <span data-ttu-id="85053-359">Metoda</span><span class="sxs-lookup"><span data-stu-id="85053-359">Method</span></span>     |    <span data-ttu-id="85053-360">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="85053-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="85053-361">GET</span><span class="sxs-lookup"><span data-stu-id="85053-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="85053-362">Nagłówek żądania</span><span class="sxs-lookup"><span data-stu-id="85053-362">Request header</span></span>

|    <span data-ttu-id="85053-363">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="85053-363">Header</span></span>     |    <span data-ttu-id="85053-364">Typ</span><span class="sxs-lookup"><span data-stu-id="85053-364">Type</span></span>     |    <span data-ttu-id="85053-365">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="85053-366">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="85053-366">Authorization</span></span>     |    <span data-ttu-id="85053-367">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-367">string</span></span> |<span data-ttu-id="85053-368">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="85053-368">Required.</span></span> <span data-ttu-id="85053-369">Token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="85053-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="85053-370">Format to  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="85053-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="85053-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85053-371">Content-Type</span></span>     |<span data-ttu-id="85053-372">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="85053-373">Parametr ścieżki</span><span class="sxs-lookup"><span data-stu-id="85053-373">Path parameter</span></span>

|    <span data-ttu-id="85053-374">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="85053-374">Parameter Name</span></span>    |    <span data-ttu-id="85053-375">Wymagany</span><span class="sxs-lookup"><span data-stu-id="85053-375">Required</span></span>    |    <span data-ttu-id="85053-376">Typ</span><span class="sxs-lookup"><span data-stu-id="85053-376">Type</span></span>    |    <span data-ttu-id="85053-377">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="85053-378">reportId</span><span class="sxs-lookup"><span data-stu-id="85053-378">reportId</span></span>    |    <span data-ttu-id="85053-379">Yes</span><span class="sxs-lookup"><span data-stu-id="85053-379">Yes</span></span>    |    <span data-ttu-id="85053-380">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-380">string</span></span>    |    <span data-ttu-id="85053-381">Filtruj, aby uzyskać szczegóły wykonywania tylko raportów z argumentem reportId podanym w tym argumentze.</span><span class="sxs-lookup"><span data-stu-id="85053-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="85053-382">Można określić wiele elementów reportId, oddzielając je średnikiem "; ".</span><span class="sxs-lookup"><span data-stu-id="85053-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="85053-383">Parametr zapytania</span><span class="sxs-lookup"><span data-stu-id="85053-383">Query parameter</span></span>

|    <span data-ttu-id="85053-384">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="85053-384">Parameter Name</span></span>    |    <span data-ttu-id="85053-385">Wymagany</span><span class="sxs-lookup"><span data-stu-id="85053-385">Required</span></span>    |    <span data-ttu-id="85053-386">Typ</span><span class="sxs-lookup"><span data-stu-id="85053-386">Type</span></span>    |    <span data-ttu-id="85053-387">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="85053-388">Executionid</span><span class="sxs-lookup"><span data-stu-id="85053-388">executionId</span></span>    |    <span data-ttu-id="85053-389">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-389">No</span></span>    |    <span data-ttu-id="85053-390">ciąg</span><span class="sxs-lookup"><span data-stu-id="85053-390">string</span></span>    |    <span data-ttu-id="85053-391">Filtruj, aby uzyskać szczegółowe informacje tylko o raportach z argumentem executionId podanym w tym argumentie.</span><span class="sxs-lookup"><span data-stu-id="85053-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="85053-392">Można określić wiele elementów executionId, oddzielając je średnikiem "; ".</span><span class="sxs-lookup"><span data-stu-id="85053-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="85053-393">Executionstatus</span><span class="sxs-lookup"><span data-stu-id="85053-393">executionStatus</span></span>    |    <span data-ttu-id="85053-394">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-394">No</span></span>    |    <span data-ttu-id="85053-395">Ciąg/wyli).</span><span class="sxs-lookup"><span data-stu-id="85053-395">String/enum</span></span>    |    <span data-ttu-id="85053-396">Filtruj, aby uzyskać szczegółowe informacje tylko o raportach z argumentem executionStatus podanym w tym argumentie.</span><span class="sxs-lookup"><span data-stu-id="85053-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="85053-397">Prawidłowe wartości to: `Pending` `Running` , i `Paused` `Completed` .</span><span class="sxs-lookup"><span data-stu-id="85053-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="85053-398">Wartość domyślna to `Completed`.</span><span class="sxs-lookup"><span data-stu-id="85053-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="85053-399">Wiele stanów można określić, oddzielając je średnikiem "; ".</span><span class="sxs-lookup"><span data-stu-id="85053-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="85053-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="85053-400">getLatestExecution</span></span>    |    <span data-ttu-id="85053-401">Nie</span><span class="sxs-lookup"><span data-stu-id="85053-401">No</span></span>    |    <span data-ttu-id="85053-402">boolean</span><span class="sxs-lookup"><span data-stu-id="85053-402">boolean</span></span>    |    <span data-ttu-id="85053-403">Interfejs API zwróci szczegóły najnowszego wykonania.</span><span class="sxs-lookup"><span data-stu-id="85053-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="85053-404">Domyślnie ten parametr ma wartość true.</span><span class="sxs-lookup"><span data-stu-id="85053-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="85053-405">Jeśli zdecydujesz się przekazać wartość tego parametru jako false, interfejs API zwróci wystąpienia wykonywania z ostatnich 90 dni.</span><span class="sxs-lookup"><span data-stu-id="85053-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="85053-406">Ładunek przykładowego żądania</span><span class="sxs-lookup"><span data-stu-id="85053-406">Sample Request Payload</span></span>

<span data-ttu-id="85053-407">Brak</span><span class="sxs-lookup"><span data-stu-id="85053-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="85053-408">Przykładowa odpowiedź</span><span class="sxs-lookup"><span data-stu-id="85053-408">Sample Response</span></span>

<span data-ttu-id="85053-409">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="85053-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="85053-410">Kody odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="85053-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="85053-411">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="85053-411">Response payload example:</span></span>

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

<span data-ttu-id="85053-412">Po zakończeniu wykonywania raportu zostanie pokazany `Completed` stan wykonywania.</span><span class="sxs-lookup"><span data-stu-id="85053-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="85053-413">Raport można pobrać, wybierając adres URL w polu `reportAccessSecureLink` .</span><span class="sxs-lookup"><span data-stu-id="85053-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="85053-414">Słownik</span><span class="sxs-lookup"><span data-stu-id="85053-414">Glossary</span></span>

<span data-ttu-id="85053-415">Kluczowe definicje elementów w odpowiedzi.</span><span class="sxs-lookup"><span data-stu-id="85053-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="85053-416">Parametr</span><span class="sxs-lookup"><span data-stu-id="85053-416">Parameter</span></span>    |    <span data-ttu-id="85053-417">Opis</span><span class="sxs-lookup"><span data-stu-id="85053-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="85053-418">Executionid</span><span class="sxs-lookup"><span data-stu-id="85053-418">ExecutionId</span></span>    |    <span data-ttu-id="85053-419">Unikatowy identyfikator wystąpienia wykonywania (UUID)</span><span class="sxs-lookup"><span data-stu-id="85053-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="85053-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="85053-420">ReportId</span></span>    |    <span data-ttu-id="85053-421">Identyfikator raportu skojarzony z wystąpieniem wykonywania</span><span class="sxs-lookup"><span data-stu-id="85053-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="85053-422">CyklInterval</span><span class="sxs-lookup"><span data-stu-id="85053-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="85053-423">Interwał cyklu zapewniany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="85053-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="85053-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="85053-424">RecurrenceCount</span></span>    |    <span data-ttu-id="85053-425">Liczba cyklów zapewniana podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="85053-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="85053-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="85053-426">CallbackUrl</span></span>    |    <span data-ttu-id="85053-427">Adres URL wywołania zwrotnego skojarzony z wystąpieniem wykonywania</span><span class="sxs-lookup"><span data-stu-id="85053-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="85053-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="85053-428">CallbackMethod</span></span>    |    <span data-ttu-id="85053-429">Metoda wywołania zwrotnego skojarzona z wystąpieniem wykonywania</span><span class="sxs-lookup"><span data-stu-id="85053-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="85053-430">Format</span><span class="sxs-lookup"><span data-stu-id="85053-430">Format</span></span>    |    <span data-ttu-id="85053-431">Format wygenerowanego pliku na końcu wykonywania</span><span class="sxs-lookup"><span data-stu-id="85053-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="85053-432">Executionstatus</span><span class="sxs-lookup"><span data-stu-id="85053-432">ExecutionStatus</span></span>    |    <span data-ttu-id="85053-433">Stan wystąpienia wykonywania raportu.</span><span class="sxs-lookup"><span data-stu-id="85053-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="85053-434">Prawidłowe wartości to: `Pending` , `Running` , `Paused` i `Completed`</span><span class="sxs-lookup"><span data-stu-id="85053-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="85053-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="85053-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="85053-436">Link, za pomocą którego można bezpiecznie uzyskać dostęp do raportu</span><span class="sxs-lookup"><span data-stu-id="85053-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="85053-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="85053-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="85053-438">Czas UTC, po którym link do raportu wygaśnie w tym formacie: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="85053-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="85053-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="85053-440">Czas UTC, o której raport został wygenerowany w tym formacie: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="85053-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="85053-441">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="85053-441">TotalCount</span></span>    |    <span data-ttu-id="85053-442">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="85053-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="85053-443">Statuscode</span><span class="sxs-lookup"><span data-stu-id="85053-443">StatusCode</span></span>    |    <span data-ttu-id="85053-444">Kod wyniku</span><span class="sxs-lookup"><span data-stu-id="85053-444">Result Code</span></span> <br> <span data-ttu-id="85053-445">Możliwe wartości to 200, 400, 401, 403, 404 i 500</span><span class="sxs-lookup"><span data-stu-id="85053-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="85053-446">message</span><span class="sxs-lookup"><span data-stu-id="85053-446">message</span></span>    |    <span data-ttu-id="85053-447">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="85053-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="85053-448">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="85053-448">Next steps</span></span>

- <span data-ttu-id="85053-449">Wypróbuj interfejsy API za pomocą adresu [URL interfejsu API swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="85053-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="85053-450">Pierwsze wywołanie interfejsu API</span><span class="sxs-lookup"><span data-stu-id="85053-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)