---
title: Tworzenie subskrypcji klientów w Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak sprzedawać klientom subskrypcje produktów publikowanych przez firmę Microsoft oraz produktów SaaS publikowanych przez zewnętrznych isvs.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 227b1cb38f255ee32563c29c3e2bced88e7c15935a244e9e2bf0b4763c9eca52
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691127"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Tworzenie, zawieszanie lub anulowanie subskrypcji klientów

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży

Po utworzeniu rekordu klienta w katalogu Partner Center można sprzedawać im subskrypcje produktów w katalogu. Dotyczy to produktów publikowanych przez firmę Microsoft oraz produktów SaaS (Software as a Service) publikowanych przez niezależnych dostawców oprogramowania (ISV) innych firm na [platformie handlowej.](https://azuremarketplace.microsoft.com/marketplace)

Niektóre oferty są ograniczone do jednej subskrypcji na klienta. Aby wyświetlić listę ofert, które są ograniczone, odwiedź stronę Partner Center Cennik i oferty.

>[!IMPORTANT]
> Jako partner w programie CSP  możesz kupować oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center. Oznacza to, że  możesz kupić dowolną ofertę **SaaS** opartą na licencjach lub taryfowej, która została ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp. [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) Aby kupić lub zarządzać innymi, komercyjnymi ofertami platformy handlowej od isvs (takimi jak oferty oparte na użyciu obejmujące aplikacje platformy Azure, kontenery lub maszyny wirtualne), musisz przejść do witryny [Azure Portal.](https://portal.azure.com/)

>[!NOTE]
>Wszystkie daty i godziny w Partner Center są podane w standardzie czasu uniwersalnego (UTC). Może się to różnić nawet o 24 godziny od czasu lokalnego.

## <a name="create-a-new-subscription"></a>Tworzenie nowej subskrypcji

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Wybierz **pozycję Dodaj subskrypcję.** Na **karcie Usługi online** będą wyświetlane wszystkie dostępne oferty SaaS w witrynie Marketplace.

4. Aby wyświetlić tylko niektóre typy subskrypcji, należy dokonać wyboru w dostępnych filtrach:
   - **Publisher:** wybierz firmę **Microsoft,** aby wyświetlić tylko  oferty firmy Microsoft lub partnera, aby wyświetlić produkty platformy handlowej opublikowane przez isvs.
   - **Typ rozliczeń:** wybierz typ rozliczeń subskrypcji, których chcesz użyć: **Licencja** lub **Użycie.** Zobacz [Rozliczenia oparte na licencjach,](license-based-billing.md) aby uzyskać informacje, które pomogą Ci wybrać między miesięczną i roczną częstotliwością rozliczeń.
   - **Kategoria:** wybierz **Enterprise,** **Małe firmy** lub Wersja **próbna.** Aby uzyskać informacje na temat subskrypcji w wersji próbnej, zobacz Offer your customers trial of Microsoft products (Oferować [klientom wersje próbne produktów firmy Microsoft).](offer-your-customers-trials-of-microsoft-products.md)

5. Wybierz subskrypcje produktów, które chcesz kupić dla klienta. Dostępne produkty zależą od typu segmentu klientów (edukacja, administracja rządowa itp.) i zastosowanych filtrów. Niektóre oferty wyświetlane w witrynie Marketplace nie zawsze mogą być dostępne dla określonego klienta lub określonego partnera CSP. Może to być spowodowane:

   - Klient ma już subskrypcję tego produktu i jest dozwolony tylko jeden

   - Subskrypcja klienta może zostać wstrzymana (w tym przypadku można ją ponownie uaktywnić, zamiast kupować nową).

   - W przypadku ofert SaaS dla isv może być kilka powodów, dla których oferta nie jest dostępna do zakupu: isv may not support the customer's billing country or region; IsV may have chosen not to make the offer available through the CSP program; lub, isV may have made the offer exclusive to only certain CSP partners.or, the ISV may have made the [offer exclusive to](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) only certain CSP partners. Oferta isv może również nie być transakcji za pośrednictwem Partner Center (na przykład kontenerów lub niektórych ofert opartych na użyciu).  

6. Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby) i wybierz **pozycję Dodaj do koszyka.**

7. Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj zamówienie.

8. Po przejrzenia zamówień i przygotowaniu się do zakupu tych subskrypcji wybierz pozycję **Kup**.

9. Po zakupie subskrypcji dla klienta wystąpią następujące zdarzenia:

    - Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji na stronie **Subskrypcje tego** klienta. W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.

    **W przypadku subskrypcji isv SaaS (opartych na licencjach i mierzonych):**
    - Otrzymasz link do witryny wydawcy ISV. Ten link powinien ułatwić ukończenie wdrażania lub konfigurowania konta subskrypcji klienta.
      
    >[!NOTE]
    > Ani Ty, ani Klient nie otrzymacie wiadomości e-mail z instrukcjami dotyczącymi ukończenia procesu skonfigurowania/aprowizowania konta dla tego typu subskrypcji isV).

    - Jeśli Twoja subskrypcja zawiera 30-dniową bezpłatną wersję próbną, bezpłatny okres próbny zostanie zastosowany automatycznie. Jako partner w programie CSP nie możesz zrezygnować z okresu bezpłatnej wersji próbnej ofert zakupu dla klientów. Po zakończeniu okresu bezpłatnej wersji próbnej rozpocznie się okres subskrypcji, a subskrypcja zostanie przekształcona w stan płatny. Subskrypcja zostanie następnie automatycznie odnowiona zgodnie z tym samym harmonogramem.
   
