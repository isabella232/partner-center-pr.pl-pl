---
title: Wypróbuj interfejs API zapytań dotyczących raportów
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Ten interfejs API umożliwia przetestowanie zapytania i zweryfikowanie wyników w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c83b56b7d52e0b9feb598597b4a8e1fdaec98a3b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845605"
---
# <a name="try-report-queries-api"></a>Wypróbuj interfejs API zapytań dotyczących raportów

Ten interfejs API wykonuje instrukcje zapytania raportu. Interfejs API zwraca tylko 100 rekordów, których partner może użyć do sprawdzenia, czy dane są zgodnie z oczekiwaniami.

> [!IMPORTANT]
> Ten interfejs API ma limit czasu wykonywania zapytania 100 sekund. Jeśli zauważysz, że interfejs API trwa dłużej niż 100 sekund, istnieje duże prawdopodobieństwo, że zapytanie ma poprawną synaktywną odpowiedź. W innym przypadku zostanie odebrany kod błędu inny niż 200. Rzeczywiste generowanie raportu przebiegnie, jeśli składnia zapytania jest poprawna.

**Składnia żądania**

|    Metoda    |    Identyfikator URI żądania    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
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
|    exportQuery     |    ciąg    |    Nie    |    Ciąg zapytania raportu, który musi zostać wykonany     |
|    queryId     |    ciąg    |    Nie    |    Prawidłowy istniejący identyfikator zapytania. Wzajemnie wykluczają się z ciągiem zapytania określonym w parametrze exportQuery    |
|    startTime     |    ciąg    |    Nie    |    Godzina rozpoczęcia, z której chcemy uzyskać dane. Zastępuje on okres określony w zapytaniu    |
|    endTime     |    ciąg    |    Nie    |    Czas zakończenia, do którego chcemy uzyskać dane. Zastępuje on okres określony w zapytaniu    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    TotalCount     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonywania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |
