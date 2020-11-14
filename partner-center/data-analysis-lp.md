---
title: Korzystanie z analizy do wglądu w dane subskrypcji
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak używać analiz w centrum partnerskim, aby lepiej zrozumieć swoją firmę i jak klienci korzystają z kupionych licencji.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19e7cf9442660a24d36b5f7c20fab156fdc0d59a
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626076"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>Skorzystaj z analizy, aby dowiedzieć się więcej na temat przychodu subskrypcji

**Odpowiednie role**

- Administrator globalny
- Administrator partnerski MPN

Planowanie sposobów opracowania działań w firmie związanych z programem CSP obejmuje zrozumienie, w jaki sposób klienci używają produktów firmy Microsoft. Dostępne są różne opcje zbierania danych w centrum partnerskim i można zbierać dane zarówno w firmie, jak i w zależności od tego, jak klienci korzystają z kupionych licencji. Jeśli korzystasz z modelu bezpośredniego dostawcy usług kryptograficznych, możesz także zainstalować aplikację Analiza Centrum partnerskiego w celu Power BI, aby zebrać dodatkowe dane.

## <a name="access-to-the-subscription-analytics"></a>Dostęp do analizy subskrypcji

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.
1. Z poziomu dostawcy CSP w menu Centrum partnerskiego wybierz pozycję **Analizuj** , a następnie wybierz pozycję **Analiza subskrypcji**.

1. Na górze strony pojawi się końcowy przychód z 12 miesięcy (CSP).

:::image type="content" source="images/analytics/subscription1.png" alt-text="Ekran subskrypcji":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>Końcowy przychód Twelve-Month (TTM) dostawcy CSP

Przychód 12-miesięczny dostawca CSP reprezentuje końcowy przychód programu dostawcy rozwiązań w chmurze w USD na poziomie konta globalnego partnera. Dane są odświeżane co miesiąc, aby wyświetlić końcowy przychód z 12 miesięcy do poprzedniego miesiąca. Na przykład na 9 września 2020 powinna być widoczna TTM dla stałego okresu od 2019 września do sierpnia 2020.

Przychód wyświetlany w centrum partnerskim jest obliczany na podstawie stałego interwału wynoszącego 12 miesięcy i nie może być modyfikowany w krótszym okresie.

Aby wyświetlić podział przychodu na poziomie konta lokalizacji partnera:

- Wybierz link "Pobierz szczegóły" i Pobierz plik TSV, który wyświetla przychód TTM we wszystkich lokalizacjach.

>[!NOTE] 
>Sumowanie indywidualnych wartości przychodu TTM z identyfikatorów MPN w pliku. tsv może wydawać się większy niż ogólny przychód TTM widoczny w centrum partnerskim. Wynika to z faktu, że przychód może być podwojony dla subskrypcji z wieloma przydziałami partnera w pobranym pliku.

## <a name="subscription-summary"></a>Podsumowanie subskrypcji

Dolna połowa ekranu zawiera podsumowanie subskrypcji. Użyj następujących filtrów, aby wyświetlić szczegóły niezbędnej subskrypcji:  

1. **Czas trwania** : możesz wybrać podsumowanie subskrypcji dla 

- 30D — ostatnie 30 dni
- 3M — ostatnie 3 miesiące
- 6 min — ostatnie 6 miesięcy
- 12M — ostatnie 12 miesięcy

2. **Typ produktu** :
 
- Office 365
- Microsoft 365
- Dynamics 365
- EMS

Zastosowanie tych filtrów nie wpłynie na metrykę przychodu TTM w górnej części tego raportu.


 
## <a name="next-steps"></a>Następne kroki

- [Analizuj, w jaki sposób klienci korzystają z zakupionych licencji](increasing-adoption-and-satisfaction.md)  
- [Wyświetlanie dzienników aktywności klienta](activity-logs.md)
- [Aplikacja analizy Centrum partnerskiego dla Power BI](power-bi-app-for-direct-partners.md)






