---
title: Harmonogramy i procesy wypłaty
description: Dowiedz się więcej o wypłatach i transakcjach, takich jak harmonogramy płatności i procesy ponownego przetwarzania dla platformy handlowej i innych transakcji.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146956"
---
# <a name="payout-schedules-and-processes"></a>Harmonogramy i procesy wypłaty

**Odpowiednie role:** Administrator konta | Administrator globalny

W tym artykule omówiono harmonogram płatności firmy Microsoft, gdzie można znaleźć stan wypłaty oraz proces braku płatności od klienta.

## <a name="payment-schedules"></a>Harmonogramy płatności

W poniższych sekcjach opisano proces wypłat dla **Enterprise Agreement** transakcji **kartą kredytową/fakturą.**

### <a name="enterprise-agreement-transactions"></a>Enterprise Agreement transakcji

Gdy klient zakupi produkt od firmy Microsoft AppSource lub Azure Marketplace przy użyciu istniejącej usługi Microsoft Enterprise Agreement dla transakcji, wystawimy wypłaty w następnym cyklu wypłat 30-dniowym po fakturze klienta. Transakcje, w których klient korzysta z karty kredytowej, mają 30-dniowy okres przechowywania przed wypłatą.

Wypłata często występuje, zanim firma Microsoft zbierze płatność od klienta. Zobacz [Przetwarzanie niepłacenia](#process-for-customer-non-payment) przez klienta poniżej, aby uzyskać informacje o akcjach, które podejmiemy, jeśli klient nie zapłaci firmie Microsoft, ale wystawiliśmy już wypłatę.

| Zdarzenie | Opis | Widoczność raportowania | Chronometraż* |
| --- | --- | --- | --- |
| Użycie lub miesiąc transakcji | Klient używa lub kupuje usługę. | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 1** |
| Firma Microsoft oblicza kwotę rozliczeniowa | Określanie łącznego użycia i łącznej liczby transakcji | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 2** |
| Opublikowana wypłata | Określanie opłat agencyjnych i zarobków wypłat | Oznaczone jako Nieprzetworzone w historii transakcji na [wyciągu z wypłat](payout-statement.md) | **3 miesiąc (1. tydzień)** |
| Przygotowywanie wypłaty | Zarobki są przygotowane do płatności miesięcznych | Oznaczone jako Nadchodzące w historii transakcji w zestawienia [wypłat](payout-statement.md) | **3 miesiąc (1. tydzień)** |
| **Wysłane wypłaty** | **Płatność jest wysyłana do wydawcy** | **Oznaczone jako Wysłane w historii transakcji i w sekcji Płatności zestawienia [wypłat](payout-statement.md)** | **Miesiąc 3 (nie później niż 15)** |
| Faktura zapłacona przez klienta | Firma Microsoft zbiera płatność od klienta | Bez zmian | **Od 4 do 12 miesięcy** |
|

\* Data wypłaty jest w czasie pacyficznym (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Oś czasu płatności dla klientów z umową Enterprise Agreement.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transakcje za pomocą karty kredytowej lub faktury (czek/przelew)

Wszystkie zakupy przy użyciu karty kredytowej lub faktury miesięcznej mają 30-dniowy okres przechowywania, aby upewnić się, że środki są zbierane od klienta.

| Zdarzenie | Opis | Widoczność raportowania | Chronometraż* |
| --- | --- | --- | --- |
| Użycie lub miesiąc transakcji | Klient używa lub kupuje usługę. | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 1** |
| Faktura zapłacona przez klienta | Określanie łącznego użycia, łącznej wartości transakcji i faktury opłacanej przez klienta | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 2** |
| Opublikowana wypłata | Określanie opłat agencyjnych i zarobków w wypłatach | Oznaczone jako Nieprzetworzone w historii transakcji na [wyciągu z wypłat](payout-statement.md) | **Miesiąc 2** |
| 30-dniowy okres przechowywania | Zapewnianie zbierania środków, możliwych opłat zwrotnych i żądań zwrotu pieniędzy | Oznaczone jako Nieprzetworzone w historii transakcji na [wyciągu z wypłat](payout-statement.md) | **Miesiąc 3** |
| Przygotowywanie wypłaty | Zarobki są przygotowane do płatności miesięcznej | Oznaczone jako Upcoming in Transaction History (Nadchodzące w historii transakcji) w [zestawienia wypłat](payout-statement.md) | **4. miesiąc (1. tydzień)** |
| **Wysłane wypłaty** | **Płatność jest wysyłana do wydawcy** | **Oznaczone jako Wysłane w historii transakcji i w sekcji Płatności zestawienia [wypłat](payout-statement.md)** | **Miesiąc 4 (nie później niż 15)** |
|

\* Data wypłaty jest w czasie pacyficznym (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Oś czasu płatności dla klientów kart kredytowych i faktur.":::

## <a name="process-for-customer-non-payment"></a>Proces niepłacący klienta

W rzadkich przypadkach firma Microsoft nie może zbierać płatności od klientów za zakupy na platformie handlowej. Gdy klient nie zapłaci firmie Microsoft zgodnie z harmonogramem rozliczeniowym, rozpoczynamy proces kolekcji. Ten proces trwa około czterech miesięcy i obejmuje trwałą komunikację firmy Microsoft. Jeśli płatność nie zostanie odebrana po zakończeniu tego procesu, firma Microsoft zapisze środki jako niekodowane.

W ramach procesu wypłaty, który został tu sformułowany, firma Microsoft może już zapłacono środki dla wydawców (Ciebie), którzy ostatecznie nie są zbierani. W związku z tym mamy proces uzgadniania tych kwot. Aby upewnić się, że masz ostrzeżenie, że płatność (już odebrana) może zostać uzgodniona, zostaniesz powiadomiona, gdy klient jest w procesie kolekcji, a zakupy prawdopodobnie zostaną zapisane.

Firma Microsoft będzie wycofać wszystkie wypłaty, które zostały ci już opłacone, korzystając z jednej z następujących metod: (1) Firma Microsoft może odjąć niezapłacone kwoty od przyszłych wypłat; Na przykład jeśli wypłaty w wysokości 1000 USD zostaną uznane za niekodowalne i zapisane, przyszłe wypłaty zostaną wstrzymane do momentu odzyskania kwoty 1000 USD lub (2) Firma Microsoft może zażądać zwrotu lub wydawców faktur dla wszelkich nieukońowanych kwot.

Oto przykładowy harmonogram:

| Zdarzenie | Przybliżona data* | Widoczność partnerów |
| --- | --- | --- |
| Przykładowa data wypłaty | 10/15/2020 | Oznaczone jako **wysłane w** historii transakcji i w sekcji Płatności na pulpicie nawigacyjnym wypłat |
| <font color="red">Jeśli klient nie płaci firmie Microsoft</font> | 12/2/2020 – 12/5/2020 | Bez zmian, tak samo jak powyżej |
| Klient otrzymuje pierwszą wiadomość e-mail z opóźnieniem płatności | 12/6/2020 | Brak |
| Klient otrzymuje regularne wiadomości e-mail o rosnącej pilności | 12/7/2020 – 1/31/2021 | Brak |
| Wydawca jest prawdopodobnie powiadamiany o zapisie | 1/7/2021 | Wiadomość e-mail z powiadomieniem wysłanym do wydawcy, że klient jeszcze nie wysłał płatności. Uwzględniane są identyfikator transakcji i kwota w dolarach. |
| Klient otrzymuje powiadomienie o zakończeniu działania | 2/1/2021 | Brak |
| Proces zbierania kończy się/środki są zapisywane | 2/15/2021 | Wiadomość e-mail z powiadomieniem wysłanym do wydawcy, że środki zostały zapisane. Uwzględniane są identyfikator transakcji i kwota w dolarach. |
| Odejmowana jest wypłata | 3/1/2021 | Wydawca zobaczy ujemną transakcję w Partner Center wypłaty |
| Wypłata jest wstrzymana | 3/15/2021 | Przyszłe wypłaty będą wyświetlane w Partner Center wypłat. Wydawca nie otrzyma płatności, dopóki saldo nie będzie ujemne.  |
|||

\* Data wypłaty jest w czasie pacyficznym (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Liczba dni, przez które płatności mają dotrzeć do konta wypłaty

Zwykle wysyłamy wszelkie płatności w danym miesiącu 15 dnia tego miesiąca, ale dotarcie płatności do Twojego konta zajmuje więcej czasu. Liczba dni zależy od formy płatności, która jest stosowana dla Twojego konta, zgodnie z poniższym opisem.

> [!NOTE]
> Poniższe dni są przybliżone. Każda płatność może potrwać więcej lub mniej czasu, aby uzyskać dostęp do konta.

| Metoda płatności     | Liczba dni do osiągnięcia konta wypłaty     |
|--------------------|--------------------------------------------|
| PayPal             | 1 dzień biznesowy                             |
| ACH/SEPA           | 2–3 dni robocze                          |
| Przelew      | 7–10 dni roboczych                         |
|

## <a name="next-steps"></a>Następne kroki

- [Szczegóły podatku](tax-details-marketplace.md)
