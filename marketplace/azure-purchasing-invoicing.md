---
title: Kupowanie oprogramowania i rozwiązań z portalu Azure Marketplace
description: Poznaj narzędzia, które upraszczają i usprawniają zakupy oprogramowania i zarządzanie nimi w portalu Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: ac20b3c0603f886104499ab8de6da1d3459bbd57
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412577"
---
# <a name="azure-marketplace-purchasing"></a>Kupowanie w portalu Azure Marketplace

Witryna Azure Marketplace oferuje wiele narzędzi i funkcji, które upraszczają i usprawniają proces kupowania, fakturowania i zarządzania zasadami zakupów.

## <a name="simplified-procurement"></a>Uproszczone zaopatrzenie

Witryna Azure Marketplace pomaga uprościć proces zaopatrzenia przy użyciu różnych opcji zakupu. Jeśli kupisz produkty przy użyciu karty kredytowej skojarzonej z kontem platformy Azure, wszystkie zakupy będą skonsolidowane na pojedynczej fakturze i rozliczane za wybraną kartę kredytową. Jeśli jesteś dużym klientem, możesz kupić przy użyciu Enterprise Agreement. W przypadku umowy EA wszystkie zakupy oprogramowania są automatycznie dołączane do faktury platformy Azure. Faktura będzie zawierać opłaty za użycie platformy Azure, a następnie opłaty za witrynę Azure Marketplace.

Zakup w witrynie Azure Marketplace pozwala wyeliminować złożoność zarządzania relacjami i fakturami poszczególnych dostawców. Otrzymasz jeden skonsolidowany miesięczny rachunek od firmy Microsoft, który obejmuje zarówno zakupy w portalu Azure Marketplace, jak i opłaty za korzystanie z platformy Azure.

## <a name="permission-to-purchase"></a>Uprawnienie do zakupu

Po znalezieniu odpowiedniej aplikacji programowej kupowanie jest proste. Będą jednak potrzebne odpowiednie uprawnienia w ramach subskrypcji platformy Azure. Ponieważ platforma Azure działa w modelu [opartym na rolach Access Control](/azure/role-based-access-control/overview) (RBAC), Twoje konto musi mieć uprawnienia **właściciela subskrypcji** lub **współautora** do zakupu.

Przed ukończeniem zakupu upewnij się, że użytkownik ma poprawną konfigurację w dzierżawie platformy Azure. Pomoże to uniknąć błędów podczas zakupu.

W środowisku portalu Azure Marketplace w Azure Portal Znajdź aplikację, którą chcesz kupić, a następnie wybierz pozycję **Utwórz** lub **Skonfiguruj + Subskrybuj**. Przed rozpoczęciem korzystania z nowego rozwiązania zostanie wyświetlony monit o ukończenie pewnych informacji.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Przycisk tworzenia oferty.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Przycisk Konfiguruj + Subskrybuj.":::

Jeśli chcesz wdrożyć rozwiązanie ze sklepu online w portalu Azure Marketplace, wybierz pozycję **Pobierz teraz** na stronie opis produktu, a następnie zaloguj się przy użyciu poświadczeń konta platformy Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Okno dialogowe logowania do portalu Azure Marketplace.":::

Po zalogowaniu nastąpi przekierowanie do produktu w Azure Portal, aby zakończyć zakupu.

## <a name="purchase-policy-management"></a>Zarządzanie zasadami zakupów

Firma Microsoft umożliwia zarządzanie zakupami użytkowników w ramach Twojego profilu rozliczeniowego jako administrator subskrypcji platformy Azure. Wybieraj spośród trzech opcji:

- **Bezpłatna i płatna** — umożliwia użytkownikom uzyskanie dowolnej aplikacji oprogramowania w portalu Azure Marketplace.
- **Bezpłatna** — umożliwia użytkownikom wdrażanie tylko bezpłatnego oprogramowania z witryny Azure Marketplace.
- **Nie** — uniemożliwia użytkownikom wdrażanie dowolnego oprogramowania z witryny Azure Marketplace.

Te ustawienia mają zastosowanie do wszystkich użytkowników mających dostęp do subskrypcji platformy Azure, co daje możliwość kontrolowania zakupów IT za pomocą Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Kontrolowanie zakupów IT za pomocą Azure Portal":::

## <a name="cost-management"></a>Zarządzanie kosztami

Gdy kupujesz produkty z witryny Azure Marketplace, chcesz uzyskać szczegółowe informacje ułatwiające zarządzanie kosztami. Azure Cost Management to bezpłatne narzędzie do wyświetlania informacji o kupionych produktach. Możesz użyć Cost Management, aby zobaczyć szczegółowe informacje o usługach, na których spędzasz pieniądze, i o tym, jak te koszty śledzą ustawione budżety. Oprócz ustawiania budżetów można planować raporty i analizować koszty subskrypcji. Dowiedz się więcej o Azure Cost Management, wypełniając moduł Microsoft Learn w celu [analizowania kosztów i tworzenia budżetów przy użyciu Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Możesz wyświetlić opłaty i faktury w witrynie Azure Marketplace w narzędziu analizy kosztów w obszarze usługi Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Użyj Azure Cost Management, aby uzyskać wgląd w zakupione produkty.":::

## <a name="purchase-validation-checks"></a>Sprawdzanie poprawności zakupów

Zakup oferty w portalu Azure Marketplace może zakończyć się niepowodzeniem z różnych powodów. Korzystanie z interfejsu wiersza polecenia (CLI) dla zakupu może spowodować błędy, ponieważ użytkownik próbuje zakupić ofertę, która nie jest dostępna ani widoczna w portalu Azure Marketplace. Poniżej przedstawiono testy, które mogą spowodować niepowodzenie zakupu:

1. Subskrypcja należy do Enterprise Agreement (EA), a administrator EA wyłączył zakupy w portalu Azure Marketplace.
1. Administrator EA włączył zakupy tylko dla bezpłatnych ofert, a oferta jest ofertą płatną.
1. Oferta nie została znaleziona w portalu Marketplace.
1. Niezależny dostawca oprogramowania (ISV) przestał sprzedawać ofertę, co najmniej w Twoim regionie.
1. Używana subskrypcja należy do konta rozliczeniowego w regionie, w którym oferta jest niedostępna.
1. Konto subskrypcji/rozliczeń nie jest skojarzone z prawidłowym instrumentem płatniczym (takim jak karta kredytowa).
1. Subskrypcja należy do dostawcy rozwiązań w chmurze (CSP) i niezależnego od dostawcy oprogramowania.
1. Dla subskrypcji jest włączona funkcja Private Marketplace, a oferta nie znajduje się na liście dozwolonych ofert.
1. Oferta jest prywatna/w wersji zapoznawczej dla określonych klientów i subskrypcja nie znajduje się na liście dozwolonych klientów.

## <a name="next-steps"></a>Następne kroki

- [Rozliczenia i fakturowanie](billing-invoicing.md)