---
title: Zarządzanie rezerwacjami platformy Azure dla klientów
description: Dowiedz się, jak zarządzać rezerwacjami platformy Azure dla klienta, w tym jak anulować rezerwację, wymienić rezerwację lub zażądać zwrotu kosztów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 627c6f8d09a904e7d988c4229ec10eeac38dc2e9
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841474"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Zarządzanie rezerwacjami, anulowanie ich, wymiana Microsoft Azure zwrot kosztów dla klientów

**Odpowiednie role:** Agent administracyjny | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży | Administrator zarządzania użytkownikami

W tym artykule wyjaśniono, jak zarządzać rezerwacjami platformy Azure dla klienta, w tym jak anulować rezerwację, wymienić rezerwację lub zażądać zwrotu kosztów.

> [!NOTE]
> Ten artykuł dotyczy tylko partnerów w programie Dostawca rozwiązań w chmurze (CSP). Klienci korzystający z innych typów subskrypcji (takich jak subskrypcje z płatnością zgodnie z użyciem, indywidualny, Umowa z Klientem Microsoft lub Enterprise Agreement) powinni zamiast tego przeczytać tę dokumentację rezerwacji platformy [Azure.](/azure/cost-management-billing/reservations)

Aby zarządzać rezerwacjami platformy Azure klientów po zakupie, należy wybrać klienta i rezerwację, którą chcesz zarządzać w usłudze Partner Center, a następnie wprowadzić zmiany w rezerwacji w Azure Portal.

1. Aby rozpocząć, wybierz **pozycję Klienci** z menu Partner Center a następnie wybierz klienta, którego rezerwacjami chcesz zarządzać. 

2. W menu strony szczegółów klienta wybierz pozycję **Rezerwacje platformy Azure,** a następnie wybierz określoną rezerwację, którą chcesz zarządzać.  

3. W **obszarze** Akcje wybierz **pozycję Zarządzaj,** aby przejść do rekordu rezerwacji klienta w Azure Portal. Na stronie szczegółów rezerwacji wykonaj poniższe kroki, aby wykonać zadania.  

    | **Wybierz**   | **Do**    |
    |:-----------------------------|:-----------------|
    | **Omówienie**   | Wyświetlanie szczegółów rezerwacji klienta, w tym daty wygaśnięcia, zakresu i danych użycia. **UWAGA** Wybierz **pozycję Zwrot,** aby utworzyć żądanie pomocy technicznej dotyczące zwrotu proporcjonalnie. Wybierz **Exchange,** aby utworzyć wniosek o pomoc techniczną w celu wymiany nieużywanej części okresu rezerwacji.  
    | **Access Control (IAM)**   | Zarządzanie dostępem do informacji o rezerwacji klienta.|
    | **Konfiguracja**   | Zmień zakres rezerwacji i/lub subskrypcję platformy Azure, z która jest skojarzona rezerwacja.    |
    | **Właściwości**   | Wyświetl właściwości rezerwacji i skopiuj do schowka identyfikator rezerwacji i identyfikator zamówienia rezerwacji. **UWAGA** Pomoc techniczna może poprosić o identyfikator rezerwacji i identyfikator zamówienia rezerwacji w przypadku żądania pomocy technicznej w imieniu klienta.    |
    | **Nowy wniosek o pomoc techniczną**    | Poproś o pomoc Pomoc techniczna Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Anulowanie lub wymiana rezerwacji

Jeśli w dowolnym momencie potrzeby biznesowe klienta zmienią się, może on chcieć anulować rezerwację i uzyskać zwrot lub wymienić proporcjonalną kwotę zwrotu rezerwacji na cenę nowej rezerwacji.

W obu tych scenariuszach firma Microsoft zwraca ci kwotę, dzięki czemu możesz zarządzać wynikowe transakcje finansowe z klientami. Firma Microsoft nie kontaktuje się bezpośrednio z klientami w sprawie rozliczeń, anulowania ani zwrotów kosztów.

### <a name="how-cancellations-work"></a>Jak działają anulowania

Klienci mogą zażądać anulowania rezerwacji w dowolnym momencie (kwota zwrotu ograniczona do 50 000 USD rocznie). Anulowanie rezerwacji umożliwia klientowi zwrócenie kwoty pozostałych miesięcy rezerwacji platformy Azure za opłatą za wcześniejsze zakończenie. Pozostałe saldo proporcjonalnie pomniejszone o opłatę za wcześniejsze zakończenie jest zwracane na Twoje konto, dzięki czemu możesz uzyskać zwrot kosztów konta klienta. 

