---
title: Partner Center wydajności odsprzedawców usługi Partner Center Insights
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pulpit nawigacyjny wydajności odsprzedawcy w Partner Center Insights zawiera omówienie wydajności różnych pośrednich odsprzedawców CSP Indirect Provider.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a2a5697f19baadb5af956a745c032ce1711574d3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855237"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>Pulpit nawigacyjny wydajności odsprzedawcy w Partner Center Insights

**Odpowiednie role:** Administrator globalny | Agent administracyjny | Przeglądarka raportów | Przeglądarka raportów dla kierownictwa

Pulpit nawigacyjny wydajności odsprzedawcy w Partner Center Insights zawiera omówienie wydajności różnych pośrednich odsprzedawców CSP Indirect Provider. Pulpit nawigacyjny zawiera dane odsprzedawców, którzy są aktywni, jakie przychody generują i jakie produkty generują przychody. Dostawcy pośredni będą mogli wyszukać określonego odsprzedawcę według nazwy i wyszukać szczegóły odsprzedawcy na pulpicie nawigacyjnym wydajności odsprzedawcy.

Poniższe sekcje można wyświetlić na pulpicie nawigacyjnym wydajności odsprzedawcy.

- Podsumowanie
- Geograficzny rozrzut odsprzedawców
- Dodawanie/rezygnacje odsprzedawców 
- Trend przychodów odsprzedawców 
- Wydajność odsprzedawcy według produktów
- Aktywni odsprzedawcy według lokalizacji partnerów
- Trend dystrybucji geograficznej przychodów
- Wydajność odsprzedawcy według segmentu klientów
- Stan podpisywania umowy MPA odsprzedawcy

 > [!NOTE]
 > Ten raport jest dostępny na pulpicie nawigacyjnym szczegółowych informacji. Aby wyświetlić ten raport, musisz mieć przypisaną określoną rolę w programie Partner Center, taką jak Administrator globalny, Administrator konta, Podgląd raportów lub Executive Report Viewer. Aby uzyskać więcej informacji, zobacz Administrator globalny firmy. Określone typy danych w tym raporcie mogą być również dostępne tylko dla użytkowników z uprawnieniami Executive Report Viewer.

## <a name="summary"></a>Podsumowanie

Sekcja podsumowania zawiera widok migawki kluczowych wskaźników wydajności (KPI) powiązanych z CSP Indirect Provider.

- Aktywni odsprzedawcy: liczba odsprzedawców, którzy mają co najmniej jedną aktywną subskrypcję w tym miesiącu.

Wykres Micro przedstawia trend miesiąc do miesiąca różnych odsprzedawców, którzy są aktywni w wybranym zakresie dat.

- Odsprzedawcy transakcji: liczba odsprzedawców, którzy sprzedali co najmniej jedną subskrypcję w tym miesiącu. 

Wykres Micro przedstawia trend sprzedawców zarejestrowanych w wybranym zakresie dat z miesiąca na miesiąc.

- Nowi odsprzedawcy: Liczba odsprzedawców, którzy rozpoczęli transakcję u dostawcy pośredniego w tym miesiącu. 

Wykres Micro przedstawia trend z miesiąca na miesiąc łącznej liczby nowych odsprzedawców w wybranym zakresie dat.

- Przychód rozliczny USD: przychód w USD sterowany przez odsprzedawców w tym miesiącu. 

Wykres Micro przedstawia trend przychodów z miesiąca na miesiąc w wybranym zakresie dat.

- Sekcja Rozliczany przychód według produktów zawiera miesiąc według miesięcznego podziału przychodu rozliczanych w USD z podziałem na sprzedane produkty. 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="podsumowanie wydajności odsprzedawców":::

## <a name="geographical-spread-of-resellers"></a>Geograficzne rozrzuty odsprzedawców

Widok **Odsprzedawcy według lokalizacji geograficznej zapewnia geograficzną dystrybucję odsprzedawców. Za pomocą tego widżetu partnerzy mogą wyświetlać łączną liczbę odsprzedawców, nowych odsprzedawców i rozliczany przychód **(USD)** z podziałem na różne lokalizacje geograficzne.

