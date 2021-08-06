---
title: Zachęty — problemy ze skojarzeniami klientów
description: Dowiedz się, jak rozwiązać problemy, które są związane z pracą ze skojarzeniami klientów CPOR (Claimed Partner of Record).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: d23c95981c39bb9b9773e3b1e6f474146f41325546cc5f96408237e2213280d2
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681811"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemy z skojarzeniami klientów w przypadku roszczeń partnerów rekordów (CPOR, Claimed Partner of Record)

**Odpowiednie role:** Administrator rozliczeń | Administrator globalny | Administrator zachęt

Zawartość poniżej pomoże Ci rozwiązać problemy, które mogą się dzieje podczas pracy ze skojarzeniami klientów.

## <a name="domain-tenant-mismatch"></a>Niezgodność dzierżawy domeny

W przepływie oświadczenia skojarzenia partnera roszczeń (CPOR, Claimed Partner of Record) zostaniesz poproszony o podanie identyfikatora dzierżawy klienta i poddomeny. Jeśli zostanie wyświetlony komunikat o błędzie z informacją, że nie są one zgodne, skontaktuj się z klientem, aby upewnić się, że masz poprawne szczegóły.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Błędy subskrypcji w przepływie skojarzenia CPOR

W przepływie roszczenia skojarzenia CPOR może zostać poproszony o podanie subskrypcji dla produktu, który próbujesz uzyskać za pośrednictwem usługi Business Applications (Dynamics 365). Pytamy o subskrypcję, ponieważ dynamicznie sprawdzamy, czy produkt i subskrypcja należą do dzierżawy, której się żąda. Sprawdzamy również, czy subskrypcja jest w stanie aktywnej/w stanie prolongaty.

Jeśli wystąpi błąd, może to być z kilku powodów:

- Wybrany produkt nie istnieje w dzierżawie klienta
- Podana subskrypcja nie jest dla usługi Dynamics
- Podana subskrypcja dotyczy dostawcy CSP
- Klient nie aktywował jeszcze/nie aprowizował produktów dla tej subskrypcji
- Subskrypcja została już przejęta
- Podany identyfikator nie jest identyfikatorem subskrypcji

Jeśli masz pytanie dotyczące dokładności subskrypcji, we współpracy z klientem upewnij się, że subskrypcja jest poprawna i że używasz poprawnego identyfikatora dzierżawy.

