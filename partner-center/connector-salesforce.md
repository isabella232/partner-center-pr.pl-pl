---
title: Łącznik do współsprzedaży dla usługi Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj polecenia w Partner Center z crm usługi Salesforce. Sprzedawcy mogą następnie sprzedawać z firmą Microsoft z poziomu systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276981"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Łącznik do współsprzedaży dla rozwiązania Salesforce CRM — omówienie

**Odpowiednie role:** Administrator poleceń | Administrator systemu lub customizer systemu w systemie CRM

Partner Center łącznika do współpracy sprzedaży umożliwia sprzedawcom sprzedawanie z firmą Microsoft z poziomu systemów CRM. Nie trzeba ich szkolić do używania Partner Center do zarządzania transakcjami sprzedaży. Za pomocą łączników do współpracy sprzedaży możesz utworzyć nowe polecenie współpracy sprzedaży, aby zaangażować sprzedawcę firmy Microsoft, otrzymać polecenia od sprzedawcy firmy Microsoft, zaakceptować/odrzucić polecenia, zmodyfikować dane transakcji, takie jak wartość transakcji i data zamknięcia.  Możesz również otrzymywać wszelkie aktualizacje od sprzedawców firmy Microsoft dotyczące tych transakcji sprzedaży. Wszystkie polecenia można wykonać podczas pracy w ramach wybranego rozwiązania CRM, a nie w Partner Center. 

Rozwiązanie jest oparte na rozwiązaniu Microsoft Power Automate i używa Partner Center API.

## <a name="before-you-install---pre-requisites"></a>Przed zainstalowaniem — wymagania wstępne

