---
title: Oferuj klientom wersje próbne produktów firmy Microsoft
ms.topic: article
ms.date: 08/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Pozwól klientom wypróbować produkty subskrypcji firmy Microsoft. Zarejestruj się, aby korzystać z tych bezpłatnych wersji próbnych w katalogu, podobnie jak wiele innych Usługi online.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f6ac84a832a0c1b0d00d03e10d1bab3f524ed1df
ms.sourcegitcommit: 8eaef380caa66ae3c8e2674535e06c3676fa35f2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/04/2021
ms.locfileid: "129415744"
---
# <a name="give-customers-free-trials-of-microsoft-products"></a>Zapewnij klientom bezpłatne wersje próbne produktów firmy Microsoft

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent sprzedaży

Dobrym sposobem na wprowadzenie klientów do nowych produktów firmy Microsoft jest oferta 30-dniowych bezpłatnych wersji próbnych. Możesz zarejestrować się, aby korzystać z wersji próbnych w katalogu, podobnie jak wiele innych Usługi online. Wszyscy partnerzy mogą uczestniczyć w programie.

## <a name="available-trial-offers"></a>Dostępne oferty wersji próbnej

Wszystkie oferty zaległej wersji próbnej można znaleźć na **stronie Klienta.** Ta strona zawiera listę wszystkich subskrypcji, w tym bezpłatne wersje próbne i płatne subskrypcje. (Ta funkcja nie jest obecnie dostępna w Chinach).

Każdy klient ma prawo do jednej bezpłatnej wersji próbnej dla każdej dostępnej oferty. Na przykład mogą uzyskać jedną bezpłatną wersję próbną dla Microsoft 365 Business Standard i jedną bezpłatną wersję próbną dla Office 365 E3. Jeśli jednak klient jest już właścicielem oferty, nie może użyć bezpłatnej wersji próbnej dla tej oferty.

### <a name="available-products"></a>Dostępne produkty

Bezpłatne wersje próbne są dostępne dla najbardziej kompleksowych i popularnych ofert opartych na licesenach. Nowe oferty wersji próbnej mogą być wprowadzane co miesiąc.

Partnerzy mogą znaleźć wersje próbne w cenniku miesięcznym na stronie **cen i ofert** w Partner Center. Oferty wersji próbnej będą zawierały "WERSJA PRÓBNA" wymienione w kolumnie cennika **Pomocniczy typ** licencji.

Obecnie nie ma **bezpłatnych wersji próbnych** ofert dla instytucji rządowych, ofert edukacyjnych ani ofert dodatków.

## <a name="licenses-for-free-trial-offers"></a>Licencje na oferty bezpłatnej wersji próbnej

Wszystkie bezpłatne wersje próbne zapewniają 25 licencji. Nie można zmienić tej liczby podczas okresu próbnego. W bezpłatnej wersji próbnej nie można dodawać ani usuwać licencji. Po przekonwertowaniu wersji próbnej na płatną subskrypcję możesz dodać więcej licencji do subskrypcji.

Licencje próbne powinny być przypisywane do użytkowników w taki sam sposób, jak licencje usług płatnych.

## <a name="sign-customers-up-for-trials"></a>Rejestracja klientów na potrzeby wersji próbnych

Uzyskaj wersję próbną dla klienta w Partner Center:

1. Z **katalogu** Sell on the Partner Center przejdź **do** katalogu . 
2. W katalogu w opcji **Częstotliwość rozliczeń** wybierz pozycję Oferta **wersji próbnej.** Umożliwia to wyświetlanie tylko bezpłatnych wersji próbnych i wyłączanie innych ofert, które nie są bezpłatne. Wersje próbne będą wyświetlane na karcie **Wersje** próbne w katalogu.
3. Wybierz bezpłatną wersję próbną, którą chcesz zaoferować, a następnie wybierz pozycję **Prześlij.** Wszystkie wersje próbne są przez 30 dni, podczas których nie będą naliczane faktury. Możesz również przekonwertować ją na płatną subskrypcję w dowolnym momencie podczas okresu próbnego.

## <a name="converting-trials-to-paid-subscriptions"></a>Konwertowanie wersji próbnych na płatne subskrypcje

