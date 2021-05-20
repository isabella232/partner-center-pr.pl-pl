---
title: Jak potwierdzić, że klient zaakceptował Umowa z Klientem Microsoft programu CSP
description: Dostawca rozwiązań w chmurze (CSP) partnerzy muszą potwierdzić akceptację przez klienta Umowa z Klientem Microsoft przed zamówieniem usługi firmy Microsoft dla klientów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: c75f129ae5a0755833462138f60901cc7ff36732
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148520"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Jak potwierdzić, że klient zaakceptował Umowa z Klientem Microsoft programu CSP

**Odpowiednie role:** Agent administracyjny | Agent sprzedaży


Klienci mają dwie opcje dotyczące sposobu akceptowania Umowa z Klientem Microsoft.

**Opcja 1:** Potwierdzenie akceptacji klienta przez partnera — partner może potwierdzić akceptację klienta przy użyciu interfejsu API lub zestawu SDK Partner Center lub za pośrednictwem pulpitu Partner Center nawigacyjnego.

**Opcja 2:** Akceptacja bezpośrednia klienta — partner może zaprosić klienta za pośrednictwem adresu URL w celu przejrzenia i zaakceptowania umowy w Microsoft 365 Administracyjnego.

## <a name="access-microsoft-customer-agreement-template"></a>Szablon Umowa z Klientem Microsoft dostępu

