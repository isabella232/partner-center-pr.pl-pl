---
title: Jak potwierdzić, że klient zaakceptował Umowa z Klientem Microsoft do programu CSP
description: Dostawca rozwiązań w chmurze (CSP) partnerzy muszą potwierdzić akceptację przez klienta Umowa z Klientem Microsoft przed usługi firmy Microsoft dla klientów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ed3b888791dad1e875db64b7ccbe20e7b0a8b4bbd71fb7c83cc677ee2d5f2d3a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115680112"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Jak potwierdzić, że klient zaakceptował Umowa z Klientem Microsoft do programu CSP

**Odpowiednie role:** Administrator | Agent sprzedaży


Klienci mają dwie opcje dotyczące sposobu akceptowania Umowa z Klientem Microsoft.

**Opcja 1.** Potwierdzenie akceptacji klienta przez partnerów — partner może potwierdzić akceptację klienta przy użyciu interfejsu API lub zestawu SDK Partner Center lub za pośrednictwem Partner Center nawigacyjnego.

**Opcja 2.** Bezpośrednia akceptacja klienta — partner może zaprosić klienta za pośrednictwem adresu URL do przejrzenia i zaakceptowania umowy w centrum Administracja Microsoft 365 klienta.

## <a name="access-microsoft-customer-agreement-template"></a>Szablon Umowa z Klientem Microsoft dostępu

