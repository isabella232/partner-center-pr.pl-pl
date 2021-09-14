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
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248112"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemy ze skojarzeniami klientów WCPOR (Claimed Partner of Record)

**Odpowiednie role:** Administrator rozliczeń | Administrator globalny | Administrator zachęt

Zawartość poniżej pomoże Ci rozwiązać problemy, które mogą się dzieje podczas pracy ze skojarzeniami klientów.

## <a name="domain-tenant-mismatch"></a>Niezgodność dzierżawy domeny

W przepływie oświadczenia o skojarzeniach claimed Partner of Record (CPOR) zostanie poproszony o podanie identyfikatora dzierżawy klienta i poddomeny. Jeśli zostanie wyświetlony komunikat o błędzie z informacją, że nie są one zgodne, skontaktuj się z klientem, aby upewnić się, że masz poprawne szczegóły.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Błędy subskrypcji w przepływie skojarzenia CPOR

W przepływie skojarzenia CPOR może zostać poproszony o podanie subskrypcji produktu, który próbujesz uzyskać za pośrednictwem usługi Business Applications (Dynamics 365). Pytamy o subskrypcję, ponieważ dynamicznie sprawdzamy, czy produkt i subskrypcja należą do dzierżawy, której się żąda. Sprawdzamy również, czy subskrypcja jest aktywna/ma stan prolongaty.

Jeśli wystąpi błąd, może to być z kilku powodów:

- Wybrany produkt nie istnieje w dzierżawie klienta
- Podana subskrypcja nie jest dla usługi Dynamics
- Podana subskrypcja dotyczy dostawcy CSP
- Klient nie aktywował jeszcze/nie aprowizował produktów dla tej subskrypcji
- Subskrypcja została już przejęta
- Podany identyfikator nie jest identyfikatorem subskrypcji

Jeśli masz pytanie dotyczące dokładności subskrypcji, we współpracy z klientem upewnij się, że subskrypcja jest poprawna i że używasz poprawnego identyfikatora dzierżawy.

