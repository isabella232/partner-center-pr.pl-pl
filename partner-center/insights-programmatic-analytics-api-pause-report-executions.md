---
title: Wstrzymywanie interfejsu API wykonywania raportu — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Ten interfejs API umożliwia wstrzymanie wykonywania dowolnego raportu w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 798c5e87a3935923bd91d8e74716999fb8be4f54
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836374"
---
# <a name="pause-report-executions-api"></a>Interfejs API wstrzymywania wykonywania raportów

Po wykonaniu ten interfejs API wstrzymuje zaplanowane wykonywanie raportów.

**Składnia żądania**

|    Metoda    |    Identyfikator URI żądania    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
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
|    ReportId     |    Uniwersalny unikatowy identyfikator (UUID) wstrzymanego raportu     |
|    Reportname     |    Nazwa nadana raportowi podczas tworzenia     |
|    Opis     |    Opis podany podczas tworzenia raportu     |
|    QueryId     |    Identyfikator zapytania przekazany w momencie utworzenia raportu     |
|    Zapytanie     |    Tekst zapytania, który zostanie wykonany dla tego raportu     |
|    Użytkownik     |    Identyfikator użytkownika użyty do utworzenia raportu     |
|    CreatedTime     |    Godzina utworzenia raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Godzina ostatniej modyfikacji raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    Flaga ExecuteNow ustawiona w czasie tworzenia raportu     |
|    StartTime     |    Godzina rozpoczęcia wykonywania raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
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
