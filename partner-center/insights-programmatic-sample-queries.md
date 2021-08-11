---
title: Lista przykładowych zapytań
description: Użyj przykładowych zapytań, aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji o partnerach.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: fff74f7bf6c58f5845c491d23a1f71c3da177e0c126e863205f0fb18eb07b7c9
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693286"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Przykładowe zapytania dotyczące Partner Center szczegółowych informacji

Ten artykuł zawiera przykładowe zapytania dotyczące raportów Szczegółowe informacje partnerów. Możesz użyć tych zapytań, wywołując punkt końcowy interfejsu API tworzenia zapytań raportów. W razie potrzeby wywołanie [interfejsu API tworzenia zapytania](insights-programmatic-access-paradigm.md#create-report-query-api) raportu można zmodyfikować w celu dodania większej liczby kolumn, dostosowania okresu obliczeniowego i dodania warunków filtrowania.

Aby uzyskać szczegółowe informacje o nazwach kolumn, atrybutach i opisach, zapoznaj się z [definicjami danych](insights-data-definitions.md).

## <a name="customer-details"></a>Szczegóły klienta

Te przykładowe zapytania dotyczą raportu szczegóły klientów:

### <a name="by-geography"></a>Według lokalizacji geograficznej

Lista klientów z określonej lokalizacji geograficznej w ostatnim miesiącu.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Według: SKU i przychód rozliowany

Lista klientów używających określonej sku i rozliczanych przychodów w ciągu ostatnich 6 miesięcy wynosi ponad 20 000

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Według dostępnych stanowisk

10 najlepszych klientów na podstawie dostępnych miejsc w ostatnim miesiącu

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Profil partnera

Te przykładowe zapytania dotyczą raportu profilu partnera:

### <a name="by-geography"></a>Według lokalizacji geograficznej

Lista partnerów z określonej lokalizacji geograficznej.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Według partnera MPN

Lista partnerów w ramach tego samego partnera PGA MPN

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Wydajność odsprzedawcy

Te przykładowe zapytania dotyczą raportu wydajności odsprzedawcy:

### <a name="by-geography"></a>Według lokalizacji geograficznej

Lista odsprzedawców z określonej lokalizacji geograficznej w ostatnim miesiącu.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Według odsprzedawcy

Liczba klientów, liczba subskrypcji, łączna liczba dostępnych stanowisk, łączna liczba przypisanych stanowisk, całkowity przychód dla określonego odsprzedawcy.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>10 najlepszych według przychodu

10 najlepszych odsprzedawców na podstawie całkowitego przychodu w ostatnim miesiącu.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Szczegóły subskrypcji

Te przykładowe zapytania dotyczą raportu szczegółów subskrypcji:

### <a name="by-renewal-eligibility"></a>Przez uprawnienie do odnawiania

Lista subskrypcji, które nie kwalifikują się do automatycznego odnawiania w ostatnim miesiącu.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Według stanu subskrypcji

Lista subskrypcji, które mają stan Wyłącz w ostatnim miesiącu.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Liczby dla sześciu miesięcy

Liczba subskrypcji, łączna liczba sprzedanych miejsc, liczba klientów dla określonego partnera w ciągu ostatnich sześciu miesięcy.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Użycie platformy Azure

Te przykładowe zapytania dotyczą raportu użycia platformy Azure:

### <a name="by-meter-category"></a>Według kategorii mierników

Lista subskrypcji użycia platformy Azure z jednostkami użycia i usługą ACR dla określonej kategorii mierników w ciągu ostatnich sześciu miesięcy.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Według łącznej liczby ACR

Lista subskrypcji użycia platformy Azure, w których łączna liczba subskrypcji usługi ACR jest większa niż 20 000 w ciągu ostatnich sześciu miesięcy

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Następne kroki

- [Interfejsy API do uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów](insights-programmatic-analytics-available-api.md)