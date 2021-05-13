---
title: Partner Center subskrypcji usługi Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sprawdź, co robisz dobrze i gdzie możesz ulepszyć subskrypcje chmury, które sprzedajesz lub zarządzasz dla swoich klientów.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89806b08485bc4bd286c2e14a19924ca0e281b6d
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854472"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Raport subskrypcji produktów dostępny na pulpicie nawigacyjnym Partner Center Insights

**Odpowiednie role:** Administrator globalny | Agent administracyjny | Przeglądarka raportów | Przeglądarka raportów dla kierownictwa

Raport Subskrypcje produktów przedstawia analizę subskrypcji w chmurze, które zostały sprzedane lub które zarządzasz dla klientów. Jest to raport specyficzny dla produktu, który zawiera informacje o wydajności subskrypcji skojarzonych z produktami w chmurze, takimi jak Office 365, Azure, Dynamics i inne.

Poniższe sekcje można wyświetlić w raporcie Subskrypcje produktów.

- Podsumowanie
- Geograficzne rozrzuty subskrypcji
- Trend dodawania/rezygnacji subskrypcji
- Dystrybucja subskrypcji według lokalizacji partnerów, kanału sprzedaży, jednostki SKU, typ dołączania partnera, segment
- Trend według stanów subskrypcji
- Trend produktów

 > [!NOTE]
 > Ten raport jest dostępny na pulpicie nawigacyjnym szczegółowych informacji. Aby wyświetlić ten raport, musisz mieć przypisaną określoną rolę w programie Partner Center, taką jak Administrator globalny, Administrator konta, Podgląd raportów lub Executive Report Viewer. Aby uzyskać więcej informacji, zobacz administrator globalny firmy. Określone typy danych w tym raporcie mogą być również dostępne tylko dla użytkowników z uprawnieniami Executive Report Viewer.

## <a name="summary"></a>Podsumowanie

Sekcja podsumowania zawiera widok migawki kluczowych wskaźników wydajności (KPI) związanych z subskrypcjami sprzedawanymi lub zarządzanymi przez Ciebie dla klientów.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="podsumowanie raportu subskrypcji":::

Aby uzyskać więcej informacji na temat każdej sekcji podsumowania, zobacz poniżej:

- Subskrypcje:
  - Bieżąca liczba subskrypcji produktów w chmurze sprzedanych lub zarządzanych przez Ciebie.
  - Procentowy wzrost lub spadek liczby subskrypcji w wybranym zakresie dat.
  - Wykres Mikro przedstawia trend liczby subskrypcji z miesiąca na miesiąc w wybranym zakresie dat.

- Aktywne subskrypcje:
  - Bieżąca liczba subskrypcji produktów w chmurze z aktywnym użyciem mierzona na podstawie telemetrii produktu. Wyklucza to wszystkie subskrypcje wersji próbnej w przypadku subskrypcji platformy Azure.
  - Procentowy wzrost lub spadek liczby aktywnych subskrypcji w wybranym okresie.
  - Wykres Mikro przedstawia trend aktywnych subskrypcji z miesiąca na miesiąc w wybranym zakresie dat.

- Dodane subskrypcje:
  - Łączna liczba subskrypcji klientów dodanych (sprzedanych lub zarządzanych) przez Ciebie w wybranym zakresie dat. Nowe subskrypcje ze **stanem Aktywne** **lub** Odnowione są liczone jako dodane subskrypcje.
  - Procentowy wzrost lub spadek liczby subskrypcji dodanych w ostatnim pełnym miesiącu w porównaniu do pierwszego pełnego miesiąca.
  - Wykres Mikro przedstawia miesięczny trend subskrypcji dodanych w wybranym zakresie dat.

- Subskrypcje z rezygnacjami:
  - Łączna liczba subskrypcji klientów w wybranym zakresie dat. Subskrypcje z **anulowaną aprowizą stanu** **lub** wstrzymaną w tym miesiącu są liczone jako subskrypcja z rezygnacją.  
  - Procent zmian subskrypcji w wybranym zakresie dat.
  - Wykres Mikro przedstawia miesięczny trend zmian subskrypcji w wybranym zakresie dat.

- Subskrypcje według produktów: podział bieżącej liczby subskrypcji według produktów w chmurze.

