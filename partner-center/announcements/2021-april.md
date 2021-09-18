---
title: Ogłoszenia z kwietnia 2021 r.
description: Ogłoszenia dotyczące platformy Microsoft Partner Center w kwietniu 2021 r., w tym nowe możliwości, promocje, oferty, rynki lub zmiany istniejących ofert.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 09/01/2021
ms.openlocfilehash: a6cd5e9734a2ba9657649f012225dee96cd1e265
ms.sourcegitcommit: 8d5c2463fc0f0c03972a6f89d01605421288daea
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/18/2021
ms.locfileid: "127932838"
---
# <a name="april-2021-announcements"></a>Ogłoszenia z kwietnia 2021 r.

Ta strona zawiera ogłoszenia dotyczące usługi Microsoft Partner Center na kwiecień 2021 r.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Gotowość: zaktualizowany interfejs API weryfikacji adresu klienta dostawcy usług w chmurze zostanie zaktualizowany w czerwcu; Możliwość testowania jest teraz dostępna

### <a name="categories"></a>Kategorie

- Data: 2021-04-30
- Gotowość

### <a name="summary"></a>Podsumowanie

Aby ułatwić partnerom i klientom prowadzenia działalności w oparciu o zaufanie, będziemy zapraszać partnerów do testowania zmian w interfejsie API weryfikowania adresów dla wszystkich krajów na całym świecie.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy tworzą nowe lub aktualizują szczegóły adresów istniejących klientów

### <a name="details"></a>Szczegóły

Firma Microsoft działa w oparciu o zaufanie. Dążymy do zapewnienia zgodnej, bezpiecznej i bezpiecznej metody weryfikacji adresu klienta na potrzeby transakcji subskrypcji klientów w programie CSP. Od 31 marca 2021 r. wprowadziliśmy zmiany w interfejsie API weryfikacji adresu. Zachęcamy partnerów do przetestowania interfejsu API przed rozpoczęciem jego transmisji na żywo pod koniec czerwca 2021 r. 

Należy pamiętać, że te zmiany mają wpływ tylko na interfejs API weryfikacji adresu. Nie ma to wpływu na interfejsy API tworzenia klienta i aktualizowania profilu rozliczeniowego. Chociaż sugerowany adres nie musi być obecnie używany z interfejsem API tworzenia klienta, jest to zdecydowanie zalecane.

Odpowiedź zwróci jeden z następujących komunikatów o stanie:

| Stan     | Opis |    Liczba zwracanych sugerowanych adresów |
|-------|---------------|-------------------|
|Zweryfikowana wysyłka | Adres jest weryfikowany i można go wysłać. | Pojedynczy |
|Sprawdzonych | Adres jest weryfikowany. | Pojedynczy |
|Wymagana interakcja | Sugerowany adres został znacząco zmieniony i wymaga potwierdzenia przez użytkownika. | Pojedynczy |
|Część częściowa ulicy | Podana ulica w adresie jest częściowa i wymaga więcej informacji. | Wielokrotność — maksymalnie trzy |
|Część lokalna | Dane lokalne (numer budynku, numer pakietu i inne) są częściowe i wymagają więcej informacji. | Wielokrotność — maksymalnie trzy |
|Wiele | Istnieje wiele pól, które są częściowo w adresie (potencjalnie również częściowe ulice i część lokalna). | Wielokrotność — maksymalnie trzy |
|Brak | Adres jest nieprawidłowy. | Brak |
|Nie sprawdzono | Nie można wysłać adresu w procesie walidacji. | Brak |

Kody pocztowe w USA zwracają dodatkowe cztery cyfry i łącznik, na przykład 12345-6789.

### <a name="next-steps"></a>Następne kroki

- Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.
- Przygotuj się do uwzględnienia zmian przy użyciu interfejsu API Partner Center i internetowego interfejsu użytkownika. 
- Udostępnij swój identyfikator dzierżawy piaskownicy ekspertowi w tej dziedzinie (Ali Ichki), który zostanie uwzględniony w teście testowym, aby rozpocząć przygotowywanie aktualizacji. 
- Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.

