---
title: Używanie Partner Center Analytics dla Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak wyświetlać dane biznesowe przy użyciu aplikacja statystyczna Centrum partnerskiego dla usługi Power BI (dla bezpośrednich partnerów w programie Dostawca rozwiązań w chmurze (CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dd50b12bdffd9594367e699e9ee044306a226736f669366e2fae9ac94c338da2
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681403"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Wyświetlanie danych biznesowych za pomocą aplikacji Partner Center Analytics dla firmy Microsoft Power BI



**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent sprzedaży | Agent administracyjny

## <a name="view-your-business-data"></a>Wyświetlanie danych biznesowych

Pobierz wizualną reprezentację danych biznesowych za pomocą aplikacji Partner Center Analytics dla usługi Microsoft Power BI, w tym:

- Rozwój bazy klientów, subskrypcji i licencji

- Użycie produktów Office 365, Microsoft Dynamics i Microsoft Azure produktów

- Jednostki dziennego zużycia dla każdego zasobu taryfowego w każdej subskrypcji platformy Azure w ciągu ostatnich 60 dni

- Szacowany koszt (na podstawie najnowszej karty stawki)

- Możliwość eksportowania zestawów danych i tworzenia raportów niestandardowych, w tym dla niestandardowych klientów.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Informacje o wersji zapoznawczej Partner Center Analytics

- Ta aplikacja jest tylko dla bezpośrednich partnerów Dostawca rozwiązań w chmurze (CSP). Inni partnerzy w programie CSP (na przykład odsprzedawcy pośredni) nie będą mogli się zalogować.

- Wszelkie szacowane koszty są danymi rozliczeń przed opodatkowaniem/fakturami i nie są prawnie związane. Szacowane koszty są przeznaczone tylko do wglądu w dane.

- Informacje o kliencie są oparte na subskrypcjach. Klienci, dla których niedawno utworzono konta, ale nie mają jeszcze subskrypcji, nie są uwzględniani w liczbach.

- Szacowany koszt jest oparty na najnowszej karcie stawki, która jest oparta na cenach CSP.

- Dni to dni kalendarzowe.

### <a name="business-insights-report"></a>Raport Szczegółowe informacje biznesowego

- **Dzierżawy klientów:** liczba różnych dzierżaw Azure Active Directory (Azure AD) klientów, którzy kupili subskrypcje

- **Nowość (ostatnie 30 dni):** nowi klienci kupują co najmniej jedną subskrypcję w ciągu ostatnich 30 dni

- **Rezygnacja (ostatnie 30 dni):** klienci bez żadnych subskrypcji "aktywnych", "w ramach prolongaty" lub "wyłączonych"

- **Nowość (ostatnie 24 godziny):** nowi klienci kupują co najmniej jedną subskrypcję w ciągu ostatnich 24 godzin

- **Szacowany miesięczny koszt w** ciągu ostatnich 12 miesięcy: trend miesiąc do miesiąca szacowanej kwoty faktury przed opodatkowaniem zagregowanej co miesiąc w okresie ostatnich 12 miesięcy

- **Szacowany koszt według produktu** w ciągu ostatnich 12 miesięcy: sprzedane produkty posortowane według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w okresie ostatnich 12 miesięcy. Ten stan wskazuje najlepsze produkty, które przynoszą najwięcej przychodów.

- **Klienci w ciągu ostatnich 12 miesięcy:** Trend miesiąc do miesiąca nowych klientów i klientów z rezygnacjami zagregowany co miesiąc w okresie ostatnich 12 miesięcy

- **Szacowany koszt według klienta w** ciągu ostatnich 12 miesięcy: klienci posortowani według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w okresie ostatnich 12 miesięcy. Ten stan wskazuje najbardziej dochodowych klientów.

- **Liczba klientów według produktu:** sprzedane produkty posortowane według skojarzonych klientów. Ten stan wskazuje najlepsze produkty sprzedane większości klientów.

### <a name="subscription-insights-report"></a>Raport Szczegółowe informacje subskrypcji

- **Stan subskrypcji:**

- Aktywne: subskrypcje należące do stanu "aktywne" lub "w stanie prolongaty"

  - Wstrzymane: subskrypcje należące do stanu "wyłączone"

  - Coprowizowane: subskrypcje należące do stanu "coprowizowane" lub "wygasłe"

- **Stan wygaśnięcia:**

  - Wygasłe: subskrypcje, które już wygasły (gdzie data zakończenia subskrypcji jest w przeszłości)

  - Wygasanie po 30 dniach: subskrypcje, które wygasną po 30 dniach (gdzie data zakończenia subskrypcji to następne 30 dni)

  - Wygasanie w ciągu 30 dni: subskrypcje, które wygasną w ciągu następnych 30 dni (gdzie data zakończenia subskrypcji to od dnia dzisiejszego do następnych 30 dni)

- **Łączna liczba subskrypcji:** subskrypcje w stanie "aktywne", "w prolongacie" lub "wyłączone"

- **Nowe (ostatnie 30 dni):** nowe subskrypcje zakupione przez klientów w ciągu ostatnich 30 dni

- **Nowe (ostatnie 24 godziny):** nowe subskrypcje zakupione przez klientów w ciągu ostatnich 24 godzin

- **Wygasanie w ciągu 30 dni:** subskrypcje, które wygasną w ciągu następnych 30 dni

- **Rezygnacja (ostatnie 30 dni):** subskrypcje, które zostały coprowizowane lub wstrzymane (wyłączone) w ciągu ostatnich 30 dni

- **Dystrybucja według typów subskrypcji:** procent dystrybucji łącznej liczby subskrypcji według typu subskrypcji na podstawie licencji i na podstawie użycia

- **Liczba aktywnych subskrypcji według produktu:** sprzedane produkty posortowane według liczby aktywnych subskrypcji

- **Subskrypcje z ostatnich 12** miesięcy: trend z miesiąca na miesiąc nowych subskrypcji i subskrypcji rezygnacji zagregowanych co miesiąc w okresie ostatnich 12 miesięcy

- **Szczegóły subskrypcji klienta:** szczegółowy widok klientów, subskrypcji i ofert

### <a name="license-insights-report"></a>Raport Szczegółowe informacje licencji:

- **Łączna liczba licencji:** łączna liczba licencji zagregowana we wszystkich subskrypcjach opartych na licencjach

- **Nowe (ostatnie 30 dni):** dodawanie licencji w ciągu ostatnich 30 dni

- **Rezygnacja (ostatnie 30 dni):** redukcja licencji w ciągu ostatnich 30 dni

- **Nowe (ostatnie 24 godziny):** dodawanie licencji w ciągu ostatnich 24 godzin

- **Licencje z ostatnich 90 dni:** trend z miesiąca na miesiąc w przypadku dodatku licencji i redukcji zagregowanych miesięcznie w okresie ostatnich 90 dni

- **Liczba aktywnych licencji według produktu:** sprzedane produkty posortowane według liczby aktywnych licencji

- **Liczba aktywnych licencji według klienta:** klienci posortowani według liczby aktywnych licencji

- Szczegóły zdarzeń licencji klienta z ostatnich **90** dni: szczegółowy widok klientów, subskrypcji i zdarzeń subskrypcji, w tym daty zdarzenia, nazwy zdarzenia, ilości i zmiany ilości.

### <a name="licenses-usage-report"></a>Raport użycia licencji:

- **Licencje przypisane według produktu:** sprzedane produkty posortowane według liczby przypisań licencji

- **Licencje w użyciu według produktu:** sprzedane produkty posortowane według liczby użycia licencji

- **Rozkład przypisanych licencji** przez klientów: procent rozkładu całkowitej liczby klientów uszkodzonych w zasobnikach o zakresie 20% według przypisania licencji %

- **Rozkład klientów licencji w użyciu:** procent rozkładu całkowitej liczby klientów uszkodzonych w zasobnikach o zakresie 20% według procent użycia licencji

- **Licencje przypisane przez klienta:** szczegółowy widok sprzedanych licencji i licencji przypisanych przez klientów i produkty

- **Licencje w użyciu przez klienta:** szczegółowy widok licencji sprzedanych i licencji w użyciu przez klientów i produkty

### <a name="azure-insights-report"></a>Raport Szczegółowe informacje platformy Azure:

- Klienci na podstawie użycia w ciągu ostatnich **12** miesięcy: trend z miesiąca na miesiąc nowych klientów opartych na użyciu i klientów opartych na użyciu z rezygnacjami zagregowanych co miesiąc w okresie ostatnich 12 miesięcy

- **Subskrypcje oparte na** użyciu w ciągu ostatnich 12 miesięcy: trend z miesiąca na miesiąc nowych subskrypcji opartych na użyciu i subskrypcje oparte na użyciu, które są agregowane co miesiąc w okresie ostatnich 12 miesięcy

- Szacowany koszt użycia według klienta w ciągu ostatnich **60** dni: klienci na podstawie użycia posortowani według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w ciągu ostatnich 60 dni. Ten stan wskazuje najbardziej dochodowych klientów opartych na użyciu

- Szacowany koszt użycia według kategorii w ciągu ostatnich **60** dni: kategorie mierników subskrypcji opartych na użyciu posortowane według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w okresie ostatnich 60 dni.

- **Szacowany koszt użycia** według subskrypcji w ciągu ostatnich 60 dni: subskrypcje oparte na użyciu według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w ciągu ostatnich 60 dni.

- **Szacowany koszt użycia przez klienta według budżetu wydatków:** Klienci posortowani według wartości procentowej bieżącego budżetu wydatków na użycie przekraczających próg (100%).

### <a name="azure-resource-usage-report"></a>Raport Użycia zasobów platformy Azure:

- **Użycie zasobów platformy Azure według dnia dla** wybranego okresu: dzienne jednostki zużycia dla każdego mierzonego zasobu w każdej subskrypcji opartej na użyciu w wybranym okresie w ciągu ostatnich 60 dni.

- **Szacowany koszt** użycia zasobów platformy Azure w wybranym okresie: Szacowany koszt oparty na najnowszej karcie stawki dla każdego mierzonego zasobu w każdej subskrypcji opartej na użyciu w wybranym okresie w ciągu ostatnich 60 dni. 

## <a name="next-steps"></a>Następne kroki

- [Partner Center Analytics for Power BI app overview (Omówienie usługi Power BI Analytics dla aplikacji internetowych)](power-bi-app-for-direct-partners.md)

- [Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
