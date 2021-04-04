---
title: Oferuj klientom wersje próbne produktów firmy Microsoft
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zezwól klientom na wypróbowanie produktów z subskrypcji firmy Microsoft przez 30 dni. Zarejestruj się, aby korzystać z bezpłatnych wersji próbnych w katalogu, tak jak w przypadku wielu innych Usługi online.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 53f4a16ac5d0f33fd534d7fd9a13eaf5a25cf3ea
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132336"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Daj klientom 30-dniowych, bezpłatnych wersji próbnych produktów firmy Microsoft

**Odpowiednie role**

- Administrator globalny
- Administrator zarządzania użytkownikami
- Agent sprzedaży

Dobrym sposobem wprowadzenia klientów do nowych produktów firmy Microsoft jest oferowanie 30-dniowych bezpłatnych wersji próbnych. Możesz zarejestrować się w celu uzyskania prób w wykazie tak jak wielu innych Usługi online. Wszyscy partnerzy mogą uczestniczyć w programie.

## <a name="available-trial-offers"></a>Dostępne oferty wersji próbnej

Wszystkie zaległe oferty wersji próbnej można znaleźć na stronie **klienta** . Ta strona zawiera listę wszystkich subskrypcji, w tym bezpłatnych wersji próbnych i płatnych subskrypcji. (Ta funkcja nie jest obecnie dostępna w Chinach).

Każdy klient jest uprawniony do korzystania z jednej bezpłatnej wersji próbnej dla każdej dostępnej oferty. Na przykład mogą skorzystać z jednej bezpłatnej wersji próbnej dla Microsoft 365 Business standardowej i jednej bezpłatnej wersji próbnej pakietu Office 365 E3. Jeśli jednak klient jest już właścicielem oferty, nie może korzystać z bezpłatnej wersji próbnej tej oferty.

### <a name="available-products"></a>Dostępne produkty

Bezpłatne wersje próbne są dostępne dla bardziej kompleksowych i popularnych ofert opartych na licesen. Nowe oferty wersji próbnej mogą być wprowadzane co miesiąc.

Partnerzy mogą znaleźć próbkę na liście cen miesięcznych na stronie **ceny i oferty** w centrum partnerskim. Oferta wersji próbnej będzie miała wartość "wersja PRÓBna" w kolumnie **pomocniczy typ licencji** cennika.

Obecnie **nie ma żadnych bezpłatnych wersji próbnych** z ofertami dla instytucji rządowych, ofertami edukacyjnymi ani ofertami dodatków.

## <a name="licenses-for-free-trial-offers"></a>Licencje na oferty bezpłatnej wersji próbnej

Wszystkie bezpłatne wersje próbne zapewniają 25 licencji. Nie można zmienić tej wartości w okresie próbnym. Nie można dodawać ani usuwać licencji w bezpłatnej wersji próbnej. Po przekonwertowaniu wersji próbnej na płatną subskrypcję możesz dodać więcej licencji do subskrypcji.

Licencje na wersję próbną powinny być przypisane do użytkowników w taki sam sposób, jak w przypadku przypisywania płatnych usług.

## <a name="sign-customers-up-for-trials"></a>Podpisz klientom do wersji próbnej

Uzyskaj wersję próbną dla klienta w centrum partnerskim:

1. Ze **sprzedającego** w centrum partnerskim przejdź do **katalogu**. 
2. W wykazie w obszarze **częstotliwość rozliczeń** wybierz pozycję **Oferta wersji próbnej**. Pozwala to na wyświetlanie tylko bezpłatnych wersji próbnych i uniemożliwia korzystanie z innych ofert, które nie są bezpłatne. Wersje próbne będą widoczne na karcie **testy** w wykazie.
3. Wybierz bezpłatną wersję próbną, którą chcesz zaoferować, a następnie wybierz pozycję **Prześlij**. Wszystkie wersje próbne są przez 30 dni, w których nie będą naliczane opłaty. Możesz również przekonwertować ją na płatną subskrypcję w dowolnym momencie w okresie próbnym.

## <a name="converting-trials-to-paid-subscriptions"></a>Konwertowanie prób na Płatne subskrypcje

