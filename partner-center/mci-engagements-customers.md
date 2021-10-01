---
title: Strona Customers (Klienci) dla zaangażowania mci
description: Użyj strony Customers (Klienci) w sekcji Microsoft Commerce Incentive (MCI) program Engagements (Angażowanie programu Microsoft Commerce Incentive, MCI), aby zarządzać klientami.
author: Karthic83
ms.author: kashanum
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: how-to
ms.date: 09/29/2021
ms.custom: template-how-to
ms.openlocfilehash: bfa3185213abe5e166c3049602d3ca2dc16be70c
ms.sourcegitcommit: 6d29e7e6d700ee5638ba10ee12f75e37f993dae9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/01/2021
ms.locfileid: "129365144"
---
# <a name="customers-page-for-mci-engagements"></a>Strona Customers (Klienci) dla zaangażowania mci

**Odpowiednie role:** Zachęty dla administratorów | Zachęty użytkownika

>[!NOTE]
>Ma to zastosowanie tylko w przypadku zaangażowania w intencję kompilacji, czyli warsztatów. 

Na **stronie Klienci** klienci są sortowane według kwalifikujących się, niekwalifikowanych i ukończonych dla każdego zaangażowania. Strona jest wstępnie zasypyowana wszystkimi klientami, którzy wyrazić zgodę na wszystkie warsztaty w Partner Center. 

:::image type="content" source="images/incentives/customers-page.png" alt-text="Zrzut ekranu przedstawiający stronę Customers (Klienci)." lightbox="images/incentives/customers-page.png":::

- Karta **Kwalifikujące** się zawiera wszystkich klientów, którzy kwalifikują się do warsztatów. 
   - Kolumna **Typ** zawiera listę klientów jako "aktywnych", jeśli otrzymano zgodę od klienta. Do tego czasu będzie ona zawierała "nie rozpoczęto".
- Karta **Bez kwalifikowania zawiera** wszystkich klientów, którzy nie są kwalifikowani do warsztatów z jednego z trzech powodów:  
   - Klient nie spełnia kryteriów kwalifikowalności dla zaangażowania. 
   - Klient wyraził zgodę dla innego partnera lub 
   - Klient brał już udział w warsztatach z innym partnerem. 
- Karta **Complete** (Ukończono) zawiera wszystkich klientów, dla których ukończono te warsztaty. Aby wyświetlić szczegóły roszczenia dla tego klienta, wybierz pozycję Wyświetl roszczenie dotyczące **warsztatów** w **kolumnie** Akcja.

W przypadku każdego zaangażowania musisz dodać klienta lub uzyskać klienta (nie oba).

## <a name="add-a-customer"></a>Dodawanie klienta 
1. Wybierz **pozycję + Dodaj klienta** na stronie **Klienci** odpowiedniego zaangażowania w warsztaty przy użyciu **karty Kwalifikowane.**
2. Podaj identyfikator lokalizacji MPN na potrzeby warsztatów oraz adres e-mail klienta. Pole **Identyfikator TPID klienta /Identyfikator dzierżawy** jest opcjonalne. Będą wyświetlane tylko identyfikatory lokalizacji MPN, które są zarejestrowane w programie MCI i są uprawnione do tego zaangażowania. Wybierz opcję **Dalej**.
   - Jeśli nie poniesiesz identyfikatora dzierżawy lub najwyższego identyfikatora nadrzędnego (TPID) dla klienta, system będzie wyprowadzać identyfikator dzierżawy z adresu e-mail klienta. Następnie zostanie uruchomiony sprawdzanie uprawnień klienta na potrzeby warsztatów.
   - Jeśli nie można znaleźć identyfikatora dzierżawy klienta przy użyciu adresu e-mail, zostanie wyświetlony monit o podanie innego adresu e-mail lub identyfikatora dzierżawy/TPID.
   - Jeśli podano identyfikator dzierżawy/identyfikator TPID, system zapewni zgodność domeny poczty e-mail z identyfikatorem dzierżawy. Jeśli zostanie znaleziona niezgodność, system poprosi o podanie przyczyny.

   :::image type="content" source="images/incentives/add-customer-1.png" alt-text="Zrzut ekranu 1 z 3 przedstawiający sposób dodawania klienta." lightbox="images/incentives/add-customer-1.png":::

3. Wybierz warsztaty, dla których chcesz dodać klienta. Można wybrać tylko te warsztaty, do których kwalifikuje się Zarówno Ty, jak i Twój klient. Wybierz opcję **Dalej**.

:::image type="content" source="images/incentives/add-customer-2.png" alt-text="Zrzut ekranu 2 z 3 przedstawiający sposób dodawania klienta." lightbox="images/incentives/add-customer-2.png":::

