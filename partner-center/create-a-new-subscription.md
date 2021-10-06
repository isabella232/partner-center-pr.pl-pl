---
title: Tworzenie subskrypcji klientów w Partner Center
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak sprzedawać klientom subskrypcje produktów publikowanych przez firmę Microsoft oraz produktów SaaS publikowanych przez zewnętrznych isvów.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: c42e2e8dbc98bdf9ed0e2994bfb7ad49848aad76
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129565335"
---
# <a name="manage-customer-subscriptions"></a>Zarządzanie subskrypcjami klientów

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży

Po utworzeniu rekordu klienta w katalogu Partner Center można sprzedawać im subskrypcje produktów w katalogu. Dotyczy to produktów publikowanych przez firmę Microsoft oraz produktów SaaS (Software as a Service) publikowanych przez niezależnych dostawców oprogramowania (ISV) innych firm na [platformie handlowej.](https://azuremarketplace.microsoft.com/marketplace)

Niektóre oferty są ograniczone do jednej subskrypcji na klienta. Aby wyświetlić listę ofert, które są ograniczone, odwiedź stronę Partner Center **Cenniki.**

> [!IMPORTANT]
> Jako partner w programie CSP  możesz kupić oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center. Oznacza to, że  możesz kupić dowolną opartą na licencjach lub mierzoną [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ofertę **SaaS,** która została Ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp. Aby kupić inne, komercyjne oferty platformy handlowej od isvs (na przykład oferty oparte na użyciu obejmujące aplikacje platformy Azure, kontenery lub maszyny wirtualne) lub zarządzać nimi, musisz przejść do witryny [Azure Portal](https://portal.azure.com/).

> [!NOTE]
> Wszystkie daty i godziny w Partner Center są podane w standardzie czasu uniwersalnego (UTC). Może się to różnić nawet o 24 godziny od czasu lokalnego.

## <a name="create-a-new-subscription"></a>Tworzenie nowej subskrypcji

> [!NOTE]
> Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych, zobacz [Getting around Partner Center (Poruszanie się po Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off)).

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Na Partner Center [nawigacyjnym](https://partner.microsoft.com/dashboard)wybierz kafelek **Klienci,** a następnie wybierz klienta z listy Klienci.

2. Wybierz **pozycję Dodaj subskrypcję.** Na **karcie Usługi online** będą wyświetlane wszystkie dostępne oferty SaaS w witrynie Marketplace.

3. Aby wyświetlić tylko niektóre typy subskrypcji, należy dokonać wyboru w dostępnych filtrach:
   - **Publisher:** wybierz firmę **Microsoft,** aby wyświetlić  tylko oferty firmy Microsoft lub partnera, aby wyświetlić produkty platformy handlowej opublikowane przez isvs.
   - **Typ rozliczeń:** wybierz typ rozliczeń subskrypcji, których chcesz użyć: **Licencja** lub **Użycie.** Zobacz [Rozliczenia oparte na licencjach,](license-based-billing.md) aby uzyskać informacje, które pomogą Ci wybrać miesięczną i roczną częstotliwość rozliczeń.
   - **Kategoria:** wybierz **Enterprise,** **Małe firmy** lub Wersja **próbna.** Aby uzyskać informacje o subskrypcjach wersji próbnej, zobacz [Temat Oferty dla klientów wersji próbnych produktów firmy Microsoft.](offer-your-customers-trials-of-microsoft-products.md)

4. Wybierz subskrypcje produktów, które chcesz kupić dla klienta. Produkty, które widzisz, zależą od typu segmentu klientów (edukacja, administracja rządowa itp.) i zastosowanych filtrów. Niektóre oferty wyświetlane w witrynie Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera CSP. Może to być spowodowane:
   - Klient ma już subskrypcję tego produktu i ma tylko jedną z nich
   - Subskrypcja klienta może zostać wstrzymana (w tym przypadku możesz ponownie aktywować subskrypcję zamiast kupować nową).
   - W przypadku ofert SaaS dla isv może być kilka powodów, dla których oferta nie jest dostępna do zakupu: isv may not support the customer's billing country or region; IsV may have chosen not make the offer available through the CSP program; lub, isv may have made the offer [exclusive to only](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) certain CSP partners. Oferta isv (isv) może być również nie do transakcji za pośrednictwem Partner Center (na przykład kontenerów lub niektórych ofert opartych na użyciu).  

5. Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby) i wybierz **pozycję Dodaj do koszyka.**

6. Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj zamówienie.

7. Po przejrzenia zamówień i przygotowaniu się do zakupu tych subskrypcji wybierz pozycję **Kup**.

8. Po zakupie subskrypcji dla klienta wystąpią następujące zdarzenia:

    - Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji na stronie **Subskrypcje tego** klienta. W tym miejscu możesz wybrać licencje dodatku, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.

    **W przypadku subskrypcji SAAS isv (opartych na licencjach i mierzonych):**
    - Otrzymasz link do witryny wydawcy isv. Ten link powinien ułatwić ukończenie wdrażania lub konfigurowania konta subskrypcji klienta.

    > [!NOTE]
    > Ani Ty, ani Klient nie otrzymacie wiadomości e-mail z instrukcjami dotyczącymi ukończenia procesu skonfigurowania/aprowizowania konta dla tego typu subskrypcji isv).

    - Jeśli Twoja subskrypcja zawiera 30-dniową bezpłatną wersję próbną, bezpłatny okres próbny zostanie zastosowany automatycznie. Jako partner w programie CSP nie możesz zrezygnować z okresu bezpłatnej wersji próbnej ofert zakupu dla klientów. Po zakończeniu okresu bezpłatnej wersji próbnej okres subskrypcji rozpocznie się, a subskrypcja zostanie przekształcona w stan płatny. Subskrypcja zostanie następnie automatycznie odnowiona zgodnie z tym samym harmonogramem.

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Na Partner Center [nawigacyjnym](https://partner.microsoft.com/dashboard)wybierz pozycję **Klienci,** a następnie wybierz klienta z listy Klienci.

2. Wybierz **pozycję Dodaj subskrypcję.** Na **karcie Usługi online** będą wyświetlane wszystkie dostępne oferty SaaS w witrynie Marketplace.

3. Aby wyświetlić tylko niektóre typy subskrypcji, należy dokonać wyboru w dostępnych filtrach:
   - **Publisher:** wybierz firmę **Microsoft,** aby wyświetlić  tylko oferty firmy Microsoft lub partnera, aby wyświetlić produkty platformy handlowej opublikowane przez isvs.
   - **Typ rozliczeń:** wybierz typ rozliczeń subskrypcji, których chcesz użyć: **Licencja** lub **Użycie.** Zobacz [Rozliczenia oparte na licencjach,](license-based-billing.md) aby uzyskać informacje, które pomogą Ci wybrać miesięczną i roczną częstotliwość rozliczeń.
   - **Kategoria:** wybierz **Enterprise,** **Małe firmy** lub Wersja **próbna.** Aby uzyskać informacje o subskrypcjach wersji próbnej, zobacz [Temat Oferty dla klientów wersji próbnych produktów firmy Microsoft.](offer-your-customers-trials-of-microsoft-products.md)

4. Wybierz subskrypcje produktów, które chcesz kupić dla klienta. Produkty, które widzisz, zależą od typu segmentu klientów (edukacja, administracja rządowa itp.) i zastosowanych filtrów. Niektóre oferty wyświetlane w witrynie Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera CSP. Może to być spowodowane:
   - Klient ma już subskrypcję tego produktu i ma tylko jedną z nich
   - Subskrypcja klienta może zostać wstrzymana (w tym przypadku możesz ponownie aktywować subskrypcję zamiast kupować nową).
   - W przypadku ofert SaaS dla isv może być kilka powodów, dla których oferta nie jest dostępna do zakupu: isv may not support the customer's billing country or region; IsV may have chosen not make the offer available through the CSP program; lub, isv may have made the offer [exclusive to only](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) certain CSP partners. Oferta isv (isv) może być również nie do transakcji za pośrednictwem Partner Center (na przykład kontenerów lub niektórych ofert opartych na użyciu).  

5. Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby) i wybierz **pozycję Dodaj do koszyka.**

6. Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj zamówienie.

7. Po przejrzenia zamówień i przygotowaniu się do zakupu tych subskrypcji wybierz pozycję **Kup**.

8. Po zakupie subskrypcji dla klienta wystąpią następujące zdarzenia:

    - Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji na stronie **Subskrypcje tego** klienta. W tym miejscu możesz wybrać licencje dodatku, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.

    **W przypadku subskrypcji SAAS isv (opartych na licencjach i mierzonych):**
    - Otrzymasz link do witryny wydawcy isv. Ten link powinien ułatwić ukończenie wdrażania lub konfigurowania konta subskrypcji klienta.

    > [!NOTE]
    > Ani Ty, ani Klient nie otrzymacie wiadomości e-mail z instrukcjami dotyczącymi ukończenia procesu skonfigurowania/aprowizowania konta dla tego typu subskrypcji isv).

    - Jeśli Twoja subskrypcja zawiera 30-dniową bezpłatną wersję próbną, bezpłatny okres próbny zostanie zastosowany automatycznie. Jako partner w programie CSP nie możesz zrezygnować z okresu bezpłatnej wersji próbnej ofert zakupu dla klientów. Po zakończeniu okresu bezpłatnej wersji próbnej okres subskrypcji rozpocznie się, a subskrypcja zostanie przekształcona w stan płatny. Subskrypcja zostanie następnie automatycznie odnowiona zgodnie z tym samym harmonogramem.

* * *

## <a name="update-subscriptions-with-add-ons"></a>Aktualizowanie subskrypcji z dodatkami

Aby kupić dodatek, klient musi najpierw mieć aktywną subskrypcję podstawową.  Nie można kupować dodatków za pomocą wykazu.

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Wybierz subskrypcję, którą chcesz zarządzać.

4. Poniżej sekcji **Stan** znajduje się lista dostępnych dodatków dla subskrypcji.  

5. Zaktualizuj liczbę licencji dla każdego wymaganego dodatku. Następnie **prześlij** zmiany.

Możliwość zakupu dodatków za pośrednictwem usługi Partner Center jest dostępna tylko dla dostawców bezpośrednich i pośrednich.
Tylko kwalifikujące się dodatki są wyświetlane na podstawie podstawowych wymagań i dostępności regionalnej. Aby uzyskać więcej informacji na temat cen i ofert, zapoznaj się z macierzą ofert odsprzedawcy chmury. Wstrzymanie subskrypcji podstawowej spowoduje również wstrzymanie wszystkich skojarzonych dodatków.

Daty rozpoczęcia dla dodatków są dopasowywane do podstawowej subskrypcji, a opłaty są obliczane na podstawie daty rozpoczęcia i zakończenia naliczania opłat z opłatami proporcjonalnymi na pierwszej fakturze. Aby uzyskać dodatkowe informacje, zobacz [Rozliczenia oparte na licencjach.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Wstrzymywanie lub anulowanie subskrypcji

Partnerzy mogą wstrzymać lub anulować subskrypcję na żądanie klienta lub w przypadku niepłacenia lub oszustwa.

### <a name="suspend-a-subscription"></a>Zawieszenie subskrypcji

Jeśli zmienisz stan subskrypcji na Wstrzymano, użytkownicy nie będą mogli logować się ani uzyskać dostępu do usług.

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Wybierz subskrypcję, którą chcesz zarządzać.

4. W sekcji **Stan** wybierz pozycję **Wstrzymano**. Następnie **prześlij** zmiany.

5. Wszystkie dane zostaną usunięte, chyba że subskrypcja zostanie ponownie aktywowana w ciągu 90 dni lub 90 dni plus liczba dni między otwarciem konta a pierwszym okresem rozliczeniowym (maksymalnie 120 dni).

Po wstrzymaniu subskrypcji data, która zostanie wyświetlony poniżej przycisku **Wstrzymano,** wskazuje, kiedy subskrypcja automatycznie wygaśnie, jeśli subskrypcja nie zostanie ponownie aktywowana. 

> [!NOTE]
> Subskrypcje CSP nie mają wygasłego okresu (jak robią to subskrypcje internetowe), w którym usługi nadal działają, ale subskrypcja nie generuje żadnych opłat rozliczeniowych. Subskrypcje CSP są aktywne lub wstrzymane (albo w pełni usunięte).

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Aby wstrzymać nowe subskrypcje handlowe lub ponownie aktywować wstrzymane nowe subskrypcje handlowe, utwórz żądanie obsługi i skontaktuj się z pomocą techniczną.


### <a name="cancel-a-subscription"></a>Anulowanie subskrypcji

Możesz anulować oparte na licencjach subskrypcje SaaS od zewnętrznych wydawców isv w ramach Partner Center [platformy handlowej.](csp-commercial-marketplace-overview.md) Dopóki anulujesz subskrypcję w okresie anulowania, otrzymasz pełny zwrot kosztów.

W przypadku ofert isv(isv) rozliczanych miesięcznie:

- Jeśli anulujesz zamówienie po upływie mniej niż 24 godzin, otrzymasz pełne środków na następnej fakturze.

- Jeśli anulujesz zamówienie później niż 24 godziny, anulowanie zostanie zaplanowane podczas odnawiania.

W przypadku ofert rozliczanych rocznie:

- Jeśli anulujesz zamówienie po upływie mniej niż 14 dni, otrzymasz pełne środków na następnej fakturze.

- Jeśli anulujesz zamówienie później niż 14 dni, anulowanie zostanie zaplanowane podczas odnawiania.

Po upływie tych okresów nie będzie już dostępna opcja anulowania subskrypcji.

> [!NOTE]
> Oparte na użyciu i mierzone usługi innych firm isv (które na przykład korzystają z maszyn wirtualnych lub kontenerów) nie kwalifikują się do zwrotu. Usługi oparte na użyciu można anulować jako metodę anulowania. Ponieważ opłaty są naliczane po użyciu, te usługi nie kwalifikują się do zwrotu.

Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Znajdź subskrypcję, którą chcesz anulować.

4. W kolumnie **Stan** wybierz pozycję **Anuluj.** Następnie **prześlij** zmiany.

5. Jeśli zostanie wyświetlone okno dialogowe, wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij.**

6. Aby potwierdzić anulowanie, wybierz pozycję **Tak, anuluj .**

> [!NOTE]
> Możesz również anulować subskrypcję usługi Azure Marketplace przy użyciu interfejsów API. Aby to zrobić, zobacz [Anulowanie Azure Marketplace subskrypcji.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

## <a name="suspend-or-cancel-a-new-commerce-subscription"></a>Wstrzymywanie lub anulowanie nowej subskrypcji handlowej

### <a name="suspend-a-new-commerce-subscription"></a>Wstrzymywanie nowej subskrypcji handlowej

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

W przypadku braku płatności od klienta, czasami nazywanego "scenariuszem duplikowania", partnerzy mogą wstrzymać i wznowić swoją subskrypcję, aby natychmiast zablokować dostęp klienta do usług subskrypcji.

Partnerzy mogą wstrzymywać i wznawiać subskrypcję w dowolnym momencie bez anulowania. Jednak rozliczenia partnerów są nadal w trakcie zawieszania. 

Wstrzymanie subskrypcji klienta spowoduje wyłączenie możliwości logowania się i korzystania z usług do czasu wznowienia subskrypcji. Wszystkie dane związane z subskrypcją zostaną usunięte, chyba że subskrypcja zostanie ponownie aktywowana w ciągu 90 dni.

Subskrypcję można wstrzymać przy użyciu Partner Center:

1. Przejdź do strony subskrypcji klienta i wybierz subskrypcję, która ma być wstrzymywana.

2. Wybierz przycisk **radiowy Wstrzymaj.**

3. W podręcznym oknie dialogowym wybierz przycisk **OK.**

4. Subskrypcja będzie teraz w stanie wstrzymania, a partner nadal będzie rozliczany za subskrypcję.

Wsuskanie jest odwracalne Partner Center interfejsu użytkownika lub interfejsów API, które natychmiast przywrócią dostęp klienta do usług subskrypcji.

> [!IMPORTANT]
> Wstrzymanie subskrypcji spowoduje wyłączenie wszystkich ustawień automatycznego odnawiania i usunięcie wszelkich istniejących zaplanowanych zmian. Wstrzymanie subskrypcji będzie miało wpływ tylko na dostęp do usługi klienta, a rozliczenia partnera będą nadal w stanie wstrzymania.

### <a name="cancel-a-new-commerce-subscription"></a>Anulowanie nowej subskrypcji handlowej

> [!Note] 
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

W przypadku nowych ofert handlowych partnerzy mogą anulować swoją subskrypcję z proporcjonalnym zwrotem w ciągu **pierwszych 72** godzin na dowolny okres (opłata obliczona **codziennie).**  

Po upływie 72 godzin anulowanie nie będzie już dostępne, a partner będzie rozliczany przez cały okres, nawet jeśli klient przestanie płacić lub korzysta z subskrypcji (dotyczy dowolnego planu rozliczeniowego).

Po zakończeniu anulowania klient natychmiast utraci dostęp do usługi i nie będzie można przywrócić usługi. Nie będzie można odzyskać stanu subskrypcji.  

Jeśli licencje są dodawane w połowie okresu, te same zasady dotyczące 72 godzin mają zastosowanie do każdej redukcji dodatkowych licencji. Zmniejszenie liczby dodanych licencji musi odbywać się za **pośrednictwem żądań pomocy technicznej.**

## <a name="subscription-renewals"></a>Odnowienia subskrypcji

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji. W [przypadku subskrypcji produktów platformy handlowej](csp-commercial-marketplace-overview.md)lub nowych subskrypcji handlowych możesz opcjonalnie zdecydować, aby nie odnawiać subskrypcji automatycznie.

Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji platformy handlowej lub nowych subskrypcji handlowych:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Wybierz pozycję **Subskrypcje**. Zawiera listę wszystkich subskrypcji opartych na licencjach zakupionych dla klienta.

4. W kolumnie **Subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.

5. Na stronie szczegółów subskrypcji znajdź sekcję **Stan** i usuń zaznaczenie pola **Automatycznie odnawiaj.**

6. Wybierz pozycję **Prześlij**.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Zarządzanie nowymi odnowieniami handlowymi za pomocą zaplanowanych zmian

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Niektóre zmiany w subskrypcjach mogą nastąpić tylko na końcu okresu. Te zmiany można zaplanować tak, aby były wygodnie stosowane na końcu terminu. Przykłady zmian, które należy zaplanować:

- redukcja licencji
- Zmiany w okresie rozliczeniowym
- Zmiany częstotliwości rozliczeń

Inne zmiany, takie jak uaktualnienia lub zwiększenie licencji, można zastosować w okresie.

Zmiany harmonogramu zostaną wprowadzone podczas odnawiania, gdy subskrypcja zostanie odnowiona na następny okres.

Wymagania wstępne dotyczące zaplanowanych zmian:

- Subskrypcja jest aktywna 
- Automatyczne odnawianie jest wł.
- SKU musi kwalifikować się do uaktualnienia

Aby zaplanować nową zmianę, która ma nastąpić podczas odnawiania:

1. Zaloguj się do pulpitu Partner Center nawigacyjnego.

2. Wybierz **klienta** z listy klientów.

3. Wybierz subskrypcję, którą chcesz zarządzać.

4. Wybierz **pozycję Zarządzaj odnowieniami.**

5. Wybierz inną zmianę wartości dla wartości SKU, ilości, okresu lub częstotliwości rozliczeń:

   - **Bieżąca** to bieżąca wartość subskrypcji

   - **Zmiana** na to ostatnia zapisana wartość, która ma zostać zastosowana podczas odnawiania nowej subskrypcji

6. Wybierz pozycję **Prześlij**.

7. Zmiany zostaną wprowadzone podczas odnawiania.

Partnerzy mogą uzyskać dostęp **do zarządzania odnowieniami,** aby wyświetlić, zaktualizować lub usunąć istniejącą zaplanowaną zmianę.

> [!NOTE]
> - Domyślnie wersje próbne są konwertowane na płatną równoważną wersję SKU na koniec okresu próbnego.
> - W przypadku zaplanowanych uaktualnień sku, jeśli liczba licencji nie zmieni się, ponowne przypisanie licencji użytkownika będzie wykonywane automatycznie. W przeciwnym razie będzie trzeba to zrobić ręcznie.
> - Zapisane zaplanowane zmiany są usuwane, jeśli w subskrypcji zostaną wprowadzone aktualizacje krótkoterminowe.

Zapisane zaplanowane zmiany są usuwane, gdy zostaną wprowadzone następujące zmiany krótkoterminowe:  

- Automatyczne odnawianie jest wyłączone 
- Ilość została zmieniona 
- Subskrypcja została anulowana 
- Uaktualniono sku 
- Konwertowanie wersji próbnej 

## <a name="upgrades-in-new-commerce-subscriptions"></a>Uaktualnienia w nowych subskrypcjach handlowych

W przypadku nowego handlu uaktualnienie oznacza przejście z jednej płatnej subskrypcji do innej płatnej subskrypcji. Nowe uaktualnienia z płatnego do płatnego handlu umożliwiają klientowi natychmiastowe uaktualnienie z bieżącej do bieżącej wersji SKU z dodanymi usługami. 

Partnerzy mogą wybrać subskrypcję, do której mają zostać uaktualnione podczas konfigurowania liczby licencji. Partnerzy mogą wybrać **nową** subskrypcję lub wybrać **istniejącą** subskrypcję, jeśli kwalifikuje się ona do uaktualnienia. 

Uaktualnienia mogą mieć dwa typy: **pełne i** **częściowe.**

> [!NOTE]
> - Uaktualnienia można zaplanować na koniec okresu lub mogą być inicjowane w połowie okresu.
> - Zainicjowanie uaktualnienia w połowie okresu spowoduje usunięcie istniejących zaplanowanych uaktualnień.
> - Uaktualnienia można inicjować tylko z subskrypcji w **stanie** Aktywny.

### <a name="full-upgrades"></a>Pełne uaktualnienia

Pełne uaktualnienie to uaktualnienie w miejscu, co oznacza, że wszystkie lub więcej licencji jest uaktualnianych. W takim przypadku identyfikator subskrypcji pozostaje taki sam, a licencje są przypisywane automatycznie. Jednak w przypadku, gdy klient kupił już docelową skuwkę u innego partnera lub kanału w starszej wersji, konieczne będzie ręczne przypisanie. Jeśli jest wymagane ręczne przypisanie, partner zobaczy na stronie Partner Center komunikat ostrzegawczy informujący o konieczności ręcznego przypisania licencji. 

### <a name="partial-upgrades"></a>Uaktualnienia częściowe

Częściowe uaktualnienia umożliwiają partnerowi wyznaczenie niektórych licencji z jednej sku na inną. Poprzednia funkcja uaktualniania w tradycyjnych subskrypcjach opartych na licencjach umożliwiała uaktualnienie tylko wszystkich licencji. Nowy handel umożliwia partnerowi przenoszenie niektórych licencji w dogodnym dla nich czasie. Daje to partnerowi większą kontrolę nad zarządzaniem uaktualnieniami, umożliwiając mu przeniesienie niektórych użytkowników do nowej wersji SKU bez przenoszenia ich wszystkich.

Szczegóły częściowego uaktualnienia:

- Zdefiniowana jako częściowa, jeśli liczba licencji uaktualnienia jest mniejsza niż początkowa subskrypcja.
- Nowa subskrypcja utworzona podczas częściowego uaktualniania będzie mieć takie same daty zakończenia okresu jak subskrypcja, z której pochodzi uaktualnienie.

## <a name="increasing-and-reducing-licenses-in-new-commerce-subscriptions"></a>Zwiększanie i zmniejszanie liczby licencji w nowych subskrypcjach handlowych

Liczbę licencji dla subskrypcji  można zwiększyć w dowolnym momencie, a korekty rozliczeń zostaną odzwierciedlone w następnym pliku faktury i uzgodnień. 

Liczbę licencji w ramach subskrypcji można **zmniejszyć:**
- tylko w ciągu pierwszych 72 godzin od pierwszego zamówienia subskrypcji lub **jego odnowienia.** 
- za pośrednictwem pomocy technicznej klienta w ciągu 72 godzin w przypadku licencji **dodanych w połowie roku**

Zmniejszenie liczby licencji w ciągu pierwszych 72 godzin okresu subskrypcji (po początkowym zakupie lub odnowieniu) można dokonać za pośrednictwem samoobsługi w usłudze Partner Center lub za pośrednictwem interfejsu API.

Zmniejszenie liczby licencji dodanych w połowie roku można wykonać tylko za pośrednictwem działu obsługi klienta w ciągu pierwszych 72 godzin.

W obu przypadkach redukcji licencji zostanie zwrócona pełna kwota pomniejszona o proporcjonalną kwotę za dni, w których została użyta subskrypcja   **(proracja** obliczana codziennie). 

Jeśli od momentu zamówienia subskrypcji lub dodania dodatkowych licencji upłynęło ponad **72** godziny, nie można zmniejszyć liczby licencji do następnego okna anulowania podczas odnawiania. 

## <a name="switching-billing-plans"></a>Przełączanie planów rozliczeniowych

Partner może elastycznie zmieniać swój plan rozliczeniowy i okres rozliczeniowy. Mogą oni również przełączać się tylko w połowie okresu rozliczeniowego bez konieczności resetowania okresu rozliczeniowego.

### <a name="just-changing-billing-frequency-scheduled-change"></a>Zmiana częstotliwości rozliczeń (zaplanowana zmiana)

Partnerzy mogą zmienić tylko plan rozliczeniowy za pośrednictwem Partner Center w kilku krokach, co zostanie wprowadzone w następnym cyklu rozliczeniowym:

1. Przejdź do strony subskrypcji klienta i wybierz subskrypcję, która chcesz zmienić.

2. Wybierz link **Zarządzaj częstotliwością rozliczeń.**

3. Zostanie otwarty panel boczny z bieżącą częstotliwością rozliczeń i listą rozwijaną zawierającą opcje zmiany częstotliwości.

4. Po wybraniu nowej wartości nowe zmiany rozliczeń zostaną wprowadzone w następnym **cyklu** rozliczeniowym (NIE jest to zmiana natychmiastowa).

### <a name="changing-billing-frequency-along-with-billing-term-and-other-fields-immediate-change"></a>Zmiana częstotliwości rozliczeń wraz z okresem rozliczeniowym i innymi polami (zmiana natychmiastowa)

Partner może również zmienić częstotliwość rozliczeń wraz z okresem rozliczeniowym i innymi polami za pośrednictwem Partner Center, co spowoduje natychmiastową zmianę:

1. Przejdź do strony subskrypcji klienta i wybierz subskrypcję, która chcesz zmienić.

2. Zmień okres trwania, zaznaczac opcję z listy rozwijanej. Spowoduje to otwarcie kolejnej listy rozwijanej w celu zmiany częstotliwości rozliczeń.

3. Wybierz inną częstotliwość rozliczeń z listy rozwijanej.

4. Po w związku z wprowadzonymi zmianami i kliknięciu przycisku Prześlij nowe zmiany rozliczeń zostaną wprowadzone **natychmiast.**

## <a name="next-steps"></a>Następne kroki

- [Kupowanie produktów komercyjnej platformy handlowej dla klientów](csp-commercial-marketplace-purchase.md)

- [Zarządzanie produktami platformy handlowej dla klientów](csp-commercial-marketplace-manage.md)

- [Omówienie komercyjnej platformy handlowej](csp-commercial-marketplace-overview.md)
