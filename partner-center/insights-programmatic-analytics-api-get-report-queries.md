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
ms.openlocfilehash: 943eea26a08f1072b6ddcaf8136b7f9f757d52b8c0170f03519b8787c1877bd3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115695190"
---
# <a name="get-report-queries-api"></a>Get report queries API

Interfejs API Pobierz zapytania dotyczące raportów pobiera wszystkie zapytania, które są dostępne do użycia w raportach. Domyślnie pobiera wszystkie zapytania systemowe i zdefiniowane przez użytkownika.

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
|    queryId     |    ciąg     |    Nie    |    Filtrowanie w celu uzyskania szczegółów dotyczących tylko zapytań o identyfikatorze podanym w argumentze     |
|    nazwa_zapytania     |    ciąg     |    Nie    |    Filtrowanie w celu uzyskania szczegółów dotyczących tylko zapytań o nazwie podanej w argumentie     |
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
|    TotalCount     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonywania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |
