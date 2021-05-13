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
ms.openlocfilehash: e274b0a637c7fd4944a395ba7e38154e36d2a9e3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855203"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Omówienie raportów pulpitu nawigacyjnego dostępnych w u Partner Center Insights
 
**Odpowiednie role:** Administrator globalny | Agent administracyjny | Przeglądarka raportów | Przeglądarka raportów dla kierownictwa

Pulpit nawigacyjny Przegląd szczegółowych informacji zawiera widok migawki kluczowych wskaźników wydajności, takich jak klienci, subskrypcje, przychód z użycia platformy Azure i licencje. Poniższe wykresy można zwizualizować w raporcie Przegląd.

- Podsumowanie  
- Geograficzne rozmieszczenie klientów, subskrypcji i licencji  
- Trend wzrostu klientów 
- Trend wzrostu subskrypcji 
- Trend wzrostu przychodów zużytych przez platformę Azure 
- Trend wzrostu liczby licencji 

## <a name="summary"></a>Podsumowanie

Podsumowanie zawiera informacje o klientach, przychód z wykorzystania platformy Azure (ACR), sprzedanych subskrypcjach, aktywnych subskrypcjach i wdrożonych licencjach. 

:::image type="content" source="images/pci/summary.png" alt-text="Licencje podsumowujące":::

Więcej informacji na temat poszczególnych sekcji w sekcji Podsumowanie można znaleźć poniżej.

### <a name="customers"></a>Klienci

Obszar **Klienci** obejmuje:

- Bieżąca liczba wszystkich klientów z co najmniej jedną aktywną subskrypcją skojarzoną z firmą za pośrednictwem różnych typów przypisania i wszystkich produktów w chmurze.
- Procentowy wzrost liczby klientów w wybranym zakresie dat.
- Na mikro wykresie przedstawia trend liczby klientów z miesiąca na miesiąc w wybranym zakresie dat.

### <a name="azure-consumed-revenue-acr"></a>przychód z wykorzystania platformy Azure (ACR)

Obszar **przychód z wykorzystania platformy Azure (ACR)** w obszarze Podsumowanie obejmuje:

- Łączna przychód z wykorzystania platformy Azure (w USD) przypisana Do Ciebie w wybranym zakresie dat.
- Procentowy wzrost lub spadek wartości ACR z przypisanymi wartościami (w USD) w wybranym zakresie dat.
- Mikro wykres przedstawia miesięczny trend ACR US$ przypisany do Ciebie w wybranym zakresie dat 

> [!NOTE]
> przychód z wykorzystania platformy Azure (ACR) są dostępne dla użytkowników, którym przypisano rolę osoby wyświetlającego raporty kadry kierowniczej 
 
### <a name="subscriptions-sold"></a>Sprzedane subskrypcje

Obszar **Sprzedane subskrypcje** w obszarze Podsumowanie obejmuje:

- Łączna bieżąca liczba subskrypcji produktów w chmurze (aktywnych i nieaktywnych) sprzedanych lub zarządzanych przez Ciebie.  
- Procent wzrostu lub spadku liczby subskrypcji w wybranym zakresie dat.
- Mikro wykres przedstawia trend łącznej liczby subskrypcji w wybranym zakresie dat z miesiąca na miesiąc.

### <a name="active-subscriptions"></a>Aktywne subskrypcje

Obszar **Aktywne subskrypcje** w obszarze Podsumowanie obejmuje:

- Bieżąca liczba subskrypcji produktów w chmurze z aktywnym użyciem mierzona na podstawie telemetrii produktu. Wyklucza to wszystkie subskrypcje wersji próbnej w przypadku subskrypcji platformy Azure.  
- Procent wzrostu aktywnych subskrypcji w wybranym zakresie dat.
- Mikro wykres przedstawia trend aktywnych subskrypcji w ciągu miesiąca w wybranym zakresie dat.
 
### <a name="licenses-deployed"></a>Wdrożone licencje

Obszar **Licencje wdrożone w** podsumowaniu zawiera:
 
- Liczba wszystkich licencji produktu w chmurze wdrożonych w subskrypcjach klientów w wybranym okresie. 
- Procent wzrostu lub spadku liczby tych licencji w wybranym zakresie dat. 
- Mikro wykres przedstawia trend miesiąc do miesiąca liczby przypisanych licencji w wybranym zakresie dat.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Geograficzne rozmieszczenie klientów, subskrypcji i licencji

Ten widok jest geograficznym rozkładem łącznej liczby klientów, subskrypcji i licencji według kraju klienta. Wybierz różne karty, aby wyświetlić każdy z tych szczegółowych informacji na mapie. Możesz wyszukać i wybrać kraj w siatce, aby powiększyć lokalizację na mapie. Przywróć oryginalny widok, naciskając przycisk Strona główna na mapie. Kliknięcie każdej karty (na przykład Klienci, Subskrypcje) pokazuje wartość metryki dla każdego kraju i wartość procentową sumy dla danego kraju.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Podsumowanie geograficzne":::

## <a name="customers-growth-trend"></a>Trend wzrostu klientów

Miesięczny trend łącznej liczby klientów dla wybranego zakresu dat. Oś X reprezentuje miesiące wybranego zakresu dat, a oś Y reprezentuje łączną liczbę klientów dla tego miesiąca. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="trend wzrostu klientów":::

## <a name="subscriptions-growth-trend"></a>Trend wzrostu subskrypcji

Wskazuje to trend liczby subskrypcji klientów dla wybranego zakresu dat. Oś X reprezentuje miesiące wybranego zakresu dat, a oś Y reprezentuje liczbę subskrypcji wybranego produktu. Przewiń suwak w górnej części wykresu, aby powiększyć wykres do określonego okresu. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Trend wzrostu subskrypcji":::

## <a name="azure-consumed-revenue-growth-trend"></a>przychód z wykorzystania platformy Azure trendu wzrostu

Miesięczny trend przychodu na platformie Azure w USD przypisany do Ciebie w wybranym zakresie dat. Oś X reprezentuje miesiące wybranego zakresu dat, a oś Y reprezentuje łączny przychód z platformy Azure zużyty przez platformę Azure w USD przypisany Do Ciebie w ciągu miesiąca.

> [!NOTE]
> przychód z wykorzystania platformy Azure (ACR) będą widoczne tylko dla użytkowników, którym przypisano rolę osoby przeglądowej raportu wykonawczego. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Zużycie na platformie Azure":::

## <a name="licenses-growth-trend"></a>Trend wzrostu liczby licencji
 
Trend licencji przypisanych przez wszystkich klientów w wybranym zakresie dat. Oś X reprezentuje miesiące wybranego zakresu dat, a oś Y reprezentuje liczbę licencji wybranego produktu. Przewiń suwak w górnej części wykresu, aby powiększyć wykres do określonego okresu.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="licencje":::

## <a name="next-steps"></a>Następne kroki

Aby uzyskać więcej raportów, [zobacz Partner Center Insights.](partner-center-insights.md)
