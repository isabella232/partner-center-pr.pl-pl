---
title: Wstrzymywanie interfejsu API wykonywania raportu — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ten interfejs API umożliwia wstrzymanie wykonywania dowolnego raportu w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377200"
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
|    QueryId     |    Identyfikator zapytania przekazany podczas tworzenia raportu     |
|    Zapytanie     |    Tekst zapytania, który zostanie wykonany dla tego raportu     |
|    Użytkownik     |    Identyfikator użytkownika użyty do utworzenia raportu     |
|    CreatedTime     |    Godzina utworzenia raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Godzina ostatniej modyfikacji raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    Flaga ExecuteNow ustawiona w czasie tworzenia raportu     |
|    StartTime     |    Czas rozpoczęcia wykonywania raportu. Format czasu to yyyy-MM-ddTHH:mm:ssZ     |
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
