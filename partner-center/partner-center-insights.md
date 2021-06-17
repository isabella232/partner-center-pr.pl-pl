---
title: Partner Center Insights
description: Zapoznaj się z tym Partner Center ujednoliconym pulpitem nawigacyjnym raportowania. Zobacz, jak radzisz sobie z wskaźnikami KPI dla sprzedaży i wdrażania, rozwoju klientów i nie tylko.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 05fad9c7eecbc8b7f639faa24b654fb0474245ca
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277627"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partner Center Insights — pulpit nawigacyjny, który pokazuje, jak działa partner komercyjny firmy Microsoft

**Odpowiednie role:** Administrator globalny | Administrator konta | Przeglądarka raportów dla kierownictwa | Przeglądarka raportów

## <a name="introduction"></a>Wprowadzenie

Pulpit nawigacyjny usługi Insights to ujednolicony pulpit nawigacyjny raportowania w usłudze Partner Center dla partnerów komercyjnych firmy Microsoft zarejestrowanych w programie Microsoft Partner Network (MPN). Pulpit nawigacyjny usługi Insights zapewnia 360-stopniowy widok kluczowych wskaźników wydajności (KPI) dla produktów w chmurze, takich jak office, Azure, Dynamics i modeli licencjonowania, takich jak CSP i EA. Udostępnia ona bogaty zestaw raportów kluczowych wskaźników wydajności, które mogą ułatwić podejmowanie decyzji opartych na danych dla organizacji. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Kontrola dostępu oparta na rolach do pulpitu nawigacyjnego szczegółowych informacji

Istnieją dwie nowe role w programie Partner Center przeznaczone specjalnie do uzyskiwania dostępu do szczegółowych **informacji:** Podgląd raportów i **Executive Report Viewer.** Użytkownicy z rolą Executive Report Viewer mają dostęp do wszystkich zestawów danych raportowania, natomiast użytkownicy z rolą Osoby wyświetlającego raporty nie będą mieć dostępu do poufnych zestawów danych, takich jak dane osobowe przychodów i klientów/pracowników. 

Administrator globalny lub administrator konta może przypisać użytkownikom te role i są przypisani do całej firmy lub dla określonej lokalizacji MPN.  

>[!Note] 
>Użytkownicy, którzy byli administratorami MPN od 20 stycznia 2020 r., zostali automatycznie dodani do roli przeglądarki raportów dla całej firmy. Mogą oni uzyskać dostęp do raportów jako przeglądarki raportów bez żadnej jawnej akcji wymaganej przez administratora globalnego lub administratora konta. Administratorzy globalni lub administratorzy kont mogą w razie potrzeby przesłonić te przypisania. 

## <a name="reports-available"></a>Dostępne raporty

Następujące raporty są dostępne w ramach pulpitu nawigacyjnego szczegółowych informacji.

**Przegląd:** Raport Przegląd przedstawia widok migawki różnych kluczowych wskaźników wydajności, takich jak liczba klientów, liczba aktywnych subskrypcji, przychód z użycia platformy Azure, aktywne licencje itp.

**Klient:** Raport klienta przedstawia analizy dotyczące klientów, takie jak dane pozyskiwania klientów, aktywni klienci itp.

**Produkt — Subskrypcje:** Raport Subskrypcje przedstawia analizę pozyskiwania i użycia dla subskrypcji w chmurze (takich jak usługi O365, Azure, Dynamics itp.)

**Licencje produktów:** pulpit nawigacyjny Licencje przedstawia analizę licencji dla opartych na licencjach produktów w chmurze, takich jak O365, Dynamics, Power BI itp.

**Produkt — użycie platformy Azure:** Raport Użycia platformy Azure przedstawia metryki związane z subskrypcjami platformy Azure klientów, w tym przychody użycia platformy Azure i użycie według kategorii mierników.

**Kompetencje:** Raport Kompetencje przedstawia metryki dotyczące kompetencji aktywnych, kwalifikowanych i zagrożonych.

**Korzyści:** Raport Korzyści przedstawia analizę korzyści, które zostały uzyskane przez partnerów w porównaniu z ich wykorzystaniem.

## <a name="navigating-the-insights-reports"></a>Nawigowanie po raportach szczegółowych informacji

**Filtry zakresu dat:** wybór zakresu dat można znaleźć w prawym górnym rogu każdej strony. Dane wyjściowe wykresów stron przeglądu można dostosować, wybierając zakres dat na podstawie ostatnich 3, 6 lub 12 miesięcy albo wybierając niestandardowy zakres dat. Domyślny zakres dat to 12 miesięcy. 

:::image type="content" source="images/pci/intro1.png" alt-text="Mapa wprowadzenia.":::

**Przycisk Opinii:** każdy wykres/kontrolka we wszystkich raportach szczegółowych informacji jest uwzględniany za pomocą przycisku opinii, aby można było przekazać opinię o wystąpieniu funkcji raportu. 

 
**Filtry na poziomie strony:** z wyjątkiem raportów Przegląd, Korzyści i Kompetencje wszystkie raporty szczegółowych informacji umożliwiają stosowanie filtrów na poziomie strony. 

- Wybrane filtry będą stosowane do wszystkich wykresów i metryk na stronie, w tym sekcji podsumowania. Element filtru będzie dostępny, jeśli masz dane w ramach tych kryteriów filtrowania. 

- Domyślnym wyborem każdej listy filtrów jest **.** Jeśli na przykład nie wybrano określonego produktu w filtrze products, domyślnym wyborem będą wszystkie produkty.

- Wybrane filtry będą wyświetlane w górnej części strony. 

:::image type="content" source="images/pci/filters.png" alt-text="Częściowy zrzut ekranu przedstawiający pasek Zastosowane filtry z wyborami filtrów dla produktów, rynków klienta, autorstwa partnerów i kanałów sprzedaży.":::

### <a name="filters-definitions"></a>Definicje filtrów:

- Produkty: lista wszystkich produktów w chmurze firmy Microsoft sprzedawanych/zarządzanych przez organizację, na przykład O365, Azure, D365, EMS, Power BI itp.
- Rynki klientów: Lista krajów klientów
- Przypisania partnerów: Typ skojarzenia z subskrypcjami klientów, na przykład Cyfrowy partner rekordów (DPOR), Delegowane uprawnienia administratora (DAP) i Link administratora partnera (PAL). 
- Lokalizacje partnerów: lista wszystkich lokalizacji MPN w organizacji.
- Kanały sprzedaży: wszystkie kanały sprzedaży/ceny, za pośrednictwem których kupujesz/aprowizujesz produkty i usługi, a mianowicie CSP, EA, CSP indirect, Direct, Advisor, Open, inne
- Segmenty klientów: lista segmentów klientów w bazie klientów partnerów.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Przeczytaj o każdym z pulpitów nawigacyjnych i raportów:

- [Partner Center Insights — omówienie pulpitu nawigacyjnego](pci-overview-report.md)

- [Partner Center Insights — pulpit nawigacyjny klienta](pci-customer-report.md)

- [Partner Center Insights — raport subskrypcji](pci-product-subscriptions-report.md)

- [Partner Center Insights — raport licencji](pci-product-licenses-report.md)

- [Partner Center Insights — raport użycia platformy Azure](pci-azure-usage-report.md)

- [Partner Center Insights — raport kompetencji](pci-competencies-report.md)

- [Partner Center Insights — raport korzyści](pci-benefits-report.md)
