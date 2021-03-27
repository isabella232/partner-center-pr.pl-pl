---
title: Jak potwierdzić, że klient zaakceptował umowę klienta firmy Microsoft do programu CSP
description: Partnerzy dostawcy rozwiązań w chmurze (CSP) muszą potwierdzić akceptację przez klienta umowy klienta firmy Microsoft przed zamawianiem usług firmy Microsoft dla klientów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633782"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Jak potwierdzić, że klient zaakceptował umowę klienta firmy Microsoft do programu CSP

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży


Klienci mogą korzystać z dwóch opcji zaakceptowania umowy klienta firmy Microsoft.

**Opcja 1**: zaświadczanie partnera dotyczącego akceptacji przez klienta może potwierdzić akceptację klienta przy użyciu interfejsu API/zestawu SDK Centrum partnerskiego lub pulpitu nawigacyjnego Centrum partnerskiego.

**Opcja 2**: klient bezpośredni akceptacji — partner może zaprosić klienta za pośrednictwem adresu URL w celu przejrzenia i zaakceptowania umowy w centrum administracyjnym Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Dostęp do szablonu umowy klienta firmy Microsoft

Możesz ręcznie pobrać najnowszą wersję szablonu umowy klienta firmy Microsoft z tego [miejsca](https://aka.ms/customeragreement). Umowa dla klientów firmy Microsoft jest specyficzna dla kraju. Podczas żądania szablonu umowy klienta firmy Microsoft upewnij się, że wybrano właściwy kraj na podstawie lokalizacji klienta.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opcja 1: potwierdzenie akceptacji przez klienta w centrum partnerskim

Bezpośredni partnerzy Bill mogą potwierdzić akceptację klienta umowy klienta firmy Microsoft w centrum partnerskim dla nowych i istniejących klientów. Pośredni odsprzedawcy nie mogą zaświadczać swoich klientów i muszą współpracować z dostawcami pośrednimi w celu uzyskania zaświadczania.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Potwierdź akceptację klienta dla nowych klientów

Podczas tworzenia nowej dzierżawy klienta w centrum partnerskim wykonaj następujące kroki, aby potwierdzić akceptację umowy klienta firmy Microsoft przez klienta. Aby wykonać te kroki, musisz być agentem administracyjnym lub agentem sprzedaży.

1. Wybierz pozycję **klienci**, a następnie **Nowy klient**.

2. W obszarze **Informacje o koncie** wprowadź informacje dotyczące firmy i jej głównej osoby kontaktowej.

3. W obszarze **Umowa Microsoft** wybierz pole, aby zatwierdzić, że klient zaakceptował umowę klienta firmy Microsoft.

4. W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej wartości na datę przyszłą.

5. Upewnij się, że wyświetlane informacje kontaktowe użytkownika podstawowego są poprawne. Jeśli jest to nieprawidłowe, wybierz pozycję **Aktualizuj** i wprowadź dokładne informacje dla osoby, która zaakceptował umowę.

6. Wybierz pozycję **dalej** , aby kontynuować tworzenie dzierżawy klienta.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nowy klient":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Potwierdzenie akceptacji przez klienta dla istniejących klientów

Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży:

1. Wybierz pozycję **Klienci**. Znajdź i wybierz klienta.

2. Wybierz pozycję **Informacje o koncie**.

3. W obszarze **Umowa klienta firmy Microsoft** wybierz pozycję **Aktualizuj**.

4. Wprowadź **imię** i **nazwisko, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) osoby, która zaakceptował umowę. W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej wartości na datę przyszłą.

5. Wybierz pozycję **Zapisz** i Kontynuuj.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Istniejący klient":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Pobierz potwierdzenie akceptacji klienta

Aby uzyskać potwierdzenie, że istniejący klient zaakceptował umowę klienta firmy Microsoft, wykonaj następujące czynności. Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.

1. Wybierz pozycję **klienci**, a następnie Znajdź i wybierz klienta, który ma zostać wyświetlony.

2. Wybierz pozycję **Informacje o koncie**.

3. W obszarze **Umowa klienta firmy Microsoft** Sprawdź, czy jest to potwierdzenie czy nie zostało dostarczone przez tego klienta.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Potwierdzenie akceptacji klienta przy użyciu interfejsu API/zestawu SDK Centrum partnerskiego

