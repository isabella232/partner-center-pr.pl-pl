---
title: Raport użycia platformy Azure w usłudze Partner Center
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zobacz, co jest potrzebne, i w jaki sposób możesz ulepszyć korzystanie z subskrypcji platformy Azure sprzedawanych lub zarządzanych przez klientów.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ef72aa2e44797c906cdd0a216cf2d8355668c0a9
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086213"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>Raport użycia platformy Azure dostępny na pulpicie nawigacyjnym usługi Partner Center Insights

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny
- Podgląd raportów
- Executive — Podgląd raportów

Raport użycia platformy Azure przedstawia metryki związane z subskrypcjami platformy Azure dla klientów. Ten raport zawiera dochody i użycie platformy Azure według kategorii mierników. Poniższe sekcje można wyświetlić w raporcie użycia platformy Azure.

- Podsumowanie
- Użycie platformy Azure według lokalizacji geograficznej
- Wykorzystanie platformy Azure

 > [!NOTE]
 > Ten raport jest dostępny na pulpicie nawigacyjnym usługi Insights. Aby wyświetlić ten raport, musisz mieć przypisaną określoną rolę w centrum partnerskim, takim jak Administrator globalny, administrator konta, Podgląd raportów lub dyrektor raportów programu. Aby uzyskać więcej informacji, zobacz Administrator globalny firmy. określone typy danych w tym raporcie mogą być również dostępne tylko dla użytkowników z uprawnieniami dyrektora raportów.

## <a name="summary"></a>Podsumowanie

Sekcja podsumowania przedstawia widok migawek kluczowych wskaźników wydajności (KPI) związanych z subskrypcjami platformy Azure sprzedawanymi lub zarządzanymi przez klienta.  

- Subskrypcje platformy Azure: Bieżąca liczba subskrypcji klientów platformy Azure sprzedawanych lub zarządzanych przez użytkownika.
Procent wzrostu lub odrzucenia subskrypcji platformy Azure w ramach wybranego zakresu dat.

Na mikrografie prezentowany jest miesięczny trend dotyczący liczby subskrypcji platformy Azure dla wybranego zakresu dat.
- Aktywne subskrypcje platformy Azure: aktualna liczba subskrypcji platformy Azure sprzedawanych lub zarządzanych przez użytkownika, którzy mieli aktywne użycie w ciągu ostatnich 30 dni.
Procent wzrostu lub odrzucenia tych subskrypcji w wybranym zakresie dat.

W ramach wybranego zakresu dat w programie Micro Chart zostanie przedliczony miesięczny Trend liczby aktywnych subskrypcji platformy Azure.

- Przychód zużyty na platformie Azure (ACR): całkowity przychód zużyty przez platformę Azure (US $) przypisany do użytkownika w wybranym zakresie dat.
Procent wzrostu lub odrzucania atrybutów ACR US $ w wybranym zakresie dat. 

W programie Micro Chart jest prezentowany miesięczny trend ACR US $ przypisany do użytkownika w wybranym okresie


> [!NOTE]
 > Przychód zużyty na platformie Azure (ACR) będzie widoczny tylko dla użytkowników, którym przypisano rolę programu Executive Report Viewer.

:::image type="content" source="images/pci/pci-azure-usage-summary-1.png" alt-text="Podsumowanie użycia platformy Azure":::

## <a name="azure-usage-by-geography"></a>Użycie platformy Azure według lokalizacji geograficznej

Widok **użycie platformy Azure według** lokalizacji geograficznej przedstawia rozkład geograficzny przychodu użycia platformy Azure (ACR US $) lub godziny użytkowania dla wszystkich lub wybranych kategorii poziomu/miernika usług platformy Azure. Jaśniejsze kolory na mapie przedstawiają mniejsze wartości, a ciemne kolory reprezentują wyższe wartości. Możesz wyszukać i wybrać kraj w siatce, aby powiększyć 

**Liczba tabeli kraje/region** przedstawia łączne kraje/regiony, w których są generowane zdarzenia użycia platformy Azure.

Możesz wyszukać i wybrać kraj w siatce, aby powiększyć do lokalizacji na mapie. Wybierz opcję **Strona główna** na mapie, aby powrócić do oryginalnego widoku.

:::image type="content" source="images/pci/pci-azure-usage-by-geography-2.png" alt-text="Użycie platformy Azure według lokalizacji geograficznej":::

## <a name="azure-utilization"></a>Wykorzystanie platformy Azure

Ten widok przedstawia miesięczny przychód użycia lub trendy zużycia na platformie Azure według wybranych kategorii poziomu usługi platformy Azure. 

Wykres słupkowy przedstawia trend miesięcznego przychodu/godziny użycia. Wykres liniowy przedstawia trend wzrostu w porównaniu do poprzedniego miesiąca dla wybranych kategorii poziomów/usług platformy Azure.

:::image type="content" source="images/pci/pci-azure-usage-utilization-3.png" alt-text="Użycie na platformie Azure":::

## <a name="next-steps"></a>Następne kroki

- Więcej raportów można znaleźć w temacie [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Możesz pobrać pierwotne dane, aby wyłączyć ten raport z sekcji Pobieranie raportów na pulpicie nawigacyjnym usługi Insights. [Więcej informacji](pci-download-reports.md) 
