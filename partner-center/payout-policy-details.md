---
title: Harmonogramy i procesy wypłaty
description: Zapoznaj się z wypłatami i transakcjami, takimi jak harmonogramy płatności i procesy odliczeń dla komercyjnych rynków i innych transakcji.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: 09e1301cb106c9e1ed40ff1fb6f70da92d2695ee
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861414"
---
# <a name="payout-schedules-and-processes"></a>Harmonogramy i procesy wypłaty

**Odpowiednie role:**

- Administrator konta
- Administrator globalny

W tym artykule omówiono harmonogram płatności firmy Microsoft, gdzie można znaleźć status wypłaty, a następnie proces niepłaty dla klienta.

## <a name="payment-schedules"></a>Harmonogramy płatności

W poniższych sekcjach opisano nasz proces wypłats dotyczący transakcji dotyczących **Enterprise Agreement** i **karty kredytowej/faktury** .

### <a name="enterprise-agreement-transactions"></a>Enterprise Agreement transakcji

Gdy klient kupuje produkt z Microsoft AppSource lub Azure Marketplace przy użyciu istniejących w firmie Microsoft Enterprise Agreement dla transakcji, będziemy wystawić wypłaty w następnym cyklu wypłaty w okresie 30 dni. Transakcje, w których klient używa karty kredytowej, ma 30-dniowy okres przechowywania przed wypłatą.

