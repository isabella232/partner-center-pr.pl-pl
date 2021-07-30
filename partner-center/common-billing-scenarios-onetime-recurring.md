---
title: Rozliczanie jednorazowych & cyklicznych zakupów
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Partner Center przykłady rozliczeń dla jednorazowych zakupów i wybierz cykliczne zakupy — w przypadku zakupu subskrypcji dodaj więcej subskrypcji, dodaj lub usuń licencje.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44594df78ba99a3762549b916265de9faa667e7b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844109"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Partner Center scenariuszy rozliczania jednorazowych i wybierz cykliczne zakupy

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Agent pomocy technicznej | Agent sprzedaży

Są to [typowe scenariusze rozliczeń.](common-billing-scenarios.md) 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Kupowanie subskrypcji i dodawanie licencji w tym samym dniu

W scenariuszu 1 subskrypcja zostanie zakupiona 11 czerwca po cenie jednostkowej 4 USD. Później tego samego dnia zakupisz kolejną subskrypcję w tej samej cenie.

Plik rekonescji będzie obejmować następujące elementy:

- Rachunek w wysokości 4 USD za okres świadczenia usługi od 10 czerwca do 9 lipca.
- 4,00 USD proporcjonalnie do okresu świadczenia usługi od 11 czerwca do 11 czerwca. Jest to okres, w którym masz licencję na te. Obliczenie = (cena miesięczna/łączna liczba dni w okresie świadczenia usługi) x dni w okresie świadczenia usługi proporcjonalnie x liczba licencji = (4/30) x 30 x 1 = 4,00.
- 8,00 USD proporcjonalnie do okresu świadczenia usługi od 10 czerwca do 9 lipca. Jest to okres, w którym masz dwie licencje. Obliczenie = (4/30) x 30 x 2 = 8,00.

|**Data zakupu**   |**Początek opłaty** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 USD                |1                 |4 USD            |Nowy         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Kupowanie subskrypcji i dodawanie kolejnych subskrypcji później

W scenariuszu 2 zakupisz subskrypcję 11 czerwca po cenie jednostkowej 4 USD, a 12 czerwca zakupisz kolejną subskrypcję tego samego produktu za tę samą cenę.

Plik rekonescji będzie obejmować następujące elementy:

- Rachunek w wysokości 4 USD za okres świadczenia usługi od 10 czerwca do 9 lipca.
- 3,87 USD proporcjonalnie do okresu świadczenia usługi od 11 czerwca do 12 czerwca. Jest to okres, w którym masz jedną licencję. Obliczenie = (cena miesięczna/łączna liczba dni w okresie świadczenia usługi) x dni w okresie świadczenia usługi proporcjonalnie x liczba licencji = (4/30) x 29 x 1 = 3,87.
- 7,74 USD proporcjonalnie do okresu świadczenia usługi od 12 czerwca do 9 lipca. Jest to okres, w którym masz dwie licencje. Obliczenie = (4/30) x 29 x 2 = 7,74.

|**Data zakupu**   |**Początek opłaty** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (masz jedną licencję)     |6/10/2019   |7/09/2019         |4 USD         |1        |4 USD            |Nowy         |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Kupowanie subskrypcji i usuwanie licencji w tym samym dniu

W scenariuszu 3 zakupisz dwie subskrypcje dla tego samego produktu w dniu 11 czerwca po cenie jednostkowej 4 USD. Później tego samego dnia usuniesz jedną z licencji.  

Plik rekonescji będzie obejmować następujące elementy:

- Rachunek 8 USD za dwie licencje na okres świadczenia usługi od 10 czerwca do 9 lipca.
- 8,00 USD proporcjonalnie do okresu świadczenia usługi od 11 czerwca do 11 czerwca. Jest to okres, w którym masz dwie licencje. Obliczenie = (cena miesięczna/łączna liczba dni w okresie świadczenia usługi) x dni w okresie świadczenia usługi proporcjonalnie x liczba licencji = (4/30) x 30 x 2 = 8,00.
- 4,00 USD proporcjonalnie do okresu świadczenia usługi od 11 czerwca do 9 lipca. Jest to okres, w którym masz jedną licencję. Obliczenie = (4/30) x 30 x 1 = 4,00.

|**Data zakupu**   |**Początek opłaty** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 USD                |2                 |8 USD            |Nowy         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        | 1      |4 USD         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Kupowanie subskrypcji i usuwanie licencji później

W scenariuszu 4 zakupisz dwie subskrypcje 11 czerwca w cenie jednostkowej 4 USD, a 12 czerwca usuniesz jedną z licencji.

Plik rekonescji będzie zawierać następujące elementy:

- Rachunek w wysokości 8 USD dla okresu świadczenia usługi od 10 czerwca do 9 lipca.
- 7,74 USD proporcjonalnie za okres świadczenia usługi od 11 czerwca do 12 czerwca. Jest to okres, w którym masz dwie licencje. Obliczenie = (cena miesięczna/łączna liczba dni w okresie świadczenia usługi) x dni w okresie świadczenia usługi proporcjonalnie x liczba licencji = (4/30) x 29 x 2 = 7,74.
- 3,87 USD proporcjonalnie za okres świadczenia usługi od 12 czerwca do 9 lipca. Jest to okres, w którym masz jedną licencję. Obliczenie = (4/30) x 29 x 1 = 3,87.

|**Data zakupu**   |**Początek opłaty** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (masz dwie licencje)     |6/10/2019   |7/09/2019         |4 USD         |2        |8 USD       |Nowy       |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12.06.2019 (masz jedną licencję)    | 6/10/2019    |7/09/2019   |4 USD    |1      |3,87 USD    |removeQuantity |

## <a name="next-steps"></a>Następne kroki

- [Przykładowe miesięczne scenariusze rozliczeń dla nowych subskrypcji, zmienianie kwot licencji lub zawieszanie](common-billing-scenarios-monthly.md)