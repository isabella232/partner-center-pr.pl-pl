---
title: Łącznik współsprzedającego dla Centrum partnerskiego programu Dynamics 365 CRM
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj odwołania w centrum partnerskim z łącznikiem współsprzedawanym dla programu Dynamics 365 CRM. Sprzedawcy mogą następnie współsprzedawać z firmą Microsoft w ramach systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645768"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Łącznik współsprzedawanych produktów Dynamics 365 CRM — Omówienie

### <a name="appropriate-roles"></a>Odpowiednie role

- Administrator odwołań
- Administrator systemu lub Konfigurator systemu w programie CRM

Łącznik współpracujący z centrum partnerskim umożliwia sprzedającym współsprzedaż z firmą Microsoft w ramach systemów CRM. Nie trzeba ich przeszkoleć w celu zarządzania pozostałymi ofertami przy użyciu Centrum partnerskiego. Użyj łączników współsprzedania, aby utworzyć nowe odwołanie do współsprzedaży, aby skontaktować się z sprzedawcą firmy Microsoft, otrzymywać odwołania od sprzedawcy firmy Microsoft, akceptować/odrzucać odwołania, modyfikować dane dotyczące transakcji, takie jak wartość transakcji i Data zamknięcia. Możesz również otrzymywać wszelkie aktualizacje od sprzedawcy firmy Microsoft w ramach tych transakcji związanych z współsprzedażą. Możesz zarządzać wszystkimi odwołaniami w wybranym przez Ciebie programie CRM, a nie w centrum partnerskim. 

Rozwiązanie jest oparte na rozwiązaniu Microsoft energooszczędne i korzysta z interfejsów API Centrum partnerskiego.

## <a name="before-you-install---pre-requisites"></a>Przed zainstalowaniem — wymagania wstępne