## <a name="update-subscriptions-with-add-ons"></a>Aktualizowanie subskrypcji z dodatkami 

Aby kupić dodatek, klient musi najpierw mieć aktywną subskrypcję podstawową.  Nie można kupować dodatków za pomocą wykazu.

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Wybierz subskrypcję, którą chcesz zarządzać.

4. Poniżej sekcji **Stan** znajduje się lista dostępnych dodatków dla subskrypcji.  

5. Zaktualizuj liczbę licencji dla każdego wymaganego dodatku. Następnie **prześlij** zmiany.

Możliwość zakupu dodatków za pośrednictwem usługi Partner Center jest dostępna tylko dla dostawców faktury bezpośredniej i dostawców pośrednich.
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

Po wstrzymaniu subskrypcji data, która  zostanie wyświetlony poniżej przycisku Wstrzymano, wskazuje, kiedy subskrypcja automatycznie wygaśnie, jeśli subskrypcja nie zostanie ponownie aktywowana. 

>[!NOTE]
>Subskrypcje programu CSP nie mają wygasłego okresu (w jaki działają subskrypcje bezpośrednie w sieci Web), w którym usługi nadal działają, ale subskrypcja nie generuje żadnych opłat rozliczeniowych. Subskrypcje CSP są aktywne lub wstrzymane (albo całkowicie usunięte).

### <a name="cancel-a-subscription"></a>Anulowanie subskrypcji

Subskrypcje SaaS oparte na licencjach można anulować od zewnętrznych wydawców isV w ramach Partner Center [platformy handlowej.](csp-commercial-marketplace-overview.md) Dopóki anulujesz subskrypcję w okresie anulowania, otrzymasz pełny zwrot pieniędzy.

W przypadku ofert isv (isv) rozliczanych miesięcznie:

- Jeśli anulujesz zamówienie po upływie mniej niż 24 godzin, otrzymasz pełne środków na następnej fakturze.

- Jeśli anulujesz subskrypcję po upływie 24 godzin od złożonego zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.

W przypadku ofert rozliczanych rocznie:

- Jeśli anulujesz zamówienie po upływie mniej niż 14 dni, otrzymasz pełne środków na następnej fakturze.

- Jeśli anulujesz subskrypcję później niż 14 dni od zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.

Po zakończeniu tych okresów nie będzie już dostępna opcja anulowania subskrypcji.

> [!NOTE]
> Oparte na użyciu i mierzone usługi innych firm isv (które używają na przykład maszyn wirtualnych lub kontenerów) nie kwalifikują się do zwrotu. Usługi oparte na użyciu można anulować. Ponieważ opłaty są naliczane po użyciu, te usługi nie kwalifikują się do zwrotu kosztów.

Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Znajdź subskrypcję, którą chcesz anulować.

4. W kolumnie **Stan** wybierz pozycję **Anuluj.** Następnie **prześlij** zmiany.

5. Jeśli zostanie wyświetlone okno dialogowe, wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij.**

6. Aby potwierdzić anulowanie, wybierz pozycję **Tak, anuluj .**

> [!NOTE]
> Możesz również anulować subskrypcję usługi Azure Marketplace przy użyciu interfejsów API. Aby to zrobić, zobacz [Anulowanie subskrypcji Azure Marketplace subskrypcji](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Wybierz, czy subskrypcja platformy handlowej ma być odnawiana automatycznie

Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji. W [przypadku subskrypcji produktów platformy handlowej](csp-commercial-marketplace-overview.md)możesz opcjonalnie zdecydować, aby nie odnawiać subskrypcji automatycznie.

Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji platformy handlowej:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. Wybierz pozycję **Subskrypcje**. Zawiera listę wszystkich subskrypcji opartych na licencjach zakupionych dla klienta.

4. W kolumnie **Subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.

5. Na stronie szczegółów subskrypcji znajdź sekcję **Stan** i usuń zaznaczenie pola **Automatycznie odnawiaj.**

6. Wybierz pozycję **Prześlij**.

## <a name="next-steps"></a>Następne kroki

- [Kupowanie produktów na platformie handlowej dla klientów](csp-commercial-marketplace-purchase.md)

- [Zarządzanie produktami na platformie handlowej dla klientów](csp-commercial-marketplace-manage.md)

- [Omówienie komercyjnej platformy handlowej](csp-commercial-marketplace-overview.md)