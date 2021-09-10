---
title: Uzyskiwanie zapłaty w Centrum partnerskim
description: Dowiedz się więcej o otrzymywaniu płatności za zarobki jako partner firmy Microsoft, na przykład za pośrednictwem ofert platformy handlowej, programów zachęt i programu Dostawca rozwiązań w chmurze platformy handlowej. Obejmuje zasady wypłat, stan wstrzymania wypłaty i zestawienia wypłat.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 07/12/2021
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 99cc0172f9cb1e09bdc77bbd9187ad2452c19c61
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958569"
---
# <a name="getting-paid-in-partner-center"></a>Uzyskiwanie zapłaty w Centrum partnerskim

**Odpowiednie role:** Administrator konta | Administrator globalny

Ten artykuł zawiera ważne informacje na temat otrzymywania płatności za oferty, dodatki i zarobki reklamowe. Zawiera podsumowanie zasad wypłat, kroków wymaganych przed uzyskaniem płatności oraz omówienie zestawienia wypłat.

## <a name="payout-policies-and-agreements"></a>Zasady wypłat i umowy

Uzyskanie płatności wymaga przestrzegania umów i zasad wypłat.

- [Microsoft Azure Marketplace Publisher Agreement:](/legal/marketplace/msft-publisher-agreement)przed uzyskaniem płatności musisz zaakceptować tę umowę wydawcy. W niniejszej umowie wyjaśniono relację między Użytkownikiem a firmą Microsoft w odniesieniu do ofert sprzedawców na platformie handlowej, w tym opłatę za sklep naliczaną przez firmę Microsoft za każdą dokonaną sprzedaż.
- [Zasady wypłat](payout-policy-details.md) pokazują zasady wypłat, w tym harmonogram płatności i formy płatności. Zasady wyjaśniają również proces niewypłacania płatności przez klienta.
- [Szczegóły podatku](tax-details-marketplace.md) objaśniają kwestie podatkowe dotyczące wyboru ceny i odpowiedzialności podatkowej w ramach umowy Microsoft [Publisher Agreement.](/legal/marketplace/msft-publisher-agreement)
- **Opłaty za sklep** są oficjalnie udostępniane w witrynie [Commercial Marketplace Fees (Opłaty za platformę handlową).](/azure/marketplace/marketplace-commercial-transaction-capabilities-and-considerations)
- **Płatności** są dokonywane co miesiąc (pod warunkiem, że został osiągnięty próg płatności). Zwykle wysyłamy wszelkie płatności w danym miesiącu do 15 dnia tego miesiąca. Płatności zwykle docierają do konta wypłat przez 3 do 10 dodatkowych dni roboczych. Aby uzyskać szczegółowe informacje, [zobacz Payment thresholds, methods, and time frames (Progi, metody i ramy czasowe płatności).](payment-thresholds-methods-timeframes.md)

## <a name="prerequisite-steps-before-getting-paid"></a>Kroki wymagań wstępnych przed uzyskaniem zapłaty

Przed uzyskaniem pierwszej płatności musisz skonfigurować konto wypłaty i wypełnić niezbędne formularze bankowe i podatkowe. W formularzach bankowych i podatkowych należy podać preferowane formy płatności i formularze podatkowe dla podatku potrącanego. Formularze bankowe i podatkowe są wymagane, aby można było zapłacić. Aby uzyskać szczegółowe informacje, [zobacz Konfigurowanie konta wypłaty i formularzy podatkowych.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Stan wstrzymania wypłat

Domyślnie będziemy wysyłać płatności co miesiąc, zgodnie z powyższym opisem. Możesz jednak chwycić wypłaty dla programu i firma Microsoft nie będzie zwalniać płatności na Twoim koncie. Jeśli zdecydujesz się chwycić wypłaty, będziemy nadal rejestrować wszelkie zarobki na **stronie Wypłaty.** Jednak nie wyślemy żadnych płatności na Twoje konto, dopóki nie usuniesz wstrzymania.

Aby chwyć płatności, wybierz **ikonę Ustawienia** koła zębatego w prawym górnym rogu, a następnie **pozycję Ustawienia konta.** Wybierz **pozycję Wypłata i** podatek w menu po lewej stronie, a następnie w sekcji **Wypłata** i przypisanie profilu podatkowego znajdź program, dla którego chcesz zatrzymać płatności. Zaznacz pole **wyboru Hold my Payment (Wstrzymaj** moją płatność), aby przechowywać płatności dla tego programu. Stan wstrzymania wypłat można zmienić w dowolnym momencie, ale decyzja będzie mieć wpływ na następną miesięczną wypłatę. Jeśli na przykład chcesz trzymać kwietniowe wypłaty, upewnij się, że stan wstrzymywania wypłaty został ustawiony **na Wł.** przed końcem marca.

Po skonfigurowaniu stanu wstrzymania **wypłaty** na Wł. wszystkie wypłaty dla tego programu będą wstrzymane do momentu wyczyszczenia pola wyboru **na Wyłączone.** Gdy to zrobisz, zostaniesz uwzględniony w następnym miesięcznym cyklu wypłaty (pod warunkiem, że został osiągnięty próg płatności). Jeśli wypłaty zostały wstrzymane, ale chcesz, aby wypłata była generowana w  czerwcu, wyczyść pole wyboru wyłączone przed końcem maja.

>[!Note]
> Stan wstrzymania wypłat ma zastosowanie do każdego programu indywidualnie (Microsoft Store, reklamy, Azure Marketplace i tak dalej). Jeśli chcesz przechowywać płatności dla wszystkich programów, wstrzymaj płatność osobno dla każdego programu.

## <a name="payout-statements"></a>Zestawienia wypłat

Zestawienie wypłat pokazuje zarobki ze sprzedaży z ofert i dodatków w historii transakcji. Możesz również wyświetlać szczegóły płatności i pobierać raporty w formacie TSV lub CSV. Zobacz [Zestawienia wypłat,](payout-statement.md) aby dowiedzieć się więcej na temat uzyskiwania dostępu do zestawienia wypłat oraz szczegółów historii transakcji i raportów płatności. Ponadto możesz używać interfejsu [API wypłat](https://apidocs.microsoft.com/services/partnerpayouts) partnerów do systemowego ściągania raportów o wypłatach.

## <a name="next-steps"></a>Następne kroki

- [Interfejs API wypłat partnerów](https://apidocs.microsoft.com/services/partnerpayouts)
- [Wypłaty — często zadawane pytania](payout-faq.yml)