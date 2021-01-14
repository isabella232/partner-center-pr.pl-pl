---
title: Kupowanie oprogramowania i rozwiązań z portalu Azure Marketplace
description: Poznaj narzędzia, które upraszczają i usprawniają zakupy oprogramowania i zarządzanie nimi w portalu Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 8f7962b1b040be90f7dc1b2696a2ced3830d25b9
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182481"
---
# <a name="azure-marketplace-purchasing"></a>Kupowanie w portalu Azure Marketplace

Witryna Azure Marketplace oferuje wiele narzędzi i funkcji, które upraszczają i usprawniają proces kupowania, fakturowania i zarządzania zasadami zakupów.

## <a name="simplified-procurement"></a>Uproszczone zaopatrzenie

Witryna Azure Marketplace pomaga uprościć proces zaopatrzenia przy użyciu różnych opcji zakupu. Jeśli kupisz produkty przy użyciu karty kredytowej skojarzonej z kontem platformy Azure, wszystkie zakupy będą skonsolidowane na pojedynczej fakturze i rozliczane za wybraną kartę kredytową. Jeśli jesteś dużym klientem, możesz kupić przy użyciu Umowa Enterprise. W przypadku umowy EA wszystkie zakupy oprogramowania są automatycznie dołączane do faktury platformy Azure. Faktura będzie zawierać opłaty za użycie platformy Azure, a następnie opłaty za witrynę Azure Marketplace.

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

## <a name="next-steps"></a>Następne kroki

- [Rozliczenia i fakturowanie](billing-invoicing.md)