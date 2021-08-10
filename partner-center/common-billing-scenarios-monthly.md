---
title: Typowe miesięczne scenariusze rozliczeń
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Typowe scenariusze w Partner Center w przypadku korzystania z rozliczeń miesięcznych — obejmuje dodawanie nowych subskrypcji, zmienianie ilości licencji i zawieszanie subskrypcji.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f6486f391925b7b283bec6b14c93c51ede095be033a307031b20bc604a2629e5
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682321"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Przykładowe miesięczne scenariusze rozliczeń dla nowych subskrypcji, zmienianie kwoty licencji lub zawieszanie

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Agent pomocy technicznej | Agent sprzedaży

Te [przykładowe typowe scenariusze rozliczeń](common-billing-scenarios.md) mają zastosowanie w przypadku korzystania z rozliczeń miesięcznych w Partner Center.

## <a name="new-monthly-subscription"></a>Nowa miesięczna subskrypcja

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia zakupisz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierzesz rozliczenia miesięczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Opłata za cykl   |4,00       |1        |4,00 |

Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Opłata za cykl   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Zmień liczbę licencji

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia zakupisz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierzesz rozliczenia miesięczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Opłata za cykl   |4,00       |1        |4,00    |

1 lutego zwiększysz liczbę licencji z jednej do dwóch. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Cykl prorate wystąpienia   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | Cykl prorate wystąpienia   |2.45       |1        |2.45    |
|2018-01-02         |2/12/2018    | Cykl prorate wystąpienia   |1,55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Cykl prorate wystąpienia   |4,00       |2        |8.00    |

Cena miesięczna wynosi 4,00, a w okresie usługi od 13.01.2018 r. do 12.02.2018 r. Odpowiada to cenie dziennej 0,129 (4/31).

W okresie proracji 13.01.2018 – 31.01.2018 istnieje 19 dni.

Cena jednostkowa proration = 2,451 = 19 x 0,129

W okresie proracji 2/1/2018 – 2/12/2018 istnieje 12 dni.

Cena jednostkowa proration = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Wstrzymaj przed 30 dniami

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia zakupisz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierzesz rozliczenia miesięczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Opłata za cykl   |4,00       |1        |4,00    |

1 lutego zawieszasz subskrypcję. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Anulowanie opłaty|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Wstrzymywanie po upływie 30 dni

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia zakupisz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierzesz rozliczenia miesięczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Opłata za cykl|4,00|1|4,00

Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Opłata za cykl|4,00|1|4,00

1 marca wstrzymujesz subskrypcję. Plik uzgodnień oparty na licencjach z 15 marca będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Anulowanie opłaty|-1.72|1|-1.72

Cena miesięczna wynosi 4,00, a w okresie usługi od 13.02.2018 r. do 12.03.2018 r. Odpowiada to cenie dziennej 0,143 (4/28).

Cena jednostkowa = dni w okresie świadczenia usługi x cena dzienna x liczba licencji.

W okresie anulowania 3/1/2018 – 3/12/2018 istnieje 12 dni.

W związku z tym cena jednostkowa = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Następne kroki

- [Scenariusze rozliczeń dla jednorazowych zakupów i wybieranie cyklicznych zakupów](common-billing-scenarios-onetime-recurring.md)