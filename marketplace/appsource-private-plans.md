---
title: Plany prywatne w Microsoft AppSource
description: Konfigurowanie planów prywatnych w Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: 2e55bd233d347cc7c23d60eb832c8fddfcfe524f4fb055e33e2a7a275eddee49
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115683861"
---
# <a name="private-plans-in-microsoft-appsource"></a>Plany prywatne w Microsoft AppSource

Plany prywatne to sposób, w jaki wydawcy zapewniają plany niestandardowe określonym klientom. Ta opcja jest teraz dostępna w Microsoft AppSource. Plany prywatne można sprzedawać w usłudze AppSource dla ofert  oprogramowania jako usługi (SaaS) za pomocą akcji Pobierz teraz.

## <a name="ask-your-isv-for-a-private-plan"></a>Poproś swojego isv isv o plan prywatny

Aby plan prywatny był dostępny w usłudze AppSource, musisz skontaktować się bezpośrednio z isv i wynegocjować niestandardową cenę i specyfikacje techniczne. Gdy warunki planu prywatnego zostaną zaakceptowane, isv isv create a plan for you and assign it to your organization's tenant ID, which you'll need to provide.

### <a name="finding-your-tenant-id"></a>Znajdowanie identyfikatora dzierżawy

1. W usłudze AppSource w prawym górnym rogu wybierz ikonę profilu konta, a następnie pozycję **Wyświetl dzierżawę.**
2. Skopiuj identyfikator dzierżawy i podaj go u isV.

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Pokazuje, jak znaleźć identyfikator dzierżawy.":::

## <a name="find-a-private-plan-in-appsource"></a>Znajdowanie planu prywatnego w usłudze AppSource

Zanim nowy plan prywatny zostanie wyświetlony w usłudze AppSource, może upłynieć do 48 godzin od opublikowania nowego planu prywatnego przez isv isv. Aby znaleźć plany prywatne skojarzone z identyfikatorem dzierżawy, wybierz pozycję **Plany prywatne** (ikona blokady) w prawym górnym rogu usługi AppSource.

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Wyświetla ikonę blokady (kłódkę) na górnym pasku narzędzi.":::

Jeśli nie zalogowano się, zostanie wyświetlony monit o jej zalogowanie. Następnie możesz kupić plany prywatne skojarzone z identyfikatorem dzierżawy na **karcie Plany i cennik.**

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Przedstawia oferty prywatne na karcie plan i cennik.":::

Jeśli plany prywatne nie są dostępne dla dzierżawy, zostanie wyświetlony komunikat informujący o tym, że nie masz żadnych planów ani ofert prywatnych.

## <a name="purchase-a-private-plan"></a>Kupowanie planu prywatnego

IsV can include one or more private plans within an offer( IsV can include one or more private plans within an offer. Każda oferta może mieć zarówno plany publiczne, jak i prywatne, ale plany prywatne są wyświetlane na osobnej stronie oferty dostępnej za pośrednictwem ikony oferty prywatnej (kłódki) w prawym górnym rogu strony.

Dostępne plany prywatne są wyświetlane na **karcie Plany i cennik.** Plany prywatne mają niebieski znaczek.

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Wyświetla niebieski wskaźnik oferty prywatnej obok ofert prywatnych.":::

Aby kupić wybrany plan, wybierz pozycję **Pobierz teraz** i wykonaj podane kroki.

## <a name="next-steps"></a>Następne kroki

- [Co to jest usługa Microsoft AppSource?](appsource-overview.md)
