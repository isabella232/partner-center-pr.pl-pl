---
title: Rozliczenia — transakcje SaaS oparte na licencji
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej na temat typowych scenariuszy Partner Center w przypadku transakcji saaS (oprogramowanie jako usługa) opartych na licencjach.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 764d5a3cb0dc6f409e5272d4119424396caff53b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148639"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Typowe scenariusze rozliczeń dla transakcji SaaS opartych na licencjach w Partner Center

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Agent pomocy technicznej | Agent sprzedaży


Te [przykładowe typowe scenariusze rozliczeń](common-billing-scenarios.md) mają zastosowanie do subskrypcji oprogramowania jako usługi (SaaS) opartych na licencjach w Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konwertowanie subskrypcji SaaS bezpłatnej wersji próbnej na płatną subskrypcję

W tym scenariuszu opisano rozliczenia za odnowienie subskrypcji SaaS bezpłatnej wersji próbnej opartej na licencji. Odnowienie konwertuje bezpłatną wersję próbną na płatną subskrypcję na koniec okresu bezpłatnej wersji próbnej.

W tym przykładzie zakupiono bezpłatną wersję próbną licencji subskrypcji SaaS (oprogramowanie jako usługa) w dniu 10 czerwca. Ta bezpłatna wersja próbna jest odnawiana automatycznie jako płatna subskrypcja po zakończeniu okresu bezpłatnej wersji próbnej.

Pliki rekonesfiguru będą obejmować następujące opłaty:

| Data zakupu | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Ilość jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Nowy | Bezpłatna wersja próbna |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 USD | 1 | 2 USD | Renew | Subskrypcja płatna |

## <a name="cancel-a-free-trial-saas-subscription"></a>Anulowanie subskrypcji saaS bezpłatnej wersji próbnej

> [!TIP]
> Subskrypcję bezpłatnej wersji próbnej SaaS opartą na licencji możesz anulować w dowolnym momencie, nawet w okresie bezpłatnej wersji próbnej.

W tym scenariuszu zakupiono subskrypcję bezpłatnej wersji próbnej SaaS opartą na licencji 1 lipca, a następnie anulowano ją natychmiast w Partner Center.

Plik rekonescji będzie zawierać następujące opłaty:

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

W tym scenariuszu zakupiono subskrypcję SaaS miernika niestandardowego na Azure Portal. Następnie anulowano subskrypcję w tym samym dniu.

| Data zakupu | SKU | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Ilość jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Brązu | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Nowy | Subskrypcja SaaS miernika niestandardowego |
| 06/10/2019 | Brązu | 06/10/2019 | 06/10/2019 | 10 USD | 1 | -10 USD | CancelImmediate | Subskrypcja SaaS miernika niestandardowego |
