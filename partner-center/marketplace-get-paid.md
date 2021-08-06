---
title: Uzyskiwanie zapłaty w Centrum partnerskim
description: Dowiedz się więcej o otrzymywaniu płatności za zarobki jako partner firmy Microsoft, na przykład za pośrednictwem ofert platformy handlowej, programów zachęt i programu Dostawca rozwiązań w chmurze platformy handlowej. Obejmuje zasady wypłat, stan wstrzymania wypłaty i zestawienia wypłat.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 07/12/2021
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: bc1a9eb3c0fde48a589d57ab40671791244c20cfa028ccae5de3cf5ee6a322ed
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697282"
---
# <a name="getting-paid-in-partner-center"></a>Uzyskiwanie zapłaty w Centrum partnerskim

**Odpowiednie role:** Administrator konta | Administrator globalny

Ten artykuł zawiera ważne informacje dotyczące otrzymywania płatności za oferty, dodatki i zarobki reklamowe. Zawiera podsumowanie zasad wypłat, kroków wymaganych przed uzyskaniem płatności oraz omówienie zestawienia wypłat.

## <a name="payout-policies-and-agreements"></a>Zasady i umowy dotyczące wypłat

Uzyskanie płatności wymaga przestrzegania umów i zasad wypłat.

- [Microsoft Azure Marketplace Publisher Agreement:](/legal/marketplace/msft-publisher-agreement)przed uzyskaniem płatności musisz zaakceptować tę umowę wydawcy. Ta umowa wyjaśnia relację między To użytkownikiem a firmą Microsoft w odniesieniu do ofert sprzedawców na platformie handlowej, w tym opłatę za sklep naliczaną przez firmę Microsoft za każdą dokonaną sprzedaż.
- [Zasady wypłat](payout-policy-details.md) pokazują zasady płatności dotyczące wypłat, w tym harmonogram płatności i formy płatności. Zasady wyjaśniają również proces niepłacenia przez klienta.
- [Szczegóły podatku](tax-details-marketplace.md) objaśniają kwestie podatkowe dotyczące wyboru cen i odpowiedzialności podatkowej w ramach umowy Microsoft [Publisher Agreement.](/legal/marketplace/msft-publisher-agreement)
- **Opłaty za sklep** są oficjalnie udostępniane w witrynie Commercial Marketplace Fees ( [Opłaty za platformę handlową).](/azure/marketplace/marketplace-commercial-transaction-capabilities-and-considerations)
- **Płatności** są dokonywane co miesiąc (pod warunkiem, że próg płatności został osiągnięty). Zwykle wysyłamy wszelkie płatności w danym miesiącu do 15 dnia tego miesiąca. Aby uzyskać dostęp do konta wypłaty, płatności zwykle trwa od 3 do 10 dodatkowych dni roboczych. Aby uzyskać szczegółowe informacje, zobacz [Progi płatności, metody i ramy czasowe](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Kroki wymagań wstępnych przed uzyskaniem zapłaty

Przed uzyskaniem pierwszej płatności musisz skonfigurować konto wypłaty i wypełnić niezbędne formularze bankowe i podatkowe. W formularzach bankowych i podatkowych należy podać preferowane formy płatności i formularze podatkowe dotyczące podatku potrącanego. Formularze bankowe i podatkowe są wymagane, aby można było zapłacić. Aby uzyskać szczegółowe informacje, [zobacz Konfigurowanie konta wypłaty i formularzy podatkowych.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Stan wstrzymania wypłat

Domyślnie będziemy wysyłać płatności co miesiąc, zgodnie z powyższym opisem. Możesz jednak chwycić wypłaty dla programu, a firma Microsoft nie będzie zwalniać Twoich płatności na Twoje konto. Jeśli zdecydujesz się trzymać wypłaty, będziemy nadal rejestrować wszelkie zarobki na **stronie Wypłaty.** Jednak nie wyślemy żadnych płatności na Twoje konto, dopóki nie usuniesz wstrzymania.

Aby trzymać płatności, wybierz **ikonę koła Ustawienia** w prawym górnym rogu, a następnie **pozycję Ustawienia konta.** Wybierz **pozycję Wypłata i** podatek w menu po lewej stronie, a następnie w sekcji **Wypłata** i przypisanie profilu podatkowego znajdź program, dla którego chcesz zatrzymać płatności. Zaznacz pole **wyboru Hold my Payment (Przytrzymaj** moją płatność), aby przechowywać płatności dla tego programu. Stan wstrzymania wypłaty można zmienić w dowolnym momencie, ale decyzja będzie mieć wpływ na następną miesięczną wypłatę. Jeśli na przykład chcesz trzymać kwietniowe wypłaty, upewnij się, że stan wstrzymywania wypłaty został ustawiony na **Wł.** przed końcem marca.

Po skonfigurowaniu stanu wstrzymania wypłaty na Wł. wszystkie wypłaty dla tego programu będą wstrzymane do momentu wyczyszczenia pola wyboru na **Wyłączone.**  Gdy to zrobisz, zostaniesz uwzględniony w następnym miesięcznym cyklu wypłaty (pod warunkiem, że próg płatności został osiągnięty). Jeśli wypłaty zostały wstrzymane, ale chcesz, aby wypłata była generowana w czerwcu, wyczyść pole wyboru na **Wyłączone** przed końcem maja.

>[!Note]
> Stan wstrzymania wypłaty ma zastosowanie do każdego programu indywidualnie (Microsoft Store, reklam, Azure Marketplace itd.). Jeśli chcesz przechowywać płatności dla wszystkich programów, wstrzymaj płatność dla każdego programu osobno.

## <a name="payout-statements"></a>Zestawienia wypłat

Zestawienie wypłat pokazuje zarobki ze sprzedaży z ofert i dodatków w historii transakcji. Możesz również wyświetlać szczegóły płatności i pobierać raporty w formacie TSV lub CSV. Zobacz [Zestawienia wypłat,](payout-statement.md) aby dowiedzieć się więcej na temat sposobu uzyskiwania dostępu do zestawienia wypłat oraz szczegółów historii transakcji i raportów płatności. Ponadto możesz użyć interfejsu API wypłat [partnerów,](https://apidocs.microsoft.com/services/partnerpayouts) aby systemowo ściągać raporty o wypłatach.

## <a name="next-steps"></a>Następne kroki

- [Interfejs API wypłat partnerów](https://apidocs.microsoft.com/services/partnerpayouts)
- [Wypłaty — często zadawane pytania](payout-faq.yml)