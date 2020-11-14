---
title: Wypłaty i profile podatkowe w Centrum partnerskim
ms.topic: how-to
ms.date: 11/12/2020
description: Utwórz wypłatę i profil podatkowy i zarządzaj nimi, aby otrzymywać opłaty za Twoje zachęty. Obejmuje tworzenie i używanie różnych profilów oraz zarządzanie nimi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 66177c6e3cd0091081866e1508d28346f49ec713
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626035"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Twórz wypłaty i profile podatków w centrum partnerskim i zarządzaj nimi

**Dotyczy:**

- Centrum partnerskie

**Odpowiednie role:**

- Administrator zachęt
- Administrator konta
- Administrator globalny

Aby można było otrzymać płatność z tytułu programów zachęt dla konkretnej lokalizacji MPN, należy ukończyć rejestrację, dokonując skojarzenia prawidłowego profilu wypłaty i profilu podatkowego z programem i lokalizacją MPN. Firma Microsoft będzie korzystać z tego profilu wypłaty i profilu podatkowego w celu realizacji płatności. W zależności od zasad programu zachęt może być możliwe wykorzystanie elektronicznego przelewu bankowego lub noty kredytowej przy płatności. 

## <a name="roles-currencies-and-other-microsoft-programs"></a>Role, waluty i inne programy firmy Microsoft

Ważne jest zapoznanie się z poniższymi informacjami przed rozpoczęciem pracy z wypłatą i profilem podatkowym.

### <a name="roles-and-permissions"></a>Role i uprawnienia

Musisz być administratorem zachęty, aby wprowadzać informacje o banku i podatku na potrzeby zachęt. Jeśli jesteś administratorem konta MPN/, możesz przypisać siebie i/lub współpracownikowi administratora zachęt.

