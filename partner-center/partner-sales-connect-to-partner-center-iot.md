---
title: Migracja z programu Partner Sales Połączenie (PSC) dla partnerów IOT
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Dowiedz się, jak partnerzy IOT firmy Microsoft mogą migrować z usługi Partner Sales Połączenie (PSC) do Partner Center i tworzyć transakcje i zarządzać nimi.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/07/2021
ms.openlocfilehash: 2b05046118c83c0d398272da68054a8a0c9c48e4
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128359469"
---
# <a name="guide-to-create-and-manage-iot-deals-in-partner-center-pc-for-iot-partners-migrating-from-partner-sales-connect-psc"></a>Przewodnik tworzenia transakcji IOT na platformie Partner Center (PC) dla partnerów IOT migrowania z usługi Partner Sales Połączenie (PSC)

**Odpowiednie role:** Administrator konta | Polecenia administratora | Partner Sales Połączenie (PSC) seller | Partner Sales Połączenie (PSC) admin | Partner Sales Połączenie (PSC) deal manager

Ten artykuł zawiera wskazówki dla partnerów IOT migrowania z programu Partner Sales Połączenie (PSC) do usługi Partner Center (PC), aby nadal tworzyć transakcje i zarządzać nimi w Partner Center.

>[!Note]
> Ten przewodnik ma zastosowanie tylko w przypadku partnerów biznesowych **IOT zarządzających** ich transakcjami w chmurze psc.

