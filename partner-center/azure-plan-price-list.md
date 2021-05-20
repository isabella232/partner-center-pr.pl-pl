---
title: Cennik planu platformy Azure dla partnerów programu CSP
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak partnerzy programu CSP mogą Partner Center, aby wyświetlić cennik subskrypcji w ramach planu platformy Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 6d8e73e664d400e8e6d80e529326e566c5fd88a8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149574"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Cennik dla nowego środowiska handlowego w programie CSP dla platformy Azure

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży | Administrator zarządzania użytkownikami

Cennik nowego doświadczenia handlowego platformy Azure w programie CSP jest publikowany w Partner Center. Cennik jest dynamicznie dostarczany w pliku dokładnym w czasie rzeczywistym, a ceny są wyświetlane tylko w USD. Od 28 stycznia 2021 r. partnerzy w regionie Unii Europejskiej/EFTA i Zjednoczonego Królestwa, którzy mają nowych klientów i istniejących klientów programu CSP, którzy kupują nowe oferty handlowe po raz pierwszy, których dzierżawy zostały utworzone przed 11 maja 2020 r., będą rozliczani za te zakupy w walucie lokalizacji partnera.  Partnerzy znajdujący się poza regionem UNII EUROPEJSKIEJ/EFTA i Zjednoczonego Królestwa będą nadal rozliczani w walucie lokalizacji partnera. Przeczytaj plan [platformy Azure — rozliczenia](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Zobacz cennik subskrypcji w obszarze cennika planu platformy Azure

1. W menu Partner Center po lewej stronie wybierz pozycję **Sprzedawaj,** a następnie wybierz pozycję **Marketplace.**

2. W obszarze Cennik planu platformy Azure wybierz kraj, dla którego chcesz uzyskać cennik.

3. Obok opcji **Typ eksportu wybierz** pozycję Cennik użycia planu platformy **Azure,** **ceny rezerwacji planu platformy Azure** lub stawki **FX.** 

>[!NOTE] 
>**Stawki FX nie** są specyficzne dla danego kraju.

4. Obok opcji **Ceny dla daty** wybierz datę, na przykład **Bieżąca**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="specyficzne dla kraju":::

>[!NOTE] 
>Możesz wyeksportować dwa różne cenniki — cennik planu platformy Azure i cennik innej firmy w witrynie Marketplace.

## <a name="azure-price-list-specifics"></a>Szczegółowe informacje o cenniku platformy Azure

- Cennik planu platformy Azure będzie dostępny na stronie witryny Marketplace w Partner Center w obszarze **Sprzedaż**.

- Eksporty będą dostępne dla usług użycia planu platformy Azure, rezerwacji platformy Azure i stawek FX.

- Opcje eksportu obejmują:

  - **Dzisiejsze ceny:** obejmuje wszystkie mierniki i ceny od 1. dnia miesiąca do bieżącej daty bieżącego miesiąca. Obejmuje to nowe ceny, zmienione ceny lub usunięte ceny. Wszystkie ceny będą mieć efektywne daty rozpoczęcia i zakończenia, aby wyjaśnić, czy są nowe, czy usunięte.

  - **Cennik z poprzedniego miesiąca:** pobieranie poszczególnych typów zasobów będzie według miesiąca. W przypadku plików cen będzie to obejmować wszystkie mierniki, które były dostępne w tym miesiącu. Jeśli w połowie miesiąca pojawi się nowy miernik, pojawi się jako miernik z datą wejścia w życie odzwierciedlającą jego dostępność. Podobnie jak w przypadku cen, które nie są już dostępne, wyświetlane ze efektywną datą zakończenia opisową, kiedy nie są już dostępne.

  - **Stawki FX:** stawki FX będą dostępne do pobrania dzień przed 1. dniem miesiąca, 18:00 PST. Jeśli na przykład chcesz uzyskać stawki za listopad, pobierz stawki z 31 października. W poprzednim miesiącu będą również dostępne stawki FX.

- Ceny w cennikach są cenami bezpośrednimi. Niektórzy partnerzy mogą kwalifikować się do środków uzyskane przez partnerów. Aby uzyskać informacje na temat sposobu obliczania środków zdobytych przez partnera, zobacz Jak są obliczane i opłacane uzyskane przez partnera [punkty.](partner-earned-credit-explanation.md)

- **Kwalifikujące się usługi:** Środków uzyskane przez partnerów dotyczy usług wymienionych w cenniku użycia planu platformy **Azure,** które partnerzy mogą eksportować ze strony [cennika planu platformy Azure.](https://partner.microsoft.com/commerce/sales) Należy pamiętać, że istnieją wyjątki, w tym między innymi produkty innych firm zidentyfikowane jako "inne firmy" w kolumnie Tagi cennika użycia planu platformy Azure i rezerwacji planu platformy Azure.

## <a name="price-list-data"></a>Dane cennika

|**Pole**   |**Opis**   |
|--------------------------|:---------------------------|
|ProductTitle  |Tytuł lub nazwa produktu|
|ProductID   |Identyfikator produktu|
|SKuId|Identyfikator SKU|
|SkuTitle|Tytuł lub nazwa SKU|
|Publisher|Firma 1 zawsze będzie firmą Microsoft|
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
|MeterType (Typ miernika)|Typ miernika|
|Tagi|Właściwości elementu w przypadku cennika planu platformy Azure będą dotyczyć platformy Azure lub platformy Azure i rezerwacji (w szczególności rezerwacji)|

Cenniki planu platformy Azure można wyeksportować ze strony [Cennik i oferty w](https://partner.microsoft.com/dashboard/sell/pricingandoffers) Partner Center.

## <a name="tiered-pricing"></a>Ceny warstwowe

Niektóre usługi użycia planu platformy Azure obsługują ceny warstwowe. Partnerzy mogą znaleźć te produkty i jednostki SKU w cenniku planu platformy Azure. Elementy, które mają wartości w kolumnach zakresu warstw cenowych, umożliwiają partnerom zrozumienie ceny na podstawie użycia. W poniższym przykładzie korzystającym z przykładowych danych mamy jedną sku produktu z trzema warstwami cenowym.

|**Productid**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

W tym przykładzie, jeśli używane jest 101 jednostek, opłata wynosi 100,80. Pierwsze 100 jednostek jest po jednej, a opłata za następną jednostkę jest naliczana na poziomie 0,80.

## <a name="pricing-api-for-azure-plan"></a>Interfejs API cennika dla planu platformy Azure

Interfejs API [cennika](/partner/develop/pricing) umożliwia programowe pobieranie cennika planu platformy Azure na potrzeby użycia i rezerwacji. Możesz również pobrać kursy wymiany walut obcych.

Interfejs API cennika znajduje się w innym punkcie końcowym niż inne Partner Center API. Informacje o cenach obejmują ceny mierników w USD dla zasobów planu platformy Azure i rezerwacje cenowe stosowane do subskrypcji planu platformy Azure.

Ten interfejs API umożliwia również partnerom pobieranie miesięcznych kursów wymiany, ponieważ ceny planu platformy Azure są dostępne tylko w USD. Za pomocą interfejsów API można pobrać zarówno ceny, jak i kursy wymiany walut dla bieżącego miesiąca lub poprzednich miesięcy.

>[!NOTE]
> Interfejs API cennika jest specyficzny dla cennika planu platformy Azure. Nadal należy używać istniejącego interfejsu API usługi RateCard i list cen opublikowanych na stronie "Cennik i oferty" usługi Partner Center dla zasobów platformy Azure lub rezerwacji wdrożonych w subskrypcjach spoza planu platformy Azure. Interfejs API cennika planu platformy Azure nie obsługuje cen oprogramowania, platformy handlowej ani licencji, takich jak Microsoft 365 lub Dynamics 365.

Aby uzyskać więcej informacji na temat cennika planu platformy Azure i interfejsów API kursów wymiany walut, zobacz pełną dokumentację [interfejsu API cennika](/partner/develop/pricing).

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
