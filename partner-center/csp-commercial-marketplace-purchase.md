---
title: Kupowanie ofert komercyjnej platformy handlowej
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak partnerzy programu CSP mogą używać platformy handlowej Partner Center, aby kupować oferty SaaS od niezależnych dostawców oprogramowania.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2984dbb3a02df91d5a2a284182476bf348a24f47
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958090"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Kupowanie produktów komercyjnej platformy handlowej dla klientów w Partner Center


**Odpowiednie role:** Administrator globalny | Agent administracyjny

Jako partner w programie Dostawca rozwiązań w chmurze (CSP) możesz używać platformy handlowej do kupowania subskrypcji dla klientów określonych produktów Oprogramowania jako usługi (SaaS) oferowanych przez niezależnych dostawców oprogramowania.

Oferowanie klientom subskrypcji SaaS od isvów może pomóc w odróżnieniu twojej firmy. Możesz również udzielić klientom dostępu do pakietów oprogramowania, które są powiązane z ich konkretnymi potrzebami biznesowymi. Licencjami i subskrypcjami tych produktów SaaS na platformie handlowej zarządza się od wydawców ISV tak samo jak licencjami i subskrypcjami produktów firmy Microsoft.

Możesz kupić **subskrypcje** SaaS oparte na licencjach lub **subskrypcje oparte na** użyciu. Aby dowiedzieć się więcej o różnicach między rozliczeniami opartymi na licencjach i na użyciu, zobacz [Podstawowe informacje o rozliczeniach.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Kupowanie opartych na licencjach i mierzonych subskrypcji SaaS w Partner Center

Subskrypcje opartych na licencjach lub mierzonych produktów SaaS oferowanych przez wydawców ISV są kupowane przy użyciu tego samego procesu, który jest procesem zakupu subskrypcji produktów firmy Microsoft.

Aby kupić subskrypcję SaaS opartą na licencji lub mierzoną w u Partner Center, zobacz Tworzenie, zawieszanie lub [anulowanie subskrypcji klientów.](create-a-new-subscription.md#create-a-new-subscription)

Za pomocą interfejsów [API Partner Center można](/partner-center/develop/) również tworzyć subskrypcje platformy handlowej dla klientów. (Aby uzyskać więcej informacji na temat używania Partner Center API, zobacz Tworzenie subskrypcji dla produktów platformy [handlowej).](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> Jako partner w programie CSP  możesz kupić oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center. Oznacza to, że  możesz kupić dowolną opartą na licencjach lub mierzoną [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ofertę **SaaS,** która została Ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp. Aby zakupić inne, komercyjne oferty platformy handlowej od isvs (np. ofert opartych na użyciu obejmujących aplikacje platformy Azure, kontenery lub maszyny wirtualne) lub zarządzać nimi, musisz przejść do witryny [Azure Portal](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Kupowanie subskrypcji opartych na użyciu w Azure Portal

W przeciwieństwie do opartych na licencjach subskrypcji SaaS od zewnętrznych wydawców isv, subskrypcje oparte na użyciu najpierw wymagają od klienta subskrypcji platformy Azure. Rozliczenia dla komercyjnej platformy handlowej zasoby oparte na użyciu są dostępne w ramach subskrypcji platformy Azure klienta. Gdy klient ma subskrypcję platformy Azure, partner w programie CSP może wykonać następujące kroki, aby kupić dla nich subskrypcję platformy handlowej:

1. Zaloguj się do Partner Center [nawigacyjnego,](https://partner.microsoft.com/dashboard)a następnie wybierz **pozycję Klienci** z menu po lewej stronie.

2. Wybierz określonego klienta, a następnie wybierz **pozycję Subskrypcje.**  

3. W obszarze **Subskrypcje oparte na użyciu** wybierz pozycję **Wszystkie zasoby.** W ten sposób zostaniesz przekierowywny do portalu zarządzania platformy Azure.

4. W portalu zarządzania platformy Azure wybierz **pozycję Utwórz zasób** z menu po lewej stronie.

5. Wybierz **pozycję Zobacz** wszystko w górnej części Azure Marketplace listy.

6. Aby zawęzić listę, użyj filtrów w górnej części listy w witrynie Marketplace. Na przykład możesz wybrać pozycję **Microsoft** lub **Partner** z listy rozwijanej **Publisher,** aby wyświetlić tylko oferty firmy Microsoft lub oferty od wydawcy isv.

7. Wybierz określoną ofertę, a następnie wybierz pozycję **Utwórz.**

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie ofertami komercyjnej platformy handlowej](csp-commercial-marketplace-purchase.md)