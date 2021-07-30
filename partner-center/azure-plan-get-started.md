---
title: Rozpoczynanie przechodzenia do planu platformy Azure
description: Dowiedz się, co Ty i Twoi klienci powinni wiedzieć o używaniu planu płatności zgodnie z potrzebami platformy Azure, w tym o pierwszych krokach, zabezpieczeniach i instrukcje dotyczące rozpoczynania pracy.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 40bf84ed47c946b84f511693d9f8351b3ffa5a95
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841661"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Rozpoczynanie korzystania ze stawek płatności zgodnie z użyciem w planie platformy Azure

**Odpowiednie role:** Agent administracyjny | Agent sprzedaży


Firma Microsoft wprowadziła nowe środowisko handlowe w Partner Center.  Dzięki nowej wersji handlowej partnerzy uzyskają dostęp do usług platformy Azure według stawek płatności zgodnie z Umowa z Klientem Microsoft.

Ten plan upraszcza proces zakupu — w planie platformy Azure można mieć wiele subskrypcji platformy Azure. Nie musisz już przesyłać oddzielnego zamówienia na subskrypcję platformy Azure. W tym nowym doświadczeniu handlowym dla platformy Azure dostosliśmy się do jednej globalnej zasady cenowej, dzięki czemu partnerzy programu CSP mogą oferować platformę Azure po opublikowanych cenach.

Potrzeby naszych klientów w zakresie transformacji cyfrowej wymagają nowych umiejętności od partnerów. Wielu klientów poszuka partnerów w celu zapewnienia usług wykraczających poza transakcję, aby ich podróż w chmurze była bardziej bezproblemowa i pomagała w wydajnym chmurze. Partnerzy firmy Microsoft odgrywają kluczową rolę na wszystkich etapach cyklu życia klienta. Tego rodzaju usługi partnerskie są w trakcie realizacji i obejmują monitorowanie majątku na platformie Azure, zarządzanie zasadami i ładem, konfigurowanie dostrajania, pomoc techniczną i wiele innych usług. Wymagają oni, aby partner dokładnie znał środowisko platformy Azure klienta oraz miał ciągłe i odpowiednie zarządzanie oraz kontrolę nad bazowymi zasobami, którym zarządza. Partnerzy rozliczeniowi, którzy zapewniają to 24 x 7 rozwiązań do zarządzania operacjami w chmurze, będą uprawnieni do otrzymania środków uzyskane przez partnerów na usługi zarządzane **na** tę pracę.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Upewnij się, że klienci podpisali Umowa z Klientem Microsoft

Od 1 października 2019 r. dostępna jest umowa Umowa z Klientem Microsoft, która upraszcza i usprawnia proces zakupów klientów w pełni cyfrowym. Wszyscy klienci, którzy chcą korzystać z nowego rozwiązania handlowego w programie CSP dla platformy Azure, muszą podpisać umowę Umowa z Klientem Microsoft.

Partnerzy, którzy chcą dokonać transakcji w ramach nowego planu platformy Azure i złożyć nowe zamówienie, powinni potwierdzić akceptację klientów Umowa z Klientem Microsoft użyciu pulpitu nawigacyjnego Partner Center i interfejsu API w środowisku produkcyjnym.

Od 1 lutego 2020 r. istniejące Umowa dotycząca platformy Microsoft Cloud zostaną usunięte z programu CSP. Od tego czasu potwierdzenie przez partnera (potwierdzenie) akceptacji przez klienta dla nowego Umowa z Klientem Microsoft będzie wymagane dla wszystkich innych ofert, w tym Microsoft 365, Dynamics 365 i istniejącej platformy Azure. Partnerzy w programie CSP nie będą mogli złożyć nowego zamówienia dla klienta bez zaświadczenia Umowa z Klientem Microsoft.

Aby uzyskać szczegółowe informacje, przeczytaj [Potwierdzanie akceptacji przez klienta Umowa z Klientem Microsoft](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Rozwiązania dotyczące zabezpieczeń i kontroli dostępu

Aby ułatwić ochronę partnerów i klientów, wprowadzamy zestaw obowiązkowych wymagań dotyczących zabezpieczeń dla doradców, dostawców Panel sterowania i partnerów biorących udział w programie Dostawca rozwiązań w chmurze zabezpieczeń.

Partnerzy, którzy nie implementują obowiązkowych wymagań dotyczących zabezpieczeń, nie będą mogli wykonać transakcji w programie Dostawca rozwiązań w chmurze ani zarządzać dzierżawami klientów, korzystając z delegowanych praw administratora, po wymuszenia tych wymagań. Jesteśmy w trakcie ustalania technicznej daty wymuszania wymagań i powiadomimy partnerów o dacie przy użyciu szczegółowych informacji.

## <a name="actions-to-take-to-implement-mfa"></a>Akcje do wykonania w celu zaimplementowania usługi MFA

Biorąc pod uwagę wysoce uprzywilejowany charakter partnera, musimy upewnić się, że każdy użytkownik ma zadanie uwierzytelniania wieloskładnikowego dla każdego pojedynczego uwierzytelniania. Można to zrobić za pomocą jednego z następujących sposobów:

- Implementowanie Azure AD — wersja Premium i upewnianie się, że uwierzytelnianie wieloskładnikowe (MFA) jest wymuszane dla każdego użytkownika
- Implementowanie ustawień [domyślnych zabezpieczeń usługi Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementowanie rozwiązania innej firmy i upewnianie się, że uwierzytelniania wieloskładnikowego jest wymuszane dla każdego użytkownika

Od 1 sierpnia 2019 r. wszyscy partnerzy muszą wymuszać uwierzytelnianie wieloskładnikowe dla wszystkich użytkowników, w tym kont usług, w dzierżawie partnera. Szczegółowe informacje na temat tych wymagań dotyczących zabezpieczeń można znaleźć na stronie [Partner security requirements (Wymagania dotyczące zabezpieczeń partnerów).](partner-security-requirements.md)

Firma Microsoft zaleca partnerom korzystanie z kontroli RBAC zgodnie z najlepszymi rozwiązaniami dostępnymi za [pośrednictwem Azure Active Directory Privileged Identity Management zasobów.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="read-more-about-the-azure-plan"></a>Przeczytaj więcej na temat planu platformy Azure

- [Kupowanie planu platformy Azure](purchase-azure-plan.md)

- [Porównanie ofert platformy Azure](compare-azure-offers.md)

- [Punkty uzyskane przez partnerów — omówienie](partner-earned-credit.md)

- Obliczenia środków uzyskane przez partnerów oraz role i uprawnienia, które kwalifikują się do otrzymania środków uzyskane przez partnera, są dostępne w cenniku pulpitu nawigacyjnego platformy Partner Center (wymagane jest zalogowanie się).

## <a name="next-steps"></a>Następne kroki 

- [Jak są określane punkty uzyskane przez partnera — szczegóły](partner-earned-credit-explanation.md)
- [Objaśniono cennik planu platformy Azure](azure-plan-price-list.md)
- [Przenoszenie klienta do planu platformy Azure](azure-plan-transition.md)
- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Pełna lista krajów/regionów, w których jest dostępny plan platformy Azure](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)