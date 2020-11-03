---
title: Zarządzanie niepłatnościami, oszustwem lub nieprawidłowym użyciem
description: Zapoznaj się z różnymi zagrożeniami związanymi z transakcjami online i najlepszymi rozwiązaniami związanymi z zarządzaniem ryzykiem i ich eliminowaniem w centrum partnerskim.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 43a35f91be9ce656157065a3d19b3643ddeff68a
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529814"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Zarządzanie przypadkami braku płatności, oszustw lub nieprawidłowego użycia w centrum partnerskim

Dotyczy:

- Centrum partnerskie
- Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA

**Odpowiednie role**
- Administrator globalny
- Administrator użytkowników
- Agent administracyjny
- Administrator rozliczeń

Użytkownik jest odpowiedzialny za oszukańcze zakupy przez klientów i/lub niepłatę zakupionych usług. W związku z tym *zdecydowanie zalecamy, aby nałożyć kontrolę oszustw i środki zaradcze zapobiegające ryzyku*.

Aby uniknąć sfałszowanych działań lub nieprawidłowego działania, ważne jest zrozumienie potencjalnych zagrożeń i opracowywanie zasad i praktyk, które mogą obniżyć poziom narażenia użytkownika.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Wymuszanie zasad akceptowalnego użycia przez firmę Microsoft

Jeśli firma Microsoft wykryje działania partnerskie lub klienta, które potwierdzają lub podejrzewają, że są naruszane, podejmiemy kroki wymuszania. Klient może zostać natychmiast zawieszony. Użytkownik zostanie powiadomiony o akcjach wymuszania lub zaktualizowanych na żądania przez firmę Microsoft.

## <a name="abuse-of-service-risks"></a>Nadużywanie zagrożeń związanych z usługą

Nadużycie zagrożeń związanych **z usługami** oznacza, że klienci korzystający z usług w chmurze naruszają zasady akceptowalnego użycia przez firmę Microsoft.

### <a name="examples-of-abuse-of-service"></a>Przykłady nadużycia usługi

Przykładami tych naruszeń zasad akceptowalnego użycia przez firmę Microsoft mogą być:

- Spamem
- Działanie hakerskie
- Rozproszone ataki typu "odmowa usługi" (DDoS)
- Bitcoin
- Dystrybucja złośliwego oprogramowania
- Odsprzedaż pirackich subskrypcji

## <a name="theft-of-service-risks"></a>Kradzież zagrożeń związanych z usługami

**Kradzież zagrożeń związanych z usługami** oznacza, że klienci nie mają zamiaru płacenia za wykorzystane usługi. To kradzież może polegać na wykorzystaniu skradzionych instrumentów płatniczych, dostarczeniu fałszywych informacji dotyczących rozliczeń i/lub domyślnych sald.

### <a name="examples-of-service-theft"></a>Przykłady kradzieży usług

Przykładami ryzyka transakcji online mogą być:

- Transakcje, które nie występują w osobie (transakcje nieobecne w karcie kredytowej)
- Niereprezentowane tożsamości
- Usługi obsługiwane i używane przed rozpoczęciem płatności początkowej
- Rozwijające się rynki i/lub regiony wysokiego ryzyka dla oszustw online
- Automatyzowanie tworzenia kont i kupowania ich przez złe aktorów

## <a name="managing-online-risk"></a>Zarządzanie ryzykiem online

Poniższe zalecenia mogą pomóc w opracowaniu zasad i praktyk w celu zmniejszenia ryzyka związanego z transakcją online w cyklu życia relacji z klientami.

### <a name="onboarding-new-customers"></a>Dołączanie nowych klientów

Sugestie dotyczące zmniejszenia ryzyka w trybie online podczas dołączania nowych klientów:

- Jeśli to możliwe, Ustanów relacje osobiste z klientami (na przykład kontaktowanie się z klientami przez telefon).
- Weryfikowanie poświadczeń i tła klientów dzięki lepszym metodom (na przykład w przypadku korzystania z instytucji kredytowych lub komercyjnych agencji sprawozdań handlowych).
- Użyj uwierzytelniania wieloskładnikowego (na przykład weryfikacji SMS) podczas tworzenia konta, aby zminimalizować narażenie na tworzenie i kupowanie kont Robotic.
- Zarządzanie tożsamościami i śledzenie ich przy użyciu usług (takich jak usługi tożsamości cyfrowych).
- Oceń siłę finansową klientów dzięki rygorystycznym systemom wykrywania oszustw związanych z kartą kredytową.
- Ustanów zasady czyszczenia kolekcji. Zastanów się nad procesem tworzenia kolekcji i w przypadku, gdy dostęp do subskrypcji będzie miał wpływ na niepłatność. (Możesz wyłączyć dostęp lub [zawiesić subskrypcje klienta](create-a-new-subscription.md#suspend-a-subscription) dotyczące niepłatności).

### <a name="managing-customer-accounts"></a>Managing customer accounts (Zarządzanie kontami klientów)

Sugestie dotyczące zarządzania kontami klientów po zakupie obejmują:

- Zaimplementuj proces, aby szybko otrzymywać powiadomienia dotyczące firmy Microsoft, przeglądać je, podejmować działania i odpowiadać na nie.
- Pracuj z klientami, aby zrozumieć swoje potrzeby biznesowe dotyczące użycia w chmurze, a następnie ustawienia odpowiednie progi monitorowania. (Na przykład możesz [ustawić miesięczny budżet wydatków na platformę Azure](set-an-azure-spending-budget-for-your-customers.md) w centrum partnerskim. To zrozumienie umożliwia monitorowanie użycia klienta w ciągu miesiąca i otrzymywanie powiadomień o bliskości budżetu przez klientów.
- Regularnie Monitoruj [dzienniki aktywności klientów](activity-logs.md) , aby pomóc w wczesnym wykrywaniu oszustw.
- Wykonaj szybką akcję w przypadku wykrycia podejrzanych działań.
- Należy unikać udzielania klientom pełnego dostępu administracyjnego do subskrypcji bez uprzedniego zaimplementowania kontroli ryzyka.

### <a name="managing-customer-billing"></a>Zarządzanie rozliczeniami klientów

Sugestie dotyczące zarządzania księgowaniem rozliczeń klienta obejmują:

- Zażądaj przedpłaty przed początkowymi transakcjami i rozliczeniami.
- Nie Akceptuj instrumentów płatniczych o wysokim ryzyku (takich jak karty z góry lub karty przechowywane).
- Monitoruj płatności klientów i rozliczenia dla kont przedawnienia. Agresywnie Wymuszaj ustandaryzowane procesy upomnień na potrzeby opóźnień lub braku płatności.

Aby uzyskać bardziej szczegółowe strategie łagodzenia ryzyka w trybie online, zobacz [Przewodnik dotyczący zarządzania ryzykiem online transakcji.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
