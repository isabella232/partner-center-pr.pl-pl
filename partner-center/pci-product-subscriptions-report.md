---
title: Raport dotyczący subskrypcji usługi Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zapoznaj się z tym, co robisz, i w jaki sposób możesz ulepszyć subskrypcje w chmurze, które są sprzedawane klientom lub którymi chcesz zarządzać.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 019e489b4738515639bf181591dfbc671e1b795d
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086196"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Raport subskrypcje produktów dostępny na pulpicie nawigacyjnym usługi Partner Center Insights

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny
- Podgląd raportów
- Executive — Podgląd raportów

Raport subskrypcje produktów przedstawia analizę w ramach subskrypcji w chmurze sprzedawanych przez użytkownika lub zarządzanych przez klientów. Jest to raport specyficzny dla produktu, który obejmuje wydajność subskrypcji skojarzonych z produktami w chmurze, takimi jak Office 365, Azure, Dynamics i innych.

Poniższe sekcje można wyświetlić w raporcie subskrypcje produktów.

- Podsumowanie
- Geograficzne rozmieszczenie subskrypcji
- Trend dodawania/zmiany subskrypcji
- Dystrybucja subskrypcji według lokalizacji partnerów, kanału sprzedaży, jednostek SKU, typu dołączania partnera, segmentu
- Trend według stanów subskrypcji
- Trend produktów

 > [!NOTE]
 > Ten raport jest dostępny na pulpicie nawigacyjnym usługi Insights. Aby wyświetlić ten raport, musisz mieć przypisaną określoną rolę w centrum partnerskim, takim jak Administrator globalny, administrator konta, Podgląd raportów lub dyrektor raportów programu. Aby uzyskać więcej informacji, zobacz Administrator globalny firmy. określone typy danych w tym raporcie mogą być również dostępne tylko dla użytkowników z uprawnieniami dyrektora raportów.

## <a name="summary"></a>Podsumowanie

Sekcja podsumowania przedstawia widok migawki kluczowych wskaźników wydajności (KPI) związanych z subskrypcjami sprzedawanymi lub zarządzanymi przez klientów.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Podsumowanie raportu dotyczącego subskrypcji":::

Aby uzyskać więcej informacji na temat każdej sekcji podsumowania, zobacz poniżej:

- Subskrypcje:
  - Bieżąca liczba subskrypcji produktu w chmurze sprzedawanych lub zarządzanych przez użytkownika.
  - Procent wzrostu lub odrzucania subskrypcji w wybranym zakresie dat.
  - Na mikrografie prezentowany jest trend miesięczny w stosunku do liczby subskrypcji w wybranym zakresie dat.

- Aktywne subskrypcje:
  - Bieżąca liczba subskrypcji produktu w chmurze z aktywnym użyciem mierzonym na podstawie danych telemetrycznych produktu. Spowoduje to wykluczenie wszystkich subskrypcji w wersji próbnej w przypadku subskrypcji platformy Azure.
  - Procent wzrostu lub odrzucania aktywnych subskrypcji w wybranym okresie.
  - Micro Chart prezentuje trend miesięczny aktywnych subskrypcji w wybranym zakresie dat.

- Dodane subskrypcje:
  - Łączna liczba dodanych subskrypcji klienta (sprzedawanych lub zarządzanych) przez użytkownika w ramach wybranego zakresu dat. Nowe subskrypcje o stanie **aktywny** lub **odnowiony** są zliczane jako dodane subskrypcje.
  - Procent wzrostu lub odrzucenia subskrypcji dodanych w ciągu ostatniego pełnego miesiąca w porównaniu do pierwszego pełnego miesiąca.
  - W programie Micro Chart jest prezentowany miesięczny trend subskrypcji dodanych w ramach wybranego zakresu dat.

- Zmienione subskrypcje:
  - Łączna liczba subskrypcji klientów, które zostały zmienione w wybranym zakresie dat. Subskrypcje z cofniętą obsługą **administracyjną** lub **zawieszoną** w tym miesiącu są zliczane jako zmieniona subskrypcja.  
  - Procent subskrypcji zmienionych w ramach wybranego zakresu dat.
  - W programie Micro Chart jest prezentowany miesięczny trend zmian subskrypcji, które zostały zmienione na wybrany zakres dat.

