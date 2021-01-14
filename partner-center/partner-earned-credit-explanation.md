---
title: Kwota uzyskana przez partnera w przypadku usług zarządzanych
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób środki na korzystanie z usługi zarządzanej przez partnerów firmy Microsoft są obliczane i płatne oraz jak zapewnić, że masz odpowiednie uprawnienia.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f274103feeadfa6fd135f99632f3013c29601972
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182413"
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

## <a name="eligibility"></a>Kryteria

Aby otrzymać środki na korzystanie z partnerów (PEC), mają zastosowanie następujące wymagania: 

- Użytkownik musi mieć aktywną umowę MPN oraz ważną rolę kontroli dostępu opartej na rolach (RBAC), aby uzyskać dostęp do dochodów z zasobów platformy Azure, którymi zarządzasz.

- Musisz mieć 24x7ą kontrolę operacyjną i zarządzanie zasobami platformy Azure klienta w dostawcy usług kryptograficznych. Oznacza to, że użytkownik musi mieć uprawnienia administratora do subskrypcji platformy Azure klienta, grupy zasobów platformy Azure, zasobu platformy Azure. W przypadku dostawców pośrednich i ich pośrednich odsprzedawców Dostawca pośredni będzie uprawniony do PEC, jeśli dostawca pośredni lub pośredni odsprzedawca lub oba mają tę kontrolę operacyjną. Aby dowiedzieć się więcej na ten temat, zobacz [przywracanie uprawnień administratora dla subskrypcji CSP platformy Azure](./revoke-reinstate-csp.md).

- Oprócz powyższych wymagań, PEC ma zastosowanie tylko do usług wymienionych w cenniku zużycia planu platformy Azure, które można eksportować ze strony [cennika planu platformy Azure](https://partner.microsoft.com/commerce/sales) .

- PEC **nie** ma zastosowania do następujących usług:
    - Rezerwacje planu platformy Azure
    - Produkty innych firm identyfikowane jako osoby trzecie w kolumnie znaczniki w cenie zużycia planu platformy Azure
    - Produkty z cennika portalu Marketplace
    - [Virtual Machines na platformie Azure](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC jest uzyskiwany do poziomu zasobów platformy Azure. Jeśli masz prawidłowy dostęp na poziomie subskrypcji lub grupy zasobów, każdy zasób, który jest rzutowany do wyższej jednostki, będzie miał wartość PEC.

- Szczegóły dotyczące komputera PEC są również dostępne na stronie [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) .

### <a name="calculation"></a>Obliczenia

Wartość PEC jest obliczana codziennie i można ją wyświetlić w pliku dziennego użycia i w pliku Rekonesans faktury miesięcznej. Partner (Dostawca pośredni lub pośredni odsprzedawca) musi mieć dostęp przez cały dzień (24x7), aby upewnić się, że uzyskują PEC. Wartość PEC jest obliczana codziennie na zarządzanych zasobach platformy Azure. Maksymalny PEC dla danego okresu rozliczeniowego (miesiąc) wynosi 15%. Partnerzy utrzymujący trwały dostęp uprzywilejowany przez miesiąc (zakres dostępu) i dla wszystkich kwalifikujących się zasobów (zakres dostępu) uzyskują pełny PEC 15%. Obniżka zakresów i zakresów spowoduje obniżenie stawki PEC przez miesiąc. Dzienny, oceniany plik użycia jest codziennie wyświetlany na podstawie zasobu platformy Azure, niezależnie od tego, czy jest on stosowany. Partnerzy mogą także rejestrować się w alertach, aby monitorować zmiany trwałego uprzywilejowanego dostępu.

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