---
title: Obliczanie obowiązującej ceny jednostkowej
ms.topic: how-to
ms.date: 04/02/2021
description: Dowiedz się więcej na temat efektywnej ceny jednostkowej i sposobu jej obliczania. Ten artykuł zawiera również przykładowe obliczenia.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4148e9be6ab5bd3e5a146c0ed5479d8ad9723204
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837326"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Obliczanie efektywnej ceny jednostkowej dla użycia planu platformy Azure

**Odpowiednie role:** Administrator rozliczeń

## <a name="the-effective-unit-price"></a>Efektywna cena jednostkowa

Efektywna cena jednostkowa jest obliczana na poziomie miernika (w przeciwieństwie do poziomu zasobu) i jest dostosowywana codziennie zgodnie z użyciem miernika.

Efektywną cenę jednostkową obliczamy przy użyciu następujących trzech czynników:

- Zużycie, które jest monitorowane codziennie w całym cyklu rozliczeniowym
- Rozliczany koszt miernika
- Warstwy (jeśli dotyczy)

Ponieważ monitorujemy dzienne zużycie w całym cyklu rozliczeniowym, efektywna cena jednostkowa będzie się zmieniać. Końcowa cena dla danego cyklu rozliczeniowego będzie dostępna po zatrzymaniu obliczenia zużycia i zamknięciu okresu rozliczeniowego. Większość zmian w zużyciu zobaczysz po czwartym lub piątym miejscu dziesiętnym.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Dowiedz się, czy miernik korzysta z cen warstwowych

Jeśli nie wiesz, czy miernik korzysta z cen warstwowych, skorzystaj z poniższej procedury, aby się tego dowiedzieć. 

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).
2. Wybierz **pozycję Sell**(Sprzedawaj), wybierz pozycję Pricing and offers **(Ceny i oferty),** a następnie wybierz **pozycję Azure plan pricing (Cennik planu platformy Azure).**
3. Znajdź miernik według identyfikatora, a następnie pobierz dane cennika. 

## <a name="sample-calculation"></a>Przykładowe obliczenie

W poniższej tabeli przedstawiono przykład sposobu obliczania efektywnej ceny jednostkowej w okresie otwarcia.

W tabeli mają zastosowanie następujące wartości: 

- **UP** = cena jednostkowa zasobu/godzina = 0,868

- **BCU** = rozliczana jednostka zużycia dla miernika

- **BC** = rozliczany koszt miernika = BCU * UP * 0,85. Odzwierciedla to korektę rabatu 15% rabatu PEC. Następnie używamy dolnego limitu funkcji, aby ograniczyć wartość do dwóch cyfr po przecinku dziesiętnym, aby naliczyć minimalną kwotę. 

- **Efektywna cena jednostkowa** = BCU/BC

>[!NOTE]

>Uwaga: Miernik w tym przykładzie nie ma warstw cenowych ani innych rabatów — współczynniki efektywnej ceny jednostkowej mają wartość procentową rabatu i inne korekty.


| Date (Data) | BCU (rozliczana jednostka zużycia) | BC (koszt rozliczany) | Efektywna cena jednostkowa |
| ------ | ----------- | ----------- | ----------- |  
| 3 sierpnia | 29 | 21.39 | 0.737586206896552 |
| 10 sierpnia | 210.950039 | 155.63 | 0.737757626107858 |
| 25 sierpnia | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Następne kroki

- [Rozliczenia i podatki](billing.md)
