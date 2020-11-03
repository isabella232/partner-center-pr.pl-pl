---
title: Migrowanie subskrypcji usługi kaizala Pro do Microsoft365
description: Dowiedz się, jak migrować subskrypcje usługi kaizala Pro do wersji Microsoft365 lub pakietu Office 365. Przeczytaj ten artykuł, aby uzyskać więcej informacji na temat przechodzenia do klientów.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530519"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Migrowanie subskrypcji autonomicznych usługi kaizala Pro do wersji Microsoft365 lub pakietu Office 365

Począwszy od 1 lipca 2020, firma Microsoft kończy sprzedaż usługi autonomicznej usługi kaizala Pro. Klienci nie będą już mogli kupować nowych subskrypcji usługi kaizala Pro po tej dacie, a istniejące subskrypcje usługi kaizala Pro nie będą odnawiane automatycznie po ich wygaśnięciu.

Aby zapewnić ciągłość dla klientów, należy przejść do klientów z wygaśnienymi subskrypcjami usługi kaizala Pro do obsługiwanej jednostki SKU wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.

W przypadku korzystania z interfejsu API (z końcówką lub Centrum partnerskiego) można odkrywać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew ustawioną na wartość false: `auto renew = False` .

Dla subskrypcji E4 zostanie ustawiona wartość `auto renew=False` 1 lipca 2020. Klientów można przenieść do nowego planu w dowolnym momencie.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Autonomiczne plany zastępcze usługi kaizala Pro

Dzięki nowym planom klienci mogą korzystać z nowszych funkcji i funkcji w Microsoft 365. Szczegóły cennika znajdują się na liście cen i macierzy list oferty w centrum partnerskim.

- [**Microsoft 365 dla firm**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), w tym:  
   - Microsoft 365 Business podstawowa
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 teraźniejszości, w**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)tym:
   - Microsoft 365 F3 (dawniej Microsoft 365 F1) i Office 365 F3
    
- [**Microsoft 365 dla przedsiębiorstw**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), w tym: 
   - Pakiet Office 365 E1
   - Microsoft 365 E3 i pakiet Office 365 E3
   - Microsoft 365 E5 i Office 365 E5

- [**Microsoft 365 dla edukacji**](https://www.microsoft.com/education/buy-license/microsoft365), w tym: 
    - Microsoft 365 a1 i Office 365 a1
    - Microsoft 365 A3 i Office 365 a3
    - Microsoft 365 A5 i Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Przejście klientów do nowych planów produktu

Firma Microsoft ciągle oferuje swoim partnerom nowe produkty i usługi. W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub przeprowadzenie migracji swoich subskrypcji z jednostek SKU, które ostatecznie zostaną zamknięte. Migrowanie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących czynności:

A. Kup nową subskrypcję

B. Ponowne przypisanie bieżących licencji użytkownika

C. Anuluj starą subskrypcję


## <a name="migrate-your-customers-to-new-plans"></a>Migrowanie klientów do nowych planów

### <a name="a-purchase-the-new-subscription"></a>A. Kup nową subskrypcję

1. Aby kupić nową subskrypcję, w menu **Centrum partnerskiego** wybierz pozycję **klienci** , wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje** .

2. Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij** .

Klient powinien mieć teraz zarówno stare, jak i nowe subskrypcje, starszą subskrypcję autonomiczną usługi kaizala Pro i nową subskrypcję "target", na przykład opcję 1-Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Ponowne przypisanie bieżących licencji użytkownika

1. Aby ponownie przypisać licencje użytkowników klienta, w menu **Centrum partnerskiego** wybierz pozycję **klienci** , wybierz przenoszony klient, a następnie wybierz pozycję **Użytkownicy i licencje** . Zostanie otwarta strona użytkownicy i licencje klienta.

2. Aby ponownie przypisać licencję użytkownika, wybierz użytkownika, którego chcesz przypisać ponownie, a następnie wybierz pozycję **Zarządzaj licencjami** .

3. Na stronie **Zarządzanie licencjami** wyczyść pole wyboru licencja autonomiczna usługi kaizala Pro, a następnie wybierz nowy plan usługi dla subskrypcji, do której jest przenoszony klient.

4.  Wybierz pozycję **Prześlij** . Na stronie potwierdzenia wyświetlane są nowe przypisania licencji. Kontynuuj ten sam proces dla innych użytkowników, którzy potrzebują przypisań licencji.

### <a name="c-cancel-old-subscription"></a>C. Anuluj starą subskrypcję

Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie klienta.

1.  W menu **Centrum partnerskiego** wybierz pozycję **Customers** . Wybierz klienta, którego subskrypcję chcesz anulować.

2.  Na stronie Szczegóły subskrypcji Ustaw subskrypcję na **zawieszone** .

3.  Wybierz pozycję **Prześlij** .

Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna. Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach. Klient nie wiąże się z żadnymi dodatkowymi kosztami dla starej subskrypcji.
