---
title: Kwota uzyskana przez partnera w przypadku usług zarządzanych
ms.topic: article
ms.date: 11/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób środki na korzystanie z usługi zarządzanej przez partnerów firmy Microsoft są obliczane i płatne oraz jak zapewnić, że masz odpowiednie uprawnienia.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 97af446c4021e9785833374131eee2f08431b5fe
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474312"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Jak są obliczane i wypłacane środki zarobione przez partnera

**Odpowiednie role**

- Administrator globalny
- Administrator użytkowników
- Agent administracyjny
- Administrator rozliczeń
- Agent sprzedaży

Środki na korzystanie z partnerów w przypadku usług zarządzanych (PEC) są rozpoznawane i nagradzane przez partnerów, którzy są właścicielami 24x7 kontroli działania IT i zarządzania częściami lub całym środowiskiem platformy Azure. Domyślnie w programie CSP partnerzy otrzymują niezbędne prawa dostępu do subskrypcji klienta, umożliwiając im wykonywanie przez 24 X 7 operacyjnych zarządzania i kontroli nad zasobami w ramach subskrypcji. Dodatkowe sposoby, w których klient może udostępnić dostęp dla partnera transakcji, został opisany w poniższej sekcji. Kwota faktury miesięcznej to wartość netto środków zdobytych przez partnera. Partnerzy mogą zobaczyć szczegóły dotyczące PEC w ich comiesięcznym pliku rekonesans. Aby uzyskać dodatkowe sposoby udostępniania dostępu dla partnera transakcji, przeczytaj artykuł [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md).

Przeczytaj również temat [przywracanie uprawnień administratora dla subskrypcji CSP platformy Azure](revoke-reinstate-csp.md)

## <a name="important-eligibility-and-calculation-information"></a>Ważne informacje dotyczące uprawnień i obliczeń

- Partner powinien mieć aktywną umowę MPN i ważną rolę RBAC, aby otrzymać środki na korzystanie z zasobów platformy Azure, którymi zarządzają. 

- W przypadku dostawców pośrednich i ich pośrednich odsprzedawców Dostawca pośredni będzie uprawniony do PEC, jeśli dostawca pośredni lub pośredni odsprzedawca lub obie osoby 24x7 kontrolę operacyjną i zarządza zasobami platformy Azure klienta w dostawcy usług kryptograficznych.

- Komputer PEC jest skojarzony z naliczaniem (odpłatnym) użyciem wartości platformy Azure klienta w programie CSP zarządzanym przez partnera. Komputer PEC jest dostępny tylko dla partnerów w dostawcy CSP rozliczanych przez firmę Microsoft (Dostawca pośredni i bezpośredni partner Bill). 

- Kwalifikujące się usługi: środki na korzystanie z partnerów mają zastosowanie do usług wymienionych w **cenniku zużycia planu platformy Azure** , które partnerzy mogą eksportować ze strony [cen planu platformy Azure](https://partner.microsoft.com/commerce/sales) . 

- Niekwalifikujące się usługi: kredyt uzyskany przez partnera *_nie_* ma zastosowania do następujących:
    - Rezerwacje planu platformy Azure
    - Produkty innych firm zidentyfikowane jako _ *trzecich** w **kolumnie Tagi** ceny zużycia planu platformy Azure    
    - Produkty z cennika portalu Marketplace
   - [Virtual Machines na platformie Azure](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- Wartość PEC jest obliczana codziennie i można ją wyświetlić w pliku dziennego użycia i w pliku Rekonesans faktury miesięcznej. Partner (Dostawca pośredni lub pośredni odsprzedawca) musi mieć dostęp przez cały dzień (24x7), aby upewnić się, że uzyskują PEC. Wartość PEC jest obliczana codziennie na zarządzanych zasobach platformy Azure. Maksymalny PEC dla danego okresu rozliczeniowego (miesiąc) wynosi 15%. Partnerzy utrzymujący trwały dostęp uprzywilejowany przez miesiąc (zakres dostępu) i dla wszystkich kwalifikujących się zasobów (zakres dostępu) uzyskują pełny PEC 15%. Obniżka zakresów i zakresów spowoduje obniżenie stawki PEC przez miesiąc. Dzienny, oceniany plik użycia jest codziennie wyświetlany na podstawie zasobu platformy Azure, niezależnie od tego, czy jest stosowany PEC. Partnerzy mogą także rejestrować się w alertach, aby wykryć, czy istnieją zmiany w trwałym dostępie uprzywilejowanym.

- PEC jest uzyskiwany do poziomu zasobów platformy Azure. Jeśli partner ma prawidłowy dostęp na poziomie subskrypcji lub grupy zasobów, każdy zasób, który ma role do wyższego poziomu, uzyska PEC.  

- Szczegóły PEC również będą dostępne w [usłudze Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners)

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) przy użyciu analizy kosztów umożliwia partnerom wyświetlanie kosztów, które otrzymały korzyść dla PEC.  

1. W [Azure Portal](https://portal.azure.com)Zaloguj się do dzierżawy partnerskiej i wybierz pozycję **Cost Management + rozliczenia**.

2. Wybierz pozycję **Zarządzanie kosztami**

3. Wybierz **analizę kosztów**

   W widoku Analiza kosztów zostaną wyświetlone koszty związane z kontem rozliczeniowym dla wszystkich usług zakupionych i zużytych według cen uiszczanych przez firmę Microsoft.

4. Wybierz pozycję **PartnerEarnedCreditApplied** na liście rozwijanej na wykresie przestawnym, aby zobaczyć koszty, do których zastosowano Pec. Gdy właściwość **PartnerEarnedCreditApplied** ma wartość true, skojarzony koszt ma korzyść dla partnera. 

Gdy właściwość PartnerEarnedCreditApplied ma wartość false, skojarzony koszt nie spełnia wymagań wymaganych do kredytowania lub zakupionej usługi nie kwalifikuje się do uzyskania kredytu za partnerów.

>[!NOTE] 
>Zazwyczaj użycie usług trwa 8-24 godzin w **Cost Management** , a kredyty dla PEC będą wyświetlane w ciągu 48 godzin od momentu uzyskania dostępu w Azure Cost Management.

5. Możesz również grupować według i filtrować według właściwości **PartnerEarnedCreditApplied** za pomocą polecenia **Grupuj według oraz dodać** funkcje filtru, aby przejść do szczegółów kosztów mających wartość PEC i koszty, które nie mają zastosowania Pec.

## <a name="next-steps"></a>Następne kroki

- [Kredyt wypracowany przez partnera — przegląd](partner-earned-credit.md)

- Szczegółowe przykłady obliczeń środków uzyskanych przez partnera znajdują się na liście cenowej, którą można połączyć za pomocą pulpitu nawigacyjnego Centrum partnerskiego (wymagane logowanie).

- [Przejdź do planu platformy Azure — wprowadzenie](azure-plan-get-started.md)

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)

- [Odwołaj lub Cofaj uprawnienia administratora dla subskrypcji CSP platformy Azure](revoke-reinstate-csp.md)
