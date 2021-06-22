---
title: Łącznik do współpracy sprzedaży dla usługi Dynamics 365 CRM Partner Center
description: Synchronizuj polecenia w Partner Center za pomocą łącznika do współpracy sprzedaży dla usługi Dynamics 365 CRM. Następnie możesz sprzedawać z firmą Microsoft z poziomu systemu CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: e656f728789bf5b13dd09732b0b2f5ef30de760a
ms.sourcegitcommit: b7203f1393c3d8f8db4683acdebd09a89e086c3c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/21/2021
ms.locfileid: "112425083"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Łącznik do współs sprzedaży dla usługi Dynamics 365 CRM — omówienie

**Odpowiednie role:** Administrator poleceń | Administrator systemu lub customizer systemu w systemie CRM

Partner Center łączniki do współpracy sprzedaży umożliwiają sprzedawcom sprzedawanie z firmą Microsoft z poziomu systemów CRM. Nie trzeba ich szkolić do używania Partner Center do zarządzania transakcjami sprzedaży. Użyj łączników do współpracy sprzedaży, aby utworzyć nowe polecenie współpracy sprzedaży, aby zaangażować sprzedawcę firmy Microsoft, otrzymać polecenia od sprzedawcy firmy Microsoft, zaakceptować lub odrzucić polecenia oraz zmodyfikować dane transakcji, takie jak wartość transakcji i data zamknięcia. Możesz również otrzymywać wszelkie aktualizacje od sprzedawców firmy Microsoft dotyczące tych transakcji sprzedaży. Możesz zarządzać wszystkimi poleceniami w wybranej przez ciebie crm, a nie w Partner Center.

Rozwiązanie jest oparte na Power Automate i używa Partner Center API.

## <a name="prerequisites"></a>Wymagania wstępne

Przed zainstalowaniem rozwiązania upewnij się, że spełniasz następujące wymagania wstępne.

