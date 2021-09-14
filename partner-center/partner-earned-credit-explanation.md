---
title: Środków uzyskane przez partnerów na usługi zarządzane
ms.topic: article
ms.date: 08/12/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak są obliczane i opłacane punkty uzyskane przez partnerów firmy Microsoft dla usług zarządzanych oraz jak upewnić się, że masz odpowiednie uprawnienia.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3583614b1bf89a3c9297f123f12355b8a2ad7d1e
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246778"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Jak są obliczane i wypłacane środki zarobione przez partnera

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Administrator rozliczeń | Agent sprzedaży

Punkty uzyskane przez partnerów dla usług zarządzanych rozpoznaje i nagradza partnerów, którzy są właścicielami kontroli operacyjnej IT i zarządzania środowiskiem platformy Azure niektórych lub wszystkich klientów. 

Domyślnie jako partner CSP masz przyznane niezbędne prawa dostępu do subskrypcji klienta, co pozwala na wykonywanie zarządzania operacyjnego i kontrolowania zasobów w ramach subskrypcji. Inne sposoby, w jakie klienci mogą aprowizują dostęp dla partnerów transakcji, opisano w poniższej sekcji.

Kwota faktury miesięcznej jest netto środków uzyskanej przez partnera. Szczegóły dotyczące PEC można zobaczyć w miesięcznym pliku rekonescji. Aby uzyskać dodatkowe informacje o sposobach, w jakie klient może aprowizuje dostęp dla partnera transakcji, zobacz następujące artykuły:

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Przywracanie uprawnień administratora dla subskrypcji w ramach programu Azure CSP](/revoke-reinstate-csp.md)

## <a name="eligibility"></a>Kwalifikowalności

Aby otrzymać punkty uzyskane przez partnera, obowiązują następujące wymagania:

- Musisz mieć aktywną umowę MPN i prawidłową rolę kontroli dostępu [na podstawie](azure-roles-perms-pec.md) ról [(RBAC).](/azure/role-based-access-control/overview)
- Musisz mieć uprawnienia [Admin on Behalf of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) w subskrypcji platformy Azure klienta, grupie zasobów platformy Azure lub zasobie platformy Azure albo prawidłowej [roli RBAC.](azure-roles-perms-pec.md)
- W przypadku dostawców pośrednich i ich odsprzedawców pośrednich dostawca pośredni kwalifikuje się do PEC, jeśli dostawca pośredni lub odsprzedawca pośredni albo obaj mają uprawnienia AOBO lub kwalifikującą się rolę RBAC. Aby uzyskać więcej informacji, zobacz [Przywróć uprawnienia](revoke-reinstate-csp.md)administratora dla Azure CSP subskrypcji.
- Identyfikator MPN partnera musi należeć do tej samej organizacji wirtualnej co identyfikator MPN nabywcy lub identyfikator MPN partnera rekordów. Aby uzyskać więcej informacji, zobacz [Łączenie identyfikatora partnera w celu śledzenia wpływu na delegowane zasoby](/azure/lighthouse/how-to/partner-earned-credit).
- PEC jest zdobywany na poziomie zasobów platformy Azure, grupie zasobów lub subskrypcji. Jeśli partner ma prawidłowy dostęp na poziomie subskrypcji lub grupy zasobów, każdy zasób, który jest zbiorczy dla wyższej jednostki, będzie zdobywać PEC.
- PEC nie ma zastosowania do następujących usług:
    - Rezerwacje planów platformy Azure
    - Produkty innych firm zidentyfikowane jako produkty innych firm w kolumnie Tagi ceny za zużycie planu platformy Azure
    - Produkty w cenniku witryny Marketplace
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