### <a name="questions"></a>Masz pytania?

Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych przez firmę Microsoft, uzyskaj pomoc techniczną Yammer partnerów lub otwórz [żądanie obsługi.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Nowa lokalizacja dokumentacji programu Swagger Partner Center API

### <a name="categories"></a>Kategorie

- Data: 2021-04-26
- Możliwości

### <a name="summary"></a>Podsumowanie

Partner Center api Swagger zostały zmigrowane z poprzedniej witryny dokumentacji programu [Swagger](https://apidocs.microsoft.com/services/partnercenter) do nowej witryny dokumentacji programu [Swagger.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy rozliczający się bezpośrednio i dostawcy pośredni biorący udział w programie Dostawca rozwiązań w chmurze (CSP), którzy korzystali z interfejsów API Partner Center internetowych

### <a name="details"></a>Szczegóły

Od 26 kwietnia 2021 r. dokumentacja programu Swagger interfejsu API Partner Center, w tym zawartość interfejsu API REST, znajduje się w [nowej witrynie.](/rest/api/partner-center-rest/) Stara witryna będzie niedostępna po kilku tygodniach.

### <a name="benefits"></a>Korzyści

Dokumentacja Partner Center API swagger będzie dostarczać funkcję **Wypróbuj.** Aby użyć tej funkcji, musisz mieć token bearer, który można wygenerować, korzystając z kroków wymienionych w te Partner Center Authentication ( [Uwierzytelnianie).](/partner-center/develop/partner-center-authentication#app--user-authentication)

### <a name="next-steps"></a>Następne kroki

Udostępnij te informacje w organizacji, aby odpowiedni zespół może przeglądać i aktualizować swoje procesy.

### <a name="questions"></a>Masz pytania?

W przypadku pytań dotyczących tych ofert sprawdź odpowiednie Yammer społeczności.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Dostawca rozwiązań w chmurze (CSP) dotyczące okresu zwrotu oprogramowania i powiadomienia o wygaśnięciu linku pobierania

### <a name="categories"></a>Kategorie

- Data: 2021-04-21
- Możliwości

### <a name="summary"></a>Podsumowanie

W zasadach okresów powrotu oprogramowania CSP i wygaśnięcia linku pobierania w programie CSP wejdą zmiany.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy w ramach transakcji bezterminowych ofert subskrypcji oprogramowania lub oprogramowania w programie CSP

### <a name="details"></a>Szczegóły

Zwróć uwagę na następujące ważne powiadomienia dotyczące bezterminowego zakupu oprogramowania i subskrypcji oprogramowania za pośrednictwem Partner Center:

#### <a name="software-return-period-policy"></a>Zasady okresu zwrotu oprogramowania

Od 1 czerwca 2021 r. okres zwrotu dla ofert oprogramowania w programie CSP, zgodnie z Microsoft Partner Agreement (MPA), zmieni się z 60 dni od daty zamówienia do 30 dni od daty zamówienia.

Po przesłaniu zamówienia na ofertę oprogramowania partnerzy będą mieć 30 dni od daty zamówienia, aby przesłać poprawki do takiego zamówienia:

- Każda bezterminowa licencja na oprogramowanie zwrócona w ciągu 30-dniowego okresu zwrotu otrzyma pełne środków z płatnej ceny zakupu.

- Każdy produkt subskrypcji oprogramowania zwrócony w 30-dniowym okresie zwrotu otrzyma proporcjonalną kredyt z płatnej ceny zakupu.

Ta wiadomość jest kontynuacją naszej wiadomości e-mail wysłanej w grudniu 2020 r. i kwietniu 2021 r. do wszystkich partnerów CSP w związku z okresem zwrotu i innymi aktualizacjami mpA. Zapoznaj się z tymi uwagami, aby uzyskać szczegółowe informacje dotyczące zmian wpływających na owe mpA.

#### <a name="software-download-link-expiry"></a>Wygaśnięcie linku pobierania oprogramowania

Od 3 czerwca 2021 r. linki do pobierania oprogramowania w przypadku bezterminowego zakupu oprogramowania i subskrypcji oprogramowania za pośrednictwem usługi Partner Center będą mieć datę wygaśnięcia 5 dni od początkowego pobrania. Okres wygaśnięcia będzie miał zastosowanie do wszystkich zakupów przed 3 czerwca 2021 r. oraz od 3 czerwca 2021 r.

### <a name="next-steps"></a>Następne kroki

Przejrzyj okres [zwrotny CSP i pobierz często](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)zadawane pytania dotyczące wygaśnięcia linku i poinformuj wszystkie odpowiednie zespoły w organizacji o tych zmianach:

### <a name="questions"></a>Masz pytania?

W przypadku pytań dotyczących tych ofert sprawdź odpowiednie Yammer społeczności.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Otwórz program licencjonowania: Przejście odsprzedawców do programu licencjonowania Dostawca rozwiązań w chmurze (CSP)

### <a name="categories"></a>Kategorie

- Data: 2021-04-19
- Rozwój firmy

### <a name="summary"></a>Podsumowanie

W tym komunikacie szczegółowo opisano sposób przygotowania się do zmian, które zostaną wkrótce wprowadzone w programie licencjonowania Open.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy CSP i Open License

### <a name="details"></a>Szczegóły

W 2020 r. firma [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) ogłosiła, że bezterminowe licencje na oprogramowanie będą szeroko dostępne dla partnerów i klientów w ramach programu Dostawca rozwiązań w chmurze (CSP). Pierwszy kamień milowy został osiągnięty w styczniu 2021 r., gdy stały się dostępne bezterminowe oferty oprogramowania komercyjnego. Następny kluczowy kamień milowy nastąpi w lipcu 2021 r., gdy [staną](https://aka.ms/openlicensepublicsector) się dostępne oferty sektora publicznego. Przekazaliśmy również informacje o tym, że od 1 stycznia 2022 r. nie będzie można kupować nowych licencji na oprogramowanie ani odnawiania licencji usługi pakiet Software Assurance ani Usługi online za pośrednictwem programu licencjonowania Open. [](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)

Przejście bezterminowego oprogramowania do programu CSP w nowym środowisku handlowym pomoże partnerom rozszerzyć możliwości zaoferowania zróżnicowanych rozwiązań i usług zarządzanych. Przyspieszy to również przejście klientów do chmury.  Aby pomóc zapewnić bezproblemowe przejście dla naszych partnerów i klientów, dostosowaliśmy te korekty i materiały, aby przyspieszyć tę transformację cyfrową:

#### <a name="april-2021"></a>Kwiecień 2021 r.

[Teraz dostępne:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Open License-to-CSP transition materials for resellers (Otwórz materiały przejściowe z licencji na program CSP dla odsprzedawców)

#### <a name="july-2021"></a>Lipiec 2021 r.

##### <a name="csp"></a>CSP

- 1 lipca: bezterminowe licencje na oprogramowanie dostępne dla klientów z sektora publicznego

- 7 lipca: Visual Studio Pro i Get Genuine Windows oprogramowania bezterminowych licencji na oprogramowanie dostępne dla wszystkich segmentów

##### <a name="open-value"></a>Otwórz wartość

- 1 lipca: dodatkowe jednostki SKU dostępne w programie Open Value dla organizacji edukacyjnych i non profit, oferując podobne oferty do programu licencjonowania Open

##### <a name="open-license"></a>Licencja Open

- 1 lipca: firma Microsoft nie będzie już uruchamiać nowych ofert w programie licencjonowania Open.

#### <a name="january-2022"></a>Styczeń 2022 r.

- 1 stycznia: w ramach programu licencjonowania Open License nie można dokonać żadnych nowych zakupów ani odnowień

### <a name="next-steps"></a>Następne kroki

#### <a name="csp-indirect-providers"></a>Dostawcy pośredni dostawcy CSP

Skorzystaj z najbliższych miesięcy, aby pomóc odsprzedawcy licencji Open w zorientowaniu się na program CSP, uczestnicząc w wydarzeniach społeczności partnerów i korzystając z materiałów przejściowych Open License-to-CSP dla odsprzedawców:

- Otwórz materiały przejściowe z licencji na CSP dla odsprzedawców — dostosowywalna prezentacja z omówieniem, szablon wiadomości [e-mail,](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)przewodnik dołączania odsprzedawcy pośredniego programu CSP i inne materiały, które ułatwiają wdrożenie dla odsprzedawców na dużą skalę.

- [Wydarzenia dla partnerów Community CSP hostowane](https://globalpbocomm.eventbuilder.com/GlobalCSP) przez operacje biznesowe firmy Microsoft.  Dołącz do różnych sesji, aby poznać podstawy programu CSP (CSP Fundamentals) lub być na bieżąco i zadawać pytania dotyczące oprogramowania w programie CSP (Q&A Sessions).

- (Już wkrótce) Sesja szkoleniowa ukierunkowana na odsprzedawcę pośredniego w programie CSP hostowana przez firmę Microsoft Business Operations.

#### <a name="open-license-resellers"></a>Odsprzedawcy licencji open

- Jeśli Twoja organizacja nie jest obecnie zarejestrowane w programie CSP, skontaktuj się z dystrybutorem, aby uzyskać informacje na temat rozpoczynania pracy. Połączenie z dostawcą pośrednim w Połączenie u zaufanego dostawcy pośredniego [i rozwijaj swoją firmę.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)

- Jeśli Twoja organizacja jest już zarejestrowane w programie CSP, dowiedz się więcej o oprogramowaniu bezterminowym w programie CSP na stronie Oprogramowanie bezterminowe [w Dostawca rozwiązań w chmurze programie](https://partner.microsoft.com/resources/collection/software-in-csp).

### <a name="questions"></a>Masz pytania?

Aby uzyskać więcej pytań dotyczących tych ofert, sprawdź odpowiednie Yammer społeczności.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Teraz na żywo: Przewodnik dotyczący gotowości na globalną promocję

### <a name="categories"></a>Kategorie

- Data: 2021-04-16
- Możliwości

### <a name="summary"></a>Podsumowanie

Launch Readiness has published a [new global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) (Gotowość do uruchomienia) opublikowano nowy przewodnik dotyczący gotowości na poziomie globalnym w galerii zasobów Operations Readiness. Ten przewodnik zawiera skonsolidowany widok wszystkich aktywnych promocji [globalnych.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Wszyscy partnerzy licencjonowania zbiorowego (VL), dynamics price list (DPL) i Dostawca rozwiązań w chmurze (CSP)

### <a name="details"></a>Szczegóły

Partnerzy firmy Microsoft udostępnili nam potrzebę zapewnienia skonsolidowanego widoku wszystkich globalnych promocji ze szczegółami pomocy technicznej. Chcesz, aby ten skonsolidowany przewodnik ułatwiał korzystanie z promocji z przekonaniem, że wszystkie dostępne informacje będą łatwo dostępne w centralnej i wygodnej lokalizacji.

Począwszy od kwietnia 2021 r., firma Microsoft będzie aktualizować ten przewodnik co miesiąc i będzie on dostępny w dedykowanej kolekcji Przewodnika po globalnej gotowości na promocję w galerii zasobów Gotowość na operacje.

Linki do tego przewodnika będą również zawarte w następujących kolekcjach:

- [Uruchom kolekcję kalendarza](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), która zapewnia scentralizowany widok przyszłych zmian i uruchomień.

- [Community kolekcje](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), które zawierają materiały do obsługi comiesięcznych rozmów z partnerami, z wyróżnieniem nadchodzących zmian i terminowych tematów zainteresowań operacyjnych.

- [Biuletyny partnerów,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)takie jak comiesięczne aktualizacje programu CSP

Jako comiesięczne przypomnienie opublikujemy również Partner Center z każdym nowym problemem przewodnika po globalnej gotowości na promocję.

### <a name="next-steps"></a>Następne kroki

Na początku każdego miesiąca w galerii [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) zasobów Operations Readiness znajdziesz najnowszy globalny przewodnik dotyczący gotowości [na promocję.](https://partner.microsoft.com/resources)

Udostępnij te informacje odpowiednim kontaktom w organizacjach i daj nam znać, jak pomocny jest przewodnik, za pośrednictwem strony "Czy ta strona była pomocna?". na końcu każdej strony.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Aktualizacja społeczności Dostawca rozwiązań w chmurze (CSP) z kwietnia

### <a name="categories"></a>Kategorie

- Data: 2021-04-16
- Community | Zaproszenia i przypomnienia

### <a name="summary"></a>Podsumowanie

Zasoby społeczności CSP są dostępne na żądanie i aktualizowane co miesiąc, aby być na bieżąco z aktualnymi i przygotowanymi do zmian w programie CSP.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy rozliczani bezpośrednio i dostawcy pośredni dostawcy CSP

### <a name="details"></a>Szczegóły

W tym miesiącu zasoby obejmują następujące kluczowe tematy:

- [Aktualizacja do ewolucji programu CSP i zmiany programu Licencjonowanie Open](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Zmiany wymagań dotyczących dołączania klientów w programie CSP w niektórych regionach](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Nowy format nowej faktury w formacie PDF dla handlu w programie CSP](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

W [kolekcji społeczności CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)znajdziesz:

- Biuletyn comiesięcznej aktualizacji programu CSP do pobrania, który agreguje najnowsze ogłoszenia, aktualizacje, zdarzenia i przypomnienia dotyczące programu [CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)w czytelnym dokumencie.

- Kalendarz [anonsów dla programu CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)który zapewnia widok osi czasu przyszłych zmian wpływających na program.

- Nowy kalendarz [uruchamiania produktu](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), w którym można wyświetlić nadchodzące premiery i oferty produktów.

- [Program CSP uruchamia zasoby aktualizacji z](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) łatwą w użyciu zawartością dla kluczowych zmian operacyjnych.

- [Odświeżenia i przypomnienia dotyczące kluczowych](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) tematów dotyczących CSP, które otrzymują zainteresowanie i zapytania.

#### <a name="csp-community-call-qas"></a>CSP Community Q&As

Community Zadzwoń do&Pytania i odpowiedzi, aby uzyskać pomoc w pytaniach związanych z nadchodzącymi zmianami. Zarejestruj się teraz, aby Community Q&Ponieważ odbywa się to w kwietniu, maju i czerwcu. Skupią się one na najnowszych startach, ważnych odświeżeniach i przypomnieniach.

[Zarejestruj się tutaj.](https://globalpbocomm.eventbuilder.com/GlobalCSP)

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby społeczności i zarejestruj się w celu Community pytania&A.

Aby upewnić się, że będziesz maksymalnie zadowoleni z usługi Community Call Q&A, przejrzyj zawartość społeczności na żądanie i prześlij swoje pytania do 48 godzin przed wywołaniem.

### <a name="questions"></a>Masz pytania?

Comiesięczny numer Community CSP&Q&A to najlepsze miejsce na pytania związane ze zmianami w programie CSP. W każdym miesiącu zapoznaj się z materiałami i prześlij pytania z wyprzedzeniem, abyśmy spędzali sesję na najważniejszych tematach.

Aby uzyskać więcej informacji, skontaktuj się z [pomocą techniczną.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Ostatnie przypomnienie: 6 maja 2021 r. oznaczało to, że kwalifikacja GET jest wyefiniowania

### <a name="categories"></a>Kategorie

- Data: 2021-05-04

- Możliwości

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy sprzedają oferty Academic, Nonprofit i Government Community Cloud (GCC) za pośrednictwem programu Dostawca rozwiązań w chmurze przy użyciu interfejsu API Partner Center api

### <a name="details"></a>Szczegóły

To zawiadomienie stanowi kontynuację rozszerzenia usługi Partner Center [wydanych w grudniu.](./2020-december.md#1) W ramach tej wersji zostały wdrożone nowe interfejsy API kwalifikacji GET i POST, w związku z tym istniejąca kwalifikacja GET zostanie wycofana 6 maja **2021 r.** W tym czasie konieczne będzie przejście do korzystania z nowych interfejsów API Partner Center POST. Nowe interfejsy API POST umożliwią zakup ofert edukacyjnych, a nowe interfejsy API GET umożliwią zakup wstępnie kwalifikowanych ofert organizacji nonprofit i GCC edukacji.

### <a name="next-steps"></a>Następne kroki

- **Zaktualizuj do nowych interfejsów API w** celu pomyślnego i terminowego przejścia.

- **Przejrzyj nowe zmiany interfejsu API Partner Center** i Przewodnik w zasobach gotowość do operacji: [ulepszenia procesu weryfikacji](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)klienta Partner Center Education.

- Udostępnij te informacje odpowiednim zespołom w organizacji oraz odsprzedawcom, aby pomóc im przygotować się do tych zmian.

### <a name="questions"></a>Masz pytania?

W przypadku jakichkolwiek pytań związanych z tym powiadomieniem skontaktuj się [z Partner Center pomocą techniczną.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)

### <a name="change-log"></a>Dziennik zmian

- 4 maja 2021 r.: Ostateczne przypomnienie o nadchodzącym cofaniu kwalifikacji GET

- 9 kwietnia 2021 r.: Przypomnienie o zbliżającym się cofaniu kwalifikacji GET 

- Luty: Zaktualizowane osie czasu dla cofania pracy z kwalifikacjami GET & PUT

- Styczeń: Przypomnienie o nadchodzących cofaniach pracy z kwalifikacjami GET & PUT

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Nowy format nowej faktury handlowej w formacie PDF w programie CSP

### <a name="categories"></a>Kategorie

- Data: 2021-04-05
- Możliwości

### <a name="summary"></a>Podsumowanie

Firma Microsoft wprowadza nowy format nowej faktury w formacie PDF dla handlu w programie Dostawca rozwiązań w chmurze (CSP) w celu wyświetlania szczegółów rozliczeń według szczegółów produktu zamiast opisu sku.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy w ramach programu CSP

### <a name="details"></a>Szczegóły

Od maja 2021 r. firma Microsoft wprowadza nowy format nowej faktury w formacie PDF dla handlu w programie CSP w celu wyświetlania szczegółów rozliczeń według szczegółów produktu zamiast opisu sku. Dzięki tej nowej aktualizacji będziemy agregować elementy wiersza według typu produktu, jednocześnie wyświetlając każdy produkt w poszczególnych wierszach.

Partnerzy zauważą, że ta zmiana rozpocznie się na fakturze za maj dla okresu rozliczeniowego od 1 kwietnia 2021 r. do 30 kwietnia 2021 r. Oferty, których to dotyczy, Microsoft Azure wystąpienie zarezerwowane, subskrypcje platformy Azure (plan platformy Azure) i marketplace.

Wszystkie żądania dotyczące środków po zaktualizowaniu formatu faktury zostaną wygenerowane w nowym formacie.

#### <a name="partner-benefits"></a>Korzyści dla partnerów

Ta aktualizacja będzie oferować następujące ulepszenia w zakresie fakturowania dla partnerów:

- Zmniejszenie rozmiaru faktury przy zachowaniu danych krytycznych

- Dopasowanie formatu do standardów branżowych dla kompaktowych i przyjaznych dla użytkownika faktur 

Nie będzie to mieć wpływu na następujące elementy:

- Strona podsumowania rozliczeń w pliku PDF faktury

- Istniejące interfejsy API fakturowania

- Pliki uzgodnień (pliki uzgodnień mogą służyć do pobierania szczegółowych danych). 

- Faktury za użycie i opłaty na podstawie licencji

### <a name="next-steps"></a>Następne kroki

Zapoznaj się z informacjami na ten temat w [galerii zasobów Operations Readiness](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) w witrynie internetowej partnerów firmy Microsoft. Aby uzyskać więcej informacji na temat rozliczeń i podatków, w tym zasobów rozliczeniowych, faktur, rozliczeń CSP i podatków, odwiedź sekcję Rozliczenia [w](../billing.md) Partner Center.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Zmiany wymagań Dostawca rozwiązań w chmurze (CSP) dotyczące dołączania klientów

### <a name="categories"></a>Kategorie

- Data: 2021-04-02
- Oferty/rynki

### <a name="summary"></a>Podsumowanie

W ramach naszego zobowiązania do pomocy partnerom i klientom w zakresie prowadzenia działalności w oparciu o zaufanie poprosimy o dodatkowe informacje o klientach od 25 marca 2021 r.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy mają nowych lub istniejących klientów w krajach wymienionych w następnej sekcji

### <a name="details"></a>Szczegóły

Firma Microsoft działa w oparciu o zaufanie. Dokładamy starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji klienta na potrzeby transakcji subskrypcji klientów w programie CSP. 25 marca 2021 r. wprowadzimy ulepszenia interfejsu API i interfejsu użytkownika usługi Partner Center, które będą mieć wpływ na partnerów spełniających oba następujące kryteria:

- Partner ma bezpośrednią relację rozliczeń z firmą Microsoft (co oznacza, że partner jest partnerem z rozliczaniem bezpośrednim lub dostawcą pośrednim).

- Partner współpracuje z nowymi lub istniejącymi klientami w następujących krajach:

    - Tajlandia
    - Wietnam
    - Turcja
    - Polska
    - Republika Południowej Afryki
    - Indie
    - Brazylia
    - Irak
    - Myanmar
    - Sudan Południowy
    - Arabia Saudyjska
    - Zjednoczone Emiraty Arabskie
    - Wenezuela

Partnerzy spełniający te kryteria muszą przesłać identyfikator rejestracji firmy klienta (znany także jako organizacja klienta), oraz numer telefonu podczas następnej aktualizacji lub tworzenia subskrypcji dla tego klienta. Ci partnerzy mogą również wprowadzić opcjonalne drugie imię klienta.

Pamiętaj, że podczas dodawania identyfikatora rejestracji firmy należy użyć identyfikatora podatku od działalności biznesowej, a nie identyfikatora osobistego klienta.

Partnerzy, którzy firma współpracuje z nowymi lub istniejącymi klientami w następujących krajach, są już dołączani do poprzedniej wersji w listopadzie 2020 r.

- Armenia
- Azerbejdżan
- Białoruś
- Węgry
- Kazachstan
- Kirgistan
- Mołdawia
- Rosja
- Tadżykistan
- Ukraina
- Uzbekistan

Pod koniec marca 2021 r. partnerzy z klientami na całym świecie będą mieć możliwość wprowadzania identyfikatora rejestracji firmy, numeru telefonu i średniego imienia dla klientów jako opcjonalnych szczegółów.

### <a name="next-steps"></a>Następne kroki

- Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.
- Przygotuj się do uwzględnienia zmian przy użyciu Partner Center API i użytkownika internetowego. Zestawy API/zestawy SDK będą dostępne do testowania.
- Pamiętaj, aby przesłać dodatkowe dane podczas dołączania nowych klientów lub modyfikowania istniejących danych klienta.
- Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.

>[!NOTE]
>Jeśli nie można przetworzyć transakcji CSP, może to oznaczać, że dzierżawa nie jest weryfikowana. W takim przypadku klient musi zakupić ofertę wersji próbnej w portalu administracyjnym firmy Microsoft.
>
>#### <a name="purchase-a-trial-offer"></a>Kupowanie oferty wersji próbnej
>
>1. Otwórz [portal Centrum administracyjnego firmy Microsoft.](https://admin.microsoft.com/)
>
>2. W menu nawigacji po lewej stronie wybierz **pozycję Rozliczenia**, a następnie pozycję **Kup usługi.**
>
>3. Wybierz plan, a następnie wybierz pozycję **Checkout (Wyewidencjuj).**
>
>Dzierżawa jest gotowa do weryfikacji i zezwalania na transakcje CSP.

### <a name="questions"></a>Masz pytania?

Skontaktuj się z doradcą podatkowym lub lokalnym urzędem podatkowym, jeśli masz pytania związane z identyfikatorem rejestracji firmy (nazywanym również INFORMACJAMI lub NIP). Firma Microsoft nie może zapewnić wskazówek dotyczących kwestii podatkowych.

Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych w firmie Microsoft, otwórz [żądanie obsługi](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Wyświetlanie ofert i uruchomień produktów w tym miesiącu

### <a name="categories"></a>Kategorie

- Data: 2021-04-01
- Możliwości
 
### <a name="summary"></a>Podsumowanie

Kalendarz uruchamiania produktów z kwietnia 2021 r. został opublikowany.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)

### <a name="details"></a>Szczegóły

Kalendarz uruchamiania produktów z [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) kwietnia 2021 r. jest teraz dostępny w galerii zasobów Gotowości do operacji. Zobacz nadchodzące wprowadzenie produktu i oferty tutaj.

### <a name="next-steps"></a>Następne kroki

Przejrzyj kalendarz [uruchamiania produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)i udostępnij informacje odpowiednim uczestnikom projektu w organizacji.  

### <a name="questions"></a>Masz pytania?

Jeśli masz dodatkowe pytania dotyczące tych ofert, sprawdź swoje Yammer społeczności.