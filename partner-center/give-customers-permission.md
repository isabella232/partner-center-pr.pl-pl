---
title: Zezwól klientom na kupowanie własnych usług w programie CSP
description: Dowiedz się, w jaki sposób partnerzy programu CSP mogą umożliwić klientom kupowanie własnych usług, takich jak rezerwacje platformy Azure, w przypadku subskrypcji zakupionej dla nich w centrum partnerskim.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19f86ec5353abc21e14a3a8ac2ef17dd17924cfe
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529980"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Przyznaj klientom uprawnienia w centrum partnerskim do kupowania własnych produktów lub usług

**Dotyczy**

- Centrum partnerskie
- Partnerzy w programie CSP

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży

W tym artykule pokazano, jak partner w programie dostawcy rozwiązań w chmurze (CSP) może przyznać klientowi uprawnienia do kupowania niektórych własnych usług lub zasobów.

Partnerzy w programie CSP często używają Centrum partnerskiego i jego komercyjnej witryny Marketplace do kupowania rozwiązań i usług dla swoich klientów. Partnerzy umożliwiają klientom samodzielne udostępnianie tych usług bezpośrednio z poziomu Azure Portal.

Oto przykład. Załóżmy, że kupisz subskrypcję planu platformy Azure dla klienta w centrum partnerskim. Następnie zdecyduje się dodać inne zasoby lub usługi do tej subskrypcji w imieniu klienta. W takim przypadku można dodać rezerwacje platformy Azure do subskrypcji klienta (na przykład dodanie zarezerwowanych wystąpień maszyn wirtualnych). Następnie można umożliwić klientowi dalsze Inicjowanie obsługi zasobów usługi Azure Reservation w Azure Portal.

