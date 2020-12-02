---
title: Korzystanie z usługi Partner Center Analytics na potrzeby Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak wyświetlać dane biznesowe za pomocą aplikacji analizy Centrum partnerskiego dla Power BI (dla partnerów bezpośrednich w dostawcy CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/14/2020
ms.locfileid: "92529207"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Wyświetl dane biznesowe za pomocą aplikacji analizy Centrum partnerskiego dla firmy Microsoft Power BI

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Administrator globalny
- Administrator użytkowników
- Agent sprzedaży
- Agent administracyjny

## <a name="view-your-business-data"></a>Wyświetlanie danych firmy

Uzyskaj wizualną reprezentację danych biznesowych za pomocą aplikacji do analizy Centrum partnerskiego dla Power BI, w tym:

- Rozwój bazy klientów, subskrypcji i licencji

- Użycie pakietu Office 365, Microsoft Dynamics i produktów Microsoft Azure

- Dzienne jednostki zużycia dla każdego zmierzonego zasobu w każdej subskrypcji platformy Azure w ciągu ostatnich 60 dni

- Szacowany koszt (na podstawie karty z najnowszą stawką)

- Możliwość eksportowania zestawów danych i tworzenia niestandardowych raportów, w tym na klientach.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Informacje o wersji zapoznawczej aplikacji Centrum partnerskiego

- Ta aplikacja jest tylko dla partnerów bezpośrednich w programie dostawcy rozwiązań w chmurze. Inni partnerzy w programie CSP (na przykład pośrednim odsprzedawcy) nie będą mogli się zalogować.

- Wszystkie szacowane koszty to dane dotyczące rozliczeń i fakturowania przed opodatkowaniem i nie są prawnie wiążące. Szacowane koszty są przeznaczone do użycia tylko na potrzeby wglądu w dane.

- Informacje o klientach są oparte na subskrypcjach. Wszyscy klienci, dla których utworzono ostatnio konta, ale którzy nie mają jeszcze subskrypcji, nie są włączeni do liczności.

- Szacowany koszt jest oparty na karcie z najnowszą stawką, która jest oparta na cenach dostawcy CSP.

- Liczba dni to dni kalendarzowe.

### <a name="business-insights-report"></a>Raport dotyczący usługi Business Insights

- **Dzierżawy klientów**: liczba różnych dzierżaw usługi Azure AD klientów, którzy kupili subskrypcje

- **Nowe (ostatnie 30 dni)**: nowi klienci kupują co najmniej jedną subskrypcję w ciągu ostatnich 30 dni

- Zmiany **(ostatnie 30 dni)**: klienci bez żadnej "aktywne", "z wyprzedzeniem" lub "wyłączone"

- **Nowość (ostatnie 24 godziny)**: nowi klienci kupują co najmniej jedną subskrypcję w ciągu ostatnich 24 godzin

- **Szacowany miesięczny koszt w ciągu ostatnich 12 miesięcy**: trend między miesiącami w przypadku szacowanej kwoty dolara za faktury przed opodatkowaniem, zagregowany miesięcznie w okresie ostatnich 12 miesięcy

- **Szacowany koszt według produktu w ciągu ostatnich 12 miesięcy**: produkty sprzedane według szacowanej kwoty dolara faktury przed opodatkowaniem zagregowanej w okresie ostatnich 12 miesięcy. Ten stan wskazuje na Najpopularniejsze produkty z największą ilością przychodów.

- **Klienci w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych klientów i zmiany klientów zagregowanych miesięcznie w okresie ostatnich 12 miesięcy

- **Szacowany koszt przez klienta w ciągu ostatnich 12 miesięcy**: klienci posortowani według szacowanej kwoty dolara za faktury przed opodatkowaniem w okresie ostatnich 12 miesięcy. Ten stan oznacza, że klienci najczęściej mają najwięcej przychodów.

- **Liczba klientów według produktu**: produkty sprzedawane posortowane przez skojarzonych klientów. Ten stan wskazuje Najpopularniejsze produkty sprzedawane większości klientów.

### <a name="subscription-insights-report"></a>Raport usługi Subscription Insights

- **Stan subskrypcji**:

- Aktywne: subskrypcje należące do "Active" lub "w stanie prolongaty"

  - Zawieszone: subskrypcje należące do stanu "wyłączone"

  - Cofnięto Inicjowanie obsługi: subskrypcje należące do stanu "de-provisioned" lub "wygasłe"

- **Stan wygaśnięcia**:

  - Wygasłe: subskrypcje, które już wygasły (Data zakończenia subskrypcji przypada w przeszłości)

  - Wygasa po 30 dniach: subskrypcje wygaśnie po upływie 30 dni (w przypadku których data zakończenia subskrypcji będzie późniejsza niż 30 dni)

  - Wygasa za 30 dni: subskrypcje wygaśnie w ciągu następnych 30 dni (w przypadku których data zakończenia subskrypcji przypada między dzisiaj a 30 dni)

- **Łączna liczba subskrypcji**: subskrypcje w "aktywny," "w stanie prolongaty" lub "wyłączone"

- **Nowe (ostatnie 30 dni)**: nowe subskrypcje zakupione przez klientów w ciągu ostatnich 30 dni

- **Nowość (ostatnie 24 godziny)**: nowe subskrypcje zakupione przez klientów w ciągu ostatnich 24 godzin

- **Wygaśnięcie za 30 dni**: subskrypcje wygaśnie w ciągu następnych 30 dni

- Zmiany **(ostatnie 30 dni)**: subskrypcje, które zostały cofnięte lub zawieszone (wyłączone) w ciągu ostatnich 30 dni

- **Dystrybucja według typów subskrypcji**:% dystrybucji łącznej liczby subskrypcji według typu subskrypcji opartej na licencji i użycia

- **Liczba aktywnych subskrypcji według produktu**: produkty sprzedane według liczby aktywnych subskrypcji

- **Subskrypcje w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych subskrypcji i subskrypcji zmian zagregowanych miesięcznie w okresie ostatnich 12 miesięcy

- **Szczegóły subskrypcji klienta**: szczegółowy widok klientów, subskrypcji i ofert

### <a name="license-insights-report"></a>Raport dotyczący informacji o licencji:

- **Łączna liczba licencji**: łączną liczbę licencji agregowanych w ramach wszystkich subskrypcji opartych na licencji

- **Nowe (ostatnie 30 dni)**: Dodanie licencji w ciągu ostatnich 30 dni

- Zmiany **(ostatnie 30 dni)**: redukcja licencji w ciągu ostatnich 30 dni

- **Nowość (ostatnie 24 godziny)**: Dodanie licencji w ciągu ostatnich 24 godzin

- **Licencje w ciągu ostatnich 90 dni**: trend w miesiącu, w którym liczba dodatkowych licencji i obniżki są agregowane miesięcznie w okresie ostatnich 90 dni

- **Liczba aktywnych licencji według produktu**: produkty sprzedawane posortowane według liczby aktywnych licencji

- **Liczba aktywnych licencji według klientów**: posortowane według liczby aktywnych licencji

- **Szczegóły zdarzenia licencji klienta w ciągu ostatnich 90 dni**: szczegółowy widok klientów, subskrypcji i zdarzeń subskrypcji, w tym data, nazwa zdarzenia, ilość i zmiana ilości.

### <a name="licenses-usage-report"></a>Raport użycia licencji:

- **Licencje przypisane przez produkt**: produkty sprzedane według liczby przypisań licencji

- **Licencje używane przez produkt**: produkty sprzedawane posortowane według liczby użycia licencji

- **Dystrybucja przez klienta przypisanych licencji**:% dystrybucji łącznej liczby klientów w przedziałach 20% zakresu przez przypisanie licencji%

- **Dystrybucja przez klienta licencji w użyciu**:% dystrybucji łącznej liczby klientów w przedziale 20% zakresu według użycia licencji%

- **Licencje przypisane przez klienta**: szczegółowy widok licencji sprzedanych i licencji przypisanych przez klientów i produkty

- **Licencje używane przez klienta**: szczegółowy widok sprzedanych licencji i licencji używanych przez klientów i produkty

### <a name="azure-insights-report"></a>Raport usługi Azure Insights:

- Klienci korzystający z **użycia w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych klientów opartych na użyciu i przetworzonych klientów korzystających z użycia zagregowanych miesięcznie w okresie ostatnich 12 miesięcy

- **Subskrypcje oparte na użyciu w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych subskrypcji opartych na użyciu i przetworzonych subskrypcji opartych na użyciu zagregowanych miesięcznie w okresie ostatnich 12 miesięcy

- **Szacowany koszt użycia przez klienta w ciągu ostatnich 60 dni**: Klienci korzystający z użycia posortowani według szacowanej kwoty dolara za faktury przed opodatkowaniem w okresie ostatnich 60 dni. Ten stan oznacza, że klienci korzystający z większości klientów korzystający z większości przychodów

- **Szacowany koszt użycia według kategorii w ciągu ostatnich 60 dni**: kategorie mierników subskrypcji opartych na użyciu sortowane według szacowanej kwoty dolara za faktury przed opodatkowaniem w okresie ostatnich 60 dni.

- **Szacowany koszt użycia według subskrypcji w ciągu ostatnich 60 dni**: subskrypcje oparte na użyciu przez szacowaną kwotę dolara za faktury przed opodatkowaniem zagregowaną w okresie ostatnich 60 dni.

- **Szacowany koszt użycia przez klienta według budżetu wydatków**: klienci posortowani według procentu bieżącego budżetu wydatków użycia przekraczają próg (100%).

### <a name="azure-resource-usage-report"></a>Raport użycia zasobów platformy Azure:

- **Użycie zasobów platformy Azure według dnia w wybranym okresie**: dzienne jednostki zużycia dla każdego zmierzonego zasobu w każdej subskrypcji opartej na użyciu dla wybranego okresu w ciągu ostatnich 60 dni.

- **Szacowany koszt użycia zasobów platformy Azure dla wybranego okresu**: szacowany koszt oparty na najnowszej stawce dla każdego zmierzonego zasobu w ramach każdej subskrypcji opartej na użyciu dla wybranego okresu w ciągu ostatnich 60 dni. 

## <a name="next-steps"></a>Następne kroki

- [Omówienie usługi Partner Center Analytics dla Power BI aplikacji](power-bi-app-for-direct-partners.md)

- [Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
