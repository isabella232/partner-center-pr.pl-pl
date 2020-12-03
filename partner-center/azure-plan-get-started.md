---
title: Rozpocznij przenoszenie do planu platformy Azure
description: Dowiedz się, co ci i czego potrzebują, aby dowiedzieć się więcej o korzystaniu z planu "płatność zgodnie z rzeczywistym użyciem" platformy Azure, w tym pierwszych kroków, środków bezpieczeństwa i sposobach rozpoczęcia pracy.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: fcf75acef4afb80c5aec889911ffc2b4a53b6edd
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534917"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Zacznij korzystać z stawek płatność zgodnie z rzeczywistym użyciem z planem platformy Azure

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży


Firma Microsoft wprowadziła nowe środowisko handlowe w centrum partnerskim.  Dzięki temu nowemu środowisku handlowym partnerzy będą uzyskiwać dostęp do usług platformy Azure w ramach stawek płatność zgodnie z rzeczywistym użyciem dla klientów w ramach umowy klienta firmy Microsoft.

Ten plan upraszcza proces zakupów — w planie platformy Azure można mieć wiele subskrypcji platformy Azure. Nie musisz już przesyłać oddzielnej kolejności na subskrypcję platformy Azure. W tym nowym środowisku handlowym dla platformy Azure została wyrównana do jednej zasady globalnego cennika, co umożliwia partnerom programu CSP oferowanie platformy Azure pod kątem opublikowanych cen.

Wymagania dotyczące transformacji cyfrowych naszych klientów wymagają nowych umiejętności od partnerów. Wielu klientów szuka partnerów w celu świadczenia usług powyżej i wykraczających poza transakcję, aby zapewnić płynność podróży w chmurze i wydajnie korzystać z usług platformy Azure. Partnerzy firmy Microsoft odgrywają kluczową rolę na wszystkich etapach cyklu życia klienta. Te rodzaje usług partnerskich są w sposób ciągły i obejmują monitorowanie, zasady i zarządzanie usługami platformy Azure, Konfigurowanie i Konfigurowanie precyzyjnego dostrajania, pomoc techniczną i różne inne usługi. Wymagają one, aby partner dokładnie się ze środowiskiem platformy Azure klienta i mieć ciągłe i właściwe zarządzanie i kontrolę nad zasobami, którymi zarządzają. Partnerzy rozliczeń, którzy zapewnią tę 24 X 7 operacji w chmurze, będą uprawnieni do uzyskania środków na korzystanie z **usług zarządzanych przez partnerów** .

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Upewnij się, że klienci zostali podpisali umowę klienta firmy Microsoft

Od 1 października 2019 umowa dla klientów firmy Microsoft, umowa bezterminowa, która upraszcza i usprawnia korzystanie z zakupów klientów w ramach pełnego procesu cyfrowego, jest dostępna. Wszyscy klienci, którzy chcą korzystać z nowego środowiska handlowego w programie CSP dla systemu Azure, muszą podpisać umowę klienta firmy Microsoft.

Partnerzy, którzy chcą korzystać z nowego planu platformy Azure i tworzą nowe zamówienie, muszą potwierdzić akceptację umowy licencyjnej klienta firmy Microsoft przy użyciu pulpitu nawigacyjnego Centrum partnerskiego i interfejsu API w środowisku produkcyjnym.

Od 1 lutego 2020, istniejąca umowa Microsoft Cloud zostanie usunięta z programu CSP. Od tego czasu potwierdzenie partnera (zaświadczanie) o akceptacji przez klienta dla nowej umowy klienta firmy Microsoft będzie wymagane dla wszystkich innych ofert, w tym Microsoft 365, Dynamics 365 i istniejącej platformy Azure. Partnerzy w dostawcy usług kryptograficznych nie będą mogli utworzyć nowego zamówienia dla klienta bez zaświadczania umowy klienta firmy Microsoft.

Aby uzyskać szczegółowe informacje, przeczytaj artykuł [potwierdzenie akceptacji klienta umowy klienta firmy Microsoft](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Zasady zabezpieczeń i kontroli dostępu

Aby pomóc w zabezpieczeniu partnerów i klientów, wprowadzamy zestaw obowiązkowych wymagań w zakresie zabezpieczeń dla doradców, dostawców panelu sterowania i partnerów uczestniczących w programie dostawcy rozwiązań w chmurze.

Partnerzy, którzy nie implementują obowiązkowych wymagań w zakresie zabezpieczeń, nie będą mogli wykonywać operacji Transact w programie dostawcy rozwiązań w chmurze ani zarządzać dzierżawami klientów, korzystając z delegowania praw administratora, gdy te wymagania są wymuszane. Jesteśmy w trakcie ustanawiania technicznego okresu wymuszania wymagań i będą powiadamiać partnerów o dacie z szczegółowymi informacjami.

## <a name="actions-to-take-to-implement-mfa"></a>Akcje podejmowane w celu zaimplementowania usługi MFA

Mając wysoce uprzywilejowany charakter partnera, musimy upewnić się, że każdy użytkownik ma wyzwanie usługi MFA dla każdego pojedynczego uwierzytelniania. Można to osiągnąć za pomocą jednej z następujących metod:

- Implementowanie Azure AD — wersja Premium i zapewnianie, że uwierzytelnianie wieloskładnikowe (MFA) jest wymuszane dla każdego użytkownika
- Implementowanie [domyślnych ustawień zabezpieczeń usługi Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementowanie rozwiązania innych firm i zapewnienie, że uwierzytelnianie wieloskładnikowe jest wymuszane dla każdego użytkownika

Od 1 sierpnia 2019 wszyscy partnerzy muszą wymusić uwierzytelnianie wieloskładnikowe dla wszystkich użytkowników, w tym kont usług, w dzierżawie partnera. Szczegółowe informacje o tych wymaganiach dotyczących zabezpieczeń znajdują się w [wymaganiach dotyczących zabezpieczeń partnerów](partner-security-requirements.md).

Firma Microsoft zaleca partnerom korzystanie z pracujemy RBAC, zgodnie z najlepszymi rozwiązaniami, które zostały włączone za pomocą [zasobów Azure Active Directory Privileged Identity Management](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>Przeczytaj więcej na temat planu platformy Azure

- [Kupowanie planu platformy Azure](purchase-azure-plan.md)

- [Porównanie ofert platformy Azure](compare-azure-offers.md)

- [Kredyt wypracowany przez partnera — przegląd](partner-earned-credit.md)

- Obliczenia związane z kredytem uzyskanym przez partnera (PEC) oraz role i uprawnienia kwalifikujące się do uzyskania kredytów uzyskanych przez partnerów są dostępne na liście cenowej pulpitu nawigacyjnego Centrum partnerskiego (wymagane jest zalogowanie się).

## <a name="next-steps"></a>Następne kroki 

- [Jak jest określony kredyt uzyskany przez partnera — szczegóły](partner-earned-credit-explanation.md)
- [Objaśniono listę cen planu platformy Azure](azure-plan-price-list.md)
- [Przenoszenie klienta do planu platformy Azure](azure-plan-transition.md)
- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Pełna lista krajów/regionów, w których jest dostępny plan platformy Azure](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)