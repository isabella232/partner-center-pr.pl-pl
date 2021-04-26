---
title: Migrowanie niektórych subskrypcji programu Skype dla firm
description: Dowiedz się, jak i kiedy migrować niektórych klientów z wygasającą subskrypcją usługi Skype dla firm Online (plan 1) do nowych wersji usługi Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: f395987ef647fa6f7ed264c6476ddae419eabc34
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002862"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 version (Migrowanie subskrypcji usługi Skype dla firm Online — plan 1 do nowszej wersji usługi Office 365)

**Odpowiednie role**

- Agent sprzedaży

Plan 1 usługi Skype dla firm Online zostanie wycofany od 1 sierpnia 2018 r. Po tej dacie klienci nie mogą już kupować nowych subskrypcji programu Skype dla firm Plan 1, a istniejące subskrypcje nie będą odnawiane automatycznie po wygaśnięciu i nie będą zapewniać opcji odnawiania. Na stronie szczegółów subskrypcji stan subskrypcji usługi Skype dla firm Online (plan 1) zmienił się na "Wygasa [data]" z "Automatyczne odnawianie [data]".  

Aby zapewnić ciągłość działania klientów, należy przejść klientów z wygasającą subskrypcją usługi Skype dla firm Online (plan 1) do obsługiwanej opcji SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w ciągu roku, aby uniknąć jakichkolwiek błędów usługi dla klientów. 

>[!NOTE]
>Zarówno komercyjne, jak i rządowe jednostki SKU planu 1 usługi Skype dla firm Online zostaną wycofane.

Jeśli używasz interfejsu API (CREST lub Partner Center), znajdź wygasające subskrypcje, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False. Subskrypcje usługi Skype dla firm Online (plan 1) zostaną ustawione na automatyczne odnawianie=Fałsz 1 września 2018 r. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Plany zastępcze usługi Skype dla firm Online (plan 1)

Dzięki nowym planom klienci mogą korzystać z nowszej funkcjonalności i funkcji w usłudze Office 365. Szczegóły cennika znajdują się w cenniku i macierzy listy ofert w Partner Center. 

- Opcja 1: Office 365 Enterprise F1
- Opcja 2: Microsoft 365 Enterprise F1
- Opcja 3. Inne plany usługi Office 365

|**Funkcja**    |**Opcja 1**   |**Opcja 2**   |**Opcja 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Pobierz wszystkie funkcje zawarte w planie 1 usługi Skype dla firm Online|Tak   |Tak   |Tak   |
|Wiadomości błyskawiczne i obecność |Tak   |Tak   |Tak   |
|Równorzędne połączenia audio i wideo za pośrednictwem protokołu IP|Tak   |Tak   |Tak   
|Dołączanie do spotkań jako uwierzytelniony użytkownik| Tak   |Tak   |Tak   |

## <a name="transition-customers-to-new-product-plans"></a>Przechodzenie klientów do nowych planów produktów

Firma Microsoft stale oferuje naszym partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub zmigrowanie ich subskrypcji z jednostki SKU, które ostatecznie zostaną zamknięte. Migrowanie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków:

- Kupowanie nowej subskrypcji
- Ponowne przypisanie bieżących licencji użytkowników
- Anulowanie starej subskrypcji

### <a name="migrate-your-customers-to-new-plans"></a>Migrowanie klientów do nowych planów

1. Aby kupić nową subskrypcję, w **menu** Partner Center wybierz pozycję **Klienci,** wybierz klienta, którego chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje.**

2. Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**. 

Klient powinien teraz mieć zarówno starą, jak i nową subskrypcję, starą subskrypcję usługi Skype dla firm Online (plan 1) i nową subskrypcję "docelową", na przykład Opcja 1 — Office 365 Enterprise F1.

3. Aby ponownie przypisać licencje użytkowników klienta, z menu usługi Partner Center wybierz pozycję **Klienci,** wybierz przenoszącego klienta, **a** następnie wybierz pozycję Użytkownicy i **licencje.** Zostanie otwarta strona Użytkownicy i licencje klienta.

4. Aby ponownie przypisać licencję użytkownika, wybierz użytkownika do ponownego przypisania, a następnie wybierz pozycję **Zarządzaj licencjami.**

5. Na stronie **Zarządzanie licencjami** wyczyść pole wyboru Licencja usługi Skype dla firm Online (plan 1) i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący.

6. Wybierz pozycję **Prześlij**. Strona potwierdzenia zawiera listę nowych przypisań licencji. Kontynuuj ten sam proces w przypadku innych użytkowników, którzy potrzebują przypisań licencji.

Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie klienta.

7. Z menu **Partner Center** wybierz pozycję **Klienci.** Wybierz klienta, którego subskrypcję anulujesz.

8. Na stronie szczegółów subskrypcji ustaw dla subskrypcji wartość **Wstrzymano**.

9. Wybierz **pozycję Prześlij.**

Stara subskrypcja zostanie wstrzymana, a nowa subskrypcja będzie aktywna. Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni. Klient nie ponosi żadnych dodatkowych kosztów dla starej subskrypcji.

## <a name="next-steps"></a>Następne kroki

- [Doradcy: tworzenie i wysyłanie zaproszenia do wersji próbnej dla klientów w celu wypróbowania usługi Office 365](advisors-create-a-trial-invitation.md)
- [Doradcy: Tworzenie bazy klientów za pomocą zaproszeń do wersji próbnej usługi Office 365 i ofert zakupu](advisors-build-your-business.md)
- [Doradcy: Tworzenie oferty zakupu](advisor-create-a-purchase-offer.md)
