---
title: Migrowanie z programu Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób partnerzy firmy Microsoft mogą migrować z usługi Partner Sales Connect (PSC) do Centrum partnerskiego i tworzyć oferty wysyłane przez sprzedawców firmy Microsoft lub zarządzać nimi.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: f84ceb4d17be7e02a4380e4da55d7ac199f43515
ms.sourcegitcommit: 2a3fe71ef30fbda25cc70f8f526b3efd2b3df687
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/05/2021
ms.locfileid: "99588754"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Przewodnik po przedsprzedaży w centrum partnerskim (komputer) dla partnerów migrowania z programu Partner Sales Connect (PSC)

**Odpowiednie role**

- Administrator konta
- Administrator odwołań
- Sprzedawca — Partner Sales Connect (PSC)
- Administrator połączenia z partnerem sprzedaży (PSC)
- Menedżer ds. sprzedaży partnera (PSC)

Ten artykuł zawiera wskazówki dotyczące partnerów migrowanych z programu partnerskiego Connect Sales do Centrum partnerskiego, dzięki czemu mogą oni nadal tworzyć i zarządzać ofertami współsprzedaży w centrum partnerskim.

Jak wiadomo, firma utraci dostęp do kontrolera PSC po 31 marca 2021. Nadal jednak znajdziesz wszystko, co chcesz zrobić w centrum partnerskim, takie jak tworzenie transakcji towarzyszących, zarządzanie transakcjami i działanie w przypadku transakcji wysyłanych do Ciebie przez sprzedawcy firmy Microsoft.

Istnieją jednak różnice między nimi. Poniższe wskazówki mogą pomóc zapewnić bezproblemowe przejście do Centrum partnerskiego i bardziej skomplikowane.

>[!Important]
> Jeśli jesteś tutaj, ponieważ zobaczysz transparent na komputerze PSC o migracji, jesteś w odpowiednim miejscu. Ten przewodnik nie ma zastosowania do oceny rozwiązań (SA) i partnerów IOT OEM zarządzających swoimi ofertami na komputerze PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Zanim przejdziesz, co musisz wiedzieć

### <a name="if-you-are-a-psc-admin"></a>Jeśli jesteś administratorem PSC

