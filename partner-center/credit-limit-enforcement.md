---
title: Wymuszanie limitu środków
ms.topic: how-to
ms.date: 05/11/2021
description: Dowiedz się więcej na temat limitu środków i sposobu jego obliczania. Zawiera często zadawane pytania.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 32dc94a4bd85160a02a4be880469f713d98449ba
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837972"
---
# <a name="credit-limit-enforcement-cle"></a>Wymuszanie limitu środków (CLE)

**Odpowiednie role:** Administrator rozliczeń

## <a name="your-credit-limit-and-how-it-works"></a>Limit środków i sposób jego działania

Limit środków to maksymalna kwota (w dolarach amerykańskich), którą partner może wydać na zakup produktów lub subskrypcji w Partner Center. W przypadku przekroczenia limitu środków nie będzie można dokonać nowych zakupów, dopóki nie zostanie dokonana wystarczająca płatność. Istniejące subskrypcje będą nadal nieprzerwane.

Limity środków mają zastosowanie do ofert w planie platformy Azure, rezerwacjach platformy Azure, oprogramowaniu, witrynie Marketplace, platformie Azure 145 P, Office i produktach Dynamics. Limity środków nie mają zastosowania do odnawiania i bieżącego użycia.

Przypisujemy Limit środków na poziomie dzierżawy w okresie dołączania. Opieramy go na prognozowanych przychodach, zakupach i historii płatności. Następnie użyjemy następującej formuły do obliczenia dostępnego salda:

**[Limit środków — (Zakup przychodzący + Zaległe niezapłacone faktury + Nierozlicone opłaty — nadpłata)]**

## <a name="frequently-asked-questions"></a>Często zadawane pytania

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>Czy limit środków został ustawiony na poziomie dzierżawy, czy na poziomie globalnym?

Poziom dzierżawy. Załóżmy na przykład, że prowadzisz działalność w Stanach Zjednoczonych, Kanadzie i Japonii. Jeśli dzierżawa w Kanadzie osiągnie limit środków, ta dzierżawa otrzyma powiadomienie, gdy spróbuje dokonać zakupu w Partner Center. Nie będzie to mieć wpływu na pozostałe dzierżawy. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>Jeśli przekroczą limit środków, czy mogę kontynuować obsługę istniejących klientów i subskrypcji z pełnym dostępem?

Tak. Istniejące subskrypcje klientów będą kontynuowane bez zakłóceń. Nie można jednak kupić nowych subskrypcji dla klientów.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>Czy CLE ma zastosowanie zarówno do partnerów rozliczanych bezpośrednio, jak i dostawców pośrednich?

Tak, dotyczy to obu tych sytuacji.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>Kiedy po przesłaniu płatności w celu przywrócenia konta mogę kupić więcej subskrypcji? 

Powinno być możliwe wznowienie zakupu w ciągu 24 godzin od płatności przy założeniu, że firma Microsoft otrzymała wszystkie wymagania dotyczące kontynuowania procesu sprawdzania środków.

### <a name="how-can-i-check-my-credit-limit"></a>Jak sprawdzić limit środków?

Skontaktuj się [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) z nami, aby wyświetlić limit środków i uzyskać informacje o ostatnich zakupach.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>Czy faktury, które są w sporze, są wliczane do limitu środków?

Tak. Możesz jednak skontaktować się z firmą Microsoft na stronie , [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) aby rozwiązać ten problem.

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>Jak szybko usłyszę, jeśli napiszę do ucmwrcsp@microsoft.com ?

Odpowiedź powinna być wyższa niż 24 godziny. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Jakie kryteria są stosowane przez firmę Microsoft do ustawiania limitu środków partnera?

Limit środków określamy na podstawie prognozowanych przychodów, zakupów i historii płatności.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>Czy limit środków jest obecnie wymuszany w nowym doświadczeniu handlowym?

Tak. Limity środków mają zastosowanie do wszystkich programów i produktów CSP w Partner Center.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>KtoTo otrzyma powiadomienie, gdy moja organizacja zbliża się do limitu środków?

Powiadomienie powinno zostać otrzymać osoba kontaktowa ds. należności dla konta finansowego Twojej organizacji.

## <a name="next-steps"></a>Następne kroki

[Billing basics (Podstawowe informacje dotyczące rozliczeń)](./billing-basics.md)
