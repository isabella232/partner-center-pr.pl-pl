---
title: Funkcje ograniczonego bezpośredniego rozliczania
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o wymaganiach partnerskich bezpośrednich rachunków dostawcy usług kryptograficznych i co należy zrobić, aby uniknąć ograniczonej funkcjonalności. Dowiedz się, czy Twoje możliwości zostały ograniczone.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ee6f4fdb537752cccbceb68716ed22bb8c5fb3a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795777"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Ograniczone możliwości płatności bezpośrednich i wymagania wymagane przez partnerów bezpośrednich weksli CSP  

## <a name="overview"></a>Omówienie

Bezpośredni partnerzy rozliczający muszą spełniać nowe [wymagania](direct-partner-new-requirements.md) , aby pozostały w programie CSP Direct Bill partner. W przeciwnym razie ich dostęp do możliwości bezpośrednich rozliczeń będzie ostatecznie ograniczony i będzie można wykonywać określone zadania, takie jak tworzenie nowych zakupów dla klientów.

> [!Note]
> Bezpośredni partnerzy rozliczeniowi, którzy nie spełniają nowych wymagań programu CSP Direct Bill partner, będą informowani przez firmę Microsoft, gdy ich bezpośrednie rozliczenie będzie ograniczone. Dotyczy to wszystkich partnerów bezpośrednich rozliczeń, niezależnie od tego, czy wybrano [przejście z bezpośredniego partnera rozliczeniowego do pośrednich odsprzedawcy](transition-direct-to-indirect.md) .  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Jak stwierdzić, czy funkcje bezpośredniego rozliczania są ograniczone

Aby upewnić się, że dostęp z dzierżawcy partnera bezpośredniego płatnika do bezpośrednich możliwości rozliczania został ograniczony, wykonaj następujące kroki.

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).

2. Przejdź do pozycji **Ustawienia partnera**  ->  **Profil partnera** .

3. W obszarze **Informacje o programie** poszukaj **Microsoft Cloud status dostawcy rozwiązań** .

4. Jeśli stan programu ma **ograniczoną** wartość, oznacza to, że bezpośredni dostęp do funkcji bezpośredniej płatności dzierżawcy partnera rozliczeniowego został ograniczony.

## <a name="affected-direct-bill-capabilities"></a>Uwzględnione bezpośrednie rozliczenia

Jeśli funkcje płatności bezpośredniej są ograniczone, nie można już tworzyć nowych zakupów dla klientów w centrum partnerskim. To ograniczenie obejmuje:

- Subskrypcje platformy Azure

- Subskrypcje oparte na licencji

- Dodaj nowe dodatki do istniejących subskrypcji opartych na licencji.

- Utwórz jednorazowe zakupy oprogramowania i rezerwacji (na przykład subskrypcje oprogramowania, bezterminowe oprogramowanie i zarezerwowane wystąpienia maszyn wirtualnych platformy Azure).

Nie można również używać [oferty udostępnionych usług partnerskich platformy Azure](shared-services.md) w ramach programu CSP do kupowania nowych subskrypcji platformy Azure do użytku.

Nie dotyczy istniejących subskrypcji bezpośrednich opłat. Pozostaną one ważne i są odnawiane z autoodnowieniem. Opłaty będą naliczane bezpośrednio przez firmę Microsoft, dopóki nie zostaną anulowane. Nadal możesz zarządzać istniejącymi subskrypcjami w następujący sposób:

- Wstrzymywanie istniejących subskrypcji

- Dostosuj liczbę licencji istniejących subskrypcji opartych na licencji

- Dostosuj liczbę licencji istniejących dodatków do subskrypcji. 
 
    >[!Note] 
    >Nie można dodawać nowych dodatków do istniejących subskrypcji, ponieważ są one traktowane jako nowe zakupy.

- Wdrażaj nowe zasoby platformy Azure i Zarządzaj istniejącymi zasobami platformy Azure w ramach istniejących subskrypcji platformy Azure. Obejmuje to zasoby, które są dostępne w ramach subskrypcji platformy Azure Marketplace i programu Visual Studio.

Oprócz nowych zakupów nie można uzyskać dostępu do następujących możliwości bezpośrednich rachunków w centrum partnerskim:

- Nie można tworzyć nowych dzierżawców klientów. Opcja **Utwórz klienta** na stronie **klienci** w centrum partnerskim będzie niedostępna.

- Nie można wygenerować zaproszenia do klienta wysyłającego żądanie dotyczące relacji bezpośredniego odsprzedawcy. Opcja **Żądaj relacji odsprzedawcy** w obszarze **klienci** w centrum partnerskim będzie niedostępna.

    >[!NOTE]
    >W ramach przechodzenia z bezpośredniego partnera rozliczeniowego do odsprzedawcy pośredniego, jeśli wcześniej zarejestrowano dzierżawcę partnera z płatnością bezpośrednią jako pośredni odsprzedawcy, można wygenerować zaproszenie do klientów żądających pośredniego odsprzedawcy.

- Nie można utworzyć nowej dzierżawy piaskownicy. Każda dzierżawa usługi Direct Bill partner może utworzyć jedną dzierżawę piaskownicy na potrzeby integracji z interfejsem API bezpośredniej rozliczania. Jeśli jeszcze tego nie zrobiono, nie możesz tego robić po przeprowadzeniu bezpośredniej możliwości partnera rozliczeniowego.  

## <a name="next-steps"></a>Następne kroki

- [Dodatkowe informacje na temat pośredniego odsprzedawcy](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nowe wymagania dla partnera CSP Direct](direct-partner-new-requirements.md)