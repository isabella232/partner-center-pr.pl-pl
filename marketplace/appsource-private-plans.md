---
title: Plany prywatne w programie Microsoft AppSource
description: Konfigurowanie planów prywatnych w Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936927"
---
# <a name="private-plans-in-microsoft-appsource"></a>Plany prywatne w programie Microsoft AppSource

Plany prywatne to sposób, w jaki wydawcy zapewniają plany niestandardowe określonym klientom. Ta opcja jest teraz dostępna w Microsoft AppSource. Plany prywatne można sprzedawać w usłudze AppSource dla ofert  oprogramowania jako usługi (SaaS) z wezwaniem do akcji Pobierz teraz.

## <a name="ask-your-isv-for-a-private-plan"></a>Poproś własnego isv o plan prywatny

Aby prywatny plan był dostępny w usłudze AppSource, musisz skontaktować się bezpośrednio z isv i wynegocjować niestandardową cenę i specyfikację techniczną. Gdy warunki planu prywatnego zostaną zaakceptowane, isv isv create a plan for you and assign it to your organization's tenant ID, which you need to provide.

### <a name="finding-your-tenant-id"></a>Znajdowanie identyfikatora dzierżawy

1. W usłudze AppSource w prawym górnym rogu wybierz ikonę profilu konta, a następnie pozycję **Wyświetl dzierżawę.**
2. Skopiuj identyfikator dzierżawy i podaj go u isV.

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Pokazuje, jak znaleźć identyfikator dzierżawy.":::

## <a name="find-a-private-plan-in-appsource"></a>Znajdowanie planu prywatnego w usłudze AppSource

Zanim nowy plan prywatny zostanie wyświetlony w usłudze AppSource, może upłynieć do 48 godzin od opublikowania przez isv isv nowego planu prywatnego. Aby znaleźć plany prywatne skojarzone z identyfikatorem dzierżawy, wybierz pozycję **Plany prywatne** (ikona blokady) w prawym górnym rogu usługi AppSource.

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Wyświetla ikonę blokady (kłódkę) na górnym pasku narzędzi.":::

Jeśli nie zalogowano się, zostanie wyświetlony monit o jej zalogowanie. Następnie możesz kupić plany prywatne skojarzone z identyfikatorem dzierżawy na **karcie Plany i cennik.**

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Przedstawia oferty prywatne na karcie planu i cennika.":::

Jeśli plany prywatne nie są dostępne dla dzierżawy, zostanie wyświetlony komunikat informujący o tym, że nie masz żadnych planów ani ofert prywatnych.

## <a name="purchase-a-private-plan"></a>Kupowanie planu prywatnego

IsV can include one or more private plans within an offer. Każda oferta może mieć zarówno plany publiczne, jak i prywatne, ale plany prywatne są wyświetlane na osobnej stronie oferty dostępnej za pośrednictwem ikony ofert prywatnych (kłódki) w prawym górnym rogu strony.

Dostępne plany prywatne są wyświetlane na **karcie Plany i cennik.** Plany prywatne mają niebieski wskaźnik.

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Wyświetla wskaźnik niebieskiej oferty prywatnej obok ofert prywatnych.":::

Aby kupić wybrany plan, wybierz pozycję **Pobierz teraz** i wykonaj podane kroki.

## <a name="next-steps"></a>Następne kroki

- [Co to jest usługa Microsoft AppSource?](appsource-overview.md)
