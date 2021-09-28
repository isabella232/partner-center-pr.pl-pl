---
title: Rozliczenia roczne — typowe scenariusze
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Partner Center rozliczenia roczne — podczas dodawania nowych subskrypcji dodaj licencje przed datą rozliczeń, zmień liczbę licencji lub wstrzymaj/ponownie aktywuj subskrypcje.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f97c36c821955570965fcebb006610f4c5c0c79
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089491"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Typowe roczne scenariusze rozliczeń w Partner Center

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Agent pomocy technicznej | Agent sprzedaży

Te [przykładowe typowe scenariusze rozliczeń](common-billing-scenarios.md) mają zastosowanie w przypadku korzystania z rozliczeń rocznych w Partner Center.

## <a name="new-annual-subscription"></a>Nowa roczna subskrypcja

Data rozliczenia to 15. dnia każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją za 4 USD miesięcznie i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Naliczanie opłat podczas zakupu|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Dodawanie licencji po dacie rocznicy subskrypcji, ale przed datą rozliczeniową

Nową subskrypcję kupujesz 11 lutego 2017 r. z jedną licencją za 211,20 USD rocznie. Rocznica subskrypcji jest ustawiana jako 11. dnia każdego miesiąca. System rozliczeń firmy Microsoft tworzy następujące wiersze rozliczeń:

- Opłata w wysokości 211,20 USD za okres od 11 lutego 2017 r. do 10 lutego 2018 r.

12 lutego 2017 r. kupujesz drugą licencję. Data rozliczenia to 14 lutego 2017 r. Generowana jest faktura i plik uzgodnień. Plik uzgodnień będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |Cena jednostkowa |Liczba | Kwota |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 lutego 2017 r. |10 lutego 2018 r. |Naliczanie opłat przy zakupie |211.20 |1 | 211.20 |

W rocznicę subskrypcji, 11 marca 2017 r., system rozliczeniowy firmy Microsoft tworzy następujące wiersze rozliczeń dla zwiększenia liczby licencji w dniu 12 lutego 2017 r.:

- 211,20 USD środków na okres od 11 lutego 2017 r. do 10 lutego 2018 r.
- Opłata proporcjonalna w wysokości 0,58 USD za licencję dla jednej licencji w okresie od 11 lutego 2017 r. do 11 lutego 2017 r.
- Opłata proporcjonalna w wysokości 15,62 USD za licencję dla dwóch licencji w okresie od 12 lutego 2017 r. do 10 marca.
- Opłata proporcjonalna w wysokości 195,00 USD za licencję dla dwóch licencji w okresie od 11 marca 2017 r. do 10 lutego 2018 r.

11 lutego 2017 r. kupujesz subskrypcję. 12 lutego 2017 r. dodasz licencję. Data rozliczenia to 14 lutego 2017 r. 11 lutego 2018 r. subskrypcja zostanie odnowiona.

Następna data rozliczeniowa to 14 marca 2017 r. Zostanie wygenerowana faktura i plik uzgodnień. Plik uzgodnień będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |Cena jednostkowa |Liczba | Kwota |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 lutego 2017 r. |10 lutego 2018 r. |Cykl prorate wystąpienia |-211.20 |1 |-211.20 |
|11 lutego 2017 r. |11 lutego 2017 r. |Cykl prorate wystąpienia |0.58 |1 |0.58 |
|12 lutego 2017 r. |10 marca 2017 r. |Cykl prorate wystąpienia |15.62 |2 |31.25 |
|11 marca 2017 r. |10 lutego 2018 r. |Cykl prorate wystąpienia |195.00 |2 |390.00 |

11 lutego 2018 r. subskrypcja zostanie odnowiona na kolejny 12-miesięczny okres.

## <a name="change-license-quantity"></a>Zmień liczbę licencji

Data rozliczenia to 15. dnia każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją za 4 USD miesięcznie i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Naliczanie opłat przy zakupie|48.00|1|48.00

1 lutego zwiększysz liczbę licencji z jednej do dwóch. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Cykl wystąpienia prorate|-48.00|1|-48.00
13 stycznia 2018 r.|31 stycznia 2018 r.|Cykl wystąpienia prorate|2.47|1|2.47
1 lutego 2018 r.|12 stycznia 2019 r.|Cykl wystąpienia prorate|44.98|2|89.96

Cena roczna wynosi 48,00 USD, co odpowiada dziennej cenie 0,13 USD (48,00 USD / 365 USD).

Cena jednostkowa = dni w okresie usługi x cena dzienna x liczba licencji.

W okresie obsługi od 13 stycznia 2018 r. do 31 stycznia 2018 r. istnieje 19 dni.

Zatem cena jednostkowa wynosi 2,47 USD (19 x 0,13 x 1)

W okresie świadczenia usługi od 1 lutego 2018 r. do 12 stycznia 2019 r. istnieje 346 dni.

