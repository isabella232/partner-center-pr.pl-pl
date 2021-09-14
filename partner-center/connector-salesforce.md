---
title: Łącznik do współsprzedaży dla usługi Salesforce CRM Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Zsynchronizuj polecenia w Partner Center z crm usługi Salesforce. Sprzedawcy mogą następnie sprzedawać z firmą Microsoft z poziomu systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 4a98bd2e98aa1533806205179812af6507b2a2af
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246958"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Łącznik do współsprzedaży dla rozwiązania Salesforce CRM — omówienie

**Odpowiednie role:** Administrator poleceń | Administrator systemu lub customizer systemu w systemie CRM

Partner Center łącznika do współpracy sprzedaży umożliwia sprzedawcom sprzedawanie z firmą Microsoft z poziomu systemów CRM. Nie trzeba ich szkolić do używania Partner Center do zarządzania transakcjami sprzedaży. Za pomocą łączników do współpracy sprzedaży możesz utworzyć nowe polecenie współpracy sprzedaży, aby zaangażować sprzedawcę firmy Microsoft, otrzymać polecenia od sprzedawcy firmy Microsoft, zaakceptować/odrzucić polecenia, zmodyfikować dane transakcji, takie jak wartość transakcji i data zamknięcia.  Możesz również otrzymywać wszelkie aktualizacje od sprzedawców firmy Microsoft dotyczące tych transakcji sprzedaży. Wszystkie polecenia można wykonać podczas pracy w ramach wybranego rozwiązania CRM, a nie w Partner Center.

Rozwiązanie jest oparte na rozwiązaniu Microsoft Power Automate i używa Partner Center API.

## <a name="before-you-install---pre-requisites"></a>Przed zainstalowaniem — wymagania wstępne

