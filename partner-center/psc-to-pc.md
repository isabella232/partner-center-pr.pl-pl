---
title: Migrowanie z programu Partner Sales Connect (PSC)
description: Dowiedz się, w jaki sposób partnerzy firmy Microsoft mogą migrować z usługi Partner Sales Connect (PSC) do Centrum partnerskiego i tworzyć oferty wysyłane przez sprzedawców firmy Microsoft lub zarządzać nimi.
ms.topic: article
author: vikramb
ms.author: vikramb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/06/2020
ms.openlocfilehash: 1f352234f47ea8b2745c649401603f931ec68957
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381435"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Przewodnik po przedsprzedaży w centrum partnerskim (komputer) dla partnerów migrowania z programu Partner Sales Connect (PSC)

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Administrator konta
- Administrator odwołań
- Sprzedawca — Partner Sales Connect (PSC)
- Administrator połączenia z partnerem sprzedaży (PSC)
- Menedżer ds. sprzedaży partnera (PSC)

Jak wiadomo, firma utraci dostęp do 31 marca 2021. Znajdziesz wszystko, co chcesz zrobić, aby utworzyć oferty współsprzedażowe, zarządzać ofertami i podejmować działania dotyczące transakcji wysyłanych przez sprzedawcy firmy Microsoft do Ciebie w centrum partnerskim. Istnieją jednak różnice, a poniższe wskazówki pomogą Ci zapewnić bezproblemowe przejście do Centrum partnerskiego i przekazanie go do przodu.

>[!Important]
> Jeśli jesteś tutaj, ponieważ zobaczysz transparent na komputerze PSC o migracji, jesteś w odpowiednim miejscu. Ten przewodnik nie ma zastosowania do oceny rozwiązań (SA) i partnerów IOT OEM zarządzających swoimi ofertami na komputerze PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Zanim przejdziesz, co musisz wiedzieć

### <a name="if-you-are-psc-admin"></a>Jeśli jesteś administratorem PSC

