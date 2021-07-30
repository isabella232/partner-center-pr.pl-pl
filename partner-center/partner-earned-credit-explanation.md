---
title: Środków uzyskane przez partnerów na usługi zarządzane
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak są obliczane i opłacane punkty uzyskane przez partnerów firmy Microsoft dla usług zarządzanych oraz jak upewnić się, że kwalifikujesz się.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 6af1e55ffdd1b807c71914ba3247ecc2d189c6ad
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114839944"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Jak są obliczane i wypłacane środki zarobione przez partnera

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny | Administrator rozliczeń | Agent sprzedaży

Punkty uzyskane przez partnerów dla usług zarządzanych rozpoznaje i nagradza partnerów, którzy są właścicielami kontroli operacyjnej IT i zarządzania niektórym lub wszystkimi środowiskami platformy Azure klientów. 

Domyślnie jako partner CSP masz przyznane niezbędne prawa dostępu do subskrypcji klienta, co pozwala na zarządzanie operacyjne i kontrolę nad zasobami w ramach subskrypcji. Inne sposoby, w jakie klienci mogą aprowizują dostęp dla partnerów transakcji, opisano w poniższej sekcji.

Miesięczna kwota faktury jest wartością netto środków uzyskanego przez partnera. Szczegóły dotyczące PEC można znaleźć w miesięcznym pliku rekonescji. Aby uzyskać dodatkowe sposoby, w jakie klient może aprowizowania dostępu dla partnera transakcji, zobacz następujące artykuły:

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Przywracanie uprawnień administratora dla subskrypcji w ramach programu Azure CSP](/revoke-reinstate-csp.md)

## <a name="eligibility"></a>Kwalifikowalności

W celu otrzymania środków uzyskane przez partnerów obowiązują następujące wymagania:

- Musisz mieć aktywną umowę MPN i [](azure-roles-perms-pec.md) prawidłową rolę kontroli dostępu opartej na rolach [(RBAC).](/azure/role-based-access-control/overview)
- Musisz mieć uprawnienia [Administratora w imieniu (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) w subskrypcji platformy Azure klienta, grupie zasobów platformy Azure lub zasobie platformy Azure albo mieć prawidłową [rolę RBAC.](azure-roles-perms-pec.md)
- W przypadku dostawców pośrednich i ich pośrednich odsprzedawców dostawca pośredni kwalifikuje się do PEC, jeśli dostawca pośredni lub odsprzedawca pośredni albo obaj mają uprawnienia AOBO lub kwalifikującą się rolę RBAC. Aby uzyskać więcej informacji, zobacz [Przywróć uprawnienia administratora dla Azure CSP subskrypcji.](revoke-reinstate-csp.md)
- Identyfikator MPN partnera musi należeć do tej samej organizacji wirtualnej co identyfikator MPN nabywcy lub identyfikator MPN partnera rekordów (POR). Aby uzyskać więcej informacji, zobacz [Łączenie identyfikatora partnera w celu śledzenia wpływu na delegowane zasoby](/azure/lighthouse/how-to/partner-earned-credit).
- PEC jest zdobywany na poziomie zasobów, grupy zasobów lub subskrypcji platformy Azure. Jeśli partner ma prawidłowy dostęp na poziomie subskrypcji lub grupy zasobów, każdy zasób, który jest zbiorczy do wyższej jednostki, będzie zdobywać PEC.
- PEC nie ma zastosowania do następujących usług:
    - Rezerwacje planu platformy Azure
    - Produkty innych firm zidentyfikowane jako produkty innych firm w kolumnie Tagi ceny za zużycie planu platformy Azure
    - Produkty w cenniku witryny Marketplace
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

Oprócz powyższych wymagań PEC ma zastosowanie tylko do usług wymienionych w cenniku użycia planu platformy Azure. Możesz je wyświetlić i wyeksportować na stronie [cennika planu platformy Azure.](https://partner.microsoft.com/commerce/sales)

Aby uzyskać więcej informacji na temat PEC, zobacz [stronę Azure Cost management (Zarządzanie kosztami platformy Azure).](/azure/cost-management-billing/costs/get-started-partners)

Aby uzyskać więcej informacji na temat uprawnień, zobacz Role i uprawnienia wymagane do [zdobywania środków zdobytych przez partnera.](azure-roles-perms-pec.md)

## <a name="calculation"></a>Obliczenia

PEC jest obliczany codziennie. Opłaty są opłacone za każdy dzień, w ramach których masz dostęp kwalifikujący się do PEC w każdej subskrypcji. Mimo że szczegóły PEC nie są wyświetlane na fakturze miesięcznej, zarobki PEC są uwzględniane w wierszu skorygowanych opłat netto na fakturze. Więcej szczegółów dotyczących PEC można znaleźć w pliku [dziennego](daily-rated-usage-recon-files.md) użycia i w miesięcznym pliku ponownego rozpoznania faktury.

W poniższej tabeli opisano elementy PEC znalezione w pliku rekonescji faktury miesięcznej. Wszystkie wartości są w USD, jak pokazano w kolumnie AI, PricingCurrency (CenyCurrency).

| Kolumna  | Opis  |
| --------  | -------  |
| Kolumna C  | CustomerName  |
| Kolumna P | UnitPrice |
| Kolumna AD | EffectiveUnitPrice. Jest to cena po zastosowaniu PEC i spełnianiu wymagań. Po zastosowaniu PEC zobaczysz, że wartość EffectiveUnitPrice w kolumnie AD jest procentowo mniejsza niż cena jednostkowa w kolumnie P.   |
| Kolumna V  | PriceAdjustmentDescription. Ta wartość będzie pusta, jeśli nie zostaną spełnione żadne wymagania dotyczące PEC lub % PEC, która zostanie zastosowana do unitPrice. Możesz jednak kwalifikować się do dodatkowych środków. Jeśli tak, zostaną one wymienione w tej kolumnie. Przykład: 100% rabat warstwy 1.   |

Aby monitorować dostęp do PEC:

- **Plik dziennego użycia ocenianego** pokazuje, gdzie PEC jest stosowany (lub nie) codziennie

- [**Alerty usługi Azure Monitor**](azure-plan-manage.md) monitorują zmiany w trwałym dostępie uprzywilejowanym.

## <a name="partner-earned-credit-api"></a>Interfejs API środków uzyskane przez partnerów

Interfejs API PEC jest dostępny w ramach zestawu narzędzi interfejsu API platformy Azure. Aby uzyskać informacje na temat programu PowerShell i interfejsów API interfejsu wiersza polecenia, zobacz [Łączenie konta platformy Azure z identyfikatorem partnera.](/azure/cost-management-billing/manage/link-partner-id)

## <a name="azure-cost-management-and-pec"></a>Azure Cost Management i PEC

Azure Cost Management (ACM) przy użyciu analizy kosztów umożliwia ci, jako partnerowi, wyświetlanie kosztów, które otrzymały korzyść z PEC. Aby uzyskać szczegółową prezentację na temat programu ACM, zobacz wywołanie funkcji W centrum uwagi CSP z maja [2021 r.](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight).

## <a name="use-acm-to-view-your-partner-earned-credit"></a>Wyświetlanie środków zdobytych przez partnera za pomocą programu ACM

1. W [Azure Portal](https://portal.azure.com/)zaloguj się do dzierżawy partnera i wybierz **pozycję Cost Management + Billing**.
2. Wybierz **pozycję Zarządzanie kosztami.**
3. Wybierz **pozycję Analiza kosztów.**
W widoku Analiza kosztów będą wyświetlane koszty dla konta rozliczeniowego dla wszystkich usług zakupionych i zużytych po cenach, które płacisz firmie Microsoft.
4. Na liście rozwijanej wykresu przestawnego wybierz pozycję PartnerEarnedCreditApplied. 

    Jeśli ta wartość ma **wartość True**, skojarzony koszt ma korzyść z środków uzyskane przez partnera.

    Jeśli ta wartość to Fałsz, skojarzony koszt nie spełnił wymaganych uprawnień do środków lub zakupiona usługa nie kwalifikuje się do środków uzyskane przez partnerów.

>[!NOTE]
>Zwykle użycie usług pojawia się w Cost Management 8–24 godzin, a środki PEC pojawią się w ciągu 48 godzin od czasu uzyskania dostępu w Azure Cost Management.

Można również grupować według i filtrować według właściwości **PartnerEarnedCreditApplied** przy użyciu **funkcji** Grupuj według **i** Dodaj filtr. Umożliwiają one przechodzenie do szczegółów kosztów, które mają PEC i koszty, które nie mają zastosowania PEC.

## <a name="how-is-pec-paid"></a>Jak jest opłacana PEC?
Zarobki w ramach PEC są uwzględniane w wierszu skorygowanych opłat netto na fakturze. Aby uzyskać szczegółowe informacje dotyczące korekty, zobacz plik uzgodnień faktury miesięcznej i plik dziennego użycia ocenianego na platformie Azure.

## <a name="next-steps"></a>Następne kroki

- [Cennik nowego środowisko handlowego dla Platforma Azure w programie CSP](azure-plan-price-list.md)
- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure](azure-plan-billing.md)
- [Przywracanie uprawnień administratora dla subskrypcji w ramach programu Azure CSP](revoke-reinstate-csp.md)
- [Środków uzyskane przez partnerów — omówienie](partner-earned-credit.md)
- [Role, uprawnienia do środków uzyskane przez partnerów](azure-roles-perms-pec.md)
- [Informacje o środków uzyskane przez partnerów (przewodnik)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (wymagane logowanie)