|**Tematy**|**Szczegóły**|**Linki**|
|--------------|--------------------|------|
|Microsoft Partner Network identyfikator |Potrzebny jest prawidłowy identyfikator MPN|Aby dołączyć [do programu MPN](https://partner.microsoft.com/)|
|Gotowość do współs sprzedaży|Twoje rozwiązanie ip/usług musi być gotowe do współpracy.|[Sell with Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Konto Centrum partnerskiego|Identyfikator MPN skojarzony z dzierżawą Partner Center musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współs sprzedaży. Przed wdrożeniem łączników sprawdź, czy polecenia dotyczące współpracy sprzedaży są Partner Center portalu.|[Zarządzanie kontem](create-user-accounts-and-set-permissions.md)|
|Partner Center ról użytkownika|Pracownik, który zainstaluje łączniki i użyje ich, musi być administratorem poleceń|[Przypisywanie ról i uprawnień użytkowników](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Rola użytkownika CRM to Administrator systemu lub Customizer systemu|[Przypisywanie ról w programie Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow konto|Utwórz nowe środowisko produkcyjne z bazą danych do testowania, przemieszczania i produkcji. Jeśli masz istniejące środowisko produkcyjne z bazą danych, możesz użyć go ponownie. Użytkownik, który zamierza zainstalować rozwiązanie łącznika, musi mieć licencję Power Automate dostęp do tego środowiska. Możesz monitorować postęp i uzyskać więcej informacji w Power Automate [przypadku](https://flow.microsoft.com/) niepowodzenia instalacji. Wybierz **pozycję Zobacz historię w** obszarze **Rozwiązania**.|[Tworzenie środowiska lub zarządzanie środowiskiem](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalacja pakietu Salesforce dla pól niestandardowych firmy Microsoft

Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, rozwiązanie Power Automate musi jasno identyfikować pola poleceń specyficzne dla firmy Microsoft. To oznaczanie daje zespołom sprzedawców partnerskich możliwość decydowania o tym, które skierowania chcą udostępnić firmie Microsoft w celu współpracy sprzedaży.

1. W u usługi Salesforce aktywuj pozycję **Notatki** i dodaj ją do listy powiązanych szans sprzedaży. [Odwołanie](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. **Aktywuj zespoły szans** sprzedaży, wykonać następujące czynności:
    - W oknie Instalatora użyj **pola Szybkie wyszukiwanie,** aby zlokalizować Ustawienia.
    - Zdefiniuj ustawienia zgodnie z potrzebami. [Odwołanie](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. W uakiecie Salesforce zainstaluj niestandardowe pola i obiekty przy użyciu [instalatora pakietu](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Użyj tego instalatora, aby zainstalować pakiet w dowolnej firmie.

    >[!NOTE]
    >Jeśli instalujesz w piaskownicy, musisz zastąpić początkową część adresu URL `http://test.salesforce.com` .

1. W u usługi Salesforce dodaj rozwiązania firmy Microsoft do listy Opportunity related **(Powiązane z szansą** sprzedaży). Po dodaniu wybierz **ikonę klucza** i zaktualizuj właściwości

## <a name="best-practice-test-before-you-go-live"></a>Najlepsze rozwiązanie: Testowanie przed rozpoczęciem transmisji na żywo

Przed zainstalowaniem, skonfigurowaniem i dostosowaniem Power Automate w środowisku produkcyjnym należy przetestować rozwiązanie w przejściowym wystąpieniu crm.

- Zainstaluj rozwiązanie Microsoft Power Automate w środowisku przejściowym/wystąpieniu crm.

- Zrób kopię rozwiązania, a następnie uruchom konfigurację i Power Automate dostosowywania przepływu w środowisku przejściowym.

- Przetestuj rozwiązanie w wystąpieniu przejściowym/CRM.

- W przypadku powodzenia zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalowanie Partner Center poleceń usługi Salesforce CRM

1. Przejdź do [Power Automate](https://flow.microsoft.com) i wybierz **pozycję Środowiska** w prawym górnym rogu. Spowoduje to pokazanie dostępnych wystąpień CRM.

1. Wybierz odpowiednie wystąpienie crm z listy rozwijanej w prawym górnym rogu.

1. Wybierz **pozycję Rozwiązania** na pasku nawigacyjnym po lewej stronie.

1. Wybierz link **Otwórz usługę AppSource** w górnym menu.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Otwórz usługę AppSource.":::

1. Wyszukaj **łączniki poleceń Partner Center dla usługi Salesforce** w oknie podręcznym.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Zrzut ekranu przedstawiający ekran Pobierz teraz.":::

1. Wybierz przycisk **Pobierz teraz,** a następnie wybierz pozycję **Kontynuuj.**

1. Na następnej stronie wybierz środowisko CRM usługi Salesforce, aby zainstalować aplikację. Wyrażanie zgody na warunki i postanowienia.

1. Następnie zostaniesz skierowany do strony **Zarządzanie rozwiązaniami.**  Przejdź do Partner Center Polecenia" przy użyciu przycisków strzałek w dolnej części strony. **Instalacja zaplanowana** powinna być wyświetlana obok Partner Center polecenia. Instalacja potrwa 10–15 minut.

1. Po zakończeniu instalacji wróć do strony Power Automate [i](https://flow.microsoft.com) wybierz **pozycję Rozwiązania** w obszarze nawigacji po lewej stronie. Zwróć **uwagę, Partner Center synchronizacja poleceń dla usługi Salesforce** jest teraz dostępna na liście rozwiązania.

1. Wybierz **Partner Center polecenia dla usługi Salesforce.** Dostępne są Power Automate przepływów i jednostek:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Przepływy usługi Salesforce.":::

## <a name="configure-the-solution"></a>Konfigurowanie rozwiązania

1. Po zainstalowaniu rozwiązania w wystąpieniu crm wróć do Power Automate [.](https://flow.microsoft.com/)

1. Z **listy rozwijanej** Środowiska w prawym górnym rogu wybierz wystąpienie crm, w którym zainstalowano Power Automate rozwiązanie.

1. Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:

   - Partner Center z poświadczeniami administratora poleceń
   - Zdarzenia Centrum partnerskiego
   - Administrator CRM z przepływami Power Automate w rozwiązaniu

   1. Wybierz **pozycję Połączenia** na pasku nawigacyjnym po lewej stronie, a następnie wybierz Partner Center **polecenia** z listy.

   1. Utwórz połączenie, wybierając **pozycję Utwórz połączenie.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Zrzut ekranu przedstawiający tworzenie połączenia.":::

   1. Wyszukaj Partner Center **polecenia (wersja zapoznawcza)** na pasku wyszukiwania w prawym górnym rogu.

   1. Utwórz połączenie dla użytkownika Partner Center z rolą poświadczeń administratora poleceń.

   1. Następnie utwórz połączenie Partner Center zdarzeń usługi Partner Center użytkownika przy użyciu poświadczeń administratora poleceń.

   1. Utwórz połączenie dla usługi Salesforce dla użytkownika administratora CRM.
  
   1. Utwórz połączenie dla usługi Microsoft Dataverse dla użytkownika administratora CRM.

   1. Po dodaniu wszystkich połączeń w środowisku powinny zostać wyświetlonych następujące połączenia:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Zrzut ekranu przedstawiający sposób obserwowania połączeń.":::

### <a name="edit-the-connections"></a>Edytowanie połączeń

1. Wróć do strony **Rozwiązania** i wybierz pozycję **Rozwiązanie domyślne.** Wybierz **pozycję Odwołanie do połączenia (wersja zapoznawcza),** klikając pozycję **Wszystkie.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Zrzut ekranu przedstawiający edytowanie połączeń.":::

1. Edytuj poszczególne połączenia indywidualnie, wybierając ikonę wielokropka. Dodaj odpowiednie połączenia.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Zrzut ekranu przedstawiający sposób edytowania łączników.":::

1. Włącz przepływy w następującej kolejności:
   - Partner Center Webhook Registration (Insider Preview)
   - [Dostosowywanie] Tworzenie lub uzyskiwanie szczegółów z usługi Salesforce
   - Tworzenie aplikacji do współpracy Referral-Salesforce do Partner Center (insider preview)
   - Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)  
   - Partner Center do usługi Salesforce (niejawny program testów w wersji zapoznawczej)
   - Salesforce to Partner Center (Insider Preview)
   - Salesforce Opportunity to Partner Center (Insider Preview)
   - Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementy webhook

Możesz użyć interfejsów API Partner Center webhook, aby zarejestrować zdarzenia zmiany zasobów. Te zdarzenia zmiany są wysyłane do Twojego adresu URL jako wpisy HTTP.

1. Wybierz **Partner Center do programu Salesforce CRM (niejawny program testów)**.

1. Wybierz **ikonę Edytuj i** wybierz pozycję **Po otrzymaniu żądania HTTP.**

1. Wybierz **ikonę Kopiuj,** aby skopiować podany adres **URL żądania HTTP POST.**

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Zrzut ekranu przedstawiający sposób kopiowania adresu URL.":::

1. Wybierz przepływ **rejestracji Partner Center webhook (Insider Preview)** Power Automate, a następnie wybierz **pozycję Uruchom.**

1. Upewnij się, że **w okienku** po prawej stronie zostanie otwarte okno Uruchamianie przepływu, a następnie wybierz pozycję **Kontynuuj.**

1. Wprowadź następujące informacje:

   - **Punkt końcowy wyzwalacza HTTP:** ten adres URL został skopiowany z wcześniejszego kroku.
   - **Zdarzenia do zarejestrowania:** wybierz wszystkie dostępne zdarzenia **(utworzone** przez polecenie, **polecenie-zaktualizowane,** **powiązane-utworzone polecenie** i **powiązane-odwołania-zaktualizowane).**
   - **Zastąp istniejące punkty końcowe wyzwalacza, jeśli są obecne?**: Tak. Dla danego zdarzenia webhook można zarejestrować tylko jeden adres URL.

1. Wybierz **pozycję Uruchom przepływ,** a następnie wybierz pozycję **Gotowe.**

Ten webhook może teraz nasłuchiwać, tworzyć i aktualizować zdarzenia.

## <a name="customize-synchronization-steps"></a>Dostosowywanie kroków synchronizacji

Systemy CRM są wysoce dostosowane i można dostosować Power Automate oparte na konfiguracji CRM. Gdy polecenia do współpracy sprzedaży są synchronizowane między Partner Center i systemem CRM, pola, które są synchronizowane na komputerze Partner Center, są wyświetlane w przewodniku mapowania pól [niestandardowych.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby dokonaj odpowiednich zmian w obszarze **[Dostosuj] Tworzenie** lub uzyskiwanie szczegółów z usługi Salesforce lub zmiennych środowiskowych. Nie aktualizuj żadnych innych przepływów w Power Automate, ponieważ może to mieć wpływ na przyszłe uaktualnienia rozwiązania.

Dostępne są następujące dostosowania:

- **Wyświetl znacznik wyboru w** nazwie szansy sprzedaży: domyślnie obok nazwy szansy sprzedaży będzie wyświetlany znacznik wyboru wskazujący, że synchronizacja między usługami Partner Center i Salesforce CRM odbywa się pomyślnie. Podobnie w przypadku niepowodzenia synchronizacji zostanie wyświetlony znak krzyżowy. Aby uniknąć dodawania znacznika wyboru lub krzyżowego w  nazwie szansy sprzedaży, ustaw bieżącą wartość znacznika wyboru Wyświetl w zmiennej środowiskowej nazwa szansy sprzedaży na nie.

- **Nazwa etapu:**

  - **Nazwa aktywnego etapu:** jest to etap w potoku sprzedaży szansy sprzedaży w u usługi Salesforce.  Reprezentuje aktywny etap i jest odpowiednikiem polecenia w stanie zaakceptowanym w Partner Center. Może to być następny etap w potoku sprzedaży po etapie wstrzymania. Przeniesienie etapu sprzedaży szansy sprzedaży z etapu wstrzymywania do etapu aktywnego spowoduje zaakceptowanie polecenia w Partner Center zmiany zaczną być synchronizowane.

  - **Nazwa etapu wstrzymywania:** nazwa etapu w potoku sprzedaży szansy sprzedaży w u usługi Salesforce. Reprezentuje on etap wstrzymywania. Nowe polecenia wspólnej sprzedaży udostępnione przez firmę Microsoft, które nie zostały jeszcze zaakceptowane, zostaną ustawione na ten etap w u usługi Salesforce. Wszelkie zmiany wprowadzone w szansie sprzedaży, gdy jest ona wstrzymana, nie zostaną zsynchronizowane z Partner Center. Przeniesienie etapu sprzedaży szansy sprzedaży poza ten wstrzymany etap spowoduje zaakceptowanie polecenia w Partner Center zmiany zaczną być synchronizowane.

- **Kod kraju konta klienta:** podczas tworzenia nowego polecenia należy podać dwuliterowy kod kraju (ISO 3166). Domyślnie kod kraju będzie synchronizowany z polem BillingCountry konta i z pola **BillingCountry** w u usługi Salesforce. Jeśli masz inne pole w uciece Salesforce, z których ma być synchronizowane kod kraju:

  - W przypadku pola kodu kraju bez funkcjilookup na koncie, które zawiera kod dwuliterowy:

    - Zaktualizuj nazwę **pola Customer Account Country Code (Kod** kraju konta klienta) w zmiennej środowiskowej Salesforce przy użyciu nazwy pola CRM. Upewnij się, że po podaj nazwę pola, a nie jego nazwę wyświetlaną.

    - Edytuj **pozycję [Dostosuj] Utwórz** lub pobierz szczegóły z usługi Salesforce, a następnie przejdź do akcji Utwórz lub pobierz konto klienta w programie **CRM,** aby przypisać wartość **Country** (Kraj) do poprawnego pola w systemie CRM. Ponadto usuń przypisanie **wartości Country** (Kraj) z **właściwości BillingCountry**.

  - W przypadku pola kodu kraju opartego na odnośniku na koncie:

    - Dodaj nowe pole niestandardowe na koncie i wypełnij je automatycznie dwuliterowym kodem kraju (ISO 3166) na podstawie wartości wybranej w polu wyszukiwania i na odwrót.

    - Wykonaj powyższe kroki dla pola kodu kraju nielokakupu, aby zsynchronizować nowe pole niestandardowe z usługi CRM do i z Partner Center.

- **Wartość transakcji:** domyślnie wartość transakcji z Partner Center będzie synchronizowana z i **z wartości w** systemie CRM. Jeśli w systemie CRM masz inne pole, z których ma być synchronizowana wartość transakcji:

  - Zaktualizuj nazwę **pola Wartość** transakcji w zmiennej środowiskowej Salesforce przy użyciu nazwy pola CRM. Upewnij się, że po podaj nazwę pola, a nie jego nazwę wyświetlaną.

  - Edytuj **pozycję [Dostosuj]** Utwórz lub pobierz  szczegóły z usługi Salesforce,  przejdź do  tematu Tworzenie lub aktualizowanie szansy sprzedaży w systemie CRM i zaktualizuj zarówno pozycję Utwórz nową szansę sprzedaży, jak i zaktualizuj istniejące akcje szansy sprzedaży, aby przypisać wartość **DealValue** do poprawnego pola w uchwale Salesforce.

- **Kod waluty wartości transakcji:** nazwa pola kodu waluty wartości transakcji w uchwale Salesforce. Ta nazwa interfejsu API pola będzie używana do uzyskania kodu waluty wartości transakcji szansy sprzedaży podczas tworzenia lub aktualizowania poleceń w u Partner Center. Jeśli pole kodu waluty wartości transakcji różni się od pola domyślnego **CurrencyIsoCode,** zaktualizuj bieżącą wartość tej zmiennej środowiskowej.

  - Zaktualizuj nazwę **pola Waluta wartości** transakcji w zmiennej środowiskowej Salesforce przy użyciu nazwy pola CRM. Upewnij się, że po podaj nazwę pola, a nie jego nazwę wyświetlaną.

  - Edytuj **pozycję [Dostosuj]** Utwórz lub pobierz  szczegóły z usługi Salesforce,  przejdź do  tematu Tworzenie lub aktualizowanie szansy sprzedaży w systemie CRM i zaktualizuj zarówno pozycję Utwórz nową szansę sprzedaży, jak i zaktualizuj istniejące akcje szansy sprzedaży, aby przypisać **wartość DealValueCurrency** do poprawnego pola w uchwale Salesforce.

- **Możliwość wspólnej sprzedaży** synchronizacji: jeśli ustawisz wartość **tak,** tylko możliwości wspólnej sprzedaży i udostępniania potoku będą synchronizowane Partner Center z usługą Salesforce. Jeśli ustawisz **wartość nie**, potencjalni klienci, wspólnej sprzedaży i możliwości udostępniania potoku zostaną zsynchronizowane z usługi Partner Center do usługi Salesforce. Ta zmienna nie ma żadnego wpływu na szanse sprzedaży synchronizowane z usługi Salesforce do Partner Center.

## <a name="update-environment-variable"></a>Aktualizowanie zmiennej środowiskowej

Aby zaktualizować wartość zmiennej środowiskowej:

1. Przejdź do strony **Rozwiązania** i wybierz pozycję **Rozwiązanie domyślne.** Wybierz **pozycję Zmienna środowiskowa,** wybierając **pozycję Wszystkie.**

1. Wybierz zmienną środowiskową dla wartości, która ma zostać zaktualizowana, a następnie wybierz pozycję **Edytuj** za pomocą ikony wielokropka.

1. Zaktualizuj **wartość bieżącą** (nie aktualizuj wartości **domyślnej**) przy użyciu opcji **Nowa** wartość i podając wartość. Wartość musi być dopasowana do typu danych zmiennej. Na przykład typ danych Tak lub Nie będzie akceptował wartości Tak lub Nie.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Zrzut ekranu przedstawiający aktualizowanie zmiennych środowiskowych.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>End-to-end bi-directional co-sell referral synchronization (End-to-end bi-directional co-sell referral synchronization)

Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania Power Automate można przetestować synchronizację poleceń współsprzedaży między usługą Salesforce CRM i Partner Center.

### <a name="pre-requisites"></a>Wymagania wstępne

Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, rozwiązanie Power Automate musi wyraźnie rozdysmarować pola poleceń specyficzne dla firmy Microsoft. Ta identyfikacja zapewnia zespołom sprzedawców możliwość decydowania o tym, które polecenia chcą udostępnić firmie Microsoft w celu współpracy sprzedaży.

Zestaw pól niestandardowych jest dostępny w ramach jednostki Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** (Synchronizacja poleceń dla rozwiązania CRM usługi Salesforce). Administrator crm musi utworzyć oddzielną sekcję CRM z **niestandardowymi** polami Szansa sprzedaży.

Następujące pola niestandardowe powinny być częścią sekcji CRM:

- **Synchronizacja z Partner Center:** czy zsynchronizować możliwość sprzedaży z Partner Center. Domyślnie wartość tego pola to Nie i musi być jawnie ustawiona na wartość Tak przez sprzedawcę, aby udostępnić szansę sprzedaży firmie Microsoft. Nowe polecenia współużytk Partner Center do systemu CRM będą mieć tę wartość pola ustawioną na Tak.

- **Identyfikator polecenia:** pole identyfikatora tylko do odczytu dla poleceń Partner Center Microsoft.

- **Link do poleceń:** link tylko do odczytu do polecenia w aplikacji Microsoft Partner Center.

- **Jak firma Microsoft może pomóc:** wymagana przez firmę Microsoft pomoc w przypadku polecenia. Aby utworzyć polecenie współpracy sprzedaży, wybierz odpowiednią pomoc wymaganą od firmy Microsoft. Osoba kontaktowa z klientem musi być skojarzona z szansą utworzenia polecenia do współpracy sprzedaży. Aby utworzyć polecenie inne niż współsieć, nie zaznaczaj tego pola. Polecenie braku współpracy sprzedaży można przekonwertować na polecenie do współpracy sprzedaży w dowolnym momencie, wybierając odpowiednią opcję wymaganą przez pomoc.

- **Microsoft Partner Center Widoczność poleceń:** wybierz widoczność Partner Center polecenia. Dzięki temu, że jest ono widoczne dla sprzedawców firmy Microsoft, polecenie inne niż sprzedaż może zostać przekonwertowane na współspozycję. Jeśli wymagana jest pomoc firmy Microsoft, polecenie jest domyślnie widoczne dla sprzedawców firmy Microsoft. Po oznaczeniu tego pola jako widocznego nie można go przywrócić.

- **Microsoft CRM identyfikatora:** po utworzeniu i zaakceptowaniu polecenia współs sprzedaży przez firmę Microsoft to pole zostanie wypełnione identyfikatorem CRM firmy Microsoft.

- **Microsoft Partner Center Solutions:** niestandardowy obiekt kojarzący gotowe do współpracy rozwiązania lub rozwiązania firmy Microsoft z szansą sprzedaży. Co najmniej jedno rozwiązanie można dodać lub usunąć z szansy sprzedaży. Przed udostępnieniem go firmie Microsoft należy dodać do szansy sprzedaży co najmniej jedno gotowe do sprzedaży lub rozwiązanie firmy Microsoft. Aby skojarzyć ten obiekt z szansą sprzedaży, zaktualizuj formularz **Szansa** sprzedaży w systemie CRM.

- **Inspekcja:** dziennik inspekcji tylko do odczytu do synchronizacji z Partner Center poleceniami

### <a name="scenarios"></a>SCENARIUSZY

1. Synchronizacja poleceń, gdy polecenie jest tworzone lub aktualizowane w systemie CRM i synchronizowane w Partner Center:

   1. Zaloguj się do środowiska CRM usługi Salesforce przy użyciu użytkownika, który ma wgląd w sekcję **Opportunity** (Szansa sprzedaży) w chmurze CRM.

   1. Upewnij się, że sekcja **Microsoft Partner Center** jest obecna podczas tworzenia nowej szansy sprzedaży w **środowisku** CRM usługi Salesforce.

   1. Szanse sprzedaży, które zostały pomyślnie zsynchronizowane z Partner Center, zostaną zidentyfikowane za ✔ crm usługi Salesforce.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Zrzut ekranu przedstawiający środowisko usługi Salesforce.":::

   1. Aby zsynchronizować tę możliwość z usługą Microsoft Partner Center, należy ustawić następujące pola w widoku karty:

      - **Jak firma Microsoft może pomóc?**: Aby utworzyć polecenie do współpracy sprzedaży, wybierz odpowiednią opcję pomocy.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Zrzut ekranu przedstawiający sposób uzyskania odpowiednich pól w widoku karty.":::

      - **Synchronizacja z Partner Center:** Tak
      - **Kontakt z** klientem: aby utworzyć polecenie współpracy sprzedaży, dodaj kontakt klienta do szansy sprzedaży.
      - **Rozwiązania firmy Microsoft:** aby udostępnić polecenie firmie Microsoft, dodaj do szansy sprzedaży prawidłowe rozwiązanie gotowe do współpracy lub rozwiązanie firmy Microsoft.

   1. Po skonfigurowaniu opcji synchronizacji **szansy** sprzedaży Partner Center ustawieniem **Tak** poczekaj 10 minut, zaloguj się do Partner Center konta. Twoje polecenia zostaną zsynchronizowane z programem Salesforce CRM, a link do poleceń zostanie wypełniony. W przypadku awarii pole Inspekcja zostanie wypełnione informacjami o błędzie.

   1. Podobnie, jeśli opcja **Synchronizuj** z Partner Center jest ustawiona na wartość **Tak,** w przypadku zaktualizowania szansy sprzedaży w programie Salesforce CRM zmiany zostaną zsynchronizowane z Partner Center magazynu.

2. Synchronizacja poleceń, gdy polecenie jest tworzone lub aktualizowane w programie Microsoft Partner Center i synchronizowane w środowisku CRM usługi Salesforce:

    1. Zaloguj się do swojego Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)

    1. Wybierz **pozycję Polecenia** z menu po lewej stronie.

    1. Utwórz nowe polecenie co-sell z Partner Center, klikając opcję "Nowa transakcja".

    1. Zaloguj się do środowiska CRM usługi Salesforce.

    1. Przejdź do okna **Otwieranie szans sprzedaży.** Polecenie utworzone w programie Microsoft Partner Center jest teraz synchronizowane w programie Salesforce CRM.

    1. Po wybraniu zsynchronizowanego polecenia zostaną wypełnione szczegóły widoku karty.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Zrzut ekranu przedstawiający stronę szans sprzedaży usługi Salesforce.":::

>[!NOTE]
>**Potrzebujesz pomocy przy wdrażaniu?**
>Aby uzyskać pomoc w zakresie wdrażania łącznika poleceń współ sprzedawania, możesz angażować konsultanta technicznego partnera. Mogą one zapewnić pomoc w zakresie wdrażania i najlepsze rozwiązania w zakresie pomyślnej implementacji.
>
>Aby uzyskać więcej informacji, zobacz How to Submit a technical presales and deployment services request (Jak przesłać żądanie usług [przedsprzedadzeń i wdrożeń technicznych)](technical-benefits.md)

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)

- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)

- [Elementy webhook Centrum partnerskiego](/partner-center/develop/partner-center-webhooks)
