---
title: Wypłata często zadawane pytania dotyczące komercyjnej witryny Marketplace firmy Microsoft
description: Uzyskaj odpowiedzi na często zadawane pytania dotyczące wypłat na rynku komercyjnym. Zawiera odpowiedzi na to, dlaczego dochody są inne niż oczekiwano.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: 44bd7f488e3d4e79c45cb2746c7e2a6da449a310
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530573"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Często zadawane pytania dotyczące komercyjnych wypłat rynkowych

W tym artykule znajdują się odpowiedzi na często zadawane pytania dotyczące wypłat w portalu komercyjnym.

## <a name="earnings-incorrect-or-missing"></a>Brak lub nieprawidłowe zarobki

#### <a name="why-are-my-earnings-missing"></a>Dlaczego brakuje moich zarobków?

- Być może zamówienie klienta nie kwalifikuje się jeszcze do wypłaty. W przypadku zamówień od klientów niekorporacyjnych firma Microsoft musi otrzymać płatność od klienta, zanim zarobki wydawcy zostaną zakwalifikowane. W przypadku zamówień od klientów korporacyjnych zarobki będą dostępne od 1 do 2 dni po dacie zamówienia zakupu. Sprawdź stan zamówienia w obszarze [Raporty zamówień](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Zarobki z tytułu transakcji sprzed lipca 2019 r. mogą nie być widoczne w raporcie historii transakcji. Możesz sprawdzić historyczne zestawienia w obszarze [Pobieranie wypłat](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Sprawdź [przedział czasu cyklu wypłaty](payment-thresholds-methods-timeframes.md) i zapoznaj się z tematem, kiedy zarobki powinny być widoczne w zestawieniu wypłaty.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Dlaczego kwota zarobków różni się od oczekiwanej?

- Jeśli zamówienie zostało częściowo opłacone przez klienta, kwota zarobków będzie obliczana na podstawie częściowo płatnej kwoty po potrąceniu Opłaty i odpowiednich podatków.
- Sprawdź odpowiedzialność za obowiązek naliczania podatku według kraju. W przypadku krajów, w których za odprowadzanie podatków odpowiada firma Microsoft, będzie ona pobierać i odliczać kwoty podatków z zarobków wydawcy. Kwota transakcji wskazana w zestawieniu jest pomniejszona o podatek. Zobacz [Szczegóły podatków](tax-details-marketplace.md).
- Oferty SaaS i IaaS mają rabat w wysokości 10% zamiast standardowego 20%, pozostawiając stawkę zarobkową wynoszącą 90% czasu. Ta promocja obowiązuje do 30 czerwca 2021 r.

**Dalsze** informacje: [komercyjna umowa dotycząca wydawcy w portalu Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Szczegóły zasad wypłaty](payout-policy-details.md) [,](tax-details-marketplace.md) [próg płatności, Metoda i ramy czasowe](payment-thresholds-methods-timeframes.md), [otrzymywanie płatności na rynku komercyjnym](marketplace-get-paid.md) [Payout statements](payout-statement.md) [Orders dashboard in commercial marketplace analytics](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Uzgadnianie zarobków
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Jak mogę uzgodnić zestawienia wypłat z raportami analizy dotyczącymi zamówień lub użycia?
Użyj AssetID, IDZamówienia i ID elementu, który pojawia się w raporcie Historia transakcji wypłaty przy użyciu zamówień analitycznych i raportów użycia. Użyj tego mapowania:

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Jak mogę określić, kiedy mam oczekiwać płatności za zamówienia klientów?
- Najpierw za pomocą assetID Sprawdź pozycję zamówienia klienta w [raportach o zamówieniach](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Sprawdź kanał klienta dla subskrypcji klienta w [raporcie Customers](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- W przypadku klientów korporacyjnych dochody wydawcy są wyświetlane w instrukcji 1-2 dni po dacie zamówienia zakupu.
- W przypadku klientów nienależących do przedsiębiorstwa dochody z tytułu wydawców pojawiają się w zestawie 1-2 dni po otrzymaniu płatności przez klienta.

**Dalsze odczytywanie** : [instrukcje wypłaty](payout-statement.md), [pulpit nawigacyjny zamówień w komercyjnej analizie Marketplace](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Zasady wypłat

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Jak mogę znaleźć bieżącą stawkę agencyjną i stawkę wypłaty?

- Zapoznaj się z umową wydawcy dotyczącą komercyjnej platformy handlowej. Standardowa stawka agencyjna wynosi 20%. SaaS Co-Sell kwalifikujące się transakcje mają rabat w wysokości 10%. Sprawdź ogłoszenia dotyczące promocyjnych stawek agencyjnych.
- W zestawieniu wypłaty wskaźnik dochodów określa rzeczywistą stawkę wypłaty dla danej transakcji.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Kiedy mogę oczekiwać płatności od firmy Microsoft po pojawieniu się zarobków w zestawieniu?
- Gdy zarobki mają stan „nieprzetworzone”, możesz sprawdzić termin zapadalności, aby określić miesiąc, w którym zarobki zostaną przetworzone na potrzeby płatności. Gdy płatność zostanie przygotowana, stan zdobywania zostanie zmieniony na "przetworzony".  Firma Microsoft zwalnia płatności do 15. dnia miesiąca, w którym przypada termin zapadalności.
- W przypadku zamówień płatnych według karty kredytowej firma Microsoft przechowuje płatności przez 30 dni do momentu zakończenia okresu zdobywania.

 **Dalsze** informacje: [komercyjna umowa dotycząca wydawcy w portalu Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Szczegóły zasad wypłaty](payout-policy-details.md), [szczegóły podatku](tax-details-marketplace.md), [próg płatności, Metoda i przedział czasu](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Płatności i korekty

#### <a name="why-is-my-payment-missing"></a>Dlaczego brakuje mojej płatności?

- Upewnij się, że stan wypłaty i stan profilu podatkowego są wyświetlane jako *prawidłowe* na [stronie Przegląd](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Być może nie osiągnięto minimalnego progu na potrzeby płatności. Aby otrzymać płatność, zarobki muszą wynosić co najmniej 50 USD.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Jak mogę ustawić moje konto, aby nie otrzymywać płatności?
Płatności można przechowywać w [profilu wypłaty](https://partner.microsoft.com/dashboard/commercial-marketplace/overview). po prostu **zaczekaj** . Firma Microsoft będzie utrzymywać płatność do momentu zwolnienia wstrzymania.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Dlaczego otrzymuję płatność w innej walucie niż waluta zakupu?

Waluta wypłaty zależy od waluty wybranej w profilu wypłat. Waluta zakupu to waluta, w której klient zrealizował płatność.

#### <a name="how-do-i-reconcile-adjustments"></a>Jak mogę uzgodnić korekty?

Korekty płatności mają na celu wyrównanie kwot płatności, na przykład w związku z problemami systemowymi. W zestawieniu wypłat przyczynę korekty określa parametr ReasonCode. Nie jest przewidywane bezpośrednie uzgodnienie z poszczególnymi transakcjami.

**Dalsze** informacje: [komercyjna umowa dotycząca wydawcy w portalu Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Szczegóły zasad wypłaty](payout-policy-details.md), [szczegóły podatku](tax-details-marketplace.md), [próg płatności, Metoda i przedział czasu](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Podatki

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Jak określamy odpowiedzialność za odprowadzanie podatków (po stronie firmy Microsoft lub Wydawcy) na zestawieniu wypłat?

W pobranym pliku historii transakcji znajdź kolumnę Tax model (Model podatkowy). Zawiera ona wartość MS Managed (Zarządzane przez firmę Microsoft) lub ISV Managed (Zarządzane przez niezależnego dostawce oprogramowania). Zapoznaj się z regułami podatkowymi właściwymi dla poszczególnych krajów i ich wpływem na wypłaty w temacie [Szczegóły podatków](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Jak mogę pobrać formularze dotyczące podatku z tytułu opłaty za usługę?

Przejdź do strony **Wypłaty — Płatności** i zobacz sekcję **Lista płatności** . Jeśli płatność jest objęta podatkiem z tytułu opłaty za usługę, będzie widoczny link do formularza podatkowego.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Jak mogę pobrać formularz dotyczący podatku potrąconego w formacie PDF?

Przejdź do strony *Wypłaty — Płatności* i zobacz sekcję **Lista płatności** . Obok płatności będzie widoczny link do formularza dotyczącego podatku potrąconego.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Gdzie mogę znaleźć formularze dotyczące rozliczenia rocznego podatku?

Przejdź do [strony profilu](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage), aby wyświetlić formularze dotyczące rozliczenia rocznego podatku.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Jak mogę znaleźć podatek potrącony dla określonej transakcji?
Podatkiem potrąconym objęci są wydawcy z USA, którzy złożyli formularz W-9. Podatek potrącony jest obliczany na podstawie płatności miesięcznych.

**Dalsze** informacje: [komercyjna umowa dotycząca wydawcy w portalu Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Szczegóły zasad wypłaty](payout-policy-details.md)

## <a name="payout-statement-access"></a>Dostęp do instrukcji wypłaty

#### <a name="how-do-i-access-a-payout-statement"></a>Jak mogę uzyskać dostęp do zestawienia wypłat?

1. Sprawdź swoje role. Aby uzyskać dostęp do zestawienia wypłat, musisz mieć rolę *współpracownika ds. finansowych* lub *właściciela konta* .
2. W prawym górnym rogu wybierz ikonę **wypłaty** , aby wyświetlić instrukcję wypłaty. Wybierz między **historią transakcji** , **płatnością** i **pobieraniem** .

**Dalsze odczytywanie** : [wypłaty ról i uprawnień](payout-statement.md#roles-and-permissions), [instrukcje wypłaty](payout-statement.md) 

## <a name="payout-statement-report"></a>Raport zestawienia wypłaty

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Co oznaczają poszczególne pola w pobranym pliku transakcji?

Zobacz [instrukcje wypłaty](payout-statement.md) , aby zapoznać się ze szczegółową listą atrybutów i ich znaczenia.

#### <a name="what-is-earning-status"></a>Co to jest stan zarobków?

Spowoduje to wyświetlenie zarobków jako nieprzetworzonych, przetwarzanych lub wysłanych.

- **Nieprzetworzony** — zarobki są w okresie płatności do momentu zakończenia.
- **Przetworzone** — dochody są dojrzałe i przygotowywane do miesięcznej płatności. Płatności są uwalniane 15. każdego miesiąca.
- **Wysłano** — płatność została pomyślnie wydana do Twojego banku w oparciu o profil wypłaty.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Jak mogę pobrać formularze dotyczące podatku z tytułu opłaty za usługę?

Przejdź do strony **Wypłaty — Płatności** i zobacz sekcję **Lista płatności** . Jeśli płatność jest objęta podatkiem z tytułu opłaty za usługę, będzie widoczny link do formularza podatkowego.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Jak mogę pobrać formularza potrąconej zaliczki w formacie PDF?

Przejdź do strony **Wypłaty — Płatności** i zobacz sekcję **Lista płatności** . Obok płatności będzie widoczny link do formularza dotyczącego podatku potrąconego.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Gdzie mogę znaleźć formularze dotyczące rozliczenia rocznego podatku?

Przejdź do [strony profilu](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage), aby wyświetlić formularze dotyczące rozliczenia rocznego podatku.

**Dalsze odczytywanie** : [instrukcje wypłaty](payout-statement.md), [Pobieranie historii transakcji](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Historyczne instrukcje

#### <a name="how-do-i-view-historical-information"></a>Jak mogę wyświetlić informacje historyczne?

Zestawienie historyczne zawiera migawkę danych dotyczących wypłat od października 2019 r. Niestety informacje o wypłatach nie są odświeżane w tym miejscu. Aby uzyskać najnowsze informacje, Prześlij bilet pomocy technicznej w celu uzyskania najnowszych danych.

**Dalsze odczytywanie** : [instrukcje wypłaty](payout-statement.md), [Pobieranie historii transakcji](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Interfejs API eksportu wypłaty

#### <a name="how-do-i-download-payout-data"></a>Jak mogę pobrać dane wypłat?

Użyj [interfejsu API wypłaty partnerów](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Następne kroki

- [Uzyskiwanie zapłaty na komercyjnej platformie handlowej](marketplace-get-paid.md)
