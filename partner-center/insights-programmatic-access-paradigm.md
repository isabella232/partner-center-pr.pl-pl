---
title: Paradygmat dostępu programowego dla danych szczegółowych informacji
description: Opis przepływu wysokiego poziomu wzorca wywołań interfejsu API dla analizy programowej. Interfejsy API służące do uzyskiwania dostępu do raportów analizy szczegółowych informacji partnerów są również objęte analizą.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 895b05f2beb8123d8b2cdc7ba43d559247b0c095ada7fddffa1bf554cfe5b233
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115687399"
---
# <a name="programmatic-access-paradigm"></a>Paradygmat dostępu programowego

Na tym diagramie przedstawiono wzorzec wywołania interfejsu API używany do tworzenia nowego szablonu raportu, planowania raportu niestandardowego i pobierania danych błędów.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Przepływ wysokiego poziomu":::
***Rysunek 1. Przepływ wysokiego poziomu wzorca wywołań interfejsu API***

Ta lista zawiera więcej szczegółów na temat rysunku 1.

1. Aplikacja kliencza może zdefiniować niestandardowy schemat/szablon raportu, wywołując [interfejs API tworzenia zapytania raportu.](#create-report-query-api) Alternatywnie możesz wybrać szablon raportu (QueryId) z przykładów biblioteki szablonów raportów wymienionych [tutaj.](insights-programmatic-system-queries.md)
2. W przypadku powodzenia interfejs API tworzenia zapytania raportu zwraca wartość QueryId.
3. Następnie aplikacja klienjąca musi wywołać interfejs [API](#create-report-api) tworzenia raportu przy użyciu parametru QueryId wraz z datą rozpoczęcia raportu, interwałem powtórzeń, cyklem i opcjonalnym URI wywołania zwrotnego.
4. W przypadku powodzenia interfejs [API tworzenia raportu](#create-report-api) zwraca wartość ReportId.
5. Aplikacja klienjąca jest powiadamiana pod adresem URL wywołania zwrotnego, gdy tylko dane raportu będą gotowe do pobrania.
6. Następnie aplikacja kliency używa interfejsu [API get report executions do](#get-report-execution-api) wykonywania zapytań o stan raportu przy użyciu identyfikatora raportu i zakresu dat.
7. W przypadku powodzenia jest zwracany link pobierania raportu, a aplikacja może zainicjować pobieranie danych.

## <a name="report-query-language-specification"></a>Specyfikacja języka zapytań raportów

Chociaż zapewniamy zapytania [systemowe, których](insights-programmatic-system-queries.md) można używać do tworzenia raportów, możesz również tworzyć własne zapytania w zależności od potrzeb biznesowych. Aby dowiedzieć się więcej na temat zapytań niestandardowych, zobacz [Custom Query Specification](insights-programmatic-custom-query.md).

## <a name="create-report-query-api"></a>Tworzenie interfejsu API zapytań raportu

Interfejs API ułatwia tworzenie zapytań niestandardowych, które definiują zestaw danych, z którego należy wyeksportować kolumny i metryki. Interfejs API zapewnia elastyczność tworzenia nowego szablonu raportowania w zależności od potrzeb biznesowych.  

Możesz również użyć zapytań [systemowych, które](insights-programmatic-system-queries.md) zapewniamy. Gdy niestandardowe szablony raportów nie są potrzebne, można wywołać interfejs [API](#create-report-api) tworzenia raportów bezpośrednio przy użyciu podanych zapytań systemowych QueryId.  

W poniższym przykładzie pokazano, jak utworzyć zapytanie niestandardowe, aby uzyskać 10 klientów z najlepszymi przychodami w ostatnim miesiącu.

### <a name="request-syntax"></a>Składnia żądania

|    Metoda     |    Identyfikator URI żądania     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Nagłówek żądania

|    Nagłówek     |    Typ     |    Opis     |
|-------|-----|------|
|    Autoryzacja     |    ciąg |Wymagane. Token Azure Active Directory (Azure AD). Format to  `Bearer <token>` .|
|    Content-Type     |ciąg |`Application/JSON` |
||||

### <a name="path-parameter"></a>Parametr ścieżki

Brak

### <a name="query-parameter"></a>Parametr zapytania

Brak

### <a name="sample-request-payload"></a>Ładunek przykładowego żądania

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Słownik

Ta tabela zawiera kluczowe definicje elementów w ładunku żądania.

|Parametr|    Wymagane     |    Opis     |    Dozwolone wartości     |
|-----|    -----    |    -----    |    -----    |
|Nazwa |    Tak     |    Przyjazna nazwa zapytania     |    ciąg     |
|    Opis     |    Nie     |    Opis danych zwracanych przez zapytanie     |    ciąg     |
|    Zapytanie     |    Tak     |    Ciąg zapytania raportu     |    Typ danych: ciąg <br> [Zapytanie niestandardowe oparte](insights-programmatic-custom-query.md) na potrzebach biznesowych |
|        |        |        |        |

> [!Note]
> Aby uzyskać przykłady zapytań niestandardowych, [zobacz Przykłady przykładowych zapytań.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Przykładowa odpowiedź

Ładunek odpowiedzi ma następującą strukturę:

Kody odpowiedzi: 200, 400, 401, 403, 500

Przykład ładunku odpowiedzi:

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

### <a name="glossary"></a>Słownik

Ta tabela zawiera kluczowe definicje elementów w ładunku żądania.

|    Parametr     |    Opis     |
|    ----    |    ----    |
|    QueryId     |    Unikatowy identyfikator (UUID) utworzonego zapytania     |
|    Nazwa     |    Przyjazna nazwa nadana zapytaniu w ładunku żądania     |
|    Opis     |    Opis podany podczas tworzenia zapytania     |
|    Zapytanie     |    Zapytanie raportu przekazane jako dane wejściowe podczas tworzenia zapytania     |
|    Typ     |    Ustaw wartość `userDefined`     |
|    Użytkownik     |    Identyfikator użytkownika użyty do utworzenia zapytania     |
|    CreatedTime     |    Czas UTC utworzenia zapytania w tym formacie: yyyy-MM-ddTHH:mm:ssZ     |
|    Łączna liczba     |    Liczba zestawów danych w tablicy Value     |
|    Statuscode     |    Kod wyniku <br> Możliwe wartości to 200, 400, 401, 403, 500     |
|    message     |    Komunikat o stanie z wykonania interfejsu API     |
|        |        |

## <a name="create-report-api"></a>Tworzenie interfejsu API raportu

Po pomyślnym utworzeniu niestandardowego szablonu raportu i [](#create-report-query-api) otrzymaniu pola QueryID w ramach odpowiedzi na zapytanie dotyczące raportu ten interfejs API może zostać wywołany w celu zaplanowania wykonywania zapytania w regularnych odstępach czasu. Można ustawić częstotliwość i harmonogram dostarczenia raportu.
W przypadku zapytań systemowych, które zapewniamy, interfejs API tworzenia raportu może być również wywoływany za pomocą [queryId](insights-programmatic-system-queries.md).

### <a name="callback-url"></a>Adres URL wywołania zwrotnego

Interfejs API tworzenia raportu akceptuje adres URL wywołania zwrotnego. Ten adres URL zostanie wywołany po pomyślnym zakończeniu generowania raportu. Adres URL wywołania zwrotnego powinien być publicznie dostępny. Oprócz adresu URL można również określić metodę wywołania zwrotnego. Metodą wywołania zwrotnego może być tylko "GET" lub "POST". Jeśli nie zostanie przekazana żadna wartość, domyślną metodą będzie "POST". Podczas wywołania zwrotnego zawsze zostanie przekazany raport reportId, który zakończył generowanie.

Wywołanie zwrotne POST: Jeśli przekazany adres URL to `https://www.contosso.com/callback` , wywołany zwrotny adres URL będzie miał 2000. `https://www.contosso.com/callback/<reportID>` 

Wywołanie zwrotne GET: jeśli przekazany adres URL to `https://www.contosso.com/callback` , wywołany zwrotny adres URL będzie miał 2000. `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>Raporty ExecuteNow

Istnieje aprowizowanie generowania raportu bez planowania. Ładunek interfejsu API tworzenia raportu może akceptować parametr , który będzie kolejkować raport do wygenerowania natychmiast po `ExecuteNow` wywołaniu interfejsu API. W `ExecuteNow` przypadku ustawienia wartości true pola , , są `StartTime` ignorowane, ponieważ te `RecurrenceCount` `RecurrenceInterval` raporty nie są zaplanowane.

W przypadku wartości true można dodać `ExecuteNow` dwa `QueryStartTime` dodatkowe pola: i `QueryEndTime` . Te dwa pola `TIMESPAN` zastąpią pole w zapytaniu. Te pola nie mają zastosowania do zaplanowanych raportów, ponieważ dane będą generowane w sposób ciągły przez ustalony czas, który nie zmienia się.

### <a name="request-syntax"></a>Składnia żądania

|    Metoda     |    Identyfikator URI żądania     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Nagłówek żądania

|    Nagłówek     |    Typ     |    Opis     |
|-------|-----|------|
|    Autoryzacja     |    ciąg |Wymagane. Token Azure Active Directory (Azure AD). Format to  `Bearer <token>` .|
|    Content-Type     |ciąg |`Application/JSON` |

### <a name="path-parameter"></a>Parametr ścieżki

Brak

### <a name="query-parameter"></a>Parametr zapytania

Brak

### <a name="sample-request-payload"></a>Ładunek przykładowego żądania

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

### <a name="glossary"></a>Słownik

Poniżej przedstawiono kluczowe definicje elementów ładunku żądania:

|    Parametr     |    Wymagane     |    Opis     |    Dozwolone wartości     |
|    ----    |    ----    |    ----    |    ----    |
|    Reportname     |    Tak     |    Nazwa, która ma zostać przypisana do raportu     |    ciąg     |
|    Opis     |    Nie     |    Opis utworzonego raportu     |    ciąg     |
|    QueryId     |    Tak     |    Identyfikator zapytania raportu     |    ciąg     |
|    StartTime     |    Tak     |    Znacznik czasu UTC, od którego rozpocznie się generowanie raportu. <br> Format powinien być: yyyy-MM-ddTHH:mm:ssZ       |    ciąg     |
|    ExecuteNow     |    Nie     |    Ten parametr powinien służyć do tworzenia raportu, który zostanie wykonany tylko raz. `StartTime`, `RecurrenceInterval` i `RecurrenceCount` są ignorowane, jeśli jest ustawiona na wartość true. Raport jest wykonywany natychmiast w sposób asynchroniczny     |    true/false     |
|    QueryStartTime     |    Nie     |    Opcjonalnie określa czas rozpoczęcia dla zapytania wyodrębniania danych. Ten parametr ma zastosowanie tylko w przypadku raportu wykonania raz, dla których `ExecuteNow` ustawiono wartość true. Ustawienie tego parametru zastępuje `TIMESPAN` podane w zapytaniu. Format powinien być yyyy-MM-ddTHH:mm:ssZ     |    Sygnatura czasowa jako ciąg     |
|    QueryEndTime     |    Nie     |    Opcjonalnie określa czas zakończenia zapytania wyodrębniania danych. Ten parametr ma zastosowanie tylko w przypadku raportu wykonania raz, dla których `ExecuteNow` ustawiono wartość true. Ustawienie tego parametru zastępuje `TIMESPAN` podane w zapytaniu. Format powinien być yyyy-MM-ddTHH:mm:ssZ     |    Sygnatura czasowa jako ciąg     |
|    RecurrenceInterval     |    Tak     |    Częstotliwość w godzinach, z jaką powinien zostać wygenerowany raport. <br> Wartość minimalna to 4, a wartość maksymalna to 2160.      |    liczba całkowita     |
|    RecurrenceCount     |    Nie     |    Liczba raportów do wygenerowania.     |    liczba całkowita     |
|    Format     |    Nie     |    Format wyeksportowanego pliku. <br> Wartość domyślna to CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    Nie     |    Publicznie dostępny adres URL, który można opcjonalnie skonfigurować jako miejsce docelowe wywołania zwrotnego     |    Ciąg (adres URL HTTP)     |
|    CallbackMethod     |    Nie     |    Metoda, która ma być używana do wywołania zwrotnego     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Przykładowa odpowiedź

Ładunek odpowiedzi ma następującą strukturę:

Kody odpowiedzi: 200, 400, 401, 403, 404, 500

Przykład ładunku odpowiedzi:

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

### <a name="glossary"></a>Słownik

Poniżej przedstawiono kluczowe definicje elementów w odpowiedzi:

|    Parametr     |    Opis     |
|    ----    |    ----    |
|    ReportId     |    Uniwersalnie unikatowy identyfikator (UUID) utworzonego raportu     |
|    Reportname     |    Nazwa nadana raportowi w ładunku żądania     |
|    Opis     |    Opis podany podczas tworzenia raportu     |
|    QueryId     |    Identyfikator zapytania przekazany w momencie utworzenia raportu     |
|    Zapytanie     |    Tekst zapytania, który zostanie wykonany dla tego raportu     |
|    Użytkownik     |    Identyfikator użytkownika użyty do utworzenia raportu     |
|    CreatedTime     |    Czas UTC utworzenia raportu w tym formacie: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Czas UTC ostatniej modyfikacji raportu w tym formacie: yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` flaga ustawiona w czasie tworzenia raportu     |
|    StartTime     |    Czas UTC rozpoczęcia wykonywania raportu w tym formacie: yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Stan wykonania raportu. Możliwe wartości to `Paused` , `Active` i `Inactive`     |
|    RecurrenceInterval     |    Interwał cyklu zapewniany podczas tworzenia raportu     |
|    RecurrenceCount     |    Liczba cyklów zapewniana podczas tworzenia raportu.      |
|    CallbackUrl     |    Adres URL wywołania zwrotnego podany w żądaniu     |
|    CallbackMethod     |    Metoda wywołania zwrotnego dostarczana w żądaniu     |
|    Format     |    Format plików raportu. Możliwe wartości to `CSV` lub `TSV` .     |
|    TotalCount     |    Liczba rekordów w tablicy Value     |
|    Statuscode     |    Kod wyniku     |
|    message     |    Możliwe wartości to 200, 400, 401, 403, 500. Komunikat o stanie z wykonywania interfejsu API     |
|        |        |

## <a name="get-report-execution-api"></a>Uzyskiwanie interfejsu API wykonywania raportu

Ta metoda umożliwia wykonywanie zapytań o stan wykonania raportu przy użyciu raportu otrzymywanego z interfejsu [API tworzenia raportu.](#create-report-api) Metoda zwraca link pobierania raportu, jeśli raport jest gotowy do pobrania. W przeciwnym razie metoda zwraca stan. Ten interfejs API umożliwia również uzyskiwanie wszystkich wykonań, które miały miejsce dla danego raportu.  

>[!IMPORTANT]
>Ten interfejs API ma domyślne parametry zapytania ustawione dla `executionStatus=Completed` i `getLatestExecution=true` . W związku z tym wywołanie interfejsu API przed pierwszym pomyślnym wykonaniem raportu zwróci kod 404. Oczekujące wykonania można uzyskać, ustawiając . `executionStatus=Pending`

### <a name="request-syntax"></a>Składnia żądania

|    Metoda     |    Identyfikator URI żądania     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Nagłówek żądania

|    Nagłówek     |    Typ     |    Opis     |
|-------|-----|------|
|    Autoryzacja     |    ciąg |Wymagane. Token Azure Active Directory (Azure AD). Format to  `Bearer <token>` .|
|    Content-Type     |ciąg |`Application/JSON` |

### <a name="path-parameter"></a>Parametr ścieżki

|    Nazwa parametru    |    Wymagany    |    Typ    |    Opis    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Tak    |    ciąg    |    Filtruj, aby uzyskać szczegóły wykonywania tylko raportów z argumentem reportId podanym w tym argumentze. Można określić wiele elementów reportId, oddzielając je średnikiem "; ".    |
|        |        |        |        |

### <a name="query-parameter"></a>Parametr zapytania

|    Nazwa parametru    |    Wymagany    |    Typ    |    Opis    |
|    ----    |    ----    |    ----    |    ----    |
|    Executionid    |    Nie    |    ciąg    |    Filtruj, aby uzyskać szczegółowe informacje tylko o raportach z argumentem executionId podanym w tym argumentie. Można określić wiele elementów executionId, oddzielając je średnikiem "; ".    |
|    Executionstatus    |    Nie    |    Ciąg/wyli).    |    Filtruj, aby uzyskać szczegółowe informacje tylko o raportach z argumentem executionStatus podanym w tym argumentie. <br> Prawidłowe wartości to: `Pending` `Running` , i `Paused` `Completed` . <br> Wartość domyślna to `Completed`. <br> Wiele stanów można określić, oddzielając je średnikiem "; ".    |
|    getLatestExecution    |    Nie    |    boolean    |    Interfejs API zwróci szczegóły najnowszego wykonania. Domyślnie ten parametr ma wartość true.<br> Jeśli zdecydujesz się przekazać wartość tego parametru jako false, interfejs API zwróci wystąpienia wykonania z ostatnich 90 dni.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Ładunek przykładowego żądania

Brak

### <a name="sample-response"></a>Przykładowa odpowiedź

Ładunek odpowiedzi ma następującą strukturę:

Kody odpowiedzi: 200, 400, 401, 403, 404, 500

Przykład ładunku odpowiedzi:

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

Po zakończeniu wykonywania raportu zostanie pokazany `Completed` stan wykonania. Raport można pobrać, wybierając adres URL w pliku `reportAccessSecureLink` .

### <a name="glossary"></a>Słownik

Kluczowe definicje elementów w odpowiedzi.

|    Parametr    |    Opis    |
|    ----    |    ----    |
|    Executionid    |    Uniwersalnie unikatowy identyfikator (UUID) wystąpienia wykonywania    |
|    ReportId    |    Identyfikator raportu skojarzony z wystąpieniem wykonywania    |
|    RecurrenceInterval    |    Interwał cyklu zapewniany podczas tworzenia raportu    |
|    RecurrenceCount    |    Liczba cyklów zapewniana podczas tworzenia raportu    |
|    CallbackUrl    |    Adres URL wywołania zwrotnego skojarzony z wystąpieniem wykonywania    |
|    CallbackMethod    |    Metoda wywołania zwrotnego skojarzona z wystąpieniem wykonywania    |
|    Format    |    Format wygenerowanego pliku na końcu wykonywania    |
|    Executionstatus    |    Stan wystąpienia wykonywania raportu. <br> Prawidłowe wartości to: `Pending` `Running` , , `Paused` i `Completed`    |
|    ReportAccessSecureLink    |Link, za pomocą którego można bezpiecznie uzyskiwać dostęp do raportu        |
|    ReportExpiryTime    |    Czas UTC, po którym link do raportu wygaśnie w tym formacie: yyyy-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime    |    Czas UTC, o której raport został wygenerowany w tym formacie: yyyy-MM-ddTHH:mm:ssZ    |
|    TotalCount    |    Liczba zestawów danych w tablicy Value    |
|    Statuscode    |    Kod wyniku <br> Możliwe wartości to 200, 400, 401, 403, 404 i 500    |
|    message    |    Komunikat o stanie z wykonywania interfejsu API    |
|        |        |

## <a name="next-steps"></a>Następne kroki

- Wypróbuj interfejsy API za pomocą adresu [URL interfejsu API swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Pierwsze wywołanie interfejsu API](insights-programmatic-first-api-call.md)