Oprócz powyższych wymagań PEC ma zastosowanie tylko do usług wymienionych w cenniku użycia planu platformy Azure. Możesz je wyświetlić i wyeksportować na stronie [cennika planu platformy Azure.](https://partner.microsoft.com/commerce/sales)

Aby uzyskać więcej informacji na temat PEC, zobacz [stronę Azure Cost Management.](/azure/cost-management-billing/costs/get-started-partners)

Aby uzyskać więcej informacji na temat uprawnień, zobacz Role i uprawnienia wymagane do [zdobywania środków zdobytych przez partnera.](azure-roles-perms-pec.md)

## <a name="calculation"></a>Obliczenia

PEC jest obliczany codziennie. Opłaty są opłacone za każdy dzień, w ramach których masz dostęp kwalifikujący się do PEC w każdej subskrypcji. Chociaż szczegóły PEC nie są wyświetlane na fakturze miesięcznej, zarobki PEC są uwzględniane w wierszu skorygowanych opłat netto na fakturze. Więcej szczegółów dotyczących PEC można znaleźć w pliku [dziennego użycia](daily-rated-usage-recon-files.md) i w pliku ponownego rozpoznania faktury miesięcznej.

:::image type="content" source="images/advanced-specializations/recon-file.png" alt-text="Zrzut ekranu przedstawiający Partner Center pliku uzgodnień identyfikującego kolumny." border="false":::

W poniższej tabeli opisano elementy PEC znalezione w pliku ponownego rozpoznania faktury miesięcznej. Wszystkie wartości są podane w USD, jak pokazano w kolumnie AI, PricingCurrency (AI, CennikCurrency).

| Kolumna  | Opis  |
| --------  | -------  |
| Kolumna C  | CustomerName  |
| Kolumna P | UnitPrice |
| Kolumna AD | EffectiveUnitPrice. Jest to cena po zastosowaniu PEC i spełnianiu wymagań. Po zastosowaniu PEC zobaczysz, że cena EffectiveUnitPrice w kolumnie AD jest procentowo mniejsza niż cena jednostkowa w kolumnie P.   |
| Kolumna V  | PriceAdjustmentDescription. Ta wartość będzie pusta, jeśli nie zostaną spełnione żadne wymagania dotyczące PEC lub % PEC, która zostanie zastosowana do cena jednostkowa. Możesz jednak kwalifikować się do dodatkowych środków. Jeśli tak, będą one wyświetlane w tej kolumnie. Przykład: 100% rabat warstwy 1.   |

Aby monitorować dostęp do PEC:

- **Plik dziennego użycia ocenianego** pokazuje, gdzie PEC jest stosowany (lub nie) codziennie

- [**Alerty usługi Azure Monitor**](azure-plan-manage.md) monitorują zmiany w trwałym dostępie uprzywilejowanym.

Plik dziennego użycia ocenianego:

:::image type="content" source="images/advanced-specializations/partner-daily.png" alt-text="Zrzut ekranu przedstawiający Partner Center dziennego użycia z wyróżnieniami efektywnej ceny jednostkowej." border="false":::

## <a name="partner-earned-credit-api"></a>Interfejs API środków uzyskane przez partnerów

Interfejs API PEC jest dostępny w ramach zestawu narzędzi interfejsu API platformy Azure. Aby uzyskać informacje na temat programu PowerShell i interfejsów API interfejsu wiersza polecenia, zobacz [Łączenie konta platformy Azure z identyfikatorem partnera.](/azure/cost-management-billing/manage/link-partner-id)

## <a name="azure-cost-management-and-pec"></a>Azure Cost Management i PEC

Azure Cost Management (ACM) przy użyciu analizy kosztów umożliwia wyświetlanie jako partnerowi kosztów, które otrzymały korzyść z PEC. Aby uzyskać szczegółową prezentację na temat programu ACM, zobacz wywołanie funkcji W centrum uwagi CSP z maja [2021 r.](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight).

## <a name="use-acm-to-view-your-partner-earned-credit"></a>Wyświetlanie środków uzyskane przez partnera za pomocą programu ACM

1. W [Azure Portal](https://portal.azure.com/)zaloguj się do dzierżawy partnera i wybierz pozycję **Cost Management + Billing**.
2. Wybierz **pozycję Zarządzanie kosztami.**
3. Wybierz **pozycję Analiza kosztów.**
W widoku Analiza kosztów będą wyświetlane koszty dla konta rozliczeniowego dla wszystkich usług zakupionych i zużytych po cenach, które płacisz firmie Microsoft.

:::image type="content" source="images/advanced-specializations/partner-cost.png" alt-text="Zrzut ekranu przedstawiający stronę analizy kosztów zarządzania kosztami." border="false":::

4. Na liście rozwijanej wykresu przestawnego wybierz pozycję PartnerEarnedCreditApplied. 

    Jeśli ta wartość to **True**, skojarzony koszt ma korzyść z środków uzyskane przez partnera.

    Jeśli ta wartość to **False,** skojarzony koszt nie spełnił wymaganych uprawnień do środków lub zakupiona usługa nie kwalifikuje się do środków uzyskane przez partnerów.

>[!NOTE]
>Zazwyczaj czas użycia usług w programie Cost Management wynosi 8–24 godziny, a środki PEC pojawią się w ciągu 48 godzin od czasu uzyskania dostępu w Azure Cost Management.

Można również grupować i filtrować według właściwości **PartnerEarnedCreditApplied** przy użyciu funkcji Grupuj według **i** **Dodaj** filtr. Umożliwiają one przechodzenie do szczegółów kosztów z pec i kosztów, które nie mają zastosowania PEC.

## <a name="how-is-pec-paid"></a>Jak jest opłacana PEC?
Zarobki w ramach PEC są uwzględniane w wierszu skorygowanych opłat netto na fakturze. Ilustruje **to** suma faktury pokazanej poniżej. Aby uzyskać szczegółowe informacje dotyczące korekty, zobacz plik uzgodnień faktury miesięcznej i plik dziennego użycia ocenianego na platformie Azure.

:::image type="content" source="images/advanced-specializations/invoice.png" alt-text="Zrzut ekranu przedstawiający fakturę Partner Center z informacją, że szczegóły korekty są wyświetlane w plikach ponownego użycia i dziennym użyciu platformy Azure." border="false":::

## <a name="next-steps"></a>Następne kroki

- [Cennik nowego środowisko handlowego dla Platforma Azure w programie CSP](azure-plan-price-list.md)
- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure](azure-plan-billing.md)
- [Przywracanie uprawnień administratora dla subskrypcji w ramach programu Azure CSP](revoke-reinstate-csp.md)
- [Punkty uzyskane przez partnerów — omówienie](partner-earned-credit.md)
- [Role, uprawnienia do środków uzyskane przez partnerów](azure-roles-perms-pec.md)
- [Informacje o środków uzyskane przez partnerów (przewodnik)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (wymagane logowanie)