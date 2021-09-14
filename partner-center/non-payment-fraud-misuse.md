---
title: Zarządzanie brakiem płatnościami, oszustwem lub nieprawidłowym użyciem
description: Poznaj różne rodzaje ryzyka związane z transakcjami online oraz najlepsze rozwiązania dotyczące zarządzania tymi czynnikami i ograniczania ich w Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: f74a1c091a4c5cd838f8856152c1498f3ecd9d2b
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247473"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Zarządzanie przypadkami braku płatności, oszustw lub nieprawidłowego użycia w centrum partnerskim

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny | Administrator rozliczeń

Ponosisz odpowiedzialność finansową za fałszywe zakupy przez klientów i/lub niepłacące zakupionych usług przez klientów. W związku z tym zdecydowanie zalecamy stosowanie środków zaradczych związanych z *zapobieganiem oszustwom i wykrywaniem.*

Aby uniknąć i/lub rozwiązać problemy związane z fałszywymi działaniami lub nieprawidłowym użyciem, ważne jest zrozumienie potencjalnych zagrożeń i opracowanie zasad i praktyk, które mogą zmniejszyć narażenie na ryzyko.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Wymuszanie zasad dopuszczalnego użycia przez firmę Microsoft

Jeśli firma Microsoft wykryje działania partnerów lub klientów, dla których potwierdzamy lub podejrzewamy, że narusza zasady dopuszczalnego użycia, podejmiemy kroki wymuszania. Klient może zostać natychmiast zawieszony. Otrzymasz powiadomienie o akcjach wymuszania lub zaktualizowanych żądaniach firmy Microsoft.

## <a name="abuse-of-service-risks"></a>Nadużycie ryzyka związanego z usługą

**Nadużycie ryzyka związanego** z usługami oznacza klientów, którzy korzystają z usług w chmurze z naruszeniem zasad dopuszczalnego użycia firmy Microsoft.

### <a name="examples-of-abuse-of-service"></a>Przykłady nadużycie usługi

Przykłady tych naruszeń zasad dopuszczalnego użycia przez firmę Microsoft mogą obejmować:

- Spamowania
- Hacking
- Rozproszone ataki typu "odmowa usługi" (DDoS)
- Wyszukiwanie bitcoinów
- Dystrybucja złośliwego oprogramowania
- Subskrypcja zdjętymi łamiąc

## <a name="theft-of-service-risks"></a>Kradzież zagrożeń związanych z usługami

**Kradzież ryzyka związanego** z usługami oznacza klientów, którzy nie mają zamiaru płacić za zużyte usługi. Ta kradzież może obejmować użycie skradzionych instrumentu płatniczego, podanie fałszywych informacji rozliczeniowych i/lub niespłacanie zaległych sald.

### <a name="examples-of-service-theft"></a>Przykłady kradzieży usług

Przykłady tych zagrożeń związanych z transakcjami online mogą obejmować:

- Transakcje, które nie występują osobiście ("transakcje z kartą kredytową nie są obecne")
- Błędnie reprezentowane tożsamości
- Usługi aprowizowane i używane przed otrzymaniem początkowej płatności
- Nowe rynki i/lub regiony wysokiego ryzyka związane z oszustwami online
- Automatyzowanie tworzenia i kupowania konta przez nieautomatyznych użytkowników

## <a name="managing-online-risk"></a>Zarządzanie ryzykiem w trybie online

Poniższe zalecenia ułatwiają opracowywanie zasad i praktyk w celu zmniejszenia narażenia na ryzyko związane z transakcjami online w cyklu życia relacji z klientami.

### <a name="onboarding-new-customers"></a>Dołączanie nowych klientów

Sugestie dotyczące zmniejszania ryzyka w trybie online podczas dołączania nowych klientów obejmują:

- Ustanawianie relacji osobistych z klientami, gdy jest to możliwe (na przykład kontaktowanie się z klientami przez telefon).
- Sprawdź poświadczenia i doświadczenie klientów za pomocą lepszych metod (takich jak korzystanie z biur kredytowych lub komercyjnych agencji raportów biznesowych).
- Użyj uwierzytelniania wieloskładnikowego (takiego jak weryfikacja SMS) podczas tworzenia konta, aby zminimalizować ryzyko utworzenia i zakupu konta robotyki.
- Śledzenie tożsamości i zarządzanie nimi przy użyciu usług (takich jak usługi tożsamości cyfrowych).
- Oceń siłę finansową klienta za pomocą rygorystycznych systemów wykrywania oszustw związanych z kartami kredytowymi.
- Ustanów zasady czystej kolekcji. Szczegóły procesu kolekcji oraz informacje o tym, kiedy brak płatności będzie mieć wpływ na dostęp do subskrypcji. (Możesz wyłączyć dostęp lub wstrzymać [subskrypcje](create-a-new-subscription.md#suspend-a-subscription) klienta w przypadku braku płatności).

### <a name="managing-customer-accounts"></a>Managing customer accounts (Zarządzanie kontami klientów)

Sugestie dotyczące zarządzania kontami klientów po zakupie obejmują:

- Implementowanie procesu szybkiego odbierania, przeglądania i reagowania na powiadomienia firmy Microsoft oraz reagowania na nie.
- Współpracowanie z klientami w celu zrozumienia ich potrzeb biznesowych dotyczących użycia chmury przy użyciu odpowiednich progów monitorowania ustawień. (Na przykład można ustawić miesięczny budżet wydatków [na platformę Azure w](set-an-azure-spending-budget-for-your-customers.md) Partner Center. Ta wiedza pozwala monitorować użycie klientów w miesiącu i być powiadamiana, gdy klienci zbliżają się do budżetu).
- Regularnie [monitoruj dzienniki aktywności klientów,](activity-logs.md) aby pomóc w wczesnym wykrywaniu oszustw.
- Szybkie działanie w przypadku wykrycia podejrzanych działań.
- Unikaj pełnego dostępu administracyjnego klientów do subskrypcji bez konieczności wcześniejszego implementowania środków zaradczych.

### <a name="managing-customer-billing"></a>Zarządzanie rozliczeniami klientów

Sugestie dotyczące zarządzania rozliczeniami klienta po zakupie obejmują:

- Zażądaj przedpłat przed początkowymi transakcjami i rozliczeniami.
- Nie akceptuj instrumentów płatniczych wysokiego ryzyka (takich jak karty z płatnościami wstępnymi lub karty z przechowywaną wartością).
- Monitorowanie płatności klientów i przedawniających się kont. Agresywne wymuszanie standardowych procesów monitowania w przypadku opóźnionych płatności lub braku płatności.

Aby uzyskać bardziej szczegółowe strategie ograniczania ryzyka w trybie online, zobacz Przewodnik zarządzania ryzykiem [transakcji online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