Bezpłatna wersja próbna nie jest automatycznie konwertowana na płatną subskrypcję. Po upływie 30 dni bezpłatna wersja próbna musi zostać przekonwertowana na płatną subskrypcję lub [wygaśnie.](#expiring-offers) Bezpłatnych wersji próbnych nie można rozszerzyć.

Musisz samodzielnie przekonwertować wersję próbną na płatną subskrypcję. Można to zrobić za [pomocą Partner Center](#convert-trials-using-partner-center) lub [za pośrednictwem Partner Center API.](#convert-trials-using-apis)

> [!NOTE]
> Bezpłatne wersje próbne klienta programu Dostawca rozwiązań w chmurze (CSP) nie mogą zostać przekonwertowane na inną dzierżawę programu (taką jak EA, Open lub MOSP).

### <a name="convert-trials-using-partner-center"></a>Konwertowanie wersji próbnych przy użyciu Partner Center

Wersje próbne można konwertować na płatne subskrypcje przy użyciu Partner Center:

1. Przejdź do strony subskrypcji klienta i wybierz bezpłatną wersję próbną.
2. Wybierz pozycję **Konwertuj wersję próbną na płatną subskrypcję.**
3. Wprowadź żądaną liczbę licencji i częstotliwość rozliczeń, a następnie wybierz pozycję **Zastosuj.**
4. Rozliczanie płatnej subskrypcji rozpoczyna się od daty konwersji, a subskrypcja jest automatycznie odnawiana po 12 miesiącach od daty konwersji. 

### <a name="convert-trials-using-apis"></a>Konwertowanie wersji próbnych przy użyciu interfejsów API

Może być konieczne zmiana interfejsów API w celu uwzględnienia konwersji bezpłatnej wersji próbnej na płatną subskrypcję. Aby uzyskać więcej informacji, zobacz następującą dokumentację dla deweloperów:

- [Konwertowanie wersji próbnej subskrypcji na płatną](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Pobieranie listy ofert konwersji wersji próbnej](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Wersje próbne bez konwersji

Nie wszystkie wersje próbne można przekonwertować na płatne subskrypcje. Partnerzy mogą korzystać z wersji próbnej, która nie ma konwersji do daty wygaśnięcia. Partnerzy mogą zakupić zgodne oferty, które obsługują te same usługi co oferta wersji próbnej.  Należy to zrobić przed wygaśnięciem wersji próbnej, aby upewnić się, że nowo zakupione usługi ofert są zgodne z usługami wersji próbnej. 

|**Wersja próbna**   |**Zgodne oferty dla małych firm**   |**Zgodne Enterprise ofert**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams Wersja próbna chmury komercyjnej (inicjowana przez użytkownika)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (wcześniej F1), Office 365 dla Enterprise (E1, E3 i E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

> [!NOTE]
> Powyższe oferty mają podobne plany usług z podobną funkcjonalnością, jednak mogą wystąpić pewne różnice między ofertami.

### <a name="expiring-offers"></a>Wygasające oferty

Nie będziesz powiadamiać o wygasających ofertach. Nadchodzące daty wygaśnięcia można śledzić przy użyciu widoku klienta Partner Center lub przez odpytanie interfejsu API. Dobrym pomysłem jest częste monitorowanie tych dat, aby można było podjąć odpowiednie działania z klientami, gdy podchodzą do punktu decyzyjnego.

Po wygaśnięciu wersji próbnej klient, który próbuje zalogować się do tej wersji próbnej, zobaczy komunikat o wygaśnięciu. Jednak dane są przechowywane zgodnie ze standardami przechowywania danych. Po zakupie nowej subskrypcji z tym samym planem usługi można ponownie uzyskać dostęp do informacji o kliencie z nowo aktywowanej subskrypcji.

## <a name="converting-new-commerce-trials-to-paid-subscriptions"></a>Konwertowanie nowych wersji próbnych handlu na płatne subskrypcje

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego doświadczenia handlowego M365/D365 w wersji Technical Preview.

Po upływie 30 dni bezpłatna wersja próbna zostanie automatycznie odnowiona do równoważnej płatnej subskrypcji. Podczas konwertowania z wersji próbnej na nową płatną subskrypcję należy przekonwertować co najmniej wszystkie 25 stanowisk na nową płatną subskrypcję. Partnerzy mogą dodać więcej niż 25 stanowisk przy konwersji, ale zmniejszenie liczby stanowisk jest niedozwolone.

Partnerzy mogą również konwertować wersje próbne na istniejące płatne subskrypcje. W tym scenariuszu istniejąca subskrypcja musi być subskrypcją, która kwalifikuje się do konwersji wersji próbnej. Jeśli tak, miejsca w wersji próbnej zostaną dodane do istniejącej subskrypcji, a data zakończenia pozostanie taka sama dla istniejącej płatnej subskrypcji.

> [!NOTE]
> Data zakończenia istniejącej płatnej jednostek SKU musi nastąpić tego samego dnia lub po dacie zakończenia okresu próbnego, aby można było wykonać konwersję z wersji próbnej na istniejącą płatną subskrypcję. 

Podczas konwertowania wersji próbnej na nową płatną subskrypcję partnerzy mogą dokonać konwersji na tę samą płatną wersję SKU lub podwyżsić poziom do wyższej wersji SKU. Jeśli chcesz przekonwertować wersję próbną na płatną subskrypcję przed zakończeniem okresu próbnego, możesz to zrobić za pośrednictwem interfejsów API usługi Partner Center lub za pośrednictwem usługi Partner Center, wykonaj poniższe kroki.



> [!NOTE]
> Bezpłatne wersje próbne klienta programu Dostawca rozwiązań w chmurze (CSP) nie mogą zostać przekonwertowane na inną dzierżawę programu (taką jak EA, Open lub MOSP).

### <a name="convert-new-commerce-trials-using-partner-center"></a>Konwertowanie nowych wersji próbnych handlu przy użyciu Partner Center

> [!NOTE]
> Nowe zmiany w handlu są obecnie dostępne tylko dla partnerów, którzy są częścią nowego doświadczenia handlowego M365/D365 w wersji Technical Preview.

Nowe wersje próbne handlu można przekonwertować na płatne subskrypcje przy użyciu Partner Center:

1. Przejdź do strony subskrypcji klienta i wybierz bezpłatną wersję próbną.
2. Wybierz pozycję **Konwertuj wersję próbną na płatną subskrypcję.**
3. Wybierz płatny odpowiednik, a następnie wybierz pozycję **Prześlij.**
4. Rozliczanie płatnej subskrypcji rozpoczyna się od daty konwersji, a subskrypcja jest odnawiana automatycznie przez 12 miesięcy od daty konwersji.

Konwersje próbne muszą być zarządzane przez partnera; nie ma żadnych alertów opartych na subskrypcji w Partner Center, aby powiadamiać partnerów o wygaśnięciu wersji próbnej.

> [!NOTE] 
> W przypadku konwersji na nową subskrypcję okres trwania domyślnie wynosi 1 rok, a cykl rozliczeniowy domyślnie jest planem miesięcznym. 

## <a name="billing"></a>Rozliczenia

Roczne rozliczenia i bezpłatne wersje próbne są takie same w suwerennych chmurach i chmurze publicznej. Jedyną różnicą są jednostki SKU w wersji próbnej dostępne w momencie uruchamiania.

## <a name="billing-for-free-trials"></a>Rozliczenia za bezpłatne wersje próbne

Bezpłatne wersje próbne mogą być używane zarówno w przypadku subskrypcji rozliczanych co miesiąc, jak i rocznie. Częstotliwość rozliczeń można wybrać podczas konwertowania wersji próbnej na płatną subskrypcję. Domyślne ustawienia konwersji są ustawione na okres 1 roku i miesięczny okres rozliczeniowy.

Data rozpoczęcia subskrypcji jest oparta na dacie konwersji. Jeśli bezpłatna wersja próbna zostanie przekonwertowana na płatną ofertę z rozliczeniami rocznymi, data odnowienia subskrypcji będzie 12 miesięcy od daty konwersji. Jeśli bezpłatna wersja próbna zostanie przekonwertowana na ofertę płatną z rozliczeniami miesięcznymi, data odnowienia subskrypcji będzie 12 miesięcy od daty rozliczeniowej następującej po dacie konwersji.

### <a name="invoices"></a>Faktury

Bezpłatne wersje próbne nie będą wyświetlane na fakturze lub w pliku uzgodnień opartym na licencjach. Bezpłatne wersje próbne będą wyświetlane w pliku uzgodnień na podstawie faktury i licencji tylko po przekonwertowaniu bezpłatnej wersji próbnej na płatną subskrypcję. Przekonwertowana subskrypcja będzie wyświetlana w taki sam sposób jak każda nowa subskrypcja.

### <a name="incentives"></a>Zachęty

Bezpłatne wersje próbne nie mają wpływu na zachęty.

## <a name="support"></a>Pomoc techniczna

Aby uzyskać pomoc techniczną w przypadku bezpłatnych wersji próbnych, prześlij żądanie obsługi za pośrednictwem Partner Center.