>[!Important]
> Od 15 sierpnia 2021 r. Twoja firma nie będzie mogła tworzyć ani edytować transakcji w chmurze psc. **Nadal będzie można pobierać istniejące dane transakcji przy użyciu funkcji eksportu zbiorczego w programie PSC. Możesz również [migrować otwarte transakcje](partner-sales-connect-to-partner-center-iot.md#psc-deals-migration) z konsoli psc do Partner Center późniejszą datą.**

Jak już wiesz, firma utraci dostęp do aplikacji **PSC po 30 sierpnia 2021 r.**. Jednak nadal znajdziesz wszystko, co chcesz zrobić w Partner Center, takie jak tworzenie transakcji i zarządzanie nimi.

Będą jednak różnice. Poniższe wskazówki mogą pomóc w sprawniejszym i prostszym Partner Center przejścia na inne urządzenia.

## <a name="before-you-move-things-you-need-to-know"></a>Przed przeniesieniem musisz wiedzieć, co musisz wiedzieć

### <a name="if-you-are-a-psc-admin"></a>Jeśli jesteś administratorem usługi PSC

- Do zalogowania się do usługi Partner Center jest [potrzebny służbowy Partner Center](https://partner.microsoft.com/).
- Skonfiguruj swoje konto za pomocą administratora Partner Center [konta.](permissions-overview.md)
- Przeczytaj ten dokument, aby dowiedzieć się, jak tworzyć transakcje IOT w Partner Center i zarządzać nimi.
- Skonfiguruj konta użytkowników w Partner Center dla wszystkich użytkowników centrum zabezpieczeń (role administratora, menedżera transakcji i sprzedawcy) i przypisz im role administratora poleceń lub [użytkowników poleceń.](permissions-overview.md)

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Jeśli jesteś menedżerem transakcji psc lub sprzedawcą

- Do zalogowania się do pulpitu nawigacyjnego usługi Partner Center potrzebna jest [służbowa wiadomość e-mail.](https://partner.microsoft.com/dashboard)
- Jeśli używasz konta nie służbowego w programie PSC lub służbowy adres e-mail jest dla innej firmy niż firma partnerska, skontaktuj się z administratorem centrum partnerskiego, aby uzyskać pomoc w skonfigurowaniu konta.
- Skontaktuj się z administratorem usługi PSC, Partner Center konfiguracja konta usługi jest ukończona niezależnie od konta, za pomocą których loguje sięsz do centrum psc.
- Sprawdź, czy masz dostęp do Partner Center i sekcji Polecenia.
- Przeczytaj ten dokument, aby zrozumieć przepływy pracy i zmiany Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Jako administrator w programie PSC, to są Twoje następne kroki

W Partner Center menu nawigacji po lewej stronie wybierz **opcję Polecenia.** Upewnij się, że możesz uzyskać dostęp do strony Możliwości współpracy sprzedaży.

  >[!Note]
  > Może być konieczne wylogowanie się z Partner Center i zalogowanie się ponownie, aby odświeżyć poświadczenia w celu uzyskania dostępu do stron Poleceń.

Jeśli nie widzisz opcji  Skierowania w menu usługi Partner Center lub na stronach związanych z [](permissions-overview.md) poleceniami, skontaktuj się z administratorem konta firmy i poproś o nadaj mu dostęp do opcji Polecenia i powiązanego obszaru. 

Aby znaleźć administratora konta firmy:

1. Wybierz **pozycję Ustawienia konta** z ikony koła zębatego w prawym górnym rogu pulpitu Partner Center nawigacyjnego.

1. Wybierz **pozycję Zarządzanie użytkownikami** z menu nawigacji drugiego poziomu po lewej stronie.

1. W górnej części listy użytkowników  wybierz menu rozwijane Filtr. Zmień opcję na **Administrator konta.**

   Na stronie zostaną wyświetleń wszyscy administratorzy kont wraz z odpowiednimi adresami e-mail. Wyślij wiadomość e-mail do jednej z nich i poproś o przypisanie roli administratora poleceń dla Twojego konta służbowego.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Obraz przedstawiający administratorów kont na stronie zarządzania użytkownikami w ustawieniach partnera.":::

>[!Important]
>- Jeśli Twoja rola obejmuje tylko zarządzanie użytkownikami w centrum zabezpieczeń firmy, poproś administratora konta firmy o przypisanie Ci roli administratora konta w programie Partner Center zgodnie z zasadami firmy. [](permissions-overview.md#manage-mpn-membership-and-your-company)
>- Jeśli Twoja rola obejmuje również zarządzanie transakcjami IoT, poproś o przypisanie odpowiedniej roli użytkownika [Administrator](permissions-overview.md#manage-referrals) poleceń lub Poleceń.
> - Dobrym pomysłem jest również wyznaczyć jednego lidera zarządzania zmianami wśród administratorów centrum zarządzania zmianą. Uniemożliwi to wszystkim administratorom centrum programu PsC indywidualną sspołędę z Partner Center administratorami kont. Zamiast tego liderem zarządzania zmianami może być podstawowa osoba pracująca z administratorem Partner Center konta.

## <a name="user-migration"></a>Migracja użytkowników

Po skonfigurowaniu konta w programie Partner Center użyj kreatora migracji użytkowników na stronie możliwości sprzedaży, aby automatycznie przypisać Partner Center do pracowników firmy.

>[!Note]
> Migracja użytkowników może być wykonywana tylko [przez administratorów](permissions-overview.md#manage-mpn-membership-and-your-company) kont w firmie. Jeśli nie masz roli administratora konta, znajdź administratora konta, który może pomóc w skonfigurowaniu kont użytkowników za pomocą kreatora migracji użytkowników.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Obraz przedstawiający kreatora migracji użytkowników.":::

Administratorzy kont zobaczą link kreatora migracji użytkowników psc na stronie możliwości współpracy sprzedaży obok przewodnika poleceń. Mogą zainicjować migrację użytkowników, wybierając link. Aby zainicjować migrację użytkowników, administratorzy mogą wybrać link. Ten krok migracji użytkownika można wykonać wiele razy, dopóki wszyscy użytkownicy nie zostaną przypisani do odpowiednich ról w Partner Center.

Tabela migracji użytkowników zawiera następujące szczegóły:

- Konto użytkownika — identyfikator e-mail pracownika
- Konto partnera PSC — konto, z którym jest skojarzony pracownik w programie PSC
- Rola użytkownika PSC — jedna z trzech ról przypisanych do w programie PSC.
- Lokalizacja MPN komputera — lokalizacja, dla której użytkownik będzie miał odpowiednie Partner Center (PC). Konto partnera PSC MPN służy do znalezienia równoważnej lokalizacji MPN w Partner Center do przypisywania uprawnień. Cała organizacja określa identyfikator MPN vOrg.
- Rola użytkownika komputera — role pracowników są przypisywane na podstawie ich ról użytkownika konsoli PSC. Administrator w programie PSC będzie mieć przypisane role administratora Poleceń w Partner Center. Sprzedawca będzie mieć przypisaną rolę użytkownika poleceń w Partner Center. Dowiedz się więcej o rolach Partner Center użytkownikach oraz o tym, co mogą robić użytkownicy z tymi rolami, zobacz Przypisywanie ról i uprawnień użytkowników w firmie, którzy muszą pracować w Partner Center [.](permissions-overview.md#manage-referrals)
- Dzierżawa usługi PC AAD — dzierżawa usługi Microsoft Azure Active Directory (Azure AD), do której są przypisani użytkownicy w Partner Center
- Stan — istnieją trzy możliwe stany stanu migracji
    - **Niemigrowane** — użytkownik nie ma przypisanej Partner Center od skierowań
    - **Zmigrowane** — użytkownik został pomyślnie zmigrowany z przypisaną odpowiednią rolą, jak pokazano w tabeli
    - **Błąd** — Nie można ukończyć migracji z powodu błędu

Czasami migracja może się nie powieść i spowodować błędy. Poniżej podano kilka przyczyn, dla których migracja może spowodować błąd, oraz kilka sposobów rozwiązania problemu:

1. Użytkownicy narzędzia PSC mogą używać konta nie służbowego.

2. Użytkownik usługi PSC może używać konta z domeny innej niż ta, która jest Partner Center.

   Aby usunąć błędy związane ze scenariuszami 1 i 2, poproś użytkownika o zalogowanie się do usługi Partner Center przy użyciu konta służbowego dołączonego do dzierżawy usługi Azure AD. Administrator [globalny może](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) ci pomóc.
   
   Aby znaleźć administratora globalnego: 
   1. Zaloguj się do pulpitu Partner Center [i](https://partner.microsoft.com/dashboard) wybierz **pozycję Ustawienia konta** z ikony koła zębatego w prawym górnym rogu.
   2. Wybierz **pozycję Zarządzanie użytkownikami** na lewym pasku nawigacyjnym drugiego poziomu.
   3. W górnej części listy użytkowników  wybierz menu rozwijane Filtr i zmień opcję na **Administrator globalny.** Następnie na stronie zostaną wyświetloni wszyscy administratorzy globalni wraz z odpowiednimi adresami e-mail. Poproś jedną z nich o przypisanie roli administratora poleceń dla twojego konta służbowego.
   
      Administrator globalny może utworzyć nowe konto użytkownika w dzierżawie usługi Azure AD lub przypisać dostęp użytkownika-gościa do innych użytkowników konta domeny. Po skonfigurowaniu kont dla wszystkich menedżerów transakcji psc i użytkowników muszą oni zalogować się do witryny Partner Center, wybrać pozycję Polecenia z menu nawigacji po lewej stronie i potwierdzić, że widzą stronę Polecenia. 

3. Użytkownik ma już przypisaną rolę odwołania w Partner Center.
    - Możesz sprawdzić istniejącą rolę użytkownika. W prawym górnym rogu okna Partner Center pozycję **Ustawienia** (ikona koła zębatego), a następnie **pozycję Ustawienia konta.** Po wyświetleniu drugiego menu nawigacji po lewej stronie wybierz pozycję **Zarządzanie użytkownikami** i wyszukaj użytkownika.

## <a name="psc-deals-migration"></a>Migracja transakcji PSC

Po zakończeniu migracji użytkowników użyj kreatora migracji transakcji na stronie możliwości współsprzedaży, aby wszystkie kwalifikujące się otwarte transakcje z programu PSC zostały Partner Center. **Link migracji transakcji będzie widoczny tylko dla administratorów poleceń z całym zakresem organizacji w Partner Center.** W prawym górnym rogu strony szans wspólnej sprzedaży będzie dostępny link o nazwie **„Migracja transakcji PSC”** umożliwiający otwarcie kreatora migracji transakcji.

Przeczytaj tę sekcję przed rozpoczęciem migracji transakcji.

**Kwalifikowanie się do migracji**

Tylko niektóre transakcje kwalifikują się do migracji z usługi PsC do Partner Center. Ten kreator migracji został zbudowany, aby pomóc partnerom w zamknięciu umowy Partner Center, gdzie nadal aktywnie współpracują ze swoimi klientami, aby zamknąć transakcję. **Do migracji kwalifikują się tylko transakcje w stanie otwartym utworzone od 1 stycznia 2020 r. z prawidłowymi szczegółami konta partnera (prawidłowy identyfikator MPN).**

## <a name="pre-requisites-for-deal-migration"></a>Wymagania wstępne dotyczące migracji transakcji

Przed rozpoczęciem migracji transakcji z Partner Center, postępuj zgodnie z poniższymi instrukcjami, aby skonfigurować transakcje w chmurze dla pomyślnej migracji.

- Wszyscy członkowie zespołu sprzedaży w Twojej firmie pracujący nad otwartymi transakcjami są poinformowani o tej migracji.
- Członkowie zespołu sprzedaży są przeszkoleni do używania Partner Center do zarządzania umowami.
- Transakcje zawierają wszystkie wymagane informacje zgodnie z poniższym opisem.
    - Szczegóły firmy klienta, w tym nazwa i adres
    - Co najmniej jedno rozwiązanie
    - Co najmniej jeden członek zespołu ze wszystkimi szczegółami — imię, nazwisko, identyfikator e-mail i numer telefonu
    - Wartość transakcji
    - Szacowana data zamknięcia transakcji
    - Uwagi partnerów

Możesz użyć funkcji zbiorczego pobierania i przekazywania w chmurze psc, aby dodać wszystkie brakujące szczegóły transakcji dla wszystkich kwalifikujących się transakcji.

>[!Note]
> Migracja transakcji powiedzie się, nawet jeśli powyższe wymagania wstępne nie zostaną spełnione. Nie można jednak zmienić stanu transakcji, jeśli dowolne z powyższych wymaganych pól w Partner Center są niedostępne. Następnie musisz wprowadzić wszystkie wymagane informacje, których brakuje w transakcjach w Partner Center, aby rozpocząć pracę nad nimi. **Zdecydowanie zaleca się oczyszczenie kwalifikujących się transakcji w programie PSC przed ich migracją do Partner Center.**

Migracja transakcji w Partner Center jest zbudowana jako środowisko jednym kliknięciem. Wystarczy kliknąć przycisk "Migruj **transakcje",** gdy firma będzie gotowa do migracji kwalifikujących się transakcji. **Nie można wybrać transakcji, które mają zostać zmigrowane z konsoli psc. Jeśli nie chcesz migrować żadnych transakcji do Partner Center, przenieś je do stanu zamkniętego w chmurze przed rozpoczęciem migracji.**

>[!Note]
> Po zainicjowaniu migracji migrowanie transakcji może potrwać do **24 godzin.**

Po zakończeniu migracji stan komunikatu baneru zmieni się na ukończony z linkiem do raportu migracji. Pobierz raport, aby wyświetlić szczegóły transakcji, które zostały zmigrowane z konsoli psc do Partner Center.

Raport zawiera poniższe szczegóły.

- **Partner Center zaangażowania —** unikatowy identyfikator w Partner Center dla wszystkich transakcji w zaangażowaniu. Istnieją dwie transakcje — jedna dla partnera i jedna dla firmy Microsoft w przypadku zaangażowania w sprzedaż Partner Center.
- **Partner Center polecenia —** unikatowy identyfikator w Partner Center dla transakcji należącej do partnera.
- **Nazwa transakcji** — identyfikator nadany transakcji w konsoli psc.
- **Identyfikator transakcji PSC** — unikatowy identyfikator transakcji w chmurze psc.
- **Błędy** — aby wskazać, czy wystąpił błąd podczas migrowania konkretnej transakcji.

Wszystkie transakcje, które zostały pomyślnie zmigrowane, nie będą widoczne w konsoli psc. Możesz kontynuować pracę nad zmigrowanych transakcji w Partner Center.

Transakcje migrowane z usługi PSC będą dostępne na karcie Dane wychodzące na stronie możliwości sprzedaży. Wszystkie transakcje będą tworzone jako transakcje prowadzone przez partnera. Są one widoczne dla sprzedawców firmy Microsoft.

>[!Important]
> Jeśli występują błędy, których nie można zmigrować niektórych transakcji, możesz ponownie zainicjować migrację transakcji, klikając przycisk **"Migruj transakcje".** Zostanie ona włączona tylko wtedy, gdy istnieją kwalifikujące się transakcje, które nie zostały jeszcze zmigrowane. Będzie to również przydatne, jeśli jesteś w fazie przejścia, w której niektóre nowe transakcje są tworzone w chmurze po zainicjowaniu migracji transakcji.

Po pomyślnym zmigrowania wszystkich transakcji pojawi się transparent z napisem "Brak transakcji do **migracji"** z wyłączonym przyciskiem "Migruj **transakcje".** 

## <a name="next-steps"></a>Następne kroki

Dowiedz się, jak tworzyć transakcje IOT i zarządzać nimi w Partner Center.
Jest to ważny krok, który pomoże Ci przygotować się do zarządzania umowami IOT w Partner Center. Poznaj przepływy pracy i zmiany w Partner Center, aby efektywnie tworzyć transakcje i zarządzać nimi. Zacznij od całkowitego przeczytania tego dokumentu.

## <a name="differences-between-psc-and-pc-workflows"></a>Różnice między przepływami pracy psc i PC

|**Scenariusz**|**Partner Sales Połączenie**|**Centrum partnerskie**|
|-----|:-----|:-----|
|Role użytkownika|PsC ma role administratora, menedżera transakcji i sprzedawcy.|Partner Center ma [role użytkownika administrator poleceń](permissions-overview.md#manage-referrals) i polecenia, które na podstawie zakresu lokalizacji dają uprawnienia zarówno do odczytu, jak i zapisu.|
|Szczegóły sprzedawcy firmy Microsoft|Widoczne zaraz po utworzeniu transakcji.|Szczegóły sprzedawcy firmy Microsoft nie są widoczne dla partnerów, ponieważ typ transakcji jest prowadzony przez partnera.
|Rozwiązania|Do transakcji można dodać dowolną liczbę rozwiązań.|Partner może dodać do transakcji maksymalnie 50 rozwiązań.
|Przypisanie transakcji|Tylko przypisany sprzedawca może wyświetlać transakcje i działać na ich podstawie.|Użytkownicy poleceń dodani do sekcji zespołu transakcji mogą wyświetlać i działać na transakcji. Administratorzy poleceń dla lokalizacji MPN, dla której transakcja została utworzona, mogą wyświetlać i działać na transakcji.|
|Organizacja klienta|Wpis tekstowy w postaci bezpłatnej.|Aby przeszukać bazę danych usługi D [&](manage-co-sell-opportunities.md#select-your-customer) B w organizacji [klienta,](https://www.dnb.com/) wystarczy wpisać kilka znaków. Nazwa i adres prawnych są wypełniane automatycznie na podstawie wyboru.|

## <a name="moving-from-psc-to-pc---faq"></a>Przenoszenie z usługi PSC na komputer — często zadawane pytania

Poniższe sekcje zawierają odpowiedzi na często zadawane pytania dotyczące migracji.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 — Co zrobić, jeśli nie mam dostępu do Partner Center?

Aby uzyskać przypisane role, możesz skontaktować się z administratorami wymienionymi na stronie "Brak dostępu". Będziesz potrzebować roli administratora [poleceń dla](permissions-overview.md#manage-referrals) uprawnień do odczytu i zapisu w sekcji polecenia. Jeśli zarządzasz tylko profilami biznesowymi, będziesz potrzebować roli administratora profilu biznesowego w Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Obraz przedstawiający środowisko bez dostępu w Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 — KtoTo udzielić mi dostępu do sekcji Polecenia w Partner Center?

Administrator [konta może](permissions-overview.md#manage-mpn-membership-and-your-company) udzielić Ci dostępu do karty Polecenia. Aby znaleźć administratora konta, wybierz pozycję **Ustawienia konta** za pomocą ikony koła zębatego w prawym górnym rogu pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard) Następnie wybierz pozycję **Zarządzanie użytkownikami** na lewym pasku nawigacyjnym drugiego poziomu. W górnej części listy użytkowników  wybierz menu rozwijane Filtr i zmień opcję na **administratora konta.** Na stronie zostaną wyświetleń wszyscy administratorzy kont wraz z odpowiednimi adresami e-mail. Poproś jedną z nich o przypisanie roli administratora poleceń dla twojego konta służbowego.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 — przycisk +Nowa transakcja jest wyszarytowany dla naszego konta. Co należy zrobić, aby rozpocząć tworzenie transakcji?

Dzieje się tak tylko wtedy, gdy identyfikator MPN skojarzony z Twoim kontem nie jest włączony do tworzenia transakcji IOT. Skontaktuj się z zespołem biznesowym IOT w wiadomości e-mail podanej podczas sesji szkoleniowych lub utwórz bilet pomocy technicznej, aby uzyskać identyfikator MPN włączony dla transakcji IOT".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 — Czy mogę przypisać transakcje do określonej osoby z organizacji, na przykład do psc?

Możesz przypisać członków zespołu do określonej transakcji. Nie blokuje to innym administratorom poleceń wyświetlania tych transakcji ani działania w ich sprawie.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 — Czy istnieje widok wszystkich przypisanych mi transakcji?

Możesz użyć funkcji Ulubione, która jest kartą na poziomie użytkownika. Możesz oznaczyć wszystkie transakcje przypisane do Ciebie jako ulubione, aby uzyskać szybki dostęp do transakcji.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 — Czy istnieje widok tylko do odczytu dla transakcji?

Nie, w sekcji skierowań nie ma widoku tylko do odczytu transakcji.

### <a name="7---is-adding-a-customer-organization-mandatory"></a>7 — Czy dodanie organizacji klienta jest obowiązkowe?

Tak, dodawanie organizacji [klienta jest obowiązkowe](./manage-co-sell-opportunities.md#select-your-customer) w Partner Center. Najpierw należy wyszukać lokalizację, w której znajduje się klient. Na podstawie posiadanych szczegółów: Możesz dodać konkretne szczegóły, w tym dokładną nazwę budynku, lub po prostu podać szczegóły miasta. Wyszukiwanie w organizacji spowoduje pobranie wszystkich jednostek prawnych zgodnych z waną nazwą, dzięki czemu nie trzeba wprowadzać żadnych szczegółów adresu. Wszystkie szczegóły są wypełniane automatycznie w zależności od wybranej organizacji.

### <a name="8---are-customer-contact-details-mandatory"></a>8 — Czy szczegóły kontaktowe klienta są obowiązkowe?

Tak, dane kontaktowe klienta są obowiązkowe w przypadku tworzenia transakcji IOT.

### <a name="9---how-many-solutions-can-i-add-to-a-deal"></a>9 — Ile rozwiązań mogę dodać do transakcji?

Do transakcji można dodać maksymalnie 50 rozwiązań (analogicznych do "produktów" w chmurze PSC). Zarówno ilość, jak i szacowana data zamknięcia rozwiązania są obowiązkowe, a szacowana data zamknięcia rozwiązań powinna być wcześniejsza niż szacowana data zamknięcia w sekcji szczegółów transakcji.

### <a name="10---where-can-i-find-the-opportunity-id"></a>10 — Gdzie mogę znaleźć identyfikator szansy sprzedaży?

Identyfikator szansy sprzedaży w programie PSC jest taki sam jak identyfikator polecenia w Partner Center. Identyfikator polecenia można znaleźć obok nazwy transakcji po otwarciu dowolnej transakcji.
