---
title: Zarządzanie rezerwacjami platformy Azure dla klientów
description: Dowiedz się, jak zarządzać rezerwacjami platformy Azure dla klienta, w tym o sposobach anulowania rezerwacji, wymianie rezerwacji lub zażądać zwrotu pieniędzy.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 937a7268caa5ae7872f8a3ec6dcb05f56dd9fbe5
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529919"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Zarządzanie rezerwacjami, anulowanie, wymiana lub zwrot Microsoft Azure dla klientów

**Dotyczy**

- Centrum partnerskie
- Microsoft Azure Portal 
- Partnerzy w programie CSP

**Odpowiednie role**

- Agent administracyjny
- Administrator globalny
- Agent pomocy technicznej
- Agent sprzedaży
- Administrator zarządzania użytkownikami

> [!NOTE]
> Ten artykuł ma zastosowanie tylko do partnerów w programie Cloud Solution Provider (CSP). Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).

Aby zarządzać księgowaniem zakupów platformy Azure dla klientów, wybierz klienta i rezerwację, którą chcesz zarządzać w centrum partnerskim, a następnie wprowadź zmiany w rezerwacji w Azure Portal.

1. Aby rozpocząć, wybierz opcję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, którego rezerwacje chcesz zarządzać. 

2. Na stronie szczegółów klienta wybierz pozycję **rezerwacje platformy Azure** , a następnie wybierz konkretną rezerwację, którą chcesz zarządzać.  

3. W obszarze **Akcje** wybierz pozycję **Zarządzaj** , aby przejść do rekordu rezerwacji klienta w Azure Portal. Na stronie Szczegóły rezerwacji postępuj zgodnie z poniższymi instrukcjami, aby wykonać zadania.  

    | **Wybierz**   | **Działanie**    |
    |:-----------------------------|:-----------------|
    | **Omówienie**   | Wyświetlanie szczegółów rezerwacji klienta, w tym daty wygaśnięcia, zakresu i danych użycia. **Uwaga** Wybierz pozycję **zwrot** , aby utworzyć żądanie pomocy technicznej dotyczące zwrotnego zwrotu. Wybierz pozycję **Exchange** , aby utworzyć żądanie pomocy technicznej w celu wymiany nieużywanej części okresu rezerwacji.  
    | **Access Control (IAM)**   | Zarządzanie dostępem do informacji o rezerwacji klienta.|
    | **Konfiguracja**   | Zmień zakres rezerwacji i/lub subskrypcję platformy Azure, z którą skojarzona jest rezerwacja.    |
    | **Właściwości**   | Wyświetl właściwości zastrzeżenia i skopiuj do schowka identyfikator rezerwacji i identyfikator zamówienia rezerwacji. **Uwaga** Pomoc techniczna może prosić o identyfikator rezerwacji i identyfikator zamówienia rezerwacji w przypadku żądania obsługi w imieniu klienta.    |
    | **Nowy wniosek o pomoc techniczną**    | Zażądaj pomocy z pomoc techniczna firmy Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Anulowanie lub wymiana rezerwacji

Jeśli w dowolnym momencie konieczna jest zmiana firmy klienta, może zaistnieć potrzeba anulowania rezerwacji i uzyskania zwrotu lub zamienienia kwoty zwrotu proporcjonalnie do użycia w ramach ceny nowej rezerwacji.

W obu tych scenariuszach firma Microsoft ponownie przyniesie kwotę do Ciebie, aby można było zarządzać uzyskanymi transakcjami finansowymi klientów. Firma Microsoft nie kontaktuje się bezpośrednio z klientami w zakresie rozliczeń, anulowania lub zwrotów.

### <a name="how-cancellations-work"></a>Jak działają anulowanie

Klienci mogą zażądać anulowania rezerwacji w dowolnym momencie (kwota zwrotu w wysokości $50 000 rocznie). Anulowanie rezerwacji umożliwia klientowi zwrócenie kwoty pozostałych miesięcy rezerwacji na platformę Azure w celu uzyskania wcześniejszej opłaty za zakończenie. Pozostałe obniżone saldo, pomniejszone o opłatę za wcześniejsze zakończenie, jest spłacane na Twoje konto, aby można było zwrócić konto klienta. 