Najnowszą wersję szablonu aplikacji można pobrać ręcznie Umowa z Klientem Microsoft [tutaj.](https://aka.ms/customeragreement) Ta Umowa z Klientem Microsoft jest specyficzna dla kraju. Podczas żądania Umowa z Klientem Microsoft szablonu należy wybrać właściwy kraj na podstawie lokalizacji klienta.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opcja 1. Potwierdzanie akceptacji przez klientów w Partner Center

Partnerzy rozliczani bezpośrednio mogą potwierdzić akceptację klientów Umowa z Klientem Microsoft w Partner Center dla nowych i istniejących klientów. Odsprzedawcy pośredni nie mogą poświadczać w imieniu swoich klientów i muszą współpracować ze swoim dostawcą pośrednim, aby uzyskać ukończone zaświadczenia.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Potwierdzanie akceptacji przez klientów dla nowych klientów

Podczas tworzenia nowej dzierżawy klienta w Partner Center, należy wykonać następujące kroki, aby potwierdzić akceptację Umowa z Klientem Microsoft. Aby wykonać te kroki, musisz być agentem administracyjnym lub agentem sprzedaży.

1. Wybierz **pozycję Klienci,** a następnie **pozycję Nowy klient.**

2. W **obszarze Informacje o** koncie wprowadź informacje dotyczące firmy i jej głównej osoby kontaktowej.

3. W **ramach umowy firmy Microsoft** zaznacz pole wyboru, aby zaświadczyć, że klient zaakceptował Umowa z Klientem Microsoft.

4. W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej daty na przyszłą datę.

5. Upewnij się, że wyświetlane informacje kontaktowe użytkownika podstawowego są poprawne. Jeśli jest niepoprawna, wybierz pozycję **Aktualizuj** i wprowadź dokładne informacje dotyczące osoby, która zaakceptowała umowę.

6. Wybierz **przycisk Dalej,** aby kontynuować tworzenie dzierżawy klienta.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nowy klient":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Potwierdzanie akceptacji przez klientów dla istniejących klientów

Aby to zrobić, musisz być agentem administratora lub agentem sprzedaży:

1. Wybierz pozycję **Klienci**. Znajdź i wybierz klienta.

2. Wybierz **pozycję Informacje o koncie.**

3. W **Umowa z Klientem Microsoft** wybierz pozycję **Zaktualizuj**.

4. Wprowadź **imię,** **nazwisko,** adres **e-mail** i numer telefonu  (opcjonalnie) osoby, która zaakceptowała umowę. W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej daty na przyszłą datę.

5. Wybierz **pozycję Zapisz** i kontynuuj.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Istniejący klient":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Pobieranie potwierdzenia akceptacji przez klienta

Aby pobrać potwierdzenie, że istniejący klient zaakceptował Umowa z Klientem Microsoft, należy wykonać następujące kroki. Aby to zrobić, musisz być agentem administratora lub agentem sprzedaży.

1. Wybierz **pozycję Klienci,** a następnie znajdź i wybierz klienta, którego chcesz wyświetlić.

2. Wybierz **pozycję Informacje o koncie.**

3. W **ramach umowy klienta firmy Microsoft** sprawdź, czy potwierdzenie nie zostało dostarczone przez tego klienta.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Potwierdzanie akceptacji przez klientów przy użyciu Partner Center API/SDK

Możesz użyć Partner Center API/zestawu SDK, aby potwierdzić akceptację przez klienta Umowa z Klientem Microsoft. Aby uzyskać szczegółowe informacje na temat interfejsu API/zestawu SDK, zobacz:

- [Pobieranie metadanych umowy dla umowy klienta firmy Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Pobieranie potwierdzenia akceptacji przez klienta umowy klienta firmy Microsoft](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Uzyskiwanie linku pobierania dla szablonu Umowa z Klientem Microsoft szablonu](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opcja 2. Akceptacja klienta w Microsoft 365 administracyjnym

Partnerzy mogą zapraszać nowych i istniejących klientów za pośrednictwem adresu URL do przejrzenia i zaakceptowania umowy w Microsoft 365 Administracyjnego. W kilku następnych sekcjach podano, jak:

- Utwórz nowego klienta i zaproś go do przejrzenia i zaakceptowania umowy.

- Zaproś nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i umowy.

- Zaproś istniejącego klienta do przejrzenia i zaakceptowania umowy.

>[!NOTE]
> Możesz użyć [Partner Center API/zestawu SDK,](/partner-center/develop/get-direct-sign-status-of-customer-agreement) aby uzyskać stan bezpośredniej akceptacji klienta dla Umowa z Klientem Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Tworzenie nowego klienta i zapraszanie go do przejrzenia i zaakceptowania umowy

Użyj poniższych kroków, aby utworzyć nowego klienta w Partner Center następnie zaprosić go do przejrzenia i zaakceptowania Umowa z Klientem Microsoft w Microsoft 365 administracyjnym.

1. Na karcie **Customers (Klienci)** w Partner Center wybierz **pozycję Add customer (Dodaj klienta).**

2. W **obszarze Informacje o** koncie wprowadź informacje o nowym kliencie we wszystkich wymaganych polach, w tym nazwę firmy klienta i podstawowy kontakt.

3. W **obszarze Umowa z** Klientem wybierz pozycję Klient zostanie poproszony o **zaakceptowanie Umowa z Klientem Microsoft w Microsoft 365 administracyjnym.** Wypełnij wszystkie inne wymagane pola na stronie.

4. Wybierz **pozycję Dalej: Przejrzyj,** a następnie kontynuuj kroki tworzenia dzierżawy klienta. 

>[!NOTE] 
>Nowi klienci nie mogą dokonać zakupu, dopóki nie zaakceptują Umowa z Klientem Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Tworzenie nowego klienta":::

5. Po osiągnięciu ekranu **Potwierdzenie** w przepływie pracy nowego klienta zapisz poświadczenia klienta. Te poświadczenia trzeba będzie przekazać później klientowi.

6. Poza Partner Center utwórz i wyślij wiadomość e-mail z zaproszeniem klienta do zaakceptowania Umowa z Klientem Microsoft w Microsoft 365 Administracyjnego. Pamiętaj, aby uwzględnić następujące elementy w wiadomości e-mail:

   - Link do tego adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (wymagane jest zalogowanie)

   - Poświadczenia klienta zapisane w kroku 5.

7. Klient otrzyma wiadomość e-mail z zaproszeniem od partnera i wybierze adres [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Klient logowania się Microsoft 365 administracyjnym przy użyciu podanych poświadczeń klienta.

9. Klient sprawdza to pole, aby zaakceptować umowę klienta firmy Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Zaproś nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i Umowa z Klientem Microsoft 

Użyj poniższych kroków, aby zaprosić nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i Umowa z Klientem Microsoft. 

1. Na karcie **Customers (Klienci)** w Partner Center wybierz link **Request a reseller relationship (Zażądaj relacji odsprzedawcy).** 

2. Zostanie wygenerowany automatyczny szablon wiadomości e-mail, w tym tekst i sparametryzowane adresy URL, które kierują klienta do centrum Microsoft 365 administracyjnego.

3. Możesz dostosować automatycznie wygenerowany szablon wiadomości e-mail, a następnie wybrać pozycję **Kopiuj do schowka** lub **Otwórz w wiadomości e-mail.**

4. Użyj tego szablonu wiadomości e-mail, aby zaprosić klienta do **zaakceptowania** żądania relacji odsprzedawcy **i Umowa z Klientem Microsoft**. (Uwaga: w wiadomości e-mail z zaproszeniem upewnij się, że partner zawiera również adres URL, który został automatycznie podany, a także poświadczenia klienta, które zostały ostatnio utworzone).

   :::image type="content" source="images/mca/createrelationship.png" alt-text="tworzenie relacji":::

5. Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika sparametryzowane adresy URL. 

6. Klient używa poświadczeń podanych w wiadomości e-mail, aby zalogować się Microsoft 365 Centrum administracyjnego.

7. Klient sprawdza pole wyboru, aby zaakceptować relację **odsprzedawcy** **i Umowa z Klientem Microsoft**. 

8. W ramach tego samego adresu URL klient może wyświetlić skonsolidowaną listę różnych partnerów, z których pracuje. Może wybrać partnera, aby wyświetlić szczegóły.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Zaakceptowanie umowy":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Zapraszanie istniejącego klienta do przejrzenia i zaakceptowania umowy

Skorzystaj z poniższych kroków, aby zaprosić istniejącego klienta do przejrzenia i zaakceptowania Umowa z Klientem Microsoft. 

1. Utwórz wiadomość e-mail klienta z osadzonym adresem URL z zaproszeniem klienta do zaakceptowania Umowa z Klientem Microsoft.

2. Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika [adres URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Klient wprowadza swoje poświadczenia w Microsoft 365 Administracyjnego.

4. Klient sprawdza to pole, aby zaakceptować Umowa z Klientem Microsoft. 

5. Pod tym samym adresem URL klient może zobaczyć skonsolidowaną listę różnych partnerów, z których pracuje. Może wybrać partnera, aby wyświetlić szczegóły.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Klienta":::

>[!NOTE]
>W niektórych scenariuszach klienci mogą nie być w stanie bezpośrednio zaakceptować Umowa z Klientem Microsoft. Aby dowiedzieć się więcej na temat tych sytuacji, przeczytaj dwa scenariusze, w których musisz zaświadczyć w imieniu klienta, poniżej.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dwa scenariusze, w których musisz zaświadczyć w imieniu klienta

Istnieją dwa scenariusze, w których klienci mogą nie być w stanie bezpośrednio zaakceptować Umowa z Klientem Microsoft w Microsoft 365 administracyjnym.

**Scenariusz 1.** Istniejący klient kupił dowolne z następujących produktów w ramach istniejącej relacji partnerskiej: oferty, subskrypcje oprogramowania lub oprogramowania, wystąpienia zarezerwowane lub plan platformy Azure. Klient próbuje teraz dokonać nowego zakupu (z wyjątkiem automatycznego odnawiania). Gdy klient kliknie adres URL, otrzyma komunikat "Skontaktuj się z partnerem, aby potwierdzić akceptację Umowa z Klientem Microsoft".  

**Aby rozwiązać** ten problem: musisz atestować w imieniu klienta.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Zrzut ekranu Microsoft 365 Centrum administracyjnego z prośbą o sprosenie się z partnerem w celu potwierdzenia akceptacji Umowa z Klientem Microsoft.":::

**Scenariusz 2.** Istniejący klient kupił dowolną z następujących ofert, subskrypcji oprogramowania i oprogramowania, wystąpień zarezerwowanych i planu platformy Azure. Klient próbuje teraz dokonać nowego zakupu u nowego partnera.

Gdy klient kliknie adres URL w centrum administracyjnym Microsoft 365, aby zaakceptować nową relację z partnerem i umowę, otrzyma komunikat "Skontaktuj się z partnerem, aby potwierdzić akceptację Umowa z Klientem Microsoft".  

**Aby rozwiązać** ten problem: musisz atestować w imieniu klienta.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Potwierdzanie, że klient zaakceptował umowę

Jeśli spróbujesz utworzyć nowe zamówienie dla istniejącego klienta, który nie został jeszcze potwierdzony, zostanie wyświetlony monit o potwierdzenie. Użyj poniższej procedury w tym celu.

1. Wprowadź **imię,** **nazwisko,** adres **e-mail** i **numer** telefonu (opcjonalnie) użytkownika, który zaakceptował umowę.

2. W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej daty na przyszłą datę.

3. Wybierz przycisk **Zapisz i kontynuuj**. 

## <a name="next-steps"></a>Następne kroki

- [Weryfikowanie lub aktualizowanie informacji o profilu firmy](update-your-partner-profile.md)
- [Umowy z Klientem Microsoft (według regionu, języka)](Agreements.md)
