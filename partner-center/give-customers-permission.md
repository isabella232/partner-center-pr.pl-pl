---
title: Nadaj klientom uprawnienia do kupowania własnych produktów i usług
description: Dowiedz się, jak partnerzy programu CSP mogą pozwolić klientom na zakup własnych usług, takich jak rezerwacje platformy Azure, dla subskrypcji zakupionej dla nich w Partner Center.
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7242bd62f2a84e4c836ad9804d8b857c7606a2ce
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072842"
---
# <a name="give-customers-permissions-to-buy-their-own-products-and-services"></a>Nadaj klientom uprawnienia do kupowania własnych produktów i usług

**Odpowiednie role:** Administrator | Agent sprzedaży

W tym artykule pokazano, w jaki sposób partner w programie Dostawca rozwiązań w chmurze (CSP) może udzielić klientowi uprawnień do zakupu niektórych własnych usług lub zasobów.

Partnerzy w programie CSP często używają Partner Center i jego platformy handlowej do kupowania rozwiązań i usług dla swoich klientów. Partnerzy umożliwią niektórym klientom aprowizować te usługi bezpośrednio z Azure Portal.

Oto przykład. Załóżmy, że kupujesz subskrypcję planu platformy Azure dla klienta w Partner Center. Następnie decydujesz się dodać inne zasoby lub usługi do tej subskrypcji w imieniu klienta. W takim przypadku możesz dodać rezerwacje platformy Azure do subskrypcji klienta (na przykład dodać wystąpienia zarezerwowane maszyn wirtualnych). Następnie możesz zezwolić klientowi na dalszą aprowizę zasobów rezerwacji platformy Azure w Azure Portal.

