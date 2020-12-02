---
title: Coroczne rozliczenia — typowe scenariusze
ms.topic: article
ms.date: 05/05/2020
description: Coroczne rozliczanie w centrum partnerskim — w przypadku dodawania nowych subskrypcji Dodaj licencje przed datą rozliczenia, Zmień liczbę licencji lub Zawieś/Uaktywnij ponownie subskrypcje.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 086a7d359e1b903684af4ecddac37eda584e55f8
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529262"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Wspólne roczne Scenariusze rozliczania w centrum partnerskim

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Agent pomocy technicznej
- Agent sprzedaży

Te przykładowe [typowe scenariusze rozliczania](common-billing-scenarios.md) są stosowane w przypadku korzystania z rozliczeń rocznych w centrum partnerskim.

## <a name="new-annual-subscription"></a>Nowa roczna subskrypcja

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia nabywasz nową subskrypcję z jedną licencją na USD/miesiąc i wybierasz opcję rozliczania rocznego. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Opłata proporcjonalna przy zakupie|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Dodaj licencję po dacie rocznicy subskrypcji, ale przed datą rozliczenia

Kup nową subskrypcję w dniu 2/11/17 przy użyciu jednej licencji dla $211.20/Year. Rocznica subskrypcji jest ustawiana jako 11 każdego miesiąca. System rozliczeń firmy Microsoft tworzy następujące wiersze rozliczeń:

- $211,20 opłata za okres 2/11/17 – 2/10/18.

W dniu 2/12/17 zakupiesz drugą licencję. Data rozliczenia to 2/14/17. Zostanie wygenerowany faktura i plik uzgadniania. Plik uzgadniania będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |Cena jednostkowa |Liczba | Kwota |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Opłata proporcjonalna przy zakupie |211,20 |1 | 211,20 |

W rocznicie subskrypcji 3/11/17 system rozliczeń firmy Microsoft tworzy następujące wiersze rozliczeń w celu zwiększenia licencji na 2/12/17:

- $211,20 środki na okres 2/11/17 – 2/10/18.
- $0,58 Opłata proporcjonalna na licencję na 1 licencję za okres 2/11/17 – 2/11/17.
- $15,62 Opłata proporcjonalna na licencję za 2 licencje za okres 2/12/17 – 3/10/2017.
- $195,00 Opłata proporcjonalna na licencję za 2 licencje za okres 3/11/2017 – 2/10/2018.

Na 2/11/17 zakupiesz subskrypcję. Na 2/12/17 dodawana jest licencja. Data rozliczenia to 2/14/17. W dniu 2/11/18 Twoje odnowienia subskrypcji.

Następnym terminem rozliczeniowym jest 3/14/17, a faktura & pliku uzgadniania jest generowany. Plik uzgadniania będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty  |Data zakończenia opłaty  |Typ opłaty  |Cena jednostkowa |Liczba | Kwota |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Tempo wystąpienia cyklu |-211,20 |1 |-211,20 |
|2/11/2017 |2/11/2017 |Tempo wystąpienia cyklu |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Tempo wystąpienia cyklu |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Tempo wystąpienia cyklu |195,00 |2 |390,00 |

W dniu 2/11/18 odnowienie subskrypcji przez inny 12-miesięczny okres.

## <a name="change-license-quantity"></a>Zmień liczbę licencji

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia nabywasz nową subskrypcję z jedną licencją na USD/miesiąc i wybierasz opcję rozliczania rocznego. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Opłata proporcjonalna przy zakupie|48,00|1|48,00

1 lutego zwiększasz ilość licencji od jednej do dwóch. Plik uzgadniania na podstawie licencji z lutego 15, będzie zawierać następujące wiersze rozliczeń:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tempo wystąpienia cyklu|-48,00|1|-48,00
1/13/2018|1/31/2018|Tempo wystąpienia cyklu|2,47|1|2,47
2018-01-02|1/12/2019|Tempo wystąpienia cyklu|44,98|2|89,96

Cena roczna to 48,00, która jest równa cenie dziennej 0,13 (48.00/365).

Cena jednostkowa = dni w okresie użytkowania x cena dzienna x liczba licencji.

W okresie usługi 1/13/2018 – 1/31/2018 znajduje się 19 dni.

W związku z tym cena jednostkowa = 2,47 (19x 0.13 x1)

W okresie usługi 2/1/2018 – 1/12/2019 istnieje 346 dni.

W związku z tym cena jednostkowa = 44,98 (346x 0.13 X2)

## <a name="suspend-before-30-days"></a>Wstrzymaj przed 30 dni

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia nabywasz nową subskrypcję z jedną licencją na USD/miesiąc i wybierasz opcję rozliczania rocznego. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Opłata proporcjonalna przy zakupie|48,00|1|48,00

1 lutego wstrzymasz subskrypcję. Plik uzgadniania na podstawie licencji z lutego 15, będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Opłata za anulowanie|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Wstrzymaj po 30 dniach

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia nabywasz nową subskrypcję z jedną licencją na USD/miesiąc i wybierasz opcję rozliczania rocznego. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Opłata proporcjonalna przy zakupie|48,00|1|48,00

Plik uzgadniania opartego na licencji z lutego 15 nie będzie zawierał żadnych wierszy rozliczeń dla tej subskrypcji.
1 marca wstrzymasz subskrypcję. 15 marca plik uzgadniania oparty na licencji będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Opłata za anulowanie|-41,34|1|-41,34

Cena roczna to 48,00, która jest równa cenie dziennej 0,13 (48.00/365).

Cena jednostkowa = dni w okresie użytkowania x cena dzienna x liczba licencji.

W okresie usługi 3/1/2018 – 1/12/2019 istnieje 318 dni.

W związku z tym cena jednostkowa = 41,34 (318x 0.13 x1). Ponieważ jest to kredyt, Cena jednostkowa to-41,34.

## <a name="suspend-and-reactivate"></a>Wstrzymywanie i ponowne aktywowanie

Data rozliczenia to 15. w każdym miesiącu. 13 stycznia nabywasz nową subskrypcję z jedną licencją na USD/miesiąc i wybierasz opcję rozliczania rocznego. Plik uzgadniania na podstawie licencji 15 stycznia będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Opłata proporcjonalna przy zakupie|48,00|1|48,00

1 lutego wstrzymasz subskrypcję. Plik uzgadniania na podstawie licencji z lutego 15, będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Opłata za anulowanie|-48,00|1|-48,00

1 marca ponownie aktywowano subskrypcję. 15 marca plik uzgadniania oparty na licencji będzie zawierać następujący wiersz rozliczenia:

|Data rozpoczęcia opłaty |Data zakończenia opłaty |Typ opłaty |Cena jednostkowa |Liczba |Kwota |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Opłata proporcjonalna przy zakupie|41,34|1|41,34

Cena roczna to 48,00, która jest równa cenie dziennej 0,13 (48.00/365).

Cena jednostkowa = dni w okresie użytkowania x cena dzienna x liczba licencji.

W okresie usługi 3/1/2018 – 1/12/2019 istnieje 318 dni.

W związku z tym cena jednostkowa = 41,34 (318x 0.13 x1).