Zatem cena jednostkowa wynosi 44,98 USD (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>Wstrzymywanie przed 30 dniami

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją za 4 USD miesięcznie i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Naliczanie opłat podczas zakupu|48.00|1|48.00

1 lutego zawieszasz subskrypcję. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Anulowanie opłaty|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Wstrzymywanie po 30 dniach

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją na 4 USD/miesiąc i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Naliczanie opłat przy zakupie|48.00|1|48.00

Plik uzgodnień oparty na licencjach z 15 lutego nie będzie zawierać żadnych wierszy rozliczeń dla tej subskrypcji.
1 marca zawieszasz subskrypcję. Plik uzgodnień oparty na licencjach z 15 marca będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 marca 2018 r.|12 stycznia 2019 r.|Anulowanie opłaty|-41.34|1|-41.34

Cena roczna wynosi 48,00 USD, co odpowiada cenie dziennej 0,13 (48,00 /365).

Cena jednostkowa = dni w okresie świadczenia usługi x cena dzienna x liczba licencji.

W okresie świadczenia usługi od 1 marca 2018 r. do 12 stycznia 2019 r. istnieje 318 dni.

Zatem cena jednostkowa wynosi 41,34 USD (318 x 0,13 x 1). Ponieważ jest to kredyt, cena jednostkowa wynosi -41,34 USD.

## <a name="suspend-and-reactivate"></a>Wstrzymywanie i ponowne aktywowanie

Data rozliczenia to 15. dzień każdego miesiąca. 13 stycznia kupujesz nową subskrypcję z jedną licencją za 4 USD miesięcznie i wybierasz rozliczenia roczne. Plik uzgodnień oparty na licencjach z 15 stycznia będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Naliczanie opłat podczas zakupu|48.00|1|48.00

1 lutego zawieszasz subskrypcję. Plik uzgodnień oparty na licencjach z 15 lutego będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 stycznia 2018 r.|12 stycznia 2019 r.|Anulowanie opłaty|-48.00|1|-48.00

1 marca ponownie aktywuj subskrypcję. Plik uzgodnień oparty na licencjach z 15 marca będzie zawierać następujący wiersz rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 marca 2018 r.|12 stycznia 2019 r.|Naliczanie opłat podczas zakupu|41.34|1|41.34

Cena roczna wynosi 48,00, co odpowiada cenie dziennej 0,13 (48,00/365).

Cena jednostkowa = dni w okresie świadczenia usługi x cena dzienna x liczba licencji.

Okres obsługi wynosi 318 dni od 1 marca 2018 r. do 12 stycznia 2019 r.

Zatem cena jednostkowa wynosi 41,34 USD (318 x 0,13 x 1).

## <a name="multiyear-offers-with-annual-billing"></a>Oferty z wieloma latami z rozliczeniami rocznymi

W przypadku ofert wielorocznych z rozliczeniami rocznymi opłaty zaczynają się od daty zakupu i są kontynuowane przez jeden rok.

(W [](#example-of-multiyear-billing) poniższym przykładzie rozliczeń wielorocznych opłaty za pierwszy rok zaczynają się 20 marca 2020 r. i kończą się rok później, 19 marca 2021 r.).

Opłaty za drugi rok zaczynają się o miesiąc wcześniej niż data zakończenia opłaty za pierwszy rok.

(W tym przykładzie opłaty za drugi rok zaczynają się 20 lutego 2021 r., czyli jeden miesiąc przed datą zakończenia pierwszego roku na dzień 19 marca 2021 r.).

Ten roczny proces rozliczeń ma różnicę o jeden miesiąc między datą zakończenia subskrypcji a datą zakończenia naliczania opłat za trzeci rok. Jednak subskrypcja pozostaje aktywna do daty zakończenia subskrypcji.

(W tym przykładzie data zakończenia subskrypcji to 19 marca 2023 r. w trzecim roku to miesiąc po dacie zakończenia opłaty 19 lutego 2023 r.).

### <a name="example-of-multiyear-billing"></a>Przykład rozliczeń wieloetapowych

W przypadku 36-miesięcznej oferty zakupionej 20 marca 2020 r. przedstawionej w poniższych tabelach plik uzgodnień będzie:

#### <a name="first-year"></a>Pierwszy rok

|Data rozpoczęcia subskrypcji  |Data zakończenia subskrypcji  |Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |
|:-:|:-:|:-:|:-:|:-:|
|20 marca 2020 r.|19 marca 2023 r.|20 marca 2020 r.|19 marca 2021 r.|Naliczanie opłat po zakupie|

#### <a name="second-year"></a>Drugi rok

|Data rozpoczęcia subskrypcji  |Data zakończenia subskrypcji  |Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |
|:-:|:-:|:-:|:-:|:-:|
|20 marca 2020 r.|19 marca 2023 r.|20 lutego 2021 r.|19 lutego 2022 r.|Opłata za cykl|

#### <a name="third-year"></a>Trzeci rok

|Data rozpoczęcia subskrypcji  |Data zakończenia subskrypcji  |Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |
|:-:|:-:|:-:|:-:|:-:|
|20 marca 2020 r.|19 marca 2023 r.|20 lutego 2022 r.|19 lutego 2023 r.|Opłata za cykl|
