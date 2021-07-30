---
title: Ograniczone możliwości rozliczania bezpośredniego
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Dowiedz się więcej Dostawca rozwiązań w chmurze (CSP) dotyczących partnerów rozliczanych bezpośrednio i dowiedz się, co zrobić, aby uniknąć ograniczenia możliwości. Sprawdź, czy Twoje możliwości zostały ograniczone.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: edb67f6ae3054bf5214611ab3ac5ef4ed6713aef
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836663"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Ograniczone możliwości rachunku bezpośredniego i wymagania wymagane przez partnerów rozliczanych bezpośrednio w programie CSP

**Odpowiednie role:** Administrator globalny

## <a name="overview"></a>Omówienie

Partnerzy rozliczani bezpośrednio muszą spełniać nowe [wymagania,](direct-partner-new-requirements.md) aby pozostać w programie partnera rozliczanych Dostawca rozwiązań w chmurze (CSP). W przeciwnym razie ich dostęp do funkcji rachunku bezpośredniego zostanie ostatecznie ograniczony i będzie można dłużej wykonywać określone zadania, takie jak dokonywanie nowych zakupów dla klientów.

> [!Note]
> Bezpośredni partnerzy rozliczani, którzy nie spełniają nowych wymagań dotyczących programu partnerskiego rozliczania bezpośredniego w programie CSP, zostaną poinformowani przez firmę Microsoft, gdy ich możliwości dotyczące rachunku bezpośredniego będą ograniczone. Dotyczy to wszystkich bezpośrednich partnerów rozliczanych niezależnie od tego, czy wybrali opcję przejścia od partnera z rozliczeniami bezpośrednimi do odsprzedawców [pośrednich.](transition-direct-to-indirect.md)  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Jak sprawdzić, czy możliwości rachunku bezpośredniego zostały ograniczone

Aby sprawdzić, czy dostęp z dzierżawy partnera z rozliczeniami bezpośrednimi do funkcji bezpośredniego rachunku został ograniczony, wykonaj następujące kroki.

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard) Centrum partnerskiego.

2. Przejdź do **ustawień konta Profil**  >  **prawny.**

3. W **obszarze Informacje o** programie **odszukaj Microsoft Cloud Solution Provider stan .**

4. Jeśli stan programu ma ograniczoną wartość **,** oznacza to, że dostęp dzierżawy partnera z rozliczeniami bezpośrednimi do funkcji rachunku bezpośredniego został ograniczony.

## <a name="affected-direct-bill-capabilities"></a>Możliwości rachunku bezpośredniego, których dotyczy problem

Jeśli możliwości rachunku bezpośredniego zostały ograniczone, nie możesz już robić nowych zakupów dla klientów w Partner Center. To ograniczenie obejmuje:

- Subskrypcje platformy Azure

- Subskrypcje oparte na licencjach

- Dodaj nowe dodatki do istniejących subskrypcji opartych na licencjach.

- Dokonaj zakupów oprogramowania i produktów rezerwacji (na przykład subskrypcji oprogramowania, oprogramowania bezterminowego i wystąpień zarezerwowanych maszyn wirtualnych platformy Azure).

Nie można również użyć oferty usług udostępnionych partnera platformy [Azure](shared-services.md) w ramach programu CSP, aby zakupić nowe subskrypcje platformy Azure na własny użytek.

Nie ma to wpływu na istniejące subskrypcje rachunku bezpośredniego. Pozostają one prawidłowe i są automatycznie dostępne. Użytkownik będzie nadal rozliczany bezpośrednio przez firmę Microsoft, dopóki nie zostanie anulowany. Nadal można zarządzać istniejącymi subskrypcjami w następujący sposób:

- Wstrzymywanie istniejących subskrypcji

- Dostosowywanie liczby licencji istniejących subskrypcji opartych na licencjach

- Dostosuj liczbę licencji istniejących dodatków do subskrypcji. 

    >[!Note]
    >Nie można dodawać nowych dodatków do istniejących subskrypcji, ponieważ są traktowane jako nowy zakup.

- Wdrażanie nowych zasobów platformy Azure i zarządzanie istniejącymi zasobami platformy Azure w ramach istniejących subskrypcji platformy Azure. Obejmuje to zasoby, które są dostępne za pośrednictwem Azure Marketplace i Visual Studio subskrypcji.

Oprócz nowych zakupów nie można uzyskać dostępu do następujących funkcji rachunku bezpośredniego w Partner Center:

- Nie można tworzyć nowych dzierżaw klientów. Opcja **Utwórz klienta** na stronie **Klienci** w Partner Center nie będzie dostępna.

- Nie można wygenerować zaproszenia dla klientów żądających bezpośredniej relacji odsprzedawcy. Opcja **Zażądaj relacji odsprzedawcy** na **stronie** Klienci Partner Center nie będzie dostępna.

    >[!NOTE]
    >W ramach przejścia z bezpośredniego partnera rozsyłania na odsprzedawcę pośredniego, jeśli dzierżawa partnera z rozliczeniami bezpośrednimi została już zarejestrowane jako odsprzedawca pośredni, możesz zamiast tego wygenerować zaproszenie do klienta z żądaniem relacji odsprzedawcy pośredniego.

- Nie można utworzyć nowej dzierżawy piaskownicy. Każda dzierżawa partnera z rozliczeniami bezpośrednimi może utworzyć jedną dzierżawę piaskownicy dla integracji interfejsu API rachunku bezpośredniego. Jeśli nie utworzono jeszcze takiego konta, nie możesz tego zrobić po ograniczeniu możliwości twojego partnera z rozliczeniami bezpośrednimi.  

## <a name="next-steps"></a>Następne kroki

- [Dodatkowe informacje na temat zostania odsprzedawcą pośrednim](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nowe wymagania dotyczące partnerów bezpośrednich w programie CSP](direct-partner-new-requirements.md)
