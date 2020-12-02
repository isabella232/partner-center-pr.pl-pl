---
title: Wspólne miesięczne scenariusze rozliczeń
ms.topic: article
ms.date: 05/13/2020
description: Typowe scenariusze w centrum partnerskim w przypadku korzystania z comiesięcznych rozliczeń — obejmuje dodanie nowych subskrypcji, zmianę liczby licencji oraz wstrzymanie subskrypcji.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 616f706ddb4613f927e0c2830dd794fa3db3944e
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529261"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Przykładowe miesięczne Scenariusze rozliczania dla nowych subskrypcji, zmiany kwot licencji lub zawieszeń

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Agent pomocy technicznej
- Agent sprzedaży

Te przykładowe [typowe scenariusze rozliczania](common-billing-scenarios.md) są stosowane w przypadku używania comiesięcznych rozliczeń w centrum partnerskim.

## <a name="new-monthly-subscription"></a>Nowa subskrypcja miesięczna

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia Użytkownik kupuje nową subskrypcję z jedną licencją na USD/miesiąc i wybiera comiesięczne rozliczanie. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Opłata za cykl   |4,00       |1        |4,00 |

Plik uzgadniania na podstawie licencji z lutego 15, będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Opłata za cykl   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Zmień liczbę licencji

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia Użytkownik kupuje nową subskrypcję z jedną licencją na USD/miesiąc i wybiera comiesięczne rozliczanie. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Opłata za cykl   |4,00       |1        |4,00    |

1 lutego zwiększasz ilość licencji od jednej do dwóch. Plik uzgadniania na podstawie licencji z lutego 15, będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Tempo wystąpienia cyklu   |-4,00       |1        |-4,00   |
|1/13/2018         |1/31/2018    | Tempo wystąpienia cyklu   |2.45       |1        |2.45    |
|2018-01-02         |2/12/2018    | Tempo wystąpienia cyklu   |1,55       |2        |3,10    |
|2/13/2018         |3/12/2018    | Tempo wystąpienia cyklu   |4,00       |2        |8,00    |

Cena miesięczna to 4,00, a okres korzystania z usługi 1/13/2018 – 2/12/2018 wynosi 31 dni. Jest to równe cenie dziennej wynoszącej 0,129 (4/31).

W okresie obowiązywania 1/13/2018 – 1/31/2018 występuje 19 dni.

Cena jednostkowa dawki = 2,451 = 19 x 0,129

W okresie obowiązywania 2/1/2018 – 2/12/2018 znajduje się 12 dni.

Cena jednostkowa dawki = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Wstrzymaj przed 30 dni

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia Użytkownik kupuje nową subskrypcję z jedną licencją na USD/miesiąc i wybiera comiesięczne rozliczanie. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Opłata za cykl   |4,00       |1        |4,00    |

1 lutego wstrzymano subskrypcję. Plik uzgadniania na podstawie licencji z lutego 15, będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Opłata za anulowanie|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Wstrzymaj po 30 dniach

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia Użytkownik kupuje nową subskrypcję z jedną licencją na USD/miesiąc i wybiera comiesięczne rozliczanie. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Opłata za cykl|4,00|1|4,00

Plik uzgadniania na podstawie licencji z lutego 15, będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Opłata za cykl|4,00|1|4,00

1 marca wstrzymano subskrypcję. 15 marca plik uzgadniania oparty na licencji będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Opłata za anulowanie|-1,72|1|-1,72

Cena miesięczna to 4,00, a okres korzystania z usługi 2/13/2018 – 3/12/2018 wynosi 28 dni. Jest to równe cenie dziennej wynoszącej 0,143 (4/28).

Cena jednostkowa = dni w okresie użytkowania x cena dzienna x liczba licencji.

W okresie anulowania 3/1/2018 – 3/12/2018 znajduje się 12 dni.

W związku z tym cena jednostkowa =-1,716 (12 x 0,143 x (-1)).