Możesz wyszukać i wybrać kraj w siatce, aby powiększyć lokalizację na mapie. Naciśnij opcję **Strona** główna na mapie, aby przywrócić oryginalny widok. Zatrzymaj wskaźnik myszy na mapie, aby wyświetlić **rozliczany przychód (USD)** według kraju. Pole Rozliczany przychód (USD) na siatce jest sortowalne.

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="Odsprzedawcy według lokalizacji geograficznej ":::

## <a name="resellers-addchurns"></a>Odsprzedawcy dodają/zrzucą

Ten widok zawiera podział miesiąc po miesiącu liczby nowych odsprzedawców, odsprzedawców z rezygnacją **i** **istniejących odsprzedawców.** 

- Nowi odsprzedawcy: liczba odsprzedawców, którzy zostali nowo zarejestrowani u dostawcy pośredniego w wybranym zakresie dat.
- Rezygnacje odsprzedawców: liczba odsprzedawców, którzy nie mieli transakcji w ciągu ostatnich sześciu miesięcy z wyłączeniem bieżącego miesiąca.
- Istniejący odsprzedawcy: Liczba odsprzedawców, którzy byli transakcjami w poprzednim miesiącu.

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="Dodawanie/rezygnacje odsprzedawców":::

## <a name="resellers-revenue-trend"></a>Trend przychodów odsprzedawców 

Ten widok przedstawia miesięczny trend rozlicznych przychodów (USD) według produktów, takich jak O365, D365, EMS, Power BI i Azure. Ogólne metryki są agregowane dla różnych produktów dla każdego miesiąca. Partner może wyszukać określonego odsprzedawcę według nazwy i wyszukać dane dla tego określonego odsprzedawcy. Pole Rozliczany przychód (USD) w siatce można sortować.

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="Trend przychodów odsprzedawców":::

## <a name="reseller-performance-by-products"></a>Wydajność odsprzedawcy według produktów

Ten widok zawiera podział kluczowych metryk, takich jak Rozliczany przychód, liczba subskrypcji i liczba licencji według różnych produktów w miesiącu. Wykres kołowy po prawej stronie wskazuje ogólny podział metryk według różnych produktów, dzięki czemu partner szybko zobaczy podział według różnych produktów, które sprzedaje odsprzedawca.

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="Wydajność odsprzedawcy według produktów":::

## <a name="active-resellers-by-partner-locations"></a>Aktywni odsprzedawcy według lokalizacji partnerów

Ten widok zawiera podział aktywnych odsprzedawców według lokalizacji geograficznych partnerów. Pięć najlepszych lokalizacji geograficznych jest wyświetlanych w legendzie, a pozostałe są skategoryzowane jako "Inne".

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="Aktywni odsprzedawcy według lokalizacji partnerów":::

## <a name="revenue-geo-distribution-trend"></a>Trend dystrybucji geograficznej przychodów

Ten widok zawiera miesiąc trendu miesięcznego przychodu (USD) podzielonego według pięciu najpokaższe lokalizacje geograficzne.  Pozostała część przychodu jest skategoryzowana jako "Inne".

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="Trend dystrybucji geograficznej przychodów":::

## <a name="reseller-performance-by-customer-segment"></a>Wydajność odsprzedawcy według segmentu klientów

Ten widok umożliwia partnerowi zrozumienie miesięcznego trendu przychodów w USD, liczby subskrypcji i licencji z podziałem na różne segmenty klientów. Pięć najlepszych segmentów klientów jest wyświetlanych na wykresie, a pozostałe są skategoryzowane jako "Inne".

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="Wydajność odsprzedawcy według segmentu klientów":::

## <a name="reseller-mpa-signing-status"></a>Stan podpisywania umowy MPA odsprzedawcy

Ten widok zawiera stan podpisywania umowy MPA dla odsprzedawców wraz z dodatkowymi meta danymi, takimi jak stan vetting MPN, stan migracji PMC do komputera itp.

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="Stan podpisywania umowy MPA odsprzedawcy":::

## <a name="next-steps"></a>Następne kroki

- Aby uzyskać więcej raportów, [zobacz Partner Center Insights.](partner-center-insights.md)

>[!NOTE] 
> Możesz pobrać nieprzetworzone dane, które są zasilane z tego raportu, z sekcji Pobieranie raportów na pulpicie nawigacyjnym szczegółowych informacji. [Więcej informacji](pci-download-reports.md) 