Za pomocą interfejsu API/zestawu SDK Centrum partnerskiego można potwierdzić akceptację umowy klienta firmy Microsoft przez klienta. Aby uzyskać szczegółowe informacje na temat interfejsu API/SDK, zobacz:

- [Pobieranie metadanych umowy dla umowy klienta firmy Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Pobieranie potwierdzenia akceptacji przez klienta umowy klienta firmy Microsoft](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Pobierz link do pobierania dla szablonu umowy klienta firmy Microsoft](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opcja 2: akceptacja klienta w centrum administracyjnym Microsoft 365

Partnerzy mogą zapraszać nowych i istniejących klientów za pośrednictwem adresu URL, aby przejrzeć i zaakceptować umowę w centrum administracyjnym Microsoft 365. W następnych sekcjach pokazano, jak:

- Utwórz nowego klienta i zaproś klienta o sprawdzenie i zaakceptowanie umowy.

- Zaproś nowego klienta o sprawdzenie i zaakceptowanie relacji odsprzedawcy oraz umowy.

- Zaproś istniejącego klienta o sprawdzenie i zaakceptowanie umowy.

>[!NOTE]
> Możesz użyć [interfejsu API/SDK Centrum partnerskiego](/partner-center/develop/get-direct-sign-status-of-customer-agreement) , aby uzyskać stan bezpośredniej akceptacji umowy klienta firmy Microsoft przez klienta.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Utwórz nowego klienta i zaproś klienta o sprawdzenie i zaakceptowanie umowy

Wykonaj następujące kroki, aby utworzyć nowego klienta w centrum partnerskim, a następnie Zaproś go o sprawdzenie i zaakceptowanie umowy klienta firmy Microsoft w centrum administracyjnym Microsoft 365.

1. Na karcie **klienci** w centrum partnerskim wybierz pozycję **Dodaj klienta**.

2. W obszarze **Informacje o koncie** wprowadź informacje o nowym kliencie we wszystkich wymaganych polach, w tym nazwę firmy klienta i kontakt podstawowy.

3. W obszarze **Umowa klienta** wybierz pozycję **klient z prośbą o zaakceptowanie umowy klienta firmy Microsoft w centrum administracyjnym Microsoft 365**. Wypełnij wszystkie inne wymagane pola na stronie.

4. Wybierz pozycję **Dalej: Przejrzyj** następnie kontynuuj kroki, aby utworzyć dzierżawę klienta. 

>[!NOTE] 
>Nowi klienci nie mogą dokonać zakupu, dopóki nie zaakceptują umowy klienta firmy Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Utwórz nowego klienta":::

5. Po dojściu do ekranu **potwierdzenia** w nowym przepływie pracy klienta Zapisz poświadczenia klienta. Musisz podać te poświadczenia klientom później.

6. Na zewnątrz Centrum partnerskiego Utwórz i Wyślij wiadomość e-mail z zaproszeniem klienta, aby zatwierdzić umowę klienta firmy Microsoft w centrum administracyjnym Microsoft 365. Upewnij się, że te elementy zostały uwzględnione w wiadomości e-mail:

   - Link do tego [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (wymagane logowanie)

   - Poświadczenia klienta zapisane w kroku 5.

7. Klient otrzyma wiadomość e-mail z zaproszeniem od partnera i wybierze [adres URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Klient loguje się do centrum administracyjnego Microsoft 365 przy użyciu podanych poświadczeń klienta.

9. Klient sprawdza pole, aby zaakceptować umowę klienta firmy Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Zaproś nowego klienta o sprawdzenie i zaakceptowanie relacji odsprzedawcy oraz umowy klienta firmy Microsoft 

Wykonaj następujące kroki, aby zaprosić nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy oraz umowy klienta firmy Microsoft. 

1. Na karcie **klienci** w centrum partnerskim wybierz pozycję **Żądaj linku relacji odsprzedawcy** . 

2. Zostanie wygenerowany automatyczny szablon wiadomości e-mail, w tym tekst i sparametryzowany adres URL kierujący klienta do centrum administracyjnego Microsoft 365.

3. Można dostosować automatycznie wygenerowany szablon wiadomości e-mail, a następnie wybrać opcję **Kopiuj do schowka** lub **otworzyć w wiadomości e-mail**.

4. Ten szablon wiadomości e-mail zaprasza klienta, aby akceptował żądanie dotyczące **relacji odsprzedawcy** oraz **umowę klienta firmy Microsoft**. (Uwaga: w wiadomości e-mail z zaproszeniem upewnij się, że partner zawiera również adres URL, który został podany automatycznie, oraz poświadczenia klienta, które zostały ostatnio utworzone).

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Utwórz relację":::

5. Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika sparametryzowany adres URL. 

6. Klient korzysta z poświadczeń podanych w wiadomości e-mail w celu zalogowania się do centrum administracyjnego Microsoft 365.

7. Klient sprawdza pole, aby zaakceptować **relację odsprzedawcy** oraz **umowę klienta firmy Microsoft**. 

8. W ramach tego samego adresu URL klient może zobaczyć skonsolidowaną listę różnych partnerów, z którymi pracują. Mogą wybrać partnera, aby wyświetlić szczegóły.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Zaakceptowanie umowy":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Zaproś istniejącego klienta o sprawdzenie i zaakceptowanie umowy

Wykonaj następujące kroki, aby zaprosić istniejącego klienta do przejrzenia i zaakceptowania umowy klienta firmy Microsoft. 

1. Utwórz adres e-mail klienta z osadzonym adresem URL, który zaprasza klienta, aby zaakceptował umowę klienta firmy Microsoft.

2. Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika [adres URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Klient wprowadza swoje poświadczenia do centrum administracyjnego Microsoft 365.

4. Klient sprawdza pole, aby zaakceptować umowę klienta firmy Microsoft. 

5. W ramach tego samego adresu URL klient może zobaczyć skonsolidowaną listę różnych partnerów, z którymi pracują. Mogą wybrać partnera, aby wyświetlić szczegóły.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Dział":::

>[!NOTE]
>W niektórych scenariuszach klienci mogą nie być w stanie bezpośrednio zaakceptować umowy klienta firmy Microsoft. Aby dowiedzieć się więcej na temat tych sytuacji, przeczytaj dwa scenariusze, w których musisz zalogować się w imieniu klienta poniżej.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dwa scenariusze, w których należy zaświadczać o swoim imieniu klienta

Istnieją dwa scenariusze, w których klienci mogą nie być w stanie bezpośrednio zaakceptować umowy klienta firmy Microsoft w centrum administracyjnym Microsoft 365.

**Scenariusz 1**: istniejący klient kupił dowolne z następujących elementów za pomocą istniejącej relacji partnera: oferty, oprogramowania lub subskrypcji oprogramowania, wystąpień zarezerwowanych lub planu platformy Azure. Klient próbuje teraz dokonać nowego zakupu (z wyjątkiem autoodnawiania). Gdy klient kliknie ten adres URL, otrzyma komunikat "Skontaktuj się z partnerem w celu potwierdzenia akceptacji umowy klienta firmy Microsoft".  

**Aby rozwiązać ten problem**: należy zaświadczać o imieniu klienta.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Zrzut ekranu przedstawiający stronę centrum administracyjnego Microsoft 365 z prośbą o skontaktowanie się z partnerem w celu potwierdzenia akceptacji umowy klienta firmy Microsoft.":::

**Scenariusz 2**. istniejący klient zakupił jedną z następujących ofert, subskrypcji oprogramowania i oprogramowania, wystąpień zarezerwowanych oraz planu platformy Azure. Klient podejmie teraz próbę dokonania nowego zakupu u nowego partnera.

Gdy klient kliknie adres URL, aby Microsoft 365 centrum administracyjnego w celu zaakceptowania nowej relacji partnera i umowy, otrzyma komunikat "Skontaktuj się z partnerem w celu potwierdzenia akceptacji umowy klienta firmy Microsoft".  

**Aby rozwiązać ten problem**: należy zaświadczać o imieniu klienta.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Potwierdź, że klient zaakceptował umowę

Jeśli spróbujesz utworzyć nowe zamówienie dla istniejącego klienta, który nie został wcześniej potwierdzony, zostanie wyświetlony monit o ukończenie potwierdzenia. Użyj poniższej procedury w tym celu.

1. Wprowadź **imię** **, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) użytkownika, który zaakceptował umowę.

2. W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej wartości na datę przyszłą.

3. Wybierz przycisk **Zapisz i kontynuuj**. 

## <a name="next-steps"></a>Następne kroki

- [Weryfikowanie lub aktualizowanie informacji o profilu firmy](update-your-partner-profile.md)
- [Umowy z Klientem Microsoft (według regionu, języka)](Agreements.md)