Poniżej znajdują się szczegółowe informacje o anulowaniu i opłatach.


|**Data anulowania**<br> (dni)   |**Użycie**    |**Środki**  |**Wczesne zakończenie**<br> Opłata    |**Limit zwrotu pieniędzy** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 lub mniej                         | Nie          | 100%       | Nie                              | 50 000 USD   |
|5 lub mniej                         | Yes         | Pro do oceny  | Nie                              | 50 000 USD   |
|Więcej niż 5                        | Nie          | Pro do oceny  | 12%                             | 50 000 USD   |
|Więcej niż 5                        | Yes         | Pro do oceny  | 12%                             | 50 000 USD   |

### <a name="how-exchanges-work"></a>Jak działają wymiany 

Jeśli klient chce kupić inną rezerwację niż ta, która została pierwotnie kupiona od Ciebie, może zażądać wymiany. Wymiana rezerwacji może być atrakcyjną alternatywą dla anulowania rezerwacji, ponieważ umożliwia klientowi użycie proporcjonalnej kwoty zwrotu na cenę nowej rezerwacji. 

Proporcjonalna kwota zwrotu jest uwzględniana na Twoim koncie, dzięki czemu możesz zaoferować klientowi wymianę.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Żądanie zwrotu lub wymiany w imieniu klienta

Aby złożyć wniosek o pomoc techniczną w sprawie zwrotu lub wymiany w imieniu klientów, należy wybrać klienta i rezerwację w Partner Center, a następnie utworzyć wniosek o pomoc techniczną w Azure Portal. 

>[!NOTE]
>Pomoc techniczna Microsoft mogą poprosić o podanie identyfikatora rezerwacji i identyfikatora zamówienia rezerwacji. Te informacje można znaleźć na stronie Właściwości rezerwacji **w** Azure Portal.

1. Aby rozpocząć, wybierz **pozycję Klienci** z menu Partner Center a następnie wybierz klienta, który chce uzyskać zwrot. 

2. Na stronie szczegółów klienta wybierz pozycję **Rezerwacje platformy Azure,** a następnie wybierz konkretną rezerwację, dla których klient chce otrzymać zwrot kosztów.  

3. W **obszarze** Akcje wybierz **pozycję Zwrot,** aby przejść do rekordu rezerwacji klienta w Azure Portal i zainicjować żądanie pomocy technicznej.  

4. Na stronie **Nowy wniosek o** pomoc techniczną wykonaj poniższe kroki, aby zażądać zwrotu pieniędzy. Po **każdym kroku** wybierz pozycję Dalej. 

   |**Krok**                    |**Wybór**    |
   |:---------------------------|:-----------------|
   |**1 Podstawowe informacje**                |Typ problemu: Rozliczenia.  |
   |**2 Problem**               |Typ problemu: Zarządzanie rezerwacjami. Kategoria: Wymiany i zwroty. |
   |**3 Informacje kontaktowe**   |Wybierz preferencje i wprowadź wymagane informacje. 

5. Po **utworzeniu wybierz** pozycję Utwórz.

## <a name="azure-reservations-resources"></a>Zasoby rezerwacji platformy Azure

|**Aby uzyskać informacje o**   |**Przeczytaj to**    |
|:-----------------------------|:-----------------|
|Rezerwacje platformy Azure w programie CSP — omówienie  | [Sprzedaż Microsoft Azure wystąpień zarezerwowanych](azure-reservations.md) |
|Kupowanie rezerwacji platformy Azure dla klientów w Partner Center   | [Kupowanie rezerwacji platformy Azure](azure-reservations-buying.md) |
|Określanie prawidłowego rozmiaru maszyny wirtualnej i weryfikowanie użycia maszyny wirtualnej klienta   | [Rozmiar maszyny wirtualnej dla maksymalnego użycia rezerwacji platformy Azure](azure-usage.md)   |
|Kupowanie rezerwacji platformy Azure przy użyciu interfejsu PARTNER CENTER API | [Informacje Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji Partner Center dewelopera   |
|Udzielanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure w ramach zakupionej dla nich subskrypcji. | [Nadaj klientom uprawnienia do zakupu własnych rezerwacji platformy Azure](give-customers-permission.md)   |