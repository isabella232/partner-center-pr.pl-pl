---
title: Pulpit nawigacyjny omówienie usługi Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zobacz migawkę sposobu, w jaki działasz ze sprzedażą i wdrażaniem, wzrostem klientów i wzrostem przychodów z licencjami, subskrypcjami i zużyciem platformy Azure.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cca136670fa2891eea32e4561b97692ca98a77a9
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565410"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Omówienie raportów pulpitu nawigacyjnego dostępnych w u Partner Center Insights
 
**Odpowiednie role:** Administrator globalny | Agent administracyjny | Przeglądarka raportów | Przeglądarka raportów dla kierownictwa

Pulpit nawigacyjny Przegląd szczegółowych informacji zawiera widok migawki kluczowych wskaźników wydajności (KPI), takich jak klienci, subskrypcje, przychód z użycia platformy Azure i licencje. Poniższe wykresy można zwizualizować w raporcie Przegląd.

- Podsumowanie  
- Geograficzne rozmieszczenie klientów, subskrypcji i licencji  
- Trend wzrostu klientów 
- Trend wzrostu subskrypcji 
- Trend wzrostu przychodów zużytych przez platformę Azure 
- Trend wzrostu liczby licencji 

## <a name="summary"></a>Podsumowanie

Podsumowanie zawiera informacje o klientach, przychód z wykorzystania platformy Azure (ACR), sprzedanych subskrypcjach, aktywnych subskrypcjach i wdrożonych licencjach. 

:::image type="content" source="images/pci/summary.png" alt-text="Licencje podsumowujące.":::

Więcej informacji na temat poszczególnych sekcji w sekcji Podsumowanie można znaleźć poniżej.

### <a name="customers"></a>Klienci

Obszar **Klienci** obejmuje:

- Bieżąca liczba wszystkich klientów z co najmniej jedną aktywną subskrypcją skojarzoną z firmą za pośrednictwem różnych typów przypisania i wszystkich produktów w chmurze.
- Procentowy wzrost liczby klientów w wybranym zakresie dat.
- Na mikro wykresie przedstawia trend liczby klientów z miesiąca na miesiąc w wybranym zakresie dat.

### <a name="azure-consumed-revenue-acr"></a>przychód z wykorzystania platformy Azure (ACR)

Obszar **przychód z wykorzystania platformy Azure (ACR)** w obszarze Podsumowanie obejmuje:

- Łączna wartość ACR (w dolarach amerykańskich) przypisana Do Ciebie w wybranym zakresie dat.
- Procentowy wzrost lub spadek wartości ACR z przypisanymi wartościami (w dolarach amerykańskich) w wybranym zakresie dat.
- Mikro wykres przedstawia miesięczny trend ACR w dolarach amerykańskich przypisany do Ciebie w wybranym zakresie dat 

> [!NOTE]
> Dane ACR są dostępne dla użytkowników, którym przypisano rolę osoby przeglądowej raportu executive.
 
### <a name="subscriptions-sold"></a>Sprzedane subskrypcje

Obszar **Sprzedane subskrypcje** w obszarze Podsumowanie obejmuje:

- Łączna bieżąca liczba subskrypcji produktów w chmurze (aktywnych i nieaktywnych) sprzedanych lub zarządzanych przez Ciebie.  
- Procent wzrostu lub spadku liczby subskrypcji w wybranym zakresie dat.
- Na mikro wykresie podano trend łącznej liczby subskrypcji w wybranym zakresie dat z miesiąca na miesiąc.

### <a name="active-subscriptions"></a>Aktywne subskrypcje

Obszar **Aktywne subskrypcje** w obszarze Podsumowanie obejmuje:

- Bieżąca liczba subskrypcji produktów w chmurze z aktywnym użyciem mierzonym na podstawie telemetrii produktu. To wyklucza wszystkie subskrypcje wersji próbnej platformy Azure.  
- Procentowy wzrost liczby aktywnych subskrypcji w wybranym zakresie dat.
- Na mikro wykresie podano trend aktywnych subskrypcji w wybranym zakresie dat z miesiąca na miesiąc.
 
### <a name="licenses-deployed"></a>Wdrożone licencje

Obszar **Licencje wdrożone w** obszarze Podsumowanie obejmuje:
 
- Liczba wszystkich licencji produktów w chmurze wdrożonych w subskrypcjach klientów w wybranym okresie. 
- Procent wzrostu lub spadku liczby tych licencji w wybranym zakresie dat. 
- Na mikro wykresie przedstawiono trend liczby przypisanych licencji w wybranym zakresie dat z miesiąca na miesiąc.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Geograficzne rozmieszczenie klientów, subskrypcji i licencji

Ten widok jest geograficznym rozkładem łącznej liczby klientów, subskrypcji i licencji według kraju klienta. Wybierz różne karty, aby wyświetlić każdy z tych szczegółowych informacji na mapie. Możesz wyszukać i wybrać kraj w siatce, aby powiększyć lokalizację na mapie. Przywróć oryginalny widok, naciskając przycisk Strona główna na mapie. Kliknięcie każdej karty (na przykład Klienci, Subskrypcje) pokazuje wartość metryki dla każdego kraju i wartość procentową sumy dla danego kraju.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Podsumowanie geograficzne.":::

## <a name="customers-growth-trend"></a>Trend wzrostu klientów

Miesięczny trend łącznej liczby klientów dla wybranego zakresu dat. Oś X reprezentuje miesiące wybranego zakresu dat, a oś Y reprezentuje łączną liczbę klientów dla tego miesiąca. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="trend wzrostu klientów.":::

## <a name="subscriptions-growth-trend"></a>Trend wzrostu subskrypcji

Wskazuje to trend liczby subskrypcji klientów dla wybranego zakresu dat. Oś X reprezentuje miesiące wybranego zakresu dat, a oś Y reprezentuje liczbę subskrypcji wybranego produktu. Przewiń suwak w górnej części wykresu, aby powiększyć wykres do określonego okresu. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Trend wzrostu subskrypcji.":::

## <a name="azure-consumed-revenue-growth-trend"></a>przychód z wykorzystania platformy Azure trendu wzrostu

Miesięczny trend przychodu zużytego przez platformę Azure w dolarach amerykańskich przypisany do Ciebie w wybranym zakresie dat. Oś X reprezentuje miesiące z wybranego zakresu dat, a oś Y reprezentuje łączny przychód zużyty przez platformę Azure w dolarach amerykańskich przypisany do Ciebie w ciągu miesiąca.

> [!NOTE]
> ACR będzie widoczny tylko dla użytkowników, którym przypisano rolę osoby przeglądowej raportu executive. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Zużycie platformy Azure.":::

## <a name="licenses-growth-trend"></a>Trend wzrostu liczby licencji
 
Trend licencji przypisanych przez wszystkich klientów w wybranym zakresie dat. Oś X reprezentuje miesiące wybranego zakresu dat, a oś Y reprezentuje liczbę licencji wybranego produktu. Przewiń suwak w górnej części wykresu, aby powiększyć wykres do określonego okresu.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="Licencje.":::

## <a name="next-steps"></a>Następne kroki

Aby uzyskać więcej raportów, [zobacz Partner Center Insights.](partner-center-insights.md)
