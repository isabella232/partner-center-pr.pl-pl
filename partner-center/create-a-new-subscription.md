---
title: Tworzenie subskrypcji klientów w centrum partnerskim
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak sprzedawać subskrypcje klientów do produktów opublikowanych przez firmę Microsoft, a także produktów SaaS opublikowanych przez niezależnych dostawców oprogramowania.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 85a40974557817825d58246c2c010c7cf8a6a5e1
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038884"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Tworzenie, zawieszanie lub anulowanie subskrypcji klientów

**Dotyczy**

- Centrum partnerskie
- Centrum partnerskie Microsoft Cloud for US Government
- Partnerzy CSP

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Administrator globalny
- Agent pomocy technicznej
- Agent sprzedaży

Po utworzeniu rekordu klienta w centrum partnerskim możesz sprzedawać te subskrypcje do produktów w katalogu. Obejmuje to produkty opublikowane przez firmę Microsoft, a także produkty SaaS (Software as a Service) opublikowane przez niezależnych dostawców oprogramowania (ISV) innych firm do [komercyjnej witryny Marketplace](https://azuremarketplace.microsoft.com/marketplace).

Niektóre oferty są ograniczone do jednej subskrypcji na klienta. Aby wyświetlić listę ofert, które są ograniczone, odwiedź stronę ceny i oferty Centrum partnerskiego.

>[!IMPORTANT]
> Jako partner w programie CSP można zakupić subskrypcje SaaS **oparte na licencjach** lub **naliczanych** od niezależnych dostawców oprogramowania w centrum partnerskim. Oznacza to, że możesz zakupić dowolną ofertę **opartą na licencji** lub **naliczaną** SaaSą oferowaną przez wydawcę niezależnego dostawcy oprogramowania, w tym [wyłączne oferty](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , do których masz dostęp. Aby kupić inne, komercyjne oferty rynkowe z niezależnych dostawców oprogramowania (na przykład oferty oparte na użyciu dotyczące aplikacji platformy Azure, kontenerów lub maszyn wirtualnych) i zarządzać nimi, musisz przejść do [Azure Portal](https://portal.azure.com/).

## <a name="create-a-new-subscription"></a>Utwórz nową subskrypcję

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).

2. W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.

3. Wybierz pozycję **Dodaj subskrypcję**. Na karcie **usługi online** zostaną wyświetlone wszystkie dostępne oferty SaaS w portalu Marketplace.

4. Aby wyświetlić tylko niektóre typy subskrypcji, należy wybrać dostępne filtry:
   - **Wydawca**: Wybierz **firmę Microsoft** , aby wyświetlić tylko oferty od firmy Microsoft lub **partnera** , aby zobaczyć komercyjne produkty Marketplace opublikowane przez niezależnych dostawców oprogramowania.
   - **Typ rozliczeń**: Wybierz typ rozliczania subskrypcji, którego chcesz użyć: **licencja** lub **użycie**. Informacje, które pomogą w wyborze miesięcznej i rocznej częstotliwości rozliczania, można znaleźć na stronie [rozliczeń opartych na licencji](license-based-billing.md) .
   - **Kategoria**: wybierz pozycję **Enterprise**, **mała firma** lub **wersja próbna**. Aby uzyskać informacje na temat subskrypcji wersji próbnej, zobacz artykuł [oferujący klientom wersje próbne produktów firmy Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Wybierz subskrypcje produktu, które chcesz kupić dla klienta. Widoczne produkty zależą od typu segmentu klienta (edukacja, rząd itp.) oraz filtrów, które zostały zastosowane. Niektóre oferty prezentowane w portalu Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera dostawcy usług kryptograficznych. Może to być spowodowane:

   - Klient ma już subskrypcję tego produktu i jest dozwolony tylko jeden

   - Subskrypcja klienta mogła zostać zawieszona (w tym przypadku można ponownie aktywować subskrypcję zamiast zakupić nową).

   - W przypadku ofert SaaS oferowanych przez niezależnych dostawców oprogramowania może istnieć kilka powodów, dla których oferta nie jest dostępna do zakupu: dostawca niezależnego dostawcy oprogramowania może nie obsługiwać kraju lub regionu rozliczeniowego klienta. Dostawca niezależnego dostawcy oprogramowania mógł zrezygnować z udostępnienia oferty za pomocą programu CSP. niezależny dostawca oprogramowania może [również oferować ofertę wyłącznie dla](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) niektórych partnerów CSP. Oferta niezależnego dostawcy oprogramowania może być również nieobsługiwana w centrum partnerskim (na przykład w przypadku kontenerów lub niektórych ofert opartych na użyciu).  

6. Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby), a następnie wybierz pozycję **Dodaj do koszyka**.

7. Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj swoją kolejność.

8. Po przejrzeniu zamówień i przygotowaniu do zakupu tych subskrypcji wybierz pozycję **Kup**.

9. Po zakupieniu subskrypcji dla klienta zostaną wykonane następujące czynności:

    - Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji ze strony **subskrypcji** tego klienta. W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.

    **W przypadku subskrypcji niezależnego dostawcy oprogramowania (SaaS):**
    - Zostanie wyświetlony link do witryny wydawcy niezależnego dostawcy oprogramowania. Ten link powinien pomóc w zakończeniu konfiguracji wdrożenia lub konta subskrypcji klienta.
      
    >[!NOTE]
    > Klient nie otrzyma wiadomości e-mail z instrukcjami dotyczącymi ukończenia konfigurowania lub aprowizacji dla tego typu subskrypcji niezależnego dostawcy oprogramowania.

    - Jeśli subskrypcja obejmuje 30-dniową bezpłatną wersję próbną, zostanie automatycznie zastosowana bezpłatna wersja próbna. Jako partner w programie CSP nie można zrezygnować z bezpłatnego okresu próbnego w przypadku ofert zakupu dla klientów. Po zakończeniu okresu bezpłatnej wersji próbnej subskrypcja zostanie rozpoczęta i subskrypcja zostanie przekonwertowana na stan płatny. Subskrypcja będzie następnie odnawiana ponownie zgodnie z tym samym harmonogramem.
   
## <a name="update-subscriptions-with-add-ons"></a>Aktualizowanie subskrypcji z dodatkami 

Aby kupić dodatek, klient musi mieć aktywną subskrypcję podstawową.  Nie można kupować dodatków za pomocą wykazu.

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.

2. W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.

3. Wybierz subskrypcję, którą chcesz zarządzać.

4. Poniżej sekcji **stan** znajdują się listy dostępnych dodatków dla subskrypcji.  

5. Zaktualizuj liczbę licencji dla każdego wymaganego dodatku. Następnie **prześlij** zmiany.

Możliwość kupowania dodatków za pośrednictwem Centrum partnerskiego jest dostępna tylko dla dostawców rachunków bezpośrednich i pośrednich.
Tylko kwalifikujące się dodatki są wyświetlane na podstawie podstawowych wymagań i dostępności regionalnej. Aby uzyskać więcej informacji na temat cen i ofert, zapoznaj się z tabelą ofert dla odsprzedawców rozwiązań w chmurze.  Wstrzymanie subskrypcji podstawowej spowoduje również wstrzymanie wszystkich skojarzonych dodatków.

Daty rozpoczęcia dla dodatków są dopasowywane do podstawowej subskrypcji, a opłaty są obliczane na podstawie daty rozpoczęcia i zakończenia naliczania opłat z opłatami proporcjonalnymi na pierwszej fakturze. Aby uzyskać dodatkowe informacje, zobacz artykuł dotyczący [rozliczeń opartych na licencji](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Wstrzymywanie lub anulowanie subskrypcji

Partnerzy mogą wstrzymywać lub anulować subskrypcję, jeśli jest to wymagane przez klienta lub w przypadku braku płatności lub oszustwa.

### <a name="suspend-a-subscription"></a>Wstrzymywanie subskrypcji

W przypadku zmiany stanu subskrypcji na **zawieszone** użytkownicy nie będą mogli się zalogować ani uzyskiwać dostępu do usług.

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.

2. W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.

3. Wybierz subskrypcję, którą chcesz zarządzać.

4. W sekcji **Stan** wybierz pozycję **Wstrzymano**. Następnie **prześlij** zmiany.

5. Wszystkie dane zostaną usunięte, chyba że subskrypcja zostanie ponownie aktywowana w ciągu 90 dni lub 90 dni i liczba dni od momentu otwarcia konta oraz pierwszego okresu rozliczeniowego (maksymalnie 120 dni).

W przypadku wstrzymania subskrypcji Data wyświetlana poniżej przycisku **Wstrzymaj** wskazuje, kiedy subskrypcja wygaśnie automatycznie, jeśli nie zostanie ponownie aktywowana. 

### <a name="cancel-a-subscription"></a>Anulowanie subskrypcji

Możesz anulować subskrypcje SaaS oparte na licencji od wydawców niezależnych od firmy Microsoft [w centrum](csp-commercial-marketplace-overview.md)partnerskim. Po anulowaniu anulowania w okresie anulowania otrzymasz pełny zwrot.

W przypadku niezależnych dostawców oprogramowania oferty są rozliczane miesięcznie:

- Jeśli po złożeniu zamówienia zostanie anulowana godzina krótsza niż 24 godziny, otrzymasz pełne środki na następną fakturę.

- Jeśli po złożeniu zamówienia zostanie anulowane później niż 24 godziny, anulowanie zostanie zaplanowane na odnowienie.

W przypadku ofert rozliczanych rocznie:

- Jeśli anulujesz subskrypcję poniżej 14 dni, otrzymasz pełne środki na następną fakturę.

- Jeśli anulujesz zamówienie później niż 14 dni po jego umieszczeniu, anulowanie zostanie zaplanowane na odnowienie.

Po przekroczeniu tych okresów nie będzie już widoczna opcja anulowania subskrypcji.

> [!NOTE]
> W przypadku korzystania z usług niezależnych dostawców oprogramowania (na przykład używanych przez maszyny wirtualne lub kontenery) nie kwalifikują się do powrotu. Usługi oparte na użyciu mogą być nieobsługiwane jako metoda anulowania. Ze względu na to, że opłaty są naliczane po użyciu, usługi te nie kwalifikują się do zwrotu pieniędzy.

Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.

2. W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.

3. Znajdź subskrypcję, którą chcesz anulować.

4. W kolumnie **stan** wybierz pozycję **Anuluj**. Następnie **prześlij** zmiany.

5. Jeśli zostanie wyświetlone okno dialogowe, Wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij**.

6. Aby potwierdzić anulowanie, wybierz pozycję **tak, Anuluj**.

> [!NOTE]
> Możesz również anulować subskrypcję portalu Azure Marketplace przy użyciu interfejsów API. Aby to zrobić, zobacz sekcję [Anulowanie subskrypcji portalu Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Zdecyduj, czy chcesz automatycznie odnawiać komercyjną subskrypcję portalu Marketplace

Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji. W przypadku [subskrypcji na komercyjne produkty Marketplace](csp-commercial-marketplace-overview.md)możesz opcjonalnie zrezygnować z automatycznego odnawiania subskrypcji.

Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji komercyjnej witryny Marketplace:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.

2. W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.

3. Wybierz pozycję **Subskrypcje**. Zawiera listę wszystkich subskrypcji opartych na licencji zakupionych dla klienta.

4. W kolumnie **subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.

5. Na stronie Szczegóły subskrypcji Znajdź sekcję **stan** i usuń zaznaczenie pola wyboru **autoodnawianie** .

6. Wybierz pozycję **Prześlij**.

## <a name="next-steps"></a>Następne kroki

- [Kup komercyjne produkty Marketplace dla klientów](csp-commercial-marketplace-purchase.md)

- [Zarządzanie komercyjnymi produktami Marketplace dla klientów](csp-commercial-marketplace-manage.md)

- [Omówienie komercyjnej platformy handlowej](csp-commercial-marketplace-overview.md)