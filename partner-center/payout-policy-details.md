---
title: Harmonogramy i procesy wypłaty
description: Dowiedz się więcej o wypłatach i transakcjach, takich jak harmonogramy płatności i procesy ponownego Azure Marketplace i innych transakcji.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: 417421ad51c30d067ce3eb2189534a391b2951a2
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958605"
---
# <a name="payout-schedules-and-processes"></a>Harmonogramy i procesy wypłaty

**Odpowiednie role:** Administrator konta | Administrator globalny

W tym artykule omówiono harmonogram płatności firmy Microsoft, gdzie można znaleźć stan wypłaty oraz proces braku płatności dla klienta.

## <a name="payment-schedules"></a>Harmonogramy płatności

W poniższych sekcjach opisano proces wypłat dla **Enterprise Agreement** i Umowa z Klientem Microsoft **lub CSP.**

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Transakcje, gdy klient ma Enterprise Agreement

Gdy klient zakupi produkt od firmy Microsoft AppSource lub Azure Marketplace przy użyciu istniejącej usługi Microsoft Enterprise Agreement dla transakcji, wystawimy wypłaty w następnym cyklu wypłat 30-dniowym po fakturze od klienta. Transakcje, w których klient korzysta z karty kredytowej, mają 30-dniowy okres przechowywania przed wypłatą.

