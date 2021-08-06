---
title: Let customers buy their own services in CSP
description: Dowiedz się, jak partnerzy programu CSP mogą pozwolić klientom na kupowanie własnych usług, takich jak rezerwacje platformy Azure, dla subskrypcji zakupionej dla nich w Partner Center.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 23ca72fada539b5036dfd6cf0ac04a5c18b5d96d
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/04/2021
ms.locfileid: "115100184"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Nadaj klientom uprawnienia Partner Center do kupowania własnych produktów lub usług

**Odpowiednie role:** Agent administracyjny | Agent sprzedaży

W tym artykule pokazano, jak partner w programie Dostawca rozwiązań w chmurze (CSP) może udzielić klientowi uprawnień do zakupu niektórych własnych usług lub zasobów.

Partnerzy w programie CSP często używają Partner Center i jego platformy handlowej do kupowania rozwiązań i usług dla swoich klientów. Partnerzy zezwalają niektórym klientom na aprowizować te usługi bezpośrednio z Azure Portal.

Oto przykład. Załóżmy, że kupujesz subskrypcję planu platformy Azure dla klienta w Partner Center. Następnie decydujesz się dodać inne zasoby lub usługi do tej subskrypcji w imieniu klienta. W takim przypadku możesz dodać rezerwacje platformy Azure do subskrypcji klienta (na przykład dodać wystąpienia zarezerwowane maszyn wirtualnych). Następnie możesz zezwolić klientowi na dalsze aprowizować zasoby rezerwacji platformy Azure samodzielnie w Azure Portal.