Teraz dzięki funkcji **uprawnień klienta** możesz zapewnić klientom dodatkowe opcje samoobsługowego używania zasobów platformy Azure. Włączenie uprawnień dla klienta umożliwia klientom kupowanie własnych zasobów (np. kupowanie własnych rezerwacji platformy Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Przegląd uprawnień klienta w centrum partnerskim

Użyj strony **konto** klienta, aby włączyć (lub wyłączyć) uprawnienia klienta. Obecnie ta funkcja obsługuje:

- **Rezerwacje platformy Azure:** Włączenie tego uprawnienia pozwala klientowi zakupić własne rezerwacje platformy Azure dla określonej subskrypcji platformy Azure, która została zakupiona.

Przed włączeniem uprawnień klienta należy zwrócić uwagę na następujące ważne punkty:

- Domyślnie uprawnienia klienta są automatycznie wyłączane (wyłączone) w centrum partnerskim.

- Aby móc włączyć (lub wyłączyć) uprawnienia dla klienta, musisz mieć przypisaną rolę Agent administracyjny w centrum partnerskim.

  Partnerzy przypisani do roli agenta sprzedaży lub agenta pomocy technicznej mają dostęp tylko do odczytu i nie mogą włączać ani wyłączać uprawnień klienta.

- Możesz włączyć (Włącz) uprawnienia dla dowolnego wybranego klienta.

- Możesz włączyć (lub wyłączyć) uprawnienia klienta przy użyciu pulpitu nawigacyjnego Centrum partnerskiego lub [interfejsów API Centrum partnerskiego](/partner-center/develop/manage-customers).

- Po włączeniu uprawnień (Włączanie) dla określonego klienta użytkownik jest zobowiązany do płacenia za kolejne zakupy dokonane przez tego klienta. Jeśli klienci chcą wymienić, anulować lub odnowić dokonane zakupy (lub chcą zmienić początkowy zakres rezerwacji), nie będą oni mogli tego robić. Muszą oni mieć pytania, jako partnera, w celu ułatwienia wymiany, anulowania i odnawiania zakupów lub wprowadzać późniejsze zmiany w zakresie rezerwacji.  

- Po włączeniu uprawnień dla określonego klienta **nie** będziesz otrzymywać powiadomień o jakichkolwiek późniejszych zakupach dokonanych przez klienta.

- Późniejsze zakupy dokonane przez klienta będą widoczne w centrum partnerskim wraz z wszelkimi zakupami dokonanymi przez Ciebie. Te zakupy można znaleźć na stronie **historia zamówienia** klienta, stronie **zastrzeżeń** lub w [**dzienniku aktywności**](activity-logs.md).

>[!NOTE]
> Aby uzyskać informacje na temat cen, które klient będzie obciążany i jak pomóc klientom w zarządzaniu zakupami, zobacz [Pomoc dla klientów zarządzających rezerwacjami, które kupują](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Przyznaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure

Rezerwacje platformy Azure to świetny sposób kupowania usług platformy Azure z obniżoną stawką. Aby dowiedzieć się więcej na temat korzyści z używania rezerwacji platformy Azure, zobacz [co to są Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Teraz masz możliwość kupowania rezerwacji platformy Azure w imieniu swoich klientów. Możesz też przyznać klientom uprawnienia do kupowania własnych rezerwacji platformy Azure.

>[!NOTE]
> Po nadaniu klientom uprawnień do zakupu własnych rezerwacji na platformę Azure Pomóż im zarządzać wszelkimi zakupionymi rezerwacjami. Aby uzyskać więcej informacji, zobacz [Pomoc dla klientów zarządzanie rezerwacjami, które kupują](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Aby umożliwić klientom kupowanie własnych rezerwacji platformy Azure

1. Upewnij się, że klient ma istniejący plan platformy Azure lub subskrypcję globalną platformy Azure, która została zakupiona w ich imieniu.

2. Sprawdź, czy klient ma przypisaną rolę **właściciela** dla tej subskrypcji.

3. Włącz uprawnienia klienta **(Włącz tę funkcję),** aby zakupić własne rezerwacje platformy Azure.

Każdy krok zostanie wyświetlony poniżej.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Sprawdź, czy klient ma istniejącą subskrypcję platformy Azure

Przed udzieleniem klientom uprawnień do kupowania własnych rezerwacji na platformę Azure należy sprawdzić, czy klient ma istniejący plan platformy Azure lub subskrypcję globalną platformy Azure. Jeśli klient nie wyświetli bieżącej subskrypcji platformy Azure w centrum partnerskim, musisz kupić subskrypcję dla nich przed włączeniem ich uprawnień.

- Aby sprawdzić, czy klient ma już subskrypcję platformy Azure, zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego, a następnie wybierz opcję **CSP** , a następnie kliknij pozycję **klienci**. Wybierz określonego klienta z listy. Następnie wybierz pozycję **subskrypcje** i poszukaj wszelkich subskrypcji opartych na użyciu usługi Azure plan lub Azure Global.

- Jeśli klient nie ma istniejącej subskrypcji platformy Azure, możesz kupić dla nich subskrypcję. Zobacz [kupowanie planu platformy Azure](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Sprawdź, czy klient został przypisany do poprawnej roli na platformie Azure

Po zweryfikowaniu, że klient ma istniejącą subskrypcję platformy Azure, należy również sprawdzić, czy użytkownicy usługi Key powiązani z klientem mają przypisaną prawidłową rolę **właściciela** dla tej subskrypcji platformy Azure. Jest to dostęp oparty na rolach (RBAC) wymagany przez klienta do kupowania rezerwacji platformy Azure dla zakupionej subskrypcji platformy Azure.

Niektórzy partnerzy mogą mieć już przypisaną rolę **właściciela** do klientów chcących aktywnie zarządzać własnymi zasobami platformy Azure i inicjować do nich udostępnianie. Jeśli masz już przypisany stan **właściciela** do klienta w celu zarządzania poprzednimi subskrybowanymi subskrypcjami, możesz pominąć ten krok.  

> [!IMPORTANT]
> Jeśli klient nie ma przypisanej roli **właściciela** , otrzyma błąd w Azure Portal uniemożliwić im kupowanie rezerwacji platformy Azure.

Aby sprawdzić, czy klient ma przypisaną rolę **właściciela** dla subskrypcji platformy Azure:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.

2. Wybierz pozycję **dostawca usług kryptograficznych** , a następnie pozycję **klienci** i wybierz określonego klienta.

3. Wybierz **subskrypcje** dla tego klienta i Znajdź określoną subskrypcję platformy Azure.

4. Wybierz przycisk **Zarządzaj** obok subskrypcji tego klienta. Spowoduje to otwarcie [Azure Portal](https://portal.azure.com/).

5. Aby przypisać rolę **właściciela** do określonego użytkownika, wykonaj następujące kroki, [Aby przypisać użytkownika jako administratora](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Włącz lub Wyłącz uprawnienia klienta, aby kupić własne rezerwacje platformy Azure

Po zweryfikowaniu, że klient ma istniejącą subskrypcję platformy Azure, a użytkownicy mają przypisaną rolę **właściciela** dla tej subskrypcji, możesz włączyć (włączyć) uprawnienia klienta. Możesz również użyć tych kroków, aby wyłączyć (wyłączyć) uprawnienia klienta. Uprawnienia klientów można włączać lub wyłączać za pomocą pulpitu nawigacyjnego Centrum partnerskiego lub [interfejsów API Centrum partnerskiego](/partner-center/develop/manage-customers).

Aby włączyć (lub wyłączyć) uprawnienia klienta w centrum partnerskim:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.

2. W menu nawigacji po lewej stronie wybierz **dostawcę CSP** , a następnie pozycję **klienci**. Zostanie wyświetlona lista klientów.

3. Wybierz konkretną nazwę klienta.

4. Wybierz pozycję **konto** z menu klient. Zostanie wyświetlona strona **konto** klienta.

5. Znajdź obszar **uprawnienia klienta** w dolnej części strony.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Uprawnienia klienta na stronie konta." border="true":::

6. W obszarze **rezerwacje platformy Azure** Znajdź opcję **Zezwalaj klientowi na zakup** .

7. Aby włączyć uprawnienia klienta, Przenieś przełącznik obok tej opcji do pozycji **włączone** . Aby wyłączyć uprawnienia klienta, przesuń przełącznik na pozycję OFF ( **Wyłącz** ).

>[!NOTE]
> Aby dowiedzieć się, co się dzieje w przypadku włączenia uprawnień klienta do zakupu własnych rezerwacji platformy Azure, zobacz [Omówienie uprawnień klientów w centrum partnerskim](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Po włączeniu lub wyłączeniu uprawnień klienta dziennik aktywności rejestruje każdą akcję. (Ten dziennik jest dostępny po wybraniu ikony koła zębatego w górnej części pulpitu nawigacyjnego Centrum partnerskiego). Po włączeniu lub wyłączeniu uprawnień klienta akcja zostanie wyświetlona w ramach opcji **Utwórz uprawnienia do zakupu klienta** lub **Usuń uprawnienia zakupu klienta** w dzienniku aktywności.

## <a name="help-customers-manage-reservations-they-purchase"></a>Pomóż klientom zarządzać rezerwacjami, które kupują

Po nadaniu klientom uprawnień do zakupu własnych rezerwacji na platformę Azure możesz pomóc im lepiej zarządzać wszelkimi zakupionymi zasobami. Klienci mogą zarządzać wieloma aspektami rezerwacji platformy Azure bezpośrednio z poziomu [Azure Portal](https://portal.azure.com/). Będą oni musieli pomóc Ci w zarządzaniu kilkoma innymi aspektami rezerwacji platformy Azure, które kupują w ramach subskrypcji programu CSP.  

Pomóż klientom dowiedzieć się więcej o zarządzaniu tymi aspektami rezerwacji platformy Azure:

- Ceny klientów będą obciążani rezerwacjami platformy Azure
- Jak klienci mogą zoptymalizować użycie rezerwacji platformy Azure
- Co się stanie, gdy klienci kupują rezerwacje z zakresem udostępnionym?
- Co się stanie, jeśli klienci chcą zmienić, anulować i odnowić rezerwację lub zmienić jej zakres?

**Ceny klientów będą płacenia za rezerwacje.** Klient będzie kupował rezerwacje platformy Azure w oparciu o subskrypcję zakupionej wcześniej na koncie rozliczeniowym partnera CSP. Cena klienta dla wszelkich rezerwacji systemu Azure, które kupują w oparciu o tę subskrypcję, jest również ustawiana przez użytkownika. Cena ta może być różna od ceny bezpośrednio w sieci Web, która widzi klient w Azure Portal.

**Jak klienci mogą zoptymalizować użycie rezerwacji.** Niektórzy klienci mogą skorzystać z dodatkowych informacji na temat optymalizowania użycia rezerwacji lub sposobu przypisywania początkowego zakresu rezerwacji podczas zakupu. Aby uzyskać więcej informacji, poprosimy klientów o odczytywanie [rezerwacji dla zasobów platformy Azure](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

**Co się stanie, gdy klient kupi rezerwację z zakresem udostępnionym?** Gdy klienci kupują rezerwację w oparciu o wcześniejszą subskrypcję dostawcy CSP i przypisująsz zakres współużytkowany do tej rezerwacji, wszystkie rabaty, które klient otrzymał przez dostawcę usług kryptograficznych, zostaną zastosowane do dopasowania użycia dla wszystkich subskrypcji, których Partner CSP zakupił dla tego klienta.

**Co powinni robić Klienci, jeśli chcą wymienić, anulować lub odnowić kupione zakupy lub zmienić początkowy zakres rezerwacji?** Klienci muszą poproś ich partnera o zmianę zakresu początkowego rezerwacji. Potrzebują także pomocy partnera w zakresie wymiany, anulowania lub odnawiania rezerwacji. Nie mogą oni wykonywać tych zadań przy użyciu rezerwacji w oparciu o subskrypcje zakupione dla nich przez partnera CSP.

## <a name="next-steps"></a>Następne kroki

- [Kupowanie rezerwacji platformy Azure w imieniu klientów](azure-reservations-buying.md)

- [Centrum partnerskie — sprzedawanie rezerwacji firmy Microsoft](azure-reservations.md)

- [Zarządzanie rezerwacjami platformy Azure w imieniu klientów](azure-reservations-manage.md)