|**Tematy**   |**Szczegóły**   |**Linki**   |
|--------------|--------------------|------|
|Identyfikator Microsoft Partner Network |Potrzebujesz prawidłowego identyfikatora MPN|Aby dołączyć [MPN](https://partner.microsoft.com/)|
|Gotowe do rozsprzedaj|Twoje rozwiązanie do adresów IP/usług musi być gotowe do współpracy.|[Sprzedawanie z firmą Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Konto Centrum partnerskiego|IDENTYFIKATOR MPN skojarzony z dzierżawcą Centrum partnerskiego musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współsprzedażu. Przed wdrożeniem łączników Sprawdź, czy w portalu Centrum partnerskiego są widoczne swoje odwołania do współsprzedawcy.|[Zarządzanie kontem](create-user-accounts-and-set-permissions.md)|
|Role użytkowników Centrum partnerskiego|Pracownik, który zainstaluje łączniki i korzysta z nich, musi być administratorem odwołań|[Przypisywanie ról i uprawnień użytkowników](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|Rola użytkownika programu CRM to administrator systemu lub Konfigurator systemu|[Przypisywanie ról w usłudze Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Konto przepływu automatyzacji|Utwórz nowe środowisko produkcyjne przy użyciu bazy danych do testowania/przemieszczania i produkcji. Jeśli masz istniejące środowisko produkcyjne z bazą danych, można je ponownie wykorzystać. Użytkownik, który zamierza zainstalować rozwiązanie łącznika, musi mieć licencję na automatyzację i dostęp do tego środowiska. Możesz monitorować postęp i uzyskać więcej szczegółów, jeśli instalacja nie powiedzie się [w programie, klikając](https://flow.microsoft.com/) pozycję Zobacz historię w obszarze rozwiązania.|[Utwórz środowisko lub Zarządzaj nim](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Zainstaluj synchronizację odwołań Centrum partnerskiego dla programu Dynamics 365 (rozwiązanie do automatyzowania zarządzania)

1. Przejdź do pozycji [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **środowiska** w prawym górnym rogu. W tym kroku przedstawiono dostępne wystąpienia programu CRM.

2. Wybierz odpowiednie wystąpienie programu CRM z listy rozwijanej w prawym górnym rogu.

3. Wybierz pozycję **rozwiązania** na lewym pasku nawigacyjnym.

4. Kliknij link **Otwórz AppSource** w górnym menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz AppSource":::

5. Wyszukaj **Łączniki dla usługi Partner Center dla Dynamics365** na ekranie podręcznym.  

6. Kliknij przycisk **Pobierz teraz** , a następnie **Kontynuuj**.

7. Spowoduje to otwarcie strony, na której można wybrać środowisko CRM (Dynamics 365), aby zainstalować aplikację.  Zgadzam się na warunki i postanowienia.

8. Możesz monitorować postęp i uzyskać więcej szczegółów, jeśli instalacja nie powiedzie się w programie, klikając pozycję **Zobacz historię** w obszarze **rozwiązania**.
 

9. Po zakończeniu instalacji przejdź z powrotem do strony [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **rozwiązania** z lewego obszaru nawigacji. Zwróć uwagę na to, że w ramach listy rozwiązań jest dostępny komunikat **dotyczący usługi Partner Center dotyczącej synchronizacji dla usługi Dynamics 365** .

10. Wybierz pozycję **Centrum partnerskie — synchronizacja dla programu Dynamics 365**. Dostępne są następujące przepływy automatyzacji i jednostki:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Dostępne CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>Najlepsze rozwiązanie: testowanie przed rzeczywistym użyciem

Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania do automatyzowania w środowisku produkcyjnym należy przetestować rozwiązanie w tymczasowym wystąpieniu programu CRM.

- Zainstaluj rozwiązanie Microsoft PowerShell automatyzuje w wystąpieniu środowiska przejściowego/programu CRM.
- Skonfiguruj i Dostosuj rozwiązanie firmy Microsoft do automatyzowania w środowisku przejściowym.
- Przetestuj rozwiązanie w wystąpieniu przemieszczania/programu CRM. 
- W przypadku powodzenia zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego. 

## <a name="configure-the-solution"></a>Skonfiguruj rozwiązanie

1. Po zainstalowaniu rozwiązania w wystąpieniu programu CRM przejdź z powrotem do narzędzia do [automatyzacji](https://flow.microsoft.com/).


2. Z listy rozwijanej **środowiska** w prawym górnym rogu wybierz wystąpienie programu CRM, na którym zainstalowano rozwiązanie do automatyzowania.

3. Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:

   - Użytkownik Centrum partnerskiego z poświadczeniami administratora

   - Zdarzenia Centrum partnerskiego

   - Administrator programu CRM z przepływem automatyzacji w rozwiązaniu.

      1. Wybierz pozycję **połączenia** na lewym pasku nawigacyjnym i wybierz z listy rozwiązanie "referencje do Centrum partnerskiego".

      2. Utwórz połączenie, klikając pozycję **Utwórz połączenie**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Tworzenie połączenia":::

      3. Wyszukaj **Referencje Centrum partnerskiego (wersja zapoznawcza)** na pasku wyszukiwania w prawym górnym rogu.

      4. Utwórz połączenie dla użytkownika Centrum partnerskiego z rolą poświadczeń administratora.

      5. Następnie utwórz połączenie zdarzeń Centrum partnerskiego dla użytkownika Centrum partnerskiego z poświadczeniami administratora odwołań.

      6. Utwórz połączenie dla Common Data Service (bieżące środowisko) dla użytkownika Administrator programu CRM.
     
      7. Po dodaniu wszystkich połączeń powinny zostać wyświetlone następujące połączenia w danym środowisku:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Połączenia":::
   
## <a name="edit-the-connections"></a>Edytuj połączenia

1. Wróć do strony **rozwiązania** i wybierz pozycję **domyślne rozwiązanie**. Wybierz pozycję **odwołanie do połączenia (wersja zapoznawcza)** , klikając pozycję **wszystkie**.

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="Połącz":::

2. Edytuj poszczególne połączenia po jednym, wybierając ikonę z trzema kropkami. Dodaj odpowiednie połączenia.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Wymienione połączenia"::: 

3.  Wróć do strony rozwiązania, wybierz pozycję Centrum partnerskie odwolania synchronizacji dla programu Dynamics 365 i Włącz przepływ, klikając trzy kropki obok każdego przepływu w następującej sekwencji. Jeśli podczas włączania przepływu wystąpią jakiekolwiek problemy, zapoznaj się z [krokami dostosowywania](connector-dynamics.md#customize-synchronization-steps) i [procedurami rozwiązywania problemów](connectors-troubleshoot.md). 

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

Interfejsy API elementu webhook Centrum partnerskiego umożliwiają rejestrację zdarzeń zmiany zasobów. Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.

1. Wybierz pozycję **Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu testowego)**.

2. Wybierz ikonę **Edytuj** i wybierz, **kiedy zostanie odebrane żądanie HTTP**.

3. Wybierz ikonę **kopiowania** , aby skopiować podany adres URL post protokołu HTTP.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopiowanie adresu URL":::

4. Teraz wybierz pozycję "Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)", a następnie wybierz pozycję **Uruchom**.

5. Upewnij się, że okno "przebieg przepływu" otwiera się w okienku po prawej stronie, a następnie kliknij przycisk **Kontynuuj**.

6. Wprowadź następujące informacje:

   - **Punkt końcowy wyzwalacza http**: adres URL skopiowany z wcześniejszego kroku

   - **Zdarzenia do zarejestrowania**: Wybierz wszystkie dostępne zdarzenia ("odwołanie-utworzone", "odwołanie-zaktualizowane", "powiązane z odwołaniem-utworzono", "powiązane z odwołaniem-zaktualizowane")

   -**Zastąp istniejące punkty końcowe wyzwalacza, jeśli istnieją**: tak należy zauważyć, że dla danego zdarzenia elementu webhook można zarejestrować tylko jeden adres URL. Należy pamiętać, że dla danego zdarzenia elementu webhook można zarejestrować tylko jeden adres URL. 

7. Wybierz pozycję **Uruchom** , a następnie wybierz pozycję **gotowe.**

Element webhook może teraz nasłuchiwać zdarzeń tworzenia i aktualizowania.

## <a name="customize-synchronization-steps"></a>Dostosowywanie kroków synchronizacji

Systemy CRM są wysoce dostosowane i można dostosować rozwiązanie do automatyzowania zarządzania, korzystając z konfiguracji programu CRM.  Po zsynchronizowaniu odwołań towarzyszących między centrum partnerskim i systemem CRM pola, które są synchronizowane na komputerze Centrum partnerskiego, są wyświetlane w [przewodniku mapowania pól niestandardowych](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w temacie **[Dostosowywanie] Utwórz lub Pobierz szczegóły z przepływu Dynamics 365**  lub zmiennych środowiskowych. Zaleca się, aby nie aktualizować żadnych innych przepływów w rozwiązaniu do automatyzacji, ponieważ mogą one wpływać na przyszłe uaktualnienia rozwiązań. 

Dostępne są następujące dostosowania:

- Znacznik wyboru w polu Nazwa szansy sprzedaży: domyślnie zostanie wyświetlony znacznik wyboru obok pozycji Nazwa szansy sprzedaży, aby wskazać, że synchronizacja między centrum partnerskim a programem Dynamics 365 CRM zakończyła się pomyślnie. Analogicznie, jeśli synchronizacja nie powiedzie się, zostanie wyświetlony krzyżyk. Aby uniknąć dodawania znacznika wyboru lub znakowania krzyżowego w polu Nazwa szansy sprzedaży, ustaw bieżącą wartość pola wyboru wyświetlania w zmiennej środowiskowej nazwa szansy do nie.

- Wartość transakcji: Domyślnie wartość transakcji z Centrum partnerskiego będzie synchronizowana z i z **estimatedvalue** w programie CRM. Jeśli masz inne pole w programie CRM dla wartości transakcji do synchronizowania z:

    a.    Zaktualizuj nazwę pola wartości transakcji w zmiennej środowiskowej Dynamics 365 przy użyciu nazwy pola CRM. Należy pamiętać, że należy podać nazwę pola, a nie jego nazwę wyświetlaną.

    b.    Edytuj **[Dostosuj] Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow**  i przejdź do w celu **utworzenia lub zaktualizowania** szans sprzedaży w programie CRM i aktualizacji **Utwórz nową szansę sprzedaży** i **zaktualizuj istniejące akcje dla szans sprzedaży** , aby przypisać wartość **DealValue** do prawidłowego pola w programie CRM. Usuń także **przypisanie DealValue** z **szacowanego pola przychód** .

- Kod kraju konta klienta: w przypadku tworzenia nowego odwołania należy podać dwuliterowy kod kraju (ISO 3166). Domyślnie kod kraju zostanie zsynchronizowany z polem address1_country i z konta w programie CRM. Jeśli masz inne pole w programie CRM for Country Code do synchronizowania:

   a.    W przypadku pola kod kraju bez wyszukiwania w ramach konta zawierającego dwuliterowy kod:

   - Zaktualizuj nazwę pola kod kraju konta klienta w zmiennej środowiskowej Dynamics 365 przy użyciu nazwy pola CRM. Należy pamiętać, że należy podać nazwę pola, a nie jego nazwę wyświetlaną.

   - Edytuj **[Dostosuj] Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow**  i przejdź do pola Utwórz lub Pobierz konto klienta w programie CRM akcja, aby przypisać wartość kraju do korekty w programie CRM. Usuń także przypisanie wartości kraju z adresu 1: pole kraju/regionu.

   b.    W przypadku pola kodu kraju wyszukiwania na koncie:

   - Dodaj nowe pole niestandardowe na koncie i wypełnij je automatycznie przy użyciu dwuliterowego kodu kraju (ISO 3166) na podstawie wartości wybranej w polu wyszukiwania i na odwrót.

   - Postępuj zgodnie z powyższymi krokami pola kod kraju bez wyszukiwania, aby synchronizować nowe pole niestandardowe z programu CRM do i z Centrum partnerskiego.

- Pola szansy sprzedaży: Jeśli istnieją obowiązkowe pola, które wymagają wypełnienia opcji Edytuj **[Dostosuj], Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow**  i przejdź do opcji **Utwórz lub zaktualizuj szansę sprzedaży** w programie CRM i zaktualizuj **nową szansę sprzedaży** , aby przypisać wartości do pól obowiązkowych zgodnie z wymaganiami biznesowymi.

- Pola potencjalnych klientów: Jeśli w potencjalnym kliencie istnieją obowiązkowe pola, które wymagają wypełnienia opcji Edytuj **[Dostosuj], Utwórz lub Pobierz szczegóły z usługi Dynamics 365 Flow**  i przejdź do opcji **Utwórz lub zaktualizuj potencjalnego klienta** w programie CRM i zaktualizuj **Tworzenie nowego potencjalnego klienta** , aby przypisać wartości do pól obowiązkowych zgodnie z wymaganiami biznesowymi.

- Konto klienta: gdy nowe odwołanie jest synchronizowane z Centrum partnerskiego do programu CRM, rozwiązanie do automatyzowania próbuje wyszukać istniejące konto w programie CRM przy użyciu nazwy firmy klienta i kodu pocztowego. Jeśli go nie znajdziesz, w programie CRM zostanie utworzone nowe konto klienta. Aby zaktualizować kryteria wyszukiwania i szczegółowe informacje dotyczące tworzenia konta, Edytuj **[Dostosuj] Utwórz lub Pobierz szczegóły z przepływu usługi Dynamics 365** i przejdź do okna **Utwórz lub Pobierz konto klienta** w programie CRM i **Utwórz akcję konta klienta**.

## <a name="update-environment-variable"></a>Aktualizowanie zmiennej środowiskowej

Aby zaktualizować wartość zmiennej środowiskowej:

1. Przejdź do strony **rozwiązania** i wybierz pozycję **domyślne rozwiązanie**. Wybierz pozycję **zmienna środowiskowa** , klikając pozycję Wszystkie.

2. Wybierz zmienną środowiskową dla wartości, która ma zostać zaktualizowana, a następnie kliknij pozycję **Edytuj** przy użyciu ikony trzy kropki.

3. Zaktualizuj **bieżącą wartość** (nie Aktualizuj wartości domyślnej) przy użyciu opcji **Nowa wartość** i podaj wartość. Wartość musi być zgodna z typem danych zmiennej dla przykładu. tak/nie typ danych akceptuje wartość tak lub nie.

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="Pole edycji dla wartości domyślnych":::

- Kompleksowa synchronizacja odwołań dwukierunkowych

Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania do automatyzowania gotowości można testować synchronizację odwołań między programem Dynamics 365 i centrum partnerskim.

### <a name="pre-requisites"></a>Wymagania wstępne

Aby synchronizować odwołania w centrum partnerskim i Dynamics 365 CRM, rozwiązanie do automatyzowania, które wyraźnie określa pola odwołań specyficzne dla firmy Microsoft. Dzięki tej identyfikacji sprzedawca może określić, które odwołania mają być udostępniane firmie Microsoft w celu współsprzedaży.

Zestaw niestandardowych pól i obiektów zostanie dodany jako część instalacji rozwiązania. Użytkownik będący administratorem programu CRM musi utworzyć osobną sekcję CRM z polami niestandardowymi **szansy sprzedaży** .

Następujące pola niestandardowe powinny być częścią sekcji CRM:

- **Synchronizuj z centrum partnerskim**: czy synchronizować szansę sprzedaży z Centrum partnerskiego firmy Microsoft. Domyślnie wartość tego pola nie jest wymagana i musi być jawnie ustawiona na tak przez sprzedawcę w celu udostępnienia szansy sprzedaży firmie Microsoft. Nowe odwołania udostępnione z Centrum partnerskiego do programu CRM będą miały ustawioną wartość tak.

- **Identyfikator odwołania**: pole identyfikatora tylko do odczytu dla odwołania do Centrum partnerskiego firmy Microsoft

- **Link do odwołania**: link tylko do odczytu do odwołania w centrum partnerskim firmy Microsoft
- **Jak może pomóc firma Microsoft?**: pomoc wymagana przez firmę Microsoft do odwołania. Aby utworzyć odwołanie do współsprzedawcy, wybierz odpowiednią pomoc wymaganą przez firmę Microsoft. Osoba kontaktowa klienta musi być skojarzona z szansą sprzedaży, aby utworzyć odwołanie do współsprzedaży. Aby utworzyć odwołanie nienależące do mnie, pozostaw to pole niezaznaczoną. Odwołanie do innej transakcji można przekonwertować na odwołanie do współsprzedawcy w dowolnym momencie, wybierając odpowiednią opcję Pomoc wymagana.

- **Widoczność referencji do Centrum partnerskiego firmy Microsoft**: Wybierz widoczność dla referencyjnego Centrum partnerskiego firmy Microsoft. Dzięki udostępnieniu go dla sprzedawcy firmy Microsoft odwołanie do niesprzedawanej transakcji może zostać przekonwertowane na współsprzedaż. Gdy pomoc firmy Microsoft jest wymagana, odwołanie jest domyślnie widoczne dla sprzedających firmy Microsoft. Po oznaczeniu jako widoczne nie można przywrócić tego pola.

- **Identyfikator programu Microsoft CRM**: po utworzeniu i zaakceptowaniu odwołania do współsprzedawcy przez firmę Microsoft to pole zostanie wypełnione identyfikatorem CRM firmy Microsoft.

- **Produkty: przestarzałe** — nie używaj tego pola ani nie dodawaj go do sekcji CRM. jest on dostępny tylko w celu zapewnienia zgodności z poprzednimi wersjami. Zamiast tego użyj rozwiązań Centrum partnerskiego firmy Microsoft.

- **Inspekcja**: dziennik inspekcji tylko do odczytu na potrzeby synchronizacji z odwołaniami do Centrum partnerskiego

- **Rozwiązania Microsoft Partner Center**: niestandardowy obiekt służący do kojarzenia gotowych rozwiązań i rozwiązań firmy Microsoft z możliwością sprzedaży. Co najmniej jedno rozwiązanie może zostać dodane i/lub usunięte z szansy sprzedaży. Przed udostępnieniem jej w firmie Microsoft należy dodać co najmniej jedno rozwiązanie do sprzedaży gotowe lub oferowane przez firmę Microsoft. Aby skojarzyć ten obiekt z szansą sprzedaży, zaktualizuj formularz szansy sprzedaży w programie CRM:

  Wybierz odpowiednią kartę w formularzu szansa i Dodaj podsiatkę, jak pokazano poniżej:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Formularz szansy sprzedaży":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- Po dodaniu rozwiązań firmy Microsoft możesz wstępnie wypełnić szczegółowe informacje o gotowych rozwiązaniach do sprzedaży, aby nie trzeba było ich dodawać. Aby dodać szczegółowe informacje o rozwiązaniu, przejdź do obiektu szczegóły rozwiązania firmy Microsoft w programie CRM i kliknij pozycję **Dodaj rekord** , aby dodać jeden wpis, lub użyj polecenia **Przekaż do programu Excel** , aby dodać wiele wpisów.

:::image type="content" source="images/dynamic-1a.png" alt-text="Szczegóły rozwiązania":::

### <a name="scenarios"></a>SYTUACJI

1. Synchronizacja odwołań podczas tworzenia lub aktualizowania odwołania w programie CRM oraz synchronizowanie w centrum partnerskim:

   1. Zaloguj się do środowiska Dynamics 365 CRM przy użyciu użytkownika, który ma wgląd w sekcję **szansa sprzedaży** w programie CRM.

   2. Upewnij się, że sekcja Centrum partnerskiego firmy Microsoft jest obecna w przypadku tworzenia nowej szansy sprzedaży w środowisku Dynamics 365

   :::image type="content" source="images/dynamic-2a.png" alt-text="Nowa szansa sprzedaży"::: 

   3. Aby zsynchronizować tę szansę sprzedaży z centrum partnerskim, upewnij się, że ustawisz następujące pola w widoku karty:

      - **Jak może pomóc firma Microsoft?**: Aby utworzyć odwołanie do współsprzedawcy, wybierz odpowiednią opcję pomocy.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Jak uzyskać odpowiednie pola w widoku karty":::

      - **Kontakt z klientem**: Aby utworzyć odwołanie do współsprzedaży, Dodaj kontakt z klientem do szansy sprzedaży.
      - **Synchronizuj z centrum partnerskim**: tak

      - Rozwiązania firmy Microsoft: aby podzielić się z firmą Microsoft, należy dodać ważne rozwiązanie do sprzedaży gotowe lub firmy Microsoft.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="Identyfikator rozwiązania":::

   4. Po utworzeniu szansy sprzedaży w usłudze Dynamics 365 z opcją Synchronizuj z centrum partnerskim ustawionym na wartość tak, odczekaj 10 minut, a następnie zaloguj się do konta Centrum partnerskiego. Twoje odwołania zostaną zsynchronizowane z usługą Dynamics 365 i identyfikatorem referencyjnym. Link odwołania zostanie wypełniony. W przypadku awarii pole inspekcji zostanie wypełnione informacjami o błędzie.
     
    5. Podobnie w przypadku opcji "Synchronizuj z centrum partnerskim" o wartości "tak" w przypadku zaktualizowania szansy sprzedaży w programie Dynamics 365 CRM zmiany zostaną zsynchronizowane na koncie Centrum partnerskiego.

    6. Prospekty, które zostały pomyślnie zsynchronizowane z centrum partnerskim, zostaną zidentyfikowane przy użyciu ikony ✔ w usłudze Dynamics 365.

2. Synchronizacja odwołań po utworzeniu lub zaktualizowaniu odwołania w centrum partnerskim firmy Microsoft i zsynchronizowaniu w środowisku Dynamics 365:

   1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.

   2. Wybierz **odwołania** z menu po lewej stronie.

   3. Utwórz nowe odwołanie do towarzyszącej współpracy z poziomu Centrum partnerskiego, wybierając opcję  **Nowa transakcja** .

   4. Zaloguj się do środowiska programu Dynamics 365 CRM.

   5. Przejdź do **okna Otwórz szanse sprzedaży**. Odwołanie utworzone w Centrum partnerskiego firmy Microsoft jest teraz synchronizowane w programie Dynamics 365 CRM.

   6. Po wybraniu synchronizowanego odwołania są wypełniane szczegóły widoku karty.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)

- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)

- [Więcej informacji na temat platformy Microsoft energooszczędnej?](/power-automate/)

- [Elementy webhook Centrum partnerskiego](/partner-center/develop/partner-center-webhooks)