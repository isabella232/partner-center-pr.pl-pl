---
title: Nowe promocje handlowe
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących odkrywania i kupowania promocji.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc2d52dd444168b32f0cadaeccec1e6d906348d1
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/16/2021
ms.locfileid: "127894068"
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



## <a name="promotions-and-renewals"></a>Promocje i odnowienia ##

Rabaty promocyjny po zastosowaniu są stosowane na okres zakupu. Subskrypcje z zastosowanymi promocjami zachowają cenę promocyjnyą, jeśli data odnowienia znajduje się w zakresie dat trwania promocji. Odnowienia poza zakresem dat trwania promocji zostaną odnowione na cenę bez podwyżsenia ceny (z cennika). Partnerzy mogą śledzić stan odnowienia do punktów cenowych na stronie szczegółów subskrypcji i w instrukcjach odnawiania danych subskrypcji getSubscription.


## <a name="promotions-and-upgrades"></a>Promocje i uaktualnienia ##
Partnerzy, którzy uaktualnią subskrypcję do innej wersji SKU, pozostawią cenę za podwyżsenie ceny. Ta akcja występuje, ponieważ podwyżsenie zostało skonfigurowane dla opuszczonej przez siebie wersji SKU podczas uaktualniania do innej wersji SKU. Partnerzy, którzy przejdą do wersji SKU, która może podwyższyć swój koszt, nie otrzymają automatycznie ceny promocji. Jeśli potrzebują lub chcą uzyskać cenę za podwyżkę dla tej, do której chcą przejść, muszą ręcznie zakupić nową subskrypcję jako nową subskrypcję. Obecnie promocje są stosowane tylko w przypadku nowych zakupów i odnowień subskrypcji.



