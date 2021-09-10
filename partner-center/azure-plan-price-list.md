---
title: Cennik planu platformy Azure dla partnerów CSP
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak partnerzy programu CSP mogą Partner Center, aby wyświetlić cennik subskrypcji w ramach planu platformy Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 73b47b62ce996156c7e780450bada1bdbec9f4b0
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957922"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Cennik dla nowego środowiska handlowego w programie CSP dla platformy Azure

**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży | Administrator zarządzania użytkownikami

Ceny w czasie rzeczywistym za nowe środowisko handlowe platformy Azure w programie CSP są dynamicznie dostarczane w czasie rzeczywistym na Partner Center. Ceny są wyświetlane tylko w USD. Od sierpnia 2021 r. wszyscy partnerzy będą rozliczani w walucie lokalizacji partnera, niezależnie od lokalizacji klienta, któremu sprzedano produkty. Aby uzyskać więcej informacji, zobacz [Plan platformy Azure — rozliczenia.](azure-plan-billing.md)

W ramach nowego rozwiązania handlowego dla platformy Azure w programie CSP wprowadziliśmy [nową ofertę platformy Azure](./azure-plan-lp.md). Ważne daty związane z poprzednią ofertą platformy Azure (MS-AZR-0145p) można znaleźć w [dokumencie oferty](https://go.microsoft.com/fwlink/p/?linkid=2164140).

W przypadku zarejestrowania *się przed* 21 lipca 2021 r.
- Poprzednia oferta platformy Azure będzie nadal wyświetlona w cenniku.

W przypadku zarejestrowania *się w dniu* 21 lipca 2021 r. lub później
- Poprzednia *oferta* platformy Azure nie zostanie wyświetlona w cenniku.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Zobacz cennik subskrypcji w obszarze cennika planu platformy Azure

1.  W menu Partner Center sprzedaży wybierz pozycję **Sell (Sprzedawaj),** **a następnie pozycję Pricing and offers (Ceny i oferty).**
2.  W **obszarze Cennik użycia planu platformy** Azure i Cennik **rezerwacji** planu platformy Azure wybierz kraj, a następnie link pobierania.
   - W **obszarze Kursy wymiany obcej** wybierz link pobierania w sekcji .

   > [!NOTE] 
   > **Stawki fx nie** są specyficzne dla kraju.

   :::image type="content" source="images/azure/pricing-new.png" alt-text="Zrzut ekranu przedstawiający cennik i oferty pokazujące nowe środowisko handlowe.":::

   > [!NOTE] 
   > Możesz wyeksportować dwa różne cenniki: cennik planu platformy Azure i cennik innych firm w witrynie Marketplace.

## <a name="azure-price-list-specifics"></a>Szczegółowe informacje o cenniku platformy Azure

- Cennik planu platformy Azure będzie dostępny na stronie **Cennik i oferty** w Partner Center w obszarze **Sprzedaż**.

- Eksporty będą dostępne dla usług użycia planu platformy Azure, rezerwacji platformy Azure i stawek FX.

- Opcje eksportu obejmują:

  - **Bieżące ceny:** ta opcja obejmuje wszystkie mierniki i ceny od pierwszego miesiąca do bieżącej daty miesiąca, takie jak nowe ceny, zmienione ceny lub usunięte ceny. Wszystkie ceny będą mieć efektywne daty rozpoczęcia i zakończenia, aby wyjaśnić, czy są nowe, czy usunięte.

  - **Cennik z poprzedniego miesiąca:** pliki do pobrania dla każdego typu zasobu będą według miesięcy. W przypadku plików cen będzie to obejmować wszystkie mierniki, które były dostępne w tym miesiącu. Jeśli nowy miernik pojawił się w połowie miesiąca, pojawi się jako miernik z datą wejścia w życie odzwierciedlającą jego dostępność. Podobnie jak w przypadku cen, które zostały wycofane, pokazując efektywną datę zakończenia opisową, kiedy nie są już dostępne.

  - **Stawki FX:** stawki fx będą dostępne do pobrania dzień przed 1. dniem miesiąca, 18:00 czasu PST. Jeśli na przykład chcesz uzyskać stawki za listopad, pobierz stawki z 31 października. W poprzednim miesiącu będą również dostępne stawki FX.

- Ceny w cennikach są cenami bezpośrednimi. Niektórzy partnerzy mogą kwalifikować się do środków uzyskane przez partnerów. Aby uzyskać informacje na temat sposobu obliczania środków uzyskane przez partnera, przeczytaj Jak są obliczane i opłacane punkty uzyskane przez [partnera.](partner-earned-credit-explanation.md)

- **Kwalifikujące się usługi:** Punkty uzyskane przez partnerów mają zastosowanie do usług wymienionych w cenniku użycia planu platformy **Azure,** które partnerzy mogą eksportować ze strony [cennika planu platformy Azure.](https://partner.microsoft.com/commerce/sales)
   > [!NOTE]
   > Istnieją wyjątki, w tym między innymi produkty innych firm zidentyfikowane jako  "Inne firmy" w kolumnie Tagi cennika użycia planu platformy Azure i rezerwacje planów platformy Azure.

## <a name="price-list-data"></a>Dane cennika

|**Pole**   |**Opis**   |
|--------------------------|:---------------------------|
|Tytuł produktu  |Tytuł lub nazwa produktu|
|ProductID   |Identyfikator produktu|
|SKuId|Identyfikator SKU|
|SkuTitle|Tytuł lub nazwa SKU|
|Publisher|Pierwszą firmą zawsze będzie firma Microsoft|
|SkuDescription|Opis sku|
|UnitOfMeasure|Jednostki, które będą naliczane lub rozliczane|
|TermDuration|W przypadku produktów opartych na terminach— długość okresu, która ma zastosowanie do rezerwacji|
|Rynku|Rynek cen|
|Waluta|Waluta cennika|
|UnitPrice|Cena za jednostkę|
|PricingTierRangeMin|W przypadku cen warstwowych obowiązuje cena minimalna|
|PricingTierRangeMax|W przypadku cen warstwowych obowiązuje maksymalna cena|
|EffectiveStartDate|Data rozpoczęcia cennika|
|EffectiveEndDate|Data zakończenia cennika|
|MeterIds|Identyfikator miernika dla sku produktu|
|Typ miernika|Typ miernika|
|Tagi|Właściwości elementu w przypadku cen planu platformy Azure to platforma Azure lub platforma Azure i rezerwacje (w szczególności w przypadku rezerwacji)|

Cenniki planu platformy Azure można wyeksportować ze strony [Cennik i oferty w](https://partner.microsoft.com/dashboard/sell/pricingandoffers) Partner Center.

## <a name="tiered-pricing"></a>Ceny warstwowe

Niektóre usługi użycia planu platformy Azure obsługują ceny warstwowe. Partnerzy mogą znaleźć te produkty i jednostki SKU w cenniku planu platformy Azure. Elementy, które mają wartości w kolumnach zakresu warstw cenowych, umożliwiają partnerom zrozumienie ceny na podstawie użycia. W poniższym przykładzie korzystającym z przykładowych danych mamy jedną sku produktu z trzema warstwami cenowych.

|**Productid**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0,50|100001|9223372036854780000|
|DDD123456ABC|01AB|0,80|101|100000|
|DDD123456ABC|01AB|1|1|100|

W tym przykładzie, jeśli zostanie użytych 101 jednostek, opłata wynosi 100,80. Pierwsze 100 jednostek to po jednej, a następna jednostka jest naliczana na poziomie 0,80.

## <a name="pricing-api-for-azure-plan"></a>Interfejs API cennika dla planu platformy Azure

Interfejs API cennika umożliwia [programowe](/partner/develop/pricing) pobieranie cennika planu platformy Azure na potrzeby użycia i rezerwacji. Można również pobrać kursy wymiany walut obcych.

Interfejs API cennika znajduje się w innym punkcie końcowym niż inne Partner Center API. Informacje o cenach obejmują ceny miernika w USD dla zasobów planu platformy Azure i cen rezerwacji stosowanych do subskrypcji planu platformy Azure.

Ten interfejs API umożliwia również partnerom pobieranie miesięcznych kursów wymiany, ponieważ ceny planu platformy Azure są dostępne tylko w USD. Za pomocą interfejsów API można pobrać zarówno ceny, jak i kursy wymiany walut z bieżącego miesiąca lub poprzednich miesięcy.

> [!NOTE]
> Interfejs API cennika jest specyficzny dla cennika planu platformy Azure. Nadal należy używać istniejącego interfejsu API usługi RateCard i list cen opublikowanych na stronie "Ceny i oferty" usługi Partner Center dla zasobów platformy Azure lub rezerwacji wdrożonych w subskrypcjach planu spoza platformy Azure. Interfejs API cennika planu platformy Azure nie obsługuje oprogramowania, platformy handlowej ani cen opartych na licencjach, takich jak Microsoft 365 lub Dynamics 365.

Aby uzyskać więcej informacji na temat cennika planu platformy Azure i interfejsów API kursów wymiany walut, zobacz pełną dokumentację [interfejsu API cennika.](/partner/develop/pricing)

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
