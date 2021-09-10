---
title: Typowe pytania dotyczące dostępu programowego do usługi Partner Insights
description: Uzyskaj odpowiedzi na często zadawane pytania dotyczące uzyskiwania dostępu do danych szczegółowych informacji partnerów za pośrednictwem interfejsu API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 418af23ae50e1f8d9086b2eb6247ba964e4c1516
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959654"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Często zadawane pytania dotyczące dostępu programistycznego do danych analizy

W tym artykule opisano często zadawane pytania dotyczące programowego uzyskiwania dostępu do danych szczegółowych informacji partnerów w Partner Center.

## <a name="api-responses"></a>Odpowiedzi interfejsu API

Jakie są różne scenariusze, w których mogę otrzymać odpowiedź interfejsu API inną niż 200 (Powodzenie)?

W tej tabeli opisano odpowiedzi interfejsu API oraz działania, które należy wykonać w przypadku ich otrzymania.

|    Opis błędu     |    Kod błędu     |    Rozwiązywanie problemów     |
|    ----    |    ----    |    ----    |
|    Brak autoryzacji     |    401     |    Jest to wyjątek uwierzytelniania. Sprawdź poprawność tokenu Azure Active Directory (AAD). Token usługi AAD jest ważny przez 60 minut. Po upływie tego czasu konieczne będzie ponowne wygenerowanie tokenu usługi AAD.     |
|    Nieprawidłowa nazwa tabeli     |    400     |    Nazwa zestawu danych jest nieprawidłowa. Ponownie sprawdź nazwę zestawu danych, wywołując interfejs API "Pobierz wszystkie zestawy danych".     |
|    Nieprawidłowa nazwa kolumny     |    400     |    Nazwa kolumny w zapytaniu jest niepoprawna. Ponownie sprawdź nazwę kolumny, wywołując interfejs API "Pobierz wszystkie zestawy danych" lub odwołując się do nazw kolumn w definicjach danych    |
|    Wartość null lub brakująca wartość     |    400     |    W ładunku żądania interfejsu API może brakować obowiązkowych parametrów.     |
|    Nieprawidłowe parametry raportu     |    400     |    Upewnij się, że parametry raportu są poprawne. Na przykład wartość parametru RecurrenceInterval może być mniejsza niż 4.     |
|    Interwał cyklu musi być z zakresu od 4 do 2160     |    400     |    Upewnij się, że wartość parametru żądania RecurrenceInterval wynosi od 4 do 2160.     |
|    Nieprawidłowy identyfikator QueryId     |    400     |    Ponownie sprawdź wygenerowany kod QueryId.     |
|    Nieprawidłowe parametry raportu do utworzenia — czas rozpoczęcia raportu powinien być co najmniej 4 godziny od bieżącego czasu UTC     |    400     |    Parametr Godzina rozpoczęcia jako część ładunku żądania nie powinien być w przeszłości. Godzina rozpoczęcia raportu powinna być co najmniej 4 godziny od bieżącego czasu UTC.     |
|    Nie znaleziono żądanej wartości "string"     |    400     |    Sprawdź, czy zaktualizowano parametry lub `callbackurl` format żądania.     |
|    Nie znaleziono elementu z danym filtrem.     |    404     |    Sprawdź parametr reportID używany w interfejsie API get report executions.     |
|    Nie ma żadnych wykonań, które wystąpiły dla danego warunków filtru. Sprawdź dwukrotnie pole reportId lub executionId i ponów próbę interfejsu API po zaplanowanym czasie wykonywania raportu     |    404     |    Upewnij się, że reportId jest poprawny. Ponów próbę interfejsu API po zaplanowanym czasie wykonywania raportu określonym w ładunku żądania.     |
|    Wystąpił błąd wewnętrzny podczas tworzenia raportu. Identyfikator korelacji <>     |    500     |    Upewnij się, że format daty dla pól *StartTime,* *QueryStartTime* i *QueryEndTime* jest poprawny.     |
|    Usługa niedostępna    |    500     |    Jeśli stale otrzymujesz komunikat o niedostępności usługi (błąd 5xx), otwórz bilet pomocy technicznej.    |
|        |        |        |

## <a name="no-records"></a>Brak rekordów

Otrzymuję odpowiedź 200 interfejsu API po pobraniu raportu z bezpiecznej lokalizacji. Dlaczego nie widzę żadnych rekordów?
Sprawdź, czy ciąg w zapytaniu ma jedną z dopuszczalnej wartości nagłówka kolumny. Na przykład to zapytanie zwróci zero wyników:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

W tym przykładzie dopuszczalne wartości dla `IsDuplicateRowForPGA` to 0 lub 1. Zapoznaj się z [definicjami danych,](insights-data-definitions.md) aby uzyskać wszystkie możliwe wartości dla różnych kolumn.
