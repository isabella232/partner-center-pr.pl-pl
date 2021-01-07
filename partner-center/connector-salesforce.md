---
title: Łącznik współsprzedawanego Centrum partnerskiego usług Salesforce CRM
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj swoje odwołania w centrum partnerskim z Twoim programem Salesforce CRM. Sprzedawcy mogą następnie współsprzedawać z firmą Microsoft w ramach systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 68b8bdf7a88c1ca8d063cf3198fc49bf87552edb
ms.sourcegitcommit: de2ac2eea26426ae8f962d29ab50b68850318ce6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/07/2021
ms.locfileid: "97960955"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Łącznik współpracujący z usługą Salesforce CRM — Omówienie

### <a name="appropriate-roles"></a>Odpowiednie role

- Administrator odwołań
- Administrator systemu lub Konfigurator systemu w programie CRM

Łącznik współpracujący z centrum partnerskim umożliwia sprzedającym współsprzedaż z firmą Microsoft w ramach systemów CRM. Nie trzeba ich przeszkoleć w celu zarządzania pozostałymi ofertami przy użyciu Centrum partnerskiego. Korzystając z łączników współsprzedających, można utworzyć nowe odwołanie do sprzedaży, aby skontaktować się z sprzedającym firmy Microsoft, otrzymać odwołania od sprzedawcy firmy Microsoft, zaakceptować/odrzucić odwołania, zmodyfikować dane dotyczące transakcji, takie jak wartość transakcji i Data zamknięcia.  Możesz również otrzymywać wszelkie aktualizacje od sprzedawcy firmy Microsoft w ramach tych transakcji związanych z współsprzedażą. Wszystkie odwołania można wykonywać podczas pracy w wybranym programie CRM, a nie w centrum partnerskim. 

Rozwiązanie jest oparte na rozwiązaniu Microsoft energooszczędne i korzysta z interfejsów API Centrum partnerskiego.

## <a name="before-you-install---pre-requisites"></a>Przed zainstalowaniem — wymagania wstępne

