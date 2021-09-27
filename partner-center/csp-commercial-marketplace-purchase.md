---
title: Kupowanie ofert komercyjnej platformy handlowej
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak partnerzy programu CSP mogą używać platformy handlowej Partner Center, aby kupować oferty SaaS od niezależnych dostawców oprogramowania.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d06f64280ee89df241e150b2ad9c44adb7f7aa2f
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072270"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Kupowanie produktów komercyjnej platformy handlowej dla klientów w Partner Center


**Odpowiednie role:** Administrator globalny | Agent administracyjny

Jako partner w programie Dostawca rozwiązań w chmurze (CSP) możesz używać platformy handlowej do kupowania subskrypcji dla klientów określonych produktów oprogramowania jako usługi (SaaS) oferowanych przez niezależnych dostawców oprogramowania.

Oferowanie klientom subskrypcji SaaS dla isv isv, może pomóc w odróżnieniu twojej firmy. Możesz również udzielić klientom dostępu do pakietów oprogramowania, które są specyficzne dla ich potrzeb biznesowych. Licencjami i subskrypcjami tych produktów SaaS na platformie handlowej zarządza się od wydawców ISV tak samo jak licencjami i subskrypcjami produktów firmy Microsoft.

Możesz kupić **subskrypcje** SaaS oparte na licencjach lub **subskrypcje oparte na** użyciu. Aby dowiedzieć się więcej na temat różnicy między rozliczeniami opartymi na licencjach i na użyciu, zobacz [Podstawowe informacje o rozliczeniach.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Kupowanie opartych na licencjach i mierzonych subskrypcji SaaS w Partner Center

Subskrypcje oparte na licencjach lub mierzone produkty SaaS oferowane przez wydawców ISV są kupowane przy użyciu tego samego procesu, który jest przetwarzany w celu zakupu subskrypcji produktów firmy Microsoft.

Aby kupić opartą na licencjach lub mierzoną subskrypcję SaaS w Partner Center, zobacz Tworzenie, wstrzymywanie lub [anulowanie subskrypcji klientów.](create-a-new-subscription.md#create-a-new-subscription)

Możesz również użyć Partner Center [API do](/partner-center/develop/) tworzenia subskrypcji platformy handlowej dla klientów. (Aby uzyskać więcej informacji na temat używania Partner Center API, zobacz Tworzenie subskrypcji dla produktów platformy [handlowej).](/partner-center/develop/create-subscription-azure-marketplace-products)

> [!IMPORTANT]
> Jako partner w programie CSP  możesz kupować oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center. Oznacza to, że  możesz kupić dowolną ofertę **SaaS** opartą na licencjach lub taryfowej, która została ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp. [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) Aby zakupić inne, komercyjne oferty platformy handlowej lub zarządzać nimi od wirtualnych klientów (takich jak oferty oparte na użyciu obejmujące aplikacje platformy Azure, kontenery lub maszyny wirtualne), musisz przejść do witryny [Azure Portal.](https://portal.azure.com/)

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Kupowanie subskrypcji opartych na użyciu w Azure Portal

W przeciwieństwie do opartych na licencjach subskrypcji SaaS od innych wydawców isv, subskrypcje oparte na użyciu najpierw wymagają od klienta subskrypcji platformy Azure. Rozliczenia dla komercyjnej platformy handlowej zasoby oparte na użyciu są dostępne w ramach subskrypcji platformy Azure klienta. Gdy klient ma subskrypcję platformy Azure, partner w programie CSP może wykonać następujące kroki, aby kupić dla nich subskrypcję platformy handlowej:

> [!NOTE]
> Interfejs Partner Center wersji zapoznawczej zapewnia bardziej wydajne i wydajne środowisko użytkownika za pośrednictwem logicznie zgrupowanych obszarów roboczych. Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych i sposobu jego włączanie, zobacz Getting around Partner Center (Poruszanie [się po Partner Center).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Zaloguj się do pulpitu [Partner Center,](https://partner.microsoft.com/dashboard)a następnie wybierz **kafelek** Klienci.

2. Wybierz określonego klienta, a następnie wybierz **pozycję Subskrypcje.**  

3. W obszarze **Subskrypcje oparte na użyciu** wybierz pozycję **Wszystkie zasoby.** Zostanie on przekierowyny do portalu zarządzania platformy Azure.

4. W portalu zarządzania platformy Azure wybierz pozycję **Utwórz zasób** z menu po lewej stronie.

5. Wybierz **pozycję Zobacz** wszystko w górnej części Azure Marketplace listy.

6. Aby zawęzić listę, użyj filtrów w górnej części listy Marketplace. Na przykład możesz wybrać pozycję **Microsoft** lub **Partner** z listy rozwijanej **Publisher,** aby wyświetlić tylko oferty firmy Microsoft lub te od wydawcy isv.

7. Wybierz określoną ofertę, a następnie wybierz **pozycję Utwórz.**

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Zaloguj się na Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **Klienci** z menu po lewej stronie.

2. Wybierz określonego klienta, a następnie wybierz **pozycję Subskrypcje.**  

3. W obszarze **Subskrypcje oparte na użyciu** wybierz pozycję **Wszystkie zasoby.** Zostanie on przekierowyny do portalu zarządzania platformy Azure.

4. W portalu zarządzania platformy Azure wybierz pozycję **Utwórz zasób** z menu po lewej stronie.

5. Wybierz **pozycję Zobacz** wszystko w górnej części Azure Marketplace listy.

6. Aby zawęzić listę, użyj filtrów w górnej części listy Marketplace. Na przykład możesz wybrać pozycję **Microsoft** lub **Partner** z listy rozwijanej **Publisher,** aby wyświetlić tylko oferty firmy Microsoft lub te od wydawcy isv.

7. Wybierz określoną ofertę, a następnie wybierz **pozycję Utwórz.**

* * *

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie ofertami komercyjnej platformy handlowej](csp-commercial-marketplace-purchase.md)
