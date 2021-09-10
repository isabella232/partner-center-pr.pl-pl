---
title: Partner Center Szczegółowe informacje
description: Zapoznaj się z Partner Center ujednoliconym pulpitem nawigacyjnym raportowania. Zobacz, jak radzisz sobie z wskaźnikami KPI dla sprzedaży i wdrażania, rozwoju klientów i nie tylko.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 2061286ecb048647d666438a34b4759175b7deb4
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958293"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partner Center Szczegółowe informacje — pulpit nawigacyjny, który pokazuje, jak działa partner komercyjny firmy Microsoft

**Odpowiednie role:** Administrator globalny | Konto administratora | Przeglądarka raportów dla kierownictwa | Przeglądarka raportów

## <a name="introduction"></a>Wprowadzenie

Pulpit Szczegółowe informacje nawigacyjny jest ujednoliconym pulpitem nawigacyjnym raportowania w usłudze Partner Center dla partnerów komercyjnych firmy Microsoft zarejestrowanych w programie Microsoft Partner Network (MPN). Pulpit Szczegółowe informacje nawigacyjny zapewnia 360-stopniowy widok kluczowych wskaźników wydajności (KPI) dla produktów w chmurze, takich jak Office, Azure, Dynamics i modeli licencjonowania, takich jak CSP i EA. Udostępnia ona bogaty zestaw raportów kluczowych wskaźników wydajności, które mogą ułatwić podejmowanie decyzji dotyczących danych w organizacji. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Kontrola dostępu oparta na rolach do pulpitu Szczegółowe informacje nawigacyjnego

Istnieją dwie nowe role w programie Partner Center przeznaczone specjalnie do uzyskiwania dostępu do **Szczegółowe informacje:** Podgląd raportów i **Executive Report Viewer.** Użytkownicy z rolą Executive Report Viewer mają dostęp do wszystkich zestawów danych raportowania, natomiast użytkownicy w roli Osoby wyświetlającego raporty nie będą mieć dostępu do poufnych zestawów danych, takich jak dane osobowe klientów/pracowników. 

Administrator globalny lub administrator konta może przypisać użytkownikom te role i są przypisani do całej firmy lub dla określonej lokalizacji MPN.  

>[!Note] 
>Użytkownicy, którzy byli administratorami MPN od 20 stycznia 2020 r., zostali automatycznie dodani do roli przeglądarki raportów dla całej firmy. Mogą oni uzyskać dostęp do raportów jako przeglądarki raportów bez żadnej jawnej akcji wymaganej przez administratora globalnego lub administratora konta. Administratorzy globalni lub administratorzy kont mogą w razie potrzeby przesłonić te przypisania. 

## <a name="reports-available"></a>Dostępne raporty

Poniższe raporty są dostępne w ramach pulpitu Szczegółowe informacje nawigacyjnego.

**Przegląd:** Raport Przegląd przedstawia widok migawek różnych kluczowych wskaźników wydajności, takich jak liczba klientów, liczba aktywnych subskrypcji, przychód z użycia platformy Azure, aktywne licencje itp.

**Klient:** Raport Klienta przedstawia analizy dotyczące klientów, takie jak dane pozyskiwania klientów, aktywni klienci itp.

**Produkt — subskrypcje:** Raport Subskrypcje przedstawia analizę pozyskiwania i użycia dla subskrypcji w chmurze (takich jak usługi O365, Azure, Dynamics itp.)

**Licencje produktów:** pulpit nawigacyjny Licencje przedstawia analizę licencji dla opartych na licencjach produktów w chmurze, takich jak O365, Dynamics, Power BI itp.

**Produkt — użycie platformy Azure:** Raport Użycia platformy Azure przedstawia metryki związane z subskrypcjami platformy Azure klientów, w tym przychody z użycia platformy Azure i użycie według kategorii mierników.

**Kompetencje:** Raport Kompetencje przedstawia metryki dotyczące kompetencji aktywnych, kwalifikowanych i zagrożonych.

**Korzyści:** Raport Korzyści przedstawia analizę korzyści dla partnerów, które zostały uzyskane, a które zostały zużyte.

## <a name="navigating-the-insights-reports"></a>Nawigowanie po Szczegółowe informacje raportów

**Filtry zakresu dat:** wybór zakresu dat można znaleźć w prawym górnym rogu każdej strony. Dane wyjściowe wykresów stron przeglądu można dostosować, wybierając zakres dat na podstawie ostatnich 3, 6 lub 12 miesięcy albo wybierając niestandardowy zakres dat. Domyślny zakres dat to 12 miesięcy. 

:::image type="content" source="images/insights/introduction.png" alt-text="Mapa wprowadzenia.":::

**Przycisk opinii:** każdy wykres/kontrolka we wszystkich raportach Szczegółowe informacje jest uwzględniany za pomocą przycisku opinii, aby można było przekazać opinię o wystąpieniu funkcji raportu. 

 
**Filtry na poziomie strony:** z wyjątkiem raportów Przegląd, Korzyści i Kompetencje wszystkie raporty Szczegółowe informacje umożliwiają stosowanie filtrów na poziomie strony. 

- Wybrane filtry będą stosowane do wszystkich wykresów i metryk na stronie, w tym do sekcji podsumowania. Element filtru będzie dostępny, jeśli masz jakiekolwiek dane w ramach tych kryteriów filtrowania. 

- Domyślnym wyborem każdej listy filtrów jest **.** Jeśli na przykład nie wybrano określonego produktu w filtrze produktów, domyślnym wyborem będą wszystkie produkty.

- Wybrane filtry będą wyświetlane w górnej części strony. 

:::image type="content" source="images/insights/filters.png" alt-text="Częściowy zrzut ekranu przedstawiający pasek Zastosowane filtry z wyborami filtrów dla produktów, rynków klienta, autorstwa partnerów i kanałów sprzedaży.":::

### <a name="filters-definitions"></a>Definicje filtrów:

- Produkty: lista wszystkich produktów w chmurze firmy Microsoft sprzedanych/zarządzanych przez organizację, na przykład O365, Azure, D365, EMS, Power BI itp.
- Rynki klientów: lista krajów klientów
- Przypisania partnerów: Typ skojarzenia z subskrypcjami klientów, na przykład Cyfrowy partner rekordu (DPOR), delegowane uprawnienia administratora (DAP) i link administratora partnera ( PAL). 
- Lokalizacje partnerów: lista wszystkich lokalizacji MPN w organizacji.
- Kanały sprzedaży: wszystkie kanały sprzedaży/ceny, za pośrednictwem których kupujesz/aprowizujesz produkty i usługi, to znaczy CSP, EA, CSP indirect, Direct, Advisor, Open, inne
- Segmenty klientów: lista segmentów klientów w obrębie bazy klientów partnerów.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Przeczytaj o każdym z pulpitów nawigacyjnych i raportów:

- [Partner Center Szczegółowe informacje — omówienie pulpitu nawigacyjnego](insights-overview-report.md)

- [Partner Center Szczegółowe informacje — pulpit nawigacyjny klienta](insights-customer-report.md)

- [Partner Center Szczegółowe informacje — raport subskrypcji](insights-product-subscriptions-report.md)

- [Partner Center Szczegółowe informacje — raport licencje](insights-product-licenses-report.md)

- [Partner Center Szczegółowe informacje — raport użycia platformy Azure](insights-azure-usage-report.md)

- [Partner Center Szczegółowe informacje — raport kompetencji](insights-competencies-report.md)

- [Partner Center Szczegółowe informacje — raport korzyści](insights-benefits-report.md)
