---
title: Łącznik współsprzedającego dla Centrum partnerskiego programu Dynamics 365 CRM
description: Zsynchronizuj odwołania w centrum partnerskim z łącznikiem współsprzedawanym dla programu Dynamics 365 CRM. Następnie można sprzedać firmie Microsoft z poziomu systemu CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768775"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Łącznik współpracujący z systemem Dynamics 365 CRM — Omówienie

### <a name="appropriate-roles"></a>Odpowiednie role

- Administrator odwołań
- Administrator systemu lub Konfigurator systemu w programie CRM

Łączniki współsprzedawanych w centrum partnerskim pozwalają sprzedającym na współsprzedaż z firmą Microsoft w ramach systemów CRM. Nie trzeba ich przeszkoleć w celu zarządzania pozostałymi ofertami przy użyciu Centrum partnerskiego. Korzystając z łączników współsprzedaj, możesz utworzyć nowe odwołanie do współsprzedaży, aby skontaktować się z sprzedającym firmy Microsoft, otrzymać odwołania od sprzedawcy firmy Microsoft, zaakceptować lub odrzucić odwołania oraz zmodyfikować dane dotyczące transakcji, takie jak wartość transakcji i Data zamknięcia. Możesz również otrzymywać wszelkie aktualizacje od sprzedawcy firmy Microsoft w ramach tych transakcji związanych z współsprzedażą. Możesz zarządzać wszystkimi odwołaniami w wybranym przez Ciebie programie CRM, a nie w centrum partnerskim.

Rozwiązanie jest oparte na automatyzacji i korzysta z interfejsów API Centrum partnerskiego.

## <a name="prerequisites"></a>Wymagania wstępne

Przed zainstalowaniem rozwiązania upewnij się, że spełnione zostały następujące wymagania wstępne.

