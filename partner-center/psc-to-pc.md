---
title: Migrowanie z programu Partner Sales Połączenie (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Dowiedz się, jak partnerzy firmy Microsoft mogą migrować z witryny Partner Sales Połączenie (PSC) Partner Center i tworzyć transakcje wysyłane przez sprzedawców firmy Microsoft oraz zarządzać nimi.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.date: 09/08/2021
ms.openlocfilehash: 96106dd84d4889c9165daf41385d1092361101c4
ms.sourcegitcommit: 731a5e2725a72ecdae40189a3f52ab6b4a4c8058
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/20/2021
ms.locfileid: "128007284"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Przewodnik dotyczący współsprzedaży w Partner Center (PC) dla partnerów migrowania z partnerów w Połączenie (PSC)

**Odpowiednie role:** Administrator konta | Administrator poleceń | Partner Sales Połączenie (PSC) seller | Partner Sales Połączenie (PSC) admin | Partner Sales Połączenie (PSC) deal manager

Ten artykuł zawiera wskazówki dla partnerów migrowania z programu Partner Sales Połączenie (PSC) do usługi Partner Center (PC), dzięki czemu mogą oni nadal tworzyć transakcje dotyczące sprzedaży Partner Center i zarządzać nimi.

> [!NOTE]
> Jeśli jesteś tutaj, ponieważ na stronie PSC został wyzłoszty baner o migracji, jesteś w odpowiednim miejscu. Ten przewodnik nie ma zastosowania w przypadku partnerów biznesowych zarządzających transakcjami w ramach programu PsC na potrzeby oceny rozwiązań (SA) i partnerów biznesowych zarządzających licencjonowaniem OEM.

> [!IMPORTANT]
> Od 1 kwietnia 2021 r. Twoja firma nie będzie mogła tworzyć ani edytować transakcji w programie PSC. **Nadal będzie można pobierać istniejące dane transakcji przy użyciu funkcji eksportu zbiorczego w konsoli psc. Możesz również [migrować otwarte transakcje](psc-to-pc.md#psc-deals-migration) z konsoli psc do Partner Center tej daty.**
> 
> Jeśli istnieją transakcje, nad które aktywnie pracujesz, które zawierają kwalifikujące się rozwiązania zachęty do współzasyłania adresów IP, masz dwie opcje:
> 
> 1. Oznacz umowę jako wygraną i ukończ rejestrację transakcji w chmurze przed 31 marca 2021 r.
> 2. [Przemigruj](psc-to-pc.md#psc-deals-migration) transakcje do Partner Center, aby uzyskać więcej czasu na pracę nad transakcją i rozpoczęcie rejestracji transakcji.

Mimo że Twoja firma utraci dostęp do centrum zabezpieczeń po 30 kwietnia 2021 r., nadal znajdziesz wszystkie działania, które chcesz wykonać w firmie Partner Center, takie jak tworzenie transakcji sprzedaży współsprzedaży, zarządzanie transakcjami i działania na podstawie transakcji wysyłanych do Ciebie przez sprzedawców firmy Microsoft.

Będą jednak różnice. Poniższe wskazówki mogą pomóc w sprawniejszym i prostszym Partner Center przejścia na inne urządzenia.

## <a name="things-to-know-before-moving"></a>Co należy wiedzieć przed przeniesieniem

### <a name="if-you-are-a-psc-admin"></a>Jeśli jesteś administratorem usługi PSC

- Do zalogowania się do usługi Partner Center potrzebna [jest służbowa Partner Center](https://partner.microsoft.com/).
- Skonfiguruj swoje konto za pomocą administratora Partner Center [konta.](permissions-overview.md)
- Dowiedz się, jak sprzedawać w Partner Center, czytając ten dokument.
- Skonfiguruj konta użytkowników w programie Partner Center dla wszystkich użytkowników centrum zabezpieczeń (role administratora, menedżera transakcji i sprzedawcy) i przypisz im role [administratora poleceń.](permissions-overview.md)

>[!IMPORTANT]
> Upewnij się, Microsoft Partner Network (MPN) identyfikator wyświetlany na banerze PSC jest dostępny na liście lokalizacji MPN w Partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Obraz przedstawiający transparent PSC, na którym partnerzy mogą znaleźć identyfikator MPN.":::

 Aby **sprawdzić,** czy identyfikator MPN jest wyświetlany jako lokalizacja Partner Center MPN, zaloguj się do pulpitu nawigacyjnego usługi [Partner Center,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję Ustawienia (ikona koła zębatego) w prawym górnym rogu ekranu, a następnie pozycję **Konto Ustawienia**. W menu nawigacji po lewej stronie  drugiego poziomu wybierz pozycję Lokalizacje, aby wyświetlić listę wszystkich identyfikatorów i lokalizacji MPN skojarzonych z Partner Center kontem.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Jeśli jesteś menedżerem transakcji psc lub sprzedawcą

- Do zalogowania się do pulpitu nawigacyjnego usługi Partner Center potrzebna jest [służbowa wiadomość e-mail.](https://partner.microsoft.com/dashboard)
- Jeśli używasz konta innego niż służbowe w programie PSC lub Służbowa poczta e-mail jest dla innej firmy niż firma partnerska, skontaktuj się z administratorem centrum partnerskiego, aby uzyskać pomoc w skonfigurowaniu konta.
- Skontaktuj się z administratorem usługi PSC, Partner Center skonfigurowanie konta usługi jest ukończone niezależnie od konta, za pomocą których logujesz się do usługi PSC.
- Sprawdź, czy masz dostęp do Partner Center i sekcji Polecenia.
- Przeczytaj ten dokument, aby zrozumieć przepływy pracy i zmiany Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Jako administrator w programie PSC, to są Twoje następne kroki

W Partner Center nawigacji po lewej stronie wybierz **opcję Polecenia.** Upewnij się, że możesz uzyskać dostęp do stron Polecenia.

  >[!Note]
  > Może być konieczne wylogowanie się z Partner Center i zalogowanie się ponownie, aby odświeżyć poświadczenia w celu uzyskania dostępu do stron Poleceń.

Jeśli nie widzisz opcji  Polecenia w menu usługi Partner Center lub na stronach związanych z poleceniami, skontaktuj się z administratorem  konta firmy i poproś go o dostęp do opcji Polecenia i powiązanego obszaru. [](permissions-overview.md)

Aby znaleźć administratora konta firmy:

1. Wybierz **pozycję Ustawienia konta** z ikony koła zębatego w prawym górnym rogu pulpitu Partner Center nawigacyjnego.

1. Wybierz **pozycję Zarządzanie użytkownikami** z menu nawigacji drugiego poziomu po lewej stronie.

1. W górnej części listy użytkowników  wybierz menu rozwijane Filtr. Zmień opcję na **Administrator konta.**

   Na stronie zostaną wyświetleń wszyscy administratorzy kont z odpowiednimi adresami e-mail. Wyślij wiadomość e-mail do jednej z nich i poproś o przypisanie roli administratora poleceń dla Twojego konta służbowego.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Obraz przedstawiający administratorów kont na stronie zarządzania użytkownikami ustawień partnera.":::

>[!Important]
>- Jeśli Twoja rola obejmuje tylko zarządzanie użytkownikami w programie PSC, poproś administratora konta firmy o przypisanie Ci roli administratora konta w Partner Center. [](permissions-overview.md#manage-mpn-membership-and-your-company) 
>- Jeśli Twoja rola obejmuje również zarządzanie możliwościami współpracy sprzedaży, poproś o przypisanie roli [administratora poleceń.](permissions-overview.md#manage-referrals)
> - Dobrym pomysłem jest również wyznaczyć jednego lidera zarządzania zmianami wśród administratorów centrum zarządzania zmianą. Spowoduje to, że wszyscy administratorzy centrum usługi nie będą mieć indywidualnego zasięgu w celu Partner Center administratorów kont. Zamiast tego lider zarządzania zmianami może być główną osobą pracującą z administratorem Partner Center konta.

## <a name="user-migration"></a>Migracja użytkowników

Po skonfigurowaniu konta w Partner Center użyj kreatora migracji użytkowników na stronie możliwości współpracy sprzedaży, aby automatycznie przypisać Partner Center do pracowników firmy.

>[!Note]
> Migrację użytkowników mogą przeprowadzać tylko [administratorzy](permissions-overview.md#manage-mpn-membership-and-your-company) kont w firmie. Jeśli nie masz roli administratora konta, znajdź administratora konta, który może pomóc w skonfigurowaniu kont użytkowników za pomocą kreatora migracji użytkowników.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Obraz przedstawiający kreatora migracji użytkowników.":::

Administratorzy kont zobaczą link kreatora migracji użytkowników PSC na stronie możliwości współpracy sprzedaży obok przewodnika po poleceniach. Mogą zainicjować migrację użytkowników, wybierając link. Aby zainicjować migrację użytkowników, administratorzy mogą wybrać link. Ten krok migracji użytkowników można wykonać wiele razy, dopóki wszyscy użytkownicy nie zostaną przypisani do odpowiednich ról w Partner Center.

Tabela migracji użytkowników zawiera następujące szczegóły:

- Konto użytkownika — identyfikator e-mail pracownika
- Konto partnera PSC — konto, z którym jest skojarzony pracownik w programie PSC
- Rola użytkownika PSC — jedna z trzech ról przypisanych do funkcji PSC.
- Lokalizacja PC MPN — lokalizacja, dla której użytkownik będzie mieć odpowiednie Partner Center (pc). Konto partnera PSC MPN służy do znalezienia równoważnej lokalizacji MPN Partner Center do przypisywania uprawnień. Cała organizacja określa identyfikator MPN vOrg.
- Rola użytkownika komputera — pracownicy mają przypisane role na podstawie ich ról użytkownika psc. Administrator usługi PSC ma przypisane role administratora poleceń w Partner Center. Sprzedawca będzie mieć przypisaną rolę użytkownika poleceń w Partner Center. Dowiedz się więcej o rolach usługi Partner Center i o tym, co mogą robić użytkownicy z tymi rolami w programie Partner Center w sekcji Zarządzanie poleceniami w sekcji Przypisywanie ról i uprawnień użytkowników dla użytkowników firmy, którzy muszą pracować w Partner Center [.](permissions-overview.md#manage-referrals)
- Dzierżawa usługi PC AAD — dzierżawa usługi Microsoft Azure Active Directory (Azure AD), do której przypisano użytkowników w usłudze Partner Center
- Stan — istnieją trzy możliwe stany stanu migracji
    - **Niemigrowane** — użytkownik nie ma przypisanej Partner Center poleceń
    - **Zmigrowane** — użytkownik został pomyślnie zmigrowany z przypisaną odpowiednią rolą, jak pokazano w tabeli
    - **Błąd** — nie można ukończyć migracji z powodu błędu

Czasami migracja może się nie powieść i spowodować błędy. Poniżej podano kilka przyczyn, dla których migracja może spowodować błąd, oraz kilka sposobów rozwiązania problemu:

1. Użytkownicy usługi PSC mogą używać konta nie służbowego.

2. Użytkownik PSC może używać konta z domeny innej niż ta, która jest Partner Center.

   Aby usunąć błędy związane ze scenariuszami 1 i 2, poproś użytkownika o zalogowanie się Partner Center przy użyciu konta służbowego dołączonego do dzierżawy usługi Azure AD. Administrator [globalny może](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) ci pomóc.
   
   Aby znaleźć administratora globalnego: 
   - Zaloguj się do pulpitu Partner Center [i](https://partner.microsoft.com/dashboard) wybierz **pozycję Ustawienia konta** z ikony koła zębatego w prawym górnym rogu.
   - Wybierz **pozycję Zarządzanie użytkownikami** na lewym pasku nawigacyjnym drugiego poziomu.
   - W górnej części listy użytkowników  wybierz menu rozwijane Filtr i zmień opcję na **Administrator globalny.** Następnie na stronie zostaną wyświetloni wszyscy administratorzy globalni wraz z ich odpowiednimi adresami e-mail. Poproś jedną z nich o przypisanie roli administratora poleceń dla konta służbowego.
   
      Administrator globalny może utworzyć nowe konto użytkownika w dzierżawie usługi Azure AD lub przypisać dostęp użytkownika-gościa do innych użytkowników konta domeny. Po skonfigurowaniu kont dla wszystkich menedżerów transakcji psc i użytkowników muszą oni zalogować się do witryny Partner Center, wybrać pozycję Polecenia z menu nawigacji po lewej stronie i potwierdzić, że widzą stronę Polecenia. 

3. Użytkownik ma już przypisaną rolę odwołania w Partner Center.
    - Możesz sprawdzić istniejącą rolę użytkownika. W prawym górnym rogu okna Partner Center wybierz pozycję **Ustawienia** (ikona koła zębatego), a następnie **pozycję Ustawienia konta.** Po wyświetleniu drugiego menu nawigacji po lewej stronie wybierz pozycję **Zarządzanie użytkownikami** i wyszukaj użytkownika.

## <a name="psc-deals-migration"></a>Migracja transakcji PSC

Po zakończeniu migracji użytkowników użyj kreatora migracji transakcji na stronie możliwości współpracy sprzedaży, aby wszystkie kwalifikujące się otwarte transakcje z witryny PSC były Partner Center. **Link migracji transakcji będzie widoczny tylko dla administratorów poleceń z całym zakresem organizacji w Partner Center.** W prawym górnym rogu strony szans wspólnej sprzedaży będzie dostępny link o nazwie **„Migracja transakcji PSC”** umożliwiający otwarcie kreatora migracji transakcji.

Przeczytaj tę sekcję przed rozpoczęciem migracji transakcji.

**Kwalifikowanie się do migracji**

Tylko niektóre transakcje kwalifikują się do migracji z usługi PSC do Partner Center. Ten kreator migracji został zbudowany w celu pomocy partnerom w wywniosce ich transakcji do Partner Center gdzie nadal aktywnie współpracują ze swoimi klientami, aby zamknąć transakcję. **Tylko transakcje, które są w stanie otwartym utworzone od 1 stycznia 2020 r. z prawidłowymi szczegółami konta partnera (prawidłowy identyfikator MPN) i które nie są objęte rejestracją transakcji, kwalifikują się do migracji.**

**Nie kwalifikuje się do migracji**

- Transakcje oceny rozwiązań nie kwalifikują się do migracji transakcji
- Umowy biznesowe licencjonowania OEM nie kwalifikują się do migracji transakcji
- Każda transakcja oznaczona jako wygrana w programie PSC nie kwalifikuje się do migracji. Rejestracja transakcji, jeśli kwalifikuje się do transakcji oznaczonych jako wygrane, powinna zostać ukończona w chmurze psc.

## <a name="pre-requisites-for-deal-migration"></a>Wymagania wstępne dotyczące migracji transakcji

Przed rozpoczęciem migracji transakcji z Partner Center, postępuj zgodnie z poniższymi instrukcjami, aby skonfigurować transakcje w chmurze dla pomyślnej migracji.

1. Wszyscy członkowie zespołu sprzedaży w Twojej firmie pracujący nad otwartymi transakcjami są poinformowani o tej migracji.
2. Członkowie zespołu sprzedaży są przeszkoleni do używania Partner Center do zarządzania umowami.
3. Transakcje zawierają wszystkie wymagane informacje zgodnie z poniższym opisem.
    - Szczegóły firmy klienta, w tym nazwa i adres
    - Szczegóły kontaktu z klientem, jeśli jest to transakcja typu "co-sell"
    - Co najmniej jedno rozwiązanie
    - Co najmniej jeden członek zespołu ze wszystkimi szczegółami — imię, nazwisko, identyfikator e-mail i numer telefonu
    - Wartość transakcji
    - Szacowana data zamknięcia transakcji
    - Uwagi partnerów

Możesz użyć funkcji zbiorczego pobierania i przekazywania w chmurze psc, aby dodać wszystkie brakujące szczegóły transakcji dla wszystkich kwalifikujących się transakcji.

>[!Note]
> Migracja transakcji powiedzie się, nawet jeśli powyższe wymagania wstępne nie zostaną spełnione. Nie można jednak zmienić stanu transakcji, jeśli dowolne z powyższych wymaganych pól w Partner Center są niedostępne. Następnie musisz wprowadzić wszystkie wymagane informacje, których brakuje w transakcjach w Partner Center, aby rozpocząć pracę nad nimi. **Zdecydowanie zaleca się oczyszczenie kwalifikujących się transakcji w programie PSC przed ich migracją do Partner Center.**

Migracja transakcji w Partner Center jest zbudowana jako środowisko jednym kliknięciem. Wystarczy wybrać przycisk "Migruj **transakcje",** gdy firma będzie gotowa do migracji kwalifikujących się transakcji. **Nie można wybrać transakcji, które mają zostać zmigrowane z konsoli psc. Jeśli nie chcesz migrować żadnych transakcji do Partner Center, przenieś je do stanu zamkniętego w konsoli psc przed rozpoczęciem migracji.**

>[!Note]
> Po zainicjowaniu migracji migrowanie transakcji może potrwać do **24 godzin.**

Po zakończeniu migracji stan komunikatu baneru zmieni się na ukończony z linkiem do raportu migracji. Pobierz raport, aby wyświetlić szczegóły transakcji, które zostały zmigrowane z konsoli psc do Partner Center.

Raport zawiera poniższe szczegóły.

1. **Partner Center zaangażowania —** unikatowy identyfikator w Partner Center dla wszystkich transakcji w zaangażowaniu. Istnieją dwie transakcje — jedna dla partnera i jedna dla firmy Microsoft w przypadku zaangażowania w sprzedaż Partner Center.
2. **Partner Center polecenia —** unikatowy identyfikator w Partner Center dla transakcji należącej do partnera.
3. **Nazwa transakcji** — identyfikator nadany transakcji w konsoli psc.
4. **Identyfikator transakcji PSC** — unikatowy identyfikator transakcji w chmurze psc.
5. **Błędy** — aby wskazać, czy wystąpił błąd podczas migrowania konkretnej transakcji.

Wszystkie transakcje, które zostały pomyślnie zmigrowane, nie będą widoczne w konsoli psc. Możesz kontynuować pracę nad zmigrowanych transakcji w Partner Center łącznie z ukończeniem rejestracji transakcji w Partner Center. Nie będzie żadnych zmian w interakcjach ze sprzedawcami firmy Microsoft w przypadku transakcji sprzedaży.

Transakcje migrowane z karty PSC będą dostępne na kartach Przychodzący i Wychodzący w zależności od źródła transakcji. Wszystkie transakcje udostępniane przez Twoją firmę będą dostępne na karcie Dane wychodzące, a transakcje inicjowane przez firmę Microsoft będą dostępne na karcie Przychodzące Partner Center. Istnieją dwa typy transakcji, które zostaną utworzone po migracji.

1. **Transakcje sprzedaży współsprzedaży** — transakcje oznaczone jako transakcje sprzedaży współsprzedaży w programie PSC będą tworzone jako transakcje sprzedaży Partner Center.
2. **Transakcje prowadzone przez partnera** — transakcje, które nie są oznaczone jako współsieć, będą tworzone jako transakcje prowadzone przez partnera w Partner Center. Transakcje prowadzone przez partnerów są widoczne dla sprzedawców firmy Microsoft i można je uaktualnić do transakcji sprzedaży typu "co sell" przed osiągnięciem stanu końcowego (wygrane, utracone). Ponadto transakcje prowadzone przez partnera kwalifikują się do rejestracji transakcji, jeśli w transakcji istnieje rozwiązanie kwalifikujące się do zachęty.

>[!Important]
> Jeśli występują błędy, których nie można zmigrować niektórych transakcji, możesz ponownie zainicjować migrację transakcji, klikając przycisk **"Migruj transakcje".** Zostanie ona włączona tylko wtedy, gdy istnieją kwalifikujące się transakcje, które nie zostały jeszcze zmigrowane. Będzie to również przydatne, jeśli jesteś w fazie przejścia, w której niektóre nowe transakcje są tworzone w chmurze po zainicjowaniu migracji transakcji.

Po pomyślnym zmigrowania wszystkich transakcji pojawi się transparent z napisem "Brak transakcji do **migracji"** z wyłączonym przyciskiem "Migruj **transakcje".** 

Po zakończeniu migracji użytkowników i/lub transakcji migracji skorzystaj z poniższych wskazówek, aby zdecydować strategię migracji:

Jeśli Twoja firma ma menedżera rozwoju partnerów (PDM) — po skonfigurowaniu konta usługi Partner Center, gdy użytkownicy przeszli do firmy i mają role oraz uprawnienia, możesz przenieść działania związane ze sprzedażą do Partner Center. Poinformuj pdm, aby przełączyć się, zamiast czekać na ukończenie terminu migracji, co umożliwi przepływ wszystkich nowych transakcji do Partner Center.

>[!Note]
>Po przełączeniu będzie można działać tylko w przypadku istniejących aktywnych transakcji w programie PSC. Nie możesz tworzyć nowych transakcji ani odbierać żadnych transakcji od sprzedawców firmy Microsoft w witrynie PSC.

Jeśli firma nie ma podstawowego kontrolera pdm — upewnij się, że wszystkie konta użytkowników zostały ustawione i zweryfikowane przez wszystkich użytkowników. Za pośrednictwem wiadomości e-mail i baneru w chmurze zostaniesz powiadomiony o dokładnej dacie rozpoczęcia sprzedaży w Partner Center. Należy pamiętać, że nadal będzie trzeba zarządzać istniejącymi aktywnymi transakcjami w chmurze.

>[!Important]
> Do 30 kwietnia 2021 r. masz czas na zarejestrowanie transakcji oznaczonych jako wygrane.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Następne kroki dla administratorów centrum psc, menedżerów transakcji psc i sprzedawców PSC

Dowiedz się, jak sprzedawać w Partner Center.
Jest to ważny krok, który pomoże Ci przygotować się na współsieć w Partner Center. Poznaj przepływy pracy i zmiany w Partner Center, aby od razu skutecznie sprzedawać. Zacznij od całkowitego przeczytania tego dokumentu. Dobry zestaw zasobów jest również dostępny w galerii obsługi [współs sprzedaży.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>Główne różnice między przepływami pracy psc Partner Center przepływami pracy

|**Scenariusz**|**Partner Sales Połączenie**|**Centrum partnerskie**|
|-----|:-----|:-----|
|Role użytkownika|PsC ma role administratora, menedżera transakcji i sprzedawcy.|Partner Center ma tylko rolę [administratora poleceń,](permissions-overview.md#manage-referrals) która zapewnia uprawnienia zarówno do odczytu, jak i zapisu dla wszystkich transakcji.|
|Zapraszanie firmy Microsoft w sprawie transakcji sprzedaży|Inicjowane przez sprzedawcę firmy Microsoft nie ma jawnego pytania od partnera.|Partner będzie musiał jawnie [poprosić o](manage-co-sell-opportunities.md#add-solutions) pomoc sprzedawcy firmy Microsoft w przypadku transakcji. Sprzedawca firmy Microsoft może odrzucić żądanie.|
|Wygaśnięcie|Nie istnieje pojęcie wygaśnięcia transakcji.|Umowy przychodzące partnerów wygasają w ciągu 14 dni, jeśli nie zostaną zaakceptowane przez partnera. Tak samo jest w przypadku transakcji wychodzących partnerów, w przypadku których mogą oni przejść w stan wygaśnięcia, jeśli sprzedawca firmy Microsoft nie będzie działać w ich sprawie w ciągu 14 dni.|
|Szczegóły sprzedawcy firmy Microsoft|Widoczne zaraz po utworzeniu transakcji.|Szczegóły sprzedawcy firmy Microsoft są udostępniane partnerowi tylko wtedy, gdy sprzedawca jawnie zaakceptuje zaproszenie do wspólnej sprzedaży od partnera.|
|[Potok prywatny](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Niedostępne.|Partnerzy mogą udostępniać swój potok bez udostępniania informacji sprzedawcom firmy Microsoft.|
|Rozwiązania|Rozwiązania należące tylko do jednego cennika można dodać do transakcji.|Partner może dodawać [rozwiązania,](manage-co-sell-opportunities.md#add-solutions) które należą do poniższych list. a) Własne rozwiązania b) Rozwiązania z wykazu firmy Microsoft (podobne do roli transakcji w psc) i c) rozwiązań do wspólna sprzedaż innych partnerów (podobnie jak w przypadku umowy dostawcy oprogramowania w chmurze).|
|Przypisanie transakcji|Tylko przypisany sprzedawca może wyświetlać transakcje i działać na ich podstawie.|Członków zespołu można dodać do transakcji, aby określić osoby pracujące nad transakcją, a inni administratorzy poleceń nie mogą wyświetlać tych transakcji ani działać w związku z nimi.|
|Organizacja klienta|Wpis tekstowy w postaci bezpłatnej.|Aby przeszukać bazę [danych usługi](manage-co-sell-opportunities.md#select-your-customer) D&B w organizacji [klienta,](https://www.dnb.com/) wystarczy wpisać kilka znaków. Nazwa i adres prawnych są wypełniane automatycznie na podstawie wyboru.|
|Kontakt z klientem|Nie jest to obowiązkowe.|Nie jest to obowiązkowe w przypadku udostępniania potoku prywatnego. Wymagane, jeśli sprzedawca firmy Microsoft jest zapraszany do wzięcia udziału w żądaniu współpracy sprzedaży.|
|Publiczny interfejs API|Niedostępne.|[Publiczny interfejs API](/partner/develop/referrals) do programowego zarządzania Partner Center poleceniami.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mapowanie pól w programie PSC na odpowiednie pola w Partner Center

W tej sekcji porównano wybrane zrzuty ekranu wyświetlane dla psc (lub "mapy") z odpowiednim widokiem w sekcji Partner Center sprzedaży.

Na każdej parze zrzutów ekranu zobaczysz po numerowane, żółte lub czerwone okręgi:

- **Co oznaczają żółte okręgi?** Po numerowane żółte okręgi są wyświetlane jako pierwsze na każdym zrzucie ekranu psc. Następnie znajdziesz pomocnika z Partner Center zrzutu ekranu z wieloma z tych samych liczb.

   Aby zobaczyć, jak każde pole lub atrybut w pliku PSC jest mapowane na jego odpowiednik w Partner Center, dopasuj numerowane okręgi na dwóch powiązanych zrzutach ekranu. Na przykład dopasuj numerowany żółty "1" na pierwszym zrzucie ekranu PSC do numerowanych, żółty "1" w drugim, a Partner Center zrzut ekranu poniżej.

- **Co oznacza czerwone kółko?** Jeśli zobaczysz czerwony okrąg na jednym zrzucie ekranu, oznacza to, że pole PSC nie jest dostępne w Partner Center.

Mapowania pól psc-to-Partner Center są wyświetlane dla następujących obszarów:

1. Strona główna psc zamapowana na Partner Center domyślny widok możliwości współsprzedaży
1. Widok siatki PSC zamapowany na widok Partner Center transakcji
1. Widok szczegółów transakcji psc zamapowany na widok Partner Center szczegóły transakcji
1. Widok DODAWANIA PRODUKTÓW PSC zamapowany na widok Partner Center Dodaj rozwiązania
1. Widok zarządzania użytkownikami psc zamapowany na widok zarządzania Partner Center użytkownikami
1. Widok przypisania roli użytkownika psc zamapowany na widok przypisania Partner Center użytkownika
1. Widok powiadomień PSC zamapowany na widok Partner Center powiadomień

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 — Strona główna narzędzia PSC zamapowana na Partner Center domyślny widok możliwości współsprzedaży

Porównaj pasujące, po numerowane okręgi między górnym zrzutem ekranu psc i Partner Center zrzutem ekranu poniżej. Pasujące liczby pokazują, gdzie można znaleźć funkcję lub atrybut związane z funkcją PSC w Partner Center. Czerwone okręgi wskazują, że nie ma pasującego Partner Center pola.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Obraz przedstawiający mapowania pól między stroną główną witryny Partner Sales Połączenie i domyślnym widokiem możliwości sprzedaży w Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 — Widok siatki PSC zamapowany na widok Partner Center transakcji

Porównaj pasujące, po numerowane okręgi między górnym zrzutem ekranu psc i Partner Center zrzutem ekranu poniżej. Pasujące liczby pokazują, gdzie można znaleźć funkcję lub atrybut związane z funkcją PSC w Partner Center. Czerwone okręgi wskazują, że nie ma pasującego Partner Center pola.  

> [!NOTE]
> Poniżej zrzutów ekranu są wyświetlane inne zagadnienia.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Obraz przedstawiający mapowania pól między widokiem siatki Partner Sales Połączenie (PSC) i widokiem Partner Center transakcji." lightbox="images/pscmigration/grid-view-expanded.png":::

**Zagadnienia specjalne:**

- Nie ma widoku listy w Partner Center jak psc.  Wszystkie transakcje są wyświetlane na podstawie najnowszej odebranej lub utworzonej daty wraz z informacjami o kliencie i typem transakcji. Pierwsza transakcja w widoku jest domyślnie zaznaczona. Większość wartości wyświetlanych w formacie tabeli PSC jest dostępna w szczegółowym widoku transakcji w Partner Center.
- Rola transakcji nie jest polem wymaganym w Partner Center. Nie jest on wyświetlany ani przechwytywany w żadnym z przepływów pracy. Jest ona dawana automatycznie po stronie sprzedawcy firmy Microsoft na podstawie rozwiązań dodanych do transakcji.
- Data ostatniej modyfikacji nie jest wyświetlana na stronie szczegółów polecenia w Partner Center. Partnerzy mogą sortować transakcje na podstawie daty ostatniej aktualizacji za pomocą funkcji sortowania.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 — Widok szczegółów transakcji PSC zamapowany na Partner Center

Porównaj pasujący, numerowany okręg na górnym zrzucie ekranu (PSC) z Partner Center zrzutu ekranu poniżej. Pasujące liczby pokazują, gdzie można znaleźć funkcję lub atrybut związane z funkcją PSC w Partner Center. Czerwone okręgi wskazują, że w Partner Center nie ma pasującego Partner Center.

> [!NOTE]
> Poniżej zrzutów ekranu są wyświetlane inne zagadnienia.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Obraz przedstawiający mapowania pól między widokiem szczegóły transakcji dla Połączenie (PSC) a widokiem Partner Center transakcji." lightbox="images/pscmigration/deal-details-expanded.png":::

**Zagadnienia specjalne:**

- Partnerzy mogą edytować ofertę, wybierając przycisk edycji w widoku szczegółów transakcji partnera (6). Po wybraniu przycisku edycji wszystkie pola staną się edytowalne. Następnie możesz zapisać lub anulować zmiany wprowadzone w transakcji.
- Nie ma możliwości zamknięcia transakcji jako duplikatu w Partner Center.
- Wynik klienta nie jest dostępny w Partner Center. Wszystkie szczegóły związane z interakcjami z klientami można zaktualizować w sekcji Uwagi w Partner Center.
- Szacowana data zamknięcia rozwiązania jest dostępna tylko dla transakcji IOT OEM w Partner Center. Te informacje nie są wyświetlane dla innych typów transakcji.
- Program licencjonowania nie jest wymagany w Partner Center. Te informacje są automatycznie wywnioskowane na podstawie rozwiązań wybranych w transakcji.

>[!Note]
>Nie można później edytować żadnej transakcji oznaczonej jako wygrana lub utracona. Należy zachować ostrożność podczas przenoszenia transakcji do jednego z tych stanów końcowych.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 — Widok "Dodaj produkty" psc zamapowany na widok Partner Center "Dodawanie rozwiązań"

Porównaj pasujący, numerowany okręg na górnym zrzucie ekranu (PSC) z Partner Center zrzutu ekranu poniżej. Pasujące liczby pokazują, gdzie można znaleźć funkcję lub atrybut związane z funkcją PSC w Partner Center. Czerwone okręgi wskazują, że w Partner Center nie ma pasującego Partner Center.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Obraz przedstawiający mapowania pól między widokiem Partner Sales Połączenie (PSC) add products (PSC) add products (Punkt Partner Center widoku dodawania rozwiązań)." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 — Zarządzanie użytkownikami w programie PSC a zarządzanie Partner Center

Porównaj pasujący, numerowany okręg na górnym zrzucie ekranu (PSC) z Partner Center zrzutu ekranu poniżej. Pasujące liczby pokazują, gdzie można znaleźć funkcję lub atrybut związane z funkcją PSC w Partner Center. Czerwone okręgi wskazują, że w Partner Center nie ma pasującego Partner Center.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Obraz przedstawiający mapowania pól między obszarem macierzy Połączenie (PSC) zarządzania użytkownikami partnerów a widokiem strony zarządzania użytkownikami aplikacji Partner Center w obszarze Ustawienia konta."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 — Przypisanie roli użytkownika w konsoli psc a przypisanie Partner Center

Porównaj pasujący, numerowany okręg na górnym zrzucie ekranu (PSC) z Partner Center zrzutu ekranu poniżej. Pasujące liczby pokazują, gdzie można znaleźć funkcję lub atrybut związane z funkcją PSC w Partner Center. Czerwone okręgi wskazują, że w Partner Center nie ma pasującego Partner Center.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Obraz przedstawiający mapowania pól między widokiem przypisania roli Partner Sales Połączenie (PSC) i widokiem przypisania Partner Center partnera." lightbox="images/pscmigration/roles-expanded.png":::

**Zagadnienia specjalne:**

- Równoważną rolą administratora centrum zabezpieczeń jest rola administratora konta w Partner Center.
- Istnieje tylko jedna rola w Partner Center do zarządzania umowami sprzedaży. Ta rola jest rolą administratora poleceń.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 — Powiadomienia w konsoli PSC a powiadomienia Partner Center

Porównaj pasujący, numerowany okręg na górnym zrzucie ekranu (PSC) z Partner Center zrzutu ekranu poniżej. Pasujące liczby pokazują, gdzie można znaleźć funkcję lub atrybut związane z funkcją PSC w Partner Center. Czerwone okręgi wskazują, że w Partner Center nie ma pasującego Partner Center.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Obraz przedstawiający mapowanie między powiadomieniami Partner Sales Połączenie (PSC) i widokiem Partner Center powiadomień."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Przechodzenie z konsoli PSC do Partner Center — często zadawane pytania

Poniższe sekcje zawierają odpowiedzi na często zadawane pytania dotyczące migracji.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 — Co zrobić, jeśli nie mam dostępu do Partner Center?

Aby uzyskać przypisane role, możesz skontaktować się z administratorami wymienionymi na stronie "Brak dostępu". Będziesz potrzebować roli administratora [poleceń dla](permissions-overview.md#manage-referrals) uprawnień do odczytu i zapisu w sekcji polecenia. Jeśli zarządzasz tylko profilami biznesowymi, będziesz potrzebować roli administratora profilu biznesowego w Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Obraz przedstawiający środowisko bez dostępu w Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 — KtoTo udzielić mi dostępu do sekcji Polecenia w Partner Center?

Administrator [konta może](permissions-overview.md#manage-mpn-membership-and-your-company) udzielić Ci dostępu do karty Polecenia. Aby znaleźć administratora konta, wybierz **pozycję Ustawienia konta** za pomocą ikony koła zębatego w prawym górnym rogu pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard) Następnie wybierz pozycję **Zarządzanie użytkownikami** na lewym pasku nawigacyjnym drugiego poziomu. W górnej części listy użytkowników  wybierz menu rozwijane Filtr i zmień opcję na **administratora konta.** Na stronie zostaną wyświetleń wszyscy administratorzy kont wraz z odpowiednimi adresami e-mail. Poproś jedną z nich o przypisanie roli administratora poleceń dla twojego konta służbowego.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 — przycisk +Nowa transakcja jest wyszarytowany dla naszego konta. Co należy zrobić, aby rozpocząć tworzenie transakcji?

Dzieje się tak tylko wtedy, gdy nie ma żadnych rozwiązań gotowych do współpracy dołączonych do organizacji MPN, których używasz w Partner Center. Skontaktuj się z pdm, aby uzyskać poprawiony identyfikator MPN swoich rozwiązań lub utwórz bilet pomocy technicznej z wzmianką o problemie "Przycisk nowej transakcji jest wyszarytowany po migracji psc".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 — Czy mogę przypisać transakcje do określonej osoby z naszej organizacji, na przykład DOC?

Możesz przypisać członków zespołu do określonej transakcji. Nie blokuje to innym administratorom poleceń wyświetlania tych transakcji ani działania na ich podstawie.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 — Czy istnieje widok wszystkich przypisanych mi transakcji?

Możesz użyć funkcji ulubionej, która jest kartą na poziomie użytkownika. Możesz oznaczyć wszystkie transakcje przypisane do Ciebie jako ulubione, aby uzyskać szybki dostęp do transakcji.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 — Czy istnieje widok tylko do odczytu dla transakcji?

Nie, w sekcji poleceń nie ma widoku tylko do odczytu transakcji. Wszyscy administratorzy poleceń będą mieć pełny dostęp do odczytu i zapisu dla wszystkich transakcji.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 — Jak zarejestrować umowę po oznaczaniu jej jako wygranych?

Jeśli transakcja spełnia poniższe kryteria, zostanie wyświetlane okno podręczne, aby rozpocząć [rejestrację transakcji.](./register-deals.md)

- Istnieje rozwiązanie kwalifikujące się do zachęty dołączone do transakcji.
- Sprzedawca firmy Microsoft jest zapraszany do wzięcia udziału w transakcji lub zaprasza Cię do transakcji.
- Karta Microsoft jest w stanie Zaakceptowane lub Wygrane w Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 — Po wybraniu przycisku "+Rejestracja nowej transakcji" w sekcji Rejestracja transakcji pojawia się komunikat o błędzie. Jak mogę zarejestrować moje transakcje?

Przycisk **+Rejestracja** nowej transakcji ma być używany tylko przez partnerów zarejestrowanych w programie ISV Connect w celu zarejestrowania transakcji bez odpowiedniej szansy sprzedaży w Partner Center. W przypadku rejestrowania transakcji z możliwością współpracy sprzedaży zostanie wyświetlone okno podręczne, gdy transakcja zostanie oznaczona jako wygrana i jeśli spełnia kryteria rejestracji transakcji.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 — Czy dodanie organizacji klienta jest obowiązkowe?

Tak, dodawanie organizacji [klienta jest obowiązkowe](./manage-co-sell-opportunities.md#select-your-customer) w Partner Center. Najpierw należy wyszukać lokalizację, w której znajduje się klient. Na podstawie posiadanych szczegółów; Możesz określić dokładną nazwę budynku lub po prostu podać szczegóły miasta. Wyszukiwanie organizacji spowoduje pobranie wszystkich jednostek prawnych zgodnych z wprowadzeniu nazwy, dzięki czemu nie trzeba wprowadzać żadnych szczegółów adresu. Wszystkie szczegóły są wypełniane automatycznie na podstawie wybranej organizacji.

### <a name="10---are-customer-contact-details-mandatory"></a>10 — Czy szczegóły kontaktowe klienta są obowiązkowe?

Zależy od [typu transakcji,](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) który tworzysz. Jeśli po prostu udostępniasz potok i nie potrzebujesz żadnej pomocy od organizacji sprzedaży firmy Microsoft, możesz nie podawać szczegółowych informacji kontaktowych klienta. Jeśli współpracujesz ze sprzedawcą firmy Microsoft, jeśli aktywnie szukasz pomocy od sprzedawcy firmy Microsoft, musisz podać dane kontaktowe klienta. Przed utworzeniem żądania współpracy sprzedaży w użytce należy uzyskać od klienta Partner Center.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 — Ile rozwiązań mogę dodać do transakcji?

Do transakcji można dodać maksymalnie 50 rozwiązań (analogicznych do "produktów" w psc). W odróżnieniu od programu PSC można mieszać rozwiązania z własnych rozwiązań kwalifikujących się do współsprzedaży, własnych jednostki SKU firmy Microsoft i innych kwalifikujących się rozwiązań do współsprzedaży. Nie ma żadnej roli transakcji, która ma być wybrana lub dostępna w Partner Center. W przypadku jednostki SKU firmy Microsoft możesz opcjonalnie dodać ilość i cenę dla każdej jednostki SKU dodanej do transakcji.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 — Kiedy poznam szczegóły sprzedawcy firmy Microsoft po utworzeniu transakcji?

Sprzedawcy firmy Microsoft są przypisywani dopiero po dopasowaniu dokładnego wymagania pomocy podanego podczas tworzenia transakcji z odpowiednią osobą sprzedawcy po stronie firmy Microsoft. Nawet po przypisaniu sprzedawcy firmy Microsoft będą mieć możliwość zaakceptowania lub odrzucenia zaproszenia do współpracy sprzedaży. Tylko jeśli zaproszenie do współpracy sprzedaży zostanie zaakceptowane przez sprzedawcę, transakcja zostanie zaktualizowana o dane kontaktowe sprzedawcy firmy Microsoft. Umowa SLA dla sprzedawców firmy Microsoft, w przypadku których będą działać w sprawie transakcji, wynosi 14 dni. Jest to ta sama umowa SLA, w przypadku których partnerzy muszą działać w oparciu o umowę, zanim przejdzie ona w stan wygaśnięcia.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 — Gdzie mogę znaleźć identyfikator szansy sprzedaży?

Identyfikator szansy sprzedaży w programie PSC jest taki sam jak identyfikator transakcji w Partner Center. Identyfikator transakcji można znaleźć obok nazwy transakcji po otwarciu dowolnej transakcji.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 — Jak mój pdm może uzyskać dostęp do aplikacji Partner Center?

Partner Center są dostępne dla twoich pdmów bezpośrednio w przeciwieństwie do PSC. Istnieje wiele opcji umożliwiających włączenie tej możliwości, o których wspomniano poniżej.

- OCP Szczegółowe informacje — jeśli pliki PDM tylko przeglądają powiązane transakcje i postęp, mogą użyć portalu OCP (One Commercial Partner Szczegółowe informacje) w celu uzyskania widoku organizacji. Jest to narzędzie wewnętrzne i dostępne tylko dla pdmów. Szczegółowe informacje o platformie OCP nie są dostępne dla użytkowników w firmie.
- Użytkownik-gość w programie Partner Center — możesz dodać konto PDM jako użytkownika-gościa w programie Partner Center i przypisać mu rolę administratora poleceń, aby można było wyświetlać polecenia i działać na @microsoft.com nich.
- Tworzenie [nowego](./create-user-accounts-and-set-permissions.md#add-a-new-user) użytkownika w dzierżawie — możesz utworzyć nowego użytkownika we własnej dzierżawie i udostępnić te szczegóły w programie PDM, aby można było wyświetlać polecenia i działać na nich podobnie jak w przypadku innych użytkowników poleceń na Twoim koncie.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Znajdowanie poprawnego identyfikatora MPN, jeśli konto w programie PSC nie jest skojarzone z prawidłowym identyfikatorem MPN

Jeśli jesteś tutaj, ponieważ w programie PSC pojawił się baner z napisem "PsC invalid MPN ID association problem" (Problem nieprawidłowego skojarzenia identyfikatora MPN PSC), jesteś w odpowiednim miejscu. Twoje konto mogło zostać połączone z nieprawidłowym identyfikatorem MPN z następujących powodów

- Twoja firma nie ma konta Partner Center konta.
- Twój pdm popełnił błąd podczas wprowadzania identyfikatora MPN twojego konta w systemach wewnętrznych, które łączyły Twoje konto PSC z kontem Partner Center (identyfikator MPN).
- Twoja firma nie ukończyła migracji z Partner Membership Center (PMC) do Partner Center.

Najpierw znajdź prawidłowy identyfikator MPN, korzystając z poniższych kroków.

1. Zaloguj się do [swojego Partner Center konta.](https://partner.microsoft.com/dashboard)
2. Użyj wskazówek podanych w [dokumentacji ustawień konta,](./partner-center-account-setup.md#locate-your-mpn-id) aby zlokalizować identyfikator MPN.

Poniżej znajduje się zrzut ekranu przedstawiający dokładną lokalizację, w której można znaleźć Partner Center IDENTYFIKATOR MPN.

:::image type="content" source="images/pscmigration/finding-mpn-id.png" alt-text="Obraz przedstawiający ustawienia konta, w których partner może znaleźć swój identyfikator MPN."  lightbox="images/pscmigration/finding-mpn-id.png":::

- Jeśli masz program PDM, poproś go o poprawienie identyfikatora MPN przy użyciu poprawnego identyfikatora MPN z Partner Center konta.
- Jeśli nie masz kontrolera PDM, wyślij wiadomość e-mail na adres podany na banerze PSC z informacjami o koncie PSC widocznymi na banerze PSC i prawidłowym identyfikatorem MPN z twojego Partner Center psc.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Zasoby, które ułatwiają tworzenie transakcji i zarządzanie nimi w Partner Center

Jeśli nie przeczytasz jeszcze tematów pomocy dotyczących współs sprzedaży, następujące zasoby pomogą Ci zarządzać transakcjami w Partner Center.

|**W tym celu**   |**Przeczytaj to**   |
|-----------------------|:-----------------------|
|Omówienie kart i nawigacji na stronie możliwości współpracy sprzedaży|[Nawigowanie po sekcji dotyczącej współpracy sprzedaży](./manage-co-sell-opportunities.md)|
|Wybieranie organizacji klienta z listy D&B |[Wybieranie klienta](./manage-co-sell-opportunities.md#select-your-customer)|
|Modyfikowanie pól w sekcji szczegółów transakcji|[Szczegóły transakcji](./manage-co-sell-opportunities.md#deal-details)|
|Dodawanie członków zespołu do zespołu transakcji|[Dodawanie pracowników](./manage-co-sell-opportunities.md#add-team-members)|
|Odpowiadanie na ofertę co-sell|[Zarządzanie transakcjami sprzedaży](./manage-co-sell-opportunities.md#respond-to-a-co-sell-opportunity)
|Rejestrowanie transakcji, które zostały wygrane w Partner Center |[Rejestrowanie nowej transakcji](./register-deals.md)
|Uzyskaj szczegółowe informacje o poleceniach i dowiedz się, jak działa twoje polecenia |[Szczegółowe informacje o poleceniach](./referral-insights.md)
|Tworzenie profilu biznesowego i zarządzanie nimi|[Zarządzanie profilem biznesowym](./create-a-marketing-profile.md)
|Zarządzanie potencjalnymi klientami dla profilu biznesowego |[Zarządzanie potencjalnymi klientami](./manage-leads.md)|

## <a name="next-steps"></a>Następne kroki


- [Partner Sales Połączenie to Partner Center workbook](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) —skoroszyt do wyrównywania procesów sprzedaży i ról partnerów z nowymi procesami sprzedaży za pośrednictwem Partner Center a partner sales Połączenie.
- [Partner Center —](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) wskazówki dotyczące identyfikowania modelu operacyjnego za pośrednictwem usługi Partner Center do zarządzania potencjalnymi klientami lub możliwościami współpracy sprzedaży i rejestrowania transakcji.
- [Wizualizacja zarządzania poleceniami](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) — wizualizowana instrukcja krok po kroku do zarządzania potencjalnymi klientami i możliwościami współpracy sprzedaży za pośrednictwem Partner Center.
- [Publikowanie i zarządzanie na](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) platformie handlowej — wizualizowane instrukcje krok po kroku dotyczące tworzenia i publikowania ofert oraz zarządzania nimi za pośrednictwem Partner Center na platformie handlowej.
