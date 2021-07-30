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
ms.openlocfilehash: f755bc13ff4e0c4bc3a2c6ceda123c6a2bc47dc5
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836391"
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
|    queryId     |    ciąg     |    Nie    |    Filtrowanie w celu uzyskania szczegółów dotyczących tylko zapytań o identyfikatorze podanym w argumentze     |
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
|    Zapytanie     |    Ciąg zapytania raportu usuniętego zapytania    |
|    Typ     |    Ustaw wartość userDefined dla zapytań utworzonych przez użytkownika     |
|    Użytkownik     |    Identyfikator użytkownika, który utworzył zapytanie     |
|    CreatedTime     |    Czas utworzenia zapytania     |
|    TotalCount     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonywania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |
