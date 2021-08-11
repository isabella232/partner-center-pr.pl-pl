---
title: Interfejs API pobierz wszystkie zestawy danych — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Ten interfejs API umożliwia uzyskiwanie szczegółowych informacji o wszystkich dostępnych zestawach danych Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 96bbb039c022d3587183b8dbec014bc362255b750ac6670fe3c1906629b7e291
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693337"
---
# <a name="get-all-datasets-api"></a>Interfejs API pobierz wszystkie zestawy danych

Interfejs API Pobierz wszystkie zestawy danych pobiera wszystkie dostępne zestawy danych. Zestawy danych zawierają listę tabel, kolumn, metryk i zakresów czasu.

**Składnia żądania**

|    Metoda    |    Identyfikator URI żądania    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    Datasetname    |    ciąg    |    Nie    |    Filtrowanie w celu uzyskania szczegółów tylko jednego zestawu danych    |
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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Słownik**

W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:

|    Parametr    |    Opis    |
|    ----    |    ----    |
|    Datasetname     |    Nazwa zestawu danych, który definiuje ten obiekt tablicy     |
|    SelectableColumns     |    Nieprzetworzone kolumny, które można określić w wybranych kolumnach     |
|    AvailableMetrics     |    Nazwy kolumn agregacji/metryk, które można określić w wybranych kolumnach     |
|    AvailableDateRanges     |    Zakres dat, który może być używany w zapytaniach raportu dla zestawu danych     |
|    minimumRecurrenceInterval     |    Minimalna wartość interwału cyklu     |
|    TotalCount     |    Liczba zestawów danych w tablicy Value     |
|    Komunikat     |    Komunikat o stanie z wykonywania interfejsu API     |
|    Statuscode     |    Kod wyniku. Możliwe wartości to 200, 400, 401, 403, 500     |
|        |        |
