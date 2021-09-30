---
title: Strona customers for MCI engagements (Strona klientów na potrzeby angażowania klientów w działania mci)
description: Użyj strony Customers (Klienci) w sekcji Microsoft Commerce Incentive (MCI) program Engagements (Ang. Microsoft Commerce Incentive) Engagements (Angażowania programu Microsoft Commerce Incentive, MCI), aby zarządzać klientami.
author: Karthic83
ms.author: kashanum
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: how-to
ms.date: 09/29/2021
ms.custom: template-how-to
ms.openlocfilehash: 4d4d3de7bc53440765538654f8e82c3c048f5922
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/29/2021
ms.locfileid: "129293463"
---
# <a name="customers-page-for-mci-engagements"></a>Strona customers for MCI engagements (Strona klientów na potrzeby angażowania klientów w działania mci)

**Odpowiednie role:** Zachęty dla administratorów | Zachęty użytkownika

>[!NOTE]
>Ma to zastosowanie tylko w przypadku zaangażowania w intencję kompilacji, czyli warsztatów. 

Strona **Customers** (Klienci) sortuje klientów według kwalifikujących się, nie kwalifikowalnych i ukończonych dla każdego zaangażowania. Strona jest wstępnie zasypyowana wszystkimi klientami, którzy wyrazić zgodę na wszelkie warsztaty w Partner Center. 

:::image type="content" source="images/incentives/customers-page.png" alt-text="Zrzut ekranu przedstawiający stronę Customers (Klienci)." lightbox="images/incentives/customers-page.png":::

- Karta **Kwalifikujące** się zawiera wszystkich klientów, którzy są uprawnieni do warsztatów. 
   - Kolumna **Typ** zawiera listę klientów jako "aktywnych", jeśli otrzymano zgodę od klienta. Do tego czasu będzie ona zawierała powiedze "not started" (nie rozpoczęto).
- Karta **Bez kwalifikowania zawiera** wszystkich klientów, którzy nie są kwalifikowani do warsztatów z jednego z trzech powodów:  
   - Klient nie spełnia kryteriów kwalifikowalności dla zaangażowania, 
   - Klient wyraził zgodę dla innego partnera lub 
   - Klient brał już udział w warsztatach z innym partnerem. 
- Karta **Ukończono** zawiera wszystkich klientów, dla których ukończono te warsztaty. Aby wyświetlić szczegóły swojego roszczenia u tego klienta, wybierz pozycję Wyświetl roszczenie dotyczące **warsztatów** w **kolumnie** Akcja.

W przypadku każdego zaangażowania musisz dodać klienta lub uzyskać klienta (nie oba).

## <a name="add-a-customer"></a>Dodawanie klienta 
1. Wybierz **pozycję + Dodaj klienta** na stronie **Klienci** odpowiedniego zaangażowania w warsztaty, korzystając z **karty Kwalifikowanie** się.
2. Podaj identyfikator lokalizacji MPN na potrzeby warsztatów oraz adres e-mail klienta. Pole **Identyfikator dzierżawy/TPID klienta** jest opcjonalne. Będą wyświetlane tylko identyfikatory lokalizacji MPN, które są zarejestrowane w programie MCI i kwalifikują się do tego zaangażowania. Wybierz opcję **Dalej**.
   - Jeśli nie poniesiesz identyfikatora dzierżawy lub najwyższego identyfikatora nadrzędnego (TPID) klienta, system będzie wyprowadzać identyfikator dzierżawy z adresu e-mail klienta. Następnie zostanie uruchomiony sprawdzanie uprawnień klienta na potrzeby warsztatów.
   - Jeśli nie można znaleźć identyfikatora dzierżawy klienta przy użyciu adresu e-mail, zostanie wyświetlony monit o podanie innego adresu e-mail lub identyfikatora dzierżawy/TPID.
   - Jeśli podano identyfikator dzierżawy/identyfikator TPID, system zapewni, że domena poczty e-mail będzie odpowiadać identyfikatorowi dzierżawy. Jeśli zostanie znaleziona niezgodność, system poprosi o podanie przyczyny.

   :::image type="content" source="images/incentives/add-customer-1.png" alt-text="Zrzut ekranu nr 1 z 3 przedstawiający sposób dodawania klienta." lightbox="images/incentives/add-customer-1.png":::

3. Wybierz warsztaty, dla których chcesz dodać klienta. Można wybrać tylko te warsztaty, do których uprawnieni są Zarówno Ty, jak i Twój klient. Wybierz opcję **Dalej**.

:::image type="content" source="images/incentives/add-customer-2.png" alt-text="Zrzut ekranu nr 2 z 3 przedstawiający sposób dodawania klienta." lightbox="images/incentives/add-customer-2.png":::

