---
title: Przenoszenie klientów z bieżących ofert platformy Azure do planu platformy Azure
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak partnerzy programu CSP mogą Partner Center do przenoszenia klientów z istniejących ofert CSP platformy Azure do usług platformy Azure w ramach planu platformy Azure.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: eb9d88935bdc339c01ac47153c3d4a23047dc406
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246381"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Przejście klientów do planu platformy Azure z istniejących ofert CSP platformy Azure

**Dotyczy:** Partner Center 

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży | Administrator zarządzania użytkownikami

W tym artykule wyjaśniono, jak partnerzy programu CSP mogą Partner Center do przenoszenia klientów z istniejących ofert CSP platformy Azure do usług platformy Azure w ramach planu platformy Azure. Dostawcy pośredni i bezpośredni partnerzy rozliczani mogą przejść na nowe środowisko handlowe dostępne w programie Microsoft Cloud Service Provider Program (CSP) dla platformy Azure. (Odsprzedawcy pośredni będą musieli współpracować ze swoimi dostawcami pośrednimi). Klienci będą mieć usprawniony sposób kupowania usług w chmurze, zarówno zakupów od partnerów, od sprzedawców firmy Microsoft, jak i bezpośrednio w Internecie.

Możliwość przejścia jest dostępna tylko dla klientów, którzy przejdą do nowego rozwiązania handlowego dla platformy Azure i którzy podpisali umowę Umowa z Klientem Microsoft. Nie są to inne oferty w programie CSP, takie jak Office 365 lub Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Przechodzenie istniejących ofert CSP do planu platformy Azure

Możesz zmienić klienta z istniejących ofert platformy Azure dla programu CSP na usługi platformy Azure w ramach planu platformy Azure w nowym doświadczeniu handlowym w programie CSP z poziomu Partner Center. W tym celu partner i klient muszą mieć ustanowioną relację odsprzedawcy za pośrednictwem Partner Center, a klient musi podpisać umowę Umowa z Klientem Microsoft.

### <a name="select-transition-to-azure-plan"></a>Wybieranie przejścia do planu platformy Azure

1. Wybierz plan platformy Azure dla klienta.

2. Wybierz **pozycję Transition billing to Azure plan (Przejście rozliczeń do planu platformy Azure).**

   :::image type="content" source="images/azure/transition1.png" alt-text="Zrzut ekranu przedstawiający informacje o raporcie subskrypcji opartych na użyciu z opcją o nazwie: Przejście rozliczeń subskrypcji platformy Azure do planu platformy Azure.":::

3. Wybierz przycisk **Kontynuuj**

   :::image type="content" source="images/azure/transition2.png" alt-text="Okno dialogowe o tytule Przejście do planu platformy Azure z implikacjami do przeczytania na temat przejścia i dwiema opcjami do wybrania: Kontynuuj lub Anuluj.":::

   Klient zostanie przenoszony do planu platformy Azure.

   **Przepływ pracy przejścia automatyzuje kroki wymagań wstępnych:**

   - Zakup planów platformy Azure
   - Jeden plan na klienta w scenariuszach bezpośredniego programu CSP  
   - Jeden plan na odsprzedawcę  

   Na przykład partner kupił dwie oferty Microsoft Azure i uwzględniał w zakupie dwie odrębne jednostki por. W takim przypadku przepływ pracy przejścia zakupi dwa plany platformy Azure (po jednym na odsprzedawcę) i automatycznie zamapuje odpowiednie subskrypcje platformy Azure w ramach planów platformy Azure.  

   **Mapowanie subskrypcji platformy Azure na plan platformy Azure**

   Po zakupie planów platformy Azure nasz system zamapuje istniejące subskrypcje platformy Azure na plany platformy Azure. Postęp można wyświetlić w Azure Portal, a także w Centrum partnerskim.

4. Wróć do strony subskrypcji Partner Center **klienta,** aby zaktualizować limit budżetu przy użyciu waluty lokalnej.

   :::image type="content" source="images/azure/transition3.png" alt-text="Częściowy widok Partner Center subskrypcje z limitami budżetu ustawionymi w walucie lokalnej dla okresu rozliczeniowego.":::

   >[!NOTE]
   >Budżet ustawiony w Partner Center nie jest przejmyny do Azure Portal. Należy również ustawić budżet i alert w Azure Portal.

   Po przejście do planu platformy Azure nie można już kupować subskrypcji platformy Azure dla tego klienta. Subskrypcje tworzy się w ramach planu platformy Azure w Azure Portal.

   >[!NOTE]
   > Wszystkie subskrypcje platformy Azure zakupione za pośrednictwem kontroli RBAC w ramach planu platformy Azure będą wycenione i rozliczane w walucie lokalnej. Stawki FX nie będą używane.

### <a name="track-your-transition-details"></a>Śledzenie szczegółów przejścia

Śledź postęp przejścia w Azure Portal, a także w Partner Center.

:::image type="content" source="images/azure/details1.png" alt-text="Zrzut ekranu przedstawiający tabelę z listą szczegółów przejścia na subskrypcję — obejmuje subskrypcję D, datę przejścia i stan przejścia.":::

### <a name="billing-impact-to-partners"></a>Wpływ na rozliczenia dla partnerów

W przypadku przejścia klienta z istniejącej oferty platformy Azure dla programu CSP będziesz mieć następujący wpływ na rozliczenia:

- Opłaty będą naliczane na istniejącej fakturze CSP za całe użycie aż do momentu zakończenia oryginalnej subskrypcji platformy Azure dostawcy usług w chmurze.

- Jeśli masz uprawnienia dostępu administratora do istniejącej subskrypcji programu CSP, będziesz nadal mieć dostęp podczas migrowania tej subskrypcji.

Aby przejść bezpośrednio Enterprise umów cSP i rejestracji serwerów i chmury do usług platformy Azure, przeczytaj Get [billing ownership of Azure subscriptions for Microsoft Partner Agreement](/azure/billing/mpa-request-ownership) (Uzyskiwanie własności rozliczeń subskrypcji platformy Azure dla usług Microsoft Partner Agreement

### <a name="audit-log"></a>Dziennik inspekcji

Aby uzgodnić rozliczenia, wyświetl historię subskrypcji "Microsoft Azure" (0145P) na **stronie** Subskrypcje.

Subskrypcja "Microsoft Azure" (0145P) składa się z dwóch części:

1. Subskrypcja handlowa
2. Subskrypcja platformy Azure (uprawnienie)

Po zakończeniu przejścia subskrypcja platformy Azure zostanie przeniesiona w ramach nowego planu platformy Azure, a subskrypcja handlowa zostanie wstrzymana, aby nie było zgłaszane żadne dalsze użycie.  

>[!NOTE]
>Gdy Microsoft Azure (0145P) jest zakupiona w programie CSP, zarówno subskrypcja handlowa, jak i subskrypcja platformy Azure (uprawnienie) mają tę samą wartość. Tylko w przypadku zmian własności rozliczeń lub transferów wartości różnią się.

### <a name="transition-issues"></a>Problemy z przejściem

Nie przewidujemy żadnych problemów podczas przejść. Jeśli tak się stanie, zaktualizujemy Cię w samym przepływie pracy przejścia. Użycie platformy Azure nie będzie mieć żadnych zakłóceń.  

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)

- [Środków uzyskane przez partnerów — omówienie](partner-earned-credit.md)