Poniżej znajdują się szczegóły i opłaty dotyczące anulowania.


|**Data anulowania**<br> dni   |**Użycie**    |**Środki**  |**Wczesne zakończenie**<br> wysokości    |**Zakończenie zwrotu** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 lub mniej                         | Nie          | 100%       | Nie                              | $50 000 USD   |
|5 lub mniej                         | Tak         | Proporcjonalnie do  | Nie                              | $50 000 USD   |
|Więcej niż 5                        | Nie          | Proporcjonalnie do  | 12%                             | $50 000 USD   |
|Więcej niż 5                        | Tak         | Proporcjonalnie do  | 12%                             | $50 000 USD   |

### <a name="how-exchanges-work"></a>Jak działają wymiany 

Jeśli klient chce zakupić inną rezerwację niż ta, która pierwotnie kupiła, może zażądać wymiany. Wymiana rezerwacji może być atrakcyjną alternatywą do anulowania rezerwacji, ponieważ pozwala klientowi na użycie proporcjonalnie do ceny za nową rezerwację. 

Kwota proporcjonalnie do kwoty zwrotu jest księgowana na koncie, dzięki czemu można zaoferować klientowi wymianę.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Żądaj zwrotu pieniędzy lub wymiany w imieniu klienta

Aby wysłać żądanie pomocy technicznej dotyczące zwrotów lub wymiany w imieniu klientów, należy wybrać klienta i rezerwację w centrum partnerskim, a następnie utworzyć żądanie pomocy technicznej w Azure Portal. 

>[!NOTE]
>Pomoc techniczna firmy Microsoft agenci mogą poprosił o podanie identyfikatora rezerwacji i identyfikatora zamówienia rezerwacji. Te informacje można znaleźć na stronie **Właściwości** zastrzeżenia w Azure Portal.

1. Aby rozpocząć, wybierz opcję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, który chce zwrócić zwrot. 

2. Na stronie szczegółów klienta wybierz opcję **rezerwacje platformy Azure** , a następnie wybierz konkretną rezerwację, której klient chce ponownie obfundować.  

3. W obszarze **Akcje** wybierz pozycję **zwrot** , aby przejść do rekordu rezerwacji klienta w Azure Portal i zainicjować żądanie pomocy technicznej.  

4. Na stronie **nowe żądanie obsługi** postępuj zgodnie z poniższymi instrukcjami, aby zażądać zwrotu. Po każdym kroku wybierz pozycję **dalej** . 

   |**Krok**                    |**Opcji**    |
   |:---------------------------|:-----------------|
   |**1 — podstawowe**                |Typ problemu: rozliczenia.  |
   |**2 problem**               |Typ problemu: Zarządzanie rezerwacjami. Kategoria: wymiany i zwroty. |
   |**3 informacje kontaktowe**   |Wybierz swoje preferencje i wprowadź wymagane informacje. 

5. Po zakończeniu wybierz pozycję **Utwórz** .

## <a name="azure-reservations-resources"></a>Zasoby rezerwacji platformy Azure

|**Aby uzyskać informacje na temat**   |**Przeczytaj to**    |
|:-----------------------------|:-----------------|
|Omówienie rezerwacji platformy Azure w programie CSP  | [Sprzedaj Microsoft Azure wystąpienia zarezerwowane](azure-reservations.md) |
|Kupowanie rezerwacji platformy Azure dla klientów w centrum partnerskim   | [Kupowanie rezerwacji platformy Azure](azure-reservations-buying.md) |
|Określ prawidłowy rozmiar maszyny wirtualnej i Sprawdź użycie maszyny wirtualnej klienta   | [Rozmiar maszyny wirtualnej dla maksymalnego użycia zastrzeżenia platformy Azure](azure-usage.md)   |
|Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Centrum partnerskiego | [Zakup Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji dla deweloperów Centrum partnerskiego   |
|Przyznanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure z subskrypcji, która została zakupiona. | [Przyznaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure](give-customers-permission.md)   |