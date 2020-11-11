---
title: Efektywne obliczanie ceny jednostkowej
ms.topic: how-to
ms.date: 11/10/2020
description: Dowiedz się więcej na temat efektywnej jednostki cenowej i sposobu jej obliczania. Zawiera przykładowe obliczanie.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/11/2020
ms.locfileid: "94499150"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Efektywne Obliczanie cen jednostkowych dla użycia planu platformy Azure

## <a name="the-effective-unit-price"></a>Obowiązująca cena jednostkowa

Obowiązująca cena jednostkowa jest obliczana na poziomie licznika (w przeciwieństwie do poziomu zasobów) i jest dostosowywana codziennie zgodnie z użyciem licznika.

Obliczamy obowiązującą cenę jednostkową przy użyciu następujących trzech czynników:

- Użycie, które jest monitorowane codziennie w całym cyklu rozliczeniowym
- Koszt do rozliczenia dla miernika
- Obsługa warstw (jeśli dotyczy)

Ze względu na to, że Twoje użycie jest monitorowane codziennie w całym cyklu rozliczeniowym, obowiązująca cena jednostkowa ulegnie zmianie. Końcowa cena danego cyklu rozliczeniowego będzie dostępna po zatrzymaniu obliczeń zużycia i zamknięciu okresu rozliczeniowego. Przed czwartym lub piątym miejscem dziesiętnym zobaczysz większość zmian w zużyciu.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Dowiedz się, czy licznik używa cen warstwowych

Jeśli nie wiesz, czy licznik używa cen warstwowych, Skorzystaj z poniższej procedury, aby dowiedzieć się. 

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).
2. Wybierz pozycję **Sprzedaj** , wybierz pozycję **Cennik i oferty** , a następnie wybierz pozycję **Cennik planu platformy Azure**.
3. Znajdź swój licznik według identyfikatora, a następnie Pobierz dane cennika. 

## <a name="sample-calculation"></a>Przykładowe Obliczanie

W poniższej tabeli przedstawiono przykład sposobu obliczania efektywnej ceny jednostkowej w okresie otwartym.

W tabeli są stosowane następujące wartości: 

- W **górę** = cena jednostkowa zasobu/godziny = 0,868

- **Bcu** = jednostka zużycia do rozliczenia dla miernika

- **BC** = koszt płatny dla licznika = bcu * w górę * 0,85. Odzwierciedla to korektę dla rabatu PEC o 15%. Następnie użyjemy dolnego limitu funkcji, aby ograniczyć wartość do dwóch cyfr po przecinku dziesiętnym, aby obciążać kwotę minimalną. 

- **Efektywna cena jednostkowa** = bcu/BC

>[!NOTE]
>Uwaga: licznik w tym przykładzie nie ma warstw w cenniku.

| Data | BCU (jednostka zużycia do rozliczania) | BC (koszt płatny) | Efektywna cena jednostkowa |
| ------ | ----------- | ----------- | ----------- |  
| 3 — sie | 29 | 21,39 | 0.737586206896552 |
| 10-sie | 210,950039 | 155,63 | 0.737757626107858 |
| 25-sie | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Następne kroki

- [Rozliczenia i podatki](billing.md)
