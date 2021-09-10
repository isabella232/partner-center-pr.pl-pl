---
title: Interfejs API pobierz zapytania dotyczące raportów — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Ten interfejs API umożliwia uzyskiwanie wszystkich dostępnych zapytań do użycia w interfejsie API raportów.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 5f65784ce93350c92e0ffe38849ce505f045e0b0
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959062"
---
# <a name="get-report-queries-api"></a>Interfejs API zapytań dotyczących raportów

Interfejs API get report queries pobiera wszystkie zapytania, które są dostępne do użycia w raportach. Domyślnie pobiera wszystkie zapytania systemowe i zdefiniowane przez użytkownika.

**Składnia żądania**

|    Metoda    |    Identyfikator URI żądania    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    queryId     |    ciąg     |    Nie    |    Filtrowanie w celu uzyskania szczegółów tylko zapytań o identyfikatorze podanym w argumentze     |
|    nazwa_zapytania     |    ciąg     |    Nie    |    Filtrowanie w celu uzyskania szczegółów tylko zapytań o nazwie podanej w argumentze     |
|    IncludeSystemQueries     |    boolean     |    Nie    |    Uwzględnianie wstępnie zdefiniowanych zapytań systemowych w odpowiedzi     |
|    IncludeOnlySystemQueries     |    boolean     |    Nie    |    Uwzględnianie w odpowiedzi tylko zapytań systemowych     |
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
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
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
|    QueryId     |    Unikatowy identyfikator UUID zapytania     |
|    Nazwa     |    Nazwa nadana zapytaniu w czasie tworzenia zapytania     |
|    Opis     |    Opis podany podczas tworzenia zapytania     |
|    Zapytanie     |    Ciąg zapytania raportu     |
|    Typ     |    Ustaw wartość userDefined dla zapytań utworzonych przez użytkownika i systemu dla wstępnie zdefiniowanych zapytań systemowych     |
|    Użytkownik     |    Identyfikator użytkownika, który utworzył zapytanie     |
|    CreatedTime     |    Czas utworzenia zapytania     |
|    Łączna liczba     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |
