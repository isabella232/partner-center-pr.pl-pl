---
title: Aktualizowanie interfejsu API raportu
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Ten interfejs API umożliwia aktualizowanie parametrów raportu w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c4425f6444603852e87d9287db720ec1b29ee57818bc949c82eed2179ac6149e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696918"
---
# <a name="update-report-api"></a>Aktualizowanie interfejsu API raportu

Ten interfejs API ułatwia modyfikowanie parametru raportu.

**Składnia żądania**

|    Metoda    |    Identyfikator URI żądania    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Nagłówek żądania**

|    Nagłówek    |    Typ    |    Opis    |
|    ----    |    ----    |    ----    |
|    Autoryzacja    |    ciąg    |    Wymagane. Token Azure Active Directory (AAD) w formularzu`Bearer <token>`    |
|    Content-Type    |    ciąg    |    `Application/JSON`    |
|        |        |        |

**Parametr ścieżki**

|    Nazwa parametru    |    Typ    |    Wymagane    |    Opis    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    ciąg    |    Nie    |    Identyfikator modyfikowanego raportu     |
|        |        |        |        |

**Parametr zapytania**

Brak

**Ładunek żądania**

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**Słownik**

W tej tabeli wymieniono kluczowe definicje elementów w odpowiedzi.

|    Parametr    |    Wymagane    |    Opis    |    Dozwolone wartości    |
|    ----    |    ----    |    ----    |    ----    |
|    Reportname     |    Tak     |    Nazwa, która ma zostać przypisana do raportu     |    Ciąg     |
|    Opis     |    Nie     |    Opis utworzonego raportu     |    Ciąg     |
|    StartTime     |    Tak    |    Znacznik czasu, po którym rozpocznie się generowanie raportu     |    Ciąg     |
|    RecurrenceInterval     |    Nie     |    Częstotliwość, z jaką raport powinien być generowany w godzinach. Wartość minimalna to 4     |    Liczba całkowita     |
|    RecurrenceCount     |    Nie     |    Liczba raportów do wygenerowania. Wartość domyślna to nieokreślony.     |    Liczba całkowita     |
|    Format     |    Nie    |    Format wyeksportowanego pliku. Wartość domyślna to CSV     |    CSV/TSV     |
|    CallbackURL     |    Nie     |    Adres URL wywołania zwrotnego HTTPS, który ma być wywoływany podczas generowania raportu     |    Ciąg     |
|    CallbackMethod    |    Nie    |    Metoda HTTP do wywołania zwrotnego    |    GET/POST    |
|        |        |        |        |


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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

**Słownik**

W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:

|    Parametr    |    Opis    |
|    ----    |    ----    |
|    ReportId     |    Uniwersalny unikatowy identyfikator (UUID) aktualizowanego raportu     |
|    Reportname     |    Nazwa nadana raportowi w ładunku żądania     |
|    Opis     |    Opis podany w raporcie w ładunku żądania     |
|    QueryId     |    Identyfikator zapytania przekazany w momencie utworzenia raportu     |
|    Zapytanie     |    Tekst zapytania, który zostanie wykonany dla tego raportu     |
|    Użytkownik     |    Identyfikator użytkownika użyty do utworzenia raportu     |
|    CreatedTime     |    Godzina utworzenia raportu. Format godziny to yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Godzina ostatniej modyfikacji raportu. Format godziny to yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    Flaga ExecuteNow ustawiona w czasie tworzenia raportu    |
|    StartTime     |    Czas rozpoczęcia wykonywania raportu. Format godziny to yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Stan wykonania raportu. Możliwe wartości to Wstrzymane, Aktywne i Nieaktywne.     |
|    RecurrenceInterval     |    Interwał cyklu podany w ładunku żądania     |
|    RecurrenceCount     |    Liczba cyklów podana w ładunku żądania     |
|    CallbackUrl     |    Adres URL wywołania zwrotnego podany w żądaniu     |
|    CallbackMethod    |    Metoda wywołania zwrotnego podana w żądaniu    |
|    Format     |    Format plików raportu     |
|    Łączna liczba     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |