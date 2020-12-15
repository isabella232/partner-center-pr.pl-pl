---
title: Uzyskiwanie płatności w centrum partnerskim
description: Dowiedz się więcej o otrzymywaniu płatności za zyski jako partner firmy Microsoft, na przykład za pomocą ofert komercyjnych, programów zachęt i programu Cloud Solution Provider. Obejmuje zasady wypłat, wypłaty i wypłaty.
ms.service: marketplace
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: fc1eea0d8a90bb2b5e11dad24a71c9c34fd1a4a0
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492453"
---
# <a name="getting-paid-in-partner-center"></a>Uzyskiwanie płatności w centrum partnerskim

**Odpowiednie role:**

- Administrator konta
- Administrator globalny

Ten artykuł zawiera ważne informacje dotyczące otrzymywania płatności za oferty, dodatki i dochody reklamowe. Zawiera podsumowanie zasad wypłaty, kroki wymagane przed uzyskaniem płatnych informacji oraz przegląd instrukcji wypłaty.

## <a name="payout-policies-and-agreements"></a>Zasady wypłaty i umowy

Po otrzymaniu płatności wymagane jest przestrzeganie zasad umów i wypłat.

- [Microsoft Azure Marketplace umowa wydawcy](https://go.microsoft.com/fwlink/p/?LinkID=699560): przed zapłaceniem musisz zaakceptować tę umowę wydawcy. Niniejsza Umowa wyjaśnia relacje między ty i firmą Microsoft w odniesieniu do ofert sprzedających w komercyjnej witrynie Marketplace, w tym opłatami za sklep, które są naliczane za każdą sprzedaż.
- [Zasady](payout-policy-details.md) wypłaty przedstawiają zasady płatności, w tym harmonogram płatności i formy płatności. W zasadach opisano również proces niepłatności dla klientów.
- [Szczegóły podatkowe](tax-details-marketplace.md) wyjaśniają nacisk na wybór cen i odpowiedzialność za podatek zgodnie z [umową wydawcy](https://go.microsoft.com/fwlink/p/?LinkID=699560)firmy Microsoft.
- **Opłaty za Sklep** są oficjalnie zdefiniowane w Umowie wydawcy. Opłata za Sklep jest stosowana do całej sprzedaży oferowanej przez komercyjną witrynę Marketplace, w tym dodatków.
- **Płatności** są dokonywane miesięcznie (pod warunkiem spełnienia progu płatności). Zwykle wysyłamy wszelkie płatności należne w danym miesiącu do 15 dnia danego miesiąca. Płatności zwykle przejęcia od 3 do 10 dodatkowych dni roboczych w celu uzyskania dostępu do konta wypłaty. Aby uzyskać szczegółowe informacje, zobacz [progi płatności, metody i klatki czasowe](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Kroki wymagań wstępnych przed uzyskaniem płatności

Przed zapłaceniem po raz pierwszy należy skonfigurować konto wypłaty i uzupełnić niezbędne formularze bankowe i podatkowe. W formularzach bankowych i skarbowych będziesz podawać preferowane metody płatności i formularze podatkowe dla potrącania podatku. W celu skorzystania z formularza Bank i podatku są wymagane. Aby uzyskać szczegółowe informacje, zobacz [Konfigurowanie konta wypłaty i formularzy podatkowych](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Stan wstrzymania

Domyślnie będziemy wysyłać płatności miesięcznie, zgodnie z powyższym opisem. Istnieje jednak możliwość nadania wypłaty dla programu w trakcie wstrzymania, a firma Microsoft nie wystawia płatności na Twoje konto. Jeśli zdecydujesz się na wstrzymanie wypłatów, będziemy nadal rejestrować wszelkie dochody na stronie **wypłaty** . Nie będziemy jednak wysyłać żadnych płatności do konta do momentu usunięcia blokady.

Aby wstrzymać płatności, wybierz **ikonę koła zębatego w prawym** górnym rogu, a następnie pozycję **Ustawienia konta**. W menu po lewej stronie wybierz pozycję **wypłata i podatek** , a następnie w sekcji **przypisanie i przypisywanie profilów podatkowych** Znajdź program, dla którego chcesz mieć płatności. Zaznacz pole wyboru **przechowuj moją płatność** , aby wstrzymać płatności za ten program. W każdej chwili możesz zmienić status wypłaty, ale decyzja wpłynie na następną wypłatę miesięczną. Na przykład jeśli chcesz wstrzymać wypłatę z kwietnia, pamiętaj, aby przed końcem marca ustawić stan wstrzymania na wartość **włączone** .

Po ustawieniu **na** wartość wypłaty stan Wstrzymaj wszystkie wypłaty dla tego programu będą przechowywane do momentu wyczyszczenia pola **wyboru.** Po wykonaniu tej czynności zostanie uwzględniony w następnym cyklu miesięcznej wypłaty (w przypadku spełnienia progu płatności). Jeśli Twoje wypłaty zostały wstrzymane, ale chcesz wystawić wypłatę w czerwcu, wyczyść to pole wyboru, aby **wyłączyć** przed końcem maja.

>[!Note]
> Status wypłaty ma zastosowanie do każdego programu osobno (Microsoft Store, reklamy, Azure Marketplace itd.). Jeśli chcesz wstrzymać płatności za wszystkie programy, zaczekaj na każdy program osobno.

## <a name="payout-statements"></a>Zestawienia wypłat

W zestawieniu wypłaty przedstawiono zyski ze sprzedaży z ofert i dodatków w historii transakcji. Możesz również wyświetlić szczegóły płatności i pobrać raporty w formacie TSV lub CSV. Zobacz [instrukcje wypłaty](payout-statement.md) , aby dowiedzieć się więcej o tym, jak uzyskać dostęp do instrukcji wypłaty i szczegółowych informacji o historii transakcji i raportach dotyczących płatności. Ponadto można użyć [interfejsu API wypłaty partnerów](https://apidocs.microsoft.com/services/partnerpayouts) do systematycznego ściągania raportów wypłat.

## <a name="next-steps"></a>Następne kroki

- [Interfejs API wypłat partnerów](https://apidocs.microsoft.com/services/partnerpayouts)
- [Wypłaty — często zadawane pytania](payout-faq.md)
