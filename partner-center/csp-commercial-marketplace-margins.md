---
title: Odnajdywanie marginesów — komercyjna platforma handlowa
ms.topic: how-to
ms.date: 10/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, Dostawca rozwiązań w chmurze (CSP) mogą używać usługi Partner Center do odnajdywania marginesów skonfigurowanych przez niezależnych dostawców oprogramowania.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8d7b5f077b3ea3f98f87121634427842db0a0f03
ms.sourcegitcommit: 77737d8f986a1afb3d923c130936e2f73ce07879
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/07/2021
ms.locfileid: "129661378"
---
# <a name="discover-margins-configured-by-independent-software-vendors-isvs"></a>Odnajdywanie marginesów skonfigurowanych przez niezależnych dostawców oprogramowania

**Odpowiednie role:** Administrator globalny | Administrator rozliczeń | Agent administracyjny | Agent sprzedaży | Agent pomocy technicznej

Niezależni dostawcy oprogramowania (ISV) mogą oferować rabaty marży dla niektórych ofert platformy handlowej określonym dostawcom rozwiązań w chmurze (CSP). Te marże zapraszają CSP do sprzedaży tych ofert swoim klientom.

> [!NOTE]
> Funkcja rabatów na marżę od isV  do CSP jest obecnie dostępna w publicznej wersji zapoznawczej, a my nadal zbieramy opinie i ulepszamy środowisko.

## <a name="notes-about-the-public-preview"></a>Uwagi dotyczące publicznej wersji zapoznawczej

Funkcja marginesów dla isv-CSP umożliwia isv tworzenie rabatów docelowych dla określonych CSP. Ta funkcja jest dostępna teraz, ale w publicznej wersji zapoznawczej. Oznacza to, że ta funkcja jest w pełni funkcjonalna i można jej używać, a my stale ulepszamy ogólne środowisko platformy handlowej CSP. Ta funkcja nie będzie już zadeklarowana w wersji zapoznawczej, ponieważ ulepszymy środowisko partnerskie. W tym przypadku nie ma konkretnych osi czasu, a partnerzy programu CSP mogą nadal korzystać z funkcji rabatów w takiej, w jaki są.

### <a name="public-preview-improvement-areas"></a>Obszary ulepszeń publicznej wersji zapoznawczej

- Dostępność oferty w usłudze AppSource: Integracja i dostępność niektórych ofert w witrynie Marketplace dla CSP, przede wszystkim ofert usługi AppSource, trwa dłużej i nie jest dostępna w Partner Center. Niektórzy partnerzy mogą szukać ofert w usłudze AppSource, ale być może będą musieli poczekać, aż zostaną udostępnione. W czasie zespół Partner Center będzie wprowadzać ulepszenia dotyczące opóźnienia między utworzeniem oferty przez isv isv a jej dostępem.
- Marże są obecnie definiowane jako rabaty procentowe dla określonej w witrynie Marketplace SKU produktu CSP. W przyszłości istnieją aspirujące do integracji punktu cenowego z przyszłymi cennikami. Dopóki tak się nie stanie, partnerzy będą w stanie sparować jednostkę SKU produktu na liście marż (i skojarzone interfejsy API) z jednostkami SKU produktów cennika witryny Marketplace, aby prognozować kwoty opłat.
- Niektóre oferty platformy handlowej z włączoną obsługą wersji próbnej, które nie są związane z rabatami na marżę, są wyświetlane jako kwoty w wysokości **00** USD w funkcji przeglądania witryny Marketplace. Partnerzy powinni uważać, aby zrozumieć, że te wersje próbne zostaną odnowione na płatne kwoty po zakończeniu okresu. 
- Oferty na wyłączność mogą być dostępne dla partnerów. Obecnie nie znajdują się one w cennikach platformy handlowej. Dopóki nie zostaną, partnerzy będą musieli znaleźć ich ceny za pomocą funkcji przeglądania witryny Marketplace dla produktu, dla którego chcą uzyskać cennik.

## <a name="view-margins-in-partner-center"></a>Wyświetlanie marginesów w Partner Center

Program CSP może wyświetlać marginesy skonfigurowane dla nich przez isvs na stronie marginesów:

> [!NOTE]
> Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych, zobacz [Getting around Partner Center (Poruszanie się po Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off)).

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Zaloguj się do pulpitu Partner Center [i](https://partner.microsoft.com/dashboard) wybierz **kafelek Cennik.**

2. Wybierz **pozycję Marginesy**. Partnerzy zobaczą listę ofert platformy handlowej, dla których isvs skonfigurowali marże.

3. Partnerzy CSP mogą przeglądać listę dostępnych marginesów lub **pobierać** dane w formacie rozdzielanym przecinkami.

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Zaloguj się do Partner Center [nawigacyjnego,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **CSP** z menu nawigacji po lewej stronie.

2. Wybierz **pozycję Sell (Sprzedawaj),** a następnie **pozycję Margins (Marże).** Partnerzy zobaczą listę ofert platformy handlowej, dla których isvs skonfigurowali marże.

3. Partnerzy CSP mogą przeglądać listę dostępnych marginesów lub **pobierać** dane w formacie rozdzielanym przecinkami.

* * *

## <a name="margins-overview"></a>Przegląd marginesów

IsVs that have established relationships with CSP Partners may want to offer margin discounts to incentivize the CSP Partner to sell the offers to their customers. W takich przypadkach partner CSP często negocjuje marżę z isv lub isv może zapewnić margines bez konsultacji z partnerem CSP. IsV may offer a margin on either license-based or consumption-based offers. Marże oparte na zużyciu mają zastosowanie tylko do produktów isv, a nie do żadnych produktów użycia platformy Azure, z których może współpracować ten produkt.

## <a name="margins-and-pricing"></a>Marże i ceny

Cennik Partner Center Marketplace zawiera oryginalne ceny CSP dla ofert. Cenniki platformy handlowej CSP są współdzielone przez wszystkich partnerów i zawierają cennik detaliczny. Następnie partnerzy stosują rabat procentowy marży dla sku produktu, który chcą kupić, aby poznać końcową cenę produktu przed jego zakupem. Partnerzy programu CSP będą również widzieć cennik detaliczny w arkuszu cen platformy Azure za pośrednictwem Azure Portal (tylko w przypadku produktów opartych na zużyciu). W tym arkuszu cen będą również widzieć szczegóły marży dla nich rozszerzonej. 

## <a name="purchasing-offers"></a>Oferty zakupu

Partnerzy programu CSP uzyskują skonfigurowany margines, po [](https://partner.microsoft.com) prostu kupując ofertę platformy handlowej w Partner Center lub wdrażając produkt z witryny Microsoft [Azure Portal.](https://portal.azure.com) Partner transakcji otrzyma rabat na marżę bez konieczności podjęcia kolejnego kroku. Partnerzy nie mogą zrezygnować z marży, jeśli isv skonfigurował ją dla partnera CSP, rabat zostanie zastosowany.

Marże mają zastosowanie do każdej transakcji wykonywanej przez partnera i mają zastosowanie do dowolnego z jego klientów. Partner programu CSP nie musi akceptować propozycji i nie jest wymagany do transakcji oferty isV, ale jeśli to zrobi i ma marżę, zostanie ona automatycznie zastosowana. 

## <a name="margins-and-indirect-resellers"></a>Marże i odsprzedawcy pośredni

Marże są dostępne tylko dla partnerów rozliczanych przez firmę Microsoft, partnerów transakcji, takich jak dostawcy pośredni i partnerzy rozliczający się bezpośrednio. Dostawca isv cannot provide a margin to an indirect reseller directly, but the indirect provider may decide to pass a margin through to their indirect reseller. Dostawcy pośredni mogą przekazać marżę do odsprzedawcy pośredniego, ale nie są oni zobowiązani do tego. 

## <a name="terms-and-billing"></a>Warunki i rozliczenia

Partnerzy mogą sprawdzić, czy marża została zastosowana dla ofert opartych na zużyciu przy użyciu funkcji zarządzania kosztami platformy Azure w Azure Portal. Partnerzy mogą sprawdzić, czy marża została zastosowana dla ofert opartych na licencjach, przeglądając plik uzgodnień na koniec cyklu rozliczeniowego.

Każdy margines ma datę rozpoczęcia i zakończenia. Redukcja ceny oparta na rabatie na marżę jest stosowana do okresu zakupu. Partner może ponownie kupić tę samą ofertę po okresie, aby uzyskać nowy okres z marżą. Odnowienia stosują margines, jeśli odnowienie ma miejsce w obrębie dat rozpoczęcia i zakończenia marginesu. Daty zakończenia dla marginesu zawsze są wyrównane do końca miesiąca. 

## <a name="margins-for-metered-billing"></a>Marginesy dla rozliczeń mierzonych

Niektóre produkty CSP są wyposażone w rozliczenia taryfowe. Jeśli partner CSP zwiększy stanowiska w przypadku ofert z rozliczeniami mierzonym, ceny dla części opłat opartej na uprawnieniach zachowają rabat do końca rocznego okresu subskrypcji, ale marża zastosowana do ceny rozliczenia taryfowego nie zostanie zachowana po upływie okresu końcowego marży. Obejście tego problemu jest dostępne dla isvs w celu utworzenia nowego marginesu dla tego partnera CSP do końca okresu subskrypcji. 

## <a name="margins-notifications"></a>Powiadomienia dotyczące marginesów

Nie ma proaktywnych powiadomień, chyba że isV kontaktuje się z programem CSP za pośrednictwem poczty e-mail i potwierdza, że rozszerzono margines. Partner CSP będzie mógł wyświetlać wszystkie dostępne marginesy za pośrednictwem karty Marginesy w Partner Center.   

### <a name="recon-files"></a>Ponowne pliki

Partner programu CSP znajdzie szczegóły rozszerzonych marż  w pliku cyklicznych i jednorazowych zakupów po wygenerowaniu. Ważne dane w pliku rekonescją w celu wyjaśnienia marginesów:

- Cena jednostkowa pozostanie zgodnie z ceną ustawioną przez isv.  

- Cena w cenie EffectiveUnitPrice będzie pokazywana po zastosowaniu marży.  

- Opis priceAdjustmentDescription będzie zawierać szczegółowe informacje o tym, jaka część marży została zapewniona partnerowi programu CSP. 

## <a name="discover-and-operationalize-margins-using-the-partner-center-apis"></a>Odnajdywanie i operationalize marginesów przy użyciu interfejsów PARTNER CENTER API

Partnerzy mogą używać interfejsu Partner Center interfejsu użytkownika lub interfejsów API do wyświetlania lub eksportowania dostępnych marginesów.

### <a name="apis-to-retrieve-margins"></a>Interfejsy API do pobierania marginesów

Partnerzy mogą zoperacyjnie przetwarzać dane, wywołując poniższe interfejsy API. Każdy z tych interfejsów API zwraca listę marginesów, do których partner ma dostęp, zdefiniowaną przez isv. Oba interfejsy API zwracają te same dane.

- [Funkcja Pobierz marginesy](/partner-center/develop/get-margins) zwraca dane w formacie wyników interfejsu API

- [Marginesy pobierania](/partner-center/develop/download-margins) zwraca dane w formacie rozdzielanym przecinkami

### <a name="apis-to-discover-marketplace-offers"></a>Interfejsy API do odnajdywania ofert na platformie handlowej

Partnerzy programu CSP mogą również używać interfejsów API do zwracania listy dostępnych marginesów. Kwalifikujące się oferty będą dotyczyć tylko ofert dostawcy isv SaaS dostępnych dla partnera do sprzedaży za pośrednictwem Partner Center marketplace. Partnerzy mogą uzyskać listę ofert SaaS w witrynie Marketplace, korzystając [z listy ofert dla rynku.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

Partnerzy programu CSP mogą używać interfejsów API Partner Center, aby ściągać listę transakcji ofert oprogramowania jako usługi (SaaS) i przesyłać zamówienia dla swoich klientów. Aby uzyskać więcej informacji, [zobacz Tworzenie subskrypcji dla produktów platformy handlowej](/partner-center/develop/create-subscription-azure-marketplace-products).

Partnerzy CSP mogą używać środowiska Azure Portal do wyświetlania wszystkich ofert na platformie handlowej. Za pomocą następujących interfejsów API mogą ściągać listę ofert maszyn wirtualnych z platformy handlowej i przesyłać zamówienia dla swoich klientów.  
- [Maszyny wirtualne: uzyskiwanie listy maszyn wirtualnych z interfejsami API](/azure/virtual-machines/windows/cli-ps-findimage)
- [Maszyny wirtualne: kupowanie interfejsów API (interfejs wiersza polecenia, program PowerShell, arm)](/azure/virtual-machines/linux/quick-create-cli) 

Nie ma żadnego filtru w Azure Portal ofert, które zostały sprzedane za pośrednictwem CSP. Partnerzy będą musieli przejrzeć cennik, aby zrozumieć, które oferty mogą być transakcje za pośrednictwem CSP. Obecnie nie ma żadnych Azure Portal API do transakcji ofert saaS lub aplikacji zarządzanych na platformie handlowej. 

Aby uzyskać więcej informacji na temat obsługi CSP na platformie handlowej, przeczytaj [omówienie komercyjnej platformy handlowej.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Następne kroki

- [Omówienie komercyjnej platformy handlowej](csp-commercial-marketplace-overview.md)
- [Kupowanie ofert komercyjnej platformy handlowej](csp-commercial-marketplace-purchase.md)
- [Przewodnik po zachętach dla programu CSP](https://aka.ms/partnerincentives)