Wypłata często nastąpi, zanim firma Microsoft będzie zbierać płatność od klienta. Zapoznaj się z artykułem [dotyczącym niepłatności klienta](#process-for-customer-non-payment) w przypadku akcji podejmowanych w przypadku niepowodzenia płatności przez klienta firmy Microsoft, ale wystawiłeś już wypłatę.

| Zdarzenie | Opis | Widoczność raportów | Terminy |
| --- | --- | --- | --- |
| Użycie lub miesiąc transakcji | Klient korzysta z usługi lub kupuje ją. | Pulpit nawigacyjny [użycia](/azure/marketplace/partner-center-portal/usage-dashboard) lub [zamówienia](/azure/marketplace/partner-center-portal/orders-dashboard) | **Miesiąc 1** |
| Firma Microsoft oblicza kwotę rozliczeń | Określanie łącznego użycia, łącznej liczby transakcji | Pulpit nawigacyjny [użycia](/azure/marketplace/partner-center-portal/usage-dashboard) lub [zamówienia](/azure/marketplace/partner-center-portal/orders-dashboard) | **Miesiąc 2** |
| Faktura zapłacona przez klienta | Firma Microsoft zbiera płatność od klienta | Bez zmian | **Miesiąc 2** |
| Opublikowano wypłaty | Ustalanie opłat za Agencję i dochodów z wypłaty | Oznaczono jako nieprzetworzony w historii transakcji w [instrukcji wypłaty](payout-statement.md) | **Miesiąc 3 (pierwszy tydzień)** |
| Przygotuj wypłatę | Dochody są przygotowywane do miesięcznej płatności | Oznaczone jako nadchodzące w historii transakcji w [instrukcji wypłaty](payout-statement.md) | **Miesiąc 3 (pierwszy tydzień)** |
| **Wysłane wypłaty** | **Płatność jest wysyłana do wydawcy** | **Oznaczone jako wysłane w historii transakcji i w sekcji płatności [instrukcji wypłaty](payout-statement.md)** | **Miesiąc 3 (nie później niż 15)** |
| Faktura zapłacona przez klienta | Firma Microsoft zbiera płatność od klienta | Bez zmian | **Miesiąc od 4 do 12** |
|

\* Data wypłaty przypada w czasie standardowym (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Oś czasu płatności dla klientów z umową Enterprise Agreement.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transakcje z kartą kredytową lub fakturą (test/przewód)

Wszystkie zakupy z kartą kredytową lub fakturą miesięczną mają 30-dniowy okres przechowywania, dzięki czemu fundusze są zbierane od klienta.

| Zdarzenie | Opis | Widoczność raportów | Terminy |
| --- | --- | --- | --- |
| Użycie lub miesiąc transakcji | Klient korzysta z usługi lub kupuje ją. | Pulpit nawigacyjny [użycia](/azure/marketplace/partner-center-portal/usage-dashboard) lub [zamówienia](/azure/marketplace/partner-center-portal/orders-dashboard) | **Miesiąc 1** |
| Faktura zapłacona przez klienta | Określanie łącznego użycia, całkowitej wartości transakcji i faktury płatnej klienta | Pulpit nawigacyjny [użycia](/azure/marketplace/partner-center-portal/usage-dashboard) lub [zamówienia](/azure/marketplace/partner-center-portal/orders-dashboard) | **Miesiąc 2** |
| Opublikowano wypłaty | Ustalanie opłat za Agencję i dochodów z wypłaty | Oznaczono jako nieprzetworzony w historii transakcji w [instrukcji wypłaty](payout-statement.md) | **Miesiąc 2** |
| 30-dniowy okres przechowywania | Upewnij się, że zebrano środki, możliwe obciążeń zwrotnych i zwrotne żądania | Oznaczono jako nieprzetworzony w historii transakcji w [instrukcji wypłaty](payout-statement.md) | **Miesiąc 3** |
| Przygotuj wypłatę | Dochody są przygotowywane do miesięcznej płatności | Oznaczone jako nadchodzące w historii transakcji w [instrukcji wypłaty](payout-statement.md) | **Miesiąc 4 (pierwszy tydzień)** |
| **Wysłane wypłaty** | **Płatność jest wysyłana do wydawcy** | **Oznaczone jako wysłane w historii transakcji i w sekcji płatności [instrukcji wypłaty](payout-statement.md)** | **Miesiąc 4 (nie później niż 15)** |
|

\* Data wypłaty przypada w pacyficznym czasie standardowym (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Oś czasu płatności dla kart kredytowych i klientów faktury.":::

## <a name="process-for-customer-non-payment"></a>Proces dla niepłaty klienta

W rzadkich przypadkach firma Microsoft nie jest w stanie zebrać płatności od klientów na potrzeby zakupów w portalu Marketplace. Gdy klient nie może uregulować firmy Microsoft zgodnie z harmonogramem rozliczeń, rozpocznie się proces zbierania danych. Ten proces trwa około czterech miesięcy i obejmuje trwałą komunikację od firmy Microsoft. Jeśli płatność nie zostanie odebrana na koniec tego procesu, firma Microsoft zapisuje środki jako niezbierane.

W ramach procesu wypłaty w tym miejscu firma Microsoft mogła już wypłacić środki na wydawców, które ostatecznie nie są zbierane. W związku z tym mamy proces uzgadniania tych kwot. Aby mieć pewność, że płatność (już otrzymana) może zostać uzgodniona, otrzymasz powiadomienie, gdy klient jest w procesie zbierania danych, a zakupy są prawdopodobnie wypisywane.

Firma Microsoft zwróci wszelkie płatne opłaty za korzystanie z jednej z następujących metod: (1) firma Microsoft może odjęciu niepłatnych kwot od przyszłych wypłat. na przykład jeśli $1 000 wypłaty są uznawane za niezbierane i odpisywane, przyszłe wypłaty zostaną wstrzymane do momentu odzyskania $1 000 lub (2) firma Microsoft może zażądać zwrotu lub wydawców faktury za jakiekolwiek niezebrane kwoty.

Poniżej przedstawiono przykładowy harmonogram:

| Zdarzenie | Przybliżona data * | Widoczność partnerów |
| --- | --- | --- |
| Przykładowa data wypłaty | 10/15/2020 | Sekcja oznaczone jako **wysłane** w historii transakcji i w sekcji płatności na pulpicie nawigacyjnym wypłaty |
| <font color="red">Jeśli klient nie płacisz firmie Microsoft</font> | 12/2/2020 – 12/5/2020 | Bez zmian, taka sama jak powyżej |
| Klient otrzymuje wiadomość e-mail z pierwszą opóźnioną płatnością | 12/6/2020 | Brak |
| Klient otrzymuje zwykłe wiadomości e-mail o rosnącej pilności | 12/7/2020 – 1/31/2021 | Brak |
| Wydawca otrzymuje powiadomienie, że jest to prawdopodobnie | 1/7/2021 | Powiadomienie e-mail wysłane do wydawcy, że jego klient nie przesłał jeszcze płatności. Identyfikator transakcji i kwota dolara są uwzględniane. |
| Klient otrzymuje powiadomienie o zakończeniu | 2/1/2021 | Brak |
| Zakończenia procesu zbierania/fundusze są wypisywane | 2/15/2021 | Powiadomienie e-mail wysłane do wydawcy, że środki zostały wypisane. Identyfikator transakcji i kwota dolara są uwzględniane. |
| Wypłata jest potrącana | 3/1/2021 | Wydawca zobaczy negatywną transakcję w zestawieniu wypłaty Centrum partnerskiego |
| Wypłata została wstrzymana | 3/15/2021 | Przyszłe wypłaty zostaną wyświetlone w zestawieniu wypłaty w centrum partnerskim. Wydawca nie otrzyma płatności do momentu, gdy saldo nie będzie już ujemne.  |
|||

\* Data wypłaty przypada w pacyficznym czasie standardowym (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Liczba dni, w przypadku których płatność osiągnie konto płatne

Zwykle wysyłamy wszelkie płatności należne w danym miesiącu w piętnastym dniu tego miesiąca, ale w celu uzyskania płatności na Twoje konto zajmiemy dodatkowy czas. Liczba dni zależy od formy płatności używanej dla Twojego konta, zgodnie z poniższym opisem.

> [!NOTE]
> Pokazane poniżej dni są przybliżone; dowolna płatność może zająć więcej czasu lub dłużej.

| Metoda płatności     | Liczba dni do uzyskania dostępu do konta wypłaty     |
|--------------------|--------------------------------------------|
| PayPal             | 1 dzień roboczy                             |
| ACH/SEPA           | 2-3 dni roboczych                          |
| Przelew      | 7-10 dni roboczych                         |
|

## <a name="next-steps"></a>Następne kroki

- [Szczegóły podatku](tax-details-marketplace.md)
