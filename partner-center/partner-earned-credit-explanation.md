---
title: Środków uzyskane przez partnerów dla usług zarządzanych
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak są obliczane i opłacane punkty uzyskane przez partnerów firmy Microsoft dla usług zarządzanych oraz jak upewnić się, że kwalifikujesz się.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba422a2feae2affb9c2b60ad345c4d6bb0d525c7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145868"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Jak są obliczane i wypłacane środki zarobione przez partnera

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny | Administrator rozliczeń | Agent sprzedaży

Uzyskane przez partnerów punkty dla usług zarządzanych (PEC) rozpoznaje i nagradza partnerów, którzy są właścicielami 24-godzinnej kontroli operacyjnej IT i zarządzania częściami lub całym środowiskiem platformy Azure swoich klientów. Domyślnie w programie CSP partnerzy mają przyznane niezbędne prawa dostępu do subskrypcji klienta, co umożliwia im wykonywanie 24 x 7 operacji zarządzania i kontrolowania zasobów w ramach subskrypcji. Inne sposoby, w jakie klienci mogą aprowizują dostęp dla partnerów transakcji, opisano w poniższej sekcji. Miesięczna kwota faktury jest wartością netto środków uzyskanego przez partnera. Partnerzy mogą zobaczyć szczegóły PEC w swoim miesięcznym pliku rekonescji. Aby uzyskać dodatkowe sposoby, w jakie klient może aprowizować dostęp dla partnera transakcji, zobacz Zarządzanie subskrypcjami i zasobami [w ramach planu platformy Azure.](azure-plan-manage.md)

Przeczytaj również [temat Przywróć uprawnienia administratora dla Azure CSP subskrypcji](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Kwalifikowalności

W celu otrzymania środków zdobytych przez partnera obowiązują następujące wymagania: 

- Aby otrzymać uzyskane środki na zasoby platformy Azure, musisz mieć aktywną umowę MPN i prawidłową rolę kontroli dostępu opartej na rolach (RBAC).

- Musisz mieć całodobową kontrolę operacyjną i zarządzanie zasobami platformy Azure klienta w programie CSP. Oznacza to, że musisz mieć uprawnienia administratora do subskrypcji platformy Azure klienta, grupy zasobów platformy Azure i zasobu platformy Azure. W przypadku dostawców pośrednich i ich pośrednich odsprzedawców dostawca pośredni będzie kwalifikować się do PEC, jeśli dostawca pośredni lub odsprzedawca pośredni albo obaj mają tę kontrolę operacyjną. Aby dowiedzieć się więcej na ten temat, zobacz [Przywróć uprawnienia](./revoke-reinstate-csp.md)administratora dla Azure CSP subskrypcji.

- Oprócz powyższych wymagań PEC ma zastosowanie tylko do usług wymienionych w cenniku użycia planu platformy Azure, który można wyeksportować ze strony [cennika planu platformy Azure.](https://partner.microsoft.com/commerce/sales)

- PEC **nie ma zastosowania** do następujących usług:
    - Rezerwacje planu platformy Azure
    - Produkty innych firm zidentyfikowane jako produkty innych firm w kolumnie Tagi ceny za zużycie planu platformy Azure
    - Produkty w cenniku witryny Marketplace
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC jest zdobywany do poziomu zasobów platformy Azure. Jeśli masz prawidłowy dostęp na poziomie subskrypcji lub grupy zasobów, każdy zasób, który jest zbiorczy dla wyższej jednostki, będzie zdobywać PEC.

- Szczegółowe informacje na temat PEC są również dostępne na [stronie Usługi Azure Cost Management.](/azure/cost-management-billing/costs/get-started-partners)

### <a name="calculation"></a>Obliczenia

PEC jest obliczany codziennie i może być przeglądany w pliku dziennego użycia i pliku ponownego faktury miesięcznej. Partner (dostawca pośredni lub odsprzedawca pośredni) musi mieć dostęp przez cały dzień (24 godziny na dobę), aby mieć pewność, że zdobywa PEC. PEC jest obliczany codziennie na podstawie zarządzanych zasobów platformy Azure. Partnerzy zachowujący trwały dostęp uprzywilejowany przez miesiąc (zakres dostępu) i dla wszystkich kwalifikujących się zasobów (zakres dostępu) uzyskają pełny dostęp. Zmniejszenie zakresu i zakresu spowoduje obniżenie stawki PEC dla miesiąca. Plik dziennego użycia jest codziennie przedstawiany w ramach zasobu platformy Azure, niezależnie od tego, czy PEC jest stosowany. Partnerzy mogą również rejestrować się w alertach, aby monitorować zmiany w trwałym uprzywilejowanym dostępie.

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) przy użyciu analizy kosztów umożliwia partnerowi wyświetlanie kosztów, które otrzymały korzyść z PEC.  

1. W [Azure Portal](https://portal.azure.com)zaloguj się do dzierżawy partnera i wybierz **pozycję Cost Management + Billing**.

2. Wybierz **pozycję Zarządzanie kosztami**

3. Wybierz **pozycję Analiza kosztów**

   W widoku Analiza kosztów będą wyświetlane koszty dla konta rozliczeniowego dla wszystkich usług zakupionych i zużytych po cenach, które płacisz firmie Microsoft.

4. Wybierz **pozycję PartnerEarnedCreditApplied** na liście rozwijanej wykresu przestawnego, aby wyświetlić koszty, dla których zastosowano PEC. Gdy **właściwość PartnerEarnedCreditApplied** ma wartość True, skojarzony koszt ma korzyść z środków uzyskane przez partnera. 

   Gdy właściwość PartnerEarnedCreditApplied ma wartość False, skojarzony koszt nie spełnił wymaganych uprawnień do środków lub zakupiona usługa nie kwalifikuje się do środków uzyskane przez partnera.

   >[!NOTE] 
   >Zwykle użycie usług w ujmce Cost Management trwa 8–24 **godziny, a** środki PEC pojawią się w ciągu 48 godzin od czasu uzyskania dostępu w Azure Cost Management.

5. Można również grupować według i filtrować według właściwości **PartnerEarnedCreditApplied** przy użyciu funkcji Grupuj według i Dodaj filtr, aby przejść do szczegółów kosztów, które mają PEC i kosztów, które nie mają zastosowania PEC. 

## <a name="next-steps"></a>Następne kroki

- [Środków uzyskane przez partnerów — omówienie](partner-earned-credit.md)

- Szczegółowe przykłady obliczeń środków uzyskane przez partnerów znajdują się na cenniku, do który można uzyskać dostęp za pośrednictwem pulpitu Partner Center (wymagane jest zalogowanie).

- [Przejście do planu platformy Azure — wprowadzenie](azure-plan-get-started.md)

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)

- [Odwoływanie lub przywróć uprawnienia administratora dla Azure CSP subskrypcji](revoke-reinstate-csp.md)
