---
title: Migrowanie subskrypcji usługi Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office wersji 365 Enterprise E4 zostanie wycofana z dniem 7 kwietnia 2017 r. Dowiedz się, jak migrować subskrypcje klientów do nowszej wersji usługi Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151563"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrate Office 365 E4 subscriptions to newer Office 365 versions (Migrowanie subskrypcji usługi Office 365 E4 do nowszych wersji usługi Office 365)

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży

Plan E4 usługi Office 365 Enterprise został wycofany od 7 kwietnia 2017 r. Po tej dacie nie można już kupować nowych subskrypcji usługi Office 365 E4, a istniejące subskrypcje E4 nie będą odnawiane automatycznie po ich wygaśnięciu.

Po zakończeniu subskrypcji E4 zostaną one anulowane. Aby zapewnić ciągłość działania klientów, należy przejść klientów z wygasającą subskrypcją E4 do obsługiwanej opcji SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w roku, aby uniknąć jakichkolwiek outages usługi dla klientów. 

> [!NOTE]  
> Zarówno komercyjne, jak i rządowe jednostki SKU usługi Office 365 Enterprise E4 zostały wycofane.
 
Na stronie szczegółów subskrypcji stan subskrypcji E4 zmienił się na "Wygasa [data]" z "Automatyczne odnowienie [data]". 

Jeśli używasz interfejsu API (CREST lub Partner Center), możesz wykryć wygasające subskrypcje, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False. 

Subskrypcje E4 zostaną ustawione na wartość auto renew=False w dniu 7 kwietnia 2017 r. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Plany wymiany wersji Office 365 Enterprise E4

Możesz zachować tę samą funkcjonalność z platformą E4 lub zapewnić klientom możliwość korzystania z nowszej funkcji w usługach Office 365 i Skype dla firm Online. Szczegóły cennika znajdują się w cenniku i macierzy listy ofert w Partner Center. Opcje Secure Product Enterprise E3 lub Secure Productive Enterprise E5 można zastąpić odpowiednio w przypadku usługi Office 365 Enterprise E3 lub Office 365 Enterprise E5.

- Opcja 1: Office 365 Enterprise E5

- Opcja 2: Office 365 Enterprise E3 + Skype dla firm Cloud PBX

- Opcja 3: Office 365 Enterprise E3 + Skype dla firm Plus CAL (cena i funkcjonalność parzystość z E4)

- Opcja 4: Office 365 Enterprise E3


| Cecha | Opcja 1 | Opcja 2 | Opcja 3 | Opcja 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Pobierz wszystkie funkcje zawarte w usłudze Office 365 Enterprise E4? | Tak | Tak | Tak | Nie |
| Numery telefonów zarządzane w usłudze Office 365? | Tak | Tak | Nie | Nie |
| Numery telefonów zarządzane zarówno lokalnie, jak i w usłudze Office 365 (wdrożenie hybrydowe)? | Tak | Tak | Nie | Nie |
| Opcja dodania planu połączeń głosowych PSTN? | Tak | Tak | Nie | Nie |
| Konferencje PSTN? | Tak | Nie | Nie | Nie |
| Zaawansowane narzędzia do współpracy, analizy i zabezpieczeń? | Tak | Nie | Nie | Nie |
| Interaktywne raporty, pulpity nawigacyjne i wizualizacje danych? | Tak | Nie | Nie | Nie | 
| Większa kontrola nad zabezpieczeniami i zgodnością danych dzięki wbudowanej ochronie prywatności, przejrzystości i udoskonalonym mechanizmom kontroli użytkowników? | Tak | Nie | Nie | Nie | 

## <a name="transition-customers-to-new-product-plans"></a>Przechodzenie klientów do nowych planów produktów

Firma Microsoft stale oferuje naszym partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub zmigrowanie ich subskrypcji z jednostki SKU, które zostaną ostatecznie zamknięte. Migrowanie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków:

-   Kupowanie nowej subskrypcji
-   Ponowne przypisanie bieżących licencji użytkowników
-   Anulowanie starej subskrypcji

Wykonaj następujące kroki, aby przeprowadzić migrację subskrypcji usługi Office 365 Enterprise E4 klienta do jednej z opcji w powyższej tabeli.

### <a name="step-1---purchase-the-new-subscription"></a>Krok 1. Zakup nowej subskrypcji

1. W menu **Partner Center** wybierz pozycję **Klienci,** wybierz klienta, który chcesz przenieść, a następnie wybierz **pozycję Dodaj subskrypcje.**

2. Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.

   Klient powinien teraz mieć zarówno starą, jak i nową subskrypcję, starą subskrypcję usługi Office 365 Enterprise E4 i nową subskrypcję "docelową", na przykład Opcja 1 — Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Krok 2. Ponowne przypisanie licencji użytkowników klienta

1. Z **Partner Center** wybierz pozycję **Klienci,** wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Użytkownicy i licencje.** Zostanie otwarta strona Użytkownicy i licencje klienta.

2. Aby ponownie przypisać licencje użytkowników, wybierz użytkownika do ponownego przypisania, a następnie wybierz pozycję **Zarządzaj licencjami.**

3. Na stronie **Zarządzanie licencjami** wyczyść pole wyboru Licencja usługi **Office 365 Enterprise E4** i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący.

4. Wybierz pozycję **Prześlij**. Strona potwierdzenia zawiera listę nowych przypisań licencji.

5. Te same kroki należy wykonać w przypadku innych użytkowników klientów, którzy potrzebują ponownego przypisania licencji.

Po przeniesieniu licencji użytkowników do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na najwyższym poziomie klienta.

### <a name="step-3---cancel-the-old-subscription"></a>Krok 3. Anulowanie starej subskrypcji

1. Z menu **Partner Center** wybierz pozycję **Klienci.** Wybierz klienta, którego chcesz przenieść, a następnie wybierz subskrypcję, którą chcesz anulować.

2. Na stronie szczegółów subskrypcji ustaw stan subskrypcji na **Wstrzymano**.

3. Wybierz pozycję **Prześlij**.

Stara subskrypcja zostanie wstrzymana, a nowa subskrypcja będzie aktywna. Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni. Klient nie ponosi żadnych dodatkowych kosztów w przypadku starej subskrypcji.



 