4. Przejrzyj informacje i wybierz pozycję **Dodaj klienta.** Otrzymasz potwierdzenie dodania klienta.

:::image type="content" source="images/incentives/add-customer-3.png" alt-text="Zrzut ekranu nr 3 z 3 przedstawiający sposób dodawania klienta." lightbox="images/incentives/add-customer-3.png":::

Powinien zostać wyświetlony dodany przez Ciebie klient  na odpowiednich stronach Customers (Klienci) dla warsztatów wybranych w kroku 3.

## <a name="claim-a-customer"></a>Roszczenie klienta 
Karta **Kwalifikujące** się na **stronie Klienci** zostanie wstępnie zasypana listą klientów, którzy są ci znani, partnerowi, za pośrednictwem innych zaangażowania. Możesz zainicjować warsztaty z dowolnym z tych klientów. 
1. W kolumnie Akcja wybierz pozycję Claim **customer** **(Roszczenie klienta).** 
2. Wybierz identyfikator lokalizacji MPN na warsztaty. Zostaną wyświetlone tylko identyfikatory lokalizacji MPN zarejestrowane w programie MCI, które kwalifikują się do tego zaangażowania. Wybierz opcję **Dalej**.

   :::image type="content" source="images/incentives/claim-customer-1.png" alt-text="Zrzut ekranu 1 z 3 przedstawiający sposób żądania klienta." lightbox="images/incentives/claim-customer-1.png":::

3. Wybierz warsztaty, które chcesz dodać, a następnie wybierz pozycję **Dalej.**

   :::image type="content" source="images/incentives/claim-customer-2.png" alt-text="Zrzut ekranu 2 z 3 przedstawiający sposób żądania klienta." lightbox="images/incentives/claim-customer-2.png":::

4. Przejrzyj informacje i wybierz pozycję **Dodaj klienta.** Otrzymasz potwierdzenie, że klient został przejmowany.

   :::image type="content" source="images/incentives/claim-customer-3.png" alt-text="Zrzut ekranu nr 3 z 3 przedstawiający sposób żądania klienta." lightbox="images/incentives/claim-customer-3.png":::

## <a name="ask-for-customer-consent"></a>Poproś o zgodę klienta 
Jeśli chcesz przeprowadzić warsztaty z klientem, musisz poprosić klienta o zgodę na uczestnictwo w warsztatach. Po dodaniu lub otrzymaniu klienta będziesz mieć łącznie 30 dni na uzyskanie zgody.

Po dodaniu lub odmówieniu klienta zobaczysz, ile dni pozostało do uzyskania zgody w kolumnie stanu na **stronie** Klienci.
1. Wybierz **pozycję Wyzwolij zgodę** klienta w **kolumnie** Akcja. 
2. Podaj adres e-mail i informacje kontaktowe klienta wraz z informacjami kontaktowymi dla Twojej firmy. Następnie wybierz przycisk **Dalej**.

   :::image type="content" source="images/incentives/ask-consent-1.png" alt-text="Zrzut ekranu 1 z 2 przedstawiający sposób żądania zgody klienta." lightbox="images/incentives/ask-consent-1.png":::

3. Przejrzyj szczegóły i wybierz pozycję **Wyślij w celu wyrażenia zgody.** Do klienta zostanie wysłana wiadomość e-mail, aby zaakceptować lub odrzucić warsztaty.
   - Jeśli nie otrzymano zgody, możesz wysłać przypomnienie, klikając link **Wyślij** ponownie zgodę klienta w **kolumnie** Akcja.
   - Jeśli klient został nowo dodany, ale odmówi udziału w warsztatach lub nie odpowie w  ramach wymaganej osi czasu, nie będzie już wyświetlany na stronie Klienci dla tego zaangażowania.

   :::image type="content" source="images/incentives/ask-consent-2.png" alt-text="Zrzut ekranu 2 z 2 przedstawiający sposób żądania zgody klienta." lightbox="images/incentives/ask-consent-2.png":::

Gdy klient wyrazić zgodę, będziesz mieć 90 dni na przeprowadzenie warsztatów.

## <a name="next-steps"></a>Następne kroki
[Przesyłanie oświadczenia o warsztatach](/partner-center/mci-engagements-workshop)

[Omówienie zaangażowania mci i uprawnienia](/partner-center/mci-engagements)

[Użyj tych zasobów, aby rozpocząć pracę z zachętami](/partner-center/incentives-get-started-intro)

[Określanie uprawnień do programu zachęt](/partner-center/incentives-determined-your-program-eligibility)

[Rejestracja i zarządzanie użytkownikami w programie zachęt](/partner-center/incentives-enroll)