4. Przejrzyj informacje i wybierz pozycję **Dodaj klienta.** Otrzymasz potwierdzenie dodania klienta.

:::image type="content" source="images/incentives/add-customer-3.png" alt-text="Zrzut ekranu nr 3 z 3 przedstawiający sposób dodawania klienta." lightbox="images/incentives/add-customer-3.png":::

Powinien zostać wyświetlony dodany klient na odpowiednich stronach **Customers** (Klienci) na potrzeby warsztatów wybranych w kroku 3.

## <a name="claim-a-customer"></a>Roszczenie klienta 
Karta **Kwalifikuje** się na **stronie Klienci** zostanie wstępnie przesłoniona listą klientów, którzy są ci znani, partnerowi, za pośrednictwem innych zaangażowania. Możesz zainicjować warsztaty z dowolnym z tych klientów. 
1. Wybierz **pozycję Claim customer (Roszczenie** klienta) w kolumnie Action **(Akcja).** 
2. Wybierz identyfikator lokalizacji MPN na warsztaty. Zostaną wyświetlone tylko identyfikatory lokalizacji MPN zarejestrowane w programie MCI, które kwalifikują się do tego zaangażowania. Wybierz opcję **Dalej**.

   :::image type="content" source="images/incentives/claim-customer-1.png" alt-text="Zrzut ekranu nr 1 z 3 przedstawiający sposób żądania klienta." lightbox="images/incentives/claim-customer-1.png":::

3. Wybierz warsztaty, które chcesz dodać, a następnie wybierz pozycję **Dalej.**

   :::image type="content" source="images/incentives/claim-customer-2.png" alt-text="Zrzut ekranu nr 2 z 3 przedstawiający sposób roszczenia klienta." lightbox="images/incentives/claim-customer-2.png":::

4. Przejrzyj informacje i wybierz pozycję **Dodaj klienta.** Otrzymasz potwierdzenie, że klient został przejmowany.

   :::image type="content" source="images/incentives/claim-customer-3.png" alt-text="Zrzut ekranu nr 3 z 3 przedstawiający sposób żądania klienta." lightbox="images/incentives/claim-customer-3.png":::

## <a name="ask-for-customer-consent"></a>Poproś o zgodę klienta 
Jeśli chcesz przeprowadzić warsztaty z klientem, musisz poprosić klienta o zgodę na uczestnictwo w warsztatach. Po dodaniu lub otrzymaniu klienta będziesz mieć łącznie 30 dni na uzyskanie zgody.

Po dodaniu lub prawu klienta zobaczysz, ile dni pozostało do uzyskania zgody, w kolumnie stanu na **stronie** Klienci.
1. Wybierz **pozycję Trigger customer consent (Wyzwolij** zgodę klienta) w kolumnie Action **(Akcja).** 
2. Podaj adres e-mail i informacje kontaktowe klienta wraz z informacjami kontaktowymi dla Twojej firmy. Następnie wybierz przycisk **Dalej**.

   :::image type="content" source="images/incentives/ask-consent-1.png" alt-text="Zrzut ekranu nr 1 z 2 przedstawiający sposób żądania zgody klienta." lightbox="images/incentives/ask-consent-1.png":::

3. Przejrzyj szczegóły i wybierz pozycję **Wyślij w celu wyrażenia zgody.** Do klienta zostanie wysłana wiadomość e-mail, dzięki czemu będzie on w stanie zaakceptować lub odrzucić warsztaty.
   - Jeśli nie otrzymano zgody, możesz wysłać przypomnienie, klikając link **Wyślij** ponownie zgodę klienta w **kolumnie** Akcja.
   - Jeśli klient został nowo dodany, ale odmawia udziału w warsztatach lub nie odpowie na wymaganej  osi czasu, nie będzie już wyświetlany na stronie Klienci dla tego zaangażowania.

   :::image type="content" source="images/incentives/ask-consent-2.png" alt-text="Zrzut ekranu 2 z 2 przedstawiający sposób żądania zgody klienta." lightbox="images/incentives/ask-consent-2.png":::

Gdy klient wyrazić zgodę, będziesz mieć 90 dni na przeprowadzenie warsztatów.

## <a name="next-steps"></a>Następne kroki
[Przesyłanie roszczenia w ramach warsztatów](/mci-engagements-workshop)

[Omówienie zaangażowania mci i uprawnienia](/mci-engagements)

[Użyj tych zasobów, aby rozpocząć pracę z zachętami](/incentives-get-started-intro)

[Określanie uprawnień do programu zachęt](/incentives-determined-your-program-eligibility)

[Rejestracja i zarządzanie użytkownikami w programie zachęt](/incentives-enroll)