|**Tematy**   |**Szczegóły**   |**Linki**   |
|--------------|--------------------|------|
|Identyfikator Microsoft Partner Network (MPN) |Wymagany jest prawidłowy identyfikator MPN.|[Dołącz do sieci partnerskiej](https://partner.microsoft.com/)|
|Gotowe do rozłożenia|Twoje rozwiązanie do adresów IP/usług musi być gotowe do współpracy.|[Sprzedawanie z firmą Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Konto Centrum partnerskiego|IDENTYFIKATOR MPN skojarzony z dzierżawcą Centrum partnerskiego musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współsprzedażu. Przed wdrożeniem łączników upewnij się, że w portalu Centrum partnerskiego są widoczne swoje odwołania do współsprzedawcy.|[Zarządzanie kontem](create-user-accounts-and-set-permissions.md)|
|Role użytkowników Centrum partnerskiego|Pracownik, który zainstaluje łączniki i korzysta z nich, musi być administratorem odwołań.|[Przypisywanie ról i uprawnień użytkowników](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Rola użytkownika programu CRM jest administratorem systemu lub konfiguratorem systemu.|[Przypisywanie ról w usłudze Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Konto przepływu automatyzacji|Utwórz nowe środowisko produkcyjne z bazą danych do testowania, przemieszczania i produkcji. Jeśli masz istniejące środowisko produkcyjne z bazą danych, można je ponownie wykorzystać. Użytkownik, który zamierza zainstalować rozwiązanie łącznika, musi mieć licencję na automatyzację i dostęp do tego środowiska. Możesz monitorować postęp i uzyskać więcej [informacji w programie](https://flow.microsoft.com/) , jeśli instalacja nie powiedzie się. Wybierz pozycję **Zobacz historię** w obszarze **rozwiązania**.|[Utwórz środowisko lub Zarządzaj nim](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Zainstaluj synchronizację odwołań Centrum partnerskiego dla programu Dynamics 365 (rozwiązanie do automatyzowania zarządzania)

1. Przejdź do pozycji [Automatyzacja](https://flow.microsoft.com)i wybierz pozycję **środowiska** w prawym górnym rogu. W tym kroku przedstawiono dostępne wystąpienia programu CRM.

1. Wybierz odpowiednie wystąpienie programu CRM z listy rozwijanej w prawym górnym rogu.

1. Wybierz pozycję **rozwiązania** po lewej stronie.

1. Wybierz link **Otwórz AppSource** w górnym menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Zrzut ekranu pokazujący otwartą AppSource.":::

1. Wyszukaj **Łączniki dotyczące odwołań Centrum partnerskiego dla programu Dynamics 365** na ekranie podręcznym.  

1. Wybierz przycisk **Pobierz teraz** , a następnie wybierz pozycję **Kontynuuj**.

1. Zostanie wyświetlona strona, na której można wybrać środowisko CRM (Dynamics 365), aby zainstalować aplikację. Zaakceptuj warunki i postanowienia.

1. Możesz monitorować postęp i, jeśli instalacja nie powiedzie się, możesz uzyskać więcej szczegółów w programie w celu automatyzacji, wybierając pozycję **Zobacz historię** w obszarze **rozwiązania**.

1. Po zakończeniu instalacji Wróć do pozycji [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **rozwiązania** po lewej stronie. W przypadku usługi Dynamics 365 jest teraz dostępna lista **rozwiązań** **Centrum partnerskiego** .

1. Wybierz pozycję **Centrum partnerskie — synchronizacja dla programu Dynamics 365**. Dostępne są następujące przepływy i jednostki automatyzacji.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Zrzut ekranu pokazujący dostępne CRMs.":::

## <a name="test-before-you-go-live"></a>Przetestuj przed rozpoczęciem

Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania do automatyzowania w środowisku produkcyjnym należy przetestować rozwiązanie w tymczasowym wystąpieniu programu CRM. Należy:

- Zainstaluj rozwiązanie do automatyzowania gotowości w wystąpieniu programu CRM środowiska przejściowego.
- Skonfiguruj i Dostosuj rozwiązanie do automatyzowania gotowości w środowisku przejściowym.
- Przetestuj rozwiązanie w tymczasowym wystąpieniu programu CRM.
- Po pomyślnym teście zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.

## <a name="configure-the-solution"></a>Skonfiguruj rozwiązanie

1. Po zainstalowaniu rozwiązania w wystąpieniu programu CRM Wróć do narzędzia do [automatyzacji](https://flow.microsoft.com/).

1. Z listy rozwijanej **środowiska** w prawym górnym rogu wybierz wystąpienie programu CRM, na którym zainstalowano rozwiązanie do automatyzowania.

1. Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:

   - Użytkownik Centrum partnerskiego z poświadczeniami administratora
   - Zdarzenia Centrum partnerskiego
   - Administrator programu CRM z przepływem automatyzacji w rozwiązaniu

   1. Wybierz pozycję **połączenia** po lewej stronie, a następnie wybierz z listy rozwiązanie z **odwołaniami do Centrum partnerskiego** .

   1. Utwórz połączenie, wybierając pozycję **Utwórz połączenie**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Zrzut ekranu przedstawiający tworzenie połączenia.":::

   1. Wyszukaj **Referencje Centrum partnerskiego (wersja zapoznawcza)** na pasku wyszukiwania w prawym górnym rogu.

   1. Utwórz połączenie dla użytkownika Centrum partnerskiego z rolą poświadczeń administratora.

   1. Następnie utwórz połączenie zdarzeń Centrum partnerskiego dla użytkownika Centrum partnerskiego z poświadczeniami administratora.

   1. Utwórz połączenie dla Common Data Service (bieżące środowisko) dla użytkownika Administrator programu CRM.
     
   1. Po dodaniu wszystkich połączeń powinny zostać wyświetlone następujące połączenia w danym środowisku.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Zrzut ekranu przedstawiający połączenia.":::

## <a name="edit-the-connections"></a>Edytuj połączenia

1. Wróć do strony **rozwiązania** i wybierz pozycję **domyślne rozwiązanie**. Wybierz pozycję **odwołanie do połączenia (wersja zapoznawcza)** , wybierając pozycję **wszystkie**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Zrzut ekranu pokazujący edytowanie połączeń.":::

1. Edytuj poszczególne połączenia po jednym z nich, wybierając ikonę wielokropka. Dodaj odpowiednie połączenia.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Zrzut ekranu pokazujący wyświetlane połączenia.":::

1.  Wróć do strony **rozwiązania** , wybierz pozycję **Centrum partnerskie odniesień do usługi Dynamics 365** i Włącz przepływ, wybierając ikonę wielokropka obok każdego przepływu w następującej kolejności. Jeśli podczas włączania przepływu wystąpią jakiekolwiek problemy, zobacz [kroki dostosowywania](connector-dynamics.md#customize-synchronization-steps) i [Rozwiązywanie problemów](connectors-troubleshoot.md).

Włącz przepływy w następującej kolejności:

- Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Utwórz odwołanie do współsprzedawcy — Dynamics 365 do Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Dostosowa Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow
- Centrum partnerskie do oprogramowania Dynamics 365 — pomocnik (wersja zapoznawcza programu testowego)
- Centrum partnerskie — aktualizacje odwołań do oprogramowania Dynamics 365 (wersja zapoznawcza programu Preview)
- Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu Preview)
- Dynamics 365 do Centrum partnerskiego (wersja zapoznawcza)
- Dynamics 365 — szansa do Centrum partnerskiego (wersja zapoznawcza)
- Dynamics 365 — rozwiązania firmy Microsoft do Centrum partnerskiego (wersja zapoznawcza)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementu webhook

Możesz użyć interfejsów API elementu webhook Centrum partnerskiego, aby zarejestrować zdarzenia zmiany zasobów. Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.

1. Wybierz pozycję **Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu testowego)**.

1. Wybierz ikonę **Edytuj** , a następnie wybierz opcję **po odebraniu żądania HTTP**.

1. Wybierz ikonę **kopiowania** , aby skopiować podany adres URL post protokołu HTTP.

   :::image type="content" source="images/webhook-video.gif" alt-text="Zrzut ekranu, który pokazuje, jak rejestrować zmiany zasobów przy użyciu elementów webhook.":::

1. Wybierz pozycję **rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza)** , a następnie wybierz pozycję **Uruchom**.

1. Upewnij się, że okno **uruchamiania przepływu** zostanie otwarte w prawym okienku, a następnie wybierz pozycję **Kontynuuj**.

1. Wprowadź następujące informacje:

   - **Punkt końcowy wyzwalacza http**: ten adres URL został skopiowany z wcześniejszego kroku.
   - **Zdarzenia do zarejestrowania**: Wybierz wszystkie dostępne zdarzenia (z **odwołaniami**, które zostały **zaktualizowane**, **powiązane z odwołaniami** i **powiązane** z odwołaniami).
   - **Zastąp istniejące punkty końcowe wyzwalacza, jeśli istnieją?**: tak. Dla danego zdarzenia elementu webhook można zarejestrować tylko jeden adres URL.

1. Wybierz pozycję **Uruchom przepływ**, a następnie wybierz pozycję **gotowe.**

Element webhook może teraz nasłuchiwać, tworzyć i aktualizować zdarzenia.

## <a name="customize-synchronization-steps"></a>Dostosowywanie kroków synchronizacji

Systemy CRM są wysoce dostosowane i można dostosować rozwiązanie do automatyzowania zarządzania, korzystając z konfiguracji programu CRM. Po zsynchronizowaniu odwołań towarzyszących między centrum partnerskim i systemem CRM pola, które są synchronizowane na komputerze Centrum partnerskiego, są wyświetlane w [przewodniku mapowania pól niestandardowych](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w temacie **[Dostosowywanie] Utwórz lub Pobierz szczegóły z przepływu Dynamics 365** lub zmiennych środowiskowych. Nie Aktualizuj żadnych innych przepływów w rozwiązaniu automatyzacji, ponieważ może to mieć wpływ na przyszłe uaktualnienia rozwiązań.

Dostępne są następujące dostosowania:

- **Wyświetl znacznik wyboru w polu Nazwa szansy sprzedaży**: domyślnie obok nazwy szansy sprzedaży zostanie wyświetlony znacznik wyboru wskazujący, że synchronizacja między centrum partnerskim a programem Dynamics 365 CRM zakończyła się pomyślnie. Analogicznie, jeśli synchronizacja nie powiedzie się, zostanie wyświetlony krzyżyk. Aby uniknąć dodawania znacznika Check lub krzyżyka w nazwie szansy sprzedaży, ustaw bieżącą wartość **znacznika wyboru wyświetlania w zmiennej środowiskowej nazwa szansy sprzedaży na wartość** nie.
- **Wartość transakcji**: Domyślnie wartość transakcji z Centrum partnerskiego będzie synchronizowana z i z **ESTIMATEDVALUE** w programie CRM. Jeśli w programie CRM istnieje inne pole do synchronizowania wartości transakcji z:

  - Zaktualizuj nazwę pola **wartości transakcji** w zmiennej środowiskowej Dynamics 365 przy użyciu nazwy pola CRM. Upewnij się, że podajesz nazwę pola, a nie jego nazwę wyświetlaną.
  - Edytuj **[Dostosuj] Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow** i przejdź do obszaru **Tworzenie lub aktualizowanie szans sprzedaży** w programie CRM i aktualizowanie **Utwórz nową szansę sprzedaży** i **zaktualizuj istniejące akcje szansy sprzedaży** , aby przypisać wartość **DealValue** do poprawnego pola w programie CRM. Usuń także przypisanie **DealValue** z **szacowanego pola przychód** .

- **Kod kraju konta klienta**: w przypadku tworzenia nowego odwołania wymagane jest podanie dwuliterowego kodu kraju (ISO 3166). Domyślnie kod kraju zostanie zsynchronizowany z i z pola **address1_country** konta w programie CRM. Jeśli w programie CRM znajduje się inne pole do synchronizowania kodu kraju:

   - W przypadku pola kod kraju niewyszukiwania w ramach konta zawierającego dwuliterowy kod:
     - Zaktualizuj nazwę pola **kod kraju konta klienta** w zmiennej środowiskowej Dynamics 365 przy użyciu nazwy pola CRM. Upewnij się, że podajesz nazwę pola, a nie jego nazwę wyświetlaną.
     - Edytuj **[Dostosuj] Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow** i przejdź do pozycji **Utwórz lub Pobierz konto klienta** w akcji CRM, aby przypisać wartość **kraju** do poprawnego pola w programie CRM. Ponadto usuń przypisanie wartości **kraju** z pola **adres 1: kraj/region** .

   - W przypadku pola kod kraju wyszukiwania na koncie:
     - Dodaj nowe pole niestandardowe na koncie i wypełnij je automatycznie przy użyciu dwuliterowego kodu kraju (ISO 3166) na podstawie wartości wybranej w polu wyszukiwania i na odwrót.
     - Postępuj zgodnie z powyższymi krokami pola kod kraju niewyszukiwania, aby synchronizować nowe pole niestandardowe z usługi CRM do i z Centrum partnerskiego.

- **Pola szansy sprzedaży**: Jeśli w polu **szansa sprzedaży** istnieją obowiązkowe pola, które należy wypełnić, Edytuj **[Dostosuj] Utwórz lub pobierz szczegóły z usługi Dynamics 365 Flow** i przejdź do obszaru **Tworzenie lub aktualizowanie szans sprzedaży** w ramach akcji CRM i Aktualizuj **Utwórz nową szansę sprzedaży** , aby przypisać wartości do obowiązkowych pól zgodnie z wymaganiami biznesowymi.
- **Pola potencjalnych klientów**: Jeśli istnieją obowiązkowe pola w **potencjalnym kliencie** , które muszą zostać wypełnione, Edytuj **[Dostosuj] Utwórz lub pobierz szczegóły z usługi Dynamics 365 Flow** i przejdź do pozycji **Utwórz lub zaktualizuj potencjalnego klienta** w programie CRM i Update **Create a New potencjalnego klienta** , aby przypisać wartości do obowiązkowych pól zgodnie z wymaganiami biznesowymi.
- **Konto klienta**: gdy nowe odwołanie jest synchronizowane z Centrum partnerskiego do programu CRM, rozwiązanie do automatyzowania próbuje wyszukać istniejące konto w programie CRM przy użyciu nazwy firmy klienta i kodu pocztowego. Jeśli go nie znajdziesz, w programie CRM zostanie utworzone nowe konto klienta. Aby zaktualizować kryteria wyszukiwania i szczegóły tworzenia nowego konta, Edytuj **[Dostosuj] Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow** i przejdź do pozycji **Utwórz lub Pobierz konto klienta** w akcji CRM i **Utwórz konto klienta**.

## <a name="update-environment-variable"></a>Aktualizowanie zmiennej środowiskowej

Aby zaktualizować wartość zmiennej środowiskowej:

1. Przejdź do strony **rozwiązania** i wybierz pozycję **rozwiązanie domyślne**. Wybierz pozycję **zmienna środowiskowa** , wybierając pozycję **wszystkie**.

1. Wybierz zmienną środowiskową dla wartości, która ma zostać zaktualizowana, a następnie wybierz pozycję **Edytuj** przy użyciu ikony wielokropka.

1. Zaktualizuj **bieżącą wartość** (nie Aktualizuj **wartości domyślnej**) przy użyciu opcji **Nowa wartość** i dostarczając wartości. Wartość musi odpowiadać typowi danych zmiennej. Na przykład typ danych tak lub nie przyjmuje wartość tak lub nie.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Zrzut ekranu przedstawiający aktualizacje zmiennych środowiskowych.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Kompleksowa, dwukierunkowa synchronizacja odwołań

Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania do automatyzowania gotowości można testować synchronizację odwołań między programem Dynamics 365 i centrum partnerskim.

### <a name="prerequisites"></a>Wymagania wstępne

Aby synchronizować odwołania w centrum partnerskim i Dynamics 365 CRM, rozwiązanie do automatyzowania, które wyraźnie określa pola odwołań specyficzne dla firmy Microsoft. Dzięki tej identyfikacji sprzedawca może określić, które odwołania mają być udostępniane firmie Microsoft w celu współsprzedaży.

Zestaw pól niestandardowych i obiektów zostanie dodany w ramach instalacji rozwiązania. Użytkownik będący administratorem programu CRM musi utworzyć osobną sekcję CRM z polami niestandardowymi **szansy sprzedaży** .

Następujące pola niestandardowe powinny być częścią sekcji CRM:

- **Synchronizuj z centrum partnerskim**: czy synchronizować szansę sprzedaży z centrum partnerskim. Domyślnie wartość tego pola nie jest wymagana i musi być jawnie ustawiona na tak przez sprzedawcę w celu udostępnienia szansy sprzedaży firmie Microsoft. Nowe odwołania udostępnione z Centrum partnerskiego do programu CRM będą miały ustawioną wartość tak.
- **Identyfikator odwołania**: pole identyfikatora tylko do odczytu dla odwołania do Centrum partnerskiego.
- **Link do odwołania**: link tylko do odczytu do odwołania w centrum partnerskim.
- **Jak może pomóc firma Microsoft?**: pomoc wymagana przez firmę Microsoft do odwołania. Aby utworzyć odwołanie do współsprzedawcy, wybierz odpowiednią pomoc wymaganą przez firmę Microsoft. Osoba kontaktowa klienta musi być skojarzona z szansą sprzedaży, aby utworzyć odwołanie do współsprzedaży. Aby utworzyć odwołanie nienależące do żadnej transakcji, nie zaznaczaj tego pola. Odwołanie do niewspółpracującej transakcji można przekonwertować na odwołanie do współsprzedawcy w dowolnym momencie, wybierając odpowiednią opcję pomocy wymaganą.
- **Widoczność odwołań w centrum partnerskim firmy Microsoft**: Wybierz widoczność dla referencyjnego Centrum partnerskiego. Dzięki udostępnieniu go dla sprzedawcy firmy Microsoft odwołanie do niewspółpracującej transakcji może zostać przekonwertowane na współsprzedaż. Gdy pomoc firmy Microsoft jest wymagana, odwołanie jest domyślnie widoczne dla sprzedających firmy Microsoft. Gdy to pole jest oznaczone jako widoczne, nie można go przywrócić.
- **Identyfikator programu Microsoft CRM**: po utworzeniu i zaakceptowaniu odwołania do współsprzedawcy przez firmę Microsoft to pole zostanie wypełnione identyfikatorem CRM firmy Microsoft.
- **Produkty: przestarzałe**: nie używaj tego pola ani nie należy go dodawać do sekcji CRM. Jest on dostępny tylko w celu zapewnienia zgodności z poprzednimi wersjami. Zamiast tego użyj rozwiązań Centrum partnerskiego.
- **Inspekcja**: dziennik inspekcji tylko do odczytu na potrzeby synchronizacji z odwołaniami do Centrum partnerskiego.
- **Rozwiązania Microsoft Partner Center**: niestandardowy obiekt służący do kojarzenia gotowych rozwiązań i rozwiązań firmy Microsoft z możliwością sprzedaży. Co najmniej jedno rozwiązanie może zostać dodane lub usunięte z szansy sprzedaży. Przed udostępnieniem jej w firmie Microsoft należy dodać co najmniej jedno rozwiązanie do sprzedaży gotowe lub rozwiązane z firmą Microsoft. Aby skojarzyć ten obiekt z szansą sprzedaży, zaktualizuj formularz **szansa sprzedaży** w programie CRM.

  Wybierz odpowiednią kartę w formularzu **szansa sprzedaży** i Dodaj podsiatkę, jak pokazano poniżej.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Zrzut ekranu pokazujący formularz szansy sprzedaży.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Zrzut ekranu przedstawiający rozwiązania firmy Microsoft.":::

- Po dodaniu rozwiązań firmy Microsoft możesz wstępnie wypełnić szczegółowe informacje o gotowym rozwiązaniu do zakupu, aby sprzedawcy nie musieli dodawać. Aby dodać szczegółowe informacje o nowym rozwiązaniu, przejdź do obiektu szczegóły rozwiązania firmy Microsoft w programie CRM i wybierz pozycję **Dodaj rekord** , aby dodać jeden wpis, lub Użyj **przekazywania programu Excel** , aby dodać wiele wpisów.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Zrzut ekranu pokazujący nowe szczegóły rozwiązania firmy Microsoft.":::

### <a name="scenarios"></a>Scenariusze

1. Synchronizacja odwołań podczas tworzenia lub aktualizowania odwołania w programie CRM oraz synchronizowanie w centrum partnerskim:

   1. Zaloguj się do środowiska Dynamics 365 CRM przy użyciu użytkownika, który ma wgląd w sekcję **szansa sprzedaży** w programie CRM.

   1. Upewnij się, że sekcja **Microsoft Partner Center** jest obecna po utworzeniu nowej szansy sprzedaży w środowisku Dynamics 365.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Zrzut ekranu pokazujący nową szansę sprzedaży.":::

   1. Aby zsynchronizować tę szansę sprzedaży z centrum partnerskim, upewnij się, że ustawisz następujące pola w widoku karty:

      - **Jak może pomóc firma Microsoft?**: Aby utworzyć odwołanie do współsprzedawcy, wybierz odpowiednią opcję pomocy.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Zrzut ekranu pokazujący, jak uzyskać odpowiednie pola w widoku karty.":::

      - **Kontakt z klientem**: Aby utworzyć odwołanie do współsprzedaży, Dodaj kontakt z klientem do szansy sprzedaży.
      - **Synchronizuj z centrum partnerskim**: tak.
      - **Rozwiązania firmy Microsoft**: aby podzielić się z firmą Microsoft, możesz dodać do niej prawidłowe rozwiązanie do tworzenia i wystawiania.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Zrzut ekranu przedstawiający Identyfikator rozwiązania.":::

   1. Po utworzeniu szansy sprzedaży w usłudze Dynamics 365 z opcją **Synchronizuj z centrum partnerskim** ustawionym na wartość tak, odczekaj 10 minut. Następnie zaloguj się do swojego konta Centrum partnerskiego. Twoje odwołania zostaną zsynchronizowane z usługą Dynamics 365 i **identyfikatorem referencyjnym**. **Link odwołania** zostanie wypełniony. Jeśli wystąpi awaria, pole **inspekcji** zostanie wypełnione informacjami o błędzie.
     
    1. Podobnie w przypadku szansy sprzedaży, która ma opcję **Synchronizuj z centrum partnerskim** z ustawioną wartością tak, w przypadku zaktualizowania szansy sprzedaży w programie Dynamics 365 CRM zmiany zostaną zsynchronizowane na koncie Centrum partnerskiego.

    1. Prospekty, które zostały pomyślnie zsynchronizowane z centrum partnerskim, zostaną zidentyfikowane przy użyciu ikony ✔ w usłudze Dynamics 365.

1. Synchronizacja odwołań po utworzeniu lub zaktualizowaniu odwołania w centrum partnerskim i zsynchronizowaniu go w środowisku Dynamics 365:

   1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.

   1. Z menu po lewej stronie wybierz pozycję **odwołania** .

   1. Utwórz nowe odwołanie do towarzyszącej współpracy z poziomu Centrum partnerskiego, wybierając opcję **Nowa transakcja** .

   1. Zaloguj się do środowiska programu Dynamics 365 CRM.

   1. Przejdź do pozycji **otwarte szanse sprzedaży**. Odwołanie utworzone w centrum partnerskim jest teraz synchronizowane w programie Dynamics 365 CRM.

   1. Po wybraniu synchronizowanego odwołania są wypełniane szczegóły widoku karty.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)
- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)
- [Więcej informacji o platformie Microsoft energooszczędnej](/power-automate/)
- [Elementy webhook Centrum partnerskiego](/partner-center/develop/partner-center-webhooks)