## <a name="geographical-spread-of-subscriptions"></a>Geograficzny rozrzut subskrypcji

Widok **Subskrypcje według lokalizacji geograficznej** pokazuje geograficzny rozkład łącznej liczby subskrypcji według rynków klientów. Łączna kwota subskrypcji obejmuje zarówno sprzedane subskrypcje, jak i aktywne subskrypcje.

Tabela **Liczba krajów/regionów** przedstawia łączną liczbę krajów/regionów, w których masz subskrypcje, oraz kwotę na kraj całkowitej i aktywnej subskrypcji.

Możesz wyszukać i wybrać kraj w siatce, aby powiększyć lokalizację na mapie. Naciśnij opcję **Strona** główna na mapie, aby przywrócić oryginalny widok. Umieść kursor na mapie, aby wyświetlić wszystkie subskrypcje i aktywne subskrypcje według kraju. Oba pola w siatce można sortować.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="subskrypcje według lokalizacji geograficznej":::

## <a name="subscription-addschurns"></a>Subskrypcje są dorzucane/rezygnacje

Ten widok przedstawia trend subskrypcji. Są one podzielone na różne kategorie (Nowy, Istniejący, Rezygnacje) dla wybranego zakresu dat. Oś X reprezentuje miesiące wybranego zakresu dat. Oś Y reprezentuje liczbę subskrypcji. Subskrypcje z rezygnacjami są reprezentowane w ujemnej skali osi Y. 

Skumulowany wykres kolumnowy przedstawia podział nowych, istniejących i rezygnacji subskrypcji dla miesiąca. Możesz ponownie skompilować wykres kolumnowy z podziałem na określone elementy stosu. W tym celu wybierz te konkretne elementy w legendzie. Możesz również użyć suwaka w górnej części wykresu, aby powiększyć określony okres.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="subskrypcje są dorzucane i rezygnacje":::

## <a name="subscription-distribution"></a>Dystrybucja subskrypcji

Ten widok przedstawia podział bieżących subskrypcji według lokalizacji MPN, segmentów klientów, kanału sprzedaży/modelu cen platformy Azure oraz typu przypisania (na przykład DPOR, DAP i inne). Wybierz odpowiednie karty, aby wyświetlić podział według tych kategorii. Aby utworzyć wykres kołowy z podziałem określonych kategorii elementów, wybierz te kategorie elementów w legendzie.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="dystrybucja subskrypcji":::

## <a name="subscription-state-distribution"></a>Dystrybucja stanu subskrypcji

Ten widok przedstawia rozkład bieżących subskrypcji klientów według stanu lub stanu subskrypcji. Obejmuje to następujące stany subskrypcji: **Aktywne,** **Wyłączone,** **Coprowizowane,** **Otwarte,** **InGracePeriod,** **Zamknięte** i **Inne.**

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="dystrybucja stanu subskrypcji":::

## <a name="products-trend"></a>Trend produktów

Ten widok przedstawia wykres słupkowy i dwa wykresy kołowe. Wykres słupkowy przedstawia miesięczny trend subskrypcji z podziałem na produkty komercyjne, takie jak Azure, Office, Dynamics itp.

Dwa wykresy kołowe pokazują podział bieżących subskrypcji klientów. Pierwszy wykres kołowy dzieli subskrypcje według produktów. Drugi wykres kołowy dzieli subskrypcje według jednostki SKU lub planów. Po wybraniu produktu na wykresie kołowym **podział** według produktów sąsiadujące wykres kołowy zawiera podział subskrypcji tego produktu według jednostki SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="trend produktów":::

> [!NOTE]
 > Liczba subskrypcji z podziałem na jednostki SKU nie zawsze może być taka, jak łączna liczba subskrypcji dla tego produktu. Może się to zdarzyć, jeśli klient zakupił wiele jednostki SKU w ramach tej samej subskrypcji produktu.

## <a name="next-steps"></a>Następne kroki

- Aby uzyskać więcej raportów, [zobacz Partner Center Insights.](partner-center-insights.md)

>[!NOTE] 
> Możesz pobrać nieprzetworzone dane, które będą zasilać ten raport, z sekcji Pobieranie raportów na pulpicie nawigacyjnym szczegółowych informacji. [Więcej informacji](pci-download-reports.md) 
