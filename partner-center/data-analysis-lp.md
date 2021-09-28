---
title: Korzystanie z analizy na użytek szczegółowych informacji o subskrypcji
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Dowiedz się, jak używać analizy w Partner Center, aby lepiej zrozumieć swoją firmę i sposób, w jaki klienci korzystają z zakupionych licencji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 640fda04742db736234f66ead0ed9a4a9b5af95b
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129090103"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>Używanie analizy, aby dowiedzieć się więcej o przychodach z subskrypcji

**Odpowiednie role:** Administrator globalny | Administrator partnera MPN

Planowanie sposobów opracowania działań w firmie związanych z programem CSP obejmuje zrozumienie, w jaki sposób klienci używają produktów firmy Microsoft. Istnieje kilka opcji zbierania danych w usługach Partner Center, które można zbierać zarówno w firmie, jak i na temat tego, czy i w jaki sposób klienci korzystali z zakupionych licencji. Jeśli korzystasz z modelu bezpośredniego programu CSP, masz również możliwość zainstalowania i użycia pakietu aplikacja statystyczna Centrum partnerskiego dla usługi Power BI w celu zebrania dodatkowych danych.

## <a name="access-to-the-subscription-analytics"></a>Dostęp do analizy subskrypcji

> [!NOTE]
> Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych, zobacz [Getting around Partner Center (Poruszanie się po Partner Center).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Zaloguj się do Partner Center [nawigacyjnego,](https://partner.microsoft.com/dashboard/home)a następnie wybierz **Szczegółowe informacje** nawigacyjny.

2. Wybierz **pozycję Analizuj,** a następnie wybierz **pozycję Analiza subskrypcji.**

3. Końcowe przychody z 12 miesięcy CSP będą wyświetlane w górnej części strony

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)

2. W obszarze CSP (Program **CSP)** Partner Center menu wybierz pozycję **Analyze**(Analizuj), a następnie wybierz **pozycję Subscription analytics (Analiza subskrypcji).**

3. Końcowe przychody z 12 miesięcy CSP będą wyświetlane w górnej części strony

* * *

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>Końcowe Twelve-Month CSP (TTM)

12-miesięczny przychód w programie CSP reprezentuje końcowe przychody Dostawca rozwiązań w chmurze w USD na poziomie globalnego konta partnera. Dane są odświeżane ósmego dnia każdego miesiąca, aby wyświetlić końcowe przychody z 12 miesięcy do poprzedniego miesiąca. Na przykład 9 września 2020 r. powinno być możliwe wyświetlanie TTM dla stałego okresu od września 2019 r. do sierpnia 2020 r. Subskrypcje oprogramowania są wykluczone. Przychód z TTM będzie odzwierciedlał tylko kwalifikowalny przychód, dla którego faktury zostały już opłacone. 

Przychód wyświetlany na Partner Center jest obliczany dla stałego przedziału czasu 12 miesięcy i nie można go zmodyfikować w krótszym przedziale czasu.

Aby wyświetlić podział przychodu na poziomie konta lokalizacji partnera:

- Wybierz link "Pobierz szczegóły" i pobierz plik tsv, który wyświetla przychód z urządzenia TTM we wszystkich lokalizacjach.

> [!NOTE]
> Sumowanie poszczególnych numerów przychodów z TTM dla identyfikatorów MPN w pliku TSV może wydawać się większe niż ogólny przychód z TTM wyświetlany na Partner Center. Wynika to z tego, że przychód może być dwukrotnie zliczony dla subskrypcji z wieloma przypisaniami partnerów w pobranym pliku.

## <a name="subscription-summary"></a>Podsumowanie subskrypcji

W dolnej części ekranu zostanie wyświetlone podsumowanie subskrypcji. Użyj następujących filtrów, aby wyświetlić wymagane szczegóły subskrypcji:  

1. **Czas** trwania — możesz wybrać, aby wyświetlić podsumowanie subskrypcji dla:

- 30D — ostatnie 30 dni
- 3M — ostatnie 3 miesiące
- 6M — ostatnie 6 miesięcy
- 12M — ostatnie 12 miesięcy

2. **Typ produktu:**

- Office 365
- Microsoft 365
- Dynamics 365
- EMS

Zastosowanie tych filtrów nie wpłynie na metrykę przychodów z TTM w górnej części tego raportu.

## <a name="next-steps"></a>Następne kroki

- [Analizowanie sposobu używania zakupionych licencji przez klientów](increasing-adoption-and-satisfaction.md)  
- [Wyświetlanie dzienników aktywności klienta](activity-logs.md)
- [aplikacja statystyczna Centrum partnerskiego dla usługi Power BI](power-bi-app-for-direct-partners.md)