Bezpłatna wersja próbna nie jest automatycznie konwertowana na płatną subskrypcję. Po 30 dniach bezpłatna wersja próbna musi być konwertowana na płatną subskrypcję lub [wygaśnie](#expiring-offers). Nie można rozszerzyć bezpłatnych wersji próbnych.

Musisz samodzielnie przekonwertować wersję próbną na płatną subskrypcję. Można to zrobić [przy użyciu Centrum partnerskiego](#convert-trials-using-partner-center) lub [interfejsów API Centrum partnerskiego](#convert-trials-using-apis).

> [!NOTE]
> Nie można przekonwertować bezpłatnych wersji próbnych klienta dla programu Cloud Solution Provider (CSP) na inną dzierżawę programu (na przykład EA, Open lub MOSP).

### <a name="convert-trials-using-partner-center"></a>Konwertuj wersje próbne przy użyciu Centrum partnerskiego

Możesz konwertować wersje próbne na Płatne subskrypcje przy użyciu Centrum partnerskiego:

1. Przejdź do strony subskrypcji klienta i wybierz bezpłatną wersję próbną.
2. Wybierz pozycję **Konwertuj wersję próbną na płatną subskrypcję**.
3. Wprowadź odpowiednią liczbę licencji i częstotliwość rozliczeń, a następnie wybierz pozycję **Zastosuj**.
4. Naliczanie opłat za płatną subskrypcję rozpoczyna się od daty konwersji, a subskrypcja subskrypcji jest odnawiana przez 12 miesięcy od daty konwersji. 

### <a name="convert-trials-using-apis"></a>Konwertowanie prób przy użyciu interfejsów API

Może być konieczne zmodyfikowanie interfejsów API w celu uwzględnienia konwersji bezpłatnej wersji próbnej na płatną subskrypcję. Aby uzyskać więcej informacji, zobacz następującą dokumentację dla deweloperów:

- [Konwertowanie wersji próbnej subskrypcji na płatną](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Pobieranie listy ofert konwersji wersji próbnej](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Próby bez konwersji

Nie wszystkie wersje próbne można przekonwertować na Płatne subskrypcje. Partnerzy mogą korzystać z wersji próbnej, która nie ma konwersji do daty wygaśnięcia. Partnerzy mogą zakupić zgodne oferty, które obsługują te same usługi co oferta wersji próbnej.  Należy to zrobić przed wygaśnięciem okresu próbnego, aby zapewnić, że nowo zakupione oferty są wyrównane z usługami w wersji próbnej. 

|**Wersja próbna**   |**Zgodne oferty małych firm**   |**Zgodne oferty dla przedsiębiorstw**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Wersja próbna chmury Microsoft Teams (zainicjowane przez użytkownika)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (dawniej F1), Office 365 dla przedsiębiorstw (E1, E3 i E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>Powyższe oferty mają podobne plany usługi o podobnej funkcjonalności, jednak mogą występować pewne różnice między ofertami.

### <a name="expiring-offers"></a>Oferty wygasające

Użytkownik nie będzie powiadamiany o wygasaniu ofert. Możesz śledzić nadchodzące daty wygaśnięcia, korzystając z widoku klienta w centrum partnerskim lub badając interfejs API. Dobrym pomysłem jest częste monitorowanie tych dat, aby można było podjąć odpowiednie działania uzupełniające klientom w miarę podejścia do punktu decyzyjnego.

Po wygaśnięciu wersji próbnej klient, który próbuje zalogować się do tej wersji próbnej, zobaczy komunikat o wygaśnięciu. Dane są jednak przechowywane zgodnie z normami przechowywania danych. Po zakupie nowej subskrypcji z tymi samymi planami usług informacje o kliencie są dostępne ponownie z nowo aktywowanej subskrypcji.

## <a name="billing"></a>Rozliczenia

Roczne Rozliczanie i bezpłatne wersje próbne są takie same w chmurach suwerennych i w chmurze publicznej. Jedyną różnicą jest to, że jednostki SKU wersji próbnej są dostępne w momencie uruchomienia.

## <a name="billing-for-free-trials"></a>Rozliczanie bezpłatnych wersji próbnych

Bezpłatnych wersji próbnych można używać zarówno w przypadku subskrypcji miesięcznych, jak i rocznych. Możesz wybrać częstotliwość rozliczeń w przypadku konwersji wersji próbnej na płatną subskrypcję.

Data rozpoczęcia subskrypcji jest określana na podstawie daty konwersji. Jeśli bezpłatna wersja próbna zostanie przekonwertowana na płatną ofertę z rocznymi rozliczeniami, Data odnowienia subskrypcji będzie 12 miesięcy od daty konwersji. Jeśli bezpłatna wersja próbna zostanie przekonwertowana na płatną ofertę za comiesięczne rozliczanie, Data odnowienia subskrypcji będzie 12 miesięcy od daty rozliczenia po dacie konwersji.

### <a name="invoices"></a>Faktury

Nie zobaczysz bezpłatnych wersji próbnych wymienionych na fakturze lub w pliku uzgadniania na podstawie licencji. Bezpłatne wersje próbne będą widoczne tylko w przypadku faktury i pliku uzgadniania opartego na licencji po przeprowadzeniu konwersji bezpłatnej wersji próbnej na płatną subskrypcję. Przekonwertowana subskrypcja zostanie wyświetlona w taki sam sposób jak w przypadku każdej nowej subskrypcji.

### <a name="incentives"></a>Zachęty

Bezpłatne wersje próbne nie mają wpływu na zachęty.

## <a name="support"></a>Pomoc techniczna

Aby uzyskać pomoc techniczną dotyczącą bezpłatnych wersji próbnych, Prześlij żądanie obsługi za pomocą Centrum partnerskiego.