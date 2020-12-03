---
title: Przenieś klientów z bieżących ofert platformy Azure do planu platformy Azure
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób partnerzy CSP mogą korzystać z Centrum partnerskiego, aby przenosić klientów z istniejących ofert dostawcy CSP Azure do usług platformy Azure w ramach planu platformy Azure.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 4e22386dc8bddd9662a0d80020a5c90c464e9d39
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534815"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Przejście klientów do planu platformy Azure z istniejących ofert platformy Azure z dostawcami CSP

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Administrator globalny
- Agent pomocy technicznej
- Agent sprzedaży
- Administrator zarządzania użytkownikami

W tym artykule wyjaśniono, w jaki sposób partnerzy CSP mogą korzystać z Centrum partnerskiego, aby przenosić klientów z istniejących ofert dostawcy CSP Azure do usług platformy Azure w ramach planu platformy Azure. Dostawcy pośrednim i bezpośredni partnerzy rozliczeń mogą przejść do nowego środowiska handlowego dostępnego w programie Microsoft Cloud Service Provider (CSP) dla platformy Azure. (Pośrednicy odsprzedawcy będą musieli współpracować z dostawcami pośrednimi). Klienci będą mieli ulepszony sposób kupowania usług w chmurze, którzy kupują od partnerów, od sprzedawcy firmy Microsoft lub bezpośrednio w sieci Web.

Możliwość przejścia jest dostępna tylko dla klientów, którzy przechodzą do nowego środowiska handlowego platformy Azure i podpisały umowę klienta firmy Microsoft. Nie jest to możliwe w przypadku innych ofert w programie CSP, takich jak Office 365 czy Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Przechodzenie istniejących ofert CSP do planu platformy Azure

Możesz przenieść klienta z istniejących ofert dostawcy CSP Azure do usług platformy Azure w ramach planu platformy Azure w ramach nowego środowiska handlowego w programie CSP w centrum partnerskim. W tym celu partner i klient muszą mieć ustanowioną relację odsprzedawcy w centrum partnerskim, a klient musi mieć podpisaną umowę klienta firmy Microsoft.

### <a name="select-transition-to-azure-plan"></a>Wybieranie przejścia do planu platformy Azure

1. Wybierz pozycję Azure plan dla klienta.

2. Wybierz pozycję **przejście rozliczenia do planu platformy Azure**.

   :::image type="content" source="images/azure/transition1.png" alt-text="Zrzut ekranu przedstawiający informacje o raportowaniu subskrypcji opartych na użyciu z opcją wyboru o nazwie: przeniesienie rozliczania subskrypcji platformy Azure do planu platformy Azure.":::

3. Wybierz przycisk **Kontynuuj**

   :::image type="content" source="images/azure/transition2.png" alt-text="Okno dialogowe zatytułowane przejście do usługi Azure plan z implikacjami dotyczącymi przejścia i dwóch opcji w celu wybrania, kontynuowania lub anulowania.":::

   Klient zostanie przeniesiony do planu platformy Azure.

   **Przepływ pracy przejścia automatyzuje wstępnie wymagane kroki**:

   - Zakup planów platformy Azure
   - Jeden plan na klienta w scenariuszach bezpośredniego dostawcy usług kryptograficznych  
   - Jeden plan na odsprzedawcę  

   Na przykład partner zakupił dwie oferty Microsoft Azure i dołączył do zakupu dwie odrębne POR. W takim przypadku przepływ pracy przejścia spowoduje zakupienie dwóch planów platformy Azure (jeden na odsprzedawcę) i zamapowanie odpowiednich subskrypcji platformy Azure w ramach planów platformy Azure automatycznie.  

   **Mapowanie subskrypcji platformy Azure do planu platformy Azure**

   Po zakupie planu platformy Azure nasz system będzie mapować istniejące subskrypcje platformy Azure do planów platformy Azure. Postęp można wyświetlić w Azure Portal, a także w centrum partnerskim.

4. Wróć do strony **subskrypcji** Centrum partnerskiego klienta, aby zaktualizować limit budżetu przy użyciu lokalnej waluty.

   :::image type="content" source="images/azure/transition3.png" alt-text="Widok części strony subskrypcji Centrum partnerskiego z limitami budżetu ustawiony w walucie lokalnej na okres rozliczeniowy.":::

   >[!NOTE]
   >Budżet ustawiony w centrum partnerskim nie jest przenoszone do Azure Portal. Należy również ustawić budżet i alert w Azure Portal.

   Po przejściu do planu platformy Azure nie można już kupować subskrypcji platformy Azure dla tego klienta. Subskrypcje są tworzone w ramach planu platformy Azure w Azure Portal.

   >[!NOTE]
   > Wszystkie subskrypcje platformy Azure zakupione za pomocą RBAC w ramach planu platformy Azure będą wyceniane i rozliczane w walucie lokalnej. Stawki FX nie będą używane.

### <a name="track-your-transition-details"></a>Śledzenie szczegółów przejścia

Postępuj zgodnie z postępem przejścia w Azure Portal, a także w centrum partnerskim.

:::image type="content" source="images/azure/details1.png" alt-text="Zrzut ekranu przedstawiający tabelę z listą szczegółów przejścia na subskrypcję — obejmuje subskrypcję I D, datę przejścia i stan przejścia.":::

### <a name="billing-impact-to-partners"></a>Wpływ rozliczania na partnerów

Jeśli przejdziesz do klienta z istniejącej oferty dostawcy CSP platformy Azure, będziesz mieć następujące wpływ na rozliczenie:

- Opłaty zostaną naliczone na podstawie istniejącej faktury dostawcy usług kryptograficznych w celu użycia do momentu zakończenia oryginalnej subskrypcji platformy Azure w ramach dostawcy CSP.

- Jeśli masz uprawnienia dostępu administratora do istniejącej subskrypcji CSP, nadal będziesz mieć dostęp w przypadku migrowania subskrypcji.

Aby przejść bezpośrednio do usług platformy Azure i rejestracje na serwerze i w chmurze, przeczytaj artykuł [Uzyskaj własność rozliczeń subskrypcji platformy Azure dla umowy partnerskiej firmy Microsoft](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Dziennik inspekcji

Aby uzgodnić rozliczenia, Wyświetl historię subskrypcji "Microsoft Azure" (0145P) na stronie **subskrypcje** .

Subskrypcja "Microsoft Azure" (0145P) składa się z dwóch części:

1. Subskrypcja handlowa
2. Subskrypcja platformy Azure (uprawnienie)

Po zakończeniu przejścia subskrypcja platformy Azure zostanie przeniesiona w ramach nowego planu platformy Azure, a subskrypcja handlowa jest zawieszona, co oznacza, że żadne dalsze użycie nie zostanie zgłoszone.  

>[!NOTE]
>Gdy subskrypcja usługi Microsoft Azure (0145P) zostanie zakupiona w programie CSP, zarówno subskrypcja handlowa, jak i subskrypcja platformy Azure (uprawnienie) mają tę samą wartość. Ma to zastosowanie tylko w przypadku zmian własności rozliczeń lub transferów, które różnią się wartościami.

### <a name="transition-issues"></a>Problemy z przejściem

Nie przewidujemy żadnych problemów podczas przejścia. Jeśli wystąpi, będziemy aktualizować użytkownika w ramach przepływu pracy przejścia. Korzystanie z platformy Azure nie będzie zakłócane.  

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)

- [Kredyt wypracowany przez partnera — przegląd](partner-earned-credit.md)