Jeśli ta trasa nie rozwiązała problemu, skontaktuj się z pomocą [techniczną](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Kiedy będą dostępne subskrypcje do oświadczenia

W przypadku żądania subskrypcji wystąpi błąd, jeśli subskrypcja nie została jeszcze aprowizowana. Istnieje kilka kroków, które klient musi wykonać, aby subskrypcja stała się dostępna dla platformy CPOR, aby ją przejąć i udostępnić do roszczenia. Jeśli podczas próby uzyskania subskrypcji występuje błąd, skontaktuj się z klientem, aby upewnić się, że została ona aprowizowana i że przejmowana subskrypcja jest poprawna. Jeśli ta trasa została już przekierowyna, skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Które działanie wybrać?

Platforma oświadczeń CPOR umożliwia oświadczenia skojarzenia CPOR związane Business Applications i Microsoft 365 rozwiązaniami. Działania, które mają zastosowanie do każdego obszaru rozwiązania, znajdują się poniżej. Wybierz odpowiednie działanie na podstawie opisów, aby uniknąć konieczności odzyskiwania w przyszłości. Oświadczenie o nieprawidłowym działaniu może spowodować nieuprawnnianie uprawnień i zarobki zachęt.


| Obszar rozwiązania | Działanie | Dotyczy |
| ------ | ----------- | ----------- |
| Aplikacje biznesowe      | Przedsprzedaż   | Wybierz pozycję , jeśli wpłynęło to na zakup kwalifikującego się produktu i chcesz złożyć wniosek o zachęty przedsprzedażowe. Ta opcja ma zastosowanie tylko w przypadku, gdy klient zakupił te produkty w ramach umowy licencjonowania zbiorowego lub usługi Web-Direct. |
|    |  Użycie  | Wybierz, czy chcesz uzyskać zachęty dotyczące użycia i wdrożenia kwalifikujących się obciążeń. Ta opcja ma zastosowanie tylko w przypadku, gdy klient zakupił te produkty w ramach umowy licencjonowania zbiorowego lub usługi Web-Direct. |
|    | Skojarzenie przychodów   | Wybierz, czy wpłynęło to na wybór kwalifikującego się produktu jako osoby wywłaszczacej działalność biznesową. Ta opcja dotyczy tylko skojarzenia przychodów, a nie płatności zachęt. Ta opcja ma zastosowanie tylko w przypadku, gdy klient zakupił te produkty w ramach umowy licencjonowania zbiorowego lub usługi Web-Direct.   |
| Microsoft 365   | Użycie   | Wybierz, czy chcesz uzyskać zachęty dotyczące użycia i wdrożenia kwalifikujących się obciążeń. |

## <a name="which-mpn-do-i-choose"></a>Który mpn wybrać?

W przepływie roszczenia skojarzenia CPOR zostanie poproszony o wybranie firmowego mpn, który powinien być skojarzony z pracą, która ma być skojarzona z pracą klienta końcowego. Firma może mieć wiele sieci MPN, z których część może być zarejestrowanych w programach zachęt, a inne mogą być skojarzone z typem partnera, takim jak FRP FastTrack. Przepływ roszczenia skojarzenia CPOR określi, które sieci MPN są zarejestrowane w programie zachęt, ale nie określi, czy jest to określony typ partnera MPN. Ważne jest, aby wybrać właściwy program MPN, aby uniknąć konieczności odzyskiwania w przyszłości. Roszczenie z nieprawidłowym programem MPN może spowodować nieuprawnianie uprawnień i zarobki zachęt.

Jeśli nie wiesz, którego programu MPN użyć, skontaktuj się z administratorem globalnym.

Jeśli program MPN, którego chcesz używać, nie jest zarejestrowany, możesz zarządzać tym na karcie [Zachęty — omówienie](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (wymagane jest zalogowanie).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Wybieranie produktu a wprowadzanie subskrypcji

Po zatwierdzeniu i zatwierdzeniu produktu Dynamics partner może wyświetlić identyfikator subskrypcji w samym roszczeniach skojarzenia CPOR. Gdy ta subskrypcja jest przejmowana, jest w stanie aktywnym lub w stanie prolongaty, ale może wystąpić czas na jej zakończenie, a nowe subskrypcje muszą zostać przejmowane w oddzielnym skojarzenia CPOR.

## <a name="competing-claims"></a>Konkurujące roszczenia

Jeśli tworzysz roszczenie dotyczące skojarzenia CPOR dla klienta i jego produktów, które są już skojarzone z innym partnerem, Twoje roszczenie zostanie rozsądzone:

1. Po utworzeniu nowego skojarzenia klienta firma Microsoft sprawdzi szczegóły skojarzenia i przesłanej weryfikacji wykonania, aby zapewnić jego dokładność.

2. Jeśli Ty i inny partner żądacie tego samego klienta i produktu/obciążenia, firma Microsoft przejmie dokumentację weryfikacji wykonania poszczególnych partnerów, aby określić, którego partnera należy zatwierdzić.

3. Od obu partnerów mogą być wymagane dodatkowe informacje, które mogą powodować opóźnienia w przetwarzaniu żądania skojarzenia.

4. Twoje roszczenie dotyczące skojarzenia CPOR będzie nadal przeglądane  w ciągu pięciu dni roboczych, chociaż jego stan może pozostać w trakcie przeglądu przez dłuższy czas. Ten scenariusz może wystąpić, gdy firma Microsoft współpracuje z partnerem, który jest obecnie właścicielem produktu/obciążenia. Jeśli tak się stanie, użytkownik zostanie powiadomiony w sekcji komentarzy roszczenia. 

>[!IMPORTANT]
>Jeśli będziemy wymagać dodatkowych informacji w celu zweryfikowania weryfikacji wykonania skojarzenia CPOR, skontaktujemy się z Tobą za pośrednictwem sekcji komentarzy roszczenia skojarzenia CPOR.

## <a name="next-steps"></a>Następne kroki

- [Wprowadzenie do zachęt](incentives-get-started-intro.md)
