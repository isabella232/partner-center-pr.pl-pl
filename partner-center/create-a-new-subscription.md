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
ms.openlocfilehash: e3696ea77d6b073e625e64425cf7764194acfd15
ms.sourcegitcommit: 1e616b52d55eff41d67a081ba3f4a8370a49e027
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/29/2021
ms.locfileid: "129191480"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Tworzenie, zawieszanie lub anulowanie subskrypcji klientów

**Dotyczy:** Partner Center | Partner Center dla Microsoft Cloud for US Government

**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży

Po utworzeniu rekordu klienta w katalogu Partner Center można sprzedawać im subskrypcje produktów w katalogu. Dotyczy to produktów publikowanych przez firmę Microsoft oraz produktów SaaS (Software as a Service) publikowanych przez niezależnych dostawców oprogramowania (ISV) innych firm na [platformie handlowej.](https://azuremarketplace.microsoft.com/marketplace)

Niektóre oferty są ograniczone do jednej subskrypcji na klienta. Aby wyświetlić listę ofert ograniczonych, odwiedź stronę Partner Center Cennik i oferty.

> [!IMPORTANT]
> Jako partner w programie CSP  możesz kupować oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center. Oznacza to, że  możesz kupić dowolną opartą na licencjach lub mierzoną [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ofertę **SaaS,** która została Ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp. Aby zakupić inne, komercyjne oferty platformy handlowej od isvs (np. ofert opartych na użyciu obejmujących aplikacje platformy Azure, kontenery lub maszyny wirtualne) lub zarządzać nimi, musisz przejść do witryny [Azure Portal](https://portal.azure.com/).

> [!NOTE]
> Wszystkie daty i godziny w Partner Center są podane w standardzie czasu uniwersalnego (UTC). Może się to różnić nawet o 24 godziny od czasu lokalnego.

## <a name="create-a-new-subscription"></a>Tworzenie nowej subskrypcji

> [!NOTE]
> Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych, zobacz [Getting around Partner Center (Poruszanie się po Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off)).

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Na [pulpicie Partner Center nawigacyjnym](https://partner.microsoft.com/dashboard)wybierz kafelek **Klienci,** a następnie wybierz klienta z listy Klienci.

2. Wybierz **pozycję Dodaj subskrypcję.** Na **karcie Usługi online** będą wyświetlane wszystkie dostępne oferty SaaS w witrynie Marketplace.

3. Aby wyświetlić tylko niektóre typy subskrypcji, należy dokonać wyboru w dostępnych filtrach:
   - **Publisher:** wybierz pozycję **Firma Microsoft,** aby  wyświetlić tylko oferty firmy Microsoft lub partnera, aby wyświetlić produkty platformy handlowej opublikowane przez isvs.
   - **Typ rozliczeń:** wybierz typ rozliczeń subskrypcji, których chcesz użyć: **Licencja** lub **Użycie.** Zobacz [Rozliczenia oparte na licencjach,](license-based-billing.md) aby uzyskać informacje, które pomogą Ci wybrać miesięczną i roczną częstotliwość rozliczeń.
   - **Kategoria:** wybierz **Enterprise,** **Małe firmy** lub Wersja **próbna.** Aby uzyskać informacje o subskrypcjach wersji próbnej, zobacz [Temat Oferty dla klientów wersji próbnych produktów firmy Microsoft.](offer-your-customers-trials-of-microsoft-products.md)

4. Wybierz subskrypcje produktów, które chcesz kupić dla klienta. Produkty, które widzisz, zależą od typu segmentu klientów (edukacja, administracja rządowa itp.) i zastosowanych filtrów. Niektóre oferty wyświetlane w witrynie Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera CSP. Może to być spowodowane:
   - Klient ma już subskrypcję tego produktu i ma tylko jedną z nich
   - Subskrypcja klienta może zostać wstrzymana (w tym przypadku możesz ponownie aktywować subskrypcję zamiast kupować nową).
   - W przypadku ofert SaaS dla isv może być kilka powodów, dla których oferta nie jest dostępna do zakupu: isv may not support the customer's billing country or region; IsV may have chosen not make the offer available through the CSP program; lub, isv may have made the offer [exclusive to only](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) certain CSP partners. Oferta isv (isv) może również nie być możliwość transakcji za pośrednictwem Partner Center (na przykład kontenerów lub niektórych ofert opartych na użyciu).  

5. Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby) i wybierz **pozycję Dodaj do koszyka.**

6. Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj zamówienie.

7. Po przejrzenia zamówień i przygotowaniu się do zakupu tych subskrypcji wybierz pozycję **Kup**.

8. Po zakupie subskrypcji dla klienta wystąpią następujące zdarzenia:

    - Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji na stronie **Subskrypcje tego** klienta. W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.

    **W przypadku subskrypcji SAAS isv (opartych na licencjach i mierzonych):**
    - Otrzymasz link do witryny wydawcy isv. Ten link powinien ułatwić ukończenie wdrażania lub konfigurowania konta subskrypcji klienta.

    > [!NOTE]
    > Ani Ty, ani Klient nie otrzymacie wiadomości e-mail z instrukcjami dotyczącymi ukończenia procesu skonfigurowania/aprowizowania konta dla tego typu subskrypcji isv).

    - Jeśli Twoja subskrypcja zawiera 30-dniową bezpłatną wersję próbną, bezpłatny okres próbny zostanie zastosowany automatycznie. Jako partner w programie CSP nie możesz zrezygnować z okresu bezpłatnej wersji próbnej ofert zakupu dla klientów. Po zakończeniu okresu bezpłatnej wersji próbnej okres subskrypcji rozpocznie się, a subskrypcja zostanie przekształcona w stan płatny. Subskrypcja zostanie następnie automatycznie odnowiona zgodnie z tym samym harmonogramem.

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Na Partner Center [nawigacyjnym](https://partner.microsoft.com/dashboard)wybierz pozycję **Klienci,** a następnie wybierz klienta z listy Klienci.

2. Wybierz **pozycję Dodaj subskrypcję.** Na **karcie Usługi online** będą wyświetlane wszystkie dostępne oferty SaaS w witrynie Marketplace.

3. Aby wyświetlić tylko niektóre typy subskrypcji, należy dokonać wyboru w dostępnych filtrach:
   - **Publisher:** wybierz pozycję **Firma Microsoft,** aby  wyświetlić tylko oferty firmy Microsoft lub partnera, aby wyświetlić produkty platformy handlowej opublikowane przez isvs.
   - **Typ rozliczeń:** wybierz typ rozliczeń subskrypcji, których chcesz użyć: **Licencja** lub **Użycie.** Zobacz [Rozliczenia oparte na licencjach,](license-based-billing.md) aby uzyskać informacje, które pomogą Ci wybrać miesięczną i roczną częstotliwość rozliczeń.
   - **Kategoria:** wybierz **Enterprise,** **Małe firmy** lub Wersja **próbna.** Aby uzyskać informacje o subskrypcjach wersji próbnej, zobacz [Temat Oferty dla klientów wersji próbnych produktów firmy Microsoft.](offer-your-customers-trials-of-microsoft-products.md)

4. Wybierz subskrypcje produktów, które chcesz kupić dla klienta. Produkty, które widzisz, zależą od typu segmentu klientów (edukacja, administracja rządowa itp.) i zastosowanych filtrów. Niektóre oferty wyświetlane w witrynie Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera CSP. Może to być spowodowane:
   - Klient ma już subskrypcję tego produktu i ma tylko jedną z nich
   - Subskrypcja klienta może zostać wstrzymana (w tym przypadku możesz ponownie aktywować subskrypcję zamiast kupować nową).
   - W przypadku ofert SaaS dla isv może być kilka powodów, dla których oferta nie jest dostępna do zakupu: isv may not support the customer's billing country or region; IsV may have chosen not make the offer available through the CSP program; lub, isv may have made the offer [exclusive to only](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) certain CSP partners. Oferta isv (isv) może również nie być możliwość transakcji za pośrednictwem Partner Center (na przykład kontenerów lub niektórych ofert opartych na użyciu).  

5. Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby) i wybierz **pozycję Dodaj do koszyka.**

6. Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj zamówienie.

7. Po przejrzenia zamówień i przygotowaniu się do zakupu tych subskrypcji wybierz pozycję **Kup**.

8. Po zakupie subskrypcji dla klienta wystąpią następujące zdarzenia:

    - Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji na stronie **Subskrypcje tego** klienta. W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.

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

Możliwość zakupu dodatków za pośrednictwem usługi Partner Center jest dostępna tylko dla dostawców rozliczanych bezpośrednio i pośrednich.
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
> Subskrypcje CSP nie mają wygasłego okresu (w jaki działają subskrypcje bezpośrednie w sieci Web), w którym usługi nadal działają, ale subskrypcja nie generuje żadnych opłat rozliczeniowych. Subskrypcje CSP są aktywne lub wstrzymane (albo całkowicie usunięte).

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Aby wstrzymać nowe subskrypcje handlowe lub ponownie aktywować wstrzymane nowe subskrypcje handlowe, utwórz żądanie obsługi i skontaktuj się z pomocą techniczną.


### <a name="cancel-a-subscription"></a>Anulowanie subskrypcji

Subskrypcje SaaS oparte na licencjach można anulować od zewnętrznych wydawców isV w ramach platformy Partner Center [komercyjnej.](csp-commercial-marketplace-overview.md) Dopóki anulujesz subskrypcję w okresie anulowania, otrzymasz pełny zwrot kosztów.

W przypadku ofert isv (isv) rozliczanych miesięcznie:

- Jeśli anulujesz zamówienie po upływie mniej niż 24 godzin, otrzymasz pełne środków na następnej fakturze.

- Jeśli anulujesz subskrypcję po upływie 24 godzin od złożonego zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.

W przypadku ofert rozliczanych rocznie:

- Jeśli anulujesz zamówienie po upływie mniej niż 14 dni, otrzymasz pełne środków na następnej fakturze.

- Jeśli anulujesz subskrypcję później niż 14 dni od zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.

Po zakończeniu tych okresów nie będzie już dostępna opcja anulowania subskrypcji.

> [!NOTE]
> Oparte na użyciu i mierzone usługi innych firm isv (na przykład które używają maszyn wirtualnych lub kontenerów) nie kwalifikują się do zwrotu. Usługi oparte na użyciu można anulować. Ponieważ opłaty są naliczane po użyciu, te usługi nie kwalifikują się do zwrotu kosztów.

Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Znajdź subskrypcję, którą chcesz anulować.

4. W kolumnie **Stan** wybierz pozycję **Anuluj.** Następnie **prześlij** zmiany.

5. Jeśli zostanie wyświetlone okno dialogowe, wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij.**

6. Aby potwierdzić anulowanie, wybierz pozycję **Tak, anuluj .**

> [!NOTE]
> Możesz również anulować subskrypcję usługi Azure Marketplace przy użyciu interfejsów API. Aby to zrobić, zobacz [Anulowanie subskrypcji Azure Marketplace subskrypcji.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="cancel-a-new-commerce-subscription"></a>Anulowanie nowej subskrypcji handlowej

> [!Note] 
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

W przypadku nowych ofert handlowych możesz anulować subskrypcję w dowolnym momencie przed okresem zobowiązania. Po anulowaniu subskrypcji klient natychmiast utraci dostęp do usługi. Nie można przywrócić dostępu po anulowaniu. Następujące opcje anulowania są dostępne dla partnera po zakupie subskrypcji: 

- W ciągu 24 godzin od daty rozpoczęcia subskrypcji: możesz anulować całą subskrypcję w ciągu pierwszych 24 godzin, aby uzyskać pełny zwrot.  
- W ciągu 30 dni od daty rozpoczęcia subskrypcji: możesz anulować całą subskrypcję w ciągu pierwszych 30 dni. Za dni, w których została użyta subskrypcja, zostanie zwrócona pełna kwota pomniejszona o proporcjonalną kwotę.
- Po upływie 30 dni od daty rozpoczęcia subskrypcji: nie można anulować subskrypcji.

### <a name="pause-and-resume-a-new-commerce-subscription"></a>Wstrzymywanie i wznawianie nowej subskrypcji handlowej

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

W przypadku braku płatności od klienta, czasami nazywanego "scenariuszem monitowania", partnerzy mogą wstrzymać i wznowić subskrypcję, aby natychmiast zablokować klientowi dostęp do usług subskrypcji.

Wstrzymanie subskrypcji klienta spowoduje wyłączenie możliwości logowania się i korzystania z jego usług do czasu wznowienia subskrypcji.

Subskrypcję można wstrzymać przy użyciu Partner Center:

1. Przejdź do strony subskrypcji klienta i wybierz subskrypcję, która ma być wstrzymana.

2. Wybierz przycisk **radiowy Wstrzymaj.**

3. W podręcznym oknie dialogowym wybierz przycisk **OK.**

4. Subskrypcja będzie teraz w stanie wstrzymania, a partner nadal będzie rozliczany za subskrypcję.

Wsłuchianie jest odwracalne Partner Center interfejsu użytkownika lub interfejsu API, co spowoduje natychmiastowe przywrócenie dostępu klienta do usług subskrypcji.

> [!IMPORTANT]
> Wstrzymanie subskrypcji spowoduje wyłączenie wszystkich ustawień automatycznego odnawiania i usunięcie wszelkich istniejących zaplanowanych zmian. Wstrzymanie subskrypcji będzie miało wpływ tylko na dostęp do usługi klienta, a rozliczenia partnera będą nadal w stanie wstrzymania.

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription-or-a-new-commerce-subscription"></a>Wybierz, czy chcesz automatycznie odnowić subskrypcję platformy handlowej, czy nową subskrypcję handlową

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji. W [przypadku subskrypcji produktów komercyjnej](csp-commercial-marketplace-overview.md)platformy handlowej lub nowych subskrypcji handlowych możesz opcjonalnie zdecydować, aby nie odnawiać subskrypcji automatycznie.

Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji platformy handlowej lub nowych subskrypcji handlowych:

Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji platformy handlowej:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Wybierz pozycję **Subskrypcje**. Zawiera listę wszystkich subskrypcji opartych na licencjach zakupionych dla klienta.

4. W kolumnie **Subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.

5. Na stronie szczegółów subskrypcji znajdź **sekcję Stan** i usuń zaznaczenie pola **Automatycznie odnawiaj.**

6. Wybierz pozycję **Prześlij**.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Zarządzanie nowymi odnowieniami handlu przy użyciu zaplanowanych zmian

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Niektóre zmiany w subskrypcjach mogą wystąpić tylko na końcu terminu. Te zmiany można zaplanować tak, aby były wygodnie stosowane na końcu terminu. Przykłady zmian, które należy zaplanować:

- Obniżanie poziomu SKU
- Redukcje liczby miejsc
- Zmiany różnych terminów
- Zmiany częstotliwości rozliczeń

Inne zmiany, takie jak uaktualnienia lub zwiększenie miejsca, można zastosować w trakcie okresu.

Zaplanowanie zmian nastąpi podczas odnawiania, gdy subskrypcja zostanie odnowiona na następny okres.

Wymagania wstępne dotyczące zaplanowanych zmian:

- Subskrypcja jest aktywna 
- Automatyczne odnawianie jest wł.
- SKU musi kwalifikować się do uaktualnienia zaplanowanych uaktualnień

Aby zaplanować nową zmianę podczas odnawiania:

1. Zaloguj się do pulpitu Partner Center nawigacyjnego.

2. Wybierz **klienta** z listy klientów.

3. Wybierz subskrypcję, którą chcesz zarządzać.

4. Wybierz **pozycję Zarządzaj odnowieniami.**

5. Wybierz inną wartość Zmień wartość dla SKU, ilości, okresu lub częstotliwości rozliczeń:

   - **Bieżąca** to bieżąca wartość subskrypcji

   - **Zmień** wartość na to ostatnia zapisana wartość, którą chcesz zastosować podczas odnawiania nowej subskrypcji

6. Wybierz pozycję **Prześlij**.

7. Zmiany zostaną wprowadzone podczas odnawiania.

Partnerzy mogą uzyskać dostęp **do zarządzania odnowieniami,** aby wyświetlić, zaktualizować lub usunąć istniejące zaplanowane zmiany.

> [!NOTE]
> - Wersje próbne są domyślnie konwertowane na płatną sku na koniec okresu. 
> - W przypadku zaplanowanych uaktualnień/obniżania poziomu licencji użytkownika ponowne przypisanie musi być wykonywane ręcznie.
> - Zapisane zaplanowane zmiany są usuwane, jeśli w subskrypcji zostaną wprowadzone następujące aktualizacje w połowie okresu.

### <a name="partial-upgrades-in-new-commerce-subscriptions"></a>Częściowe uaktualnienia w nowych subskrypcjach handlowych

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Częściowe uaktualnienia umożliwiają partnerowi wyznaczenie niektórych licencji z jednej sku na inną. Poprzednia funkcja uaktualniania w tradycyjnych subskrypcjach opartych na licencjach umożliwiała uaktualnienie tylko wszystkich licencji. Nowy handel umożliwia partnerowi przenoszenie niektórych licencji w dogodnym dla nich czasie. Daje to partnerowi większą kontrolę nad zarządzaniem uaktualnieniami, umożliwiając mu przeniesienie niektórych użytkowników do nowej wersji SKU bez przenoszenia ich wszystkich.

Częściowe uaktualnienia można zaplanować na koniec okresu lub mogą być inicjowane w połowie okresu.

Szczegóły częściowego uaktualnienia:

- Zdefiniowana jako częściowa, jeśli liczba licencji uaktualnienia jest inna niż początkowa subskrypcja.
- Inicjowanie uaktualnień w połowie okresu spowoduje usunięcie istniejących zaplanowanych uaktualnień.
- Uaktualnienia można inicjować tylko z subskrypcji w **stanie Aktywny.**
- Nowa subskrypcja utworzona podczas uaktualniania będzie miała takie same daty zakończenia jak subskrypcja, z której pochodzi uaktualnienie.

Partnerzy mogą uzyskać dostęp do subskrypcji, do której mają zostać uaktualnione, podczas konfigurowania liczby licencji i subskrypcji, do której mają zostać uaktualnione. Partnerzy mogą wybrać **nową subskrypcję** lub wybrać istniejącą subskrypcję.

## <a name="next-steps"></a>Następne kroki

- [Kupowanie produktów komercyjnej platformy handlowej dla klientów](csp-commercial-marketplace-purchase.md)

- [Zarządzanie produktami platformy handlowej dla klientów](csp-commercial-marketplace-manage.md)

- [Omówienie komercyjnej platformy handlowej](csp-commercial-marketplace-overview.md)
