---
title: Odnajdywanie ofert — komercyjna platforma handlowa
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak partnerzy programu CSP mogą używać usługi Partner Center do wyświetlania lub wyszukiwania na platformie handlowej ofert SaaS lub cen od niezależnych dostawców oprogramowania.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bd1f9d0a881021fc97bbf94eb190acb6e6e69f14
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246898"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Odnajdywanie ofert i cen na platformie Partner Center platformie handlowej

**Odpowiednie role:** Administrator globalny | Agent administracyjny

Gdy niezależni dostawcy oprogramowania zdecydują się opublikować ofertę na platformie handlowej, mogą również zdecydować, czy oferta ma być dostępna w programie CSP. Jeśli zdecyduje się sprzedawać ofertę za pośrednictwem programu CSP, partnerzy programu CSP powinni zobaczyć ofertę w Partner Center Marketplace.

Jeśli oferta isv nie jest wyświetlana zgodnie z oczekiwaniami w Partner Center, może to być spowodowane:

- IsV decided not to sell the offer through the CSP program. Na przykład niektóre produkty isv mogą zostać udostępnione w innych obszarach platformy handlowej (np. w usługach [Microsoft AppSource](https://appsource.microsoft.com/) i [Azure Marketplace),](https://azuremarketplace.microsoft.com/)ale mogą nie być widoczne dla partnerów w programie CSP na platformie Partner Center Marketplace.

- Isv decided to make the offer exclusive to only a select number of CSP partners. Aby uzyskać więcej informacji na temat ofert na wyłączność, zobacz w dalszej części tego tematu pomocy.

- Transakcje typu oferty mogą być Partner Center lub Azure Portal (np. kontenery lub niektóre oferty oparte na użyciu).

- Kraj rozliczeniowy skojarzonych klientów może nie być obsługiwany dla tej oferty isv.

## <a name="view-marketplace-offers-in-partner-center"></a>Wyświetlanie ofert w witrynie Marketplace w Partner Center

Aby wyświetlić dostępne oferty platformy handlowej w programie CSP:

1. Zaloguj się Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **CSP** z menu nawigacji po lewej stronie.

2. Wybierz **pozycję Sell (Sprzedawaj),** a następnie **pozycję Marketplace ( Marketplace).** Domyślnie będą dostępne produkty wszystkich typów i kategorii.

3. Wybierz filtr według typu lub kategorii. Możesz również użyć funkcji **wyszukiwania,** aby znaleźć określone słowa kluczowe, nazwy ofert lub nazwy wydawców ISV.

4. Wybierz z listy określoną ofertę produktu. Spowoduje to przejść do karty Przegląd produktu, na której można dowiedzieć się więcej o ofercie. Informacje na tej karcie mogą obejmować: 

    - Opis produktu lub oferty

    - Więcej informacji na temat wydawcy isv

    - Linki do dokumentacji lub materiałów marketingowych przekazanych przez wydawcę isV

    - Inne możliwe kontakty z isv w zakresie obsługi klienta, inżynierii lub kontaktu dla programu CSP

5. Aby wyświetlić więcej informacji o dostępnych planach, jednostkach SKU lub cenach oferty, wybierz **kartę Plany i** cennik. Na tej karcie są wyświetlane:

    - Rynki, na których ta oferta jest dla Ciebie dostępna

    - Lista dostępnych dla oferty jednostki SKU lub planów

    - Cennik każdej dostępnej wersji SKU lub planu

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Wyświetlanie ofert w witrynie Marketplace za pośrednictwem Partner Center API

Partnerzy programu CSP mogą również używać interfejsów API do zwracania listy kwalifikujących się ofert. Kwalifikujące się oferty będą dotyczyć tylko ofert dostawcy ISV SaaS dostępnych dla partnera do sprzedaży za pośrednictwem Partner Center marketplace. W przypadku partnerów używających interfejsów API do identyfikowania ofert w katalogu zapoznaj się ze wskazówkami, aby uzyskać listę ofert [dla rynku.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Zobacz najnowsze ceny ofert witryny Marketplace w witrynie Partner Center

Wykonaj następujące kroki, aby uzyskać najnowsze szczegóły cennika skojarzone z ofertą:

1. Zaloguj się Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **CSP** z menu nawigacji po lewej stronie.

2. Wybierz **pozycję Sell**(Sprzedawaj), a następnie pozycję Pricing and offers **(Ceny i oferty).**

3. Przewiń w dół do **sekcji Marketplace,** wybierz lokalizację i pobierz cennik **witryny Marketplace.** W ten sposób zostanie wygenerowany arkusz kalkulacyjny z najnowszymi danymi cennika usług SaaS, ofert opartych na licencjach i ofert mierzonych dostępnych od wydawców ISV. Niektóre cenniki aplikacji platformy Azure mogą być również wyświetlane tutaj. Te informacje są aktualizowane codziennie, więc możesz sprawdzać bieżące ceny tak często, jak wybierzesz.

4. Jeśli produkt isv zawiera bezpłatny okres próbny, arkusz kalkulacyjny wyświetli dwa wiersze dla tego produktu:

    - Jeden wiersz zawiera cenę bezpłatnej wersji próbnej o wartości zero. Oznacza to, że dostępny jest bezpłatny okres próbny.

    - W drugim wierszu przedstawiono cenę i warunki, które będą stosowane po zakończeniu bezpłatnego okresu próbnego.

Jako partner programu CSP możesz kwalifikować się do innych zachęt skojarzonych z określonymi ofertami platformy handlowej. Aby uzyskać więcej informacji na temat innych zachęt, zobacz przewodnik zachęt [CSP](https://aka.ms/partnerincentives) (wymaga logowania WSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Dowiedz się więcej o ofertach na wyłączność na platformie handlowej

IsVs have the option to make their offers available only to specific partners in the CSP program. Ta oferta jest znana jako oferta wyłączna. Wszyscy partnerzy w programie CSP mogą nadal wyświetlać wszystkie oferty isv na platformie handlowej Partner Center, w tym oferty oznaczone jako wyłącznie.

Jeśli oferta nie **jest** oznaczona jako Wyłączna, wszyscy partnerzy mogą ją zakupić (przy założeniu, że kraj rozliczeniowy wybranego klienta odpowiada dostępności oferty isV w kraju).

Jednak w przypadku każdej oferty oznaczonej jako Wyłączna tylko partnerzy wybrani przez isv będą mogli kupić tę ofertę.

> [!NOTE]
> Jeśli widzisz ofertę oznaczoną jako Wyłączna, która ma być sprzedawana klientom, sproś się bezpośrednio do isv i poproś o zgodę na sprzedaż oferty exclusive. Podczas wyświetlania szczegółów oferty na wyłączność może zostać wyświetlony link Skontaktuj się z **isv,** który możesz wybrać.

Aby dowiedzieć się więcej na temat obsługi usługodawców internetowych na platformie handlowej, przeczytaj [temat Cloud Solution Providers (Dostawcy rozwiązań w chmurze).](/azure/marketplace/cloud-solution-providers)

Aby uzyskać więcej informacji na temat obsługi CSP na platformie handlowej, przeczytaj [omówienie komercyjnej platformy handlowej.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Następne kroki

- [Kupowanie ofert komercyjnej platformy handlowej](csp-commercial-marketplace-purchase.md)