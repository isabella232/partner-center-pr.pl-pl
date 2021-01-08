---
title: Odkryj oferty — komercyjne witryny Marketplace
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób partnerzy usług kryptograficznych mogą korzystać z Centrum partnerskiego, aby wyświetlać lub przeszukiwać oferty SaaS w portalu Marketplace lub z cennika niezależnych dostawców oprogramowania (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f741ef4e44632e1d239285b58e99fbb38a8f37e7
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979604"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Odkryj oferty i ceny w komercyjnym portalu partnerskim

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny

Gdy niezależni dostawcy oprogramowania (ISV) zdecydują się na opublikowanie oferty w portalu komercyjnym, mogą także zdecydować, czy chcą udostępnić ofertę w programie CSP. Jeśli wybierzesz sprzedawanie oferty za pomocą programu CSP, partnerzy CSP powinni zobaczyć ofertę w obszarze witryny Marketplace Centrum partnerskiego.

Jeśli oferta niezależnego dostawcy oprogramowania nie jest wyświetlana zgodnie z oczekiwaniami w centrum partnerskim, może to być spowodowane tym, że:

- Dostawca oprogramowania nie zdecydował się sprzedawać oferty za pomocą programu CSP. Na przykład niektóre produkty niezależnego dostawcy oprogramowania mogły zostać udostępnione w innych obszarach portalu komercyjnego (na przykład w [Microsoft AppSource](https://appsource.microsoft.com/) i w [witrynie Azure Marketplace](https://azuremarketplace.microsoft.com/)), ale mogą nie być wyświetlane dla partnerów w programie CSP w witrynie Marketplace Centrum partnerskiego.

- Niezależny dostawca oprogramowania zdecydował się udzielić oferty wyłącznie wyłącznie wybranej liczbie partnerów CSP. Aby uzyskać więcej informacji na temat ofert z wyłączeniem, zobacz w dalszej części tego tematu pomocy.

- Typ oferty nie może być transakcyjny za pośrednictwem Centrum partnerskiego lub Azure Portal (np. kontenerów lub niektórych ofert opartych na użyciu).

- Dla tej oferty niezależnego dostawcy oprogramowania mogą nie być obsługiwane kraje rozliczeniowe skojarzonych klientów.

## <a name="view-marketplace-offers-in-partner-center"></a>Wyświetl oferty z witryny Marketplace w centrum partnerskim

Aby wyświetlić dostępne komercyjne oferty rynkowe w programie CSP:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego, a następnie wybierz pozycję **CSP** w menu nawigacji po lewej stronie.

2. Wybierz opcję **Sprzedaj**, a następnie pozycję **Marketplace**. Domyślnie zobaczysz produkty wszystkich typów i kategorii.

3. Wybierz filtr według typu lub kategorii. Możesz również użyć **wyszukiwania** , aby znaleźć określone słowa kluczowe, nazwy ofert lub nazwy wydawców niezależnych dostawców oprogramowania.

4. Wybierz ofertę określonego produktu z listy. Spowoduje to przejście do karty przegląd produktu, w której można dowiedzieć się więcej o ofercie. Na tej karcie mogą znajdować się następujące informacje: 

    - Opis produktu lub oferty

    - Więcej informacji na temat wydawcy niezależnego dostawcy oprogramowania

    - Linki do dokumentacji lub materiałów marketingowych przekazanych przez wydawcę niezależnego dostawcy oprogramowania

    - Inne możliwe kontakty niezależnego dostawcy oprogramowania do obsługi klienta, inżynierów lub kontaktu dla programu CSP

5. Aby uzyskać więcej informacji na temat dostępnych planów, jednostek SKU lub cennika oferty, wybierz kartę **plany i Cennik** . Na tej karcie zostanie wyświetlona wartość:

    - Rynki, w których ta oferta jest dostępna

    - Lista jednostek SKU lub planów dostępnych dla oferty

    - Cennik dla każdej jednostki SKU lub planu

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Wyświetlanie ofert portalu Marketplace za pośrednictwem interfejsów API Centrum partnerskiego

Partnerzy programu CSP mogą również używać interfejsów API do zwracania listy kwalifikujących się ofert. Kwalifikujące się oferty będą dostępne tylko dla tych SaaS niezależnych dostawców oprogramowania, które mogą sprzedawać dla partnerów za pośrednictwem witryny Marketplace Centrum partnerskiego. W przypadku partnerów korzystających z interfejsów API do identyfikowania ofert w katalogu zapoznaj się ze wskazówkami, aby [uzyskać listę ofert dla rynku](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Wyświetlanie najnowszych cen oferty portalu Marketplace w centrum partnerskim

Wykonaj następujące kroki, aby uzyskać najnowsze szczegóły cennika związane z ofertą:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego, a następnie wybierz pozycję **CSP** w menu nawigacji po lewej stronie.

2. Wybierz opcję **sprzedaż**, a następnie pozycję **Cennik i oferty**.

3. Przewiń w dół do sekcji **Marketplace** , wybierz lokalizację i Pobierz **Cennik portalu Marketplace**. Spowoduje to wygenerowanie arkusza kalkulacyjnego z najnowszymi danymi cen dla SaaS, ofert opartych na licencji i ofert taryfowych dostępnych od wydawców niezależnych dostawców oprogramowania. Niektóre ceny aplikacji platformy Azure mogą być również wyświetlane w tym miejscu. Te informacje są aktualizowane codziennie, więc można je sprawdzać pod kątem bieżących cen tak często, jak to możliwe.

4. Jeśli produkt niezależnego dostawcy oprogramowania zawiera bezpłatny okres próbny, w arkuszu kalkulacyjnym zostanie wyświetlonych dwa wiersze dla tego produktu:

    - Jeden wiersz przedstawia cenę bezpłatnej wersji próbnej równą zero. Oznacza to, że dostępny jest bezpłatny okres próbny.

    - W drugim wierszu jest wyświetlana cena i warunki, które będą stosowane po przekroczeniu okresu bezpłatnej wersji próbnej.

Jako partner programu CSP można kwalifikować się do innych bodźców związanych z konkretnymi ofertami komercyjnych rynków rynkowych. Aby uzyskać więcej informacji na temat innych bodźców, zobacz [Przewodnik dotyczący zachęty dla dostawcy CSP](https://aka.ms/partnerincentives) (wymagane jest logowanie do dostawcy CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Dowiedz się więcej o ofertach dostępnych w portalu Marketplace

Dostawcy ISV mają możliwość udostępnienia ofert tylko określonym partnerom w programie CSP. Jest to tzw. Oferta wyłączna. Wszyscy partnerzy w programie CSP nadal mogą wyświetlać wszystkie oferty niezależnego dostawcy oprogramowania w witrynie komercyjne Centrum partnerskiego, w tym oferty oznaczone jako wyłączne.

Jeśli oferta **nie** zostanie oznaczona jako wyłączna, wszyscy partnerzy mogą zakupić tę ofertę (przy założeniu, że kraj rozliczeniowy wybranego klienta odpowiada dostępności oferty niezależnego dostawcy oprogramowania).

Jednak w przypadku każdej oferty oznaczonej jako wyłączny tylko partnerzy wybierani przez niezależnego dostawcę oprogramowania będą mogli zakupić tę ofertę.

> [!NOTE]
> Jeśli zobaczysz ofertę oznaczoną jako wyłączną, którą chcesz sprzedać klientom, skontaktuj się bezpośrednio z własnym dostawcą oprogramowania i podawaj uprawnienia do sprzedaży oferty wyłącznej. Po wyświetleniu szczegółów oferty wyłącznej może zostać wyświetlony link **skontaktuj się z dostawcą ISV** , który można wybrać.

Aby dowiedzieć się więcej na temat środowiska niezależnego dostawcy oprogramowania, zobacz temat [dostawcy rozwiązań w chmurze](/azure/marketplace/cloud-solution-providers).

Aby uzyskać więcej informacji na temat środowiska CSP w portalu Marketplace, przeczytaj artykuł [komercyjne Omówienie witryny Marketplace](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Następne kroki

- [Kup komercyjne oferty rynkowe](csp-commercial-marketplace-purchase.md)