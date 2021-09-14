---
title: Jak zasady podatkowe wpływają na wypłaty dla Azure Marketplace
description: Dowiedz się, jak zasady podatkowe wpływają na wypłaty dla Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 6a069db0334b13309e39e08bcc7b70f22eaa5c69
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246615"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Jak zasady podatkowe wpływają na wypłaty dla Azure Marketplace

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny

## <a name="introduction"></a>Wprowadzenie

Platforma handlowa firmy Microsoft ma globalny zasięg. Transakcje występują za granice i w zależności od tego, gdzie znajduje się niezależny dostawca oprogramowania i klient, implikacje podatkowe mogą się różnić. Microsoft AppSource i Azure Marketplace informacji o profilu Partner Center, aby określić kraj isv.isv. Aby określić kraj klienta, użyj informacji rozliczeniowych klienta lub, jeśli klient znajduje się w Unii Europejskiej, użyjemy dwóch różnych informacji.

Aby lepiej zrozumieć poniższe scenariusze, zapoznaj się z tabelą Szczegóły podatku, w której pokazano, czy firma Microsoft zbiera i płaci podatki w imieniu wydawcy, czy też ta odpowiedzialność należy do wydawcy. [](tax-details-marketplace.md)

> [!NOTE]
> Wszystkie przykłady wartości sprzedaży i wartości procentowe podatku w tym temacie mają charakter wyłącznie ilustrujący, a nie dokładne wartości.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Publisher Transakcje w kraju podatkowym zarządzanym przez firmę Microsoft

**Scenariusz A** — transakcje, które odbywają się między wydawcą a klientem w kraju podatkowym zarządzanym przez firmę [Microsoft.](tax-details-marketplace.md#microsoft-managed-countries) Te transakcje będą mieć zastosowanie do podatku dodanego w momencie sprzedaży, a firma Microsoft wyśle ten podatek do odpowiedniego kraju. Żadne podatki nie są potrącone z wypłaty, a obliczenia wypłat są bez podatku.

Zobacz [scenariusz D](#foreign-publisher-transacts-with-us-customer) dla transakcji między wydawcą w innym niż USA a klientem w USA.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Przedstawia przepływ pracy dla scenariusza A procesu wypłaty.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher Transakcje w kraju podatkowym zarządzanym przez firmę Microsoft, w którym opłata za korzystanie z witryny Marketplace jest usługą serwisową

Scenariusz **B** — transakcje, które odbywają się między wydawcą w Usa (określonym w informacjach o profilu podatkowym w usłudze Partner Center) dla klienta w kraju podatkowym zarządzanym przez firmę Microsoft, w którym kraj nakłada podatek na opłatę za korzystanie z witryny Marketplace (usługę w witrynie Marketplace). W tym scenariuszu podatek od opłaty za usługę sklepu jest odejmowany od wypłaty wydawcy.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Publisher Transakcje w zarządzanym Publisher podatkowym

**Scenariusz C** — transakcje odbywające się między wydawcą i klientem w kraju podatkowym zarządzanym przez wydawcę, który nie nakłada na klientów podatku potrącanego. Klienci nie płacą podatku w punkcie sprzedaży i wydawca ma obowiązek płacenia wszystkich obowiązujących podatków.

Aby uzyskać więcej informacji na temat cen specyficznych dla kraju (na przykład w celu przesunięcia przyszłego podatku), zobacz Plany i ceny ofert [platformy handlowej](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Transakcje Publisher z klientem w USA

**Scenariusz D** — wszyscy wydawcy obcy (zgodnie z definicją w informacjach o profilu podatkowym w Partner Center) w krajach bez amerykańskiej firmy (zobacz scenariusz [E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)dokonujący sprzedaży klientowi z USA (zgodnie z jego adresem konta klienta). Rząd STANÓW Zjednoczonych wymaga, aby firma Microsoft wstrzymała podatek w imieniu wydawcy. Wstrzymanie podatku od wypłaty do wydawcy jest obliczane na podstawie ceny oferty.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Wydawca obcy z transakcyjną transakcją ze strony klienta w USA

**Scenariusz E** — wszyscy obci wydawcy (zgodnie z definicją w informacjach o profilu podatkowym w Partner Center) w krajach, w których w Usa dokonano sprzedaży dla klienta z siedzibą w USA (zgodnie z jego adresem konta klienta). Rząd STANÓW Zjednoczonych nie wymaga od firmy Microsoft wstrzymać podatku w imieniu wydawcy.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Obcy wydawca sprzedaje klientowi zarejestrowanego w UNII podatku VAT w kraju zarządzanym przez firmę Microsoft (poza Irlandią)

**Scenariusz F** — wszystkie transakcje między wydawcami zewnętrznymi a klientami zarejestrowanymi w unii europejskiej z tytułu podatku od wartości dodanej (VAT) (poza Irlandią) w Microsoft-Managed kraju. Klient nie płaci podatku od sprzedaży.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Obcy wydawca sprzedaje klientowi zarejestrowanego w UNII podatku VAT w kraju zarządzanym przez firmę Microsoft (w Niemczech)

**Scenariusz G** — wszystkie transakcje między wydawcami obcymi a klientami zarejestrowanymi w ue pod rygorami VAT (w Niemczech) w Microsoft-Managed kraju. Klient płaci podatku VAT w witrynie Microsoft, a firma Microsoft płaci ten podatek rządowi w Witrynie.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY G.":::

## <a name="next-steps"></a>Następne kroki

- [Publisher FAQ](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instrukcje dotyczące tworzenia profilów płatności i profilów podatkowych](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)