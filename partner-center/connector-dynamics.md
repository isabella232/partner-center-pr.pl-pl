---
title: Łącznik współsprzedającego dla Centrum partnerskiego programu Dynamics 365 CRM
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj swoje odwołania w centrum partnerskim z łącznikiem do współsprzedażu dla programu Dynamics 365 CRM. Sprzedawcy mogą następnie współsprzedawać z firmą Microsoft w ramach systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947776"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Łącznik współsprzedawanych produktów Dynamics 365 CRM — Omówienie

### <a name="appropriate-roles"></a>Odpowiednie role

- Administrator odwołań
- Administrator systemu lub Konfigurator systemu w programie CRM

Łącznik współpracujący z centrum partnerskim umożliwia sprzedającym współsprzedaż z firmą Microsoft w ramach systemów CRM. Nie trzeba ich przeszkoleć w celu zarządzania pozostałymi ofertami przy użyciu Centrum partnerskiego. Użyj łączników współsprzedania, aby utworzyć nowe odwołanie do współsprzedaży, aby skontaktować się z sprzedawcą firmy Microsoft, otrzymywać odwołania od sprzedawcy firmy Microsoft, akceptować/odrzucać odwołania, modyfikować dane dotyczące transakcji, takie jak wartość transakcji i Data zamknięcia. Możesz również otrzymywać wszelkie aktualizacje od sprzedawcy firmy Microsoft w ramach tych transakcji związanych z współsprzedażą. Wszystkie odwołania można wykonać w wybranym przez siebie programie CRM, a nie w centrum partnerskim. 

Rozwiązanie jest oparte na rozwiązaniu Microsoft energooszczędne i korzysta z interfejsów API Centrum partnerskiego.

## <a name="before-you-install---pre-requisites"></a>Przed zainstalowaniem — wymagania wstępne