Najnowszą wersję szablonu aplikacji można pobrać ręcznie Umowa z Klientem Microsoft [tutaj.](https://aka.ms/customeragreement) Ta Umowa z Klientem Microsoft jest specyficzna dla kraju. Żądając szablonu Umowa z Klientem Microsoft, należy wybrać właściwy kraj na podstawie lokalizacji klienta.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opcja 1. Potwierdzenie akceptacji klienta w Partner Center

Partnerzy rozliczani bezpośrednio mogą potwierdzić akceptację klienta Umowa z Klientem Microsoft w Partner Center dla nowych i istniejących klientów. Odsprzedawcy pośredni nie mogą zaświadczenia w imieniu swoich klientów i muszą współpracować ze swoim dostawcą pośrednim, aby uzyskać ukończone zaświadczenia.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Potwierdzanie akceptacji przez klientów dla nowych klientów

Podczas tworzenia nowej dzierżawy klienta w Partner Center, należy wykonać następujące kroki, aby potwierdzić akceptację Umowa z Klientem Microsoft. Aby wykonać te kroki, musisz być agentem administratora lub agentem sprzedaży.

1. Wybierz **pozycję Klienci,** a następnie **pozycję Nowy klient.**

2. W **obszarze Informacje o** koncie wprowadź informacje dotyczące firmy i jej głównej osoby kontaktowej.

3. W **ramach umowy firmy Microsoft** zaznacz pole wyboru, aby zaświadczyć, że klient zaakceptował Umowa z Klientem Microsoft.

4. W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej daty na przyszłą datę.

5. Upewnij się, że wyświetlane informacje kontaktowe użytkownika podstawowego są poprawne. Jeśli jest niepoprawna, wybierz pozycję **Aktualizuj** i wprowadź dokładne informacje dotyczące osoby, która zaakceptowała umowę.

6. Wybierz **przycisk Dalej,** aby kontynuować tworzenie dzierżawy klienta.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nowy klient.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Potwierdzanie akceptacji przez klientów dla istniejących klientów

Aby to zrobić, musisz być agentem administratora lub agentem sprzedaży:

1. Wybierz pozycję **Klienci**. Znajdź i wybierz klienta.

2. Wybierz **pozycję Informacje o koncie.**

3. W **Umowa z Klientem Microsoft** wybierz pozycję **Zaktualizuj**.

4. Wprowadź **imię,** **nazwisko,** **adres** **e-mail i Telefon** (opcjonalnie) osoby, która zaakceptowała umowę. W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej daty na przyszłą datę.

5. Wybierz **pozycję Zapisz** i kontynuuj.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Istniejący klient.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Pobieranie potwierdzenia akceptacji przez klienta

Aby pobrać potwierdzenie, że istniejący klient zaakceptował Umowa z Klientem Microsoft, należy wykonać następujące kroki. Aby to zrobić, musisz być agentem administratora lub agentem sprzedaży.

1. Wybierz **pozycję Klienci,** a następnie znajdź i wybierz klienta, którego chcesz wyświetlić.

2. Wybierz **pozycję Informacje o koncie.**

3. W **ramach umowy klienta firmy Microsoft** sprawdź, czy ten klient dostarczył potwierdzenie lub nie.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Potwierdzanie akceptacji przez klientów przy użyciu Partner Center API/zestawu SDK

Możesz użyć Partner Center API/zestawu SDK, aby potwierdzić akceptację przez klienta Umowa z Klientem Microsoft. Aby uzyskać szczegółowe informacje na temat interfejsu API/zestawu SDK, zobacz:

- [Pobieranie metadanych umowy dla umowy klienta firmy Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Pobieranie potwierdzenia akceptacji przez klienta umowy klienta firmy Microsoft](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Pobierz link pobierania dla Umowa z Klientem Microsoft szablonu](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opcja 2. Akceptacja klienta w Administracja Microsoft 365 Center

Partnerzy mogą zapraszać nowych i istniejących klientów za pośrednictwem adresu URL w celu przejrzenia i zaakceptowania umowy w Administracja Microsoft 365 Center. W kilku następnych sekcjach opisano, jak:

- Utwórz nowego klienta i zaproś go do przejrzenia i zaakceptowania umowy.

- Zaproś nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i umowy.

- Zaproś istniejącego klienta do przejrzenia i zaakceptowania umowy.

>[!NOTE]
> Możesz użyć [Partner Center API/zestawu SDK,](/partner-center/develop/get-direct-sign-status-of-customer-agreement) aby uzyskać stan bezpośredniej akceptacji klienta Umowa z Klientem Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Tworzenie nowego klienta i zapraszanie klienta do przejrzenia i zaakceptowania umowy

Użyj poniższych kroków, aby utworzyć nowego klienta w Partner Center, a następnie zaproś go do przejrzenia i zaakceptowania Umowa z Klientem Microsoft w Administracja Microsoft 365 Center.

1. Na karcie **Customers (Klienci)** w Partner Center wybierz pozycję **Add customer (Dodaj klienta).**

2. W **obszarze Informacje o** koncie wprowadź informacje o nowym kliencie we wszystkich wymaganych polach, w tym nazwę firmy klienta i podstawowy kontakt.

3. W **obszarze Umowa z** Klientem wybierz pozycję Klient zostanie poproszony o **zaakceptowanie Umowa z Klientem Microsoft w Administracja Microsoft 365 Center.** Wypełnij wszystkie inne wymagane pola na stronie.

4. Wybierz **pozycję Dalej: Przejrzyj,** a następnie kontynuuj kroki tworzenia dzierżawy klienta. 

>[!NOTE] 
>Nowi klienci nie mogą dokonać zakupu, dopóki nie zaakceptują Umowa z Klientem Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Tworzenie nowego klienta.":::

5. Po osiągnięciu ekranu **Potwierdzenia** w przepływie pracy nowego klienta zapisz poświadczenia klienta. Te poświadczenia będą potrzebne później klientowi.

6. Poza Partner Center utwórz i wyślij wiadomość e-mail z zaproszeniem klienta do zaakceptowania Umowa z Klientem Microsoft w Administracja Microsoft 365 Center. Pamiętaj, aby w wiadomości e-mail uwzględnić następujące elementy:

   - Link do tego adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (wymagane jest zalogowanie)

   - Poświadczenia klienta zapisane w kroku 5.

7. Klient otrzyma wiadomość e-mail z zaproszeniem od partnera i wybierze adres [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Klient korzysta z Administracja Microsoft 365 Center przy użyciu podanych poświadczeń klienta.

9. Klient sprawdza to pole, aby zaakceptować umowę klienta firmy Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Zaproś nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i Umowa z Klientem Microsoft 

Skorzystaj z poniższych kroków, aby zaprosić nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i Umowa z Klientem Microsoft. 

1. Na karcie **Customers (Klienci)** Partner Center pozycję Request a reseller relationship link **(Zażądaj linku do relacji odsprzedawcy).** 

2. Zostanie wygenerowany automatyczny szablon wiadomości e-mail, w tym tekst i sparametryzowane adresy URL, które kierują klienta do centrum Administracja Microsoft 365 usługi.

3. Możesz dostosować automatycznie wygenerowany szablon wiadomości e-mail, a następnie wybrać pozycję **Kopiuj do schowka** lub **Otwórz w wiadomości e-mail.**

4. Użyj tego szablonu wiadomości e-mail, aby zaprosić klienta do **zaakceptowania** żądania relacji odsprzedawcy **i Umowa z Klientem Microsoft**. (Uwaga: W wiadomości e-mail z zaproszeniem upewnij się, że partner zawiera również adres URL, który został podany automatycznie, a także poświadczenia klienta, które zostały ostatnio utworzone).

   :::image type="content" source="images/mca/createrelationship.png" alt-text="utwórz relację.":::

5. Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika sparametryzowane adresy URL. 

6. Klient używa poświadczeń podanych w wiadomości e-mail, aby zalogować się do Administracja Microsoft 365 Center.

7. Klient sprawdza pole wyboru, aby zaakceptować relację **odsprzedawcy** **i Umowa z Klientem Microsoft**. 

8. W ramach tego samego adresu URL klient może wyświetlić skonsolidowaną listę różnych partnerów, z których pracuje. Może wybrać partnera, aby wyświetlić szczegóły.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Zaakceptuj umowę.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Zapraszanie istniejącego klienta do przejrzenia i zaakceptowania umowy

Skorzystaj z poniższych kroków, aby zaprosić istniejącego klienta do przejrzenia i zaakceptowania Umowa z Klientem Microsoft. 

1. Utwórz wiadomość e-mail klienta z osadzonym adresem URL z zaproszeniem klienta do zaakceptowania Umowa z Klientem Microsoft.

2. Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika [adres URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Klient wprowadza swoje poświadczenia w Administracja Microsoft 365 Center.

4. Klient sprawdza to pole, aby zaakceptować Umowa z Klientem Microsoft. 

5. Pod tym samym adresem URL klient może zobaczyć skonsolidowaną listę różnych partnerów, z których pracuje. Może wybrać partnera, aby wyświetlić szczegóły.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Klienta.":::

>[!NOTE]
>W niektórych scenariuszach klienci mogą nie być w stanie bezpośrednio zaakceptować Umowa z Klientem Microsoft. Aby dowiedzieć się więcej na temat tych sytuacji, przeczytaj dwa scenariusze, w których musisz zaświadczyć w imieniu klienta, poniżej.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dwa scenariusze, w których musisz zaświadczyć w imieniu klienta

Istnieją dwa scenariusze, w których klienci mogą nie być w stanie bezpośrednio zaakceptować Umowa z Klientem Microsoft w Administracja Microsoft 365 Center.

**Scenariusz 1.** Istniejący klient kupił dowolne z następujących produktów w ramach istniejącej relacji partnerskiej: oferty, subskrypcje oprogramowania lub oprogramowania, wystąpienia zarezerwowane lub plan platformy Azure. Klient próbuje teraz dokonać nowego zakupu (z wyjątkiem automatycznego odnawiania). Gdy klient kliknie adres URL, otrzyma komunikat "Skontaktuj się z partnerem, aby potwierdzić akceptację Umowa z Klientem Microsoft".  

**Aby rozwiązać** ten problem: musisz atestować w imieniu klienta.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Zrzut ekranu Administracja Microsoft 365 Centrum z prośbą o sprosenie się z partnerem w celu potwierdzenia akceptacji Umowa z Klientem Microsoft.":::

**Scenariusz 2.** Istniejący klient kupił dowolną z następujących ofert, subskrypcji oprogramowania i oprogramowania, wystąpień zarezerwowanych i planu platformy Azure. Klient próbuje teraz dokonać nowego zakupu u nowego partnera.

Gdy klient kliknie adres URL w centrum Administracja Microsoft 365, aby zaakceptować nową relację z partnerem i umowę, otrzyma komunikat "Skontaktuj się z partnerem, aby potwierdzić akceptację Umowa z Klientem Microsoft".  

**Aby rozwiązać** ten problem: musisz atestować w imieniu klienta.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Potwierdzanie, że klient zaakceptował umowę

Jeśli spróbujesz utworzyć nowe zamówienie dla istniejącego klienta, który nie został jeszcze potwierdzony, zostanie wyświetlony monit o potwierdzenie. Użyj poniższej procedury w tym celu.

1. Wprowadź **imię,** **nazwisko,** **adres** e-mail i **Telefon** (opcjonalnie) użytkownika, który zaakceptował umowę.

2. W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej daty na przyszłą datę.

3. Wybierz przycisk **Zapisz i kontynuuj**. 

## <a name="next-steps"></a>Następne kroki

- [Weryfikowanie lub aktualizowanie informacji o profilu firmy](update-your-partner-profile.md)
- [Umowy z Klientem Microsoft (według regionu, języka)](Agreements.md)
