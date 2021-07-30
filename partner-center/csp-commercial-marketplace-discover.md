---
title: Odnajdywanie ofert — komercyjna platforma handlowa
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak partnerzy programu CSP mogą Partner Center do wyświetlania lub wyszukiwania na platformie handlowej ofert SaaS lub cen od niezależnych dostawców oprogramowania.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bd1f9d0a881021fc97bbf94eb190acb6e6e69f14
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837751"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Odnajdywanie ofert i cen na platformie Partner Center platformie handlowej

**Odpowiednie role:** Administrator globalny | Agent administracyjny

Gdy niezależni dostawcy oprogramowania (ISV) zdecydują się opublikować ofertę na platformie handlowej, mogą również zdecydować, czy mają być udostępniane w programie CSP. Jeśli zdecyduje się sprzedawać ofertę za pośrednictwem programu CSP, partnerzy programu CSP powinni zobaczyć tę ofertę w Partner Center Marketplace.

Jeśli oferta isV nie jest wyświetlana zgodnie z oczekiwaniami w Partner Center, może to być spowodowane:

- IsV decided not to sell the offer through the CSP program. Na przykład niektóre produkty isv mogą zostać udostępnione w innych obszarach platformy handlowej (np. w usługach [Microsoft AppSource](https://appsource.microsoft.com/) i [Azure Marketplace),](https://azuremarketplace.microsoft.com/)ale mogą nie być widoczne dla partnerów w programie CSP na platformie Partner Center Marketplace.

- IsV decided to make the offer exclusive to only a select number of CSP partners. Aby uzyskać więcej informacji na temat ofert na wyłączność, zobacz w dalszej części tego tematu pomocy.

- Nie można transakcjiować typu oferty za pośrednictwem Partner Center lub Azure Portal (np. kontenerów lub niektórych ofert opartych na użyciu).

- Kraj rozliczeniowy skojarzonych klientów może nie być obsługiwany dla tej oferty isv.

## <a name="view-marketplace-offers-in-partner-center"></a>Wyświetlanie ofert w witrynie Marketplace w Partner Center

Aby wyświetlić dostępne oferty platformy handlowej w programie CSP:

1. Zaloguj się Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **CSP** z menu nawigacji po lewej stronie.

2. Wybierz **pozycję Sell (Sprzedawaj),** a następnie **pozycję Marketplace ( Marketplace).** Domyślnie zobaczysz produkty wszystkich typów i kategorii.

3. Wybierz filtr według typu lub kategorii. Możesz również użyć funkcji **Wyszukiwania,** aby znaleźć określone słowa kluczowe, nazwy ofert lub nazwy wydawców ISV.

4. Wybierz z listy określoną ofertę produktu. Spowoduje to dostęp do karty Przegląd produktu, na której można dowiedzieć się więcej o ofercie. Informacje na tej karcie mogą obejmować: 

    - Opis produktu lub oferty

    - Więcej informacji na temat wydawcy isv publisher

    - Linki do dokumentacji lub materiałów marketingowych przekazanych przez wydawcę isV

    - Inne możliwe kontakty isv w zakresie pomocy technicznej, inżynierii lub kontaktu dla programu CSP

5. Aby wyświetlić więcej informacji o dostępnych planach, jednostkach SKU lub cenach oferty, wybierz **kartę Plany i** cennik. Na tej karcie są wyświetlane:

    - Rynki, na których ta oferta jest dostępna

    - Lista dostępnych dla oferty jednostki SKU lub planów

    - Cennik każdej dostępnej wersji SKU lub planu

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Wyświetlanie ofert w witrynie Marketplace za pośrednictwem Partner Center API

Partnerzy programu CSP mogą również zwracać listę kwalifikujących się ofert za pomocą interfejsów API. Kwalifikujące się oferty będą dotyczyć tylko ofert dostawcy oprogramowania SaaS dostępnych dla partnera do sprzedaży za pośrednictwem Partner Center marketplace. W przypadku partnerów korzystających z interfejsów API do identyfikowania ofert w katalogu zapoznaj się ze wskazówkami, aby uzyskać [listę ofert dla rynku.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Zobacz najnowsze ceny ofert w witrynie Marketplace w Partner Center

Wykonaj następujące kroki, aby uzyskać najnowsze szczegóły cennika skojarzone z ofertą:

1. Zaloguj się Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **CSP** z menu nawigacji po lewej stronie.

2. Wybierz **pozycję Sell**(Sprzedawaj), a następnie pozycję Pricing **(Ceny) i offers (oferty).**

3. Przewiń w dół do **sekcji Marketplace,** wybierz lokalizację i pobierz cennik **witryny Marketplace.** W ten sposób zostanie wygenerowany arkusz kalkulacyjny z najnowszymi danymi cen usługi SaaS, ofert opartych na licencjach i ofert mierzonych dostępnych od wydawców ISV. Niektóre cenniki aplikacji platformy Azure mogą również pojawić się tutaj. Te informacje są aktualizowane codziennie, dzięki czemu można sprawdzać bieżące ceny tak często, jak to możliwe.

4. Jeśli produkt isV obejmuje bezpłatny okres próbny, arkusz kalkulacyjny wyświetli dwa wiersze dla tego produktu:

    - Jeden wiersz zawiera cenę bezpłatnej wersji próbnej o wartości zero. Oznacza to, że dostępny jest bezpłatny okres próbny.

    - Drugi wiersz zawiera cenę i warunki, które będą stosowane po zakończeniu bezpłatnego okresu próbnego.

Jako partner programu CSP możesz kwalifikować się do innych zachęt skojarzonych z niektórymi ofertami platformy handlowej. Aby uzyskać więcej informacji na temat innych zachęt, zobacz przewodnik zachęt dla programu [CSP](https://aka.ms/partnerincentives) (wymaga logowania do programu CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Dowiedz się więcej o ofertach na wyłączność na platformie handlowej

IsVs have the option to make their offers available only to specific partners in the CSP program. Jest to nazywane ofertą wyłączną. Wszyscy partnerzy w programie CSP mogą nadal wyświetlać wszystkie oferty isv na platformie handlowej Partner Center, w tym oferty oznaczone jako wyłącznie.

Jeśli oferta nie **jest** oznaczona jako Wyłączna, wszyscy partnerzy mogą ją zakupić (przy założeniu, że kraj rozliczeniowy wybranego klienta jest powiązany z dostępnością oferty isV w danym kraju).

Jednak w przypadku każdej oferty oznaczonej jako Wyłączna tylko ci partnerzy wybrani przez isV będą mogli kupić tę ofertę.

> [!NOTE]
> Jeśli widzisz ofertę oznaczoną jako Wyłączna, która chcesz sprzedawać swoim klientom, s kontaktuj się bezpośrednio z isV i poproś o zgodę na sprzedaż oferty exclusive. Podczas wyświetlania szczegółów oferty na wyłączność może zostać wyświetlony link Skontaktuj się z **isv,** który możesz wybrać.

Aby dowiedzieć się więcej na temat obsługi usługodawców internetowych na platformie handlowej, przeczytaj [temat Cloud Solution Providers (Dostawcy rozwiązań w chmurze).](/azure/marketplace/cloud-solution-providers)

Aby uzyskać więcej informacji na temat obsługi CSP na platformie handlowej, przeczytaj [omówienie komercyjnej platformy handlowej.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Następne kroki

- [Kupowanie ofert komercyjnej platformy handlowej](csp-commercial-marketplace-purchase.md)