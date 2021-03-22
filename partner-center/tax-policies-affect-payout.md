---
title: Jak zasady podatkowe wpływają na wypłatę w portalu Azure Marketplace
description: Dowiedz się, jak zasady podatkowe wpływają na wypłatę w portalu Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 817cdb895efab553b6f0131cdcdcf9b24bc6db3e
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768826"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Jak zasady podatkowe wpływają na wypłatę w portalu Azure Marketplace

**Odpowiednie role**
-    Administrator globalny
-    Administrator zarządzania użytkownikami
-    Agent administracyjny

## <a name="introduction"></a>Wprowadzenie

Komercyjny Portal firmy Microsoft ma globalne zasięg. Transakcje odbywają się w różnych granicach i w zależności od tego, gdzie znajdują się niezależnego dostawcy oprogramowania i klienta, implikacje podatkowe mogą się różnić. Microsoft AppSource i Portal Azure Marketplace używają informacji o profilu podatkowym Centrum partnerskiego, aby określić kraj niezależnego dostawcy oprogramowania. Aby określić kraj klienta, użyj informacji rozliczeniowych klienta lub, jeśli klient znajduje się w Unii Europejskiej, korzystamy z dwóch różnych informacji.

Aby lepiej zrozumieć poniższe scenariusze, zapoznaj się z tabelą [szczegóły podatku](tax-details-marketplace.md) , która pokazuje, czy firma Microsoft zbiera i płaci podatki w imieniu wydawcy, czy też odpowiedzialność należy do wydawcy.

> [!NOTE]
> Wszystkie przykłady wartości sprzedaży i procenty podatku w tym temacie są przeznaczone tylko do celów informacyjnych.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Transakcje transakcyjne wydawcy w kraju podatków zarządzanym przez firmę Microsoft

**Scenariusz A** — transakcje, które odbywają się między wydawcą a klientem w [kraju podatków zarządzanym przez firmę Microsoft](tax-details-marketplace.md#microsoft-managed-countries). W tych transakcjach w momencie sprzedaży zostanie dodany podatek, a firma Microsoft wyśle ten podatek do odpowiedniego kraju. Nie są potrącane żadne podatki z tytułu wypłaty i opłaty za wypłaty są na wyłączność.

Zapoznaj się z [scenariuszem D](#foreign-publisher-transacts-with-us-customer) w przypadku transakcji między wydawcy spoza USA a klientem USA.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Pokazuje przepływ pracy dla scenariusza procesu wypłaty A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Operacje transakcyjne wydawcy w kraju podatków zarządzanym przez firmę Microsoft, w którym opłata za witrynę Marketplace to usługa opodatkowana

**Scenariusz B** — transakcje, które odbywają się między wydawcą w Stanach Zjednoczonych (zgodnie z informacjami o profilu podatkowym Centrum partnerskiego) do klienta w kraju podatków zarządzanym przez firmę Microsoft, w którym kraj nakłada podatek od opłaty witryny Marketplace (usługa podlegająca opodatkowaniu). W tym scenariuszu opłata za usługę magazynu jest odejmowana od wypłaty wydawcy.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Operacje transakcyjne wydawcy w kraju podatków zarządzanym przez program Publisher

**Scenariusz C** — transakcje, które odbywają się między wydawcą a klientem w kraju podatków zarządzanym przez wydawcę, które nie nakładają potrąconej zaliczki na podatek dla klientów. Klienci nie będą obciążani podatkiem w momencie sprzedaży i są zobowiązani przez wydawcę, aby uregulować wszystkie stosowne podatki.

Aby uzyskać więcej informacji na temat cen specyficznych dla kraju (na przykład w celu przesunięcia nadchodzącego opodatkowania) [, zobacz plany i cenniki dla ofert komercyjnych w portalu Marketplace](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Obce transakcje wydawcy z klientem USA

**Scenariusz D** — wszyscy wydawcy zagraniczni (zgodnie z informacjami o profilu podatkowym w centrum partnerskim) w krajach bez Traktatu USA (patrz [scenariusz E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) w celu sprzedaży do klienta opartego na USA (zgodnie z definicją adresu konta klienta). Rząd USA wymaga od firmy Microsoft potrącenia w imieniu wydawcy. Podatek potrącony od wypłaty do wydawcy jest obliczany na podstawie ceny oferty.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Wydawca obcy z postanowieniami umowy Transacting z klientem USA

**Scenariusz E** — wszyscy wydawcy zagraniczni (zgodnie z informacjami o profilu podatkowym w centrum partnerskim) w krajach z Traktatem Stanów Zjednoczonych, którzy wprowadzają sprzedaż do klienta opartego na USA (zgodnie z definicją adresu konta klienta). Administracja USA nie wymaga od firmy Microsoft powstrzymania podatku w imieniu wydawcy.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Wydawca obcy jest sprzedawany do klienta zarejestrowanego w Unii VAT w kraju zarządzanym przez firmę Microsoft (poza Irlandią)

**Scenariusz F** — wszystkie transakcje między wydawcami obcymi i klientami zarejestrowanymi w Unii VAT (poza Irlandią) w Microsoft-Managed kraju. Klient nie uiszcza podatku od sprzedaży.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Wydawca obcy jest sprzedawany do klienta zarejestrowanego w Unii VAT w kraju zarządzanym przez firmę Microsoft (w Irlandii)

**Scenariusz G** — wszystkie transakcje między wydawcami obcymi i klientami zarejestrowanymi w Unii VAT (w Irlandii) w Microsoft-Managed kraju. Klient płaci irlandzki podatek VAT, a firma Microsoft płaci ten podatek dla Irlandii rządowego.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty G.":::

## <a name="next-steps"></a>Następne kroki

- [Często zadawane pytania dotyczące programu Publisher](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instrukcje dotyczące tworzenia profilów płatności i podatków](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)