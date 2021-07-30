---
title: Oferuj klientom wersje próbne produktów firmy Microsoft
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Pozwól klientom wypróbować produkty subskrypcji firmy Microsoft przez 30 dni. Zarejestruj się, aby korzystać z tych bezpłatnych wersji próbnych w katalogu, podobnie jak wiele innych Usługi online.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 393bd70096ba3cd7d1c9889d5b521cc94a389d90
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845979"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Zapewnij klientom 30-dniowe bezpłatne wersje próbne produktów firmy Microsoft

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent sprzedaży

Dobrym sposobem na wprowadzenie klientów do nowych produktów firmy Microsoft jest oferta 30-dniowych bezpłatnych wersji próbnych. Możesz zarejestrować się, aby korzystać z wersji próbnych w katalogu, podobnie jak wiele innych Usługi online. Wszyscy partnerzy mogą uczestniczyć w programie.

## <a name="available-trial-offers"></a>Dostępne oferty wersji próbnej

Wszystkie zaległe oferty wersji próbnej można znaleźć na **stronie** klienta. Ta strona zawiera listę wszystkich subskrypcji, w tym bezpłatnych wersji próbnych i subskrypcji płatnych. (Ta funkcja nie jest obecnie dostępna w Chinach).

Każdy klient jest uprawniony do jednej bezpłatnej wersji próbnej dla każdej dostępnej oferty. Na przykład mogą uzyskać jedną bezpłatną wersję próbną Microsoft 365 Business Standard jedną bezpłatną wersję próbną na Office 365 E3. Jeśli jednak klient jest już właścicielem oferty, nie może skorzystać z bezpłatnej wersji próbnej dla tej oferty.

### <a name="available-products"></a>Dostępne produkty

Bezpłatne wersje próbne są dostępne w przypadku najbardziej kompleksowych i popularnych ofert opartych na licesenach. Nowe oferty wersji próbnej mogą być wprowadzane co miesiąc.

Partnerzy mogą znaleźć wersje próbne w cenniku miesięcznym na **stronie cen i ofert** w Partner Center. Oferty wersji próbnej będą mieć "WERSJĘ PRÓBNĄ" wymienioną w kolumnie typ licencji pomocniczej **cennika.**

Obecnie nie ma **bezpłatnych wersji próbnych** ofert dla instytucji rządowych, ofert edukacyjnych ani ofert dodatków.

## <a name="licenses-for-free-trial-offers"></a>Licencje na oferty bezpłatnej wersji próbnej

Wszystkie bezpłatne wersje próbne zapewniają 25 licencji. Nie można zmienić tego numeru podczas okresu próbnego. W bezpłatnej wersji próbnej nie można dodawać ani usuwać licencji. Po przekonwertowaniu wersji próbnej na płatną subskrypcję możesz dodać więcej licencji do subskrypcji.

Licencje próbne powinny być przypisywane do użytkowników w taki sam sposób, w jaki są przypisywane licencje usług płatnych.

## <a name="sign-customers-up-for-trials"></a>Rejestracja klientów na potrzeby wersji próbnych

Uzyskaj wersję próbną dla klienta w Partner Center:

1. Z **katalogu Sell** on the Partner Center (Sprzedaż w katalogu) przejdź do **katalogu**. 
2. W katalogu w opcji Częstotliwość **rozliczeń** wybierz pozycję **Oferta wersji próbnej.** Umożliwia to wyświetlanie tylko bezpłatnych wersji próbnych i wyłączanie innych ofert, które nie są bezpłatne. Wersje próbne będą wyświetlane na karcie **Wersje** próbne w katalogu.
3. Wybierz bezpłatną wersję próbną, którą chcesz zaoferować, a następnie wybierz pozycję **Prześlij.** Wszystkie wersje próbne są dostępne przez 30 dni, podczas których nie będą naliczane faktury. Możesz również przekonwertować ją na płatną subskrypcję w dowolnym momencie okresu próbnego.

## <a name="converting-trials-to-paid-subscriptions"></a>Konwertowanie wersji próbnych na płatne subskrypcje