- Subskrypcje według produktów: podział bieżącej liczby subskrypcji na produkty w chmurze.

## <a name="geographical-spread-of-subscriptions"></a>Geograficzne rozmieszczenie subskrypcji

Widok **subskrypcje według** lokalizacji geograficznej przedstawia dystrybucję geograficzną łącznej liczby subskrypcji według rynków klientów. Łączna kwota subskrypcji obejmuje sprzedane subskrypcje i aktywne subskrypcje.

**Liczba krajów/** regionów w tabeli zawiera łączną liczbę krajów/regionów, w których masz subskrypcje, a także kwotę za kraj z łącznej i aktywnej subskrypcji.

Możesz wyszukać i wybrać kraj w siatce, aby powiększyć do lokalizacji na mapie. Naciśnij pozycję **Strona główna** na mapie, aby powrócić do oryginalnego widoku. Umieść kursor na mapie, aby wyświetlić wszystkie subskrypcje i aktywne subskrypcje według kraju. Oba pola siatki są sortowane.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="subskrypcje według lokalizacji geograficznej":::

## <a name="subscription-addschurns"></a>Dodawanie/zmiany subskrypcji

Ten widok przedstawia trend subskrypcji. Są one podzielone na różne kategorie (nowe, istniejące, zmienione) dla wybranego zakresu dat. Oś X reprezentuje miesiące wybranego zakresu dat. Oś Y reprezentuje liczbę subskrypcji. Zmienione subskrypcje są reprezentowane w ujemnej skali osi Y. 

Skumulowany wykres kolumnowy przedstawia podział nowych, istniejących i zmienionych subskrypcji na miesiąc. Możesz ponownie skompilować wykres kolumnowy, podzielony na określone elementy stosu. Aby to zrobić, wybierz te konkretne elementy w legendzie. Możesz również użyć suwaka na górze wykresu, aby powiększyć do określonego okresu.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="Dodawanie i zmiany subskrypcji":::

## <a name="subscription-distribution"></a>Dystrybucja subskrypcji

Ten widok przedstawia podział bieżących subskrypcji według lokalizacji MPN, segmentów klientów, kanału sprzedaży/modelu cen platformy Azure oraz typu przypisywania (na przykład DPOR, DAP i inne). Wybierz odpowiednie karty, aby wyświetlić podział według tych kategorii. Aby skompilować wykres kołowy z podziałem określonych kategorii elementów, wybierz te kategorie elementów w legendzie.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="Dystrybucja subskrypcji":::

## <a name="subscription-state-distribution"></a>Dystrybucja stanu subskrypcji

Ten widok przedstawia dystrybucję bieżących subskrypcji klienta według stanu subskrypcji lub stanu. Obejmuje to następujące stany subskrypcji: **aktywne**, **wyłączone**, cofnięcie aprowizacji, **otwarte**, **InGracePeriod**, **zamknięte** i **inne**. 

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="Dystrybucja stanu subskrypcji":::

## <a name="products-trend"></a>Trend produktów

Ten widok przedstawia wykres słupkowy i dwa wykresy kołowe. Wykres słupkowy przedstawia miesięczny trend subskrypcji podzielony na produkty komercyjne, takie jak Azure, Office, Dynamics itp.

Dwa wykresy kołowe pokazują podział bieżących subskrypcji klientów. Pierwszy wykres kołowy przerywa subskrypcje według produktów. Drugi wykres kołowy dzieli subskrypcje na jednostki SKU lub plany. Po wybraniu produktu na wykresie kołowym podział **według produktów** , na sąsiednim wykresie kołowym zostanie wyświetlony podział subskrypcji tego produktu według jednostek SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="Trend produktów":::

> [!NOTE]
 > Liczba subskrypcji podzielona przez jednostki SKU może nie zawsze odpowiadać całkowitej liczbie subskrypcji dla tego produktu. Taka sytuacja może wystąpić, jeśli klient kupił wiele jednostek SKU w ramach tej samej subskrypcji produktu.

## <a name="next-steps"></a>Następne kroki

- Więcej raportów można znaleźć w temacie [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Możesz pobrać pierwotne dane, aby wyłączyć ten raport z sekcji Pobieranie raportów na pulpicie nawigacyjnym usługi Insights. [Więcej informacji](pci-download-reports.md) 
