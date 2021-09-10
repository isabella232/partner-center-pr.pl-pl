---
title: Uzyskiwanie interfejsu API raportów — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Ten interfejs API umożliwia uzyskiwanie wszystkich dostępnych identyfikatorów raportów w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: dc0e3925aeb07adc0e2b38af2913c63d3183941e
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959050"
---
# <a name="get-report-api"></a>Uzyskiwanie interfejsu API raportu

Ten interfejs API pobiera wszystkie raporty, które zostały zaplanowane.

**Składnia żądania**

|    Metoda    |    Identyfikator URI żądania    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

**Nagłówek żądania**

|    Nagłówek    |    Typ    |    Opis    |
|    ----    |    ----    |    ----    |
|    Autoryzacja    |    ciąg    |    Wymagane. Token Azure Active Directory (AAD) w formularzu`Bearer <token>`    |
|    Content-Type    |    ciąg    |    `Application/JSON`    |
|        |        |        |

**Parametr ścieżki**

Brak

**Parametr zapytania**

|    Nazwa parametru    |    Typ    |    Wymagane    |    Opis    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    ciąg    |    Nie    |    Filtruj, aby uzyskać szczegółowe informacje tylko o raportach z argumentem reportId podanym w tym argumentie     |
|    Reportname     |    ciąg    |    Nie    |    Filtruj, aby uzyskać szczegółowe informacje tylko o raportach z parametrem reportName podaną w tym argumentie     |
|    queryId     |    ciąg    |    Nie    |    Filtruj, aby uzyskać szczegółowe informacje tylko o raportach z argumentem queryId podanym w tym argumentze     |
|        |        |        |        |


**Ładunek żądania**

Brak

**Słownik**

Brak

**Odpowiedź**

Ładunek odpowiedzi ma następującą strukturę:

Kod odpowiedzi: 200, 400, 401, 403, 404, 500

Przykład ładunku odpowiedzi:

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**Słownik**

W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:

|    Parametr    |    Opis    |
|    ----    |    ----    |
|    ReportId     |    Unikatowy identyfikator UUID utworzonego raportu     |
|    Reportname     |    Nazwa nadana raportowi w ładunku żądania     |
|    Opis     |    Opis podany podczas tworzenia raportu     |
|    QueryId     |    Identyfikator zapytania przekazany podczas tworzenia raportu     |
|    Zapytanie     |    Tekst zapytania, który zostanie wykonany dla tego raportu     |
|    Użytkownik     |    Identyfikator użytkownika użyty do utworzenia raportu     |
|    CreatedTime     |    Godzina utworzenia raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Godzina ostatniej modyfikacji raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
|    executeNow     |    Flaga ExecuteNow ustawiona w czasie tworzenia raportu    |
|    StartTime     |    Rozpocznie się wykonywanie czasu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Stan wykonania raportu. Możliwe wartości to Wstrzymane, Aktywne i Nieaktywne.     |
|    RecurrenceInterval     |    Interwał cyklu zapewniany podczas tworzenia raportu     |
|    RecurrenceCount     |    Liczba cyklów zapewniana podczas tworzenia raportu     |
|    CallbackUrl     |    Adres URL wywołania zwrotnego podany w żądaniu     |
|    CallbackMethod    |    Metoda wywołania zwrotnego dostarczana w żądaniu    |
|    Format     |    Format plików raportu     |
|    TotalCount     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonywania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |