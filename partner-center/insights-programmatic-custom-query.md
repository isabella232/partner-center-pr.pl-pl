---
title: Specyfikacja zapytania niestandardowego
description: Dowiedz się, jak tworzyć zapytania niestandardowe do wyodrębniania danych z tabel analitycznych.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 8749e9c65a232514028e0842a020267d0df7fcadcd9f36ac9dd9ba165377f401
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696919"
---
# <a name="custom-query-specification"></a>Specyfikacja zapytania niestandardowego

Partnerzy mogą używać tej specyfikacji zapytań, aby łatwo formułować niestandardowe zapytania do wyodrębniania danych z tabel analitycznych. Zapytania mogą służyć do wybierania tylko żądanych kolumn i metryk, które pasują do określonego kryterium. Sednem specyfikacji języka jest definicja zestawu danych, w której można utworzyć zapytanie niestandardowe.

## <a name="datasets"></a>Zestawy danych

W taki sam sposób, w jaki niektóre zapytania są uruchamiane względem bazy danych zawierającej tabele i kolumny, zapytanie niestandardowe działa na zestawach danych, które mają kolumny i metryki. Pełną listę dostępnych zestawów danych do formułowania zapytania można uzyskać przy użyciu interfejsu API zestawów danych.

Jest to przykład zestawu danych wyświetlanego jako JSON:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Części zestawu danych

- Nazwa zestawu danych jest jak nazwa tabeli bazy danych. Na przykład OfficeUsage. Zestaw danych zawiera listę kolumn, które można wybrać, na przykład CustomerTenantId.
- Zestaw danych zawiera również metryki, które są podobne do funkcji agregacji w bazie danych. Na przykład TotalMonthlyActiveUsers.
- Istnieją stałe zakresy czasu, w których można eksportować dane.

## <a name="formulating-a-query-on-a-dataset"></a>Formułowanie zapytania na zestawie danych

Są to przykładowe zapytania, które pokazują, jak wyodrębniać różne typy danych.

|Zapytanie|    Opis    |
|----|    ----    |
|**WYBIERZ** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    To zapytanie pobierze każdy cusotmerTenantID i odpowiadające mu jednostki PaidAvailableUnits w ciągu ostatniego miesiąca.    |
|**WYBIERZ** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    To zapytanie spowoduje, że 10 najcięgszych dzierżaw klientów otrzyma malejącą kolejność liczby płatnych dostępnych jednostek.     |
|**WYBIERZ** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    To zapytanie pobierze jednostki PaidAvailableUnits i MonthlyActiveUsers wszystkich klientów, którzy mają co miesiąc aktywnych użytkowników więcej niż 100 000.     |
|**WYBIERZ** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    To zapytanie pobierze wartość CustomerTenantId i aktywnych użytkowników miesięcznie dla każdego miesiąca według dwóch wartości CustomerTpId: '2a31c234-1f4e-4c60-909e-7 "6d234f93161" i "80780748-3f9a-11eb-b378-0242ac130002".     |
|        |        |

## <a name="query-specification"></a>Specyfikacja zapytania

W tej sekcji opisano definicję i strukturę zapytania.

## <a name="grammar-reference"></a>Informacje o gramatyki

W tej tabeli opisano symbole używane w zapytaniach.

|    Zapytanie    |    Opis    |
|    ----    |    ----    |
|    `?`    |    Opcjonalne    |
|    `*`    |    Zero lub więcej    |
|    `+`    |    Co najmniej jeden    |
|    `\|`    |    Lub / Jedna z list    |
|        |        |

## <a name="query-definition"></a>Definicja zapytania

Instrukcja query ma następujące klauzule: SelectClause, FromClause, WhereClause, OrderClause, LimitClause i TimeSpan.

- **Wybierz pozycjęZamkń**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName:** kolumny i metryki zdefiniowane w zestawie danych
- **FromClause**: `FROM DatasetName`
    - **DatasetName:** nazwa zestawu danych zdefiniowana w zestawie danych
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition:** wartość operatora ColumOrMetricName
        - **Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Wartość:** Liczba | StringLiteral | MultiNumberList | MultiStringList
            - **Liczba:**`-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition:**`ColumOrMetricName (ASC | DESC)*`
- **LimitClause**: `LIMIT [0-9]+`
- **TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Struktura zapytań

Zapytanie raportu składa się z wielu części:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Każda część jest opisana poniżej.

### `SELECT`

Ta część zapytania określa kolumny, które zostaną wyeksportowane. Kolumny, które można wybrać, to pola wymienione w sekcjach *selectableColumns* i *availableMetrics* zestawu danych.

Opcjonalnie można `DISTINCT` określić słowo kluczowe po `SELECT` . Jeśli `DISTINCT` zostanie określony, końcowe wyeksportowane wiersze zawsze będą zawierać odrębne wartości wybranych kolumn. Metryki będą obliczane dla każdej odrębnej kombinacji wybranych kolumn, dlatego słowo kluczowe nie jest wymagane, gdy kolumna metryki znajduje się `DISTINCT` na liście wybranych kolumn.

**Przykład:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Ta część zapytania wskazuje zestaw danych, z którego należy wyeksportować dane. Nazwa zestawu danych podana w tym miejscu musi być prawidłową nazwą zestawu danych zwróconą przez interfejs API zestawów danych.

**Przykład:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Ta część zapytania służy do określania warunków filtrowania w zestawie danych. Tylko wiersze spełniające wszystkie warunki wymienione w tej klauzuli będą obecne w końcowym wyeksportowaniu pliku. Warunek filtru może być dla dowolnej kolumny wymienionej w *selectableColumns* i *availableMetrics*. Wartości określone w warunku filtru mogą być listą liczb lub listą ciągów tylko wtedy, gdy operatorem jest `IN` lub `NOT IN` . Wartości mogą być zawsze podane jako ciąg literału i zostaną przekonwertowane na natywne typy kolumn. Wiele warunków filtrowania należy oddzielić za pomocą operacji AND.

**Przykład:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Ta część zapytania określa kryteria kolejności dla wyeksportowanych wierszy. Kolumny, w których można zdefiniować kolejność, muszą pochodzić z kolumn *selectableColumns* i *availableMetrics* zestawu danych. Jeśli nie określono kierunku kolejności, zostanie on domyślnie desc w kolumnie. Kolejność można zdefiniować w wielu kolumnach, oddzielając kryteria przecinkami.

**Przykład:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Ta część zapytania określa liczbę wierszy, które zostaną wyeksportowane. Określana liczba musi być dodatnią liczbą całkowitą niezerową.

### `TIMESPAN`

Ta część zapytania określa czas trwania, dla którego dane muszą zostać wyeksportowane. Możliwe wartości powinny pochodzić z pola *availableDateRanges* w definicji zestawu danych.

### <a name="case-sensitivity-in-query-specification"></a>Czułość wielkości liter w specyfikacji zapytania

W specyfikacji jest całkowicie bez uwzględniania liter. Wstępnie zdefiniowane słowa kluczowe, nazwy kolumn i wartości można określić przy użyciu wielkich lub wielkich liter.

## <a name="next-steps"></a>Następne kroki

- [Lista zapytań systemowych](insights-programmatic-system-queries.md)
- [Lista przykładowych zapytań](insights-programmatic-sample-queries.md)