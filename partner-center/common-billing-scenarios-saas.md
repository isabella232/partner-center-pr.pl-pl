---
title: Rozliczenia — transakcje SaaS oparte na licencjach
ms.topic: article
ms.date: 05/05/2020
description: Poznaj typowe scenariusze rozliczeń w centrum partnerskim dla transakcji opartych na licencji, oprogramowania jako usługi (SaaS).
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d63e8345bf127cb91f1812193b1f0311cd569b3
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530303"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Typowe scenariusze rozliczania dla transakcji SaaS opartych na licencji w centrum partnerskim

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Agent pomocy technicznej
- Agent sprzedaży


Te przykładowe [typowe scenariusze rozliczania](common-billing-scenarios.md) mają zastosowanie do subskrypcji oprogramowania opartego na licencji jako usługi (SaaS) w centrum partnerskim.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konwertuj subskrypcję bezpłatnej wersji próbnej SaaS na subskrypcję płatną

W tym scenariuszu opisano rozliczenia w przypadku odnowienia subskrypcji bezpłatnej wersji próbnej usługi SaaS opartej na licencji. Odnowienie spowoduje przekonwertowanie bezpłatnej wersji próbnej na płatną subskrypcję na koniec okresu bezpłatnej wersji próbnej.

W tym przykładzie zakupiona została bezpłatna wersja próbna subskrypcji SaaS (oprogramowanie jako usługa) oparta na licencji. Ta bezpłatna wersja próbna zostanie automatycznie odnowiona w ramach płatnej subskrypcji po zakończeniu okresu bezpłatnej wersji próbnej.

Pliki Rekonesans będą zawierać następujące opłaty:

| Data zakupu | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Liczba jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Nowy | Bezpłatna wersja próbna |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $2 | 1 | $2 | Renew | Płatna subskrypcja |

## <a name="cancel-a-free-trial-saas-subscription"></a>Anuluj subskrypcję bezpłatnej wersji próbnej SaaS

> [!TIP]
> Subskrypcję bezpłatnej wersji próbnej usługi SaaS można anulować w dowolnym momencie, nawet w okresie bezpłatnej wersji próbnej.

W tym scenariuszu zakupiłeś subskrypcję bezpłatnej wersji próbnej opartej na licencji SaaS 1 lipca, a następnie natychmiast ją anulowano w centrum partnerskim.

Plik Rekonesans będzie zawierać następujące opłaty:

| Data zakupu | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Liczba jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Nowy | Bezpłatna wersja próbna |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Anuluj | Bezpłatna wersja próbna |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Konwertuj niestandardową subskrypcję SaaS na inną jednostkę SKU

W tym scenariuszu opisano sposób konwertowania niestandardowej subskrypcji SaaS z jednej jednostki składowania (SKU) na inną jednostkę SKU dla tego samego produktu w tym samym dniu.

W tym scenariuszu zakupiono jedną jednostkę SKU (Silver) w ramach produktu i przekonwertowano ją na inną dostępną jednostkę SKU (brązowy) w tym produkcie w tym samym dniu.

Plik Rekonesans będzie zawierać następujące opłaty:

| Data zakupu | SKU | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Liczba jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Srebrny | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Nowy | Niestandardowa subskrypcja SaaS miernika |
| 06/10/2019 | Srebrny | 06/10/2019 | 06/10/2019 | 20 USD | 1 | -$20 | Convert | Rozliczanie opłat naliczanych za niestandardową subskrypcję SaaS |
| 06/10/2019 | Bron | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Convert | Niestandardowa subskrypcja SaaS miernika |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Kup i Anuluj subskrypcję SaaS miernika klienta w tym samym dniu

W tym scenariuszu opisano rozliczenia za subskrypcję SaaS dla miernika klienta zakupionej i anulowanej za pomocą Azure Portal w tym samym dniu.

W tym scenariuszu zakupiono niestandardową subskrypcję SaaS na Azure Portal. Następnie subskrypcja została anulowana w tym samym dniu.

| Data zakupu | SKU | Data rozpoczęcia opłaty | Data zakończenia opłaty | Cena jednostkowa | Liczba jednostek | Suma | Typ opłaty | Opis subskrypcji |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bron | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Nowy | Niestandardowa subskrypcja SaaS miernika |
| 06/10/2019 | Bron | 06/10/2019 | 06/10/2019 | 10 USD | 1 | -$10 | CancelImmediate | Niestandardowa subskrypcja SaaS miernika |
