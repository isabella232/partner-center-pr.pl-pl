---
title: Rozliczenia — transakcje SaaS oparte na licencjach
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Dowiedz się więcej na temat typowych scenariuszy Partner Center w przypadku transakcji saaS (oprogramowanie jako usługa) opartych na licencjach.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9568a014de926682dd89dd9d06d1c6ca5b98ac71
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247041"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Typowe scenariusze rozliczeń dla opartych na licencjach transakcji SaaS w Partner Center

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Agent pomocy technicznej | Agent sprzedaży


Te [przykładowe typowe scenariusze rozliczeń](common-billing-scenarios.md) mają zastosowanie do subskrypcji oprogramowania jako usługi (SaaS) opartych na licencjach w Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konwertowanie bezpłatnej wersji próbnej subskrypcji SaaS na płatną subskrypcję

W tym scenariuszu opisano rozliczenia za odnowienie subskrypcji SaaS bezpłatnej wersji próbnej opartej na licencjach. Odnowienie konwertuje bezpłatną wersję próbną na płatną subskrypcję na koniec okresu bezpłatnej wersji próbnej.

W tym przykładzie zakupiono bezpłatną wersję próbną subskrypcji SaaS (oprogramowanie jako usługa) na podstawie licencji 10 czerwca. Ta bezpłatna wersja próbna jest automatycznie odnawiana jako płatna subskrypcja po zakończeniu okresu bezpłatnej wersji próbnej.

Pliki rekonesji będą obejmować następujące opłaty:

| Data zakupu | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Ilość jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Nowy | Bezpłatna wersja próbna |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 USD | 1 | 2 USD | Renew | Subskrypcja płatna |

## <a name="cancel-a-free-trial-saas-subscription"></a>Anulowanie subskrypcji SaaS bezpłatnej wersji próbnej

> [!TIP]
> Subskrypcję bezpłatnej wersji próbnej SaaS opartą na licencjach można anulować w dowolnym momencie, nawet w okresie bezpłatnej wersji próbnej.

W tym scenariuszu zakupiono subskrypcję bezpłatnej wersji próbnej SaaS opartą na licencjach 1 lipca, a następnie anulowano ją natychmiast w Partner Center.

Plik rekonescji będzie obejmować następujące opłaty:

| Data zakupu | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Ilość jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Nowy | Bezpłatna wersja próbna |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Anuluj | Bezpłatna wersja próbna |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Konwertowanie subskrypcji SaaS miernika niestandardowego na inną subskrypcję SKU

W tym scenariuszu opisano sposób konwertowania subskrypcji SaaS miernika niestandardowego z jednej jednostki magazynowej (SKU) na inną jednostkę SKU dla tego samego produktu w tym samym dniu.

W tym scenariuszu zakupiono jedną sku (Silver) w ramach produktu i przekonwertowano ją na inną dostępną sku (brązową) w ramach tego produktu w tym samym dniu.

Plik rekonescji będzie obejmować następujące opłaty:

| Data zakupu | SKU | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Ilość jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Srebrny | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Nowy | Subskrypcja SaaS miernika niestandardowego |
| 06/10/2019 | Srebrny | 06/10/2019 | 06/10/2019 | 20 USD | 1 | -$20 | Convert | Proporcjonalna subskrypcja SaaS miernika niestandardowego |
| 06/10/2019 | Brązu | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Convert | Subskrypcja SaaS miernika niestandardowego |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Kupowanie i anulowanie subskrypcji SaaS miernika klienta w tym samym dniu

W tym scenariuszu opisano rozliczenia dla subskrypcji SaaS miernika klienta, która została zakupiona i anulowana w Azure Portal tego samego dnia.

W tym scenariuszu zakupiono subskrypcję SaaS miernika niestandardowego w Azure Portal. Następnie anulowano subskrypcję w tym samym dniu.

| Data zakupu | SKU | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Ilość jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Brązu | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Nowy | Subskrypcja SaaS miernika niestandardowego |
| 06/10/2019 | Brązu | 06/10/2019 | 06/10/2019 | 10 USD | 1 | -10 USD | CancelImmediate | Subskrypcja SaaS miernika niestandardowego |
