---
title: Rozliczenia roczne — typowe scenariusze
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Partner Center rozliczenia roczne — podczas dodawania nowych subskrypcji, dodawania licencji przed datą rozliczeń, zmieniania ilości licencji lub zawieszania/ponownego aktywowania subskrypcji.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2baab834c3d31639f1353a53fb8787da041aec1c1c59776df49bd590fb7452f0
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682372"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Typowe roczne scenariusze rozliczeń w Partner Center

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Agent pomocy technicznej | Agent sprzedaży

Te [przykładowe typowe scenariusze rozliczeń](common-billing-scenarios.md) mają zastosowanie w przypadku korzystania z rozliczeń rocznych w Partner Center.

## <a name="new-annual-subscription"></a>Nowa roczna subskrypcja

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Naliczanie opłat podczas zakupu|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Dodawanie licencji po dacie rocznicy subskrypcji, ale przed datą rozliczeniową

Kupujesz nową subskrypcję w dniu 11.02.2017 r. z jedną licencją za 211,20 USD/rok. Rocznica subskrypcji jest ustawiana jako 11. dnia każdego miesiąca. System rozliczeń firmy Microsoft tworzy następujące wiersze rozliczeń:

- Opłata w wysokości 211,20 USD za okres 2/11/17 – 2/10/18.

12.02.17 kupujesz drugą licencję. Data rozliczenia to 14.02.17. Generowana jest faktura i plik uzgodnień. Plik uzgodnień będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |Cena jednostkowa |Liczba | Kwota |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Naliczanie opłat przy zakupie |211.20 |1 | 211.20 |

W rocznicę subskrypcji, 11.03.17, system rozliczeniowy firmy Microsoft tworzy następujące wiersze rozliczeń dla zwiększenia liczby licencji w dniu 12.02.17:

- 211,20 USD środków na okres 2/11/17 – 2/10/18.
- Opłata proporcjonalna w wysokości 0,58 USD za licencję dla jednej licencji w okresie 2/11/17 – 2/11/17.
- Opłata proporcjonalna w wysokości 15,62 USD za licencję dla dwóch licencji w okresie 2/12/17 – 3/10/2017.
- Opłata proporcjonalna w wysokości 195,00 USD za licencję dla dwóch licencji w okresie od 3.11.2017 r. do 10.02.2018 r.

11.02.17 kupujesz subskrypcję. 12.02.17 dodasz licencję. Data rozliczenia to 14.02.17. 11.02.18 subskrypcja zostanie odnowiona.

Następna data rozliczeniowa to 14.03.17 i zostanie wygenerowana faktura i plik uzgodnień. Plik uzgodnień będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |Cena jednostkowa |Liczba | Kwota |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Cykl prorate wystąpienia |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Cykl prorate wystąpienia |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Cykl prorate wystąpienia |15.62 |2 |31.25 |
|3/11/2017 |2/10/2018 |Cykl prorate wystąpienia |195.00 |2 |390.00 |

11.02.18 subskrypcja zostanie odnowiona na kolejny 12-miesięczny okres.

## <a name="change-license-quantity"></a>Zmień liczbę licencji

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Naliczanie opłat podczas zakupu|48.00|1|48.00

1 lutego zwiększysz liczbę licencji z jednej do dwóch. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cykl wystąpienia prorate|-48.00|1|-48.00
1/13/2018|1/31/2018|Cykl wystąpienia prorate|2.47|1|2.47
2018-01-02|1/12/2019|Cykl wystąpienia prorate|44.98|2|89.96

Cena roczna wynosi 48,00, co odpowiada cenie dziennej 0,13 (48,00/365).

Cena jednostkowa = dni w okresie świadczenia usługi x cena dzienna x liczba licencji.

W okresie obsługi od 13.01.2018 r. do 31.01.2018 r. istnieje 19 dni.

W związku z tym cena jednostkowa = 2,47 (19x0,13x1)

W okresie obsługi od 1.02.2018 r. do 12.01.2019 r. istnieje 346 dni.

W związku z tym cena jednostkowa = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Wstrzymywanie przed 30 dniami

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia zakupisz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierzesz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Naliczanie opłat podczas zakupu|48.00|1|48.00

1 lutego zawieszasz subskrypcję. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Anulowanie opłaty|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Wstrzymywanie po 30 dniach

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia zakupisz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierzesz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Naliczanie opłat podczas zakupu|48.00|1|48.00

Plik uzgodnień oparty na licencjach z 15 lutego nie będzie zawierać żadnych wierszy rozliczeń dla tej subskrypcji.
1 marca zawieszasz subskrypcję. Plik uzgodnień oparty na licencjach z 15 marca będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Anulowanie opłaty|-41.34|1|-41.34

Cena roczna wynosi 48,00, co odpowiada cenie dziennej 0,13 (48,00/365).

Cena jednostkowa = dni w okresie świadczenia usługi x cena dzienna x liczba licencji.

W okresie obsługi od 1.03.2018 r. do 12.01.2019 r. istnieje 318 dni.

W związku z tym cena jednostkowa = 41,34 (318x0,13x1). Ponieważ jest to kredyt, cena jednostkowa wynosi -41,34.

## <a name="suspend-and-reactivate"></a>Wstrzymywanie i ponowne aktywowanie

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Naliczanie opłat podczas zakupu|48.00|1|48.00

1 lutego zawieszasz subskrypcję. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Anulowanie opłaty|-48.00|1|-48.00

1 marca ponownie aktywuj subskrypcję. Plik uzgodnień oparty na licencjach z 15 marca będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Naliczanie opłat podczas zakupu|41.34|1|41.34

Cena roczna wynosi 48,00, co odpowiada cenie dziennej 0,13 (48,00/365).

Cena jednostkowa = dni w okresie świadczenia usługi x cena dzienna x liczba licencji.

W okresie świadczenia usługi 3.1.2018 – 12.01.2019 r. istnieje 318 dni.

W związku z tym cena jednostkowa = 41,34 (318x0,13x1).
