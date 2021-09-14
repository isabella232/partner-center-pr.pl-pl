---
title: Wypłaty i profile podatkowe w Centrum partnerskim
ms.topic: how-to
ms.date: 04/15/2021
description: Utwórz profil wypłaty i profil podatkowy oraz zarządzaj nimi, aby uzyskać płatności za pracę z zachętami. Obejmuje tworzenie i używanie różnych profilów oraz zarządzanie nimi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248123"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Tworzenie profilów wypłat i profilów podatkowych zachęt i zarządzanie nimi w Partner Center

**Odpowiednie role:** Zachęty dla administratorów | Konto administratora | Administrator globalny

Aby można było otrzymać płatność z tytułu programów zachęt dla konkretnej lokalizacji MPN, należy ukończyć rejestrację, dokonując skojarzenia prawidłowego profilu wypłaty i profilu podatkowego z programem i lokalizacją MPN. Firma Microsoft będzie korzystać z tego profilu wypłaty i profilu podatkowego w celu realizacji płatności. W zależności od zasad programu zachęt może być możliwe wykorzystanie elektronicznego przelewu bankowego lub noty kredytowej przy płatności. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Role, waluty i wiele programów zachęt firmy Microsoft

Ważne jest, aby zrozumieć poniższe informacje przed rozpoczęciem pracy z profilem wypłaty i profilem podatkowym.

### <a name="roles-and-permissions"></a>Role i uprawnienia

Musisz być administratorem zachęt, aby wprowadzać informacje bankowe i podatkowe dla płatności zachęt. Jeśli jesteś administratorem mpn/konta, możesz przypisać siebie i/lub współpracownika jako administratora zachęt.

