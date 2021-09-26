---
title: Nowe promocje handlowe
ms.topic: article
ms.date: 09/24/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących odkrywania i kupowania promocji.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8abd34ff7cc47edf59be6532dcc7e9c7e0dd1533
ms.sourcegitcommit: dd900161830c59bcf3c5d700d524436ee05cd987
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128714151"
---
# <a name="introduction-new-commerce-promotions"></a>Wprowadzenie: Nowe promocje handlowe

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży
- Administrator globalny

> [!Note] 
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Firma Microsoft będzie obsługiwać promocje w nowym handlu. Te promocje będą mieć różne kwoty rabatów i czasy trwania. 

## <a name="discovering-promotions"></a>Odkrywanie promocji ##

Partnerzy mogą odkrywać promocje, odwiedzając zaległość promocji lub wywołując interfejs API getPromotions. Lista prac dotyczących promocji to lista dostępnych promocji firmy Microsoft, o których partnerzy muszą wiedzieć. Lista jest stale utrzymywana i aktualizowana co miesiąc. 


## <a name="operationalize-promotions"></a>Operationalize promotions (Z operationalize promotions) ##

Partnerzy mogą zrealizować promocje, wdrażając interfejs API getPromotions. Ten interfejs API zwraca wszystkie promocje istniejące dla danego rynku (kraju klienta) i segmentu. Interfejs API zwraca listę promocji i ważnych informacji, aby pomóc partnerowi zrozumieć, które promocje są dostępne dla klientów w różnych krajach. 


Interfejs API getPromotions zawiera następujące dane dotyczące danego poziomu:

- Czas trwania promocji
- Rabat procentowy dla promocji
- Produkty i jednostki SKU, dla których jest dostępna promocja

Promocje są stosowane przez centrum partnerskie, gdy partner kupi dla produktu sku produktu, dla których jest dostępna. Promocje dla partnerów są dostępne w interfejsie użytkownika katalogu centrum partnerskiego w szczegółach dotyczących wersji SKU produktu. Mogą oni kliknąć pozycję "Wyświetl szczegóły promocji", aby uzyskać więcej informacji o promocji. Do wyświetlania szczegółów promocji można uzyskać dostęp z widoku sku strony katalogu, strony przeglądu przed przesłaniem zakupu, potwierdzenia po przesłaniu zamówienia oraz strony historii zamówienia. 

## <a name="verify-eligibility"></a>Weryfikowanie uprawnień ##

Partnerzy mogą sprawdzić, czy zakup klienta kwalifikuje się do promocji, wyświetlając informacje na stronie przeglądu w Centrum partnerskim przed zakupem produktu. Partnerzy mogą również wywołać interfejs API verifyPromotionEligibility ,przekazując identyfikator dzierżawy klienta i identyfikator promocji. Wywołanie zwraca wartość true, jeśli klient jest uprawniony. Jeśli klient nie kwalifikuje się, interfejs API zwraca warunki, które nie zostały spełnione, aby można było skorzystać z promocji. 

Partnerzy mogą wywołać weryfikację uprawnień i uzyskać wyniki z powrotem. Błędy uprawnień mogą być oparte na liczbach miejsc, niezgodnych warunkach lub limitach liczby razy, gdy można zastosować promocję do sku produktu klienta.

>[!IMPORTANT]
> Partnerzy powinni zweryfikować promocje przed przesłaniem transakcji. Jeśli na Partner Center  partnerów nie zostanie wyświetlony promocję, nie zostanie ona zastosowana do transakcji, partner otrzyma cenę bez promocji. Partnerzy mogą również sprawdzić interfejs API elementu wiersza koszyka, aby sprawdzić, czy przed przesłaniem transakcji jest obecna promocja. Partnerzy mogą wywołać interfejs API weryfikacji promocji przed przesłaniem transakcji, aby sprawdzić, czy kombinacja sku produktu klienta kwalifikuje się do promocji, a jeśli nie, przyczyny niekwalifikowania się.

Istnieją trzy powody, dla których klient może nie kwalifikować się do promocji. Te typy, które nie są kwalifikowane, zostaną zwrócone w interfejsie API weryfikacji promocji w przypadkach, gdy klient nie jest uprawniony.

### <a name="seat-count"></a>Liczba miejsc ###