Jeśli ta trasa nie rozwiązała problemu, skontaktuj się z pomocą [techniczną](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Kiedy będą dostępne subskrypcje do żądania

W przypadku żądania subskrypcji wystąpi błąd, jeśli subskrypcja nie została jeszcze aprowizowana. Istnieje kilka kroków, które klient musi wykonać, aby subskrypcja stała się dostępna dla platformy CPOR, aby ją przejąć i udostępnić do żądania. Jeśli podczas próby uzyskania subskrypcji występuje błąd, skontaktuj się z klientem, aby upewnić się, że została ona aprowizowana i że przejmowana subskrypcja jest poprawna. Jeśli ta trasa została już przekierowyna, skontaktuj się z pomocą [techniczną](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Które działanie wybrać?

Platforma oświadczeń CPOR umożliwia oświadczenia skojarzenia CPOR związane Business Applications i Microsoft 365 rozwiązania. Poniżej przedstawiono działania, które mają zastosowanie do każdego obszaru rozwiązania. Wybierz odpowiednie działanie na podstawie opisów, aby uniknąć konieczności odzyskiwania w przyszłości. Oświadczenie o nieprawidłowym działaniu może spowodować nieuprawnną kwalifikowalność i zarobki zachęt.


| Obszar rozwiązania | Działanie | Dotyczy |
| ------ | ----------- | ----------- |
| Aplikacje biznesowe      | Przedsprzedaż   | Wybierz, czy wpłynęło to na zakup kwalifikującego się produktu, i chcesz zastosować zachęty przedsprzedażowe. Ta opcja ma zastosowanie tylko wtedy, gdy klient zakupił te produkty w ramach umowy licencjonowania zbiorowego lub usługi Web-Direct. |
|    |  Użycie  | Wybierz, czy chcesz uzyskać zachęty dotyczące użycia i wdrożenia kwalifikującego się obciążenia. Ta opcja ma zastosowanie tylko wtedy, gdy klient zakupił te produkty w ramach umowy licencjonowania zbiorowego lub usługi Web-Direct. |
|    | Skojarzenie przychodów   | Wybierz, czy wpłynęło to na wybór kwalifikującego się produktu jako osoby wpłynęły na działalność biznesową. Ta opcja dotyczy tylko skojarzenia przychodów, a nie płatności zachęt. Ta opcja ma zastosowanie tylko wtedy, gdy klient zakupił te produkty w ramach umowy licencjonowania zbiorowego lub usługi Web-Direct.   |
| Microsoft 365   | Użycie   | Wybierz, czy chcesz uzyskać zachęty dotyczące użycia i wdrożenia kwalifikującego się obciążenia. |

## <a name="which-mpn-do-i-choose"></a>Który mpn wybrać?

W przepływie roszczenia skojarzenia CPOR zostanie poproszony o wybranie firmowego mpn, który powinien być skojarzony z pracą, w przypadku których klient końcowy ma pracować. Firma może mieć wiele sieci MPN, z których część może być zarejestrowanych w programach zachęt, a inne skojarzone z typem partnera, takim jak frp FastTrack. Przepływ roszczenia skojarzenia CPOR określi, które sieci MPN są zarejestrowane w programie zachęt, ale nie określi, czy jest to określony typ partnera MPN. Ważne jest, aby wybrać prawidłowy program MPN, aby uniknąć konieczności odzyskiwania w przyszłości. Roszczenie za pomocą nieprawidłowego mpn może spowodować nieuprawnną kwalifikowalność i zarobki zachęt.

Jeśli nie wiesz, którego programu MPN użyć, skontaktuj się z administratorem globalnym.

Jeśli program MPN, którego chcesz użyć, nie jest zarejestrowany, możesz zarządzać tym na karcie [Przegląd](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) zachęt (wymagane jest zalogowanie).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Wybieranie produktu a wprowadzanie subskrypcji

Po zatwierdzeniu i zatwierdzeniu produktu Dynamics partner może wyświetlić identyfikator subskrypcji w samym oświadczeniem skojarzenia CPOR. Gdy ta subskrypcja jest przejmowana, jest w stanie aktywnym lub w stanie prolongaty, ale może wystąpić czas, gdy subskrypcja się zakończy, a nowe subskrypcje muszą zostać przejmowane w oddzielnym skojarzeniach CPOR.

## <a name="competing-claims"></a>Konkurujące roszczenia

Jeśli tworzysz roszczenie dotyczące skojarzenia CPOR dla klienta i jego produktów, które są już skojarzone z innym partnerem, Twoje roszczenie zostanie rozsądzone:

1. Po utworzeniu nowego skojarzenia klienta firma Microsoft sprawdzi szczegóły skojarzenia i przesłanej weryfikacji wykonania, aby zapewnić jego dokładność.

2. Jeśli Ty i inny partner przejmiecie ten sam klient i produkt/obciążenie, firma Microsoft przejmie dokumentację weryfikacji wykonania każdego partnera, aby określić, którego partnera należy zatwierdzić.

3. Obaj partnerzy mogą zażądać dodatkowych informacji, co może spowodować opóźnienia w przetwarzaniu żądania skojarzenia.

4. Twoje roszczenie dotyczące skojarzenia CPOR będzie nadal przeglądane  w ciągu pięciu dni roboczych, chociaż jego stan może pozostać w obszarze Przeglądu przez dłuższy czas. Ten scenariusz może wystąpić, gdy firma Microsoft współpracuje z partnerem, który jest obecnie właścicielem produktu/obciążenia. Jeśli tak się stanie, użytkownik zostanie powiadomiony w sekcji komentarzy swojego roszczenia. 

>[!IMPORTANT]
>Jeśli będziemy wymagać dodatkowych informacji w celu zweryfikowania weryfikacji wykonania skojarzenia CPOR, skontaktujemy się z Tobą za pośrednictwem sekcji komentarzy skojarzenia CPOR.

## <a name="next-steps"></a>Następne kroki

- [Wprowadzenie do zachęt](incentives-get-started-intro.md)
