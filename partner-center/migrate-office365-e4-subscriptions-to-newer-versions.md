---
title: Migrowanie Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Microsoft Office 365 Enterprise wersji E4 zostanie wycofana z dniem 7 kwietnia 2017 r. Dowiedz się, jak migrować subskrypcje klientów do nowszej wersji Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b440b7baaad26ac6ee1c1e8313a13c4aa3cc271f9d84f5421aeb07edf1ea8a84
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681522"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrate Office 365 E4 subscriptions to newer Office 365 versions (Migrowanie subskrypcji usługi Office 365 E4 do nowszych wersji usługi Office 365)

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny | Agent sprzedaży

Plan Office 365 Enterprise E4 został wycofany, 7 kwietnia 2017 r. Po tej dacie nie Office 365 nowych subskrypcji E4, a istniejące subskrypcje E4 nie będą odnawiane automatycznie po wygaśnięciu.

Po zakończeniu subskrypcji E4 zostaną one anulowane. Aby zapewnić ciągłość działania klientów, należy przejść klientów z wygasającą subskrypcją E4 do obsługiwanej opcji SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w ciągu roku, aby uniknąć jakichkolwiek outages usług dla klientów. 

> [!NOTE]  
> Obie Office 365 Enterprise E4 komercyjne i rządowe zostaną wycofane.
 
Na stronie szczegółów subskrypcji stan subskrypcji E4 zmienił się na "Wygasa [data]" z "Automatycznie odnawia się [data]". 

Jeśli używasz interfejsu API (CREST lub Partner Center), możesz wykryć wygasające subskrypcje, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False. 

Subskrypcje E4 zostaną ustawione na automatyczne odnawianie=Fałsz w dniu 7 kwietnia 2017 r. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise E4 planów wymiany wersji

Możesz zachować tę samą funkcjonalność, co E4, lub zapewnić klientom możliwość korzystania z nowszej funkcji w usługach Office 365 i Skype dla firm Online. Szczegóły cennika znajdują się w cenniku i macierzy listy ofert w Partner Center. Bezpieczny produkt Enterprise E3 lub Secure Productive Enterprise E5 można zastąpić odpowiednio następującymi opcjami dla Office 365 Enterprise E3 lub Office 365 Enterprise E5.

- Opcja 1: Office 365 Enterprise E5

- Opcja 2: Office 365 Enterprise E3 + Skype dla firm Cloud PBX

- Opcja 3: Office 365 Enterprise E3 + Skype dla firm Plus CAL (cena i funkcjonalność parzystość z E4)

- Opcja 4: Office 365 Enterprise E3


| Cecha | Opcja 1 | Opcja 2 | Opcja 3 | Opcja 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Pobierz wszystkie funkcje zawarte w Office 365 Enterprise E4? | Tak | Tak | Tak | Nie |
| Telefon zarządzane w Office 365? | Tak | Tak | Nie | Nie |
| Telefon zarządzane zarówno lokalnie, jak i w Office 365 (wdrożenie hybrydowe)? | Tak | Tak | Nie | Nie |
| Opcja dodania planu połączeń głosowych PSTN? | Tak | Tak | Nie | Nie |
| Konferencje PSTN? | Tak | Nie | Nie | Nie |
| Zaawansowane narzędzia do współpracy, analizy i zabezpieczeń? | Tak | Nie | Nie | Nie |
| Interakcyjne raporty, pulpity nawigacyjne i wizualizacje danych? | Tak | Nie | Nie | Nie | 
| Większa kontrola nad zabezpieczeniami danych i zgodnością dzięki wbudowanym mechanizmom kontroli prywatności, przejrzystości i udoskonalonym użytkownikom? | Tak | Nie | Nie | Nie | 

## <a name="transition-customers-to-new-product-plans"></a>Przechodzenie klientów do nowych planów produktów

Firma Microsoft stale oferuje naszym partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub zmigrowanie ich subskrypcji z jednostki SKU, które zostaną ostatecznie zamknięte. Migrowanie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków:

-   Kupowanie nowej subskrypcji
-   Ponowne przypisanie bieżących licencji użytkowników
-   Anulowanie starej subskrypcji

Wykonaj następujące kroki, aby przeprowadzić migrację subskrypcji Office 365 Enterprise E4 klienta do jednej z opcji w powyższej tabeli.

### <a name="step-1---purchase-the-new-subscription"></a>Krok 1. Zakup nowej subskrypcji

1. Z **Partner Center** wybierz pozycję **Klienci,** wybierz klienta, który chcesz przenieść, a następnie wybierz **pozycję Dodaj subskrypcje.**

2. Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.

   Klient powinien teraz mieć zarówno starą, jak i nową subskrypcję, starą subskrypcję Office 365 Enterprise E4 i nową subskrypcję "docelową", na przykład opcję 1 — Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Krok 2. Ponowne przypisanie licencji użytkowników klienta

1. Z **Partner Center** wybierz pozycję **Klienci,** wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Użytkownicy i licencje.** Zostanie otwarta strona Użytkownicy i licencje klienta.

2. Aby ponownie przypisać licencje użytkowników, wybierz użytkownika do ponownego przypisania, a następnie wybierz pozycję **Zarządzaj licencjami.**

3. Na stronie **Zarządzanie licencjami** wyczyść pole **wyboru Office 365 Enterprise E4** licencji usługi i wybierz nowy plan usługi dla subskrypcji, do których klient jest przekierowyny.

4. Wybierz pozycję **Prześlij**. Strona potwierdzenia zawiera listę nowych przypisań licencji.

5. Kontynuuj te same czynności z innymi użytkownikami klientów, którzy potrzebują ponownego przypisania licencji.

Po przeniesieniu licencji użytkowników do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na najwyższym poziomie klienta.

### <a name="step-3---cancel-the-old-subscription"></a>Krok 3. Anulowanie starej subskrypcji

1. Z menu **Partner Center** wybierz pozycję **Klienci.** Wybierz klienta, którego chcesz przenieść, a następnie wybierz subskrypcję, którą chcesz anulować.

2. Na stronie szczegółów subskrypcji ustaw stan subskrypcji na **Wstrzymano**.

3. Wybierz pozycję **Prześlij**.

Stara subskrypcja zostanie wstrzymana, a nowa subskrypcja będzie aktywna. Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni. Klient nie ponosi żadnych dodatkowych kosztów dla starej subskrypcji.



 



