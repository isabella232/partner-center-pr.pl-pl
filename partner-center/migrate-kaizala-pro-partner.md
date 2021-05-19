---
title: Migrowanie subskrypcji Kaizala Pro na platformę Microsoft 365
description: Dowiedz się, jak migrować subskrypcje usługi Kaizala Pro do Microsoft 365 usługi Office 365. Przeczytaj ten artykuł, aby uzyskać więcej informacji na temat przechodzenia klientów.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146429"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migrowanie autonomicznych subskrypcji usługi Kaizala Pro Microsoft 365 wersji usługi Office 365

**Odpowiednie role:** Agent sprzedaży

Od 1 lipca 2020 r. firma Microsoft kończy sprzedaż autonomicznej usługi Kaizala Pro. Klienci nie będą już mogli kupować nowych subskrypcji usługi Kaizala Pro po tej dacie, a istniejące subskrypcje usługi Kaizala Pro nie będą odnawiane automatycznie po wygaśnięciu.

Aby zapewnić ciągłość działania klientów, należy przejść klientów z wygasającą autonomiczną subskrypcją usługi Kaizala Pro do obsługiwanej opcji jednostki SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w ciągu roku, aby uniknąć jakichkolwiek błędów usługi dla klientów.

Jeśli używasz interfejsu API (CREST lub Partner Center), możesz wykryć wygasające subskrypcje, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania ustawioną na wartość false: `auto renew = False` .

Subskrypcje E4 zostaną ustawione `auto renew=False` na 1 lipca 2020 r. Klientów można przenieść do nowego planu w dowolnym momencie.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Plany zastępcze autonomicznej aplikacji Kaizala Pro

Dzięki nowym planom klienci mogą korzystać z nowszej funkcjonalności w Microsoft 365. Szczegóły cennika znajdują się w cenniku i macierzy listy ofert w Partner Center.

- [**Microsoft 365 for Business,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)w tym:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 dla frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)w tym:
   - Microsoft 365 F3 (wcześniej Microsoft 365 F1) i Office 365 F3
    
- [**Microsoft 365 for Enterprise, w**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)tym: 
   - Office 365 E1
   - Microsoft 365 E3 i Office 365 E3
   - Microsoft 365 E5 i Office 365 E5

- [**Microsoft 365 for Education, w**](https://www.microsoft.com/education/buy-license/microsoft365)tym: 
    - Microsoft 365 A1 i Office 365 A1
    - Microsoft 365 A3 i Office 365 A3
    - Microsoft 365 A5 i Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Przechodzenie klientów do nowych planów produktów

Firma Microsoft stale oferuje naszym partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub zmigrowanie ich subskrypcji z jednostki SKU, które ostatecznie zostaną zamknięte. Migrowanie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków:

A. Kupowanie nowej subskrypcji

B. Ponowne przypisanie bieżących licencji użytkowników

C. Anulowanie starej subskrypcji


## <a name="migrate-your-customers-to-new-plans"></a>Migrowanie klientów do nowych planów

### <a name="a-purchase-the-new-subscription"></a>A. Kupowanie nowej subskrypcji

1. Aby kupić nową subskrypcję, z menu **Partner Center** wybierz pozycję **Klienci,** wybierz klienta, którego chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje.**

2. Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.

Klient powinien teraz mieć zarówno starą, jak i nową subskrypcję, starą autonomiczną subskrypcję usługi Kaizala Pro i nową "docelową" subskrypcję, na przykład opcja 1 — Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Ponowne przypisanie bieżących licencji użytkowników

1. Aby ponownie przypisać licencje użytkowników klienta, z menu usługi Partner Center wybierz pozycję **Klienci,** wybierz klienta, który przenosisz, **a** następnie wybierz pozycję Użytkownicy i **licencje.** Zostanie otwarta strona Użytkownicy i licencje klienta.

2. Aby ponownie przypisać licencję użytkownika, wybierz użytkownika do ponownego przypisania, a następnie wybierz pozycję **Zarządzaj licencjami.**

3. Na stronie **Manage licenses (Zarządzanie** licencjami) wyczyść pole wyboru Kaizala Pro Standalone license (Licencja autonomiczna usługi Kaizala Pro) i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący.

4.  Wybierz pozycję **Prześlij**. Strona potwierdzenia zawiera listę nowych przypisań licencji. Kontynuuj ten sam proces dla innych użytkowników, którzy potrzebują przypisań licencji.

### <a name="c-cancel-old-subscription"></a>C. Anulowanie starej subskrypcji

Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie klienta.

1.  Z menu **Partner Center** wybierz pozycję **Klienci.** Wybierz klienta, którego subskrypcję anulujesz.

2.  Na stronie szczegółów subskrypcji ustaw dla subskrypcji wartość **Wstrzymano**.

3.  Wybierz pozycję **Prześlij**.

Stara subskrypcja zostanie wstrzymana, a nowa subskrypcja będzie aktywna. Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni. Klient nie ponosi żadnych dodatkowych kosztów dla starej subskrypcji.
