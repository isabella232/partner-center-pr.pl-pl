---
title: Migrowanie Skype dla firm subskrypcji
description: Dowiedz się, jak i kiedy migrować niektórych klientów z wygasającą subskrypcją Skype dla firm Online (plan 1) do nowych Office 365 wersji.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 58908e966eb80d219afa0cbc8c043932f5aef1a1
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842511"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 version (Migrowanie subskrypcji usługi Skype dla firm Online — plan 1 do nowszej wersji usługi Office 365)

**Odpowiednie role:** Agent sprzedaży

Plan 1 Skype dla firm Online zostanie wycofany od 1 sierpnia 2018 r. Po tej dacie klienci nie mogą już kupować nowych subskrypcji Skype dla firm Plan 1, a istniejące subskrypcje nie będą odnawiane automatycznie po wygaśnięciu i nie będą zapewniać opcji odnawiania. Na stronie szczegółów subskrypcji stan subskrypcji usługi Skype dla firm Online Plan 1 został zmieniony na "Wygasa [data]" z "Automatycznie odnawia się w dniu [data]".  

Aby zapewnić ciągłość działania klientów, należy przejść klientów z wygasającą subskrypcją Skype dla firm Online Plan 1 do obsługiwanej opcji SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w ciągu roku, aby uniknąć jakichkolwiek outages usług dla klientów. 

>[!NOTE]
>Obie Skype dla firm usługi Online Plan 1 komercyjne i rządowe jednostki SKU zostaną wycofane.

Jeśli używasz interfejsu API (Commerce REST (CREST) lub Partner Center), znajdź wygasające subskrypcje, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False. 1 września 2018 r. subskrypcja usługi Skype dla firm Online Plan 1 zostanie ustawiona na automatyczne odnawianie=Fałsz. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype dla firm Plany zastępcze planu 1 w trybie online

Dzięki nowym planom klienci mogą korzystać z nowszej funkcjonalności w Office 365. Szczegóły cennika znajdują się w cenniku i macierzy listy ofert w Partner Center. 

- Opcja 1: Office 365 Enterprise F1
- Opcja 2: Microsoft 365 Enterprise F1
- Opcja 3. Inne Office 365 planów

|**Funkcja**    |**Opcja 1**   |**Opcja 2**   |**Opcja 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Pobierz wszystkie funkcje zawarte w planie 1 usługi Skype dla firm Online|Yes   |Yes   |Yes   |
|Wiadomości błyskawiczne i obecność |Yes   |Yes   |Yes   |
|Komunikacja równorzędna audio i wideo za pośrednictwem protokołu IP|Yes   |Yes   |Yes   
|Dołączanie do spotkań jako uwierzytelniony użytkownik| Yes   |Yes   |Yes   |

## <a name="transition-customers-to-new-product-plans"></a>Przechodzenie klientów do nowych planów produktów

Firma Microsoft stale oferuje naszym partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub zmigrowanie ich subskrypcji z jednostki SKU, które zostaną ostatecznie zamknięte. Migrowanie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków:

- Kupowanie nowej subskrypcji
- Ponowne przypisanie bieżących licencji użytkowników
- Anulowanie starej subskrypcji

### <a name="migrate-your-customers-to-new-plans"></a>Migrowanie klientów do nowych planów

1. Aby kupić nową subskrypcję, z **menu Partner Center wybierz** pozycję Klienci, wybierz klienta, którego chcesz przenieść, a następnie wybierz pozycję Dodaj **subskrypcje.** 

2. Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**. 

Klient powinien teraz mieć zarówno starą, jak i nową subskrypcję, starą subskrypcję planu 1 usługi Skype dla firm Online i nową subskrypcję "docelową", na przykład opcję 1 — Office 365 Enterprise F1.

3. Aby ponownie przypisać licencje użytkowników klienta, z menu usługi Partner Center wybierz pozycję **Klienci,** wybierz klienta, który przenosisz, **a** następnie wybierz pozycję Użytkownicy i **licencje.** Zostanie otwarta strona Użytkownicy i licencje klienta.

4. Aby ponownie przypisać licencję użytkownika, wybierz użytkownika do ponownego przypisania, a następnie wybierz pozycję **Zarządzaj licencjami.**

5. Na **stronie Zarządzanie licencjami** wyczyść pole wyboru Skype dla firm Online Plan 1 i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący.

6. Wybierz pozycję **Prześlij**. Strona potwierdzenia zawiera listę nowych przypisań licencji. Kontynuuj ten sam proces dla innych użytkowników, którzy potrzebują przypisań licencji.

Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie klienta.

7. Z menu **Partner Center** wybierz pozycję **Klienci.** Wybierz klienta, którego subskrypcję anulujesz.

8. Na stronie szczegółów subskrypcji ustaw dla subskrypcji wartość **Wstrzymano**.

9. Wybierz **pozycję Prześlij.**

Stara subskrypcja zostanie wstrzymana, a nowa subskrypcja będzie aktywna. Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni. Klient nie ponosi żadnych dodatkowych kosztów dla starej subskrypcji.

## <a name="next-steps"></a>Następne kroki

- [Doradcy: utwórz i wyślij zaproszenie do wersji próbnej, aby klienci próbowali Office 365](advisors-create-a-trial-invitation.md)
- [Doradcy: tworzenie bazy klientów przy użyciu ofert zakupu i zaproszeń do wersji próbnej usługi Office 365](advisors-build-your-business.md)
- [Doradcy: Tworzenie oferty zakupu](advisor-create-a-purchase-offer.md)
