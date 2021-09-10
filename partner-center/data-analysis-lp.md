---
title: Korzystanie z analizy na użytek szczegółowych informacji o subskrypcji
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Dowiedz się, jak używać analiz w Partner Center, aby lepiej zrozumieć swoją firmę i sposób, w jaki klienci korzystają z zakupionych licencji.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e94a57b6e93c86a24458862a3dd4a6ccc0b14885
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959577"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>Używanie analizy, aby dowiedzieć się więcej o przychodach z subskrypcji

**Odpowiednie role:** Administrator globalny | Administrator partnera MPN

Planowanie sposobów opracowania działań w firmie związanych z programem CSP obejmuje zrozumienie, w jaki sposób klienci używają produktów firmy Microsoft. Istnieje kilka opcji zbierania danych w usługach Partner Center. Możesz zbierać dane dotyczące zarówno firmy, jak i tego, czy i w jaki sposób klienci korzystali z zakupionych licencji. Jeśli korzystasz z modelu bezpośredniego programu CSP, masz również możliwość zainstalowania i użycia pakietu aplikacja statystyczna Centrum partnerskiego dla usługi Power BI w celu zebrania dodatkowych danych.

## <a name="access-to-the-subscription-analytics"></a>Dostęp do analizy subskrypcji

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)
1. W programie CSP w menu Partner Center wybierz **pozycję** Analizuj, a następnie wybierz pozycję **Analiza subskrypcji.**

1. Końcowe przychody z 12 miesięcy CSP będą wyświetlane w górnej części strony

:::image type="content" source="images/analytics/subscription1.png" alt-text="Ekran subskrypcji.":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>Końcowe Twelve-Month CSP (TTM) Revenue

12-miesięczny przychód w programie CSP reprezentuje Dostawca rozwiązań w chmurze przychodu z programu w USD na poziomie globalnego konta partnera. Dane są odświeżane ósmego dnia każdego miesiąca, aby wyświetlić końcowe przychody z 12 miesięcy do poprzedniego miesiąca. Na przykład 9 września 2020 r. powinno być możliwe wyświetlanie TTM dla stałego okresu od września 2019 r. do sierpnia 2020 r. Subskrypcje oprogramowania są wykluczone. Przychód z TTM będzie odzwierciedlał tylko kwalifikowalny przychód, dla którego faktury zostały już opłacone. 

Przychód wyświetlany na Partner Center jest obliczany dla stałego przedziału czasu 12 miesięcy i nie można go zmodyfikować w krótszym przedziale czasu.

Aby wyświetlić podział przychodu na poziomie konta lokalizacji partnera:

- Wybierz link "Pobierz szczegóły" i pobierz plik tsv, który wyświetla przychód z urządzenia TTM we wszystkich lokalizacjach.

>[!NOTE] 
>Sumowanie poszczególnych numerów przychodów z TTM dla identyfikatorów MPN w pliku TSV może wydawać się większe niż ogólny przychód z TTM wyświetlany na Partner Center. Wynika to z tego, że przychód może być dwukrotnie zliczony dla subskrypcji z wieloma przypisaniami partnerów w pobranym pliku.

## <a name="subscription-summary"></a>Podsumowanie subskrypcji

W dolnej części ekranu zostanie wyświetlone podsumowanie subskrypcji. Użyj następujących filtrów, aby wyświetlić wymagane szczegóły subskrypcji:  

1. **Czas** trwania: Możesz wybrać opcję zobaczenia podsumowania subskrypcji dla 

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






