---
title: Migrowanie subskrypcji pakietu Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition zostanie wycofana od 7 kwietnia 2017. Dowiedz się, jak migrować subskrypcje klientów do nowszych wersji pakietu Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132625"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrate Office 365 E4 subscriptions to newer Office 365 versions (Migrowanie subskrypcji usługi Office 365 E4 do nowszych wersji usługi Office 365)

**Odpowiednie role**

- Administrator globalny
- Administrator zarządzania użytkownikami
- Agent administracyjny
- Agent sprzedaży

Plan programu Office 365 Enterprise E4 został wycofany, obowiązuje 7 kwietnia 2017. Nie można już kupić nowych subskrypcji programu Office 365 E4 po tej dacie, a istniejące subskrypcje E4 nie będą odnawiane automatycznie po ich wygaśnięciu.

Po zakończeniu subskrypcji E4 zostaną one anulowane. Aby zapewnić ciągłość dla klientów, należy przejść do klientów z wygasaniem subskrypcji E4 do obsługiwanej opcji jednostki SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów. 

> [!NOTE]  
> Pakiety SKU komercyjnego i rządowego programu Office 365 Enterprise E4 zostały wycofane.
 
Na stronie szczegółów subskrypcji stan subskrypcji E4 został zmieniony na "wygasa w dniu [Date]" z "autonews w dniu [Date]". 

W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można odkrywać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false. 

Dla subskrypcji E4 zostanie ustawiona wartość autorenew = false w 7 kwietnia 2017. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Plany wymiany pakietu Office 365 Enterprise E4 Edition

Możesz korzystać z tych samych funkcji z E4 lub korzystać z nowszych funkcji w pakietach Office 365 i Skype dla firm Online. Szczegóły cennika znajdują się na liście cen i macierzy list oferty w centrum partnerskim. Bezpieczny produkt Enterprise w wersji E3 lub bezpieczna produktywność w przedsiębiorstwie E5 można zastąpić następującymi opcjami odpowiednio dla pakietu Office 365 Enterprise E3 lub pakietu Office 365 Enterprise E5.

- Opcja 1: Office 365 Enterprise E5

- Opcja 2: Office 365 Enterprise E3 + Skype dla firm — PBX

- Opcja 3: Office 365 Enterprise E3 + Skype dla firm Plus CAL (cena i funkcjonalność z parzystością)

- Opcja 4: Office 365 Enterprise E3


| Cecha | Opcja 1 | Opcja 2 | Opcja 3 | Opcja 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Pobrać wszystkie funkcje zawarte w pakiecie Office 365 Enterprise E4? | Tak | Tak | Tak | Nie |
| Numery telefonów zarządzane w pakiecie Office 365? | Tak | Tak | Nie | Nie |
| Numery telefonów zarządzane zarówno lokalnie, jak i w pakiecie Office 365 (wdrożenie hybrydowe)? | Tak | Tak | Nie | Nie |
| Czy można dodać plan rozmowy głosowej PSTN? | Tak | Tak | Nie | Nie |
| Konferencje PSTN? | Tak | Nie | Nie | Nie |
| Zaawansowane narzędzia do współpracy, analizy i zabezpieczeń? | Tak | Nie | Nie | Nie |
| Interaktywne raporty, pulpity nawigacyjne i wizualizacje danych? | Tak | Nie | Nie | Nie | 
| Większą kontrolę nad bezpieczeństwem danych i zgodnością z wbudowaną ochroną prywatności, przezroczystością i udoskonalonymi kontrolkami użytkowników? | Tak | Nie | Nie | Nie | 

## <a name="transition-customers-to-new-product-plans"></a>Przejście klientów do nowych planów produktu

Firma Microsoft ciągle oferuje swoim partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub przeprowadzenie migracji swoich subskrypcji z jednostek SKU, które ostatecznie zostaną zamknięte. Migrowanie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących czynności:

-   Kup nową subskrypcję
-   Ponowne przypisanie bieżących licencji użytkownika
-   Anuluj starą subskrypcję

Wykonaj następujące kroki, aby zmigrować subskrypcję pakietu Office 365 Enterprise E4 klienta do jednej z opcji w powyższej tabeli.

### <a name="step-1---purchase-the-new-subscription"></a>Krok 1 — kupowanie nowej subskrypcji

1. W menu **Centrum partnerskiego** wybierz pozycję **klienci**, wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje**.

2. Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.

   Klient powinien mieć teraz zarówno stare, jak i nowe subskrypcje, starszą subskrypcję pakietu Office 365 Enterprise E4 i nową subskrypcję "target", na przykład opcję 1 — pakiet Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Krok 2. przypisanie licencji użytkownika klienta

1. W menu **Centrum partnerskiego** wybierz pozycję **klienci**, wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Użytkownicy i licencje**. Zostanie otwarta strona użytkownicy i licencje klienta.

2. Aby ponownie przypisać licencje użytkownika, wybierz użytkownika, którego chcesz przypisać ponownie, a następnie wybierz pozycję **Zarządzaj licencjami**.

3. Na stronie **Zarządzanie licencjami** wyczyść pole wyboru licencja **Office 365 Enterprise E4** , a następnie wybierz nowy plan usługi dla subskrypcji, do której będzie przenoszony klient.

4. Wybierz pozycję **Prześlij**. Na stronie potwierdzenia wyświetlane są nowe przypisania licencji.

5. Kontynuuj te same kroki dla wszystkich innych użytkowników klienta, którzy potrzebują ponownego przypisania licencji.

Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie najwyższego poziomu klienta.

### <a name="step-3---cancel-the-old-subscription"></a>Krok 3. Anulowanie starej subskrypcji

1. W menu **Centrum partnerskiego** wybierz pozycję **Customers**. Wybierz klienta, który chcesz przenieść, a następnie wybierz subskrypcję, którą chcesz anulować.

2. Na stronie Szczegóły subskrypcji Ustaw stan subskrypcji na **zawieszone**.

3. Wybierz pozycję **Prześlij**.

Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna. Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach. Klient nie wiąże się z żadnymi dodatkowymi kosztami dla starej subskrypcji.



 