|**Tematy**   |**Szczegóły**   |**Linki**   |
|--------------|--------------------|------|
|Identyfikator Microsoft Partner Network |Potrzebujesz prawidłowego identyfikatora MPN|Aby dołączyć [MPN](https://partner.microsoft.com/)|
|Gotowe do rozłożenia|Twoje rozwiązanie do adresów IP/usług musi być gotowe do współpracy.|[Sprzedawanie z firmą Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Konto Centrum partnerskiego|IDENTYFIKATOR MPN skojarzony z dzierżawcą Centrum partnerskiego musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współsprzedażu. Przed wdrożeniem łączników Sprawdź, czy w portalu Centrum partnerskiego są widoczne swoje odwołania do współsprzedawcy.|[Zarządzanie kontem](create-user-accounts-and-set-permissions.md)|
|Role użytkowników Centrum partnerskiego|Pracownik, który zainstaluje łączniki i korzysta z nich, musi być administratorem odwołań|[Przypisywanie ról i uprawnień użytkowników](create-user-accounts-and-set-permissions.md)|
|Aplikacja Salesforce CRM|Rola użytkownika programu CRM to administrator systemu lub Konfigurator systemu|[Przypisywanie ról w programie Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Konto przepływu automatyzacji|Aktywne konto usługi [Automatyzowanie](https://flow.microsoft.com) dla administratora systemu lub konfiguratora systemu programu CRM. Ten użytkownik powinien zalogować się do programu w celu [automatyzacji](https://flow.microsoft.com) co najmniej raz przed instalacją.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalacja pakietu Salesforce dla pól niestandardowych firmy Microsoft 

Aby zsynchronizować odwołania w centrum partnerskim i programie Salesforce CRM, rozwiązanie do automatyzowania oprogramowania musi jasno identyfikować pola odwołań określonych przez firmę Microsoft. To rozgraniczenie zapewnia zespołom sprzedawcy partnerskiego możliwość decydowania, które odwołania chcą udostępnić firmie Microsoft w celu współsprzedaży.

1. W usłudze Salesforce Aktywuj **uwagi** i Dodaj je do listy powiązane szanse sprzedaży. 
[Odwołanie](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aktywuj **zespoły szans sprzedaży** , wykonując następujące czynności: 
    - W obszarze Konfiguracja Użyj pola **szybkiego wyszukiwania** , aby zlokalizować ustawienia zespołu szans sprzedaży.
    - Zdefiniuj ustawienia zgodnie z wymaganiami.
[Odwołanie](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. W usłudze Salesforce Zainstaluj pola niestandardowe i obiekty przy użyciu Instalatora pakietów poniżej.
  
Przejdź [tutaj](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) , aby zainstalować pakiet w dowolnej firmie.


Uwaga: w przypadku instalowania w piaskownicy należy zamienić początkową część adresu URL na http://test.salesforce.com

4. W usłudze Salesforce Dodaj rozwiązania firmy Microsoft do listy powiązanej z **szansą sprzedaży** . Po dodaniu **kliknij ikonę klucza** i zaktualizuj właściwości.

## <a name="best-practice-test-before-you-go-live"></a>Najlepsze rozwiązanie: testowanie przed rzeczywistym użyciem

Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania do automatyzowania w środowisku produkcyjnym należy przetestować rozwiązanie w tymczasowym wystąpieniu programu CRM.

- Zainstaluj rozwiązanie Microsoft PowerShell automatyzuje w wystąpieniu środowiska przejściowego/programu CRM.

- Utwórz kopię rozwiązania i przeprowadź konfigurację i uruchom dostosowania przepływu w środowisku przejściowym.

- Przetestuj rozwiązanie w wystąpieniu przemieszczania/programu CRM.

- Po pomyślnym zaimportowaniu jako rozwiązania zarządzanego do wystąpienia produkcyjnego.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Zainstaluj synchronizację odwołań Centrum partnerskiego dla programu Salesforce CRM

1. Przejdź do pozycji [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **środowiska** w prawym górnym rogu. Spowoduje to wyświetlenie dostępnych wystąpień programu CRM.

2. Wybierz odpowiednie wystąpienie programu CRM z listy rozwijanej w prawym górnym rogu.

3. Wybierz pozycję **rozwiązania** na lewym pasku nawigacyjnym.

4. Kliknij link **Otwórz AppSource** w górnym menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz AppSource":::

5. Wyszukaj **Łączniki dla Centrum partnerskiego dla usługi Salesforce** na ekranie podręcznym.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Kliknij przycisk **Pobierz teraz** , a następnie **Kontynuuj**.

7. Spowoduje to otwarcie strony, na której można wybrać środowisko CRM programu Salesforce do zainstalowania aplikacji.  Zgadzam się na warunki i postanowienia.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostępne CRMS":::

8. Następnie nastąpi przekierowanie do strony **zarządzanie rozwiązaniami** .  Przejdź do pozycji "referencje do Centrum partnerskiego" przy użyciu przycisków strzałek u dołu strony. **Zaplanowana instalacja** powinna pojawić się obok rozwiązania do tworzenia odwołań do Centrum partnerskiego. Instalacja zajmie 10-15 minut.

9. Po zakończeniu instalacji przejdź z powrotem do strony [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **rozwiązania** z lewego obszaru nawigacji. Zwróć uwagę na to, że na liście rozwiązań jest dostępna informacja **dotycząca usługi Partner Center dotyczącej synchronizacji dla usługi Salesforce** .

10. Wybierz pozycję **Centrum partnerskie — synchronizacja** z usługą Salesforce. Dostępne są następujące przepływy automatyzacji i jednostki:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Przepływy usług Salesforce":::



## <a name="configure-the-solution"></a>Skonfiguruj rozwiązanie

1. Po zainstalowaniu rozwiązania w wystąpieniu programu CRM przejdź z powrotem do narzędzia do [automatyzacji](https://flow.microsoft.com/).

2. Z listy rozwijanej **środowiska** w prawym górnym rogu wybierz wystąpienie programu CRM, na którym zainstalowano rozwiązanie do automatyzowania.
3. Konieczne będzie utworzenie połączeń, które kojarzą trzy konta użytkowników:
    - Użytkownik Centrum partnerskiego z poświadczeniami administratora
    - Zdarzenia Centrum partnerskiego
    - Administrator programu CRM z przepływem automatyzacji w rozwiązaniu.
4. Wybierz pozycję **połączenia** na lewym pasku nawigacyjnym i wybierz z listy rozwiązanie "referencje do Centrum partnerskiego".

5. Utwórz połączenie, klikając pozycję **Utwórz połączenie**.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Tworzenie połączenia":::

- Wyszukaj Referencje Centrum partnerskiego (wersja zapoznawcza) na pasku wyszukiwania w prawym górnym rogu.

- Utwórz połączenie dla użytkownika Centrum partnerskiego z rolą poświadczeń administratora.

-  Następnie utwórz połączenie zdarzeń Centrum partnerskiego dla użytkownika Centrum partnerskiego z poświadczeniami administratora odwołań.

- Utwórz połączenie usługi Salesforce dla użytkownika administratora programu CRM.

-  Po dodaniu wszystkich połączeń powinny zostać wyświetlone następujące połączenia w danym środowisku:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Obserwuj połączenia":::

### <a name="edit-the-connections"></a>Edytuj połączenia

1. Wróć do strony rozwiązania i wybierz pozycję **domyślne rozwiązanie**.  Wybierz pozycję **odwołanie do połączenia (wersja zapoznawcza)** , klikając pozycję **wszystkie**.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Rozpocznij edycję łącznika":::

2. Edytuj poszczególne połączenia po jednym, wybierając ikonę z trzema kropkami. Dodaj odpowiednie połączenia.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edytuj łączniki":::

3. Włącz przepływy w następującej kolejności:

- Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Utwórz odwołanie do towarzyszącej usługi Salesforce do Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Centrum partnerskie — aktualizacje referencyjne firmy Microsoft do usługi Salesforce (wersja zapoznawcza programu testowego)
- Centrum partnerskie do usługi Salesforce (wersja zapoznawcza programu testowego)
- Centrum usług Salesforce dla partnerów partnerskich (wersja zapoznawcza)
- Okazja do Centrum partnerskiego w usłudze Salesforce (wersja zapoznawcza)
- Rozwiązania firmy Microsoft do Centrum partnerskiego (wersja zapoznawcza)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementu webhook

Interfejsy API elementu webhook Centrum partnerskiego umożliwiają rejestrację zdarzeń zmiany zasobów. Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.

1. Aby zarejestrować adres URL, wybierz pozycję **rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza)** .

2. Dodaj połączenia dla (a) użytkownika Centrum partnerskiego z poświadczeniami administratora (b.) Centrum partnerskiego, jak zostało to wyróżnione poniżej

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz":::

3. Po wprowadzeniu tych aktualizacji zobaczysz

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Elementy webhook":::

4. Zapisz zmiany i wybierz pozycję **Włącz**.

   Aby włączyć elementy webhook Centrum partnerskiego do nasłuchiwania zmian zdarzeń, wykonaj następujące czynności:

5. Wybierz pozycję **Centrum partnerskie w programie Salesforce CRM (wersja zapoznawcza programu testowego)**.

6. Wybierz ikonę **Edytuj** i wybierz, **kiedy zostanie odebrane żądanie HTTP**.

7. Wybierz ikonę **kopiowania** , aby skopiować podany adres URL post protokołu HTTP.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopiowanie adresu URL":::

8. Teraz wybierz pozycję "Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)", a następnie wybierz pozycję **Uruchom**.

9. Upewnij się, że okno "przebieg przepływu" otwiera się w okienku po prawej stronie, a następnie kliknij przycisk **Kontynuuj**.

10. Wprowadź następujące informacje:

    1. **Punkt końcowy wyzwalacza http**: adres URL skopiowany z wcześniejszego kroku

    2. **Zdarzenia do zarejestrowania**: "utworzono odwołanie" i "odwołanie-zaktualizowane"

    3. **Zastąp istniejące punkty końcowe wyzwalacza, jeśli istnieją**: tak (spowoduje to zastąpienie wszystkich istniejących punktów końcowych).

11. Wybierz pozycję **Uruchom** , a następnie wybierz pozycję **gotowe.**

Element webhook może teraz nasłuchiwać zdarzeń tworzenia i aktualizowania.

## <a name="customize-synchronization-steps"></a>Dostosowywanie kroków synchronizacji

Po zsynchronizowaniu odwołań między centrum partnerskim i systemem CRM pola, które są synchronizowane na komputerze Centrum partnerskiego, są wyświetlane w tym miejscu.

Często Systemy CRM są wysoce dostosowane. Można dostosować przepływy automatyzacji. Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w krokach przepływów automatyzacji.  Dostępne są mapowania centrów partnerskich firmy Microsoft do programu CRM, ale w oparciu o środowisko programu CRM można wybrać dalsze Dostosowywanie pól.

W zależności od potrzeb można dostosować wiele kroków poszczególnych przepływów automatyzacji. Poniżej przedstawiono przykłady dostępnych dostosowań:

1. Aby dostosować pola dla zdarzeń tworzenia lub aktualizacji w centrum partnerskim do synchronizacji odwołań CRM:

   1. Wybierz pozycję Centrum partnerskie w programie Salesforce CRM (wersja zapoznawcza programu testowego).

   2. Wybierz pozycję **Edytuj** , aby edytować/dostosować przepływ automatyzacji.

   3. Wybierz **(zakres) zsynchronizuj potencjalnego klienta lub szansę sprzedaży**.

2. Aby dostosować mapowania pól programu CRM dla zdarzeń tworzenia, wybierz opcję **Jeśli jest to nowa udostępniona okazja, a następnie**. Wybierz podkrok, **Jeśli tak** , a następnie rozwiń pozycję **Tworzenie nowej szansy sprzedaży w programie CRM**. Mapowania w tej sekcji można edytować za pomocą przewodnika mapowania pól.

   1. Aby dostosować mapowania pól programu CRM dla zdarzeń aktualizacji, kliknij krok "(zakres) zsynchronizuj potencjalny klient lub szansę".

   2. Wybierz **, czy jest to aktualizacja szansy sprzedaży, a następnie**. Wybierz podkrok, **Jeśli tak** , a następnie rozwiń **, jeśli różnica między obiektami szansy sprzedaży w centrum partnerskim i CRM**.  

   3. Wybierz opcję **tak** , po której następuje **Aktualizacja istniejącej szansy sprzedaży**

3. Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla zdarzeń aktualizacji:

   1. Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.

   2. Wybierz **(zakres) zsynchronizuj szansę sprzedaży**.

   3. Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń aktualizacji, należy wybrać, **czy istnieje różnica między obiektami lidera w centrum partnerskim i CRM, a następnie**.

   4. Wybierz krok podrzędny, **Jeśli tak** , a następnie rozwiń krok **Aktualizuj odwołanie z danymi o szansie sprzedaży**.

   Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.

4. Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla tworzenia zdarzeń?

   1. Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.

   2. Wybierz **(zakres) synchronizowanie odwołań.**

   3. Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz pozycję **Utwórz odwołanie do firmy Microsoft**.

Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Kompleksowa synchronizacja odwołań dwukierunkowych

Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania do automatyzowania gotowości można testować synchronizację odwołań między programem Salesforce CRM a centrum partnerskim.

### <a name="pre-requisites"></a>Wymagania wstępne

Aby zsynchronizować odwołania w centrum partnerskim i programie Salesforce CRM, rozwiązanie do automatyzowania oprogramowania musi wyraźnie oddzielić pola referencyjne specyficzne dla firmy Microsoft. Ta identyfikacja zapewnia zespołom sprzedawcy możliwość decydowania, które odwołania chcą udostępnić firmie Microsoft w celu współsprzedaży.

Zestaw pól niestandardowych jest dostępny w ramach synchronizacji odwołań Centrum partnerskiego dla jednostki **szansy sprzedaży** rozwiązania w usłudze Salesforce CRM. Użytkownik będący administratorem programu CRM musi utworzyć osobną sekcję CRM z polami niestandardowymi **szansy sprzedaży** .

Następujące pola niestandardowe powinny być częścią sekcji CRM:

- **Synchronizuj z centrum partnerskim**: czy synchronizować szansę sprzedaży z Centrum partnerskiego firmy Microsoft

- **Identyfikator odwołania**: pole identyfikatora tylko do odczytu dla odwołania do Centrum partnerskiego firmy Microsoft

- **Link do odwołania**: link tylko do odczytu do odwołania w centrum partnerskim firmy Microsoft

- **Jak może pomóc firma Microsoft**: pomoc wymagana przez firmę Microsoft do odwołania

- **Produkty**: Lista produktów skojarzonych z tą szansą sprzedaży

- **Inspekcja**: dziennik inspekcji tylko do odczytu na potrzeby synchronizacji z odwołaniami do Centrum partnerskiego

### <a name="scenarios"></a>SYTUACJI

1. Synchronizacja odwołań podczas tworzenia lub aktualizowania odwołania w programie CRM oraz synchronizowanie w centrum partnerskim:

   1. Zaloguj się do środowiska usługi Salesforce CRM przy użyciu użytkownika, który ma widoczność w sekcji **szansa sprzedaży** w programie CRM.

   2. Upewnij się, że Poniższa sekcja jest obecna podczas tworzenia nowej szansy sprzedaży w środowisku programu Salesforce CRM

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Środowisko Salesforce":::

   3. Aby zsynchronizować tę szansę sprzedaży z centrum partnerskim firmy Microsoft, upewnij się, że ustawisz następujące pola w widoku karty:

       - "Synchronizuj z centrum partnerskim": tak
       - "Jak mogę pomóc firmie Microsoft?": Wybierz jedną z następujących opcji:
       - Produkty: identyfikatory rozwiązań produktu

   4. Po ustawieniu opcji  **Synchronizuj z centrum partnerskim** na **wartość tak**, odczekaj 10 minut, zaloguj się na swoim koncie Centrum partnerskiego. Twoje odwołania zostaną zsynchronizowane z programem Salesforce CRM.

   5. Jeśli opcja "Synchronizuj z centrum partnerskim" jest ustawiona na wartość "tak", po zaktualizowaniu szansy sprzedaży w programie Salesforce CRM zmiany zostaną zsynchronizowane z kontem Centrum partnerskiego.

   6. Pomyślnie zsynchronizowane szanse sprzedaży z Centrum partnerskiego zostaną oznaczone ikoną ✔ w programie Salesforce CRM.

2. Synchronizacja odwołań po utworzeniu lub zaktualizowaniu odwołania w centrum partnerskim firmy Microsoft i zsynchronizowaniu w środowisku usługi Salesforce CRM:

    1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.

    2. Wybierz **odwołania** z menu po lewej stronie.

    3. Utwórz nowe odwołanie towarzyszące w centrum partnerskim, klikając pozycję "Nowa transakcja".

    4. Zaloguj się do środowiska usługi Salesforce CRM.

    5. Przejdź do **okna Otwórz szanse sprzedaży**. Odwołanie utworzone w Centrum partnerskiego firmy Microsoft jest teraz synchronizowane w programie Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Ekran możliwości usługi Salesforce":::

    6. Po wybraniu synchronizowanego odwołania są wypełniane szczegóły widoku karty.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)

- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)

- [Elementy webhook Centrum partnerskiego](/partner-center/develop/partner-center-webhooks)