|**Tematy**   |**Szczegóły**   |**Linki**   |
|--------------|--------------------|------|
|Identyfikator Microsoft Partner Network |Potrzebujesz prawidłowego identyfikatora MPN|Aby dołączyć [MPN](https://partner.microsoft.com/)|
|Gotowe do rozsprzedaj|Twoje rozwiązanie do adresów IP/usług musi być gotowe do współpracy.|[Sprzedawanie z firmą Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Konto Centrum partnerskiego|IDENTYFIKATOR MPN skojarzony z dzierżawcą Centrum partnerskiego musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współsprzedażu. Przed wdrożeniem łączników Sprawdź, czy w portalu Centrum partnerskiego są widoczne swoje odwołania do współsprzedawcy.|[Zarządzanie kontem](create-user-accounts-and-set-permissions.md)|
|Role użytkowników Centrum partnerskiego|Pracownik, który zainstaluje łączniki i korzysta z nich, musi być administratorem odwołań|[Przypisywanie ról i uprawnień użytkowników](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|Rola użytkownika programu CRM to administrator systemu lub Konfigurator systemu|[Przypisywanie ról w usłudze Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Konto przepływu automatyzacji|Aktywne konto usługi [Automatyzowanie](https://flow.microsoft.com) dla administratora systemu lub konfiguratora systemu programu CRM. Ten użytkownik powinien zalogować się do programu w celu [automatyzacji](https://flow.microsoft.com) co najmniej raz przed instalacją.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Zainstaluj synchronizację odwołań Centrum partnerskiego dla programu Dynamics 365 (rozwiązanie do automatyzowania zarządzania)

1. Przejdź do pozycji [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **środowiska** w prawym górnym rogu. W tym kroku przedstawiono dostępne wystąpienia programu CRM.

2. Wybierz odpowiednie wystąpienie programu CRM z listy rozwijanej w prawym górnym rogu.

3. Wybierz pozycję **rozwiązania** na lewym pasku nawigacyjnym.

4. Kliknij link **Otwórz AppSource** w górnym menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz AppSource":::

5. Wyszukaj **Łączniki dla usługi Partner Center dla Dynamics365** na ekranie podręcznym.  

6. Kliknij przycisk **Pobierz teraz** , a następnie **Kontynuuj**.

7. Spowoduje to otwarcie strony, na której można wybrać środowisko CRM (Dynamics 365), aby zainstalować aplikację.  Zgadzam się na warunki i postanowienia.

8. Następnie nastąpi przekierowanie do strony **zarządzanie rozwiązaniami** .  Przejdź do pozycji "referencje do Centrum partnerskiego" przy użyciu przycisków strzałek u dołu strony. **Zaplanowana instalacja** powinna pojawić się obok rozwiązania do tworzenia odwołań do Centrum partnerskiego. Instalacja zajmie 10-15 minut. 

9. Po zakończeniu instalacji przejdź z powrotem do strony [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **rozwiązania** z lewego obszaru nawigacji. Zwróć uwagę na to, że w ramach listy rozwiązań jest dostępny komunikat **dotyczący usługi Partner Center dotyczącej synchronizacji dla usługi Dynamics 365** .

10. Wybierz pozycję **Centrum partnerskie — synchronizacja dla programu Dynamics 365**. Dostępne są następujące przepływy automatyzacji i jednostki:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Dostępne CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>Najlepsze rozwiązanie: testowanie przed rzeczywistym użyciem

Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania do automatyzowania w środowisku produkcyjnym należy przetestować rozwiązanie w tymczasowym wystąpieniu programu CRM.

- Zainstaluj rozwiązanie Microsoft PowerShell automatyzuje w wystąpieniu środowiska przejściowego/programu CRM.
- Utwórz kopię rozwiązania i przeprowadź konfigurację i uruchom dostosowania przepływu w środowisku przejściowym.
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

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Tworzenie połączenia":::

      3. Wyszukaj **Referencje Centrum partnerskiego (wersja zapoznawcza)** na pasku wyszukiwania w prawym górnym rogu.

      4. Utwórz połączenie dla użytkownika Centrum partnerskiego z rolą poświadczeń administratora.

      5. Następnie utwórz połączenie zdarzeń Centrum partnerskiego dla użytkownika Centrum partnerskiego z poświadczeniami administratora odwołań.

      6. Utwórz połączenie dla Common Data Service (bieżące środowisko) dla użytkownika Administrator programu CRM.
       
     
      7. Po dodaniu wszystkich połączeń powinny zostać wyświetlone następujące połączenia w danym środowisku:

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Połączenia":::
   
## <a name="edit-the-connections"></a>Edytuj połączenia

1. Wróć do strony **rozwiązania** i wybierz pozycję **domyślne rozwiązanie**. Wybierz pozycję **odwołanie do połączenia (wersja zapoznawcza)** , klikając pozycję **wszystkie**.

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Połącz":::

2. Edytuj poszczególne połączenia po jednym, wybierając ikonę z trzema kropkami. Dodaj odpowiednie połączenia.

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Wymienione połączenia"::: 

3.  Włącz przepływy w następującej kolejności:
- Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Utwórz odwołanie do współsprzedawcy — Dynamics 365 do Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Centrum partnerskie — aktualizacje odwołań do oprogramowania Dynamics 365 (wersja zapoznawcza programu Preview)
- Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu Preview)
- Dynamics 365 do Centrum partnerskiego (wersja zapoznawcza)
- Dynamics 365 — szansa do Centrum partnerskiego (wersja zapoznawcza)
- Dynamics 365 — rozwiązania firmy Microsoft do Centrum partnerskiego (wersja zapoznawcza)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementu webhook

Interfejsy API elementu webhook Centrum partnerskiego umożliwiają rejestrację zdarzeń zmiany zasobów. Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.

1. Aby zarejestrować adres URL, wybierz pozycję **rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza)** .

2. Dodaj połączenia dla (a) użytkownika Centrum partnerskiego z poświadczeniami administratora (b.) Centrum partnerskiego, jak zostało to wyróżnione poniżej

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz":::

3. Po wprowadzeniu tych aktualizacji zobaczysz

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Elementy webhook":::

4. Zapisz zmiany i wybierz pozycję **Włącz**.

   Aby włączyć elementy webhook Centrum partnerskiego do nasłuchiwania zmian w zdarzeniach, wykonaj następujące czynności:

5. Wybierz pozycję **Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu testowego)**.

6. Wybierz ikonę **Edytuj** i wybierz, **kiedy zostanie odebrane żądanie HTTP**.

7. Wybierz ikonę **kopiowania** , aby skopiować podany adres URL post protokołu HTTP.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopiowanie adresu URL":::

8. Teraz wybierz pozycję "Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)", a następnie wybierz pozycję **Uruchom**.

9. Upewnij się, że okno "przebieg przepływu" otwiera się w okienku po prawej stronie, a następnie kliknij przycisk **Kontynuuj**.

10. Wprowadź następujące wartości:

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

    a. Wybierz pozycję Centrum partnerskie do usługi Dynamics 365 (wersja zapoznawcza programu testowego) lub Centrum partnerskiego w usłudze Salesforce (wersja zapoznawcza programu testowego).

    b. Wybierz pozycję **Edytuj** , aby edytować/dostosować przepływ automatyzacji.

    c. Wybierz **(zakres) zsynchronizuj potencjalnego klienta lub szansę sprzedaży**.

2. Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz opcję **Jeśli jest to nowa udostępniona okazja, a następnie**. Wybierz podkrok, **Jeśli tak** , a następnie rozwiń pozycję **Tworzenie nowej szansy sprzedaży w programie CRM**. Mapowania w tej sekcji można edytować za pomocą przewodnika mapowania pól.

    d. Aby dostosować mapowania pól programu CRM (na podstawie przewodnika po mapowaniach pól) dla zdarzeń aktualizacji, kliknij krok "(zakres) zsynchronizuj lidera lub szansę sprzedaży".

    e. Wybierz **, czy jest to aktualizacja szansy sprzedaży, a następnie**. Wybierz podkrok, **Jeśli tak** , a następnie rozwiń **, jeśli różnica między obiektami szansy sprzedaży w centrum partnerskim i CRM**.  

    f. Wybierz opcję **tak** , po której następuje **Aktualizacja istniejącej szansy sprzedaży**

3. Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla zdarzeń aktualizacji:

    a. Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.

    b. Wybierz **(zakres) zsynchronizuj szansę sprzedaży**.

    c. Aby dostosować mapowania pól programu CRM dla zdarzeń aktualizacji, należy wybrać, **czy istnieje różnica między obiektami lidera w centrum partnerskim i CRM, a następnie**. 

    d. Wybierz krok podrzędny, **Jeśli tak** , a następnie rozwiń krok **Aktualizuj odwołanie z danymi o szansie sprzedaży**.

   Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.

4. Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla tworzenia zdarzeń?

   a. Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.

   b. Wybierz **(zakres) synchronizowanie odwołań.**

   c. Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz pozycję **Utwórz odwołanie do firmy Microsoft**.

   Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.

Istnieją dwie zmienne środowiskowe, które zostały utworzone:

- Znacznik wyboru: oznacza, czy potrzebna jest ikona znacznika wyboru poza szansami, które są synchronizowane dwukierunkowo między centrum partnerskim i Dynamics 365 CRM.

- Synchronizuj tylko okazje do sprzedaży: oznacza to, czy chcesz synchronizować tylko okazje do sprzedaży.

Można edytować wartość domyślną zmiennych środowiskowych.

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Pole edycji dla wartości domyślnych":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Kompleksowa synchronizacja odwołań dwukierunkowych

Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania do automatyzowania gotowości można testować synchronizację odwołań między programem Dynamics 365 i centrum partnerskim.

### <a name="pre-requisites"></a>Wymagania wstępne

Aby synchronizować odwołania w centrum partnerskim i Dynamics 365 CRM, rozwiązanie do automatyzowania, które wyraźnie określa pola odwołań specyficzne dla firmy Microsoft. Dzięki tej identyfikacji sprzedawca może określić, które odwołania mają być udostępniane firmie Microsoft w celu współsprzedaży.

Zestaw pól niestandardowych jest dostępny w ramach jednostki **szansy sprzedaży** . Użytkownik będący administratorem programu CRM musi utworzyć osobną sekcję CRM z polami niestandardowymi **szansy sprzedaży** .

Następujące pola niestandardowe powinny być częścią sekcji CRM:

- **Synchronizuj z centrum partnerskim**: czy synchronizować szansę sprzedaży z Centrum partnerskiego firmy Microsoft

- **Identyfikator odwołania**: pole identyfikatora tylko do odczytu dla odwołania do Centrum partnerskiego firmy Microsoft

- **Link do odwołania**: link tylko do odczytu do odwołania w centrum partnerskim firmy Microsoft

- **Jak może pomóc firma Microsoft?**: pomoc wymagana przez firmę Microsoft do odwołania

- **Produkty**: Lista produktów skojarzonych z tą szansą sprzedaży

- **Inspekcja**: dziennik inspekcji tylko do odczytu na potrzeby synchronizacji z odwołaniami do Centrum partnerskiego

Aktualizowanie formularza szansa sprzedaży w programie Dynamics 365 CRM w celu uwzględnienia rozwiązań dla produktów.

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formularz szansy sprzedaży":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a>SYTUACJI

1. Synchronizacja odwołań podczas tworzenia lub aktualizowania odwołania w programie CRM oraz synchronizowanie w centrum partnerskim:

   1. Zaloguj się do środowiska Dynamics 365 CRM przy użyciu użytkownika, który ma wgląd w sekcję **szansa sprzedaży** w programie CRM.

   2. Upewnij się, że Poniższa sekcja jest obecna podczas tworzenia "nowej szansy" w środowisku Dynamics 365

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Sekcja Przykładowa okazja przedstawiająca informacje Centrum partnerskiego firmy Microsoft w usłudze Dynamics 365.":::

   3. Aby zsynchronizować tę szansę sprzedaży z centrum partnerskim firmy Microsoft, upewnij się, że ustawisz następujące pola w widoku karty:

      - **Synchronizuj z centrum partnerskim**: tak

      - **Jak może pomóc firma Microsoft?**: Wybierz jedną z następujących opcji:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sekcja przykładowej szansy sprzedaży w usłudze Dynamics 365, która zawiera opcje pomocy Centrum partnerskiego firmy Microsoft obok pola o nazwie jak może pomóc firma Microsoft?":::

      - **Produkty**: identyfikatory rozwiązań produktu

   4. Po utworzeniu szansy sprzedaży w usłudze Dynamics 365 z opcją **Synchronizuj z centrum partnerskim** ustawionym na **wartość tak**, odczekaj 10 minut, a następnie zaloguj się do konta Centrum partnerskiego. Twoje odwołania zostaną zsynchronizowane z usługą Dynamics 365.

   5. Podobnie w przypadku opcji "Synchronizuj z centrum partnerskim" o wartości "tak" w przypadku zaktualizowania szansy sprzedaży w programie Dynamics 365 CRM zmiany zostaną zsynchronizowane na koncie Centrum partnerskiego.

   6. Prospekty, które zostały pomyślnie zsynchronizowane z centrum partnerskim, zostaną zidentyfikowane przy użyciu ikony ✔ w usłudze Dynamics 365.

2. Synchronizacja odwołań po utworzeniu lub zaktualizowaniu odwołania w centrum partnerskim firmy Microsoft i zsynchronizowaniu w środowisku Dynamics 365:

   1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.

   2. Wybierz **odwołania** z menu po lewej stronie.

   3. Utwórz nowe odwołanie towarzyszące w centrum partnerskim, klikając pozycję "Nowa transakcja".

   4. Zaloguj się do środowiska programu Dynamics 365 CRM.

   5. Przejdź do **okna Otwórz szanse sprzedaży**. Odwołanie utworzone w Centrum partnerskiego firmy Microsoft jest teraz synchronizowane w programie Dynamics 365 CRM.

   6. Po wybraniu synchronizowanego odwołania są wypełniane szczegóły widoku karty.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)

- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)

- [Więcej informacji na temat platformy Microsoft energooszczędnej?](/power-automate/)

- [Elementy webhook Centrum partnerskiego](/partner-center/develop/partner-center-webhooks)