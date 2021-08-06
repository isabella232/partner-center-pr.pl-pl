---
title: Partner Center Szczegółowe informacje subskrypcji
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Sprawdź, co robisz dobrze i gdzie możesz ulepszyć subskrypcje w chmurze, które sprzedajesz klientom lub zarządzasz nimi.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e77452a5715b0953852c5efc1f36e8f801d87993334049aaa0a905439abc8f0c
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115678468"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Raport subskrypcje produktów dostępny na pulpicie nawigacyjnym Partner Center Szczegółowe informacje nawigacyjnym

**Odpowiednie role:** Administrator globalny | Agent administracyjny | Przeglądarka raportów | Przeglądarka raportów dla kierownictwa

Raport Subskrypcje produktów przedstawia analizę subskrypcji w chmurze, które zostały sprzedane lub które zarządzasz dla klientów. Jest to raport specyficzny dla produktu, który obejmuje wydajność subskrypcji skojarzonych z produktami w chmurze, takimi jak Office 365, Azure, Dynamics i inne.

Poniższe sekcje można wyświetlić w raporcie Subskrypcje produktów.

- Podsumowanie
- Geograficzny rozrzut subskrypcji
- Trend dodawania/rezygnacji subskrypcji
- Dystrybucja subskrypcji według lokalizacji partnerów, kanału sprzedaży, jednostki SKU, typ dołączania partnera, segment
- Trend według stanów subskrypcji
- Trend produktów

 > [!NOTE]
 > Ten raport jest dostępny na pulpicie Szczegółowe informacje nawigacyjnym. Aby wyświetlić ten raport, musisz mieć przypisaną określoną rolę w programie Partner Center, taką jak Administrator globalny, Administrator konta, Przeglądarka raportów lub Przeglądarka raportów kierownictwa. Aby uzyskać więcej informacji, zobacz Administrator globalny twojej firmy. Określone typy danych w tym raporcie mogą być również dostępne tylko dla użytkowników z uprawnieniami do przeglądarki raportów executive.

## <a name="summary"></a>Podsumowanie

Sekcja podsumowania przedstawia widok migawki kluczowych wskaźników wydajności (KPI) związanych z subskrypcjami sprzedanymi lub zarządzanymi przez Ciebie dla klientów.  

:::image type="content" source="images/insights/sub-report-summary.png" alt-text="podsumowanie raportu subskrypcji.":::

Aby uzyskać więcej informacji na temat każdej sekcji podsumowania, zobacz poniżej:

- Subskrypcje:
  - Bieżąca liczba subskrypcji produktów w chmurze sprzedanych lub zarządzanych przez Ciebie.
  - Procent wzrostu lub spadku liczby subskrypcji w wybranym zakresie dat.
  - Wykres Mikro przedstawia trend liczby subskrypcji z miesiąca na miesiąc w wybranym zakresie dat.

- Aktywne subskrypcje:
  - Bieżąca liczba subskrypcji produktów w chmurze z aktywnym użyciem mierzona na podstawie telemetrii produktu. Wyklucza to wszystkie subskrypcje wersji próbnej dla subskrypcji platformy Azure.
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

Możesz wyszukać i wybrać kraj w siatce, aby powiększyć lokalizację na mapie. Naciśnij opcję **Strona główna** na mapie, aby przywrócić oryginalny widok. Umieść kursor na mapie, aby wyświetlić wszystkie subskrypcje i aktywne subskrypcje według kraju. Oba pola w siatce można sortować.

:::image type="content" source="images/insights/sub-report-sub-by-geography.png" alt-text="subskrypcje według lokalizacji geograficznej.":::

## <a name="subscription-addschurns"></a>Dodanie/rezygnacje subskrypcji

Ten widok przedstawia trend subskrypcji. Są one podzielone na różne kategorie (Nowy, Istniejący, Rezygnacje) dla wybranego zakresu dat. Oś X reprezentuje miesiące wybranego zakresu dat. Oś Y reprezentuje liczbę subskrypcji. Subskrypcje z rezygnacjami są reprezentowane w ujemnej skali osi Y. 

Skumulowany wykres kolumnowy przedstawia podział nowych, istniejących i przechyconych subskrypcji dla miesiąca. Możesz ponownie skompilować wykres kolumnowy z podziałem na określone elementy stosu. W tym celu wybierz te określone elementy w legendzie. Możesz również użyć suwaka w górnej części wykresu, aby powiększyć widok do określonego okresu.

:::image type="content" source="images/insights/sub-report-sub-adds-churns.png" alt-text="subskrypcja dodaje i zwiększa rezygnacje.":::

## <a name="subscription-distribution"></a>Dystrybucja subskrypcji

Ten widok przedstawia podział bieżących subskrypcji według lokalizacji Microsoft Partner Network (MPN), segmentów klientów, kanału sprzedaży/modelu cen platformy Azure oraz typu przypisania. Wybierz odpowiednie karty, aby wyświetlić podział według tych kategorii. Aby utworzyć wykres kołowy z podziałem określonych kategorii elementów, wybierz te kategorie elementów w legendzie.

:::image type="content" source="images/insights/sub-report-distribution.png" alt-text="dystrybucja subskrypcji.":::

## <a name="subscription-state-distribution"></a>Dystrybucja stanu subskrypcji

Ten widok przedstawia rozkład bieżących subskrypcji klientów według stanu lub stanu subskrypcji. Obejmuje to następujące stany subskrypcji: **Aktywne,** **Wyłączone,** **Coprowizowane,** **Otwarte,** **InGracePeriod,** **Zamknięte** i **Inne.**

:::image type="content" source="images/insights/sub-report-sub-states.png" alt-text="dystrybucja stanu subskrypcji.":::

## <a name="products-trend"></a>Trend produktów

Ten widok przedstawia wykres słupkowy i dwa wykresy kołowe. Wykres słupkowy przedstawia miesięczny trend subskrypcji z podziałem na produkty komercyjne, takie jak azure, Office i Dynamics.

Dwa wykresy kołowe pokazują podział bieżących subskrypcji klientów. Pierwszy wykres kołowy dzieli subskrypcje według produktów. Drugi wykres kołowy dzieli subskrypcje według jednostki SKU lub planów. Po wybraniu produktu na wykresie kołowym **podział** według produktów sąsiadujące wykres kołowy zawiera podział subskrypcji tego produktu według jednostki SKU.

:::image type="content" source="images/insights/sub-report-prods-trend.png" alt-text="trend produktów.":::

> [!NOTE]
 > Liczba subskrypcji z podziałem na jednostki SKU nie zawsze może być taka, jak łączna liczba subskrypcji dla tego produktu. Może się to zdarzyć, jeśli klient zakupił wiele jednostki SKU w ramach tej samej subskrypcji produktu.

## <a name="next-steps"></a>Następne kroki

- Aby uzyskać więcej raportów, [zobacz Partner Center Szczegółowe informacje](partner-center-insights.md).

>[!NOTE] 
> Możesz pobrać nieprzetworzone dane, które będą zasilać ten raport, z sekcji Pobieranie raportów na Szczegółowe informacje nawigacyjnym. [Więcej informacji](insights-download-reports.md) 