Bezpłatna wersja próbna nie jest automatycznie konwertowana na płatną subskrypcję. Po upływie 30 dni bezpłatna wersja próbna musi zostać przekonwertowana na płatną subskrypcję lub [wygaśnie.](#expiring-offers) Bezpłatnych wersji próbnych nie można rozszerzyć.

Musisz samodzielnie przekonwertować wersję próbną na płatną subskrypcję. Możesz to zrobić przy [użyciu interfejsu Partner Center](#convert-trials-using-partner-center) lub [za pośrednictwem Partner Center API.](#convert-trials-using-apis)

> [!NOTE]
> Bezpłatne wersje próbne klienta programu Dostawca rozwiązań w chmurze (CSP) nie mogą zostać przekonwertowane na inną dzierżawę programu (taką jak EA, Open lub MOSP).

### <a name="convert-trials-using-partner-center"></a>Konwertowanie wersji próbnych przy użyciu Partner Center

Wersje próbne można konwertować na płatne subskrypcje przy użyciu Partner Center:

1. Przejdź do strony subskrypcji klienta i wybierz bezpłatną wersję próbną.
2. Wybierz pozycję **Konwertuj wersję próbną na płatną subskrypcję.**
3. Wprowadź żądaną liczbę licencji i częstotliwość rozliczeń, a następnie wybierz pozycję **Zastosuj.**
4. Rozliczanie płatnej subskrypcji rozpoczyna się od daty konwersji, a subskrypcja jest odnawiana automatycznie 12 miesięcy od daty konwersji. 

### <a name="convert-trials-using-apis"></a>Konwertowanie wersji próbnych przy użyciu interfejsów API

Może być konieczne zmiana interfejsów API w celu uwzględnienia konwersji bezpłatnej wersji próbnej na płatną subskrypcję. Aby uzyskać więcej informacji, zobacz następującą dokumentację dla deweloperów:

- [Konwertowanie wersji próbnej subskrypcji na płatną](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Pobieranie listy ofert konwersji wersji próbnej](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Wersje próbne bez konwersji

Nie wszystkie wersje próbne można przekonwertować na subskrypcje płatne. Partnerzy mogą korzystać z wersji próbnej, która nie ma konwersji do daty wygaśnięcia. Partnerzy mogą zakupić zgodne oferty, które obsługują te same usługi co oferta wersji próbnej.  Należy to zrobić przed wygaśnięciem wersji próbnej, aby upewnić się, że usługi nowo zakupionych ofert są zgodne z usługami wersji próbnej. 

|**Wersja próbna**   |**Zgodne oferty dla małych firm**   |**Zgodne Enterprise ofert**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams Wersja próbna chmury komercyjnej (inicjowana przez użytkownika)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (wcześniej F1), Office 365 dla Enterprise (E1, E3 i E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>Powyższe oferty mają podobne plany usług z podobną funkcjonalnością, jednak mogą wystąpić pewne różnice między ofertami.

### <a name="expiring-offers"></a>Wygasające oferty

Nie będziesz powiadamiać o wygasających ofertach. Przyszłe daty wygaśnięcia można śledzić przy użyciu widoku klienta na Partner Center lub przez odpytanie interfejsu API. Dobrym pomysłem jest częste monitorowanie tych dat, aby można było podjąć odpowiednie działania z klientami, gdy podchodzą do punktu decyzyjnego.

Po wygaśnięciu wersji próbnej klient, który spróbuje zalogować się do tej wersji próbnej, zobaczy komunikat o wygaśnięciu. Jednak dane są przechowywane zgodnie ze standardami przechowywania danych. Po zakupie nowej subskrypcji przy użyciu tych samych planów usług informacje o kliencie będą ponownie dostępne z nowo aktywowanej subskrypcji.

## <a name="billing"></a>Rozliczenia

Roczne rozliczenia i bezpłatne wersje próbne są takie same w suwerennych chmurach i w chmurze publicznej. Jedyną różnicą są jednostki SKU w wersji próbnej dostępne w momencie uruchomienia.

## <a name="billing-for-free-trials"></a>Rozliczenia za bezpłatne wersje próbne

Bezpłatne wersje próbne mogą być używane w przypadku subskrypcji rozliczanych co miesiąc i rocznie. Częstotliwość rozliczeń można wybrać podczas konwertowania wersji próbnej na płatną subskrypcję.

Data rozpoczęcia subskrypcji zależy od daty konwersji. Jeśli bezpłatna wersja próbna zostanie przekonwertowana na płatną ofertę z rozliczeniami rocznymi, data odnowienia subskrypcji będzie 12 miesięcy od daty konwersji. Jeśli bezpłatna wersja próbna zostanie przekonwertowana na ofertę płatną z rozliczeniami miesięcznymi, data odnowienia subskrypcji będzie 12 miesięcy od daty rozliczeniowej następującej po dacie konwersji.

### <a name="invoices"></a>Faktury

Bezpłatne wersje próbne nie będą wyświetlane na fakturze lub w pliku uzgodnień opartym na licencjach. Bezpłatne wersje próbne będą wyświetlane w pliku uzgodnień na podstawie faktury i licencji tylko po przekonwertowaniu bezpłatnej wersji próbnej na płatną subskrypcję. Przekonwertowana subskrypcja będzie wyświetlana w taki sam sposób jak każda nowa subskrypcja.

### <a name="incentives"></a>Zachęty

Bezpłatne wersje próbne nie mają wpływu na zachęty.

## <a name="support"></a>Pomoc techniczna

Aby uzyskać pomoc techniczną w przypadku bezpłatnych wersji próbnych, prześlij żądanie obsługi za pośrednictwem Partner Center.