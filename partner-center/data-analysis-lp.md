---
title: Korzystanie z analizy na użytek szczegółowych informacji o subskrypcji
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Dowiedz się, jak używać analizy w Partner Center, aby lepiej zrozumieć swoją firmę i sposób, w jaki klienci korzystają z zakupionych licencji.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e94a57b6e93c86a24458862a3dd4a6ccc0b14885
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842120"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>Korzystanie z analizy, aby dowiedzieć się więcej o przychodach z subskrypcji

**Odpowiednie role:** Administrator globalny | Administrator partnera MPN

Planowanie sposobów opracowania działań w firmie związanych z programem CSP obejmuje zrozumienie, w jaki sposób klienci używają produktów firmy Microsoft. Istnieje kilka opcji zbierania danych w Partner Center i zbierać dane dotyczące zarówno firmy, jak i sposobu używania zakupionych licencji przez klientów. Jeśli korzystasz z modelu bezpośredniego programu CSP, masz również możliwość instalowania i używania tego modelu aplikacja statystyczna Centrum partnerskiego dla usługi Power BI zbierania dodatkowych danych.

## <a name="access-to-the-subscription-analytics"></a>Dostęp do analizy subskrypcji

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)
1. W programie CSP w menu Partner Center wybierz pozycję Analizuj, a następnie wybierz pozycję **Analiza subskrypcji.**

1. Końcowe przychody z 12 miesięcy dla CSP zostaną wyświetlone w górnej części strony

:::image type="content" source="images/analytics/subscription1.png" alt-text="Ekran subskrypcji.":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>Końcowe Twelve-Month CSP (TTM)

Końcowe przychody z 12-miesięcznego programu CSP reprezentują końcowe przychody z programu Dostawca rozwiązań w chmurze w USD na poziomie globalnego konta partnera. Dane są odświeżane ósmego dnia każdego miesiąca, aby wyświetlić końcowe przychody z 12 miesięcy do poprzedniego miesiąca. Na przykład 9 września 2020 r. powinno być możliwe wyświetlanie TTM dla stałego okresu od września 2019 r. do sierpnia 2020 r. Subskrypcje oprogramowania są wykluczone. Przychód z TTM będzie odzwierciedlał tylko kwalifikujący się przychód, dla którego faktury zostały już opłacone. 

Przychód wyświetlany na Partner Center jest obliczany dla stałego przedziału czasu 12 miesięcy i nie można go zmodyfikować w krótszym przedziale czasu.

Aby wyświetlić podział przychodu na poziomie konta lokalizacji partnera:

- Wybierz link "Pobierz szczegóły" i pobierz plik tsv, który wyświetla przychód z TTM we wszystkich Lokalizacjach.

>[!NOTE] 
>Sumowanie poszczególnych numerów przychodów z TTM dla identyfikatorów MPN w pliku TSV może wydawać się większe niż ogólny przychód TTM wyświetlany na Partner Center. Jest to spowodowane tym, że przychód może być dwukrotnie zliczony dla subskrypcji z wieloma przypisaniami partnerów w pobranym pliku.

## <a name="subscription-summary"></a>Podsumowanie subskrypcji

W dolnej części ekranu zostanie wyświetlone podsumowanie subskrypcji. Użyj następujących filtrów, aby wyświetlić wymagane szczegóły subskrypcji:  

1. **Czas** trwania: możesz wybrać wyświetlanie podsumowania subskrypcji dla 

- 30D — ostatnie 30 dni
- 3M — ostatnie 3 miesiące
- 6 M — ostatnie 6 miesięcy
- 12M — ostatnie 12 miesięcy

2. **Typ produktu:**
 
- Office 365
- Microsoft 365
- Dynamics 365
- EMS

Zastosowanie tych filtrów nie wpłynie na metrykę przychodu z TTM w górnej części tego raportu.


 
## <a name="next-steps"></a>Następne kroki

- [Analizowanie sposobu używania zakupionych licencji przez klientów](increasing-adoption-and-satisfaction.md)  
- [Wyświetlanie dzienników aktywności klienta](activity-logs.md)
- [aplikacja statystyczna Centrum partnerskiego dla usługi Power BI](power-bi-app-for-direct-partners.md)






