---
title: Specyfikacja zapytania niestandardowego
description: Dowiedz się, jak tworzyć zapytania niestandardowe w celu wyodrębniania danych z tabel analitycznych.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377164"
---
# <a name="custom-query-specification"></a><span data-ttu-id="8fc3e-103">Specyfikacja zapytania niestandardowego</span><span class="sxs-lookup"><span data-stu-id="8fc3e-103">Custom query specification</span></span>

<span data-ttu-id="8fc3e-104">Partnerzy mogą używać tej specyfikacji zapytań, aby łatwo formułować zapytania niestandardowe do wyodrębniania danych z tabel analitycznych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="8fc3e-105">Zapytania mogą służyć do wybierania tylko żądanych kolumn i metryk, które pasują do określonego kryterium.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="8fc3e-106">Sednem specyfikacji języka jest definicja zestawu danych, w której można zapisywać zapytanie niestandardowe.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="8fc3e-107">Zestawy danych</span><span class="sxs-lookup"><span data-stu-id="8fc3e-107">Datasets</span></span>

<span data-ttu-id="8fc3e-108">W taki sam sposób, w jaki niektóre zapytania są uruchamiane względem bazy danych zawierającej tabele i kolumny, zapytanie niestandardowe działa na zestawach danych, które mają kolumny i metryki.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="8fc3e-109">Pełną listę dostępnych zestawów danych do formułowania zapytania można uzyskać przy użyciu interfejsu API zestawów danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="8fc3e-110">Jest to przykład zestawu danych wyświetlanego jako JSON:</span><span class="sxs-lookup"><span data-stu-id="8fc3e-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="8fc3e-111">Części zestawu danych</span><span class="sxs-lookup"><span data-stu-id="8fc3e-111">Parts of a dataset</span></span>

- <span data-ttu-id="8fc3e-112">Nazwa zestawu danych jest jak nazwa tabeli bazy danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="8fc3e-113">Na przykład OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-113">For example, OfficeUsage.</span></span> <span data-ttu-id="8fc3e-114">Zestaw danych zawiera listę kolumn, które można wybrać, na przykład CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="8fc3e-115">Zestaw danych zawiera również metryki, które są podobne do funkcji agregacji w bazie danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="8fc3e-116">Na przykład TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="8fc3e-117">Istnieją stałe zakresy czasu, w których można eksportować dane.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="8fc3e-118">Formułowanie zapytania na zestawie danych</span><span class="sxs-lookup"><span data-stu-id="8fc3e-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="8fc3e-119">Są to przykładowe zapytania, które pokazują, jak wyodrębniać różne typy danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="8fc3e-120">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="8fc3e-120">Query</span></span>|    <span data-ttu-id="8fc3e-121">Opis</span><span class="sxs-lookup"><span data-stu-id="8fc3e-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="8fc3e-122">**WYBIERZ** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="8fc3e-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="8fc3e-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="8fc3e-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="8fc3e-124">To zapytanie pobierze każdy kod CusotmerTenantID i odpowiadające mu jednostki PaidAvailableUnits w ciągu ostatniego 1 miesiąca.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="8fc3e-125">**WYBIERZ** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="8fc3e-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="8fc3e-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="8fc3e-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="8fc3e-127">To zapytanie spowoduje, że 10 najlepszych dzierżaw klientów otrzyma malejącą kolejność liczby płatnych dostępnych jednostek.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="8fc3e-128">**WYBIERZ** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="8fc3e-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="8fc3e-129">To zapytanie pobierze jednostki PaidAvailableUnits i MonthlyActiveUsers wszystkich klientów, którzy mają użytkowników MonthlyActiveUser więcej niż 100 000.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="8fc3e-130">**WYBIERZ** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="8fc3e-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="8fc3e-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="8fc3e-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="8fc3e-132">To zapytanie pobierze wartości CustomerTenantId i monthly active users dla każdego miesiąca według dwóch wartości CustomerTpId: '2a31c234-1f4e-4c60-909e-76d234f93161" i "80780748-3f9a-11eb-b378-0242ac130002".</span><span class="sxs-lookup"><span data-stu-id="8fc3e-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="8fc3e-133">Specyfikacja zapytania</span><span class="sxs-lookup"><span data-stu-id="8fc3e-133">Query specification</span></span>

<span data-ttu-id="8fc3e-134">W tej sekcji opisano definicję i strukturę zapytania.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="8fc3e-135">Informacje o gramatyki</span><span class="sxs-lookup"><span data-stu-id="8fc3e-135">Grammar reference</span></span>

<span data-ttu-id="8fc3e-136">W tej tabeli opisano symbole używane w zapytaniach.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="8fc3e-137">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="8fc3e-137">Query</span></span>    |    <span data-ttu-id="8fc3e-138">Opis</span><span class="sxs-lookup"><span data-stu-id="8fc3e-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="8fc3e-139">Opcjonalne</span><span class="sxs-lookup"><span data-stu-id="8fc3e-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="8fc3e-140">Zero lub więcej</span><span class="sxs-lookup"><span data-stu-id="8fc3e-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="8fc3e-141">Co najmniej jeden</span><span class="sxs-lookup"><span data-stu-id="8fc3e-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="8fc3e-142">Lub / Jedna z list</span><span class="sxs-lookup"><span data-stu-id="8fc3e-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="8fc3e-143">Definicja zapytania</span><span class="sxs-lookup"><span data-stu-id="8fc3e-143">Query definition</span></span>

