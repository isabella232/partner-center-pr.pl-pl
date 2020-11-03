---
title: Zachęty — problemy ze skojarzeniami klientów
description: Dowiedz się, jak rozwiązywać problemy, które można napotkać podczas pracy z żądanymi skojarzeniami klientów z systemem CPOR.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: ab2c26cf097d6212375382cadd9ac5f4f80b5c2a
ms.sourcegitcommit: b91119c587d37b4ed36dda00c2b0b1946beb3012
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/17/2020
ms.locfileid: "92529722"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemy z zażądanymi powiązaniami partnera rekordów (CPOR)

**Dotyczy:**

- Centrum partnerskie

**Odpowiednie role:**

- Administrator rozliczeń
- Administrator globalny
- Administrator zachęt

Poniższa zawartość pomoże rozwiązać problemy, które można napotkać podczas pracy z skojarzeniami klientów.

## <a name="domain-tenant-mismatch"></a>Niezgodność dzierżawy domeny

W przepływie wiązania powiązania partnera rekordu (CPOR), zostanie wyświetlony monit o podanie identyfikatora dzierżawy klienta i poddomeny. Jeśli zostanie wyświetlony komunikat o błędzie informujący, że nie są zgodne, skontaktuj się z klientem, aby upewnić się, że masz odpowiednie szczegóły.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Błędy subskrypcji w przepływie powiązań powiązania CPOR

W przepływie CPOR powiązań skojarzenia może zostać wyświetlony monit o podanie subskrypcji dla produktu, który próbujesz zgłosić za pośrednictwem Business Applications (Dynamics 365). Prosimy o subskrypcję, ponieważ firma Microsoft zaleca dynamiczne sprawdzanie, czy produkt i subskrypcja należy do dzierżawy, dla której ma zostać przejęte żądanie. Sprawdzamy również, czy subskrypcja jest w stanie aktywnym/z stanem prolongaty.

Jeśli wystąpi błąd, może się to zdarzyć z kilku powodów:

- Wybrany produkt nie istnieje w dzierżawie klienta
- Podana subskrypcja nie jest dla usługi Dynamics
- Podana subskrypcja dotyczy dostawcy CSP
- Klient nie został jeszcze aktywowany/nie zainicjowano obsługi administracyjnej produktów dla tej subskrypcji
- Subskrypcja została już przejęta
- Podany identyfikator nie jest IDENTYFIKATORem subskrypcji

Jeśli masz pytanie dotyczące dokładności subskrypcji, skontaktuj się z klientem, aby upewnić się, że subskrypcja jest poprawna i czy używasz prawidłowego identyfikatora dzierżawy.

Jeśli ta trasa nie rozwiązała problemu, skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Gdy subskrypcje będą dostępne dla roszczeń

Po odebraniu subskrypcji zostanie wyświetlony komunikat o błędzie, jeśli subskrypcja nie została jeszcze zainicjowana. Istnieje kilka kroków, które klient musi podjąć, aby uzyskać dostęp do tej subskrypcji dla platformy CPOR i udostępnić ją do roszczeń. Jeśli wystąpi błąd podczas próby zgłoszenia subskrypcji, skontaktuj się z klientem, aby upewnić się, że został on zainicjowany, a poprawność subskrypcji jest prawidłowa. Jeśli ta trasa została już wykonana, skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Jakie działania wybieramy?

Platforma CPORing platform umożliwia korzystanie z oświadczeń skojarzenia CPOR powiązanych z obszarami rozwiązań Business Applications i Microsoft 365. Poniżej przedstawiono działania, które mają zastosowanie do każdego obszaru rozwiązania. Wybierz odpowiednie działanie na podstawie opisów, aby uniknąć konieczności ponownego zgłoszenia w przyszłości. Pozyskanie z nieprawidłowym działaniem może spowodować nieodebrane zyski i zysk zachęty.