- Aby zalogować się do [Centrum partnerskiego](https://partner.microsoft.com/), potrzebujesz służbowego adresu e-mail.
- Skonfiguruj swoje konto za pomocą pomocy [administratora konta](permissions-overview.md)Centrum partnerskiego.
- Dowiedz się, jak sprzedawać w centrum partnerskim, czytając ten dokument.
- Skonfiguruj konta użytkowników w centrum partnerskim dla wszystkich użytkowników PSC (administratorów, menedżerów transakcji i ról sprzedających) i przypisz im [role administratora odwołań](permissions-overview.md).

>[!Important]
> Upewnij się, że identyfikator MPN wyświetlany na banerze PSC jest dostępny na liście lokalizacji MPN w centrum partnerskim. Możesz sprawdzić, czy w centrum partnerskim, przechodząc do pozycji "Ustawienia konta" i "[lokalizacje](manage-locations.md)" w obszarze, aby znaleźć listę wszystkich usługi MPNS skojarzonych z kontem Centrum partnerskiego.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Obraz przedstawiający transparent PSC, w którym partnerzy mogą znaleźć identyfikator MPN.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Jeśli jesteś menedżerem PSC transakcji lub sprzedawcą

- Aby zalogować się do [Centrum partnerskiego](https://partner.microsoft.com/), potrzebujesz służbowego adresu e-mail.
- Jeśli używasz konta innego niż służbowego na komputerze PSC lub służbowy adres e-mail jest przeznaczony dla innej firmy niż firma partnerska, skontaktuj się z administratorem kontrolera konfiguracji, aby uzyskać pomoc dotyczącą konfigurowania konta.
- Skontaktuj się z administratorem systemu PSC, jeśli skonfigurowano konto Centrum partnerskiego niezależnie od konta, którego używasz do logowania się do komputera PSC.
- Sprawdź, czy masz dostęp do Centrum partnerskiego i sekcji odwołania.
- Przeczytaj ten dokument, aby poznać przepływy pracy i zmiany w centrum partnerskim.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Jako administrator w PSC, są to kolejne kroki

Jeśli nie widzisz karty odwołania:

- [Administrator globalny](permissions-overview.md) firmy może udzielić dostępu do karty odwołania. Aby znaleźć administratora globalnego, przejdź do obszaru Ustawienia partnera z ikony koła zębatego w prawym górnym rogu Centrum partnerskiego. Wybierz stronę Zarządzanie użytkownikami na drugim poziomie lewego paska nawigacyjnego. Kliknij menu rozwijane zawierające wartość "Wszyscy użytkownicy" w prawym górnym rogu strony i zmień wartość na "Administratorzy globalni". Na stronie zostaną wyświetlone wszystkie Administratorzy globalni z odpowiednimi identyfikatorami poczty e-mail. Skontaktuj się z pomocą techniczną, aby uzyskać dostęp do konta służbowego z uprawnieniami administratora.

  >[!Important]
  > Jeśli Twoja rola zarządza użytkownikami tylko w komputerze PSC, możesz uzyskać rolę [administratora konta](permissions-overview.md#manage-mpn-membership-and-your-company) w centrum partnerskim. Jeśli rola obejmuje również zarządzanie szansami do sprzedaży, należy uzyskać rolę [administratora odwołań](permissions-overview.md#manage-referrals) . Ponadto należy mianować jednego lidera zarządzania zmianami wśród administratorów systemu PSC do współpracy z administratorem konta Centrum partnerskiego, a nie wszystkich administratorów systemu PSC, którzy nie mają dostępu do administratorów konta na komputerze osobno.

  :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Obraz przedstawiający administratorów konta na stronie Zarządzanie użytkownikami ustawień partnera.":::

- Przejdź do karty odwołania w lewym okienku nawigacji i sprawdź, czy możesz uzyskać dostęp do stron.

  >[!Note]
  > Może być konieczne wylogowanie się z Centrum partnerskiego i ponowne zalogowanie się w celu odświeżenia poświadczeń w celu uzyskania dostępu do stron odwołań.

## <a name="user-migration"></a>Migracja użytkowników

Po skonfigurowaniu konta w centrum partnerskim Użyj Kreatora migracji użytkowników na stronie z możliwością współsprzedaży, aby przypisać role Centrum partnerskiego do pracowników firmy.

>[!Note]
> Migracja użytkowników może być przeprowadzana tylko przez [administratorów konta](permissions-overview.md#manage-mpn-membership-and-your-company) Twojej firmy. Jeśli nie masz roli administratora konta, Znajdź administratora konta, który może pomóc skonfigurować konta użytkowników za pomocą Kreatora migracji użytkowników. Funkcja migracji użytkowników będzie dostępna od 16 listopada 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Obraz przedstawiający Kreatora migracji użytkowników.":::

Administratorzy konta otrzymają link Kreator migracji użytkowników komputera PSC na stronie możliwości wspólnej sprzedaży obok podręcznika odwołania. Aby rozpocząć migrację użytkownika, kliknij link. Tę akcję można wykonać wiele razy, dopóki wszyscy użytkownicy, którzy chcą przeprowadzić migrację, mają przypisane odpowiednie role w centrum partnerskim.

Tabela migracji użytkowników zawiera następujące szczegóły

- Konto użytkownika — identyfikator E-mail pracownika
- Konto partnera PSC — konto, z którym jest skojarzony pracownik w systemie PSC
- Rola użytkownika PSC — jedna z trzech ról przypisanych do programu na komputerze PSC.
- Lokalizacja komputera MPN — lokalizacja, w której użytkownik będzie miał odpowiednie role komputerów. Konto partnera PSC MPN jest używane do znajdowania równoważnej lokalizacji MPN w centrum partnerskim do przypisywania uprawnień. Cała organizacja oznacza identyfikator vOrg MPN.
- Rola użytkownika komputera — pracownicy są przypisani do ról na podstawie ich ról użytkownika kontrolera systemu. Administrator na komputerze PSC zostanie przypisany do ról administratorów na komputerach. Sprzedawca zostanie przypisany do roli użytkownika z odwołaniami na komputerze. Dowiedz się więcej o rolach komputera i o tym, co użytkownicy z tymi rolami mogą wykonać w centrum partnerskim [tutaj](permissions-overview.md#manage-referrals)
- Dzierżawa komputera usługi AAD — dzierżawa, do której użytkownicy są przypisani w centrum partnerskim
- Stan — istnieją trzy możliwe stany migracji stanu
    - Nie przeprowadzono migracji — użytkownik nie ma przypisanej roli żadnych odwołań komputera
    - Migracja — użytkownik został pomyślnie zmigrowany z odpowiednimi przypisanymi rolami, jak pokazano w tabeli
    - Błąd — nie można ukończyć migracji z powodu błędu

Migracja może zakończyć się niepowodzeniem i spowodować błędy w niektórych warunkach, dla których rozwiązania są podane poniżej

1. Użytkownicy PSC mogą korzystać z konta innego niż konto służbowe.

2. Użytkownicy PSC mogą korzystać z konta z domeny innej niż ta, która jest używana w centrum partnerskim.

   - Aby rozwiązać problemy związane z scenariuszami 1 i 2, wszyscy użytkownicy muszą zalogować się do Centrum partnerskiego przy użyciu konta służbowego dołączonego do dzierżawy usługi Azure AD. [Administrator globalny](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) może Ci pomóc. Aby znaleźć administratora globalnego, przejdź do obszaru Ustawienia partnera z ikony koła zębatego w prawym górnym rogu Centrum partnerskiego. Kliknij stronę Zarządzanie użytkownikami na drugim poziomie lewego paska nawigacyjnego. Kliknij menu rozwijane zawierające wartość "Wszyscy użytkownicy" w prawym górnym rogu strony i zmień wartość na "Administratorzy globalni". Administrator globalny może utworzyć nowe konto użytkownika w dzierżawie usługi Azure AD lub przypisać dostęp użytkownika-gościa do innych użytkowników konta domeny. Po skonfigurowaniu kont dla wszystkich menedżerów i użytkowników w organizacji PSC należy zalogować się do Centrum partnerskiego, przejść do karty odwołanie w lewym obszarze nawigacji i upewnić się, że mogą oni zobaczyć stronę odwołania.

3. Użytkownik ma już przypisaną rolę odwołania w centrum partnerskim.
    - Istniejącą rolę użytkownika można sprawdzić na stronie Zarządzanie użytkownikami w ustawieniach konta i zmodyfikować tak samo, jak to konieczne.

Po zakończeniu migracji użytkowników Skorzystaj z poniższych wskazówek, aby określić strategię migracji: 

Jeśli Twoja firma ma PDM — po skonfigurowaniu konta Centrum partnerskiego i przeniesieniu przez użytkowników ról i uprawnień, możesz przenieść swoje działania towarzyszące do Centrum partnerskiego. Przed upływem ostatecznego terminu migracji poinformuj PDM o tym, aby przełączać się do programu, co pozwoli na przepływ wszystkich nowych transakcji do Centrum partnerskiego.

>[!Note]
>Po dokonaniu tego przełącznika będzie można działać tylko na istniejących aktywnych okazjach na komputerze PSC. Nie można tworzyć nowych transakcji ani otrzymywać żadnych transakcji od sprzedawcy firmy Microsoft na komputerze PSC.

Jeśli firma nie ma PDM — upewnij się, że wszystkie konta użytkowników zostały skonfigurowane i zweryfikowane przez wszystkich użytkowników. Otrzymasz powiadomienie za pośrednictwem wiadomości e-mail i transparentu na komputerze PSC w sprawie dokładnej daty rozpoczęcia sprzedaży w centrum partnerskim. Pamiętaj, że nadal będziesz mieć możliwość zarządzania istniejącymi aktywnymi transakcjami na komputerze PSC.

>[!Important]
>Aktywne transakcje nie będą migrowane do komputera. Do 31 grudnia 2020 do zamknięcia i rejestrowania transakcji.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Następne kroki dla administratorów PSC, menedżerów transakcji PSC i sprzedawcy PSC

Dowiedz się, jak sprzedawać w centrum partnerskim.
Jest to ważny krok, który pomoże Ci przygotować się do sprzedaży w centrum partnerskim. Poznaj przepływy pracy i zmiany w centrum partnerskim, dzięki czemu możesz efektywnie sprzedawać od samego dnia. Zacznij od pełnego przeczytania tego dokumentu. Dobry zestaw zasobów jest również dostępny w [galerii z możliwością współsprzedażowej](https://aka.ms/cosellexperience).

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

## <a name="psc-and-partner-center-field-mapping"></a>Kontroler PSC i mapowanie pola Centrum partnerskiego

W tej części przedstawiono dokładne Mapowanie atrybutów między kontrolerem PSC a centrum partnerskim. Każdy ekran w systemie PSC jest porównywany z odpowiednim widokiem w sekcji możliwości wspólnej sprzedaży w centrum partnerskim. 

>[!Note]
>Aby znaleźć odpowiedni atrybut w centrum partnerskim, postępuj zgodnie z liczbami widocznymi na żółtych bąbelkach na zrzutach ekranu PSC. Czerwone bąbelki wskazują, że zarejestrowana nie jest dostępna w centrum partnerskim.

**Strona główna PSC i domyślny widok możliwości wspólnej sprzedaży w centrum partnerskim**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Obraz przedstawiający Mapowanie pól między stroną główną programu partnerskiego połączenia z partnerem sprzedaży a domyślnym widokiem możliwości wspólnej sprzedaży w centrum partnerskim.":::

**Widok siatki PSC i widok transakcji Centrum partnerskiego**

- W centrum partnerskim nie ma widoku listy, takiego jak kontroler PSC.  Wszystkie transakcje są wyświetlane na podstawie najnowszej otrzymanej lub utworzonej daty z informacjami o kliencie i typem transakcji. Pierwsza transakcja w widoku jest domyślnie zaznaczona. Większość wartości, które są wyświetlane w formacie tabeli PSC, są dostępne w widoku szczegółowym transakcji na komputerze.
- Rola transakcji nie jest polem wymaganym na komputerze. Nie jest on wyświetlany ani przechwytywany w żadnym przepływie pracy. Jest ona tworzona automatycznie na stronie sprzedawcy firmy Microsoft w oparciu o rozwiązania dodane do transakcji.
- Data ostatniej modyfikacji nie jest wyświetlana na stronie szczegółów odwołania na komputerze. Partnerzy mogą używać funkcji sortowania do sortowania transakcji na podstawie daty ostatniej aktualizacji.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem siatki Połącz z partnerem sprzedaży partnera (PSC) i widokiem transakcji Centrum partnerskiego.":::

**Widok szczegółów transakcji w centrum komputerów PSC i partnerskim**

- Partnerzy mogą edytować ofertę, klikając przycisk Edytuj w widoku szczegółów transakcji partnera (6). Po kliknięciu przycisku Edytuj wszystkie pola zostaną edytowane z opcją Zapisz lub Anuluj zmiany wprowadzone w ramach transakcji.
- Nie ma możliwości zamknięcia transakcji jako duplikatu w centrum partnerskim.
- Wynik klienta nie jest dostępny w centrum partnerskim. Wszystkie szczegóły dotyczące interakcji z klientami można zaktualizować w sekcji notatki na komputerze.
- Szacowana data zamknięcia rozwiązania jest dostępna tylko w przypadku firmowych producentów OEM w centrum partnerskim. Nie jest ona wyświetlana dla żadnych innych typów transakcji.
- Program licencjonowania nie jest wymagany na komputerze. Jest on wywnioskowany na podstawie rozwiązań wybranych w ramach transakcji.

>[!Note]
>Wszystkie transakcje oznaczone jako wygrane lub utracone nie mogą być edytowane. Należy zachować ostrożność podczas przechodzenia do jednego z tych stanów terminalu.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem szczegółów rozdziału partnera sprzedaży (PSC) i widokiem szczegółów transakcji Centrum partnerskiego.":::

**Widok "Dodaj produkty" kontrolera PSC i widok "Dodaj rozwiązania" Centrum partnerskiego**

:::image type="content" source="images/pscmigration/products.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem Dodawanie produktów partnera (PSC) do programu oraz widok dodawania rozwiązań Centrum partnerskiego.":::

**Zarządzanie użytkownikami na komputerze PSC i w centrum partnerskim**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Obraz przedstawiający Mapowanie pól między domem i zarządzanie użytkownikami Centrum partnerskiego w widoku Ustawienia konta.":::

**Przypisanie roli użytkownika w komputerze PSC i w centrum partnerskim**

- Równoważną rolę administratora PSC jest rola administratora konta w centrum partnerskim.
- Istnieje tylko jedna rola w centrum partnerskim do zarządzania sprzedażą w celu współdziałania, która jest rolą administratora odwołań.

:::image type="content" source="images/pscmigration/roles.png" alt-text="Obraz przedstawiający Mapowanie pól między widokiem przypisywania roli Partner Sales Connect (PSC) i widok przypisania roli Centrum partnerskiego.":::

**Powiadomienia na komputerze PSC i w centrum partnerskim**

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Obraz przedstawiający mapowanie między powiadomieniami partnera (Partner Sales Connect) i widokiem powiadomień Centrum partnerskiego.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Przejście z komputera PSC do Centrum partnerskiego — często zadawane pytania

**Pierwszym. Co należy zrobić, jeśli nie mam dostępu do Centrum partnerskiego?**

Aby uzyskać przypisane role, możesz skontaktować się z administratorami na liście na stronie "Brak dostępu". W sekcji odwołania będzie potrzebna rola "[administrator odwołań](permissions-overview.md#manage-referrals)" dla uprawnień Odczyt i zapis. Jeśli zarządzasz tylko profilami biznesowymi, w centrum partnerskim będzie potrzebna rola "Administrator profilu biznesowego".

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Obraz przedstawiający sposób braku dostępu w centrum partnerskim.":::

**Q2. Kto może udzielić mi dostępu do sekcji odwołań w centrum partnerskim?**

[Administrator konta](permissions-overview.md#manage-mpn-membership-and-your-company) może udzielić dostępu do karty odwołania. Aby znaleźć administratora konta, przejdź do obszaru Ustawienia partnera z ikony koła zębatego w prawym górnym rogu Centrum partnerskiego. Kliknij stronę Zarządzanie użytkownikami na drugim poziomie lewego paska nawigacyjnego. Kliknij listę rozwijaną, która zawiera wartość "Wszyscy użytkownicy" w prawym górnym rogu strony i przejdź do "Administratorzy konta". Na stronie zostaną wyświetlone wszystkie Administratorzy konta z odpowiednimi identyfikatorami poczty e-mail. Skontaktuj się z pomocą techniczną, aby uzyskać dostęp do konta służbowego z uprawnieniami administratora.

**Kwartał. Przycisk + Nowa transakcja jest wyszarzony dla naszego konta. Co należy zrobić, aby zacząć tworzyć oferty?**

Dzieje się tak tylko wtedy, gdy nie ma żadnych gotowych do zakupu rozwiązań do organizacji MPN, które są używane w centrum partnerskim. Skontaktuj się z PDM, aby uzyskać poprawiony identyfikator MPN rozwiązań, lub Utwórz bilet pomocy technicznej z informacją o problemie "nowy przycisk rozproszenia jest wyszarzony po migracji kontrolera systemu".

**Kwartale. Czy mogę przypisywać oferty do określonej osoby z naszej organizacji, takiej jak PSC?**

Można przypisać członków zespołu do konkretnej transakcji. Nie blokuje ona wyświetlania ani działania innych administratorów odwołań do tych transakcji. 

**Q5. Czy istnieje widok wszystkich przypisanych do mnie okazji?**

Możesz użyć funkcji Ulubione, która jest kartą poziomu użytkownika. Możesz oznaczyć wszystkie oferty, które są przypisane do Ciebie jako Ulubione, aby uzyskać szybki dostęp do tych transakcji.

**Q6. Czy istnieje widok tylko do odczytu dla transakcji?**

Nie. w sekcji odwołania nie ma widoku tylko do odczytu transakcji. Wszyscy administratorzy odwołań będą mieć pełny dostęp do odczytu i zapisu do wszystkich transakcji.

**Q7. Jak mogę zarejestrować ofertę po jej wykorzystaniu?**

Jeśli transakcja spełnia poniższe kryteria, zostanie wyświetlone okno podręczne, aby rozpocząć [rejestrację transakcji](./register-deals.md).

- Istnieje rozwiązanie uprawniające do oferty.
- Sprzedawca firmy Microsoft jest zapraszany do wzięcia udziału w transakcji lub zaprosił Cię do zawarcia umowy.
- Karta Microsoft jest w stanie zaakceptowana lub wygrana w centrum partnerskim.

**Q8. Otrzymuję komunikat o błędzie po kliknięciu przycisku "+ Nowa rejestracja transakcji" w sekcji Rejestracja transakcji. Jak mogę zarejestrować moje transakcje?**

"+ Nowa rejestracja transakcji" ma być używana tylko przez partnerów zarejestrowanych w programie do łączenia niezależnych dostawców oprogramowania w celu zarejestrowania transakcji bez odpowiadającej jej szansy sprzedaży w centrum partnerskim. W celu zarejestrowania transakcji z możliwością współsprzedaży zostanie wyświetlone okno podręczne, gdy transakcja zostanie oznaczona jako wykorzystana i będzie spełniać kryteria rejestracji transakcji.

**Q9. Czy dodanie organizacji klienta jest obowiązkowe?**

Tak, dodanie [organizacji klienta](./manage-co-sell-opportunities.md#select-your-customer) jest obowiązkowe w centrum partnerskim. Najpierw Zacznij od wyszukania lokalizacji, w której znajduje się klient. Na podstawie szczegółowych informacji; można określić, w tym dokładną nazwę budynku, lub po prostu podać szczegóły miasta. W ramach wyszukiwania organizacji zostaną pobrane wszystkie jednostki prawne pasujące do wprowadzonej nazwy, aby nie trzeba było wprowadzać żadnych szczegółowych informacji o adresie. Wszystkie szczegóły są wypełniane automatycznie w oparciu o wybraną organizację.

**Q10. Czy dane kontaktowe klienta są obowiązkowe?**

Zależy od typu tworzonej [transakcji](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) . Jeśli po prostu udostępniasz swój potok i nie potrzebujesz pomocy od organizacji sprzedaży firmy Microsoft, możesz zrezygnować z podawania szczegółów kontaktowych klienta. Jeśli sprzedajesz, gdzie aktywnie szukasz pomocy od sprzedawcy firmy Microsoft, konieczne będzie podanie szczegółowych informacji kontaktowych klienta. Przed utworzeniem żądania współsprzedaży w centrum partnerskim należy uzyskać jawną zgodę od klienta.

**Q11. Ile rozwiązań można dodać do transakcji?**

Do rozpatrzenia można dodać do 50 rozwiązań (analogicznie do "produktów" w PSC). W przeciwieństwie do systemu PSC, możesz mieszać rozwiązania z własnych, oferowanych przez siebie rozwiązań, jednostek SKU pierwszej firmy Microsoft oraz innych firmowych rozwiązań do sprzedawania. Nie ma roli transakcji, która ma być wybrana lub dostępna w centrum partnerskim. W przypadku jednostek SKU firmy Microsoft można opcjonalnie dodać ilość i cenę dla każdej jednostki SKU, która jest dodawana do transakcji.

**Q12. Kiedy otrzymasz informacje o sprzedawcy firmy Microsoft po utworzeniu transakcji?**

Sprzedawcy firmy Microsoft są przypisani dopiero po dopasowaniu dokładnego wymagania dotyczącego pomocy, które zostały podane podczas tworzenia transakcji z odpowiednią osobą sprzedającą po stronie firmy Microsoft. Nawet po przypisaniu sprzedawcy firmy Microsoft będą mogli zaakceptować lub odrzucić zaproszenie do współsprzedażu. W przypadku zaakceptowania przez sprzedawcę zaproszenia do sprzedaży zostanie ona zaktualizowana informacjami o kontaktach sprzedawcy firmy Microsoft. Umowa SLA dla sprzedawcy firmy Microsoft do działania w ramach umowy wynosi 14 dni. Jest to ta sama umowa SLA, którą partnerzy muszą podejmować działania w odniesieniu do stanu sprzed wygaśnięcia.

**Q13. Gdzie mogę znaleźć identyfikator szansy sprzedaży?**

Identyfikator szansy sprzedaży w PSC jest taki sam jak identyfikator transakcji na komputerze. Identyfikator transakcji można znaleźć obok nazwy transakcji po otwarciu każdej transakcji.

**Q14. Jak mój PDM może uzyskać dostęp do komputera?**

Nie można uzyskać dostępu do Centrum partnerskiego za pomocą PDM bezpośrednio w przeciwieństwie do komputera PSC. Istnieje wiele opcji umożliwiających tę możliwość, które są wymienione poniżej.

- OCP Insights — Jeśli PDM się, że właśnie przeglądasz & transakcje związane z postępem, mogą oni korzystać z portalu OCP Insights w celu uzyskania widoku organizacji. Jest to narzędzie wewnętrzne i dostępne tylko dla PDM. Pamiętaj, że w firmie OCP Insights nie są dostępne dla użytkowników Twojej firmy.
- Użytkownik-Gość w centrum partnerskim — możesz dodać @microsoft.com konto PDM jako użytkownika-gościa w centrum partnerskim i przypisać do nich rolę administratora odwołań, aby mogli oni wyświetlać i podejmować działania dotyczące odwołań.
- Tworzenie [nowego użytkownika](./create-user-accounts-and-set-permissions.md#add-a-new-user) w dzierżawie — możesz utworzyć nowego użytkownika w swojej dzierżawie i udostępnić te szczegóły w PDM, aby mogły wyświetlać i działać na odwołaniach podobnych do innych użytkowników referencyjnych na Twoim koncie.

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

Wykonaj następujące dodatkowe zasoby:

- [Partner Sales Connect z skoroszytem Centrum partnerskiego](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) — skoroszyt do wyrównania procesów sprzedaży i ról partnerów przy użyciu nowych procesów sprzedaży za pośrednictwem Centrum partnerskiego a łącznej sprzedaży partnera.
- [Przewodnik po współpracy z centrum partnerskim](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) — wskazówki pozwalające zidentyfikować model operacyjny za pośrednictwem Centrum partnerskiego, aby zarządzać potencjalnymi klientami lub okazjami do sprzedaży oraz rejestrować oferty.
- [Pokład zarządzania odwołaniami](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) — Wizualizacja krok po kroku do zarządzania potencjalnymi klientami i możliwościami współsprzedaży za pośrednictwem Centrum partnerskiego.
- [Publikowanie i zarządzanie ofertami w komercyjnym portalu Marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) — Wizualizacja krok po kroku umożliwiająca tworzenie i publikowanie ofert oraz zarządzanie nimi za pośrednictwem Centrum partnerskiego w komercyjnej witrynie Marketplace.