Wypłata często występuje, zanim firma Microsoft zbierze płatność od klienta. Zobacz [przetwarzanie w przypadku braku](#process-for-customer-non-payment) płatności dla klienta poniżej, aby uzyskać informacje o akcjach, które podejmiemy, jeśli klient nie zapłaci firmie Microsoft, ale wystawiliśmy już wypłatę.

| Zdarzenie | Opis | Widoczność raportowania | Chronometraż* |
| --- | --- | --- | --- |
| Użycie lub miesiąc transakcji | Klient używa lub kupuje usługę. | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 1** |
| Firma Microsoft oblicza kwotę rozliczeniowa | Określanie łącznego użycia i łącznej liczby transakcji | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 2** |
| Opublikowana wypłata | Określanie opłat agencyjnych i zarobków w wypłatach | Oznaczone jako Nieprzetworzone w historii transakcji na [wyciągu z wypłat](payout-statement.md) | **3 miesiąc (1. tydzień)** |
| Przygotowywanie wypłaty | Zarobki są przygotowane do płatności miesięcznej | Oznaczone jako Upcoming in Transaction History (Nadchodzące w historii transakcji) w [zestawienia wypłat](payout-statement.md) | **3 miesiąc (1. tydzień)** |
| **Wysłane wypłaty** | **Płatność jest wysyłana do wydawcy** | **Oznaczone jako wysłane w historii transakcji i w sekcji Płatności zestawienia [wypłat](payout-statement.md)** | **3 miesiąc (nie później niż 15. miesiąc)** |
| Faktura zapłacona przez klienta | Firma Microsoft zbiera płatność od klienta | Bez zmian | **Od 4 do 12 miesięcy** |
|

\* Data wypłaty jest w czasie pacyficznym (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Oś czasu płatności dla klientów z umową Enterprise Agreement.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Transakcje, gdy klient ma Umowa z Klientem Microsoft lub CSP

Wszystkie zakupy przy użyciu karty kredytowej lub faktury miesięcznej mają 30-dniowy okres przechowywania, aby upewnić się, że środki są zbierane od klienta.

| Zdarzenie | Opis | Widoczność raportowania | Chronometraż* |
| --- | --- | --- | --- |
| Użycie lub miesiąc transakcji | Klient używa lub kupuje usługę. | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 1** |
| Faktura zapłacona przez klienta | Określanie łącznego użycia, łącznej wartości transakcji i faktury opłacanej przez klienta | [Pulpit nawigacyjny](/azure/marketplace/partner-center-portal/usage-dashboard) użycia [lub](/azure/marketplace/partner-center-portal/orders-dashboard) zamówienia | **Miesiąc 2** |
| Opublikowana wypłata | Określanie opłat agencyjnych i zarobków w wypłatach | Oznaczone jako Nieprzetworzone w historii transakcji na [wyciągu z wypłat](payout-statement.md) | **Miesiąc 2** |
| 30-dniowy okres przechowywania | Zapewnianie zbierania środków, możliwych opłat zwrotnych i żądań zwrotu pieniędzy | Oznaczone jako Nieprzetworzone w historii transakcji na [wyciągu z wypłat](payout-statement.md) | **Miesiąc 3** |
| Przygotowywanie wypłaty | Zarobki są przygotowane do płatności miesięcznej | Oznaczone jako Upcoming in Transaction History (Nadchodzące w historii transakcji) w [zestawienia wypłat](payout-statement.md) | **4 miesiąc (1. tydzień)** |
| **Wysłane wypłaty** | **Płatność jest wysyłana do wydawcy** | **Oznaczone jako wysłane w historii transakcji i w sekcji Płatności zestawienia [wypłat](payout-statement.md)** | **4. miesiąc (nie później niż 15. miesiąc)** |
|

\* Data wypłaty jest w czasie pacyficznym (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Oś czasu płatności dla klientów korzystających z kart kredytowych i faktur.":::

## <a name="process-for-customer-non-payment"></a>Proces braku płatności przez klienta

W rzadkich przypadkach firma Microsoft nie może zbierać płatności od klientów za zakupy na platformie handlowej. Gdy klient nie płaci firmie Microsoft zgodnie z harmonogramem rozliczeniowym, rozpoczynamy proces kolekcji. Ten proces trwa około czterech miesięcy i obejmuje trwałą komunikację z firmą Microsoft. Jeśli płatność nie zostanie odebrana po zakończeniu tego procesu, firma Microsoft zapisze środki jako niekodowalne.

W ramach procesu wypłaty, który został tu sformułowany, firma Microsoft może już zapłacić wydawcom (Ty) środki, które są ostatecznie nie do odzywania. W związku z tym mamy proces uzgadniania tych kwot.

Firma Microsoft będzie wycofać wszelkie wypłaty, które zostały ci już zapłacone, przy użyciu jednej z następujących metod: (1) Firma Microsoft może odjąć niezapłacone kwoty od przyszłych wypłat; Na przykład jeśli 1000 USD w wypłatach zostanie uznane za niekodowalne i zapisane, przyszłe wypłaty zostaną wstrzymane do momentu odzyskania 1000 USD lub (2) firma Microsoft może zażądać zwrotu lub wydawców faktur dla wszelkich nieukońowanych kwot.

Oto przykładowy harmonogram:

| Zdarzenie | Przybliżona data* | Widoczność partnerów |
| --- | --- | --- |
| Przykładowa data wypłaty | 10/15/2020 | Oznaczone jako **wysłane w** historii transakcji i w sekcji Płatności na pulpicie nawigacyjnym wypłat |
| <font color="red">Jeśli klient nie płaci firmie Microsoft</font> | 12/2/2020 – 12/5/2020 | Bez zmian, tak jak powyżej |
| Klient otrzymuje pierwszą wiadomość e-mail z opóźnieniem płatności | 12/6/2020 | Brak |
| Klient otrzymuje regularne wiadomości e-mail o rosnącej pilności | 12/7/2020 – 1/31/2021 | Brak |
| Publisher jest prawdopodobnie powiadamiany o zapisie | 1/7/2021 | - |
| Klient otrzymuje powiadomienie o zakończeniu działania | 2/1/2021 | Brak |
| Proces zbierania kończy się/środki są zapisywane | 2/15/2021 | Wysyłane do wydawcy powiadomienie e-mail o tym, że środki zostały zapisane. |
| Odejmowana jest wypłata | 3/1/2021 | Publisher będzie ujemna transakcja w Partner Center wypłaty |
| Wypłata jest wstrzymana | 3/15/2021 | Przyszłe wypłaty będą wyświetlane w Partner Center wypłat. Publisher nie otrzyma płatności, dopóki saldo nie będzie już ujemne.  |
|||

\* Data wypłaty jest w czasie pacyficznym (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Liczba dni, przez które płatności mają uzyskać dostęp do konta wypłaty

Zwykle wysyłamy wszelkie płatności w danym miesiącu w dniu 15 dnia tego miesiąca, ale dotarcie płatności do Twojego konta zajmuje więcej czasu. Liczba dni zależy od formy płatności, która jest stosowana dla Twojego konta, zgodnie z poniższym opisem.

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
