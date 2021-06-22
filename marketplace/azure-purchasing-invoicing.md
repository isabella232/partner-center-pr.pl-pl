---
title: Kupowanie oprogramowania i rozwiązań od Azure Marketplace
description: Dowiedz się więcej na temat narzędzi, które upraszczają i usprawniają zakupy oprogramowania i zarządzanie nim w Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: 11145280aad1ecd9777ec2fb7540e7d6479acfae
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431547"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace zakupu

Azure Marketplace wiele narzędzi i funkcji, które upraszczają i upraszczają proces zakupów, fakturowania i zarządzania zasadami zakupów.

## <a name="simplified-procurement"></a>Uproszczone zaopatrzenie

Witryna Azure Marketplace pomaga uprościć proces zaopatrzenia przy użyciu różnych opcji zakupu. W przypadku zakupu produktów przy użyciu karty kredytowej skojarzonej z kontem platformy Azure wszystkie zakupy zostaną skonsolidowane na jednej fakturze i rozliczane na wybranej karcie kredytowej. Jeśli jesteś dużym klientem, możesz dokonać zakupu przy użyciu konta Enterprise Agreement. W przypadku umowy EA wszelkie zakupy oprogramowania są automatycznie uwzględniane na fakturze za platformę Azure. Faktura będzie zawierać opłaty za użycie platformy Azure, a następnie opłaty za witrynę Azure Marketplace.

Zakup za pośrednictwem Azure Marketplace pozwala wyeliminować złożoność zarządzania poszczególnymi relacjami z dostawcami i fakturami. Otrzymasz jeden skonsolidowany miesięczny rachunek od firmy Microsoft, który obejmuje zarówno zakupy Azure Marketplace jak i opłaty za platformę Azure.

## <a name="permission-to-purchase"></a>Uprawnienie do zakupu

Po znaleźć odpowiednią aplikację, ukończenie zakupu jest proste. Będziesz jednak potrzebować odpowiednich uprawnień w ramach subskrypcji platformy Azure. Ponieważ platforma Azure działa w oparciu [o](/azure/role-based-access-control/overview) model Access Control (RBAC), Twoje  konto musi mieć uprawnienia właściciela subskrypcji lub współautora, aby dokonać zakupu. 

Przed zakończeniem zakupu upewnij się, że użytkownik ma poprawną konfigurację w dzierżawie platformy Azure. Pomoże to zapobiec błędom podczas zakupu.

W Azure Marketplace aplikacji w Azure Portal znajdź aplikację, którą chcesz kupić, a  następnie wybierz pozycję Utwórz lub Skonfiguruj **i zasubskrybuj**. Przed rozpoczęciem korzystania z nowego rozwiązania zostanie wyświetlony monit o ukończenie niektórych informacji.

> [!CAUTION]
> Zatwierdzenie w prywatnej witrynie Marketplace nie wskazuje zakupu rozwiązania.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Przycisk Utwórz oferty.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Przycisk Skonfiguruj i subskrybuj.":::

Jeśli chcesz wdrożyć rozwiązanie ze sklepu Azure Marketplace online, wybierz pozycję Pobierz teraz na stronie opisu produktu, a następnie zaloguj się przy użyciu poświadczeń konta platformy Azure. 

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Okno Azure Marketplace logowania.":::

Po zalogowaniu nastąpi przekierowanie do produktu w Azure Portal w celu ukończenia zakupu.

## <a name="purchase-policy-management"></a>Zarządzanie zasadami zakupu

Firma Microsoft umożliwia zarządzanie zakupami użytkowników za pośrednictwem profilu rozliczeniowego jako administrator subskrypcji platformy Azure. Wybierz jedną z trzech opcji:

- **Bezpłatna i płatna** — umożliwia użytkownikom uzyskanie Azure Marketplace aplikacji.
- **Bezpłatne** — umożliwia użytkownikom wdrażanie tylko bezpłatnego oprogramowania z Azure Marketplace.
- **Nie** — uniemożliwia użytkownikom wdrażanie jakiegokolwiek oprogramowania z Azure Marketplace.

Te ustawienia dotyczą wszystkich użytkowników z dostępem do subskrypcji platformy Azure, co daje możliwość kontrolowania zakupów IT za pośrednictwem Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Kontrolowanie zakupów IT za pośrednictwem Azure Portal.":::

## <a name="cost-management"></a>Zarządzanie kosztami

Podczas zakupu produktów w Azure Marketplace chcesz uzyskać szczegółowe informacje, które ułatwiają zarządzanie kosztami. Azure Cost Management to bezpłatne narzędzie do wyświetlania informacji o zakupionych produktach. Możesz użyć Cost Management, aby wyświetlić szczegółowe informacje o usługach, na które wydajesz pieniądze w czasie, oraz o tym, jak te koszty są śledzone względem ustawionych budżetów. Oprócz ustawiania budżetów można planować raporty i analizować koszty subskrypcji. Dowiedz się więcej o Azure Cost Management, wykonując Microsoft Learn modułu analizowania kosztów i tworzenia budżetów za [pomocą Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Możesz wyświetlić opłaty i faktury w witrynie Azure Marketplace w narzędziu analizy kosztów w obszarze usługi Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Użyj Azure Cost Management, aby uzyskać wgląd w zakupione produkty.":::

## <a name="purchase-validation-checks"></a>Sprawdzanie poprawności zakupu

Zakup oferty za pośrednictwem usługi Azure Marketplace może się nie powieść z różnych powodów. Użycie interfejsu wiersza polecenia (CLI) do zakupu jest bardziej prawdopodobne, że spowoduje błędy, ponieważ możesz próbować kupić ofertę, która jest niedostępny lub widoczny w Azure Marketplace. Poniżej przedstawiono kontrole, które mogą spowodować niepowodzenie zakupu:

1. Subskrypcja należy do grupy Enterprise Agreement (EA), a administrator UMOWY EA jest wyłączony Azure Marketplace zakupów.
1. Administrator umowy EA włączył zakupy tylko dla bezpłatnych ofert, a oferta jest ofertą płatną.
1. Oferta nie znajduje się na platformie handlowej.
1. Niezależny dostawca oprogramowania przestał sprzedawać ofertę, przynajmniej w Twoim regionie.
1. Subskrypcja, której używasz, należy do konta rozliczeniowego w regionie, w którym oferta nie jest dostępna.
1. Subskrypcja/konto rozliczeniowe nie jest skojarzone z prawidłowym instrumentem płatniczym (takim jak ważna karta kredytowa).
1. Subskrypcja należy do grupy Dostawca rozwiązań w chmurze (CSP), a isV odrzucił sprzedaż za pośrednictwem CSP.
1. Prywatna platforma handlowa jest włączona dla subskrypcji, a oferta nie znajduje się na liście dozwolonych ofert.
1. Oferta jest prywatna/w wersji zapoznawczej dla określonych klientów, a subskrypcja nie znajduje się na liście dozwolonych klientów.

## <a name="next-steps"></a>Następne kroki

- [Rozliczenia i fakturowanie](billing-invoicing.md)