|**Tematy**   |**Szczegóły**   |**Linki**   |
|--------------|--------------------|------|
|Microsoft Partner Network identyfikator |Potrzebny jest prawidłowy identyfikator MPN|Aby dołączyć [do programu MPN](https://partner.microsoft.com/)|
|Gotowość do współs sprzedaży|Twoje rozwiązanie ip/usług musi być gotowe do współpracy.|[Sell with Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Konto Centrum partnerskiego|Identyfikator MPN skojarzony z dzierżawą Partner Center musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współs sprzedaży. Przed wdrożeniem łączników sprawdź, czy polecenia dotyczące współpracy sprzedaży są Partner Center portalu.|[Zarządzanie kontem](create-user-accounts-and-set-permissions.md)|
|Partner Center ról użytkownika|Pracownik, który zainstaluje łączniki i użyje ich, musi być administratorem poleceń|[Przypisywanie ról i uprawnień użytkowników](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Rola użytkownika CRM to administrator systemu lub customizer systemu|[Przypisywanie ról w programie Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Account|Aktywne konto [Power Automate](https://flow.microsoft.com) administratora systemu CRM lub customizera systemu. Ten użytkownik powinien zalogować się [Power Automate](https://flow.microsoft.com) co najmniej raz przed instalacją.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalacja pakietu Salesforce dla pól niestandardowych firmy Microsoft 

Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, rozwiązanie Power Automate musi jasno identyfikować pola poleceń specyficzne dla firmy Microsoft. To oznaczanie zapewnia zespołom sprzedawców partnerskich możliwość decydowania o tym, które polecenia mają być współużytkowania przez nich udostępnianie firmie Microsoft.

1. W u usługi Salesforce aktywuj pozycję **Notatki** i dodaj ją do listy powiązanych szans sprzedaży. 
[Odwołanie](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. **Aktywuj zespoły szans** sprzedaży, wykonać następujące czynności: 
    - W instalatorze użyj pola **Szybkie wyszukiwanie,** aby zlokalizować ustawienia zespołu szans sprzedaży.
    - Zdefiniuj ustawienia zgodnie z potrzebami.
[Odwołanie](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. W uakiecie Salesforce zainstaluj niestandardowe pola i obiekty przy użyciu [instalatora pakietu](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Użyj tej funkcji, aby zainstalować pakiet w dowolnej firmie.

>[!NOTE]
>Jeśli instalujesz w piaskownicy, musisz zastąpić początkową część adresu URL wartością http://test.salesforce.com

4. W u usługi Salesforce dodaj rozwiązania firmy Microsoft do listy Opportunity related **(Powiązane z szansą** sprzedaży). Po dodaniu wybierz **ikonę klucza** i zaktualizuj właściwości

## <a name="best-practice-test-before-you-go-live"></a>Najlepsze rozwiązanie: Testowanie przed rozpoczęciem transmisji na żywo

Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania Power Automate w środowisku produkcyjnym należy przetestować rozwiązanie w przejściowym wystąpieniu crm.

- Zainstaluj rozwiązanie Microsoft Power Automate w środowisku przejściowym/wystąpieniu crm.

- Zrób kopię rozwiązania, a następnie uruchom konfigurację i Power Automate dostosowywania przepływu w środowisku przejściowym.

- Przetestuj rozwiązanie w wystąpieniu przejściowym/CRM.

- W przypadku powodzenia zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalowanie Partner Center poleceń usługi Salesforce CRM

1. Przejdź do [Power Automate](https://flow.microsoft.com) i wybierz **pozycję Środowiska** w prawym górnym rogu. Spowoduje to pokazanie dostępnych wystąpień CRM.

2. Wybierz odpowiednie wystąpienie crm z listy rozwijanej w prawym górnym rogu.

3. Wybierz **pozycję Rozwiązania** na pasku nawigacyjnym po lewej stronie.

4. Wybierz link **Otwórz usługę AppSource** w górnym menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz usługę AppSource.":::

5. Wyszukaj **łączniki poleceń Partner Center dla usługi Salesforce** w oknie podręcznym.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. Wybierz przycisk **Pobierz teraz, a** następnie pozycję **Kontynuuj.**

7. Spowoduje to otwarcie strony, na której można wybrać środowisko CRM usługi Salesforce do zainstalowania aplikacji.  Wyrażanie zgody na warunki i postanowienia.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostępne rozwiązania CRMS.":::

8. Następnie zostaniesz skierowany do strony **Zarządzanie rozwiązaniami.**  Przejdź do pozycji "Partner Center polecenia" przy użyciu przycisków strzałek w dolnej części strony. **Instalacja zaplanowana** powinna być wyświetlana obok Partner Center polecenia. Instalacja potrwa 10–15 minut.

9. Po zakończeniu instalacji wróć do strony Power Automate [i](https://flow.microsoft.com) wybierz pozycję **Rozwiązania** w obszarze nawigacji po lewej stronie. Zwróć **uwagę Partner Center że synchronizacja poleceń dla usługi Salesforce** jest dostępna na liście Rozwiązania.

10. Wybierz **Partner Center polecenia dla usługi Salesforce.** Dostępne są Power Automate przepływów i jednostek:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Przepływy usługi Salesforce.":::



## <a name="configure-the-solution"></a>Konfigurowanie rozwiązania

1. Po zainstalowaniu rozwiązania w wystąpieniu crm przejdź z powrotem do Power Automate [.](https://flow.microsoft.com/)

2. Z **listy rozwijanej** Środowiska w prawym górnym rogu wybierz wystąpienie crm, w którym zainstalowano Power Automate rozwiązanie.
3. Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:
    - Partner Center z poświadczeniami administratora poleceń
    - Zdarzenia Centrum partnerskiego
    - Administrator CRM z przepływami Power Automate w rozwiązaniu.
4. Wybierz **pozycję** Połączenia na pasku nawigacyjnym po lewej stronie i wybierz rozwiązanie "Partner Center polecenia" z listy.

5. Utwórz połączenie, klikając **pozycję Utwórz połączenie.**

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Utwórz połączenie.":::

- Wyszukaj Partner Center poleceń (wersja zapoznawcza) na pasku wyszukiwania w prawym górnym rogu.

- Utwórz połączenie dla użytkownika Partner Center z rolą poświadczeń administratora poleceń.

-  Następnie utwórz połączenie Partner Center zdarzeń sieciowych dla Partner Center użytkownika przy użyciu poświadczeń administratora poleceń.

- Utwórz połączenie dla usługi Salesforce dla użytkownika administratora CRM.

-  Po dodaniu wszystkich połączeń w środowisku powinny zostać wyświetlony następujące połączenia:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Obserwuj połączenia.":::

### <a name="edit-the-connections"></a>Edytowanie połączeń

1. Wróć do strony Rozwiązania i wybierz pozycję **Rozwiązanie domyślne.**  Wybierz **pozycję Odwołanie do połączenia (wersja zapoznawcza),** klikając pozycję **Wszystkie.**
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Rozpocznij edytowanie łącznika.":::

2. Edytuj poszczególne połączenia, wybierając ikonę z trzema kropkami. Dodaj odpowiednie połączenia.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edytowanie łączników.":::

3. Włącz przepływy w następującej kolejności:

- Partner Center Webhook Registration (Insider Preview)
- Tworzenie polecenia do współpracy sprzedaży — salesforce do Partner Center (niejawny program testów w wersji zapoznawczej)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Partner Center do usługi Salesforce (niejawny program testów w wersji zapoznawczej)
- Salesforce to Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementy webhook

Interfejsy API Partner Center Webhook umożliwiają rejestrowanie zdarzeń zmiany zasobów. Te zdarzenia zmiany są wysyłane na twój adres URL jako wpisy HTTP.

1. Aby zarejestrować swój adres URL, wybierz **Partner Center webhook Registration (Insider Preview)** Power Automate przepływu.

2. Dodaj połączenia dla (a.) Partner Center z poświadczeniami administratora poleceń (b.) Partner Center zdarzenia, jak wyróżnione poniżej

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz.":::

3. Po wdowy tych aktualizacjach zobaczysz

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook ( Webhook).":::

4. Zapisz zmiany i wybierz pozycję **Włącz.**

   Aby umożliwić Partner Center webhook nasłuchiwać zmian zdarzeń, wykonaj następujące kroki:

5. Wybierz **Partner Center do programu Salesforce CRM (niejawny program zapoznawczy).**

6. Wybierz **ikonę Edytuj** i wybierz pozycję **Po otrzymaniu żądania HTTP.**

7. Wybierz **ikonę Kopiuj,** aby skopiować podany adres URL żądania HTTP POST.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Skopiuj adres URL.":::

8. Teraz wybierz przepływ "Rejestracja Partner Center webhook (niejawny program testów)" i wybierz Power Automate **Uruchom.**

9. Upewnij się, że w okienku po prawej stronie zostanie otwarte okno "Uruchom przepływ", a następnie wybierz pozycję **Kontynuuj.**

10. Wprowadź następujące informacje:

    1. **Punkt końcowy wyzwalacza HTTP:** adres URL skopiowany z wcześniejszego kroku

    2. **Zdarzenia do zarejestrowania:**"utworzono polecenie" i "polecenie-zaktualizowane"

    3. **Zastąp istniejące punkty końcowe wyzwalacza, jeśli są obecne:** Tak (spowoduje to zastąpienie wszystkich istniejących punktów końcowych).

11. Wybierz **pozycję Uruchom,** a następnie wybierz pozycję **Gotowe.**

Teraz może nasłuchiwać zdarzeń tworzenia i aktualizowania.

## <a name="customize-synchronization-steps"></a>Dostosowywanie kroków synchronizacji

Gdy polecenia dotyczące współpracy sprzedaży są synchronizowane między Partner Center i systemem CRM, pola, które są synchronizowane na Partner Center PC, są wymienione tutaj.

Często systemy CRM są wysoce dostosowane. Możesz dostosować przepływy Power Automate przepływów. Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w krokach Power Automate przepływów.  Dostępne są mapowania rozwiązań Microsoft Partner Centers do crm, ale w zależności od środowiska CRM można dostosować pola.

Wiele kroków każdego z przepływów Power Automate można dostosować w zależności od potrzeb. Poniżej przedstawiono przykłady dostępnych dostosowań:

1. Aby dostosować pola dla zdarzeń tworzenia lub aktualizowania w Partner Center do synchronizacji poleceń CRM:

   1. Wybierz pozycję Partner Center do programu Salesforce CRM (niejawny program zapoznawczy).

   2. Wybierz **pozycję Edytuj,** aby edytować/dostosować Power Automate przepływu.

   3. Wybierz **pozycję (Zakres) Synchronizuj potencjalnego klienta lub szansę sprzedaży.**

2. Aby dostosować mapowania pól CRM dla tworzenia zdarzeń, wybierz pozycję Jeśli jest to nowa szansa sprzedaży **udostępnionej, a następnie pozycję**. Wybierz krok podrzędny, **jeśli tak,** a następnie rozwiń pozycję **Tworzenie nowej szansy sprzedaży w crm**. Mapowania można edytować w tej sekcji, korzystając z przewodnika mapowania pól.

   1. Aby dostosować mapowania pól CRM dla zdarzeń aktualizacji, wybierz krok "(Zakres) Synchronizowanie potencjalnego klienta lub szansy sprzedaży".

   2. Wybierz **pozycję Jeśli jest to aktualizacja szansy sprzedaży, a następnie .** Wybierz krok podrzędny, **jeśli tak,** a następnie rozwiń pozycję Jeśli różnica między obiektami szansy sprzedaży w **programie Partner Center crm,** a następnie .  

   3. Wybierz **pozycję Jeśli tak, a** następnie zaktualizuj **istniejącą szansę sprzedaży**

3. Aby dostosować pola synchronizacji poleceń crm na komputer dla zdarzeń aktualizacji:

   1. Wybierz **pozycję Edytuj,**  aby edytować/dostosować Power Automate przepływu.

   2. Wybierz **pozycję (Zakres) Zsynchronizuj szansę sprzedaży.**

   3. W przypadku dostosowywania mapowań pól CRM (na podstawie przewodnika mapowania pól) dla zdarzeń aktualizacji wybierz opcję Jeśli istnieje różnica między obiektami potencjalnych klientów w systemach **Partner Center i CRM,** a następnie .

   4. Wybierz krok podrzędny, **jeśli tak,** a następnie rozwiń krok Aktualizuj odwołanie **przy użyciu danych szansy sprzedaży.**

   Mapowania można edytować w tej sekcji na podstawie przewodnika mapowania pól.

4. Aby dostosować pola synchronizacji poleceń z systemu CRM do komputera w celu utworzenia zdarzeń?

   1. Wybierz **pozycję Edytuj,**  aby edytować/dostosować Power Automate przepływu.

   2. Wybierz **pozycję (zakres) Synchronizowanie poleceń.**

   3. W celu dostosowywania mapowań pól CRM (na podstawie przewodnika mapowania pól) dla zdarzeń tworzenia wybierz pozycję **Utwórz polecenie firmy Microsoft.**

Mapowania można edytować w tej sekcji na podstawie przewodnika mapowania pól.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>End-to-end bi-directional co-sell referral synchronization

Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania Power Automate można przetestować synchronizację poleceń współsprzedaży między usługą Salesforce CRM i Partner Center.

### <a name="pre-requisites"></a>Wymagania wstępne

Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, Power Automate rozwiązanie musi wyraźnie rozdysmarować pola poleceń specyficzne dla firmy Microsoft. Ta identyfikacja zapewnia zespołom sprzedawców możliwość decydowania o tym, które polecenia chcą udostępnić firmie Microsoft w celu współpracy sprzedaży.

Zestaw pól niestandardowych jest dostępny w ramach jednostki Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** (Synchronizacja poleceń dla rozwiązania CRM usługi Salesforce). Administrator crm musi utworzyć oddzielną sekcję CRM z **niestandardowymi** polami Szansa sprzedaży.

Następujące pola niestandardowe powinny być częścią sekcji CRM:

- **Synchronizacja z Partner Center:** czy zsynchronizować możliwość sprzedaży z usługą Microsoft Partner Center

- **Identyfikator polecenia:** pole identyfikatora tylko do odczytu dla poleceń Partner Center Microsoft

- **Link do poleceń:** link tylko do odczytu do polecenia w aplikacji Microsoft Partner Center

- **Jak firma Microsoft może pomóc:** wymagana przez firmę Microsoft pomoc w przypadku polecenia

- **Produkty:** lista produktów skojarzonych z tą szansą sprzedaży

- **Inspekcja:** dziennik inspekcji tylko do odczytu do synchronizacji z Partner Center poleceniami

### <a name="scenarios"></a>Scenariuszy:

1. Synchronizacja poleceń, gdy polecenie jest tworzone lub aktualizowane w systemie CRM i synchronizowane w Partner Center:

   1. Zaloguj się do środowiska CRM usługi Salesforce przy użyciu użytkownika, który ma wgląd w sekcję **Szansa** sprzedaży w systemie CRM.

   2. Upewnij się, że podczas tworzenia nowej szansy sprzedaży w środowisku CRM usługi Salesforce jest obecna następująca sekcja

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Środowisko usługi Salesforce.":::

   3. Aby zsynchronizować tę możliwość z usługą Microsoft Partner Center, należy ustawić następujące pola w widoku karty:

       - "Synchronizuj z Partner Center": Tak
       - "Jak może pomóc firma Microsoft?": wybierz jedną z następujących opcji:
       - Produkty: identyfikatory rozwiązań produktu

   4. Po skonfigurowaniu opcji synchronizacji szansy sprzedaży  **Partner Center** na wartość **Tak,** poczekaj 10 minut, zaloguj się do Partner Center konta. Twoje polecenia zostaną zsynchronizowane z programem Salesforce CRM.

   5. Gdy opcja "Synchronizuj z Partner Center" jest ustawiona na wartość "Tak", jeśli zaktualizujemy możliwość sprzedaży w programie Salesforce CRM, zmiany zostaną zsynchronizowane z kontem Partner Center sprzedaży.

   6. Szanse sprzedaży, które zostały pomyślnie zsynchronizowane z Partner Center zostaną zidentyfikowane za pomocą ✔icon w programie Salesforce CRM.

2. Synchronizacja poleceń, gdy polecenie jest tworzone lub aktualizowane w programie Microsoft Partner Center i synchronizowane w środowisku CRM usługi Salesforce:

    1. Zaloguj się do swojego Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)

    2. Wybierz **pozycję Polecenia** z menu po lewej stronie.

    3. Utwórz nowe polecenie co-sell z Partner Center klikając opcję "Nowa transakcja".

    4. Zaloguj się do środowiska CRM usługi Salesforce.

    5. Przejdź do okna **Otwieranie szans sprzedaży.** Polecenie utworzone w programie Microsoft Partner Center jest teraz synchronizowane w programie Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Ekran szans sprzedaży usługi Salesforce.":::

    6. Po wybraniu zsynchronizowanego polecenia zostaną wypełnione szczegóły widoku karty.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)

- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)

- [Elementy webhook Centrum partnerskiego](/partner-center/develop/partner-center-webhooks)
