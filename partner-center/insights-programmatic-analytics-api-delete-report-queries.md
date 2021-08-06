---
title: Interfejs API usuwania zapytań dotyczących raportów — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Użyj tego interfejsu API, aby usunąć zapytanie zdefiniowane przez użytkownika w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 4714d523ff9942838e9666fe75f3df21aae69e043b6d9be1e1819cbd52dfb6ff
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681658"
---
# <a name="delete-report-queries-api"></a>Interfejs API usuwania zapytań dotyczących raportów

Ten interfejs API usuwa zapytania zdefiniowane przez użytkownika.

**Składnia żądania**

|    Metoda    |    Identyfikator URI żądania    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
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
|    queryId     |    ciąg     |    Nie    |    Filtrowanie w celu uzyskania szczegółów tylko zapytań o identyfikatorze podanym w argumentze     |
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
|    QueryId     |    Unikatowy identyfikator UUID zapytania, które zostało usunięte    |
|    Nazwa     |    Nazwa zapytania, które zostało usunięte    |
|    Opis     |    Opis usuniętego zapytania     |
|    Zapytanie     |    Ciąg zapytania raportu dla usuniętego zapytania    |
|    Typ     |    Ustaw wartość userDefined dla zapytań utworzonych przez użytkownika     |
|    Użytkownik     |    Identyfikator użytkownika, który utworzył zapytanie     |
|    CreatedTime     |    Czas utworzenia zapytania     |
|    Łączna liczba     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |
