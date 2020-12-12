---
title: Rozliczanie za jednorazowe zakupy cykliczne &
ms.topic: article
ms.date: 05/05/2020
description: Przykładowe rozliczenia Centrum partnerskiego i wybieranie cyklicznych zakupów — w przypadku zakupu subskrypcji należy dodać więcej subskrypcji, dodać lub usunąć licencje.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a301aa85310142b3327baabbf3c8545b31f489bd
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354393"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Scenariusze rozliczania Centrum partnerskiego dla jednorazowych i wybranych cyklicznych zakupów

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Agent pomocy technicznej
- Agent sprzedaży

Są to [typowe scenariusze rozliczania](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Kup subskrypcję i Dodaj licencję w tym samym dniu

W scenariuszu 1 w przypadku zakupu subskrypcji na 11 czerwca cena jednostkowa wynosząca $4. Później ten sam dzień kupuje inną subskrypcję w tej samej cenie.

Plik Rekonesans będzie zawierać następujące elementy:

- $4 rachunek za okres korzystania z usługi 10 czerwca — Lipiec 9.
- opłaty za usługę $-4,00 proporcjonalnie do liczby dni dla okresu korzystania z usług 11 czerwca — Czerwiec 11. Jest to okres, w którym masz 1 licencję. Obliczanie = (cena miesięczna/suma dni w okresie korzystania z usługi) x dni w okresie usługi proporcjonalnie do liczby licencji = (4/30) x 30 x 1 = 4,00.
- $8,00 opłat naliczanych za okres korzystania z usługi 10 czerwca — Lipiec 9. Jest to okres, w którym wystąpiły 2 licencje. Obliczanie = (4/30) x 30 x 2 = 8,00.

|**Data zakupu**   |**Opłata zaczyna się** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Nowy         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addilooć           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addilooć           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Kup subskrypcję i Dodaj więcej subskrypcji później

W scenariuszu 2, kupisz subskrypcję od 11 czerwca według ceny jednostkowej $4 i 12 czerwca, kupisz kolejną subskrypcję dla tego samego produktu w tej samej cenie.

Plik Rekonesans będzie zawierać następujące elementy:

- $4 rachunek za okres korzystania z usługi 10 czerwca — Lipiec 9.
- opłaty za korzystanie z stawki $-3,87 dla okresu korzystania z usług 11 czerwca – 12 czerwca. Jest to okres, w którym masz 1 licencję. Obliczanie = (cena miesięczna/suma dni w okresie korzystania z usługi) x dni w okresie usługi proporcjonalnie do liczby licencji = (4/30) x 29 x 1 = 3,87.
- $7,74 opłat naliczanych za okres korzystania z usług 12 czerwca – Lipiec 9. Jest to okres, w którym wystąpiły 2 licencje. Obliczanie = (4/30) x 29 x 2 = 7,74.

|**Data zakupu**   |**Opłata zaczyna się** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (masz jedną licencję)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Nowy         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3,87       |addilooć           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7,74       |addilooć           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Kup subskrypcję i Usuń licencję w tym samym dniu

W scenariuszu 3 zakupiono dwie subskrypcje dla tego samego produktu w dniu 11 czerwca z ceną jednostkową wynoszącą $4. Później ten sam dzień usunął jedną z licencji.  

Plik Rekonesans będzie zawierać następujące elementy:

- $8 Bill dla dwóch licencji dla okresu korzystania z usług 10 czerwca — Lipiec 9.
- opłaty za usługę $-8,00 proporcjonalnie do liczby dni dla okresu korzystania z usług 11 czerwca — Czerwiec 11. Jest to okres, w którym wystąpiły 2 licencje. Obliczanie = (cena miesięczna/suma dni w okresie korzystania z usługi) x dni w okresie usługi proporcjonalnie do liczby licencji = (4/30) x 30 x 2 = 8,00.
- $4,00 opłaty za okres korzystania z usługi w wysokości 11 czerwca – Lipiec 9. Jest to okres, w którym masz 1 licencję. Obliczanie = (4/30) x 30 x 1 = 4,00.

|**Data zakupu**   |**Opłata zaczyna się** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Nowy         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Kup subskrypcję i Usuń licencje później

W scenariuszu 4 zakupiono 2 subskrypcje w dniu 11 czerwca w cenie jednostkowej wynoszącej $4, a w dniu 12 czerwca zostanie usunięta jedna z licencji.

Plik Rekonesans będzie zawierać następujące elementy:

- $8 rachunek za okres korzystania z usługi 10 czerwca — Lipiec 9.
- opłaty za korzystanie z stawki $-7,74 dla okresu korzystania z usług 11 czerwca – 12 czerwca. Jest to okres, w którym wystąpiły 2 licencje. Obliczanie = (cena miesięczna/suma dni w okresie korzystania z usługi) x dni w okresie usługi proporcjonalnie do liczby licencji = (4/30) x 29 x 2 = 7,74.
- $3,87 opłat naliczanych za okres korzystania z usług 12 czerwca – Lipiec 9. Jest to okres, w którym masz 1 licencję. Obliczanie = (4/30) x 29 x 1 = 3,87.

|**Data zakupu**   |**Opłata zaczyna się** |**Koniec opłaty**  |**Cena jednostkowa**  |**Liczba**  |**Kwota** |**Typ opłaty** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (masz 2 licencje)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Nowy       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7,74       |removeQuantity           |
|6/12/2019 (masz 1 licencję)    | 6/10/2019    |7/09/2019   |$4    |1      |$3,87    |removeQuantity |

## <a name="next-steps"></a>Następne kroki

- [Przykładowe miesięczne Scenariusze rozliczania dla nowych subskrypcji, zmiany kwot licencji lub zawieszeń](common-billing-scenarios-monthly.md)