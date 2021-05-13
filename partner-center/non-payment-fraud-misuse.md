---
title: Zarządzanie brakiem płatnościami, oszustwem lub nieprawidłowym użyciem
description: Dowiedz się więcej o różnych ryzykach związanych z transakcjami online i najlepszych rozwiązaniach dotyczących zarządzania tymi czynnikami i ograniczania ich w Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 1d8e59ea2d2e8d40163ea06b305845c37a356f16
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818664"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Zarządzanie przypadkami braku płatności, oszustw lub nieprawidłowego użycia w centrum partnerskim

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Administrator rozliczeń

Klient jest odpowiedzialny finansowo za fałszywe zakupy przez klientów i/lub niepłać za zakupione usługi. Dlatego zdecydowanie zalecamy stosowanie środków zaradczych związanych z *zapobieganiem oszustwom i ich wykrywaniem.*

Aby uniknąć i/lub rozwiązać problemy związane z fałszywymi działaniami lub nieprawidłowym użyciem, ważne jest zrozumienie potencjalnych zagrożeń i opracowanie zasad i praktyk, które mogą zmniejszyć narażenie na ryzyko.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Wymuszanie zasad dopuszczalnego użycia przez firmę Microsoft

Jeśli firma Microsoft wykryje działania partnerów lub klientów, które potwierdzimy lub podejrzewamy, naruszają zasady dopuszczalnego użycia, podejmiemy kroki wymuszania. Klient może zostać natychmiast zawieszony. Otrzymasz powiadomienie o działaniach wymuszania lub zaktualizowanych żądaniach firmy Microsoft.

## <a name="abuse-of-service-risks"></a>Nadużycie ryzyka związanego z usługą

**Nadużycie ryzyka związanego** z usługami oznacza, że klienci, którzy korzystają z usług w chmurze, narusza zasady dopuszczalnego użycia firmy Microsoft.

### <a name="examples-of-abuse-of-service"></a>Przykłady nadużycie usługi

Przykłady tych naruszeń zasad dopuszczalnego użycia przez firmę Microsoft mogą obejmować:

- Spamowania
- Hacking
- Rozproszone ataki typu "odmowa usługi" (DDoS)
- Wyszukiwanie bitcoinów
- Dystrybucja złośliwego oprogramowania
- Subskrypcja z 1999 r.

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
- Użyj uwierzytelniania wieloskładnikowego (na przykład weryfikacji SMS) podczas tworzenia konta, aby zminimalizować ryzyko utworzenia i zakupu konta robotyki.
- Śledzenie tożsamości i zarządzanie nimi przy użyciu usług (takich jak usługi tożsamości cyfrowych).
- Oceń siłę finansową klienta za pomocą rygorystycznych systemów wykrywania oszustw związanych z kartami kredytowymi.
- Ustanów zasady czystej kolekcji. Szczegóły procesu kolekcji oraz tego, kiedy brak płatności będzie mieć wpływ na dostęp do subskrypcji. (Możesz wyłączyć dostęp lub [wstrzymać subskrypcje klienta w](create-a-new-subscription.md#suspend-a-subscription) przypadku braku płatności).

### <a name="managing-customer-accounts"></a>Managing customer accounts (Zarządzanie kontami klientów)

Sugestie dotyczące zarządzania kontami klientów po zakupie obejmują:

- Implementowanie procesu szybkiego odbierania, przeglądania i reagowania na powiadomienia firmy Microsoft oraz reagowania na nie.
- Pracuj z klientami, aby zrozumieć ich potrzeby biznesowe dotyczące użycia chmury przy zachowaniu odpowiednich progów monitorowania. (Na przykład możesz ustawić miesięczny budżet wydatków na [platformę Azure w](set-an-azure-spending-budget-for-your-customers.md) Partner Center. Dzięki temu można monitorować użycie klientów w miesiącu i być powiadamiane, gdy klienci zbliżają się do budżetu).
- Regularnie [monitoruj dzienniki aktywności klientów,](activity-logs.md) aby pomóc w wczesnym wykrywaniu oszustw.
- Szybkie działanie w przypadku wykrycia podejrzanych działań.
- Unikaj pełnego dostępu administracyjnego klientów do subskrypcji bez konieczności wcześniejszego implementowania środków zaradczych.

### <a name="managing-customer-billing"></a>Zarządzanie rozliczeniami klientów

Sugestie dotyczące zarządzania rozliczeniami klienta po zakupie obejmują:

- Zażądaj przedpłat przed początkowymi transakcjami i rozliczeniami.
- Nie akceptuj instrumentów płatniczych wysokiego ryzyka (takich jak karty przedpłacone lub karty z przechowywaną wartością).
- Monitoruj płatności klientów i starzejące się należności. Agresywne wymuszanie standardowych procesów dunning w przypadku opóźnionych płatności lub braku płatności.

Aby uzyskać bardziej szczegółowe strategie ograniczania ryzyka w trybie online, zobacz [Przewodnik zarządzania ryzykiem transakcji online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