Teraz dzięki funkcji **Uprawnień klienta** możesz zapewnić klientom więcej opcji samoobsługi dzięki zasobom platformy Azure. Włączając uprawnienia dla klienta, umożliwiasz klientom kupowanie własnych zasobów (na przykład kupowanie własnych rezerwacji platformy Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Omówienie uprawnień klientów w Partner Center

Użyj strony Konto **klienta,** aby włączyć (lub wyłączyć) uprawnienia klienta. Obecnie ta funkcja obsługuje:

- **Rezerwacje platformy Azure:** Włączenie tego uprawnienia umożliwia klientowi zakup własnych rezerwacji platformy Azure dla konkretnej subskrypcji platformy Azure, która została dla nich zakupiona.

Przed włączeniem uprawnień klienta należy zwrócić uwagę na następujące ważne kwestie:

- Domyślnie uprawnienia klienta są automatycznie wyłączane (wyłączone) w Partner Center.

- Aby można było włączyć (lub wyłączyć) uprawnienia dla klienta, musisz mieć przypisaną rolę agenta administracyjnego w Partner Center.

  Partnerzy przypisani do roli Agent sprzedaży lub Agent pomocy technicznej mają dostęp tylko do odczytu i nie mogą włączać ani wyłączać uprawnień klientów.

- Możesz włączyć (włączyć) uprawnienia dla dowolnego klienta, który wybierzesz.

- Możesz włączyć (lub wyłączyć) uprawnienia klienta przy użyciu pulpitu nawigacyjnego Partner Center lub Partner Center [API.](/partner-center/develop/manage-customers)

- Po włączeniu (włączeniu) uprawnień dla określonego klienta będziesz ponosić odpowiedzialność za wszystkie kolejne zakupy dokonane przez tego klienta. Jeśli klienci chcą wymienić, anulować lub odnowić dokonany zakup (lub chcą zmienić początkowy zakres rezerwacji), nie będą mogli tego zrobić samodzielnie. Musi poprosić Cię jako partnera o pomoc w wymianie, anulowaniu i odnowieniu zakupów lub późniejszym wprosieniu zmian w zakresie rezerwacji.  

- Po włączeniu uprawnień dla określonego klienta  nie będziesz powiadamiany o kolejnych zakupach dokonanych przez klienta.

- Późniejsze zakupy dokonane przez klienta będą wyświetlane w Partner Center wraz z dowolnymi zakupami dokonanym przez Ciebie. Te zakupy można znaleźć na stronie  Historia zamówień klienta, na stronie **Rezerwacje** lub w [**dzienniku aktywności**](activity-logs.md).

>[!NOTE]
> Aby uzyskać informacje o cenach, które klient zapłaci, oraz o tym, jak pomóc klientom w zarządzaniu zakupami, zobacz Pomaganie klientom w zarządzaniu [rezerwacjami, które kupują.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Nadaj klientom uprawnienia do zakupu własnych rezerwacji platformy Azure

Rezerwacje platformy Azure to doskonały sposób na kupowanie usług platformy Azure po obniżonej cenie. Aby dowiedzieć się więcej na temat zalet rezerwacji platformy Azure, zobacz [Co to są rezerwacje platformy Azure?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Teraz masz możliwość zakupu rezerwacji platformy Azure w imieniu klientów, co być może już robiliśmy. Możesz też udzielić klientom uprawnień do zakupu własnych rezerwacji platformy Azure.

>[!NOTE]
> Po nadasz klientom uprawnienia do zakupu własnych rezerwacji platformy Azure, pomóż im zarządzać zakupami rezerwacji. Aby uzyskać więcej informacji, zobacz [Pomaganie klientom w zarządzaniu rezerwacjami, które kupują.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Aby umożliwić klientom kupowanie własnych rezerwacji platformy Azure

1. Sprawdź, czy klient ma istniejący plan platformy Azure lub globalną subskrypcję platformy Azure kupioną w jego imieniu.

2. Sprawdź, czy klientowi przypisano **rolę właściciela** dla tej subskrypcji.

3. Włącz uprawnienia klienta (włącz tę **funkcję),** aby zakupić własne rezerwacje platformy Azure.

Każdy krok jest wyświetlany poniżej.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Sprawdzanie, czy klient ma istniejącą subskrypcję platformy Azure

Zanim udzielisz klientom uprawnień do zakupu własnych rezerwacji platformy Azure, musisz sprawdzić, czy klient ma istniejący plan platformy Azure lub subskrypcję globalną platformy Azure. Jeśli klient nie pokazuje bieżącej subskrypcji platformy Azure w usłudze Partner Center, musisz kupić dla nich subskrypcję przed włączeniem uprawnień klienta.

- Aby sprawdzić, czy klient ma już subskrypcję platformy Azure, zaloguj się do pulpitu Partner Center, a następnie wybierz pozycję **CSP,** a następnie **pozycję Customers (Klienci).** Wybierz określonego klienta z listy. Następnie wybierz **pozycję Subskrypcje** i poszukaj dowolnych subskrypcji opartych na użyciu dla planu platformy Azure lub globalnej platformy Azure.

- Jeśli klient nie ma istniejącej subskrypcji platformy Azure, możesz kupić dla nich subskrypcję. Zobacz [Zakup planu platformy Azure.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Sprawdź, czy klientowi przypisano prawidłową rolę na platformie Azure

Po sprawdzeniu, czy klient ma istniejącą subskrypcję platformy Azure, musisz również sprawdzić,  czy kluczowi użytkownikom skojarzonym z klientem przypisano prawidłową rolę właściciela dla tej subskrypcji platformy Azure. Jest to dostęp oparty na rolach (RBAC), który klient musi kupić rezerwacje platformy Azure dla zakupionej subskrypcji platformy Azure.

Niektórzy partnerzy mogą już przypisać rolę **właściciela** klientom, którzy chcą aktywnie zarządzać własnymi zasobami platformy Azure i aprowizować je. Jeśli masz już przypisany stan **właściciela** do klienta w celu zarządzania wcześniejszymi subskrypcjami, które zostały dla nich zakupione, możesz pominąć ten krok.  

> [!IMPORTANT]
> Jeśli klientowi nie przypisano  roli właściciela, zostanie wyświetlony błąd w Azure Portal uniemożliwiający mu zakup rezerwacji platformy Azure.

Aby sprawdzić, czy klientowi przypisano **rolę właściciela** dla subskrypcji platformy Azure:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Wybierz **pozycję CSP**, **a następnie pozycję Klienci** i wybierz określonego klienta.

3. Wybierz **pozycję Subskrypcje** dla tego klienta i znajdź określoną subskrypcję platformy Azure.

4. Wybierz przycisk **Zarządzaj** obok subskrypcji tego klienta. Spowoduje to otwarcie [Azure Portal](https://portal.azure.com/).

5. Aby przypisać **rolę właściciela** do określonego użytkownika, wykonaj następujące kroki, aby przypisać użytkownika jako [administratora.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Włączanie lub wyłączanie uprawnień klienta w celu zakupu własnych rezerwacji platformy Azure

Po sprawdzeniu, czy klient ma istniejącą subskrypcję platformy Azure, a użytkownikom przypisano rolę właściciela dla tej subskrypcji, możesz włączyć (włączyć) uprawnienia klienta.  Możesz również użyć tych kroków, aby wyłączyć (wyłączyć) uprawnienia klienta. Uprawnienia klientów można włączać lub wyłączać przy użyciu pulpitu nawigacyjnego Partner Center lub [Partner Center API.](/partner-center/develop/manage-customers)

Aby włączyć (lub wyłączyć) uprawnienia klienta w Partner Center:

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. W menu nawigacji po lewej stronie wybierz pozycję **CSP**, a następnie **pozycję Klienci.** Zostanie wyświetlona lista klientów.

3. Wybierz konkretną nazwę klienta.

4. Wybierz **pozycję Konto** z menu klienta. Zostanie **wyświetlona strona Konto** klienta.

5. Znajdź obszar **Uprawnienia klienta** w dolnej części strony.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Uprawnienia klienta na stronie Konto." border="true":::

6. W **obszarze Rezerwacje platformy Azure** znajdź opcję **Zezwalaj klientowi na zakup.**

7. Aby włączyć uprawnienia klienta, przenieś przełącznik obok tej opcji do **pozycji** Wł. Aby wyłączyć uprawnienia klienta, przenieś przełącznik do **pozycji** Wyłączone.

>[!NOTE]
> Aby dowiedzieć się, co jeszcze się dzieje po włączeniu uprawnień klienta do zakupu własnych rezerwacji platformy Azure, zobacz Overview of customer permissions in Partner Center ( Omówienie uprawnień klientów w [usłudze Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Po włączeniu (lub włączeniu) uprawnień klienta dziennik aktywności rejestruje każdą akcję. (Ten dziennik jest dostępny po wybraniu ikony koła zębatego w górnej części pulpitu Partner Center nawigacyjnego). Gdy włączysz lub wyłączysz uprawnienia klienta, akcja będzie  wyświetlana jako Utwórz uprawnienia do zakupu klienta lub Usuń uprawnienia do zakupu klienta w dzienniku aktywności. 

## <a name="help-customers-manage-reservations-they-purchase"></a>Pomaganie klientom w zarządzaniu rezerwacjami, które kupują

Gdy udzielisz klientom uprawnień do zakupu własnych rezerwacji platformy Azure, możesz pomóc im lepiej zarządzać zakupami zasobów. Klienci mogą zarządzać wieloma aspektami rezerwacji platformy Azure bezpośrednio z [Azure Portal.](https://portal.azure.com/) Będą oni potrzebować Twojej pomocy w zarządzaniu kilkoma innymi aspektami rezerwacji platformy Azure, które kupują w ramach subskrypcji programu CSP.  

Pomóż klientom dowiedzieć się więcej na temat zarządzania tymi aspektami rezerwacji platformy Azure:

- Ceny, za które klienci będą płacić za rezerwacje platformy Azure
- Jak klienci mogą zoptymalizować użycie rezerwacji platformy Azure
- Co się stanie, gdy klienci kupią rezerwacje w zakresie udostępnionym?
- Co się stanie, jeśli klienci będą chcieli zmienić, anulować i odnowić rezerwację lub zmienić jej zakres?

**Ceny, za które klienci będą płacić za rezerwacje.** Klient będzie kupować rezerwacje platformy Azure na podstawie wcześniej zakupionej subskrypcji na koncie rozliczeniowym partnera CSP. Cena klienta za wszelkie rezerwacje platformy Azure, które kupują na podstawie tej subskrypcji, również jest ustawiana przez Ciebie. Ta cena może różnić się od ceny bezpośredniej internetowej, jaką klient widzi w Azure Portal.

**Jak klienci mogą zoptymalizować użycie rezerwacji.** Niektórzy klienci mogą skorzystać z większej wiedzy na temat optymalizowania wykorzystania rezerwacji lub przypisywania początkowego zakresu rezerwacji podczas zakupu. Aby uzyskać więcej informacji, poproś klientów o przeczytanie [tematu Zarządzanie rezerwacjami zasobów platformy Azure.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Co się stanie, gdy klient zakupi rezerwację z zakresem udostępnionym?** Gdy klienci zakupią rezerwację na podstawie poprzedniej subskrypcji programu CSP i przypisują jej zakres udostępniony, wszelkie rabaty, które klient otrzymał, będą stosowane do pasującego użycia dla wszystkich subskrypcji zakupionych przez partnera CSP dla tego klienta.

**Co powinni zrobić klienci, jeśli chcą wymienić, anulować lub odnowić dokonany zakup lub zmienić początkowy zakres rezerwacji?** Klienci muszą poprosić partnera o pomoc w zmianie początkowego zakresu rezerwacji. Potrzebują oni również pomocy partnera w wymianie, anulowaniu lub odnowieniu rezerwacji. Nie mogą oni samodzielnie wykonywać tych zadań z rezerwacjami opartymi na subskrypcjach zakupionych dla nich przez partnera CSP.

## <a name="next-steps"></a>Następne kroki

- [Kupowanie rezerwacji platformy Azure w imieniu klientów](azure-reservations-buying.md)

- [Partner Center — sprzedaż rezerwacji firmy Microsoft](azure-reservations.md)

- [Zarządzanie rezerwacjami platformy Azure w imieniu klientów](azure-reservations-manage.md)