---
title: Lista przykładowych zapytań
description: Użyj przykładowych zapytań, aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji partnerów.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376660"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="5fdc9-103">Przykładowe zapytania dotyczące Partner Center szczegółowych informacji</span><span class="sxs-lookup"><span data-stu-id="5fdc9-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="5fdc9-104">Ten artykuł zawiera przykładowe zapytania dotyczące raportów Szczegółowe informacje partnerów.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="5fdc9-105">Możesz użyć tych zapytań, wywołując punkt końcowy interfejsu API tworzenia zapytania raportu.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="5fdc9-106">W razie potrzeby wywołanie [interfejsu API](insights-programmatic-access-paradigm.md#create-report-query-api) tworzenia zapytania raportu można zmodyfikować, aby dodać więcej kolumn, dostosować okres obliczeniowy i dodać warunki filtrowania.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="5fdc9-107">Aby uzyskać szczegółowe informacje o nazwach kolumn, atrybutach i opisach, zapoznaj się z [definicjami danych](insights-data-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="5fdc9-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="5fdc9-108">Szczegóły klienta</span><span class="sxs-lookup"><span data-stu-id="5fdc9-108">Customer details</span></span>

<span data-ttu-id="5fdc9-109">Te przykładowe zapytania dotyczą raportu szczegóły klientów:</span><span class="sxs-lookup"><span data-stu-id="5fdc9-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="5fdc9-110">Według lokalizacji geograficznej</span><span class="sxs-lookup"><span data-stu-id="5fdc9-110">By geography</span></span>

<span data-ttu-id="5fdc9-111">Lista klientów z określonej lokalizacji geograficznej w ostatnim miesiącu.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="5fdc9-112">Według: SKU i przychód rozliowany</span><span class="sxs-lookup"><span data-stu-id="5fdc9-112">By SKU and billed revenue</span></span>

<span data-ttu-id="5fdc9-113">Lista klientów korzystających z określonej sku i rozliczanych przychodów w ciągu ostatnich 6 miesięcy wynosi ponad 20 000</span><span class="sxs-lookup"><span data-stu-id="5fdc9-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="5fdc9-114">Według dostępnych stanowisk</span><span class="sxs-lookup"><span data-stu-id="5fdc9-114">By available seats</span></span>

<span data-ttu-id="5fdc9-115">10 najlepszych klientów na podstawie dostępnych miejsc w ostatnim miesiącu</span><span class="sxs-lookup"><span data-stu-id="5fdc9-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="5fdc9-116">Profil partnera</span><span class="sxs-lookup"><span data-stu-id="5fdc9-116">Partner Profile</span></span>

<span data-ttu-id="5fdc9-117">Te przykładowe zapytania dotyczą raportu profilu partnera:</span><span class="sxs-lookup"><span data-stu-id="5fdc9-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="5fdc9-118">Według lokalizacji geograficznej</span><span class="sxs-lookup"><span data-stu-id="5fdc9-118">By geography</span></span>

<span data-ttu-id="5fdc9-119">Lista partnerów z określonej lokalizacji geograficznej.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="5fdc9-120">Według partnera MPN</span><span class="sxs-lookup"><span data-stu-id="5fdc9-120">By MPN partner</span></span>

<span data-ttu-id="5fdc9-121">Lista partnerów w ramach tego samego partnera PGA MPN</span><span class="sxs-lookup"><span data-stu-id="5fdc9-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="5fdc9-122">Reseller Performance</span><span class="sxs-lookup"><span data-stu-id="5fdc9-122">Reseller Performance</span></span>

<span data-ttu-id="5fdc9-123">Te przykładowe zapytania dotyczą raportu wydajności odsprzedawcy:</span><span class="sxs-lookup"><span data-stu-id="5fdc9-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="5fdc9-124">Według lokalizacji geograficznej</span><span class="sxs-lookup"><span data-stu-id="5fdc9-124">By geography</span></span>

<span data-ttu-id="5fdc9-125">Lista odsprzedawców z określonej lokalizacji geograficznej w ostatnim miesiącu.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="5fdc9-126">Według odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="5fdc9-126">By reseller</span></span>

<span data-ttu-id="5fdc9-127">Liczba klientów, liczba subskrypcji, łączna liczba dostępnych stanowisk, łączna liczba przypisanych stanowisk, całkowity przychód dla określonego odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="5fdc9-128">10 najlepszych według przychodu</span><span class="sxs-lookup"><span data-stu-id="5fdc9-128">Top 10 by revenue</span></span>

<span data-ttu-id="5fdc9-129">10 najlepszych odsprzedawców na podstawie całkowitego przychodu w ostatnim miesiącu.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="5fdc9-130">Szczegóły subskrypcji</span><span class="sxs-lookup"><span data-stu-id="5fdc9-130">Subscription Details</span></span>

<span data-ttu-id="5fdc9-131">Te przykładowe zapytania dotyczą raportu szczegółów subskrypcji:</span><span class="sxs-lookup"><span data-stu-id="5fdc9-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="5fdc9-132">Przez uprawnienie do odnawiania</span><span class="sxs-lookup"><span data-stu-id="5fdc9-132">By renewal eligibility</span></span>

<span data-ttu-id="5fdc9-133">Lista subskrypcji, które nie kwalifikują się do automatycznego odnawiania w ostatnim miesiącu.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="5fdc9-134">Według stanu subskrypcji</span><span class="sxs-lookup"><span data-stu-id="5fdc9-134">By subscription state</span></span>

<span data-ttu-id="5fdc9-135">Lista subskrypcji, które mają stan Wyłącz w ostatnim miesiącu.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="5fdc9-136">Liczby dla sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="5fdc9-136">Counts for six months</span></span>

<span data-ttu-id="5fdc9-137">Liczba subskrypcji, łączna liczba sprzedanych miejsc, liczba klientów dla określonego partnera w ciągu ostatnich sześciu miesięcy.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="5fdc9-138">Użycie platformy Azure</span><span class="sxs-lookup"><span data-stu-id="5fdc9-138">Azure Usage</span></span>

<span data-ttu-id="5fdc9-139">Te przykładowe zapytania dotyczą raportu użycia platformy Azure:</span><span class="sxs-lookup"><span data-stu-id="5fdc9-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="5fdc9-140">Według kategorii mierników</span><span class="sxs-lookup"><span data-stu-id="5fdc9-140">By meter category</span></span>

<span data-ttu-id="5fdc9-141">Lista subskrypcji użycia platformy Azure z jednostkami użycia i usługą ACR dla określonej kategorii mierników w ciągu ostatnich sześciu miesięcy.</span><span class="sxs-lookup"><span data-stu-id="5fdc9-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="5fdc9-142">Według łącznej liczby ACR</span><span class="sxs-lookup"><span data-stu-id="5fdc9-142">By total ACR</span></span>

<span data-ttu-id="5fdc9-143">Lista subskrypcji użycia platformy Azure, w których łączna liczba subskrypcji usługi ACR jest większa niż 20 000 w ciągu ostatnich sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="5fdc9-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="5fdc9-144">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="5fdc9-144">Next steps</span></span>

- [<span data-ttu-id="5fdc9-145">Interfejsy API do uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów</span><span class="sxs-lookup"><span data-stu-id="5fdc9-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)