<span data-ttu-id="8fc3e-144">Instrukcja query ma następujące klauzule: SelectClause, FromClause, WhereClause, OrderClause, LimitClause i TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="8fc3e-145">**Wybierz pozycjęZamkń**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="8fc3e-146">**ColumOrMetricName:** kolumny i metryki zdefiniowane w zestawie danych</span><span class="sxs-lookup"><span data-stu-id="8fc3e-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="8fc3e-147">**FromClause**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="8fc3e-148">**DatasetName:** nazwa zestawu danych zdefiniowana w zestawie danych</span><span class="sxs-lookup"><span data-stu-id="8fc3e-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="8fc3e-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="8fc3e-150">**FilterCondition:** wartość operatora ColumOrMetricName</span><span class="sxs-lookup"><span data-stu-id="8fc3e-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="8fc3e-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="8fc3e-152">**Wartość:** Liczba | StringLiteral | Lista MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="8fc3e-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="8fc3e-153">**Liczba:**`-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="8fc3e-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="8fc3e-155">**MultiNumberList:**`(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="8fc3e-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="8fc3e-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="8fc3e-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="8fc3e-159">**LimitClause**: `LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="8fc3e-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="8fc3e-161">Struktura zapytań</span><span class="sxs-lookup"><span data-stu-id="8fc3e-161">Query Structure</span></span>

<span data-ttu-id="8fc3e-162">Zapytanie raportu składa się z wielu części:</span><span class="sxs-lookup"><span data-stu-id="8fc3e-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="8fc3e-163">Każda część jest opisana poniżej.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="8fc3e-164">Ta część zapytania określa kolumny, które zostaną wyeksportowane.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="8fc3e-165">Kolumny, które można wybrać, to pola wymienione w sekcjach *selectableColumns* i *availableMetrics* zestawu danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="8fc3e-166">Opcjonalnie można `DISTINCT` określić słowo kluczowe po . `SELECT`</span><span class="sxs-lookup"><span data-stu-id="8fc3e-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="8fc3e-167">Jeśli `DISTINCT` zostanie określony, końcowe wyeksportowane wiersze zawsze będą zawierać odrębne wartości wybranych kolumn.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="8fc3e-168">Metryki będą obliczane dla każdej odrębnej kombinacji wybranych kolumn, dlatego słowo kluczowe nie jest wymagane, gdy kolumna metryki znajduje się `DISTINCT` na liście wybranych kolumn.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="8fc3e-169">**Przykład:**</span><span class="sxs-lookup"><span data-stu-id="8fc3e-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="8fc3e-170">Ta część zapytania wskazuje zestaw danych, z którego należy wyeksportować dane.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="8fc3e-171">Nazwa zestawu danych podana w tym miejscu musi być prawidłową nazwą zestawu danych zwróconą przez interfejs API zestawów danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="8fc3e-172">**Przykład:**</span><span class="sxs-lookup"><span data-stu-id="8fc3e-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="8fc3e-173">Ta część zapytania służy do określania warunków filtrowania w zestawie danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="8fc3e-174">Tylko wiersze zgodne ze wszystkimi warunkami wymienionymi w tej klauzuli będą obecne w końcowym wyeksportowaniu pliku.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="8fc3e-175">Warunek filtru może być dla dowolnej kolumny wymienionej w *selectableColumns* i *availableMetrics*.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="8fc3e-176">Wartości określone w warunku filtru mogą być listą liczb lub listą ciągów tylko wtedy, gdy operatorem jest `IN` lub `NOT IN` .</span><span class="sxs-lookup"><span data-stu-id="8fc3e-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="8fc3e-177">Wartości mogą być zawsze podane jako ciąg literału i zostaną przekonwertowane na natywne typy kolumn.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="8fc3e-178">Wiele warunków filtrowania należy oddzielić za pomocą operacji AND.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="8fc3e-179">**Przykład:**</span><span class="sxs-lookup"><span data-stu-id="8fc3e-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="8fc3e-180">Ta część zapytania określa kryteria zamawiania wyeksportowanych wierszy.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="8fc3e-181">Kolumny, na których można zdefiniować kolejność, muszą pochodzić z kolumn *selectableColumns* i *availableMetrics* zestawu danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="8fc3e-182">Jeśli nie określono kierunku kolejności, zostanie on domyślnie desc w kolumnie.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="8fc3e-183">Kolejność można zdefiniować w wielu kolumnach, oddzielając kryteria przecinkiem.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="8fc3e-184">**Przykład:**</span><span class="sxs-lookup"><span data-stu-id="8fc3e-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="8fc3e-185">Ta część zapytania określa liczbę wierszy, które zostaną wyeksportowane.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="8fc3e-186">Określana liczba musi być dodatnią liczbą całkowitą niezerową.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="8fc3e-187">Ta część zapytania określa czas, dla którego dane muszą zostać wyeksportowane.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="8fc3e-188">Możliwe wartości powinny pochodzić z *pola availableDateRanges* w definicji zestawu danych.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="8fc3e-189">Czułość wielkości liter w specyfikacji zapytania</span><span class="sxs-lookup"><span data-stu-id="8fc3e-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="8fc3e-190">W specyfikacji jest całkowicie bez uwzględniania liter.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="8fc3e-191">Wstępnie zdefiniowane słowa kluczowe, nazwy kolumn i wartości można określić przy użyciu wielkich lub wielkich liter.</span><span class="sxs-lookup"><span data-stu-id="8fc3e-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8fc3e-192">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="8fc3e-192">Next steps</span></span>

- [<span data-ttu-id="8fc3e-193">Lista zapytań systemowych</span><span class="sxs-lookup"><span data-stu-id="8fc3e-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="8fc3e-194">Lista przykładowych zapytań</span><span class="sxs-lookup"><span data-stu-id="8fc3e-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)