Wiele promocji ma stanowisko, które może mieć maksymalnie 2400 stanowisk. W takich przypadkach transakcja, w tym ponad 2400, zostanie przesłana po cenach bez promocji. Te liczby stanowisk są również wymuszane podczas dodawania stanowisk do subskrypcji podyscytowania z tymi limitami. Partnerzy otrzymają komunikat o błędzie, jeśli spróbują zwiększyć subskrypcję z obsługą promocji poza limity. Limity liczby miejsc w ramach promocji są wymuszane między partnerami, więc jeśli jeden partner kupi podwyżkę o 2300 miejsc z limitem liczby miejsc w promocji, drugi partner, który kupi 200 stanowisk, otrzyma cenę subskrypcji po cenie bez podwyższenia. Poziom promocji jest wymuszany na poziomie sku produktu, w ramach transakcji partnera, dzięki czemu partner może uzyskać ceny promocyjny za 2400 miejsc w programie Microsoft 365 E3, a także za inną Microsoft 365 E5. Partnerzy mogą wywołać interfejs [API subskrybowanych SKU,](/partner-center/develop/get-a-list-of-available-licenses) aby zobaczyć, ile licencji klient ma dla danej aprowizowanego interfejsu SKU.

### <a name="term"></a>Okres ###

Ograniczenia terminów definiują, które warunki SKU produktu są dopasowane do danego promocji. Wiele promocji ma różne rabaty zdefiniowane w zależności od terminu. Jeśli partner przesłał transakcję i termin nie jest dopasowany do promocji, oczekuje, że transakcja będzie po cenie bez podwyższenia. Przykładami terminów są *roczne lub* *miesięczne*.

### <a name="first-purchase"></a>Pierwszy zakup ###

Niektóre promocje wymuszają nabywanie tylko raz. Partner zobaczy uprawnienie fałsz przy użyciu interfejsu API weryfikacji uprawnień z typem błędu *FirstPurchase*.  Partner może nadal zakupić podaną sku produktu, ale subskrypcja będzie w cenie bez podwyżsienia ceny. To ograniczenie dotyczy 1 klienta, a nie partnera. Gdy klient ma podyscytować tę regułę, nie może uzyskać drugiego wystąpienia promocji zastosowanego przez drugiego partnera.

## <a name="promotions-and-renewals"></a>Promocje i odnowienia ##

Rabaty promocyjny po zastosowaniu są stosowane na okres zakupu. Subskrypcje z zastosowanymi promocjami zachowają cenę promocyjnyą, jeśli data odnowienia znajduje się w zakresie dat trwania promocji. Odnowienia poza zakresem dat trwania promocji zostaną odnowione na cenę bez podwyżsenia ceny (z cennika). Partnerzy mogą śledzić stan odnowienia do punktów cenowych na stronie szczegółów subskrypcji i w instrukcjach odnawiania danych subskrypcji getSubscription.

## <a name="promotions-and-upgrades"></a>Promocje i uaktualnienia ##
Partnerzy, którzy uaktualnią subskrypcję do innej wersji SKU, pozostawią cenę za podwyżsenie ceny. Ta akcja występuje, ponieważ podwyżsenie zostało skonfigurowane dla opuszczonej przez siebie wersji SKU podczas uaktualniania do innej wersji SKU. Partnerzy, którzy przejdą do wersji SKU, która może podwyższyć swój koszt, nie otrzymają automatycznie ceny promocji. Jeśli potrzebują lub chcą uzyskać cenę za podwyżkę dla tej, do której chcą przejść, muszą ręcznie zakupić nową subskrypcję jako nową subskrypcję. Obecnie promocje są stosowane tylko w przypadku nowych zakupów i odnowień subskrypcji.

## <a name="promotions-and-migrations"></a>Promocje i migracje ##
Partnerzy mogą migrować subskrypcje swoich klientów z tradycyjnych subskrypcji Microsoft 365/Dynamics 365 do nowych wersji handlowych swoich subskrypcji. Migracje są dostępne zarówno z interfejsu użytkownika Partner Center, jak i z wywoływania interfejsów API migracji. Partnerzy, którzy przeprowadzają migrację z tradycyjnej subskrypcji do nowego handlu, otrzymają promocję, jeśli migrują, o ile ich wersja SKU produktu jest dostosowana do definicji promocji. Partnerzy powinni wywołać interfejs API weryfikacji uprawnień, aby upewnić się, że docelowa cena sku produktu zostanie wywołana przed migracją.




