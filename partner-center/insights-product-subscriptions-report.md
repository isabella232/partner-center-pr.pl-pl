---
title: Partner Center Szczegółowe informacje subskrypcji
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Sprawdź, co robisz dobrze i gdzie możesz ulepszyć subskrypcje chmury, które sprzedajesz lub zarządzasz dla swoich klientów.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eefb4f4ee6657acf583ad0b5d4149e662c320184
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114846183"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Raport subskrypcji produktów dostępny na pulpicie nawigacyjnym Partner Center Szczegółowe informacje nawigacyjnym

**Odpowiednie role:** Administrator globalny | Agent administracyjny | Przeglądarka raportów | Przeglądarka raportów dla kierownictwa

Raport Subskrypcje produktów przedstawia analizę subskrypcji w chmurze, które zostały sprzedane lub które zarządzasz dla klientów. Jest to raport specyficzny dla produktu, który obejmuje wydajność subskrypcji skojarzonych z produktami w chmurze, takimi jak Office 365, Azure, Dynamics i inne.

Poniższe sekcje można wyświetlić w raporcie Subskrypcje produktów.

- Podsumowanie
- Geograficzne rozrzuty subskrypcji
- Trend dodawania/rezygnacji subskrypcji
- Dystrybucja subskrypcji według lokalizacji partnerów, kanału sprzedaży, jednostki SKU, typ dołączania partnera, segment
- Trend według stanów subskrypcji
- Trend produktów

 > [!NOTE]
 > Ten raport jest dostępny na pulpicie nawigacyjnym Szczegółowe informacje nawigacyjnym. Aby wyświetlić ten raport, musisz mieć przypisaną określoną rolę w programie Partner Center, taką jak Administrator globalny, Administrator konta, Podgląd raportów lub Przeglądarka raportów kierownictwa. Aby uzyskać więcej informacji, zobacz Administratora globalnego firmy. Określone typy danych w tym raporcie mogą być również dostępne tylko dla użytkowników z uprawnieniami do przeglądarki raportów executive.

## <a name="summary"></a>Podsumowanie

Sekcja podsumowania zawiera widok migawki kluczowych wskaźników wydajności (KPI) związanych z subskrypcjami sprzedawanymi lub zarządzanymi przez Ciebie dla klientów.  

:::image type="content" source="images/insights/sub-report-summary.png" alt-text="podsumowanie raportu subskrypcji.":::

Aby uzyskać więcej informacji na temat każdej sekcji podsumowania, zobacz poniżej:

- Subskrypcje:
  - Bieżąca liczba subskrypcji produktów w chmurze sprzedanych lub zarządzanych przez Ciebie.
  - Procentowy wzrost lub spadek liczby subskrypcji w wybranym zakresie dat.
  - Wykres Mikro przedstawia trend liczby subskrypcji z miesiąca na miesiąc w wybranym zakresie dat.

- Aktywne subskrypcje:
  - Bieżąca liczba subskrypcji produktów w chmurze z aktywnym użyciem mierzonym na podstawie telemetrii produktu. To wyklucza wszystkie subskrypcje wersji próbnej dla subskrypcji platformy Azure.
  - Procentowy wzrost lub spadek liczby aktywnych subskrypcji w wybranym okresie.
  - Wykres Mikro przedstawia trend aktywnych subskrypcji z miesiąca na miesiąc w wybranym zakresie dat.

- Dodane subskrypcje:
  - Łączna liczba subskrypcji klientów dodanych przez Ciebie (sprzedanych lub zarządzanych) w wybranym zakresie dat. Nowe subskrypcje ze **stanem Aktywne** **lub** Odnowione są liczone jako dodane subskrypcje.
  - Procentowy wzrost lub spadek liczby subskrypcji dodanych w ostatnim pełnym miesiącu w porównaniu do pierwszego pełnego miesiąca.
  - Wykres Mikro przedstawia miesięczny trend subskrypcji dodanych w wybranym zakresie dat.

- Subskrypcje z rezygnacją:
  - Łączna liczba rezygnacji subskrypcji klientów w wybranym zakresie dat. Subskrypcje ze stanem **Anulowana aprowizowana** **lub** Wstrzymane w tym miesiącu są liczone jako subskrypcja z rezygnacją.  
  - Procent zmian subskrypcji w wybranym zakresie dat.
  - Wykres Mikro przedstawia miesięczny trend rezygnacji subskrypcji w wybranym zakresie dat.

- Subskrypcje według produktów: podział bieżącej liczby subskrypcji według produktów w chmurze.

## <a name="geographical-spread-of-subscriptions"></a>Geograficzne rozrzuty subskrypcji

