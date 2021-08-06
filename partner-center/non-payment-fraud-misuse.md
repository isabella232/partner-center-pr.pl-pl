---
title: Zarządzanie brakiem płatnościami, oszustwem lub nieprawidłowym użyciem
description: Dowiedz się więcej o różnych ryzykach związanych z transakcjami online i najlepszych rozwiązaniach dotyczących zarządzania tymi czynnikami i ograniczania ich w Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 54130356ae9388e78affb2e9ff19f54d9f55c64444981a82da1d29ff27fe4d39
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696669"
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

## <a name="theft-of-service-risks"></a>Kradzież ryzyka związanego z usługą

**Kradzież ryzyka związanego** z usługą oznacza, że klienci, którzy nie mają zamiaru płacić za zużyte usługi. Ta kradzież może obejmować użycie skradzionego instrumentu płatniczego, podanie fałszywych informacji rozliczeniowych i/lub niespłacanie zaległych sald.

### <a name="examples-of-service-theft"></a>Przykłady kradzieży usług

Przykłady tych zagrożeń związanych z transakcjami online mogą być następujące:

- Transakcje, które nie występują osobiście ("transakcje z kartą kredytową nie są obecne")
- Błędnie reprezentowane tożsamości
- Usługi aprowowane i używane przed otrzymaniem początkowej płatności
- Nowe rynki i/lub regiony wysokiego ryzyka związane z oszustwem online
- Automatyzowanie tworzenia i kupowania kont przez nieautomatyznych użytkowników

## <a name="managing-online-risk"></a>Zarządzanie ryzykiem w trybie online

Poniższe zalecenia ułatwiają opracowywanie zasad i rozwiązań w celu zmniejszenia narażenia na ryzyko transakcji online w cyklu życia relacji z klientami.

### <a name="onboarding-new-customers"></a>Dołączanie nowych klientów

Sugestie dotyczące zmniejszania ryzyka w trybie online podczas dołączania nowych klientów obejmują:

- Ustanawianie relacji osobistych z klientami, gdy jest to możliwe (na przykład kontaktowanie się z klientami przez telefon).
- Sprawdź poświadczenia i doświadczenie klientów za pomocą lepszych metod (takich jak korzystanie z biur kredytowych lub agencji raporty biznesowe).
- Użyj uwierzytelniania wieloskładnikowego (takiego jak weryfikacja SMS) podczas tworzenia konta, aby zminimalizować ryzyko utworzenia i zakupu konta robotyki.
- Śledzenie tożsamości i zarządzanie nimi przy użyciu usług (takich jak usługi zarządzania tożsamościami cyfrowymi).
- Ocena siły finansowej klienta za pomocą rygorystycznych systemów wykrywania oszustw związanych z kartami kredytowymi.
- Ustanów zasady czystej kolekcji. Szczegóły procesu kolekcji oraz tego, kiedy brak płatności będzie mieć wpływ na dostęp do subskrypcji. (Możesz wyłączyć dostęp lub [wstrzymać subskrypcje klienta w](create-a-new-subscription.md#suspend-a-subscription) przypadku braku płatności).

### <a name="managing-customer-accounts"></a>Managing customer accounts (Zarządzanie kontami klientów)

Sugestie dotyczące zarządzania kontami klientów po zakupie obejmują:

- Implementowanie procesu szybkiego odbierania, przeglądania i reagowania na powiadomienia firmy Microsoft oraz reagowania na nie.
- Pracuj z klientami, aby zrozumieć ich potrzeby biznesowe dotyczące użycia chmury przy odpowiednich progach monitorowania ustawień. (Na przykład możesz ustawić miesięczny budżet wydatków na [platformę Azure w](set-an-azure-spending-budget-for-your-customers.md) Partner Center. Dzięki temu można monitorować użycie klientów w miesiącu i być powiadamiane, gdy klienci zbliżają się do budżetu).
- Regularnie [monitoruj dzienniki aktywności klientów,](activity-logs.md) aby pomóc w wczesnym wykrywaniu oszustw.
- Szybkie działanie w przypadku wykrycia podejrzanych działań.
- Unikaj pełnego dostępu administracyjnego klientów do subskrypcji bez konieczności wcześniejszego implementowania środków zaradczych.

### <a name="managing-customer-billing"></a>Zarządzanie rozliczeniami klientów

Sugestie dotyczące zarządzania rozliczeniami klienta po zakupie obejmują:

- Zażądaj przedpłat przed początkowymi transakcjami i rozliczeniami.
- Nie akceptuj instrumentów płatniczych wysokiego ryzyka (takich jak karty przedpłacone lub karty z przechowywaną wartością).
- Monitoruj płatności klientów i starzejące się należności. Agresywne wymuszanie standardowych procesów dunning w przypadku opóźnionych płatności lub braku płatności.

Aby uzyskać bardziej szczegółowe strategie ograniczania ryzyka w trybie online, zobacz [Przewodnik zarządzania ryzykiem transakcji online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