|**Tematy**   |**Szczegóły**   |**Linki**   |
|--------------|--------------------|------|
|Microsoft Partner Network (MPN) ID |Potrzebny jest prawidłowy identyfikator MPN.|[Dołączanie do sieci partnerów](https://partner.microsoft.com/)|
|Gotowość do współs sprzedaży|Twoje rozwiązanie ip/usług musi być gotowe do współpracy.|[Sell with Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Konto Centrum partnerskiego|Identyfikator MPN skojarzony z dzierżawą Partner Center musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współpracy sprzedaży. Przed wdrożeniem łączników sprawdź, czy w portalu usługi Partner Center są dostępne polecenia dotyczące współpracy sprzedaży.|[Zarządzanie kontem](create-user-accounts-and-set-permissions.md)|
|Partner Center ról użytkownika|Pracownik, który zainstaluje łączniki i będzie ich używać, musi być administratorem poleceń.|[Przypisywanie ról i uprawnień użytkowników](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Rola użytkownika CRM to Administrator systemu lub Customizer systemu.|[Przypisywanie ról w u usługi Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate przepływu|Utwórz nowe środowisko produkcyjne z bazą danych do testowania, przemieszczania i produkcji. Jeśli masz istniejące środowisko produkcyjne z bazą danych, możesz użyć go ponownie. Użytkownik, który zamierza zainstalować rozwiązanie łącznika, musi mieć licencję Power Automate dostęp do tego środowiska. Możesz monitorować postęp i uzyskać więcej informacji w Power Automate [przypadku](https://flow.microsoft.com/) niepowodzenia instalacji. Wybierz **pozycję Zobacz historię w** obszarze **Rozwiązania**.|[Tworzenie środowiska lub zarządzanie środowiskiem](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalowanie Partner Center od skierowań dla usługi Dynamics 365 (Power Automate rozwiązania)

1. Przejdź do [Power Automate](https://flow.microsoft.com)i wybierz pozycję **Środowiska** w prawym górnym rogu. Ten krok spowoduje pokazanie dostępnych wystąpień CRM.

1. Wybierz odpowiednie wystąpienie crm z listy rozwijanej w prawym górnym rogu.

1. Wybierz **pozycję Rozwiązania** po lewej stronie.

1. Wybierz link **Otwórz usługę AppSource** w górnym menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Zrzut ekranu przedstawiający otwieranie usługi AppSource.":::

1. Wyszukaj **łączniki poleceń Partner Center dla usługi Dynamics 365** w oknie podręcznym.  

1. Wybierz przycisk **Pobierz teraz,** a następnie wybierz pozycję **Kontynuuj.**

1. Zostanie wyświetlona strona, na której można wybrać środowisko CRM (Dynamics 365), aby zainstalować aplikację. Wyrażanie zgody na warunki i postanowienia.

1. Możesz monitorować postęp, a jeśli instalacja zakończy się niepowodzeniem, możesz uzyskać więcej szczegółów w te Power Automate wybierając pozycję **Zobacz** historię w obszarze **Rozwiązania.**

1. Po zakończeniu instalacji wróć do strony Power Automate [i](https://flow.microsoft.com) wybierz **pozycję Rozwiązania** po lewej stronie. **Partner Center synchronizacji poleceń dla usługi Dynamics 365** jest teraz dostępna na **liście** rozwiązań.

1. Wybierz **Partner Center synchronizację poleceń dla usługi Dynamics 365.** Dostępne są Power Automate przepływów i jednostek.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Zrzut ekranu przedstawiający dostępne crms.":::

## <a name="test-before-you-go-live"></a>Testowanie przed rozpoczęciem transmisji na żywo

Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania Power Automate w środowisku produkcyjnym należy przetestować rozwiązanie w przejściowym wystąpieniu crm. Musisz:

- Zainstaluj Power Automate w wystąpieniu rozwiązania CRM w środowisku przejściowym.
- Skonfiguruj i dostosuj Power Automate w środowisku przejściowym.
- Przetestuj rozwiązanie w przejściowym wystąpieniu crm.
- Po pomyślnym teście zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.

## <a name="configure-the-solution"></a>Konfigurowanie rozwiązania

1. Po zainstalowaniu rozwiązania w wystąpieniu crm wróć do Power Automate [.](https://flow.microsoft.com/)

1. Z **listy rozwijanej** Środowiska w prawym górnym rogu wybierz wystąpienie crm, w którym zainstalowano Power Automate rozwiązanie.

1. Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:

   - Partner Center z poświadczeniami administratora poleceń
   - Zdarzenia Centrum partnerskiego
   - Administrator CRM z przepływami Power Automate w rozwiązaniu

   1. Wybierz **pozycję** Połączenia po lewej stronie, a następnie **wybierz Partner Center polecenia** z listy.

   1. Utwórz połączenie, wybierając **pozycję Utwórz połączenie.**

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Zrzut ekranu przedstawiający tworzenie połączenia.":::

   1. Wyszukaj Partner Center **poleceń (wersja zapoznawcza)** na pasku wyszukiwania w prawym górnym rogu.

   1. Utwórz połączenie dla użytkownika Partner Center z rolą poświadczeń administratora poleceń.

   1. Następnie utwórz połączenie zdarzeń Partner Center dla użytkownika Partner Center przy użyciu poświadczeń administratora poleceń.

   1. Utwórz połączenie dla usługi Common Data Service (bieżące środowisko) dla użytkownika administratora CRM.
     
   1. Po dodaniu wszystkich połączeń w środowisku powinny zostać wyświetlony następujące połączenia.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Zrzut ekranu przedstawiający połączenia.":::

## <a name="edit-the-connections"></a>Edytowanie połączeń

1. Wróć do strony **Rozwiązania** i wybierz pozycję **Rozwiązanie domyślne.** Wybierz **pozycję Odwołanie do połączenia (wersja zapoznawcza),** wybierając pozycję **Wszystkie.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Zrzut ekranu przedstawiający edytowanie połączeń.":::

1. Edytuj poszczególne połączenia pojedynczo, wybierając ikonę wielokropka. Dodaj odpowiednie połączenia.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Zrzut ekranu przedstawiający wymienione połączenia.":::

1. Wróć do strony **Rozwiązania,** wybierz pozycję Partner Center Synchronizacja poleceń dla usługi **Dynamics 365** i włącz przepływ, wybierając ikonę wielokropka obok każdego przepływu w poniższej sekwencji. Jeśli podczas włączanie przepływu wystąpią jakiekolwiek problemy, zobacz [Kroki](connector-dynamics.md#customize-synchronization-steps) dostosowywania i [Kroki rozwiązywania problemów.](connectors-troubleshoot.md)

Włącz przepływy w następującej kolejności:

- Partner Center Webhook Registration (Insider Preview)
- Tworzenie odwołania do współpracy — dynamics 365 do Partner Center (niejawny program testów w wersji zapoznawczej)
- [Dostosowywanie] Tworzenie lub uzyskiwanie szczegółów z przepływu usługi Dynamics 365
- Partner Center do usługi Dynamics 365 — Pomocnik (niejawny program testów w wersji zapoznawczej)
- Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)
- Partner Center do usługi Dynamics 365 (insider preview)
- Dynamics 365 do Partner Center (insider preview)
- Dynamics 365 Opportunity to Partner Center (Insider Preview)
- Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementy webhook

Możesz użyć interfejsów API Partner Center webhook, aby zarejestrować zdarzenia zmiany zasobów. Te zdarzenia zmiany są wysyłane do Twojego adresu URL jako wpisy HTTP.

1. Wybierz **Partner Center do usługi Dynamics 365 (niejawny program testów w wersji zapoznawczej).**

1. Wybierz **ikonę Edytuj,** a następnie wybierz pozycję **Po otrzymaniu żądania HTTP.**

1. Wybierz **ikonę Kopiuj,** aby skopiować podany adres URL żądania HTTP POST.

   :::image type="content" source="images/webhook-video.gif" alt-text="Zrzut ekranu przedstawiający używanie webhook do rejestrowania zmian zasobów.":::

1. Wybierz przepływ **rejestracji Partner Center webhook (insider preview)** Power Automate, a następnie wybierz **pozycję Uruchom.**

1. Upewnij się, że **w okienku** po prawej stronie zostanie otwarte okno Uruchamianie przepływu, a następnie wybierz pozycję **Kontynuuj.**

1. Wprowadź następujące informacje:

   - **Punkt końcowy wyzwalacza HTTP:** ten adres URL został skopiowany z wcześniejszego kroku.
   - **Zdarzenia do zarejestrowania:** wybierz wszystkie dostępne zdarzenia **(utworzone** przez polecenie , **polecenie-zaktualizowane,** **powiązane-utworzone polecenie** i **powiązane-odwołania-zaktualizowane).**
   - **Zastąp istniejące punkty końcowe wyzwalacza, jeśli są obecne?**: Tak. Dla danego zdarzenia webhook można zarejestrować tylko jeden adres URL.

1. Wybierz **pozycję Uruchom przepływ,** a następnie wybierz pozycję **Gotowe.**

Ten webhook może teraz nasłuchiwać, tworzyć i aktualizować zdarzenia.

## <a name="customize-synchronization-steps"></a>Dostosowywanie kroków synchronizacji

Systemy CRM są wysoce dostosowane i można dostosować Power Automate oparte na konfiguracji CRM. Gdy polecenia dotyczące współpracy sprzedaży są synchronizowane między usługą Partner Center i systemem CRM, pola, które są synchronizowane na komputerze Partner Center, są wyświetlane w przewodniku mapowania pól [niestandardowych.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w obszarze [Dostosuj] Tworzenie lub uzyskiwanie szczegółów z przepływu lub zmiennych środowiskowych usługi **Dynamics 365.** Nie aktualizuj żadnych innych przepływów w Power Automate, ponieważ może to mieć wpływ na przyszłe uaktualnienia rozwiązania.

Dostępne są następujące dostosowania:

- **Wyświetl znacznik wyboru** w nazwie szansy sprzedaży: domyślnie obok nazwy szansy sprzedaży będzie wyświetlany znacznik wyboru wskazujący, że synchronizacja między usługami Partner Center i Dynamics 365 CRM odbywa się pomyślnie. Podobnie w przypadku niepowodzenia synchronizacji zostanie wyświetlony znak krzyżowy. Aby uniknąć dodawania znacznika wyboru lub krzyżowego w  nazwie szansy sprzedaży, ustaw bieżącą wartość znacznika wyboru Wyświetl w zmiennej środowiskowej nazwa szansy sprzedaży na nie.
- **Wartość transakcji:** domyślnie wartość transakcji z Partner Center będzie synchronizowana z i z **szacowanej wartości** w systemie CRM. Jeśli w systemie CRM masz inne pole dla wartości transakcji do zsynchronizowania:

  - Zaktualizuj nazwę **pola Wartość** transakcji w zmiennej środowiskowej usługi Dynamics 365 przy użyciu nazwy pola CRM. Upewnij się, że po podaj nazwę pola, a nie jego nazwę wyświetlaną.
  - Edytuj pozycję [Dostosuj] Tworzenie lub uzyskiwanie szczegółów z przepływu **usługi Dynamics 365,** a  następnie przejdź do tematu Tworzenie lub aktualizowanie szansy sprzedaży w systemie CRM i aktualizowanie pól Utwórz nową szansę sprzedaży i Zaktualizuj istniejące akcje szansy sprzedaży, aby przypisać wartość **DealValue** do poprawnego pola w uciece CRM.   Ponadto usuń przypisanie **DealValue** z pola **Szacowany przychód.**

- **Kod kraju konta klienta:** podczas tworzenia nowego polecenia należy podać dwuliterowy kod kraju (ISO 3166). Domyślnie kod kraju będzie synchronizowany z i z pola address1_country **konta** w systemie CRM. Jeśli w systemie CRM masz inne pole, z których ma być synchronizowane kod kraju:

  - W przypadku pola kodu kraju bez funkcjilookup na koncie, które zawiera kod dwuliterowy:
    - Zaktualizuj nazwę **pola Kod kraju konta klienta** w zmiennej środowiskowej usługi Dynamics 365 przy użyciu nazwy pola CRM. Upewnij się, że po podaj nazwę pola, a nie jego nazwę wyświetlaną.
    - Edytuj pozycję [Dostosuj] Create or Get Details from Dynamics 365 flow (Tworzenie lub  uzyskiwanie szczegółów z przepływu **usługi Dynamics 365)** i przejdź do tematu Create or get **customer account** (Tworzenie lub uzyskiwanie konta klienta) w akcji CRM, aby przypisać wartość Country (Kraj) do poprawnego pola w programie CRM. Ponadto usuń przypisanie **wartości** Country (Kraj) z **pola Address 1: Country/Region (Adres 1: kraj/region).**

  - W przypadku pola kodu kraju opartego na odnośniku na koncie:
    - Dodaj nowe pole niestandardowe na koncie i wypełnij je automatycznie dwuliterowym kodem kraju (ISO 3166) na podstawie wartości wybranej w polu wyszukiwania i na odwrót.
    - Wykonaj powyższe kroki dla pola kodu kraju nielookupu, aby zsynchronizować nowe pole niestandardowe z usługi CRM do i z Partner Center.

- **Pola** Szansy sprzedaży: jeśli  w polu Szansa sprzedaży znajdują się obowiązkowe pola, które muszą zostać wypełnione,  edytuj pozycję [Dostosuj]  Utwórz lub pobierz szczegóły z przepływu **usługi Dynamics 365,** a następnie przejdź do tematu Tworzenie lub aktualizowanie szansy sprzedaży w programie CRM i zaktualizuj akcję Utwórz nową szansę sprzedaży, aby przypisać wartości do obowiązkowych pól zgodnie z wymaganiami biznesowymi.
- Pola potencjalnych **klientów:** jeśli  w polu Potencjalny użytkownik istnieją obowiązkowe pola, które muszą zostać wypełnione, edytuj pozycję [Dostosuj] Utwórz  lub pobierz szczegóły z przepływu **usługi Dynamics 365,** a następnie przejdź do tematu Tworzenie lub aktualizowanie potencjalnych klientów w systemie CRM i zaktualizuj akcję Utwórz nowego potencjalnego klienta, aby przypisać wartości do obowiązkowych pól na podstawie wymagań biznesowych. 
- Konto **klienta:** gdy nowe polecenie jest synchronizowane z usługi Partner Center do systemu CRM, rozwiązanie Power Automate próbuje wyszukać istniejące konto w systemie CRM przy użyciu nazwy firmy klienta i kodu pocztowego. Jeśli go nie znajdzie, w systemie CRM zostanie utworzone nowe konto klienta. Aby zaktualizować kryteria wyszukiwania i szczegóły tworzenia nowego konta, edytuj pozycję [Dostosuj] Tworzenie  lub uzyskiwanie szczegółów z przepływu **usługi Dynamics 365,** a następnie przejdź do akcji Utwórz lub pobierz konto klienta w akcjach CRM i Utwórz konto **klienta.**

## <a name="update-environment-variable"></a>Aktualizowanie zmiennej środowiskowej

Aby zaktualizować wartość zmiennej środowiskowej:

1. Przejdź do strony **Rozwiązania** i wybierz pozycję **Rozwiązanie domyślne.** Wybierz **pozycję Zmienna środowiskowa,** wybierając **pozycję Wszystkie.**

1. Wybierz zmienną środowiskową dla wartości, która ma zostać zaktualizowana, a następnie wybierz pozycję **Edytuj** za pomocą ikony wielokropka.

1. Zaktualizuj **wartość bieżącą** (nie aktualizuj wartości **domyślnej**) przy użyciu opcji **Nowa** wartość i podając wartość. Wartość musi być dopasowana do typu danych zmiennej. Na przykład typ danych Tak lub Nie będzie akceptował wartości Tak lub Nie.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Zrzut ekranu przedstawiający aktualizowanie zmiennych środowiskowych.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>End-to-end bidirectional co-sell referral synchronization (End-to-end bidirectional co-sell referral synchronization)

Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania Power Automate można przetestować synchronizację poleceń do współpracy sprzedaży między usługami Dynamics 365 i Partner Center.

### <a name="prerequisites"></a>Wymagania wstępne

Aby zsynchronizować polecenia w usługach Partner Center i Dynamics 365 CRM, rozwiązanie Power Automate wyraźnie demarcates pola poleceń specyficzne dla firmy Microsoft. Ta identyfikacja daje zespołom sprzedawców możliwość decydowania o tym, które polecenia chcą udostępnić firmie Microsoft w celu współpracy sprzedaży.

Zestaw niestandardowych pól i obiektów zostanie dodany w ramach instalacji rozwiązania. Administrator crm musi utworzyć oddzielną sekcję CRM z **niestandardowymi** polami Szansa sprzedaży.

Następujące pola niestandardowe powinny być częścią sekcji CRM:

- **Synchronizacja z Partner Center:** czy zsynchronizować możliwość sprzedaży z Partner Center. Domyślnie wartość tego pola to Nie i musi być jawnie ustawiona na wartość Tak przez sprzedawcę, aby udostępnić szansę sprzedaży firmie Microsoft. Nowe polecenia udostępniane z Partner Center crm będą mieć tę wartość pola ustawioną na Tak.
- **Identyfikator odwołania:** pole identyfikatora tylko do odczytu dla Partner Center polecenia.
- **Link polecenia:** link tylko do odczytu do polecenia w Partner Center.
- **Jak firma Microsoft może pomóc?**: Wymagana przez firmę Microsoft pomoc w przypadku odwołania. Aby utworzyć polecenie współpracy sprzedaży, wybierz odpowiednią pomoc wymaganą od firmy Microsoft. Osoba kontaktowa z klientem musi być skojarzona z szansą utworzenia polecenia do współpracy sprzedaży. Aby utworzyć polecenie inne niż współsieć, nie zaznaczaj tego pola. Polecenie braku współpracy sprzedaży można przekonwertować na polecenie do współpracy sprzedaży w dowolnym momencie, wybierając odpowiednią opcję wymaganą przez pomoc.
- **Microsoft Partner Center Widoczność poleceń:** wybierz widoczność Partner Center polecenia. Dzięki temu, że jest ono widoczne dla sprzedawców firmy Microsoft, polecenie inne niż sprzedaż może zostać przekonwertowane na współspojęcie. Jeśli wymagana jest pomoc firmy Microsoft, polecenie jest domyślnie widoczne dla sprzedawców firmy Microsoft. Po oznaczeniu tego pola jako widocznego nie można go przywrócić.
- **Identyfikator microsoft CRM:** po utworzeniu i zaakceptowaniu polecenia współpracy sprzedaży przez firmę Microsoft to pole zostanie wypełnione identyfikatorem CRM firmy Microsoft.
- **Produkty: Przestarzałe:** nie używaj tego pola ani nie dodawaj go do sekcji CRM. Jest ona dostępna tylko w celu zapewnienia zgodności z poprzednimi wersjami. Zamiast tego Partner Center rozwiązań.
- **Inspekcja:** dziennik inspekcji tylko do odczytu do synchronizacji z Partner Center poleceniami.
- **Microsoft Partner Center Solutions:** niestandardowy obiekt kojarzący gotowe do współpracy rozwiązania lub rozwiązania firmy Microsoft z szansą sprzedaży. Co najmniej jedno rozwiązanie można dodać lub usunąć z szansy sprzedaży. Przed udostępnieniem go firmie Microsoft należy dodać do szansy sprzedaży co najmniej jedno gotowe do sprzedaży lub rozwiązanie firmy Microsoft. Aby skojarzyć ten obiekt z szansą sprzedaży, zaktualizuj formularz **Szansa** sprzedaży w systemie CRM.

  Wybierz odpowiednią kartę w **formularzu Szansa** sprzedaży i dodaj podsiatę, jak pokazano poniżej.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Zrzut ekranu przedstawiający formularz Szansa sprzedaży.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Zrzut ekranu przedstawiający rozwiązania firmy Microsoft.":::

- Po dodaniu rozwiązań firmy Microsoft możesz wstępnie zasypować szczegóły gotowego rozwiązania do współsprzedaży, aby sprzedawcy nie mieli ich dodawać. Aby dodać nowe szczegóły rozwiązania, przejdź do obiektu Szczegóły  rozwiązania firmy Microsoft w systemie CRM i wybierz pozycję Dodaj rekord, aby dodać jeden wpis, lub użyj funkcji przekazywania programu **Excel,** aby dodać wiele wpisów.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Zrzut ekranu przedstawiający szczegóły nowego rozwiązania firmy Microsoft.":::

### <a name="scenarios"></a>Scenariusze

1. Synchronizacja poleceń, gdy polecenie jest tworzone lub aktualizowane w systemie CRM i synchronizowane w Partner Center:

   1. Zaloguj się do środowiska CRM usługi Dynamics 365 przy użyciu użytkownika, który ma wgląd w sekcję **Opportunity** (Szansa sprzedaży) w chmurze CRM.

   1. Upewnij **się, że Partner Center** Microsoft jest obecna podczas tworzenia nowej szansy sprzedaży w środowisku usługi Dynamics 365.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Zrzut ekranu przedstawiający nową szansę sprzedaży.":::

   1. Aby zsynchronizować tę możliwość z Partner Center, należy ustawić następujące pola w widoku karty:

      - **Jak firma Microsoft może pomóc?**: Aby utworzyć polecenie do współpracy sprzedaży, wybierz odpowiednią opcję pomocy.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Zrzut ekranu przedstawiający sposób uzyskania odpowiednich pól w widoku karty.":::

      - **Kontakt z** klientem: aby utworzyć polecenie współpracy sprzedaży, dodaj kontakt klienta do szansy sprzedaży.
      - **Synchronizuj z Partner Center:** Tak.
      - **Rozwiązania firmy Microsoft:** Aby udostępnić polecenie firmie Microsoft, dodaj do szansy sprzedaży prawidłowe rozwiązanie gotowe do sprzedaży lub rozwiązanie firmy Microsoft.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Zrzut ekranu przedstawiający identyfikator rozwiązania.":::

   1. Po utworzeniu szansy sprzedaży w uchu Dynamics 365 z opcją **Synchronizuj** z Partner Center ustawioną na wartość Tak zaczekaj 10 minut. Następnie zaloguj się do swojego Partner Center konta. Twoje polecenia zostaną zsynchronizowane z programem Dynamics 365 i **identyfikatorem poleceń**. **Link do** polecenia zostanie wypełniony. Jeśli wystąpi błąd, pole **Inspekcja** zostanie wypełnione informacjami o błędzie.

      1. Podobnie w przypadku szansy sprzedaży, dla których opcja Synchronizuj z usługą **Partner Center** została ustawiona na wartość Tak, w przypadku zaktualizowania szansy sprzedaży w programie Dynamics 365 CRM zmiany zostaną zsynchronizowane na Partner Center klienta.

      1. Szanse sprzedaży pomyślnie zsynchronizowane z Partner Center zostaną zidentyfikowane za pomocą ✔icon w u usługi Dynamics 365.

1. Synchronizacja od skierowań, gdy polecenie jest tworzone lub aktualizowane Partner Center i synchronizowane w środowisku usługi Dynamics 365:

   1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)

   1. Wybierz **pozycję Polecenia** z menu po lewej stronie.

   1. Utwórz nowe polecenie współpracy sprzedaży z Partner Center, wybierając **opcję Nowa transakcja.**

   1. Zaloguj się do środowiska CRM usługi Dynamics 365.

   1. Przejdź do okna **Otwieranie szans sprzedaży.** Polecenia utworzone w Partner Center są teraz synchronizowane w uchu Dynamics 365 CRM.

   1. Po wybraniu zsynchronizowanego polecenia zostaną wypełnione szczegóły widoku karty.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)
- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)
- [Więcej informacji na temat platformy Power Automate Microsoft](/power-automate/)
- [Elementy webhook Centrum partnerskiego](/partner-center/develop/partner-center-webhooks)
