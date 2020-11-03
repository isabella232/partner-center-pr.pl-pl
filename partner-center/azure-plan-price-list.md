---
title: Lista cen planu platformy Azure dla partnerów programu CSP
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób partnerzy programu CSP mogą korzystać z Centrum partnerskiego, aby wyświetlić listę cen dla subskrypcji w ramach planu platformy Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 57e976f2968f0bd6b13f36eb04be9f68577d1389
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529931"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Cennik dla nowego środowiska handlowego w programie CSP dla platformy Azure

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Administrator globalny
- Agent pomocy technicznej
- Agent sprzedaży
- Administrator zarządzania użytkownikami

Cennik dla nowego środowiska Azure commerce w programie CSP jest ogłaszany w centrum partnerskim. Cennik jest dostarczany dynamicznie w czasie rzeczywistym, a ceny są wyświetlane tylko w USD. Rozliczanie jest jednak wykonywane w ramach obsługiwanej waluty dotyczącej lokalizacji waluty klienta. Aby uzyskać więcej informacji na temat rozliczeń w lokalizacji walutowej klienta, zapoznaj się z artykułem [Azure plan — rozliczenia](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Zobacz cennik dla subskrypcji w ramach cennika usługi Azure plan

1. W menu Centrum partnerskiego po lewej stronie wybierz pozycję **Sprzedaj** , a następnie wybierz pozycję Portal **Marketplace**.

2. W obszarze Cennik planu platformy Azure wybierz kraj, dla którego chcesz uzyskać cennik.

3. Obok pozycji **Typ eksportu** wybierz pozycję **Cennik użycia planu platformy Azure** , **Cennik rezerwacji planu platformy Azure** lub **kursy FX**. 

>[!NOTE] 
>**Stawki FX** nie są specyficzne dla kraju.

4. Obok pozycji **Cennik** wybierz żądaną datę, na przykład **Current**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="specyficzne dla kraju":::

>[!NOTE] 
>Możesz wyeksportować dwie różne cenniki — Cennik planu platformy Azure i ceny innych firm.

## <a name="azure-price-list-specifics"></a>Szczegóły cennika platformy Azure

- Cennik planu platformy Azure będzie dostępny na stronie witryny Marketplace w centrum partnerskim w obszarze **Sprzedaj**.

- Eksporty będą dostępne dla usług zużycia planu platformy Azure, Azure Reservations i kursów FX.

- Opcje eksportu obejmują:

  - **Dzisiejsze ceny** : obejmują wszystkie liczniki i ceny z 1. miesiąca do bieżącej daty bieżącego miesiąca. Obejmuje to nowe ceny, zmienione ceny lub ceny zostały usunięte. Wszystkie ceny będą mieć efektywne daty rozpoczęcia i zakończenia, aby wyjaśnić, czy są one nowe lub usunięte.

  - **Cennik w poprzednim miesiącu** : pliki do pobrania dla każdego typu zasobu będą według miesiąca. W przypadku plików cenowych zostaną uwzględnione wszystkie liczniki, które były dostępne w danym miesiącu. Jeśli nowy licznik pojawił się w połowie miesiąca, zostanie pokazany jako licznik z rzeczywistą datą odzwierciedlającą jego dostępność. Podobnie jak w przypadku cen, które są wycofane, pokazując, że nie są już dostępne.

  - **Kursy FX** : stawki FX będą dostępne do pobrania dnia przed 1. dnia miesiąca, 18:00 PST. Na przykład jeśli chcesz użyć stawek za listopad, Pobierz stawki w dniu 31 października. Dostępne są również stawki za poprzedni miesiąc FX.

- Ceny na cenniku są cenami bezpośrednimi. Niektórzy partnerzy mogą kwalifikować się do kredytów na korzystanie z partnerów. Aby uzyskać informacje o tym, jak naliczany jest kredyt uzyskany przez partnera, należy zapoznać się z informacjami o [tym, jak są obliczane i płatne środki w ramach](partner-earned-credit-explanation.md)

- **Kwalifikujące się usługi** : środki na korzystanie z partnerów mają zastosowanie [w przypadku usług](https://partner.microsoft.com/commerce/sales) wymienionych w obszarze partnerów **cen za użycie planu platformy Azure** . Należy pamiętać, że istnieją wyjątki, w tym między innymi produkty innych firm zidentyfikowane jako "trzecie" w kolumnie Tagi listy cen zużycia planu platformy Azure i rezerwacje planu platformy Azure.

## <a name="price-list-data"></a>Cennik — dane

|**Pole**   |**Opis**   |
|--------------------------|:---------------------------|
|ProductTitle  |Tytuł lub nazwa produktu|
|ProductID   |Identyfikator produktu|
|Identyfikatora skuId|Identyfikator jednostki SKU|
|SkuTitle|Tytuł lub nazwa jednostki SKU|
|Publisher|Pierwsza strona będzie zawsze firmą Microsoft|
|SkuDescription|Opis jednostki SKU|
|UnitOfMeasure|Jednostki, za które będą naliczane opłaty lub opłaty|
|TermDuration|W przypadku produktów opartych na terminach długość okresu, która ma zastosowanie do rezerwacji|
|Do|Rynek cen|
|Waluta|Waluta cen|
|Cena jednostkowa|Cena za jednostkę|
|PricingTierRangeMin|W przypadku cen warstwowych stosowana jest cena minimalna|
|PricingTierRangeMax|W przypadku cen warstwowych stosowana jest maksymalna cena|
|EffectiveStartDate|Data rozpoczęcia cennika|
|EffectiveEndDate|Data końcowa cen|
|MeterIds|Identyfikator licznika jednostki SKU produktu|
|Licznik mierników|Typ miernika|
|Tagi|Właściwości dla elementu — Cennik planu platformy Azure to platforma Azure lub platforma Azure i rezerwacje (w przypadku zastrzeżeń)|

Cennik usługi Azure plan można wyeksportować ze [strony Cennik i oferty](https://partner.microsoft.com/dashboard/sell/pricingandoffers) w centrum partnerskim.

## <a name="tiered-pricing"></a>Cennik warstwowy

Niektóre usługi zużycia w planie platformy Azure obsługują ceny warstwowe. Partnerzy mogą znaleźć te produkty i jednostki SKU na liście cen planu platformy Azure. Elementy, które mają wartości w kolumnie zakres warstwy cenowej, umożliwiają partnerom zrozumienie ceny na podstawie użycia. W poniższym przykładzie za pomocą przykładowych danych mamy jedną jednostkę SKU produktu z trzema warstwami cenowymi.

|**Produktu**   |**Identyfikatora skuId**   |**Cena jednostkowa**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

W tym przykładzie, jeśli są używane jednostki 101, opłata wynosi 100,80. Pierwsze 100 jednostek to jedna z nich, a kolejna jednostka jest naliczana na. 80.

## <a name="pricing-api-for-azure-plan"></a>Interfejs API cen dla planu platformy Azure

Korzystając z [interfejsu API cennika](/partner/develop/pricing) , można programowo pobrać Cennik usługi Azure plan na potrzeby użycia i rezerwacji. Możesz również pobrać obce kursy wymiany.

Interfejs API cen znajduje się w innym punkcie końcowym niż inne interfejsy API Centrum partnerskiego. Informacje o cenach obejmują Cennik taryfowy w USD dla zasobów planu platformy Azure i zastrzeżeń związanych z subskrypcjami planu platformy Azure.

Ten interfejs API umożliwia także partnerom pobieranie miesięcznych stawek za wymianę, ponieważ Cennik usługi Azure plan jest tylko w USD. Interfejsów API można używać do pobierania cen i kursów wymiany walut w bieżącym miesiącu lub w poprzednich miesiącach.

>[!NOTE]
> Interfejs API cen jest specyficzny dla cen planu platformy Azure. Nadal powinieneś korzystać z istniejącego interfejsu API RateCard i cenników opublikowanych na stronie "Cennik i oferty" Centrum partnerskiego dla zasobów platformy Azure lub rezerwacji wdrożonych w ramach subskrypcji planu niezwiązanego z platformą Azure. Interfejs API cen planu platformy Azure nie obsługuje oprogramowania, platformy Marketplace ani cen opartych na licencji, takich jak Microsoft 365 lub Dynamics 365.

Aby uzyskać więcej informacji na temat cen planu platformy Azure i interfejsów API obcych kursów wymiany, zobacz [dokumentację interfejsu API pełnej ceny](/partner/develop/pricing).