| Obszar rozwiązania | Działanie | Dotyczy |
| ------ | ----------- | ----------- |
| Aplikacje biznesowe      | Przedsprzedażna   | Wybierz, czy ma wpływ na zakup kwalifikującego się produktu i czy ma zostać zastosowany do bodźci przedsprzedaży. Ta opcja ma zastosowanie tylko wtedy, gdy klient kupił te produkty za pośrednictwem umowy licencjonowania zbiorowego lub sieci Web. |
|    |  Użycie  | Wybierz, jeśli chcesz, aby system został rozłożenie i użycie kwalifikującego się obciążenia, i chcesz zastosować do bodźci dotyczącej użycia. Ta opcja ma zastosowanie tylko wtedy, gdy klient kupił te produkty za pośrednictwem umowy licencjonowania zbiorowego lub sieci Web. |
|    | Skojarzenie przychodu   | Wybierz, czy ma wpływ na wybór kwalifikującego się produktu jako osoba mająca wpływ na działalność biznesową. Ta opcja dotyczy tylko skojarzenia przychodu, a nie do zapłacenia zachęty. Ta opcja ma zastosowanie tylko wtedy, gdy klient kupił te produkty za pośrednictwem umowy licencjonowania zbiorowego lub sieci Web.   |
| Microsoft 365   | Użycie   | Wybierz, jeśli chcesz, aby system został rozłożenie i użycie kwalifikującego się obciążenia, i chcesz zastosować do bodźci dotyczącej użycia. |

## <a name="which-mpn-do-i-choose"></a>Które MPN mam wybrać?

W przepływie CPOR powiązań skojarzenia zostanie wyświetlony monit o wybranie firmy MPN, która powinna zostać skojarzona z podaną przez Ciebie klientem. Firma może mieć wiele usługi MPNS, z których część może zostać zarejestrowana w programach zachęty i innych skojarzonych z typem partnera, takim jak FRP FastTrack. Przepływ CPOR powiązań skojarzenia będzie identyfikować, które usługi MPNS są zarejestrowane w programie zachęty, ale nie powiedzie się, jeśli jest to konkretny typ partnera MPN. Ważne jest, aby wybrać poprawną MPN, aby uniknąć konieczności ponownego zgłoszenia w przyszłości. Pozyskanie z nieprawidłowym MPN może spowodować nieodebrane zyski i zysk zachęty.

Jeśli nie wiesz, których MPN użyć, skontaktuj się z administratorem globalnym.

Jeśli MPN, którego chcesz użyć, nie jest zarejestrowana, możesz nim zarządzać na [karcie Przegląd zachęt](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (wymagane jest zalogowanie się).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Wybieranie produktu a wprowadzenie do subskrypcji

Gdy produkt Dynamics zostanie przejęty i zatwierdzony, partner może wyświetlić identyfikator subskrypcji w samym roszczeniu skojarzenia CPOR. Gdy ta subskrypcja jest przejęta, jest ona aktywna lub w stanie prolongaty, ale może istnieć czas na zakończenie subskrypcji, a w oddzielnym wystąpieniu skojarzenia CPOR muszą zostać przejęte nowe subskrypcje.

## <a name="competing-claims"></a>Oświadczenia konkurujące

Jeśli tworzysz CPOR skojarzenie skojarzenia dla klienta i ich produktów, które są już skojarzone z innym partnerem, Twoje zgłoszenie przejdzie przez proces rozstrzygania:

1. Po utworzeniu nowego skojarzenia klienta firma Microsoft sprawdzi szczegóły skojarzenia i przesłanej weryfikacji wykonania, aby zapewnić jego dokładność.

2. Jeśli ty i inny partner zawiążą ten sam Klient i produkt/obciążenie, firma Microsoft zapoznaje się z dokumentacją dotyczącą wykonywania każdego partnera, aby określić, który partner ma zatwierdzić.

3. Mogą być wymagane dodatkowe informacje od obu partnerów, co może powodować opóźnienia w przetwarzaniu żądania skojarzenia.

4. Twoje powiązanie skojarzenia CPOR będzie nadal weryfikowane w ciągu pięciu dni roboczych, mimo że jego stan może pozostać w _ramach przeglądu_ przez dłuższy czas. Ten scenariusz może wystąpić, gdy firma Microsoft współpracuje z partnerem, który aktualnie jest właścicielem produktu/obciążenia. W takim przypadku użytkownik zostanie powiadomiony w sekcji komentarzy Twojego żądania. 

>[!IMPORTANT]
>Jeśli będziemy potrzebować dodatkowych informacji w celu zweryfikowania poprawności CPORu skojarzenia (PoE), skontaktujemy się z Tobą za pośrednictwem sekcji komentarzy dotyczących roszczeń dotyczących powiązań CPOR.

## <a name="next-steps"></a>Następne kroki

- [Wprowadzenie do zachęt](incentives-get-started-intro.md)