Jeśli musisz zażądać uprawnień administratora programu zachęty, skontaktuj się z administratorem MPN lub administratorem globalnym. Aby dowiedzieć się, kto w firmie ma te role, zaloguj się na [pulpicie nawigacyjnym Centrum partnerskiego](https://partner.microsoft.com/dashboard/). Na ikonie **ustawień** w prawym górnym rogu wybierz pozycję **Zarządzanie użytkownikami** , a następnie odfiltruj uprawnienia administratora globalnego.

Zachęcaj użytkowników do wyświetlania zarobków i szczegółów płatności oraz raportów, ale nie możesz edytować informacji o banku i podatku.

### <a name="choose-your-disbursement-currency"></a>Wybierz walutę płatności

Płatności zachęty są wprowadzane w walucie wybranej podczas konfigurowania profilu płatności. Płatności będą obliczane przy użyciu stawki wymiany ustawionej miesięcznie przez firmę Microsoft. Użytkownik jest odpowiedzialny za wszelkie zmiany wartości ze względu na wybraną walutę.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Używanie różnych profilów dla różnych programów firmy Microsoft

Jeśli Twoja firma jest zarejestrowana w wielu programach zachęty, możesz użyć tego samego konta płatności dla wszystkich z nich lub użyć różnych kont płatności dla różnych programów.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Utwórz wypłaty i profile podatków w centrum partnerskim i zarządzaj nimi

Poniższe sekcje przeprowadzą Cię przez proces tworzenia i zarządzania profilami płatności i podatków w centrum partnerskim.

>[!IMPORTANT]
>Aby tworzyć profile płatności w centrum partnerskim lub zarządzać nimi, musisz być administratorem zachęty. Role zachęty muszą być przypisane do każdej lokalizacji MPN w ramach każdego programu zachęty. Aby uzyskać więcej informacji na temat dodawania administratorów zachęty w centrum partnerskim, zobacz [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Dostęp do sekcji wypłaty i opodatkowania w centrum partnerskim

1. Zaloguj się na [pulpicie nawigacyjnym Centrum partnerskiego](https://partner.microsoft.com/dashboard/) przy użyciu konta Azure Active Directory (Azure AD) (konta firmowego) lub odpowiedniego adresu e-mail, jeśli został przypisany.

   - W ramach jednego konta usługi Azure AD można zarejestrować wiele domen. Skontaktuj się z administratorem globalnym, aby określić, które domeny są skojarzone.
   - Jeśli możesz zalogować się tylko za pomocą @onmicrosoft.com domeny, skontaktuj się z administratorem konta w celu dodania dodatkowych domen do konta usługi Azure AD.
   - Jeśli zostanie wyświetlony monit o wybranie **konta służbowego** lub **konta osobistego** , wybierz pozycję **konto służbowe**.

2. Wybierz ikonę koła zębatego, aby otworzyć menu **Ustawienia** , a następnie wybierz pozycję **Ustawienia partnera**.

3. W menu **Ustawienia konta** wybierz pozycję **wypłata i podatek**. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Przypisywanie wypłat i profilów podatkowych do poszczególnych programów

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/), a następnie wybierz ikonę koła zębatego, aby otworzyć menu **Ustawienia** . 

2. Wybierz pozycję **Ustawienia partnera** , rozwiń **sekcję wypłata i podatek** , a następnie wybierz pozycję **wypłata i przypisanie profilu podatku**. 
   
   Zostanie wyświetlona lista programów. Wybierz strzałkę obok programu, aby wyświetlić szczegóły profilu. 

3. W menu rozwijanym **profil podatkowy** wybierz odpowiedni profil podatkowy lub wybierz opcję utworzenia nowego profilu. Po wybraniu opcji tworzenia nowego profilu nastąpi odpowiednie przekierowanie.  W oknie podręcznym wybierz pozycję Kontynuuj. Proces tworzenia nowego profilu podatkowego został podany poniżej.

4. Wybierz pozycję **płatność**.

   - Jeśli jako formę płatności wybrano opcję **elektronicznego transferu banku** , wybierz odpowiedni profil płatności lub wybierz opcję utworzenia nowego profilu. Po wybraniu opcji tworzenia nowego profilu nastąpi odpowiednie przekierowanie. W oknie podręcznym wybierz pozycję Kontynuuj. Proces tworzenia nowego profilu płatności został przedstawiony poniżej.

   - Jeśli jako formę płatności została wybrana **Nota kredytowa** , wykonaj weryfikację. Pozwala to upewnić się, że przywoływany numer SAP należy do organizacji.

    >[!NOTE]
    >Jeśli na liście znajduje się wiele jednostek firmy Microsoft, należy wybrać profil płatności dla każdej jednostki.

    >[!NOTE]
    >Dostępność metody płatności zależy od reguł programu zachęty.
    
5. Wybierz **walutę**.

6. Po zakończeniu wszystkich pól płatności wybierz pozycję **Prześlij**.

## <a name="create-your-bank-profile"></a>Tworzenie profilu bankowego

Profile bankowe są tworzone na poziomie organizacji. Umożliwia to przypisanie jednego profilu bankowego do wielu programów MPN ID i zachęt w organizacji. W przypadku zastosowania profilu bankowego do różnych krajów mogą wystąpić wyjątki, ponieważ mogą być stosowane różne reguły bankowości i podatkowej.

>[!NOTE]
>Na następujących stronach wymagane są pola z gwiazdką. Jeśli nie wiesz, co to jest pole, wybierz ikonę informacji. 

1. Na stronie **szczegóły** wypełnij następujące pola: **Nazwa profilu:** wprowadź unikatową nazwę identyfikującą ten profil płatności.
    **Lokalizacja konta bankowego:** Kraj, w którym znajduje się bank firmy.
    **Forma płatności:** Preferowana metoda płatności w centrum partnerskim to elektroniczny transfer bankowy.

2. Wybierz opcję **Dalej**.

3. Na stronie **konto bankowe** wprowadź informacje. Pola wyświetlane na tej stronie różnią się w zależności od kraju. 

4. Wybierz opcję **Dalej**.

5. Na stronie **beneficjent** wprowadź odpowiednie informacje. Beneficjentem jest osoba w firmie, którą będzie mogła skontaktować się z kontem, jeśli trzeba omówić Twoje konto.

6. Po zakończeniu pól wybierz pozycję **Zakończ** , a następnie wybierz pozycję **Potwierdź** , aby utworzyć profil banku.

Nastąpi przekierowanie do strony z **profilami wypłaty i podatkiem** . Stan nowego profilu będzie odzwierciedlać **oczekiwanie na zweryfikowanie firmy Microsoft** , dopóki weryfikacja nie zostanie ukończona. Ten proces może potrwać do 48 godzin. Po zakończeniu walidacji stan Twojego profilu będzie odzwierciedlać **zatwierdzenie** lub **wymagane działanie**. Jeśli **wymagana jest akcja** , powtórz powyższe kroki, podając wymagane informacje. 

## <a name="create-your-tax-profile"></a>Utwórz swój profil podatkowy

Poniższa procedura umożliwia firmie Microsoft podanie informacji podatkowych wymaganych przez organizację. Strony w tej sekcji są dynamiczne i różnią się w zależności od kraju lub regionu. Jeśli potrzebujesz pomocy przy identyfikacji poprawnych informacji podatkowych, skontaktuj się z odpowiednimi źródłami rządowymi w danym kraju.

W przypadku firm partnerskich u Ameryki Północnej, jeśli potrzebne są informacje dotyczące kończenia formularzy W8 lub W9, następujące adresy przekazują użytkownika do lokacji urzędu skarbowego:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Wprowadź tylko szczegóły dla swojej firmy. Nigdy nie wprowadzaj szczegółów osobistych.

1. Na stronie **profil biznesowy** Wypełnij wymagane pola, a następnie wybierz przycisk **dalej**. 

2. Na stronie **Instalator** wybierz opcję, która ma zastosowanie do Twojej firmy.

   - Wybierz opcję po lewej stronie, jeśli Twoja firma jest włączona tylko do Stany Zjednoczone lub jeśli ten profil jest przeznaczony dla osoby.
   - Wybierz opcję po prawej stronie, jeśli Twoja firma jest wbudowana poza Stany Zjednoczone, a następnie wybierz z listy swój kraj/region.

3. Wybierz opcję **Dalej**. 

4. Na stronie **stan podatkowy** wprowadź wymagane informacje, a następnie wybierz przycisk **dalej**. Pola na tej stronie różnią się w zależności od kraju. Twoje szczegóły. 

5. Na stronie **dodatkowe dokumenty** wymagane pola i wybierz przycisk **dalej**. 

6. Wybierz pozycję **Przeglądaj** , aby przekazać dokumenty wymagane przez kraj lub region. Gdy zostanie wyświetlona nazwa dokumentu, wybierz pozycję **Przekaż**. 

7. Jeśli musisz usunąć dokument, wybierz pozycję **Usuń**.

8. Aby zapisać i kontynuować, wybierz pozycję **Zakończ**.

9. W oknie podręcznym wybierz pozycję **Potwierdź** . Nastąpi powrót do strony **konfiguracji wypłaty i podatku** .

## <a name="next-steps"></a>Następne kroki

- [Zachęty wypłaty i profil podatkowy — często zadawane pytania](incentives-payout-tax-profile-faqs.md)
