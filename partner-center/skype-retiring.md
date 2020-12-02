---
title: Migrowanie niektórych subskrypcji usługi Skype dla firm
description: Dowiedz się, jak i kiedy przeprowadzić migrację niektórych klientów z wygasaniem subskrypcji usługi Skype dla firm Online (plan 1) do nowych wersji pakietu Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: c9ad5b1c0671ff1d27d25c6f92499b72d77e6c22
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/02/2020
ms.locfileid: "92529654"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 version (Migrowanie subskrypcji usługi Skype dla firm Online — plan 1 do nowszej wersji usługi Office 365)

**Dotyczy**

- Centrum partnerskie

Plan 1 usługi Skype dla firm Online zostanie wycofany, od 1 sierpnia 2018. Po tym dniu klienci nie mogą już kupować nowych subskrypcji usługi Skype dla firm (plan 1), a istniejące subskrypcje nie będą odnawiane automatycznie, gdy wygasną i nie będą udostępniać opcji odnowienia. Na stronie szczegółów subskrypcji stan subskrypcji usługi Skype dla firm Online plan 1 zmienił się na "wygasa w dniu [Date]" z "autonews w dniu [Date]".  

Aby zapewnić ciągłość dla klientów, należy przejść do klientów z wygasaniem subskrypcji usługi Skype dla firm Online (plan 1) do obsługiwanej opcji jednostki SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów. 

>[!NOTE]
>Zarówno magazyny usługi Skype dla firm Online (plan 1) komercyjne i rządowe zostały wycofane.

Jeśli używasz interfejsu API (SZCZYTu lub Centrum partnerskiego), Znajdź wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false. Subskrypcje usługi Skype dla firm Online plan 1 będą ustawione na wartość autorenew = false 1 września 2018. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Plany zamiany usługi Skype dla firm Online plan 1

Dzięki nowym planom klienci mogą korzystać z nowszych funkcji w pakiecie Office 365. Szczegóły cennika znajdują się na liście cen i macierzy list oferty w centrum partnerskim. 

- Opcja 1: Office 365 Enterprise F1
- Opcja 2: Microsoft 365 Enterprise F1
- Opcja 3: inne plany pakietu Office 365

|**Funkcja**    |**Opcja 1**   |**Opcja 2**   |**Opcja 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Pobierz wszystkie funkcje dostępne w usłudze Skype dla firm Online plan 1|Tak   |Tak   |Tak   |
|Wiadomości błyskawiczne i obecność |Tak   |Tak   |Tak   |
|Audio równorzędne i wideo za pośrednictwem adresu IP|Tak   |Tak   |Tak   
|Dołącz do spotkań jako uwierzytelnionego użytkownika| Tak   |Tak   |Tak   |

## <a name="transition-customers-to-new-product-plans"></a>Przejście klientów do nowych planów produktu

Firma Microsoft ciągle oferuje swoim partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub przeprowadzenie migracji swoich subskrypcji z jednostek SKU, które ostatecznie zostaną zamknięte. Migrowanie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących czynności:

- Kup nową subskrypcję
- Ponowne przypisanie bieżących licencji użytkownika
- Anuluj starą subskrypcję

### <a name="migrate-your-customers-to-new-plans"></a>Migrowanie klientów do nowych planów

1. Aby kupić nową subskrypcję, w **menu Centrum partnerskiego** wybierz pozycję **klienci**, wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje**.

2. Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**. 

Klient powinien mieć teraz zarówno stare, jak i nowe subskrypcje, starszą subskrypcję usługi Skype dla firm Online (plan 1) i nową subskrypcję "target", na przykład opcję 1 — pakiet Office 365 Enterprise F1.

3. Aby ponownie przypisać licencje użytkowników klienta, w menu **Centrum partnerskiego** wybierz pozycję **klienci**, wybierz przenoszony klient, a następnie wybierz pozycję **Użytkownicy i licencje**. Zostanie otwarta strona użytkownicy i licencje klienta.

4. Aby ponownie przypisać licencję użytkownika, wybierz użytkownika, którego chcesz przypisać ponownie, a następnie wybierz pozycję **Zarządzaj licencjami.**

5. Na stronie **Zarządzanie licencjami** wyczyść pole wyboru licencja usługi Skype dla firm Online plan 1 i wybierz nowy plan usług dla subskrypcji, do której jest przenoszony klient.

6. Wybierz pozycję **Prześlij**. Na stronie potwierdzenia wyświetlane są nowe przypisania licencji. Kontynuuj ten sam proces dla innych użytkowników, którzy potrzebują przypisań licencji.

Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie klienta.

7. W menu **Centrum partnerskiego** wybierz pozycję **Customers**. Wybierz klienta, którego subskrypcję chcesz anulować.

8. Na stronie Szczegóły subskrypcji Ustaw subskrypcję na **zawieszone**.

9. Wybierz pozycję **Prześlij.**

Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna. Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach. Klient nie wiąże się z żadnymi dodatkowymi kosztami dla starej subskrypcji.