Widok **Subskrypcje według lokalizacji** geograficznej pokazuje rozkład geograficzny łącznej liczby subskrypcji według rynków klientów. Łączna kwota subskrypcji obejmuje zarówno sprzedane subskrypcje, jak i aktywne subskrypcje.

Tabela **Liczba krajów/regionów** przedstawia łączną liczbę krajów/regionów, w których masz subskrypcje, oraz kwotę na kraj całkowitej i aktywnej subskrypcji.

Możesz wyszukać i wybrać kraj w siatce, aby powiększyć lokalizację na mapie. Naciśnij opcję **Strona** główna na mapie, aby przywrócić oryginalny widok. Umieść kursor na mapie, aby wyświetlić wszystkie subskrypcje i aktywne subskrypcje według kraju. Oba pola na siatce można sortować.

:::image type="content" source="images/insights/sub-report-sub-by-geography.png" alt-text="subskrypcje według lokalizacji geograficznej.":::

## <a name="subscription-addschurns"></a>Subskrypcje — dodaje/churns

Ten widok przedstawia trend subskrypcji. Są one podzielone na różne kategorie (Nowy, Istniejący, Rezygnacje) dla wybranego zakresu dat. Oś X reprezentuje miesiące z wybranego zakresu dat. Oś Y reprezentuje liczbę subskrypcji. Subskrypcje z rezygnacjami są reprezentowane w ujemnej skali osi Y. 

Skumulowany wykres kolumnowy przedstawia podział nowych, istniejących i rezygnacji subskrypcji dla miesiąca. Możesz ponownie skompilować wykres kolumnowy z podziałem na określone elementy stosu. Aby to zrobić, wybierz te konkretne elementy w legendzie. Możesz również użyć suwaka w górnej części wykresu, aby powiększyć określony okres.

:::image type="content" source="images/insights/sub-report-sub-adds-churns.png" alt-text="subskrypcja dodaje i churns.":::

## <a name="subscription-distribution"></a>Dystrybucja subskrypcji

Ten widok przedstawia podział bieżących subskrypcji według lokalizacji usługi Microsoft Partner Network (MPN), segmentów klientów, kanału sprzedaży/modelu cen platformy Azure i typu przypisania. Wybierz odpowiednie karty, aby wyświetlić podział według tych kategorii. Aby utworzyć wykres kołowy z podziałem na kategorie określonych elementów, wybierz te kategorie elementów w legendzie.

:::image type="content" source="images/insights/sub-report-distribution.png" alt-text="dystrybucja subskrypcji.":::

## <a name="subscription-state-distribution"></a>Dystrybucja stanu subskrypcji

Ten widok przedstawia dystrybucję bieżących subskrypcji klientów według stanu lub stanu subskrypcji. Obejmuje to następujące stany subskrypcji: **Aktywne,** **Wyłączone,** **Coprovisioned,** **Open,** **InGracePeriod,** **Closed** i **inne.**

:::image type="content" source="images/insights/sub-report-sub-states.png" alt-text="dystrybucja stanu subskrypcji.":::

## <a name="products-trend"></a>Trend produktów

Ten widok przedstawia wykres słupkowy i dwa wykresy kołowe. Wykres słupkowy przedstawia miesięczny trend subskrypcji z podziałem na produkty komercyjne, takie jak azure, Office i Dynamics.

Dwa wykresy kołowe pokazują podział bieżących subskrypcji klientów. Pierwszy wykres kołowy dzieli subskrypcje według produktów. Drugi wykres kołowy dzieli subskrypcje według jednostki SKU lub planów. Po wybraniu produktu na wykresie kołowym **Podział** według produktów na sąsiednim wykresie kołowym zostanie pokazany podział subskrypcji tego produktu według jednostki SKU.

:::image type="content" source="images/insights/sub-report-prods-trend.png" alt-text="trend produktów.":::

> [!NOTE]
 > Liczba subskrypcji z podziałem na jednostki SKU nie zawsze może być taka, jak łączna liczba subskrypcji dla tego produktu. Może się to zdarzyć, jeśli klient zakupił wiele jednostki SKU w ramach tej samej subskrypcji produktu.

## <a name="next-steps"></a>Następne kroki

- Aby uzyskać więcej raportów, [zobacz Partner Center Szczegółowe informacje](partner-center-insights.md).

>[!NOTE] 
> Możesz pobrać nieprzetworzone dane, które są zasilane z tego raportu, z sekcji Pobieranie raportów na pulpicie Szczegółowe informacje nawigacyjnym. [Więcej informacji](insights-download-reports.md) 