- Aby zalogować się do [Centrum partnerskiego](https://partner.microsoft.com/), potrzebujesz służbowego adresu e-mail.
- Skonfiguruj swoje konto, korzystając z pomocy [administratora konta](permissions-overview.md)Centrum partnerskiego.
- Dowiedz się, jak sprzedawać w centrum partnerskim, czytając ten dokument.
- Skonfiguruj konta użytkowników w centrum partnerskim dla wszystkich użytkowników komputerów PSC (administratorów, menedżerów transakcji i ról sprzedawcy) i przypisz im [role administratora odwołań](permissions-overview.md).

>[!IMPORTANT]
> Upewnij się, że identyfikator MPN wyświetlany na banerze PSC jest dostępny na liście lokalizacji MPN w centrum partnerskim.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Obraz przedstawiający transparent PSC, w którym partnerzy mogą znaleźć identyfikator MPN.":::

 Aby sprawdzić, czy identyfikator MPN jest wyświetlany jako lokalizacja MPN Centrum partnerskiego, zaloguj się na [pulpicie nawigacyjnym](https://partner.microsoft.com/dashboard)Centrum partnerskiego, a następnie wybierz pozycję **Ustawienia** (ikona koła zębatego) w prawym górnym rogu ekranu, a następnie **Ustawienia konta**. W menu nawigacji po lewej stronie wybierz pozycję **lokalizacje** , aby wyświetlić listę wszystkich identyfikatorów MPN i lokalizacji skojarzonych z kontem Centrum partnerskiego.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Jeśli jesteś menedżerem rozwiązania PSC lub sprzedawcą

- Aby zalogować się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego, potrzebujesz służbowego adresu e-mail.
- Jeśli używasz konta innego niż służbowego na komputerze PSC lub służbowy adres e-mail jest przeznaczony dla innej firmy niż firma partnerska, skontaktuj się z administratorem kontrolera konfiguracji, aby uzyskać pomoc dotyczącą konfigurowania konta.
- Skontaktuj się z administratorem systemu PSC, jeśli skonfigurowano konto Centrum partnerskiego niezależnie od konta, którego używasz do logowania się do komputera PSC.
- Sprawdź, czy masz dostęp do Centrum partnerskiego i sekcji odwołania.
- Przeczytaj ten dokument, aby poznać przepływy pracy i zmiany w centrum partnerskim.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Jako administrator w PSC, są to kolejne kroki

W menu nawigacji po lewej stronie Centrum partnerskiego wybierz opcję **odwołania** . Potwierdź, że możesz uzyskać dostęp do stron odwołań.

  >[!Note]
  > Może być konieczne wylogowanie się z Centrum partnerskiego i ponowne zalogowanie się w celu odświeżenia poświadczeń w celu uzyskania dostępu do stron odwołań.

Jeśli nie widzisz opcji **odwołania** w menu Centrum partnerskiego lub stronach związanych z odwołaniami, skontaktuj się z [administratorem konta](permissions-overview.md) Twojej firmy i poproś o przyznanie dostępu do opcji **odwołania** i powiązanego obszaru.

Aby znaleźć administratora konta firmowego:

1. Wybierz pozycję **Ustawienia konta** z ikony koła zębatego w prawym górnym rogu pulpitu nawigacyjnego Centrum partnerskiego.

1. Wybierz pozycję **Zarządzanie użytkownikami** z poziomu drugiego menu nawigacji po lewej stronie.

1. W górnej części listy użytkowników wybierz menu rozwijane **Filtr** . Zmień opcję na **administrator konta**.

   Na stronie zostaną wyświetlone wszystkie Administratorzy konta z odpowiednimi adresami e-mail. Wyślij jedną z nich i poproś o przypisanie roli administratora odwołań dla Twojego konta służbowego.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Obraz przedstawiający administratorów konta na stronie Zarządzanie użytkownikami ustawień partnera.":::

>[!Important]
>- Jeśli rola obejmuje tylko zarządzanie użytkownikami na komputerze PSC, poproszenie administratora konta firmy o przypisanie roli [administratora konta](permissions-overview.md#manage-mpn-membership-and-your-company) w centrum partnerskim. 
>- Jeśli rola obejmuje również zarządzanie szansami sprzedaży, należy polecić przypisanie roli [administratora odwołań](permissions-overview.md#manage-referrals) .
> - Dobrym pomysłem jest również mianowanie jednego lidera zarządzania zmianami między administratorami PSC. Dzięki temu wszyscy administratorzy PSC będą mogli skontaktować się indywidualnie z administratorami konta Centrum partnerskiego. Zamiast tego lider zarządzania zmianami może być wtedy główną osobą korzystającą z administratora konta Centrum partnerskiego.

## <a name="user-migration"></a>Migracja użytkowników

Po skonfigurowaniu konta w centrum partnerskim Użyj Kreatora migracji użytkowników na stronie z możliwością wspólnej sprzedaży, aby przypisać role Centrum partnerskiego do pracowników firmy.

>[!Note]
> Migracja użytkowników może być przeprowadzana tylko przez [administratorów konta](permissions-overview.md#manage-mpn-membership-and-your-company) Twojej firmy. Jeśli nie masz roli administratora konta, Znajdź administratora konta, który może pomóc w skonfigurowaniu kont użytkowników za pomocą Kreatora migracji użytkowników. Funkcja migracji użytkowników będzie dostępna od 18 listopada 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Obraz przedstawiający Kreatora migracji użytkowników.":::

Administratorzy konta zobaczą link Kreatora migracji użytkowników komputera PSC na stronie z możliwością wspólnej sprzedaży obok podręcznika odwołania. Można zainicjować migrację użytkownika, wybierając link. Aby zainicjować migrację użytkowników, Administratorzy mogą wybrać link. Ten krok migracji użytkowników może wykonać wiele razy, dopóki wszyscy użytkownicy nie zostaną przypisani do odpowiednich ról w centrum partnerskim.

Tabela migracji użytkowników zawiera następujące szczegóły:

- Konto użytkownika — identyfikator E-mail pracownika
- Konto partnera PSC — konto, z którym jest skojarzony pracownik w systemie PSC
- Rola użytkownika PSC — jedna z trzech ról przypisanych do programu na komputerze PSC.
- Lokalizacja komputera MPN — lokalizacja, w której użytkownik będzie miał odpowiednie role komputerów. Konto partnera PSC MPN jest używane do znajdowania równoważnej lokalizacji MPN w centrum partnerskim do przypisywania uprawnień. Cała organizacja oznacza identyfikator vOrg MPN.
- Rola użytkownika komputera — pracownicy są przypisani do ról na podstawie ich ról użytkownika kontrolera systemu. Administrator na komputerze PSC zostanie przypisany do ról administratorów na komputerach. Sprzedawca zostanie przypisany do roli użytkownika z odwołaniami na komputerze. Dowiedz się więcej o rolach komputera i o tym, co użytkownicy z tymi rolami mogą wykonać w centrum partnerskim [tutaj](permissions-overview.md#manage-referrals)
- Dzierżawa komputera usługi AAD — dzierżawa, do której użytkownicy są przypisani w centrum partnerskim
- Stan — istnieją trzy możliwe stany migracji stanu
    - **Nie przeprowadzono migracji** — użytkownik nie ma przypisanej roli żadnych odwołań komputera
    - **Migracja** — użytkownik został pomyślnie zmigrowany z odpowiednimi przypisanymi rolami, jak pokazano w tabeli
    - **Błąd** — nie można ukończyć migracji z powodu błędu

Czasami migracja może zakończyć się niepowodzeniem i spowodować błędy. Poniżej przedstawiono kilka powodów, dla których migracja może spowodować błąd i niektóre sposoby rozwiązania problemu:

1. Użytkownicy PSC mogą korzystać z konta innego niż konto służbowe.

2. Użytkownik PSC może korzystać z konta z domeny innej niż ta, która jest używana w centrum partnerskim.

   Aby rozwiązać problemy związane z scenariuszami 1 i 2, poproszenie użytkownika o zalogowanie się do Centrum partnerskiego przy użyciu konta służbowego dołączonego do dzierżawy usługi Azure AD. [Administrator globalny](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) może pomóc.
   
   Aby znaleźć administratora globalnego: 
   - Zaloguj się na [pulpicie nawigacyjnym](https://partner.microsoft.com/dashboard) Centrum partnerskiego i wybierz pozycję **Ustawienia konta** z ikony koła zębatego w prawym górnym rogu.
   - Wybierz pozycję **Zarządzanie użytkownikami** na pasku nawigacyjnym drugiego poziomu, po lewej stronie.
   - W górnej części listy użytkownik Wybierz menu rozwijane **Filtr** i zmień opcję na **administrator globalny**. Następnie na stronie zostaną wyświetlone wszystkie Administratorzy globalni z odpowiednimi adresami e-mail. Poproś jednego z nich, aby przypisać rolę administratora odwołania dla konta służbowego.
   
      Administrator globalny może utworzyć nowe konto użytkownika w dzierżawie usługi Azure AD lub przypisać dostęp użytkownika-gościa do innych użytkowników konta domeny. Po skonfigurowaniu kont dla wszystkich menedżerów i użytkowników z systemem PSC należy zalogować się do Centrum partnerskiego, wybrać **odwołania** z menu nawigacji po lewej stronie, a następnie potwierdzić, że mogą wyświetlić stronę odwołania.

3. Użytkownik ma już przypisaną rolę odwołania w centrum partnerskim.
    - Istnieje możliwość zweryfikowania istniejącej roli użytkownika. W prawym górnym rogu Centrum partnerskiego wybierz opcję **Ustawienia** (ikona koła zębatego), a następnie pozycję **Ustawienia konta**. Gdy zobaczysz drugie menu nawigacji po lewej stronie, wybierz pozycję **Zarządzanie użytkownikami** i Wyszukaj użytkownika.

## <a name="psc-deals-migration"></a>Migracja transakcji PSC

Po zakończeniu migracji użytkowników Użyj Kreatora migracji transakcji na stronie z możliwością współsprzedaży, aby uzyskać wszystkie kwalifikujące się otwarte transakcje z komputera PSC na komputerze. **Link migracji transakcji będzie widoczny tylko dla administratorów odwołań mających cały zakres organizacji w centrum partnerskim.** W prawym górnym rogu strony z możliwością współsprzedaży zostanie utworzone łącze **"Migracja transakcji PSC"** , co spowoduje otwarcie Kreatora migracji transakcji.

Przeczytaj tę sekcję przed rozpoczęciem migracji transakcji.

**Kwalifikuje się do migracji**

Tylko niektóre oferty są uprawnione do migracji z komputera PSC na komputer. Ten Kreator migracji został utworzony w celu ułatwienia partnerom przełączenia ich do Centrum partnerskiego, gdzie nadal aktywnie pracują z klientami w celu zamknięcia transakcji. **Tylko transakcje, które są w stanie otwartym z prawidłowymi szczegółami konta partnera (prawidłowym IDENTYFIKATORem MPN) i nie przechodzą rejestracji transakcji, kwalifikują się do migracji.**

**Nie kwalifikuje się do migracji**

- Oferty oceny rozwiązania nie kwalifikują się do migracji transakcji
- Oferty firmy OEM dotyczące licencjonowania nie są uprawnione do migracji transakcji
- Wszystkie transakcje oznaczone jako kupione na komputerze PSC nie kwalifikują się do migracji. Rejestracja transakcji, jeśli kwalifikuje się do transakcji oznaczonych jako wygrane, powinna zostać zakończona na komputerze PSC.

## <a name="pre-requisites-for-deal-migration"></a>Wymagania wstępne dotyczące migracji transakcji

Przed rozpoczęciem migracji transakcji z komputera postępuj zgodnie z poniższymi instrukcjami, aby skonfigurować te transakcje na komputerze PSC dla pomyślnej migracji.

1. Wszyscy członkowie zespołu sprzedaży w firmie, którzy pracują nad otwartymi transakcjami, są informowani o tej migracji.
2. Członkowie zespołu ds. sprzedaży są przeszkoleni do korzystania z usługi Partner Center w celu zarządzania okazjami.
3. Wszystkie wymagane informacje są podane poniżej.
    - Szczegóły firmy klienta, w tym nazwa i adres
    - Szczegóły kontaktowe klienta, jeśli jest to transakcja do sprzedaży
    - Co najmniej jedno rozwiązanie
    - Co najmniej jeden członek zespołu ze wszystkimi szczegółami — imię i nazwisko, nazwisko, adres e-mail i numer telefonu
    - Wartość transakcji
    - Szacowana data zamknięcia transakcji
    - Uwagi dla partnerów

Możesz użyć funkcji pobierania zbiorczego i przekazywania danych na komputerze PSC, aby wyczyścić dane dla wszystkich kwalifikujących się transakcji.

>[!Note]
> Migracja transakcji powiedzie się, nawet jeśli powyższe wymagania wstępne nie są spełnione. Nie można jednak zmienić stanu transakcji, jeśli którykolwiek z powyższych pól wymaganych w centrum partnerskim nie jest dostępny. Następnie będzie trzeba wprowadzić wszystkie wymagane informacje w centrum partnerskim, aby rozpocząć pracę nad nimi. **Zdecydowanie zaleca się oczyszczenie kwalifikujących się operacji na komputerze PSC przed przeprowadzeniem migracji ich do Centrum partnerskiego.**

Migracja transakcji w centrum partnerskim jest oparta na jednym doświadczeniu. Wystarczy kliknąć przycisk **"Migruj oferty"** , gdy firma będzie gotowa do migracji kwalifikujących się transakcji. **Nie można wybrać transakcji, które mają być migrowane z komputera PSC. Jeśli nie chcesz migrować żadnych transakcji do Centrum partnerskiego, przenieś je do stanu zamkniętego na komputerze PSC przed rozpoczęciem migracji.**

>[!Note]
> Po zainicjowaniu migracji **może upłynąć nawet 24 godziny, aby można było przeprowadzić migrację**.

Po zakończeniu migracji komunikat transparentu będzie miał stan zmieniony na zakończony przy użyciu linku do raportu migracji. Pobierz raport, aby wyświetlić szczegóły dotyczące transakcji, które zostały zmigrowane z systemu PSC do komputera.

Raport zawiera poniższe szczegóły.

1. **Identyfikator zaangażowania Centrum partnerskiego** — unikatowy identyfikator w centrum partnerskim dla wszystkich transakcji w ramach zaangażowania. Istnieją dwie oferty — jeden dla partnera i jeden dla firmy Microsoft w ramach współsprzedawcy w centrum partnerskim.
2. **Identyfikator odwołania Centrum partnerskiego** — unikatowy identyfikator w centrum partnerskim dla transakcji należącej do partnera.
3. **Nazwa transakcji** — identyfikator nadany w ramach umowy PSC.
4. **Identyfikator transakcji PSC** — unikatowy identyfikator na komputerze PSC dla transakcji.
5. **Błędy** — aby wskazać, czy wystąpił błąd podczas migrowania konkretnej transakcji.

Wszystkie transakcje, które zostały pomyślnie zmigrowane, nie będą widoczne na komputerze PSC. Możesz korzystać z zmigrowanych transakcji na komputerze. Brak zmian w interakcjach ze sprzedawcami firmy Microsoft w przypadku transakcji związanych z współsprzedażą.

Transakcje migrowane z komputera PSC będą dostępne na kartach przychodzących i wychodzących na podstawie źródła transakcji. Wszystkie oferty utworzone przez partnera będą dostępne na karcie wychodzące, a transakcje zainicjowane przez firmę Microsoft będą dostępne na karcie przychodzące w centrum partnerskim. Istnieją dwa typy transakcji, które zostaną utworzone po migracji.

1. **Oferty towarzyszące** rozdaniom, które są oznaczone jako współsprzedażowe na komputerze PSC, zostaną utworzone jako sprzedaż w centrum partnerskim.
2. **Oferty dla partnerów** — transakcje, które nie zostały oznaczone jako towarzyszące, zostaną utworzone jako oferty partnerskie w centrum partnerskim. Transakcje dotyczące partnerskich partnerów są widoczne dla sprzedawcy firmy Microsoft i można je uaktualnić do transakcji współsprzedawanych przed osiągnięciem stanu terminalu (wygranych, utraconych). Ponadto w przypadku oferty uprawniającego do korzystania z platformy partnerskiej usługi mogą skorzystać z rejestracji transakcji.

>[!Important]
> Jeśli występują błędy, z powodu których nie można migrować niektórych transakcji, **można ponownie zainicjować migrację transakcji, klikając przycisk "Migrowanie transakcji"**. Zostanie ona włączona tylko wtedy, gdy istnieją pewne kwalifikujące się do migracji. Ta wartość będzie również przydatna, jeśli jesteś w fazie przejścia, w której nowe oferty są tworzone w komputerze PSC po zainicjowaniu migracji transakcji.

Po pomyślnym przeprowadzeniu migracji wszystkich transakcji **zostanie wyświetlony transparent** z informacją o tym, że przycisk **"Migrowanie transakcji"** jest **wyłączony**.

Po zakończeniu migracji użytkowników i/lub przeprowadzeniu migracji należy skorzystać z poniższych wskazówek, aby określić strategię migracji:

Jeśli Twoja firma ma Menedżera deweloperów rozwiązań (PDM) — po skonfigurowaniu konta Centrum partnerskiego i przeniesieniu użytkowników do swoich ról i uprawnień możesz przenieść swoje działania towarzyszące do Centrum partnerskiego. Przed upływem ostatecznego terminu migracji poinformuj PDM o tym, aby przełączać się do programu, co pozwoli na przepływ wszystkich nowych transakcji do Centrum partnerskiego.

>[!Note]
>Po dokonaniu tego przełącznika będzie można działać tylko na istniejących aktywnych okazjach na komputerze PSC. Nie można tworzyć nowych transakcji ani otrzymywać żadnych transakcji od sprzedawcy firmy Microsoft na komputerze PSC.

Jeśli firma nie ma PDM — upewnij się, że wszystkie konta użytkowników zostały skonfigurowane i zweryfikowane przez wszystkich użytkowników. Otrzymasz powiadomienie za pośrednictwem wiadomości e-mail i transparentu na komputerze PSC w sprawie dokładnej daty rozpoczęcia sprzedaży w centrum partnerskim. Pamiętaj, że nadal będziesz mieć możliwość zarządzania istniejącymi aktywnymi transakcjami na komputerze PSC.

>[!Important]
>Aktywne transakcje nie będą migrowane do komputera. Do 31 marca 2021 należy zamknąć i zarejestrować oferty.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Następne kroki dla administratorów PSC, menedżerów transakcji PSC i sprzedawcy PSC

Dowiedz się, jak sprzedawać w centrum partnerskim.
Jest to ważny krok, który pomoże Ci przygotować się do sprzedaży w centrum partnerskim. Zapoznaj się z przepływami pracy i zmianami w centrum partnerskim, dzięki czemu możesz efektywnie współsprzedawać. Zacznij od pełnego przeczytania tego dokumentu. Dobry zestaw zasobów jest również dostępny w [galerii z możliwością współsprzedażowej](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Główne różnice między systemem PSC a przepływami pracy komputera

|**Scenariusz**|**Połączenie z partnerem sprzedaży**|**Centrum partnerskie**|
|-----|:-----|:-----|
|Role użytkownika|Kontroler PSC ma role Administrator, Menedżer transakcji i sprzedawca.|Komputer PC ma tylko rolę [administratora odwołań](permissions-overview.md#manage-referrals) , która nadaje uprawnienia do odczytu i zapisu dla wszystkich transakcji.|
|Zapraszanie firmy Microsoft do rozdzielenia transakcji|Zainicjowany przez sprzedawcę firmy Microsoft nie ma jawnego podawania przez partnera.|Jeśli potrzebujesz pomocy sprzedającej firmy Microsoft, Partner będzie musiał wykonać [jawne żądanie](manage-co-sell-opportunities.md#add-solutions) . Sprzedawca firmy Microsoft ma możliwość odrzucania żądania.|
|Wygaśnięcie|Nie ma koncepcji wygaśnięcia transakcji.|Transakcje przychodzące partnerów wygasną w ciągu 14 dni, jeśli nie zostaną zaakceptowane przez partnera. Jest to sytuacja, w której w przypadku transakcji wychodzących przez partnera można przejść do stanu wygasłego, jeśli sprzedawca firmy Microsoft nie działa na nich w ciągu 14 dni.|
|Szczegóły sprzedawcy firmy Microsoft|Widoczne, gdy tylko zostanie utworzona transakcja.|Szczegóły sprzedawcy firmy Microsoft są udostępniane partnerom tylko wtedy, gdy sprzedający jawnie zaakceptuje zaproszenie do sprzedaży od partnera.|
|[Potok prywatny](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Niedostępne.|Partnerzy mogą udostępniać swój potok bez podawania wglądu dla sprzedawcy firmy Microsoft.|
|Rozwiązania|Rozwiązania należące do tylko jednej z cennika można dodać do transakcji.|Partner może dodawać [rozwiązania](manage-co-sell-opportunities.md#add-solutions) , które należą do poniższych list. a) ich własne rozwiązania b) — rozwiązania z wykazu pierwszej firmy Microsoft (podobnie jak rola transakcji w systemie PSC) i c) współsprzedawanych rozwiązań od innych partnerów innych firm (podobnie jak w przypadku roli klient niezależnego dostawcy oprogramowania).|
|Przypisanie transakcji|Tylko przypisani sprzedawcy mogą wyświetlać i podejmować działania w ramach transakcji.|Członkowie zespołu mogą zostać dodani do transakcji, aby określić osoby pracujące nad transakcjami, nie ma możliwości blokowania innych administratorów odwołań ani działania nad nimi.|
|Organizacja klienta|Wpis tekstu w postaci bezpłatnej.|Możesz przeszukać [organizację klienta](manage-co-sell-opportunities.md#select-your-customer) w [bazie danych D&B](https://www.dnb.com/) , wpisując kilka znaków. Legalna nazwa i adres są wypełniane automatycznie na podstawie wyboru.|
|Kontakt z klientem|Nieobowiązkowe.|Nieobowiązkowe dla prywatnego udostępniania potoku. Wymagane, jeśli sprzedawca firmy Microsoft jest zapraszany do wzięcia udziału w żądaniu współsprzedaży.|
|Publiczny interfejs API|Niedostępne.|[Publiczny interfejs API](/partner/develop/referrals) umożliwiający programowe Zarządzanie odwołaniami do Centrum partnerskiego.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mapuj pola na komputerze PSC do odpowiednich pól w centrum partnerskim

W tej sekcji porównano wybrane zrzuty ekranu (lub "Maps") dla komputera PSC z odpowiednim widokiem w sekcji możliwości wspólnej sprzedaży w centrum partnerskim.

Na każdej parze zrzutów ekranu będą widoczne okrągłe, żółte lub czerwone kółka:

- **Co oznaczają żółte koła?** Ponumerowane, żółte kółka są pierwsze na każdym zrzucie ekranu komputera PSC. Następnie znajdziesz zrzut ekranu centrum partnera pomocniczego poniżej tego z wieloma tymi samymi numerami.

   Aby zobaczyć, w jaki sposób każde pole lub atrybut w elemencie PSC mapuje na jego odpowiednik w centrum partnerskim, Dopasuj do ponumerowanych okręgów w dwóch powiązanych zrzutach ekranu. Na przykład Dopasuj do ponumerowanego, żółtego "1" pierwszego zrzutu ekranu PSC do numerowanego, żółtego "1" w drugim, na poniższym zrzucie ekranu Centrum partnerskiego.

- **Co oznacza czerwony okrąg?** Jeśli zobaczysz czerwony okrąg na jednym zrzucie ekranu, oznacza to, że pole PSC nie jest dostępne w centrum partnerskim.

Mapowania pola PSC na partnera są wyświetlane dla następujących obszarów:

1. Strona główna kontrolera PSC zamapowana na widok domyślny możliwości wspólnej sprzedaży do Centrum partnerskiego
1. Widok siatki komputera PSC mapowany do widoku transakcji Centrum partnerskiego
1. Widok szczegółów transakcji komputera PSC zamapowany do widoku szczegółów transakcji Centrum partnerskiego
1. Widok ustawień PSC Dodaj produkty zamapowany do widoku Dodawanie rozwiązań Centrum partnerskiego
1. Widok zarządzania użytkownikami komputera PSC mapowany do widoku zarządzania użytkownikami Centrum partnerskiego
1. Widok przypisania roli użytkownika komputera PSC zamapowany na widok przypisania roli Centrum partnerskiego
1. Widok powiadomień PSC mapowany na Widok powiadomień Centrum partnerskiego

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>Strona główna z 1-kontrolerem PSC zamapowana na widok domyślny możliwości wspólnej sprzedaży do Centrum partnerskiego

Porównaj pasujące, numerowane okręgi między górnym ekranem PSC a zrzutem ekranu Centrum partnerskiego poniżej. Pasujące numery pokazują, gdzie można znaleźć funkcję lub atrybut związany z kontrolerem PSC w centrum partnerskim. Czerwone kółka wskazują, że nie ma pasującego pola Centrum partnerskiego.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Obraz przedstawiający Mapowanie pól między stroną główną programu partnerskiego połączenia z partnerem sprzedaży a domyślnym widokiem możliwości wspólnej sprzedaży w centrum partnerskim." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>Widok siatki 2-PSC zamapowany na widok transakcji Centrum partnerskiego

Porównaj pasujące, numerowane okręgi między górnym ekranem PSC a zrzutem ekranu Centrum partnerskiego poniżej. Pasujące numery pokazują, gdzie można znaleźć funkcję lub atrybut związany z kontrolerem PSC w centrum partnerskim. Czerwone kółka wskazują, że nie ma pasującego pola Centrum partnerskiego.  

> [!NOTE]
> Inne zagadnienia są wyświetlane poniżej zrzutów ekranu.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem siatki Połącz z partnerem sprzedaży partnera (PSC) i widokiem transakcji Centrum partnerskiego." lightbox="images/pscmigration/grid-view-expanded.png":::

**Uwagi specjalne:**

- W centrum partnerskim nie ma widoku listy, takiego jak kontroler PSC.  Wszystkie transakcje są wyświetlane na podstawie najnowszej otrzymanej lub utworzonej daty z informacjami o kliencie i typem transakcji. Pierwsza transakcja w widoku jest domyślnie zaznaczona. Większość wartości, które są wyświetlane w formacie tabeli PSC, są dostępne w widoku szczegółowym transakcji na komputerze.
- Rola transakcji nie jest polem wymaganym na komputerze. Nie jest on wyświetlany ani przechwytywany w żadnym przepływie pracy. Jest ona tworzona automatycznie na stronie sprzedawcy firmy Microsoft w oparciu o rozwiązania dodane do transakcji.
- Data ostatniej modyfikacji nie jest wyświetlana na stronie szczegółów odwołania na komputerze. Partnerzy mogą używać funkcji sortowania do sortowania transakcji na podstawie daty ostatniej aktualizacji.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>Widok szczegółów transakcji z 3-kontrolerem PSC mapowany do Centrum partnerskiego

Porównaj pasujące, numerowane okręgi na górnym zrzucie ekranu (PSC) przy użyciu zrzutu ekranu centrum partnera poniżej. Pasujące numery pokazują, gdzie można znaleźć funkcję lub atrybut związany z kontrolerem PSC w centrum partnerskim. Czerwone kółka wskazują, że w centrum partnerskim nie ma dopasowanego pola lub obszaru.

> [!NOTE]
> Inne zagadnienia są wyświetlane poniżej zrzutów ekranu.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem szczegółów rozdziału partnera sprzedaży (PSC) i widokiem szczegółów transakcji Centrum partnerskiego." lightbox="images/pscmigration/deal-details-expanded.png":::

**Uwagi specjalne:**

- Partnerzy mogą edytować ofertę, wybierając przycisk Edytuj w widoku szczegółów transakcji partnera (6). Po wybraniu przycisku Edytuj wszystkie pola staną się edytowalne. Następnie można zapisać lub anulować zmiany wprowadzone w ramach transakcji.
- Nie ma możliwości zamknięcia transakcji jako duplikatu w centrum partnerskim.
- Wynik klienta nie jest dostępny w centrum partnerskim. Wszystkie szczegóły dotyczące interakcji z klientami można zaktualizować w sekcji notatki na komputerze.
- Szacowana data zamknięcia rozwiązania jest dostępna tylko w przypadku transakcji związanych z producentem OEM w centrum partnerskim. Te informacje nie są wyświetlane dla żadnych innych typów transakcji.
- Program licencjonowania nie jest wymagany na komputerze. Te informacje są wywnioskowane na podstawie rozwiązań wybranych w ramach transakcji.

>[!Note]
>Wszystkie transakcje oznaczone jako wygrane lub utracone nie mogą być edytowane później. Podczas przechodzenia do jednego z tych stanów terminalu należy zachować ostrożność.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>Widok "Dodaj produkty" z 4 kontrolerami PSC zamapowany do widoku "Dodaj rozwiązania" Centrum partnerskiego

Porównaj pasujące, numerowane okręgi na górnym zrzucie ekranu (PSC) przy użyciu zrzutu ekranu centrum partnera poniżej. Pasujące numery pokazują, gdzie można znaleźć funkcję lub atrybut związany z kontrolerem PSC w centrum partnerskim. Czerwone kółka wskazują, że w centrum partnerskim nie ma dopasowanego pola lub obszaru.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem Dodawanie produktów partnera (PSC) do programu oraz widok dodawania rozwiązań Centrum partnerskiego." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 — Zarządzanie użytkownikami na komputerze PSC a centrum partnerskim

Porównaj pasujące, numerowane okręgi na górnym zrzucie ekranu (PSC) przy użyciu zrzutu ekranu centrum partnera poniżej. Pasujące numery pokazują, gdzie można znaleźć funkcję lub atrybut związany z kontrolerem PSC w centrum partnerskim. Czerwone kółka wskazują, że w centrum partnerskim nie ma dopasowanego pola lub obszaru.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Obraz przedstawiający Mapowanie pól między domem (Partner Sales Connect) — Strona główna i widok strony zarządzania użytkownikami Centrum partnerskiego w obszarze Ustawienia konta."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 — przypisanie roli użytkownika na komputerze PSC a centrum partnerskie

Porównaj pasujące, numerowane okręgi na górnym zrzucie ekranu (PSC) przy użyciu zrzutu ekranu centrum partnera poniżej. Pasujące numery pokazują, gdzie można znaleźć funkcję lub atrybut związany z kontrolerem PSC w centrum partnerskim. Czerwone kółka wskazują, że w centrum partnerskim nie ma dopasowanego pola lub obszaru.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem przypisywania roli Partner Sales Connect (PSC) i widok przypisania roli Centrum partnerskiego." lightbox="images/pscmigration/roles-expanded.png":::

**Uwagi specjalne:**

- Równoważną rolę administratora PSC jest rola administratora konta w centrum partnerskim.
- Istnieje tylko jedna rola w centrum partnerskim do zarządzania transsprzedażą. Ta rola jest rolą administratora odwołań.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 — powiadomienia w kontrolerach PSC a centrum partnerskie

Porównaj pasujące, numerowane okręgi na górnym zrzucie ekranu (PSC) przy użyciu zrzutu ekranu centrum partnera poniżej. Pasujące numery pokazują, gdzie można znaleźć funkcję lub atrybut związany z kontrolerem PSC w centrum partnerskim. Czerwone kółka wskazują, że w centrum partnerskim nie ma dopasowanego pola lub obszaru.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Obraz przedstawiający mapowanie między powiadomieniami partnera (Partner Sales Connect) i widokiem powiadomień Centrum partnerskiego."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Przejście z komputera PSC do Centrum partnerskiego — często zadawane pytania

W poniższych sekcjach znajdują się odpowiedzi na często zadawane pytania dotyczące migracji.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 — co mam zrobić, jeśli nie mam dostępu do Centrum partnerskiego?

Aby uzyskać przypisane role, możesz skontaktować się z administratorami na liście na stronie "Brak dostępu". W sekcji odwołania będzie potrzebna rola [administratora odwołań](permissions-overview.md#manage-referrals) dla uprawnień do odczytu i zapisu. Jeśli zarządzasz tylko profilami biznesowymi, w centrum partnerskim będzie potrzebna rola administratora profilu biznesowego.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Obraz przedstawiający sposób braku dostępu w centrum partnerskim.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 — kto może udzielić dostępu do sekcji odwołań w centrum partnerskim?

[Administrator konta](permissions-overview.md#manage-mpn-membership-and-your-company) może udzielić dostępu do karty odwołania. Aby znaleźć administratora konta, wybierz pozycję **Ustawienia konta** z ikony koła zębatego w prawym górnym rogu [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego. Następnie wybierz pozycję **Zarządzanie użytkownikami** na pasku nawigacyjnym drugiego poziomu, po lewej stronie. W górnej części listy użytkownik Wybierz menu rozwijane **Filtr** i zmień opcję na wartość **administrator konta**. Na stronie zostaną wyświetlone wszystkie Administratorzy konta z odpowiednimi adresami e-mail. Poproś jednego z nich, aby przypisać rolę administratora odwołania dla konta służbowego.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 — przycisk + Nowa transakcja jest wyszarzony dla naszego konta. Co należy zrobić, aby zacząć tworzyć oferty?

Dzieje się tak tylko wtedy, gdy nie ma żadnych gotowych do zakupu rozwiązań do organizacji MPN, które są używane w centrum partnerskim. Skontaktuj się z PDM, aby uzyskać poprawiony identyfikator MPN rozwiązań, lub Utwórz bilet pomocy technicznej z informacją o problemie "nowy przycisk transakcji jest wyszarzony po migracji PSC".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 — Czy mogę przypisywać oferty do określonej osoby z naszej organizacji, takiej jak PSC?

Można przypisać członków zespołu do konkretnej transakcji. Nie blokuje ona wyświetlania ani działania innych administratorów odwołań do tych transakcji.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 — czy istnieje widok wszystkich przypisanych do mnie okazji?

Możesz użyć funkcji Ulubione, która jest kartą na poziomie użytkownika. Możesz oznaczyć wszystkie oferty, które są przypisane do Ciebie jako Ulubione, aby uzyskać szybki dostęp do tych transakcji.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 — czy istnieje widok tylko do odczytu dla transakcji?

Nie. w sekcji odwołania nie ma widoku tylko do odczytu transakcji. Wszyscy administratorzy odwołań będą mieć pełny dostęp do odczytu i zapisu do wszystkich transakcji.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 — Jak mogę zarejestrować ofertę po oznaczeniu jej jako wygranej?

Jeśli transakcja spełnia poniższe kryteria, zostanie wyświetlone okno podręczne, aby rozpocząć [rejestrację transakcji](./register-deals.md).

- Istnieje rozwiązanie uprawniające do oferty.
- Sprzedawca firmy Microsoft jest zapraszany do wzięcia udziału w transakcji lub zaprosił Cię do zawarcia umowy.
- Karta Microsoft jest w stanie zaakceptowana lub wygrana w centrum partnerskim.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 — otrzymuję komunikat o błędzie w przypadku wybrania przycisku "+ Nowa rejestracja transakcji" w sekcji Rejestracja transakcji. Jak mogę zarejestrować moje transakcje?

Przycisk **+ nowy proces rejestracji transakcji** ma być używany tylko przez partnerów zarejestrowanych w programie do łączenia niezależnych dostawców oprogramowania w celu zarejestrowania transakcji bez odpowiadającej jej szansy sprzedaży w centrum partnerskim. W celu zarejestrowania transakcji z możliwością współsprzedaży zostanie wyświetlone okno podręczne, gdy transakcja zostanie oznaczona jako wykorzystana i będzie spełniać kryteria rejestracji transakcji.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 — Dodawanie organizacji klienta jest obowiązkowe?

Tak, dodanie [organizacji klienta](./manage-co-sell-opportunities.md#select-your-customer) jest obowiązkowe w centrum partnerskim. Najpierw Zacznij od wyszukania lokalizacji, w której znajduje się klient. Na podstawie szczegółowych informacji; można określić, w tym dokładną nazwę budynku, lub po prostu podać szczegóły miasta. W ramach wyszukiwania organizacji zostaną pobrane wszystkie jednostki prawne pasujące do wprowadzonej nazwy, aby nie trzeba było wprowadzać żadnych szczegółowych informacji o adresie. Wszystkie szczegóły są wypełniane automatycznie w oparciu o wybraną organizację.

### <a name="10---are-customer-contact-details-mandatory"></a>10 — czy dane kontaktowe klienta są obowiązkowe?

Zależy od typu tworzonej [transakcji](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) . Jeśli po prostu udostępniasz swój potok i nie potrzebujesz pomocy od organizacji sprzedaży firmy Microsoft, możesz zrezygnować z podawania szczegółów kontaktowych klienta. Jeśli sprzedajesz, gdzie aktywnie szukasz pomocy od sprzedawcy firmy Microsoft, konieczne będzie podanie szczegółowych informacji kontaktowych klienta. Przed utworzeniem żądania współsprzedaży w centrum partnerskim należy uzyskać jawną zgodę od klienta.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 — ile rozwiązań można dodać do transakcji?

Do rozpatrzenia można dodać do 50 rozwiązań (analogicznie do "produktów" w PSC). W przeciwieństwie do systemu PSC, możesz mieszać rozwiązania z własnych, oferowanych przez siebie rozwiązań, jednostek SKU pierwszej firmy Microsoft oraz innych firmowych rozwiązań do sprzedawania. Nie ma roli transakcji, która ma być wybrana lub dostępna w centrum partnerskim. W przypadku jednostek SKU firmy Microsoft można opcjonalnie dodać ilość i cenę dla każdej jednostki SKU, która jest dodawana do transakcji.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 — gdy otrzymasz informacje o sprzedawcy firmy Microsoft po utworzeniu transakcji?

Sprzedawcy firmy Microsoft są przypisani dopiero po dopasowaniu dokładnego wymagania dotyczącego pomocy, które zostały podane podczas tworzenia transakcji z odpowiednią osobą sprzedającą po stronie firmy Microsoft. Nawet po przypisaniu sprzedawcy firmy Microsoft będą mogli zaakceptować lub odrzucić zaproszenie do współsprzedażu. W przypadku zaakceptowania przez sprzedawcę zaproszenia do sprzedaży zostanie ona zaktualizowana informacjami o kontaktach sprzedawcy firmy Microsoft. Umowa SLA dla sprzedawcy firmy Microsoft do działania w ramach umowy wynosi 14 dni. Jest to ta sama umowa SLA, którą partnerzy muszą podejmować działania w odniesieniu do stanu sprzed wygaśnięcia.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 — gdzie mogę znaleźć identyfikator szansy sprzedaży?

Identyfikator szansy sprzedaży w PSC jest taki sam jak identyfikator transakcji na komputerze. Identyfikator transakcji można znaleźć obok nazwy transakcji po otwarciu każdej transakcji.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14 — jak mój PDM może uzyskać dostęp do komputera?

Nie można uzyskać dostępu do Centrum partnerskiego za pomocą PDM bezpośrednio w przeciwieństwie do komputera PSC. Istnieje wiele opcji umożliwiających tę możliwość, które są wymienione poniżej.

- OCP Insights — Jeśli PDM wyświetlają tylko te transakcje i postęp związany z nimi, mogą korzystać z portalu OCP Insights w celu uzyskania widoku organizacji. Jest to narzędzie wewnętrzne i dostępne tylko dla PDM. Pamiętaj, że w firmie OCP Insights nie są dostępne dla użytkowników Twojej firmy.
- Użytkownik-Gość w centrum partnerskim — możesz dodać @microsoft.com konto PDM jako użytkownika-gościa w centrum partnerskim i przypisać do nich rolę administratora odwołań, aby mogli oni wyświetlać i podejmować działania dotyczące odwołań.
- Tworzenie [nowego użytkownika](./create-user-accounts-and-set-permissions.md#add-a-new-user) w dzierżawie — możesz utworzyć nowego użytkownika w swojej dzierżawie i udostępnić te szczegóły w PDM, aby mogły wyświetlać i działać na odwołaniach podobnych do innych użytkowników referencyjnych na Twoim koncie.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Znajdowanie prawidłowego identyfikatora MPN, jeśli konto w systemie PSC nie jest skojarzone z prawidłowym MPN

Jeśli jesteś tutaj, ponieważ zobaczysz baner na komputerze PSC z informacją o problemie związanym z skojarzeniem "PSC nieprawidłowy identyfikator MPN", jesteś w odpowiednim miejscu.

Najpierw Znajdź prawidłowy identyfikator MPN, postępując zgodnie z poniższymi instrukcjami.

- Zaloguj się do konta Centrum partnerskiego
- Aby zlokalizować identyfikator MPN, skorzystaj ze wskazówek zawartych w [dokumentacji ustawień konta](./partner-center-account-setup.md#locate-your-mpn-id) .

Dalej,

- Jeśli masz PDM, poproś o podanie identyfikatora MPN z prawidłowym IDENTYFIKATORem MPN z konta Centrum partnerskiego.
- Jeśli nie masz PDM, Wyślij wiadomość e-mail na adres podany na banerze PSC z informacjami o kontach PSC wyświetlanymi na banerze PSC oraz prawidłowym IDENTYFIKATORem MPN z konta Centrum partnerskiego.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Zasoby ułatwiające tworzenie i zarządzanie ofertami w centrum partnerskim

Jeśli nie odczytano jeszcze tematów pomocy dotyczących współsprzedawcy, następujące zasoby ułatwią zarządzanie nimi w centrum partnerskim.

|**Aby to zrobić**   |**Przeczytaj to**   |
|-----------------------|:-----------------------|
|Informacje na temat kart i nawigacji na stronie z możliwością wspólnej sprzedaży|[Nawigowanie w sekcji "co do lewej"](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Wybieranie organizacji klienta z listy D&B |[Wybierz klienta](./manage-co-sell-opportunities.md#select-your-customer)|
|Modyfikowanie pól w sekcji Szczegóły transakcji|[Szczegóły transakcji](./manage-co-sell-opportunities.md#deal-details)|
|Dodawanie członków zespołu do zespołu ds. transakcji|[Dodawanie pracowników](./manage-co-sell-opportunities.md#add-team-members)|
|Reagowanie na rozproszenie na sprzedaż|[Zarządzaj pozostałymi ofertami](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Rejestrowanie transakcji kupionych w centrum partnerskim |[Zarejestruj nową ofertę](./register-deals.md)
|Uzyskaj informacje o odwołaniach i Dowiedz się, w jaki sposób trwają odwołania |[Szczegółowe informacje o poleceniach](./referral-insights.md)
|Tworzenie profilu biznesowego i zarządzanie nim|[Zarządzanie profilem biznesowym](./create-a-marketing-profile.md)
|Zarządzanie potencjalnymi klientami dla profilu firmy |[Zarządzanie potencjalnymi klientami](./manage-leads.md)|

## <a name="next-steps"></a>Następne kroki


- [Partner Sales Connect z skoroszytem Centrum partnerskiego](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) — skoroszyt do wyrównania procesów sprzedaży i ról partnerów przy użyciu nowych procesów sprzedaży za pośrednictwem Centrum partnerskiego a łącznej sprzedaży partnera.
- [Przewodnik po współpracy z centrum partnerskim](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) — wskazówki pozwalające zidentyfikować model operacyjny za pośrednictwem Centrum partnerskiego, aby zarządzać potencjalnymi klientami lub okazjami do sprzedaży oraz rejestrować oferty.
- [Pokład zarządzania odwołaniami](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) — Wizualizacja krok po kroku do zarządzania potencjalnymi klientami i możliwościami współsprzedaży za pośrednictwem Centrum partnerskiego.
- [Publikowanie i zarządzanie ofertami w komercyjnym portalu Marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) — Wizualizacja krok po kroku umożliwiająca tworzenie i publikowanie ofert oraz zarządzanie nimi za pośrednictwem Centrum partnerskiego w komercyjnej witrynie Marketplace.