Teraz dzięki funkcji **Uprawnienia klienta** możesz zapewnić klientom więcej opcji samoobsługi dzięki zasobom platformy Azure. Włączając uprawnienia dla klienta, umożliwiasz klientom kupowanie własnych zasobów (na przykład kupowanie własnych rezerwacji platformy Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Omówienie uprawnień klientów w Partner Center

Użyj strony **Konto klienta,** aby włączyć (lub wyłączyć) uprawnienia klienta. Obecnie ta funkcja obsługuje:

- **Rezerwacje platformy Azure:** Włączenie tego uprawnienia umożliwia klientowi zakup własnych rezerwacji platformy Azure dla konkretnej subskrypcji platformy Azure, która została dla niej zakupiona.

Przed włączeniem uprawnień klientów należy zwrócić uwagę na następujące ważne kwestie:

- Domyślnie uprawnienia klientów są automatycznie wyłączane (wyłączone) w Partner Center.

- Aby można było włączyć (lub wyłączyć) uprawnienia dla klienta, musisz mieć przypisaną rolę agenta administracyjnego w Partner Center.

  Partnerzy z przypisaną rolą agenta sprzedaży lub agenta pomocy technicznej mają dostęp tylko do odczytu i nie mogą włączać ani wyłączać uprawnień klientów.

- Możesz włączyć (włączyć) uprawnienia dla dowolnego klienta, który wybierzesz.

- Uprawnienia klientów można włączyć (lub wyłączyć) przy użyciu pulpitu nawigacyjnego Partner Center lub [Partner Center API.](/partner-center/develop/manage-customers)

- Po włączeniu (włączeniu) uprawnień dla określonego klienta użytkownik będzie odpowiedzialny za płatności za kolejne zakupy dokonane przez tego klienta. Jeśli klienci chcą wymienić, anulować lub odnowić dokonany zakup (lub chcą zmienić początkowy zakres rezerwacji), nie będą mogli tego zrobić samodzielnie. Należy poprosić Cię jako partnera o pomoc w wymianie, anulowaniu i odnowieniu zakupów lub w późniejszym wymusieniu zmian w zakresie rezerwacji.  

- Po włączeniu uprawnień dla określonego klienta  nie będziesz powiadamiać o kolejnych zakupach dokonanych przez klienta.

- Późniejsze zakupy dokonane przez klienta będą wyświetlane w Partner Center wraz z zakupami dokonanym przez Ciebie. Te zakupy można znaleźć na stronie  Historia zamówień  klienta, na stronie Rezerwacje lub w [**dzienniku aktywności.**](activity-logs.md)

> [!NOTE]
> Aby uzyskać informacje o cenach, które klient zapłaci, i o tym, jak pomóc klientom w zarządzaniu zakupami, zobacz Pomaganie klientom w zarządzaniu [rezerwacjami, które kupują.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Nadaj klientom uprawnienia do zakupu własnych rezerwacji platformy Azure

Rezerwacje platformy Azure to doskonały sposób na zakup usług platformy Azure po obniżonej stawce. Aby dowiedzieć się więcej na temat zalet rezerwacji platformy Azure, zobacz [Co to są rezerwacje platformy Azure?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Teraz masz możliwość zakupu rezerwacji platformy Azure w imieniu klientów, co być może już robisz. Możesz też udzielić klientom uprawnień do zakupu własnych rezerwacji platformy Azure.

> [!NOTE]
> Po nadasz klientom uprawnienia do zakupu własnych rezerwacji platformy Azure, pomóż im zarządzać wszystkimi zakupami rezerwacji. Aby uzyskać więcej informacji, zobacz [Pomaganie klientom w zarządzaniu rezerwacjami, które kupują.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Aby umożliwić klientom zakup własnych rezerwacji platformy Azure

1. Sprawdź, czy klient ma istniejący plan platformy Azure lub subskrypcję globalną platformy Azure kupioną w jego imieniu.

2. Sprawdź, czy klientowi przypisano **rolę właściciela** dla tej subskrypcji.

3. Włącz uprawnienia klienta (włącz tę **funkcję),** aby kupić własne rezerwacje platformy Azure.

Każdy krok jest wyświetlany poniżej.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Sprawdzanie, czy klient ma istniejącą subskrypcję platformy Azure

Zanim udzielisz klientom uprawnień do zakupu własnych rezerwacji platformy Azure, musisz sprawdzić, czy klient ma istniejący plan platformy Azure lub subskrypcję globalną platformy Azure. Jeśli klient nie pokazuje bieżącej subskrypcji platformy Azure w Partner Center, musisz kupić dla nich subskrypcję przed włączeniem uprawnień klienta.

- Aby sprawdzić, czy klient ma już subskrypcję platformy [](https://partner.microsoft.com/commerce/customers/list) Azure, przejdź do Partner Center listy klientów i wybierz określonego klienta z listy. Następnie wybierz **pozycję Subskrypcje** i poszukaj dowolnych subskrypcji opartych na użyciu dla planu platformy Azure lub globalnej platformy Azure.

- Jeśli klient nie ma istniejącej subskrypcji platformy Azure, możesz kupić dla nich subskrypcję. Zobacz [Zakup planu platformy Azure.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Sprawdź, czy klientowi przypisano prawidłową rolę na platformie Azure

Po sprawdzeniu, czy klient ma istniejącą subskrypcję platformy Azure, musisz również sprawdzić,  czy kluczom skojarzonym z klientem przypisano prawidłową rolę właściciela dla tej subskrypcji platformy Azure. Jest to dostęp oparty na rolach (RBAC), który klient musi kupić rezerwacje platformy Azure dla zakupionej subskrypcji platformy Azure.

Niektórzy partnerzy mogą już przypisać rolę **właściciela** klientom, którzy chcą aktywnie zarządzać własnymi zasobami platformy Azure i aprowizować je. Jeśli masz już przypisany **stan Właściciel** do klienta w celu zarządzania wcześniejszymi subskrypcjami, które zostały dla nich zakupione, możesz pominąć ten krok.  

> [!IMPORTANT]
> Jeśli klientowi nie przypisano roli **właściciel,** zostanie wyświetlony błąd w witrynie Azure Portal uniemożliwiający mu zakup rezerwacji platformy Azure.

Aby sprawdzić, czy klientowi przypisano **rolę właściciela** subskrypcji platformy Azure:

> [!NOTE]
> Interfejs Partner Center wersji zapoznawczej zapewnia bardziej wydajne i wydajne środowisko użytkownika za pośrednictwem logicznie zgrupowanych obszarów roboczych. Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych i sposobu jego włączanie, zobacz Getting around Partner Center (Poruszanie [się po Partner Center).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Wybierz **kafelek Klienci,** a następnie wybierz określonego klienta.

3. Wybierz **pozycję Subskrypcje** dla tego klienta i znajdź określoną subskrypcję platformy Azure.

4. Wybierz przycisk **Zarządzaj** obok subskrypcji tego klienta. Spowoduje to otwarcie [Azure Portal](https://portal.azure.com/).

5. Aby przypisać **rolę właściciela** do określonego użytkownika, wykonaj następujące kroki, aby przypisać użytkownika jako [administratora.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Wybierz **pozycję CSP**, **a następnie pozycję Klienci** i wybierz określonego klienta.

3. Wybierz **pozycję Subskrypcje** dla tego klienta i znajdź określoną subskrypcję platformy Azure.

4. Wybierz przycisk **Zarządzaj** obok subskrypcji tego klienta. Spowoduje to otwarcie [Azure Portal](https://portal.azure.com/).

5. Aby przypisać **rolę właściciela** do określonego użytkownika, wykonaj następujące kroki, aby przypisać użytkownika jako [administratora.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

* * *

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Włączanie lub wyłączanie uprawnień klientów w celu zakupu własnych rezerwacji platformy Azure

Po sprawdzeniu, czy klient ma istniejącą subskrypcję platformy Azure i użytkownikom przypisano rolę właściciela dla tej subskrypcji, możesz włączyć (włączyć) uprawnienia klienta.  Możesz również użyć tych kroków, aby wyłączyć (wyłączyć) uprawnienia klienta. Uprawnienia klientów można włączać lub wyłączać przy użyciu pulpitu nawigacyjnego Partner Center lub [Partner Center API.](/partner-center/develop/manage-customers)

Aby włączyć lub wyłączyć uprawnienia klientów w Partner Center:

> [!NOTE]
> Interfejs Partner Center wersji zapoznawczej zapewnia bardziej wydajne i wydajne środowisko użytkownika za pośrednictwem logicznie zgrupowanych obszarów roboczych. Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych i sposobu jego włączanie, zobacz Getting around Partner Center (Poruszanie [się po Partner Center).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Wybierz **kafelek Klienci,** a następnie wybierz określonego klienta.

3. Wybierz **pozycję Konto** z menu klienta. Zostanie **wyświetlona strona Konto** klienta.

4. Znajdź **obszar Uprawnienia** klienta w dolnej części strony.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Uprawnienia klienta na stronie Konto." border="true":::

5. W **obszarze Rezerwacje platformy Azure** znajdź opcję **Zezwalaj klientowi na zakup.**

6. Aby włączyć uprawnienia klienta, przenieś przełącznik obok tej opcji do **pozycji** Wł. Aby wyłączyć uprawnienia klienta, przenieś przełącznik do **pozycji** Wyłączone.

> [!NOTE]
> Aby dowiedzieć się, co jeszcze się dzieje po włączeniu uprawnień klienta do zakupu własnych rezerwacji platformy Azure, zobacz Overview of customer permissions in Partner Center ( Omówienie uprawnień klientów w [usłudze Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
> Gdy włączysz (lub wyłączysz) uprawnienia klienta, dziennik aktywności będzie rejestrować każdą akcję. (Ten dziennik jest dostępny po wybraniu ikony koła zębatego w górnej części pulpitu Partner Center nawigacyjnego). Gdy włączysz lub wyłączysz uprawnienia klienta, akcja będzie wyświetlana jako Utwórz uprawnienia zakupu klienta lub Usuń uprawnienia zakupu klienta **w** dzienniku aktywności. 

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. W menu nawigacji po lewej stronie wybierz pozycję **CSP,** a następnie **pozycję Klienci.** Zostanie wyświetlona lista klientów.

3. Wybierz określoną nazwę klienta.

4. Wybierz **pozycję Konto** z menu klienta. Zostanie **wyświetlona strona Konto** klienta.

5. Znajdź **obszar Uprawnienia** klienta w dolnej części strony.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Uprawnienia klienta na stronie Konto." border="true":::

6. W **obszarze Rezerwacje platformy Azure** znajdź opcję **Zezwalaj klientowi na zakup.**

7. Aby włączyć uprawnienia klienta, przenieś przełącznik obok tej opcji do **pozycji** Wł. Aby wyłączyć uprawnienia klienta, przenieś przełącznik do **pozycji** Wyłączone.

> [!NOTE]
> Aby dowiedzieć się, co jeszcze się dzieje po włączeniu uprawnień klienta do zakupu własnych rezerwacji platformy Azure, zobacz Overview of customer permissions in Partner Center ( Omówienie uprawnień klientów w [usłudze Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
> Gdy włączysz (lub wyłączysz) uprawnienia klienta, dziennik aktywności będzie rejestrować każdą akcję. (Ten dziennik jest dostępny po wybraniu ikony koła zębatego w górnej części pulpitu Partner Center nawigacyjnego). Gdy włączysz lub wyłączysz uprawnienia klienta, akcja będzie wyświetlana jako Utwórz uprawnienia zakupu klienta lub Usuń uprawnienia zakupu klienta **w** dzienniku aktywności. 

* * *

## <a name="help-customers-manage-reservations-they-purchase"></a>Pomaganie klientom w zarządzaniu rezerwacjami, które kupują

Gdy udzielisz klientom uprawnień do zakupu własnych rezerwacji platformy Azure, możesz pomóc im lepiej zarządzać wszystkimi zakupiatymi zasobami. Klienci mogą zarządzać wieloma aspektami samych rezerwacji platformy Azure bezpośrednio z [Azure Portal.](https://portal.azure.com/) Będą oni potrzebować Twojej pomocy w zarządzaniu kilkoma innymi aspektami rezerwacji platformy Azure, które kupują w ramach subskrypcji programu CSP.  

Pomóż klientom zrozumieć więcej na temat zarządzania tymi aspektami rezerwacji platformy Azure:

- Ceny, za które klienci płacą za rezerwacje platformy Azure
- Jak klienci mogą zoptymalizować użycie rezerwacji platformy Azure
- Co się stanie, gdy klienci kupią rezerwacje w zakresie udostępnionym?
- Co się stanie, jeśli klienci będą chcieli zmienić, anulować i odnowić rezerwację lub zmienić jej zakres?

**Ceny, za które klienci będą płacić za rezerwacje.** Klient będzie kupować rezerwacje platformy Azure na podstawie wcześniej zakupionej subskrypcji na koncie rozliczeniowym partnera CSP. Cena wszystkich rezerwacji platformy Azure kupowanych w oparciu o tę subskrypcję jest również ustawiana przez klienta. Ta cena może różnić się od ceny bezpośredniej dla sieci Web, które klient widzi w Azure Portal.

**Jak klienci mogą zoptymalizować użycie rezerwacji.** Niektórzy klienci mogą skorzystać z informacji na temat optymalizowania użycia rezerwacji lub przypisywania początkowego zakresu rezerwacji podczas zakupu. Aby uzyskać więcej informacji, poproś klientów o przeczytanie [tematu Zarządzanie rezerwacjami zasobów platformy Azure.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Co się stanie, gdy klient zakupi rezerwację w zakresie udostępnionym?** Gdy klienci kupują rezerwację na podstawie poprzedniej subskrypcji programu CSP i przypisują jej zakres udostępniony, wszelkie rabaty, które klient otrzymał, będą dotyczyć pasującego użycia dla wszystkich subskrypcji zakupionych dla tego klienta przez partnera CSP.

**Co powinni zrobić klienci, jeśli chcą wymienić, anulować lub odnowić dokonany zakup lub zmienić początkowy zakres rezerwacji?** Klienci muszą poprosić partnera o pomoc w zmianie początkowego zakresu rezerwacji. Potrzebują oni również pomocy partnera w wymianie, anulowaniu lub odnowieniu rezerwacji. Nie mogą oni samodzielnie wykonywać tych zadań z rezerwacjami opartymi na subskrypcjach zakupionych dla nich przez partnera CSP.

## <a name="next-steps"></a>Następne kroki

- [Kupowanie rezerwacji platformy Azure w imieniu klientów](azure-reservations-buying.md)

- [Partner Center — sprzedaż rezerwacji firmy Microsoft](azure-reservations.md)

- [Zarządzanie rezerwacjami platformy Azure w imieniu klientów](azure-reservations-manage.md)