Jeśli musisz poprosić o uprawnienia administratora zachęt, skontaktuj się z administratorem MPN lub administratorem globalnym. Aby dowiedzieć się, kto w firmie ma te role, należy zalogować się do [pulpitu Partner Center nawigacyjnego.](https://partner.microsoft.com/dashboard/) Na **ikonie Ustawienia** w prawym górnym rogu wybierz pozycję **Zarządzanie użytkownikami,** a następnie odfiltruj pozycję Administrator globalny.

Zachęty Użytkownicy mogą wyświetlać zarobki zachęt oraz szczegóły płatności i raporty, ale nie mogą edytować danych bankowych i podatkowych.

### <a name="choose-your-disbursement-currency"></a>Wybierz walutę wydatków

Płatności zachęt są dokonywane w walucie wybranej podczas konfigurowanie profilu płatności. Płatności będą obliczane przy użyciu kursu wymiany ustawionego co miesiąc przez firmę Microsoft. Ponosisz odpowiedzialność za wszelkie zmiany wartości spowodowane wybraną walutą.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Używanie różnych profilów dla różnych programów firmy Microsoft

Jeśli Twoja firma jest zarejestrowanych w wielu programach zachęt, możesz użyć tego samego konta płatności dla wszystkich z nich lub wybrać używanie różnych kont płatności dla różnych programów.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Tworzenie profilów wypłat i profilów podatkowych oraz zarządzanie nimi w Partner Center

W poniższych sekcjach przedstawiono proces tworzenia profilów płatności i profilów podatkowych oraz zarządzania nimi w Partner Center.

>[!IMPORTANT]
>Musisz być administratorem zachęty do tworzenia profilów płatności i profilów podatkowych oraz zarządzania nimi w Partner Center. Role zachęt muszą być przypisane do każdej lokalizacji MPN w ramach każdego programu zachęt. Aby uzyskać więcej informacji na temat dodawania administratorów zachęt w Partner Center, zobacz [Tworzenie kont użytkowników.](create-user-accounts-and-set-permissions.md)

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Uzyskaj dostęp do sekcji wypłaty i podatku w Partner Center

1. Zaloguj się do [pulpitu Partner Center nawigacyjnego](https://partner.microsoft.com/dashboard/) przy użyciu konta Azure Active Directory (Azure AD) (konta firmowego) lub odpowiedniego adresu e-mail, jeśli został przypisany.

   - W ramach jednego konta usługi Azure AD można zarejestrować wiele domen. Skontaktuj się z administratorem globalnym, aby określić, które domeny są skojarzone.
   - Jeśli możesz zalogować się tylko przy użyciu domeny i potrzebujesz dodatkowych domen, skontaktuj się z administratorem konta, aby dodać dodatkowe domeny @onmicrosoft.com do konta usługi Azure AD.
   - Jeśli zostanie wyświetlony monit  o wybranie konta służbowego lub osobistego, wybierz pozycję Konto **służbowe.**

2. Wybierz ikonę koła zębatego, aby **otworzyć menu Ustawienia, a** następnie wybierz pozycję Ustawienia **konta.**

3. W menu **Ustawień konta** wybierz pozycję **Wypłata i podatek.**

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Przypisywanie profilów wypłat i profilów podatkowych do poszczególnych programów

1. Zaloguj się na Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard/)a następnie wybierz ikonę koła zębatego, aby otworzyć **Ustawienia** menu. 

2. Wybierz **pozycję Ustawienia konta,** rozwiń **sekcję Wypłata i podatek,** a następnie wybierz **pozycję Przypisanie wypłaty i profilu podatkowego.** 
   
   Zostanie wyświetlona lista programów. Wybierz strzałkę obok programu, aby wyświetlić szczegóły profilu. 

3. Z menu **rozwijanego** Profil podatkowy wybierz profil podatkowy lub wybierz opcję utworzenia nowego profilu. Po wybraniu opcji utworzenia nowego profilu nastąpi odpowiednie przekierowanie.  Wybierz **pozycję Kontynuuj** w oknie podręcznym. Poniżej przedstawiono proces tworzenia nowego profilu podatkowego.

4. Wybierz **pozycję Payment method (Metoda płatności).**

   - Jeśli jako formę płatności wybrano opcję **Elektroniczne przelewy** bankowe, wybierz wybrany profil płatności lub wybierz opcję utworzenia nowego profilu. Po wybraniu opcji utworzenia nowego profilu nastąpi odpowiednie przekierowanie. Wybierz pozycję Kontynuuj w oknie podręcznym. Poniżej przedstawiono proces tworzenia nowego profilu płatności.

   - Jeśli jako formę płatności **wybrano** notę kredytową, ukończ weryfikację. Potwierdza to, że numer SAP, do którego się odwołujesz, należy do Twojej organizacji.

    >[!NOTE]
    >Jeśli na liście znajduje się wiele jednostek biznesowych firmy Microsoft, należy wybrać profil płatności dla każdej jednostki.

    >[!NOTE]
    >Dostępność formy płatności zależy od reguł programu zachęt.

    - Jeśli identyfikator MPN Twojej lokalizacji jest opłacany przez lokalny podmiot zależny firmy Microsoft za określony program zachęt i zezwala na notę kredytową LRD (dystrybutor ograniczonego ryzyka) jako formę płatności, Twój profil płatności zostanie wstępnie wypełniony metodą płatności LRD Credit Note. W wierszu formy płatności za kartę kredytową LRD dla odpowiedniego  programu zachęt i identyfikatora MPN lokalizacji w sekcji profilu płatności zostanie wyświetlony stan **Wymagane** potwierdzenie lub weryfikacja.
    
       Wybierz **pozycję Weryfikacja, która** jest potrzebna, aby potwierdzić i zweryfikować szczegóły identyfikatora dzierżawy dostawcy CSP skojarzone z lokalizacją MPN i formy płatności w celu otrzymania płatności za pomocą faktury kredytowej. W **oknie dialogowym Szczegóły faktury** kredytowej sprawdź i sprawdź, czy podany identyfikator dzierżawy i podane szczegóły dzierżawy programu CSP są poprawne. Jeśli zostanie wyświetlony więcej niż jeden identyfikator dzierżawy, starannie wybierz identyfikator dzierżawy CSP, dla którego chcesz otrzymywać płatności. Następnie wybierz pozycję **Potwierdź,** aby potwierdzić, że szczegóły twojej firmy są poprawne, i że płatność zachęty powinna zostać wykonana dla wybranego identyfikatora dzierżawy dostawcy CSP.
 
      Jeśli stan ma stan **Potwierdzony,** przypisanie identyfikatora dzierżawy CSP zostało ukończone i nie są wymagane żadne dalsze działania. Możesz nadal wybrać pozycję Potwierdzone, aby wyświetlić szczegóły przypisania.
   
      W krajach, w których partnerzy jawnie żądają zastosowania zwolnienia z podatku, istnieje możliwość zastosowania zwolnienia z podatku obok profilu podatkowego w sekcji profilu podatkowego programu zachęt i lokalizacji MPN. Zaznaczenie tego pola spowoduje zastosowanie korzyści wynikających ze zwolnienia z podatku do faktury kredytowej zachęty. 
   
      Obecnie metoda płatności LRD Credit Note jest dostępna tylko dla partnerów z Australii, Nowej Zelandii i Kanady w ramach programu Microsoft Commerce Incentive. Jeśli jesteś partnerem rozliczania bezpośredniego lub dostawcą pośrednim w tych trzech krajach zarejestrowanych w programie MCI i nie widzisz noty kredytowej LRD jako dostępnej formy płatności, potwierdź, że identyfikator dzierżawy jest skojarzony z odpowiednim kontem lokalizacji MPN partnera. Aby uzyskać więcej informacji na ten temat, [przeczytaj, jak zaktualizować profil organizacji.](update-your-partner-profile.md)

    
5. Wybierz **walutę**.

6. Po ukończeniu wszystkich pól płatności wybierz pozycję **Prześlij**.

## <a name="set-up-a-default-bank-profile"></a>Konfigurowanie domyślnego profilu bankowego

Możesz skonfigurować domyślne profile bankowe i przypisać je do lokalizacji MPN. Te profile domyślne będą używane przez firmę Microsoft do kolejnych rejestracji w tej lokalizacji MPN. 

1. Zaloguj się do [Partner Center,](https://partner.microsoft.com/dashboard/)a następnie wybierz ikonę koła zębatego, aby otworzyć **Ustawienia**   nawigacyjnym. 

2. Wybierz **pozycję Ustawienia konta,** rozwiń **sekcję Wypłata i podatek,** a następnie wybierz **pozycję Profile wypłaty i profile podatkowe.** 

3. Wybierz **pozycję Zarządzaj profilami domyślnymi** w **sekcji Profile** płatności. 

4. Aby utworzyć domyślny profil bankowy, wybierz **pozycję Dodaj domyślny profil bankowy.** 

5. Wybierz profil bankowy z listy dostępnych profilów bankowych Twojej firmy, wybierz walutę, która ma być używana z tym profilem banku, a następnie wybierz listę lokalizacji MPN, dla których chcesz zastosować ten profil domyślny.

6. Po **zakończeniu** wyboru wybierz pozycję Gotowe. Przycisk Gotowe nie będzie można klikać do momentu ukończenia wszystkich wymaganych pól. 

>[!NOTE]
>To samo parowanie banków i walut można zastosować do wielu lokalizacji. Jeśli do lokalizacji MPN przypisano jeden raz domyślny profil i kombinację waluty, nie będzie ona już wyświetlana na liście rozwijanej lokalizacji dla przyszłych domyślnych przypisań profilów. Jeśli wybór domyślny zostanie usunięty, lokalizacja MPN pojawi się ponownie w przypadku przyszłych domyślnych przypisań profilów. Każda kombinacja profilu bankowego i waluty jest dodawana jako unikatowy, edytowalny wiersz.

7. Po dodaniu wszystkich wymaganych zmian wybierz pozycję **Zapisz**.  

## <a name="create-your-bank-profile"></a>Tworzenie profilu bankowego

Profile bankowe są tworzone na poziomie firmy. Dzięki temu jeden profil bankowy może być przypisany do wielu identyfikatorów MPN i programów zachęt w firmie. Mogą wystąpić wyjątki podczas stosowania profilu bankowego do różnych krajów, ponieważ mogą mieć zastosowanie różne reguły dotyczące bankowości i podatków.

>[!NOTE]
>Na poniższych stronach wymagane są pola oznaczone gwiazdką. Jeśli nie wiesz, co to jest pole, wybierz ikonę informacji. 

1. Na stronie **Szczegóły** wypełnij następujące pola: **Nazwa profilu:** Wprowadź unikatową nazwę identyfikującą ten profil płatności.
    **Lokalizacja konta bankowego:** Kraj, w którym znajduje się bank firmy.
    **Formy płatności:** Preferowaną metodą płatności za Partner Center jest elektroniczne przelew bankowy.

2. Wybierz opcję **Dalej**.

3. Na stronie **Konto bankowe** wprowadź swoje informacje. Pola wyświetlane na tej stronie różnią się w zależności od kraju. 

4. Wybierz opcję **Dalej**.

5. Na **stronie** Wzręb wprowadź odpowiednie informacje. Jest to osoba w firmie, z którą bank skontaktuje się, jeśli będzie musiał omówić Twoje konto.

6. Po zakończeniu pól wybierz pozycję **Zakończ,** a następnie wybierz pozycję **Potwierdź,** aby utworzyć profil bankowy.

Nastąpi przekierowanie do strony **Wypłaty** i profile podatkowe. Stan nowego profilu będzie odzwierciedlał **oczekującą** weryfikację firmy Microsoft do momentu ukończenia walidacji. Ten proces może potrwać do 48 godzin. Po zakończeniu walidacji stan profilu będzie odzwierciedlał stan **Zatwierdzone** lub **Wymagana akcja**. Jeśli **wymagana jest** akcja , powtórz powyższe kroki, podając niezbędne informacje. 

## <a name="create-your-tax-profile"></a>Tworzenie profilu podatkowego

Użyj poniższej procedury, aby przekazać firmie Microsoft informacje podatkowe wymagane dla Twojej organizacji. Strony w tej sekcji są dynamiczne i różnią się w zależności od kraju lub regionu. Jeśli potrzebujesz pomocy przy identyfikowaniu prawidłowych informacji podatkowych, skontaktuj się z odpowiednimi źródłami rządowymi w Twoim kraju.

W przypadku firm partnerskich w Ameryce Północnej i Południowej, jeśli potrzebujesz informacji na temat wypełniania formularzy W8 lub W9, następujące adresy przejdą do witryny IRS:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Wprowadź tylko szczegóły dotyczące twojej firmy. Nigdy nie wprowadzaj danych osobowych.

1. Na stronie **Profil biznesowy** wypełnij wymagane pola, a następnie wybierz pozycję **Dalej.** 

2. Na **stronie Konfiguracja** wybierz opcję, która ma zastosowanie do Twojej firmy.

   - Wybierz opcję po lewej stronie, jeśli twoja firma jest włączona tylko do Stany Zjednoczone lub jeśli ten profil jest dla osoby poszczególnych.
   - Wybierz opcję po prawej stronie, jeśli firma jest włączona poza Stany Zjednoczone, a następnie wybierz kraj/region z listy.

3. Wybierz opcję **Dalej**. 

4. Na stronie **Stan podatkowy** wprowadź wymagane informacje, a następnie wybierz pozycję **Dalej.** Pola na tej stronie będą się różnić w zależności od kraju. Twoje szczegóły. 

5. Na stronie **Dodatkowa dokumentacja** wybierz wymagane pola i wybierz pozycję **Dalej.** 

6. Wybierz **pozycję Przeglądaj,** aby przekazać wszystkie dokumenty wymagane przez kraj lub region. Gdy zostanie pokazana nazwa dokumentu, wybierz pozycję **Upload**. 

7. Jeśli musisz usunąć dokument, wybierz pozycję **Usuń**.

8. Aby zapisać i kontynuować, wybierz pozycję **Zakończ.**

9. Wybierz **pozycję Potwierdź** w wyskakującym komunikacie. Powrócisz do strony Wypłaty i **konfiguracja podatku.**
 
## <a name="update-expired-tax-profiles"></a>Aktualizowanie wygasłych profilów podatkowych

1. Zaloguj się na Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard/)a następnie wybierz ikonę koła zębatego, aby otworzyć **Ustawienia** menu.

1. Wybierz **pozycję Ustawienia konta,** rozwiń **sekcję Wypłata i** podatek, a następnie wybierz pozycję **Wypłata i profil podatkowy.**

1. Wybierz **pozycję Profil podatkowy.**

1. Sprawdź kolumnę **Data wygaśnięcia i** przejdź do profilu podatkowego, który wygasł lub który ma wygasnąć.

1. Wybierz pozycję **Edytuj**.

1. W sekcji formularza podatkowego zaktualizuj formularze podatkowe, podając nowe szczegóły. 

## <a name="next-steps"></a>Następne kroki

- [Typowe pytania dotyczące wypłat i podatków](payout-faq.yml)
