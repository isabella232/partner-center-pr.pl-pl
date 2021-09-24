---
title: Ogłoszenia z września 2021 r.
description: Ogłoszenia dotyczące platformy Microsoft Partner Center z września 2021 r., w tym nowe możliwości, promocje, oferty, rynki lub zmiany istniejących ofert.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 09/20/2021
ms.openlocfilehash: 51706ec685519ea297e851cb4f2b862b96db3da1
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128373425"
---
# <a name="september-2021-announcements"></a>Ogłoszenia z września 2021 r.

Ta strona zawiera ogłoszenia dotyczące usługi Microsoft Partner Center na wrzesień 2021 r.

________________

## <a name="product-keys-available-for-business-central-for-dual-use-rights"></a><a name="13"></a> Klucze produktów dostępne dla usługi Business Central na potrzeby praw podwójnego użycia

### <a name="categories"></a>Kategorie

- Data: 2021-09-23
- Możliwości

### <a name="summary"></a>Podsumowanie

Od 23 września 2021 r. klucze produktów lokalnej wersji usługi Business Central na potrzeby praw podwójnego użycia będą dostępne dla klientów za pośrednictwem centrum administracyjne platformy Microsoft 365.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy CSP

### <a name="details"></a>Szczegóły

Od 23 września 2021 r. klucze produktów dla lokalnej wersji programu Business Central na potrzeby korzyści z praw podwójnego użycia nie będą już dostępne w Centrum biznesowym programu Partner Source (PSBC). Klienci mogą samodzielnie obsługiwać klucze produktów organizacji za pośrednictwem centrum administracyjne platformy Microsoft 365.

Proces zamawiania ani proces realizacji zmiany kodu kraju nie są zmieniane.

### <a name="next-steps"></a>Następne kroki

- Przejrzyj zasoby dotyczące tego tematu i udostępnij je odpowiednim uczestnikom projektu w organizacji.  
- Upewnij się, że Twoja organizacja i organizacje klientów znają tę zmianę.
- Jeśli nie wiesz, jak pobrać klucze produktów, zapoznaj się z tematem Pobieranie oprogramowania bezterminowego i [kluczy licencji produktów.](/microsoft-365/admin/setup/download-software-licenses-csp?view=o365-worldwide)
- Zapoznaj się ze zaktualizowanym procesem realizacji licencji na prawa do podwójnego użycia usługi Dynamics 365 Business Central w kolekcji zasobów usługi [Dynamics 365 Business Central z](https://partner.microsoft.com/resources/collection/dynamics-365-business-central-dual-use-rights-resources#/)prawami do podwójnego użycia.

### <a name="questions"></a>Masz pytania?

Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie Yammer społeczności.

________________

## <a name="reminder-introducing-api-throttling-to-partners-calling-partner-center-apis"></a><a name="12"></a>Przypomnienie: Wprowadzenie ograniczania interfejsu API partnerom wywołującym interfejsy API Partner Center API

### <a name="summary"></a>Podsumowanie

Od października 2021 r. firma Microsoft wdroży ograniczanie przepustowości interfejsów API dla partnerów wywołujących Partner Center API.

### <a name="categories"></a>Kategorie

- Data: 2021-09-21
- Możliwości

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy inicjujące transakcje za pośrednictwem Dostawca rozwiązań w chmurze programu  

### <a name="details"></a>Szczegóły

Od października 2021 r. firma Microsoft będzie implementować ograniczanie interfejsów API w celu zapewnienia bardziej spójnej wydajności w okresie dla partnerów wywołujących interfejsy API Partner Center API.Aby zapobiec nadużytości zasobów, ograniczanie ogranicza liczbę żądań do usługi w okresie.Po przekroczeniu progu ograniczania Partner Center ogranicza wszelkie dalsze żądania od tego klienta przez określony czas.
  
#### <a name="partner-benefits"></a>Korzyści dla partnerów

Chociaż Partner Center jest przeznaczona do obsługi dużej liczby żądań, w przypadku wystąpienia przytłaczającej liczby żądań ograniczanie przepływności pomaga zachować optymalną wydajność i niezawodność dla wszystkich partnerów.

Oto przykładowe korzyści:

- Ograniczanie zapewnia minimalny czas przestoju.
- Dzięki zmniejszeniu liczby żądań o dużej ilości danych możemy zapewnić spójną wydajność dla wszystkich partnerów.  

#### <a name="apis-to-be-throttled"></a>Interfejsy API do ograniczenia

| Operacja | Dokumentacja Centrum partnerskiego |
| ----------- | ---------------------- |
| Pobierz v1/customers/{customer_id}/users/{user_id}/licenses | [Pobieranie licencji przypisanych do użytkownika](/partner-center/develop/check-which-licenses-are-assigned-to-a-user) |
| Pobierz /v1/customers/{customer_id}/subscribedskus | [Pobieranie listy dostępnych licencji](/partner-center/develop/get-a-list-of-available-licenses) |
| Pobierz /v1/customers/{customer_id}/entitlements | [Pobieranie kolekcji uprawnień](/partner-center/develop/get-a-collection-of-entitlements) |
| Pobierz plik /v1/customers/{customer_id}/artifacts/{artifact_type}<br>/groups/{group_id}/lineItems/{lineitem_id}<br>/resource/{resource_id} | [Pobieranie kolekcji uprawnień](/partner-center/develop/get-a-collection-of-entitlements#retrieve-reservation-details-from-an-entitlement-by-using-sdk-v19) |
| Pobierz /v1/customers/{customer_id}/users/{use<br>r_id}/directoryroles | [Pobieranie ról użytkowników dla klienta](/partner-center/develop/get-user-roles-for-a-customer) |

Zalecamy rozważenie użycia interfejsu API dziennika aktywności w celu zwiększenia wydajności i uniknięcia ograniczania. Aby uzyskać więcej informacji na temat tej funkcji, zapoznaj się ze [szczegółami](/partner-center/develop/api-throttling-guidance)tutaj.  

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby [dotyczące](/partner-center/develop/api-throttling-guidance) tego tematu i podjąć niezbędne kroki.

### <a name="change-log"></a>Dziennik zmian

- 21 września: Przypomnienie o nadchodzących zmianach
- 19 lipca: oryginalne zawiadomienie

________________

## <a name="coming-soon-delegated-administrative-privileges-monitoring-and-self-service-removal"></a><a name="11"></a> Już wkrótce: Monitorowanie delegowanych uprawnień administracyjnych i usuwanie samoobsługi

### <a name="categories"></a>Kategorie

- Data: 2021-14-10
- Możliwości

### <a name="summary"></a>Podsumowanie

Firma Microsoft uruchamia nowe narzędzia do raportowania, które wyświetlają aktywne delegowane połączenia uprawnień administracyjnych (DAP), dzięki czemu partnerzy mogą wyłączyć nieużywane połączenia DAP.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy z rozliczeniami bezpośrednimi, dostawcy pośredni i odsprzedawcy pośredni, którzy Dostawca rozwiązań w chmurze programie

### <a name="details"></a>Szczegóły

Partnerzy mogą używać delegowanych uprawnień administracyjnych (DAP, delegated administrative privileges) do zarządzania usługami swoich klientów i ich obsługi.

Aby zwiększyć bezpieczeństwo w ekosystemie partnerów i klientów, firma Microsoft zaleca wyłączenie programu DAP, gdy nie jest on w użyciu.

Od końca października firma Microsoft będzie uruchamiać nowe narzędzia do raportowania, aby agenci administracyjni partnerów mogą inspekcję połączeń DAP ze swoimi klientami. To raportowanie będzie przechwytywać sposób uzyskiwania przez agentów partnerskich dostępu do dzierżaw klientów we wszystkich dzierżawach za pośrednictwem daP. Partnerzy mogą następnie przeglądać i usuwać połączenia DAP, które nie są w użyciu.

Aby dowiedzieć się więcej na temat tej [](https://partner.microsoft.com/resources/detail/dap-monitoring-and-self-serve-removal-pdf) nowej funkcji raportowania, utworzono przewodnik, który dokumentuje różne filtry i pola dostępne w raporcie.

#### <a name="key-considerations"></a>Najważniejsze zagadnienia

- Wyłączenie dostępu DAP dla klienta spowoduje wyłączenie uprawnień administratora partnera do zarządzania możliwościami w dzierżawie klienta.  
- Partnerzy transakcji mogą nadal składać zamówienia w imieniu swoich klientów.
- Agenci partnerscy nie mogą już zgłaszać biletu pomocy technicznej dla swoich klientów do firmy Microsoft.  
- Wyłączenie funkcji DAP nie będzie miało wpływu na bieżące role kontroli dostępu opartej na rolach w ramach subskrypcji i nie wpłynie na środki uzyskane przez partnerów.

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby [dotyczące tego](https://partner.microsoft.com/resources/collection/delegated-administrative-privileges-dap#/) tematu i udostępnij je odpowiednim uczestnikom projektu w organizacji.

## <a name="september-cloud-solution-provider-community-update-and-reminders"></a><a name="10"></a>Aktualizacja Dostawca rozwiązań w chmurze społeczności i przypomnienia

### <a name="categories"></a>Kategorie

- Data: 2021-9-10
- Community | Możliwości

### <a name="summary"></a>Podsumowanie

Biuletyn [Dostawca rozwiązań w chmurze (CSP)](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) jest teraz dostępny wraz z dodatkowymi zasobami społeczności programu [CSP,](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/) które zapewniają podstawowe aktualizacje programu.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy rozliczani bezpośrednio i dostawcy pośredni dostawcy CSP

### <a name="details"></a>Szczegóły

Zasoby z tego miesiąca obejmują następujące tematy:

#### <a name="launches"></a>Uruchamia

- [Usługa Microsoft Dynamics 365, Microsoft 365, Microsoft Power Platform i Windows 365 w nowym witrynie handlowej w programie CSP](https://partner.microsoft.com/resources/detail/d365-m365-power-platform-w365-in-the-new-commerce-experience-in-csp-pdf)

#### <a name="clinics"></a>Kliniki

- [Wprowadzenie do pomocy technicznej dotyczącej licencjonowania dla partnerów](https://partner.microsoft.com/resources/detail/introduction-to-licensing-support-for-partners-pdf)
- [Przewodnik po witrynie z warunkami produktu dla partnerów](https://partner.microsoft.com/resources/detail/product-terms-site-guide-for-partners-pdf)
- [Jak zgłosić wyłudzenie pomocy technicznej](https://partner.microsoft.com/resources/detail/how-to-report-a-support-scam-pdf)
- [Zmiana atrybutu programu dla Aplikacje Microsoft 365 dla Enterprise](https://partner.microsoft.com/resources/detail/program-attribute-change-for-microsoft-365-apps-for-enterprise-pdf)

#### <a name="csp-community-qa-reminder"></a>CSP Community Q&Przypomnienie

Miesięczna sesja Q&CSP (Q&A społeczności programu CSP) umożliwia dowiedzenie się więcej i zadawanie pytań dotyczących zmian wpływających na program. W tym miesiącu rozmowy skupią się na tematach wymienionych w poprzedniej sekcji i nie tylko.

[Zarejestruj się tutaj, aby dołączyć do wywołania](https://globalpbocomm.eventbuilder.com/GlobalCSP).

#### <a name="always-availablelaunch-content-on-demand"></a>Zawsze dostępna — uruchamianie zawartości na żądanie

W comiesięcznej [kolekcji społeczności CSP](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/)można znaleźć:

- Biuletyn comiesięcznej aktualizacji programu CSP do pobrania, który agreguje najnowsze ogłoszenia, aktualizacje, zdarzenia i przypomnienia dotyczące programu [CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) w czytelnym dokumencie.
- Kalendarz [anonsów dla programu CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-september-2021-pdf) który zawiera widok osi czasu przyszłych zmian wpływających na program.
- Nowy **kalendarz** [uruchamiania produktu,](https://partner.microsoft.com/resources/detail/product-launch-calendar-september-pdf) w którym można wyświetlić nadchodzące uruchomienia i oferty produktów.
- Przewodnik [globalna gotowość na promocje,](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/) który sortuje najnowsze i nadchodzące promocje, które są dostępne dla partnerów i klientów.
- [Program CSP uruchamia zasoby aktualizacji z](https://partner.microsoft.com/resources/collection/csp-launch-topics-collection#/) łatwą w użyciu zawartością dla kluczowych zmian operacyjnych.
- [Odświeżenia i przypomnienia dotyczące kluczowych](https://partner.microsoft.com/resources/detail/csp-september-2021-refreshers-and-reminders-pdf) tematów dotyczących CSP, które otrzymują zainteresowanie i zapytania.

Potrzebujesz gotowości do licencjonowania? [Comiesięczne seminaria internetowe dotyczące W](https://commercial_licensing.eventbuilder.com/YearToDate_ALL) centrum uwagi CSP obejmują najnowsze informacje o licencjonowaniu CSP dostępne dla wszystkich partnerów.

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby społeczności i zarejestruj się w celu&pytań i odpowiedzi.

### <a name="questions"></a>Masz pytania?

Miesięczna społeczność CSP&Q A call to najlepsze miejsce, aby zadać pytania dotyczące zmian operacyjnych w programie CSP. Możesz [przesłać pytanie do](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) 48 godzin przed wezwaniem. Odpowiedzi na wszystkie pytania związane z uruchamianiem zostaną udzielone w wywołaniu i/lub w dokumencie Q&A opublikowanym po wywołaniu. Możesz odwiedzić kolekcję [](https://partner.microsoft.com/resources/collection/august-2021-csp-partner-community-content#/) społeczności z ostatniego miesiąca i przejrzeć dokument Q&A, który został opublikowany po sierpniowym zdarzeniu.

Masz pytania dotyczące innych tematów dotyczących CSP? Odwiedź stronę [Partner Center pomocy technicznej.](https://partner.microsoft.com/support/?stage=1)

_____________

## <a name="september-co-sell-with-microsoft-qa-community-call-reminder"></a><a name="9"></a> Wrześniowa współpraca ze społecznością Microsoft Q&przypomnienie dotyczące rozmowy społecznościowej

### <a name="categories"></a>Kategorie

- Data: 2021-09-09
- Community | Zaproszenia i przypomnienia

### <a name="summary"></a>Podsumowanie

[Zarejestruj się teraz,](https://globalpbocomm.eventbuilder.com/GlobalCoSell) aby rozpocząć wrześniową sesję społeczności, w której wyróżnione są najnowsze uruchomienia i ulepszenia platformy handlowej oraz moduły poleceń w Partner Center.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Ta sesja jest dedykowana Partner Center ról użytkowników, którzy zarządzają:

- Moduł komercyjnej platformy handlowej do zarządzania publikowaniem ofert.
- Moduł poleceń do zarządzania potencjalnymi klientami i współdzielenie szans sprzedaży.

Wszyscy inni Partner Center mogą uzyskać dostęp do zawartości na żądanie w galerii zasobów [Operations Readiness.](https://partner.microsoft.com/resources/cloud-solution-provider-program)

### <a name="details"></a>Szczegóły

Najważniejsze artykuły w tym miesiącu obejmują:

#### <a name="commercial-marketplace"></a>Komercyjna platforma handlowa

- [Program wyszukiwania rozwiązań jest teraz zintegrowany z usługą AppSource](https://appsource.microsoft.com/blogs/now-live-on-microsoft-appsource-tap-into-the-unrivaled-microsoft-partner-ecosystem-to-accelerate-your-digital-transformation)
- [Wskazówki i uprawnienia wymagane do publikowania oferty na platformie handlowej (pliki do pobrania PowerPoint prezentacji)](https://assetsprod.microsoft.com/mpn/guidance-and-permissions-needed-to-publish-an-offer-and-co-sell-with-ms.pptm)

#### <a name="referral"></a>Skierowania

- [Konfigurowanie współpracy sprzedaży dla oferty platformy handlowej](/azure/marketplace/co-sell-configure)
- [Tworzenie reguł routingu dla szans przychodzących i zarządzanie nimi: Partner Center](../routing-rules.md)
- [Zarządzanie możliwościami współpracy sprzedaży: Partner Center](../manage-co-sell-opportunities.md#accepted-stage)
- [Dane rejestracji transakcji są teraz dostępne do eksportowania w poleceniu Szczegółowe informacje](./2021-july.md#17)

#### <a name="refresh"></a>Odśwież

- [Środowisko współpracy sprzedaży w Partner Center](/azure/marketplace/co-sell-configure#enter-your-contacts)
- [Zarządzanie poleceniami w Partner Center](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx)
- [Udostępnianie transakcji sprzedaży zbiorczej na dużą skalę przy użyciu Partner Center operacji zbiorczych](./2021-february.md#13)
- [Większa elastyczność dzięki transakcjom sprzedaży typu "co sell" prowadzonym przez partnerów](./2021-february.md#11)
- [Pobierz Szczegółowe informacje poleceń w Partner Center](../referral-insights.md)

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby [społeczności i](https://partner.microsoft.com/resources/collection/september-2021-co-sell-partner-community-content#/)zarejestruj się w celu&pytań i odpowiedzi.

### <a name="questions"></a>Masz pytania?

Zaproszenie społeczności&Q&jest najlepszym miejscem do zadawać pytania dotyczące zmian operacyjnych. Możesz [przesłać pytanie do](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) 48 godzin przed wezwaniem. Odpowiedzi na wszystkie pytania związane z uruchamianiem zostaną udzielone w wywołaniu i/lub w dokumencie Q&A opublikowanym po wywołaniu.  

Jeśli masz pytania dotyczące innych tematów, odwiedź stronę pomocy [Partner Center pomocy technicznej.](https://partner.microsoft.com/support/?stage=1)

_____________

## <a name="new-validation-rules-for-company-name-and-email-address-on-september-22"></a><a name="8"></a>Nowe reguły weryfikacji nazwy i adresu e-mail firmy 22 września

### <a name="categories"></a>Kategorie

- Data: 2021-09-07
- Gotowość

### <a name="summary"></a>Podsumowanie

Aby pomóc partnerom i klientom w prowadzenia działalności w oparciu o zaufanie, aktualizujemy reguły weryfikacji nazwy firmy i adresu e-mail klienta. Dotyczy to zarówno nowych, jak i istniejących szczegółów klienta. Nie są wymagane żadne zmiany interfejsu API.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy rozliczani bezpośrednio i dostawcy pośredni dostawcy CSP

### <a name="details"></a>Szczegóły

Firma Microsoft działa w oparciu o zaufanie. Dokładamy wszelkich starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę sprawdzania poprawności informacji o nazwie firmy i adresie e-mail klienta. Od 22 września 2021 r. będziemy aktualizować weryfikacje poczty e-mail i nazwy firmy. Aby uzyskać dodatkowe informacje, zobacz How to add a new customer record (Jak [dodać nowy rekord klienta).](../add-a-new-customer.md)

#### <a name="new-rules-for-company-name-and-email-address"></a>Nowe reguły dotyczące nazwy firmy i adresu e-mail

Od 22 września 2021 r. będą stosowane następujące nowe reguły weryfikacji.

Podczas wprowadzania nazwy firmy następujące elementy nie będą dozwolone:

- Przy użyciu tylko jednego znaku.
- Używanie tylko znaków specjalnych, takich jak &$^# (zobacz [tabelę](../add-a-new-customer.md#table-of-special-characters)).
- Używanie tylko spacji i/lub tabulatorów.
- Używanie skrótów autonomicznych z listy z ograniczeniami, takich jak LLC, Inc itp. (zobacz [tabelę](../add-a-new-customer.md#table-of-abbreviations)).
- Używanie nazw z rozszerzeniami domeny internetowej Top-Level (TDL), takich jak ".com", ".org", ".edu", ".club" itp. (zobacz [tabelę](../add-a-new-customer.md#table-of-top-level-domain-extensions)).
- Użycie tego samego znaku powtórzone trzy lub więcej razy bez innych znaków, takich jak 999.
- Używanie spacji i/lub tabulatorów mieszanych z poszczególnymi znakami, takimi jak 1 2 3.

Podczas wprowadzania adresu e-mail klienta następujące warunki nie będą dozwolone:
- Adres e-mail nie może zawierać adresu @microsoft.com .
- Adres e-mail klienta nie może zawierać tej samej nazwy domeny co partner. Na przykład partner o nazwie ABC nie może utworzyć wiadomości e-mail klienta za @abc.com pomocą .

Więcej szczegółowych informacji można znaleźć podczas seminarium internetowego na temat protokołu EAP:
- Pokładzie: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240](https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240)

- Nagrywania: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216](https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216)
 
#### <a name="partner-and-customer-impact"></a>Wpływ na partnerów i klientów

Partnerzy nie będą mogli tworzyć klientów, chyba że będą przestrzegać powyższych reguł od 22 września.

_____________

## <a name="readiness-dual-mode-attestation-and-additional-reseller-declaration"></a><a name="7"></a>Gotowość: zaświadczenia w trybie podwójnym i dodatkowa deklaracja odsprzedawcy

### <a name="summary"></a>Podsumowanie

Aby pomóc partnerom i klientom w prowadzenia działalności w oparciu o zaufanie, wymagamy od partnerów potwierdzania, że działają oni jako bezpośredni lub pośredni partnerzy, używając tego samego identyfikatora dzierżawy dla każdej transakcji.

Żądamy również od wszystkich partnerów transakcyjnych w krajach UNII/DSW zadeklarowania dodatkowych odsprzedawców (maksymalnie 5) zaangażowanych w transakcję.

### <a name="categories"></a>Kategorie

- Data: 2021-09-07
- Gotowość pilotażowa do startu rakiety w grudniu

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Dostawcy pośredni dostawcy CSP, którzy są partnerami bezpośrednimi i pośrednimi

Transakcje partnerów pośrednich w krajach UNII/DSW

### <a name="details"></a>Szczegóły

Firma Microsoft działa w oparciu o zaufanie. Dokładamy starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę transakcji subskrypcji klientów w programie CSP.

Od 7 września 2021 r. będziemy otwierać pilotaż dla partnerów, aby umożliwić partnerom testowanie pod względem nowych wymagań dotyczących zaswiadczania oraz dodatkowych odsprzedawców (tylko w Unii Europejskiej/KRAJACH) występujących w interfejsach API tworzenia koszyka, aktualizowania koszyka i tworzenia zamówienia. Należy pamiętać, że te zmiany przerwą istniejące środowisko dla tych interfejsów API. Dlatego zdecydowanie zaleca się, aby partnerzy mogli wziąć udział w pilotażu przed pełnym startem w grudniu.

#### <a name="partner-and-customer-impact"></a>Wpływ na partnerów i klientów

- ZMIANA NIEWAŻNA: Partnerzy pośredni nie będą mogli dopełnić zakupów bez uprzedniego poświadczania, że działają jako partnerzy bezpośredni lub pośredni
- Partnerzy z UE/DSM nie będą zgodne z przepisami UE, jeśli nie zadeklarują ani nie uwzględnią żadnych dodatkowych odsprzedawców, którzy są zaangażowani w transakcję
- Więcej szczegółowych informacji można znaleźć podczas seminarium internetowego na temat protokołu EAP: 
- Pokładzie: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240](https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240)
- Nagrywania: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216](https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216)

Będzie to miało wpływ na następujące interfejsy API, a szczegóły zostaną udostępnione i odpowiednio zaktualizowane:

- [Tworzenie zamówienia klienta — Partner Center deweloper aplikacji](/partner-center/develop/create-an-order)
- [Tworzenie koszyka — Partner Center deweloper aplikacji](/partner-center/develop/create-a-cart)
- [Aktualizowanie koszyka — Partner Center deweloper aplikacji](/partner-center/develop/update-a-cart)

Dodatkowi odsprzedawcy będą mieć wpływ na transakcje partnerów w następujących krajach UNII Europejskiej/DSM:

| Kraje UNII Europejskiej/Spoza Unii Europejskiej | &nbsp; | &nbsp; |
| --- | --- | --- |
| Andora<br>Austria<br>Belgia<br>Wyspa Bouveta<br>Bułgaria<br>Chorwacja<br>Cypr<br>Czechy<br>Dania<br>Estonia<br>Wyspy Owcze<br>Finlandia<br>Francja<br>Niemcy<br>Gibraltar | Grecja<br>Grenlandia<br>Guernsey<br>See (Obejmuje Miasto IoT)<br>Węgry<br>Islandia<br>Irlandia<br>Wyspa Man<br>Włochy<br>Jersey<br>Łotwa<br>Liechtenstein<br>Litwa<br>Luksemburg<br>Malta | Monako<br>Holandia<br>Norwegia<br>Polska<br>Portugalia<br>Rumunia<br>San Marino<br>Słowacja<br>Słowenia<br>Hiszpania<br>Svalbard i Jan Mayen<br>Szwecja<br>Szwajcaria<br>Zjednoczone Królestwo: TBD |
|

Aby wziąć udział w pilotażu, skontaktuj się z ekspertem w swojej dziedzinie (Ali Dostępki) i podaj identyfikator dzierżawy partnera, aby mógł zostać dodany do lotu.

_____________

## <a name="perpetual-software-and-software-subscriptions-price-lists-republished-to-fix-price-increases-in-russia"></a><a name="6"></a>Cenniki bezterminowych subskrypcji oprogramowania i oprogramowania zostały ponownie opublikowane w celu naprawienia wzrostu cen w Rosyjskim

### <a name="categories"></a>Kategorie

- Data: 2021-09-03
- Oferty/rynki

### <a name="summary"></a>Podsumowanie

Cennik oprogramowania bezterminowego i subskrypcji oprogramowania opublikowany 1 września 2021 r. został ponownie opublikowany 3 września w celu skorygowania problemu z cenami w Rosyjskim.

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Dostawcy pośredni i partnerzy rozliczający się bezpośrednio w ramach ciągłego oprogramowania i subskrypcji oprogramowania w ramach programu Dostawca rozwiązań w chmurze w Tym kraju.

### <a name="details"></a>Szczegóły

Cennik oprogramowania bezterminowego i subskrypcji oprogramowania opublikowany 1 września miał niepoprawny wzrost cen o 15,2% dla wszystkich produktów.

Wzrost ceny o ok. 15,2% rozpocznie się **1 października 2021 r.,** a nie we wrześniu. Cenniki zostały ponownie opublikowane z prawidłowymi informacjami o cenach.

Partnerzy, którzy kupili produkty od 1 września do 3 września, będą obciążani opłatami po poprawionych cenach, które są odzwierciedlone w najnowszych cennikach.

### <a name="next-steps"></a>Następne kroki

- Partnerzy, którzy transakcjują bezterminowe subskrypcje oprogramowania i oprogramowania w Rosyjskim, powinni pobrać najnowszy cennik, aby zobaczyć poprawione ceny.
- Aby uzyskać szczegółowe informacje na temat wzrostu cen w październiku, zobacz artykuł [Microsoft adjusts licensing program for commercial customers in Russia (Firma Microsoft](https://news.microsoft.com/ru-ru/licensing-changes-at-microsoft-russia-2021/)dostosowuje program licencjonowania dla klientów komercyjnych w Rosyjskim ).

_____________

## <a name="corrections-to-september-license-based-services-price-list-and-october-preview-for-microsoft-365-business-basic-usd"></a><a name="5"></a>Poprawki do cennika usług opartych na licencjach z września i październikowa wersja zapoznawcza Microsoft 365 Business Basic (USD)

### <a name="summary"></a>Podsumowanie

Cennik z września i październikowa wersja zapoznawcza zawierały niepoprawną cenę Microsoft 365 Business Basic w USD.

### <a name="categories"></a>Kategorie

- Data: 2021-09-02
- Oferty/rynki

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Dostawcy pośredni i partnerzy rozliczający się bezpośrednio w ramach programu licencjonowania Dostawca rozwiązań w chmurze usługami.

### <a name="details"></a>Szczegóły

Cennik wrześniowy i październikowa wersja zapoznawcza usług opartych na licencjach opublikowane 1 września 2021 r. miały niepoprawną cenę Microsoft 365 Business Basic. Poprawione cenniki zostały opublikowane 2 września 2021 r. Ma to wpływ tylko na USD.

Oferta, na która ma to wpływ, obejmuje:

- Nazwa oferty: Microsoft 365 Business Basic
- Identyfikator oferty: bd938f12-058f-4927-bba3-ae36b1d2501c
- Przed: Cennik = 2
- Po: Cena cenowa = 4

### <a name="next-steps"></a>Następne kroki

Partnerzy, którzy inwestują w licencjonowane usługi w USD, powinni pobrać najnowszy cennik, aby zobaczyć poprawioną cenę.

________________
## <a name="nigeria-and-thailand-are-now-microsoft-managed-countries"></a><a name="4-5"></a>Do krajów zarządzanych przez firmę Microsoft są teraz kraje, które są zarządzane przez firmę Microsoft

### <a name="categories"></a>Kategorie

- Data: 2021-09-01
- Możliwości

### <a name="summary"></a>Podsumowanie

Teraz są to kraje zarządzane przez firmę Microsoft.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy indyjscy i partnerzy.

### <a name="details"></a>Szczegóły

Zobacz [Szczegóły podatku dla wydawców komercyjnej platformy handlowej.](../tax-details-marketplace.md)

### <a name="questions"></a>Pytania

Aby uzyskać dalsze pytania dotyczące tych ofert, sprawdź odpowiednie Yammer społeczności.

________________
## <a name="announcing-intune-per-device-for-enterprise-for-csp-partners"></a><a name="4"></a>Announcing Intune per-device for Enterprise for CSP partners (Announcing Intune per-device for Enterprise for CSP partners

### <a name="categories"></a>Kategorie

- Data: 2021-09-02
- Możliwości

### <a name="summary"></a>Podsumowanie

Ogłaszamy nową ofertę usługi Intune dla każdego urządzenia, która będzie dostępna od 1 września.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy inicjujące transakcje w Dostawca rozwiązań w chmurze (CSP).

### <a name="details"></a>Szczegóły

Microsoft Intune to najbardziej kompleksowa, ujednolicona platforma do zarządzania punktami końcowymi, która umożliwia zarządzanie fizycznymi i wirtualnymi punktami końcowymi w organizacji oraz ich zabezpieczanie. Ogłaszamy nową ofertę usługi Intune dla każdego urządzenia, która ma ułatwić organizacjom Enterprise zarządzanie urządzeniami przypisanymi do uwierzytelnionego użytkownika (nie jest używana przez wielu uwierzytelnionych użytkowników).

Ta oferta, dostępna 1 września 2021 r., korzysta z usługi Intune na urządzenie podczas dodawania Azure Active Directory (Azure AD). Jest to w pełni funkcjonalne środowisko, które jest w pełni funkcjonalne i obejmuje następujące plany usług:

- Exchange Foundation
- Microsoft Intune
- Azure Active Directory for Education.

Na podstawie opinii naszych partnerów firmy Microsoft utworzono usługę Intune na urządzenie dla usługi Enterprise, która ma zostać uwzględniona w sprzedaży na urządzenie (urządzenia + Windows + Intune) jako ofertę 5-letnią, która będzie obejmować okres eksploatacji urządzenia. Ta nowa oferta pomoże CSP uprościć struktury transakcji i zaoferować klientom bardziej konkurencyjną umowę.

Elementy, które należy zwrócić uwagę na nową ofertę usługi Intune na urządzenie:

- Jest to oferta usługi SaaS Enterprise nie jest przeznaczona dla małych & średnich firm (SMB).
- Jest ona dostępna tylko dla CSP i nie jest dostępna w przypadku licencjonowania zbiorowego ani usługi Web Direct.
- Koszt wynosi 150 USD/ERP w przypadku subskrypcji 5-letniej.
- Identyfikator oferty: 5170ccfb-e95b-49a4-b7f3-31f631a356ba
- Będzie ona działać jako urządzenie w przypadku Windows przypisanych do jednego uwierzytelnionego użytkownika.
- Oferta nie obejmuje dostępu warunkowego opartego na urządzeniach.  

### <a name="questions"></a>Pytania

Aby uzyskać dalsze pytania dotyczące tych ofert, sprawdź odpowiednie Yammer społeczności.

_____________

## <a name="key-updates-for-the-new-commerce-experience-for-cloud-solution-provider-csp-seat-based-offers"></a><a name="3"></a>Najważniejsze aktualizacje nowego doświadczenia handlowego dla ofert opartych na Dostawca rozwiązań w chmurze (CSP)

### <a name="summary"></a>Podsumowanie

W związku z ujawnieniem z 19 sierpnia 2021 r. firma Microsoft ma kluczowe aktualizacje dotyczące nowego doświadczenia handlowego dla ofert opartych na stanowiskoch WSP.

### <a name="categories"></a>Kategorie

- Data: 2021-09-01
- Możliwości

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni oraz odsprzedawcy za pośrednictwem ich dostawców pośrednich

### <a name="details"></a>Szczegóły

19 sierpnia 2021 r. firma [Microsoft](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) ogłosiła nowe środowisko handlowe dla usług Microsoft 365, Dynamics 365, Power Platform i Windows 365, które będą oparte na ofertach dla klientów w październiku 2021 r. W związku z tym ogłoszeniem mamy następujące kluczowe aktualizacje, które pomogą Twojej organizacji przygotować się do tej transformacji:

- Uruchamianie ofert opartych na stanowiskoch na temat zintegrowanego testowania piaskownicy
- Przypomnienie dotyczące nadchodzących wywołań Q&CSP A we wrześniu
- Program Microsoft Commerce Incentive

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Uruchamianie ofert opartych na stanowiskoch w celu zintegrowanego testowania piaskownicy

Od 1 września 2021 r. firma Microsoft [](/partner-center/develop/test-and-debug) włączyła oparte [](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) na stanowisko oferty zintegrowanego testowania piaskownicy w nowym środowisku handlowym dla programu CSP.

Dodanie ofert Microsoft 365, Dynamics 365, Power Platform i Windows 365 w programie CSP do nowego doświadczenia handlowego jest kolejnym ważnym kamieniem milowym w naszej nowej podróży handlowej. Firma Microsoft inwestuje w innowacje produktów, lepsze narzędzia i dostęp do nowych możliwości biznesowych, które umożliwiają partnerom wzrost przychodów z programu CSP i zapewnienie klientom większej liczby opcji. Rozwijamy naszą platformę handlową i usprawniamy procesy zamawiania i zarządzania subskrypcjami, aby pomóc partnerom i klientom odnosić sukcesy dzięki transformacji cyfrowej.

Partnerzy, którzy uczestniczą w środowisku testowania piaskownicy, będą mieć wczesny wgląd w nowe środowisko handlowe dla ofert opartych na stanowiskoch, co umożliwia zaawansowane planowanie, operationalization i integrację techniczną tych ofert.

Uczestnictwo w środowisku piaskownicy umożliwia organizacji:

- Wykonywanie integracji interfejsu API w środowisku testowym przed wdrożeniem w środowisku produkcyjnym
- Mieć odpowiedni czas na zoperacyjność nowego doświadczenia handlowego przed jego uruchomieniem

Tabela zawiera podsumowanie najważniejszych funkcji dostępnych w zintegrowanym środowisku testowania piaskownicy:

| Konfigurowanie delegowanych uprawnień administratora partnera/klienta | Funkcja częściowego uaktualnienia podrzędnego i pełnego |
| ----------- | ---------------|
| Modele 1-warstwowe i 2-warstwowe | Częściowe uaktualnianie subskrypcji za pośrednictwem pomocy technicznej |
| Odnajdywanie obok siebie bieżącego i nowego typu | Zaplanowane zmiany podczas odnawiania  |
| Odnajdywanie i kupowanie nowoczesnego (wybierz produkty) | Wstrzymywanie/wznawianie (za pośrednictwem pomocy technicznej) |
| Zarządzanie subskrypcją (automatyczne odnawianie przełącznika, dodawanie stanowisk, anulowanie ruchu) | Bezpłatne wersje próbne (prezentowanie tylko dla komputerów MAC) |
| Niezależne dodatki  | Waluta partnera |
| Plany rozliczeniowe | Przezroczystość cen  |
| Zarządzanie cyklem życia subskrypcji (okres prolongaty) | Roczne plany rozliczeniowe dla ofert wielorocznych  |
| Ograniczenia własności | Wstrzymywanie/wznawianie (za pośrednictwem samoobsługi)  |
| Pliki faktury/rekonesfiguru | Ponowne przypisanie automatycznego stanowiska dla przejść do pełnej ilości SKU |
| Uaktualnienia średniej pełnej ilości SKU | Bezpłatna wersja próbna (z pełnym prezentem) |
| Wymuszanie zasad anulowania: anulowanie 30-dniowego bloku po 30 dniach (zostanie on zmieni się po ogólnej dostępności na 72 godziny) |  |
|

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Przypomnienie dotyczące nadchodzących wywołań Q&CSP A we wrześniu

Zarejestruj się, aby 15 września i 16 września 2016 r. zadawać pytania dotyczące nowego doświadczenia handlowego dla usług Microsoft 365, Dynamics 365, Power Platform i Windows 365, aby poznać nowe środowisko handlowe dla usług Microsoft 365 [Community,](https://globalpbocomm.eventbuilder.com/GlobalCSP) Dynamics 365, Power Platform i Windows 365.& Wywołania CSP Community Q&A mają na celu pomoc partnerom bezpośrednim i partnerom WSP w pytaniach dotyczących startów programu CSP i nadchodzących zmian. Dla Twojej wygody kolekcje społeczności są udostępniane [](https://partner.microsoft.com/resources/assets/#/?prog=CSP%7CCSP-Direct%7CCSP-Indirect-Partner&type=collection&search=community%20collection%202021&sort=updated) z wyprzedzeniem w galerii gotowości partnerów, gdzie możesz przejrzeć materiały, które zostaną omówione w wywołaniu Q&A.

Jeśli chcesz wziąć udział i/lub znaleźć wcześniejsze nagrania rozmów z podstawami CSP, zapoznaj się z rejestracją w portalu [CSP fundamentals (Podstawy CSP).](https://globalpbocomm.eventbuilder.com/CSPFundamentals)

#### <a name="microsoft-commerce-incentive-program"></a>Program Microsoft Commerce Incentive

1 września 2021 r. firma Microsoft powiadomiła partnerów o kolejnych krokach ewolucji programu zachęt dla partnerów, który będzie dostępny w październiku. Dwoma podstawowymi składnikami tej komunikacji będą przewodniki dotyczące zachęt FY22 oraz informacje na temat ulepszonego doświadczenia w zakresie zachęt opracowywanego w ramach Partner Center.

- **Ulepszone środowisko partnerów**  Na początku października firma Microsoft inwestuje w jedną platformę zaangażowania i działań w ramach usługi Partner Center, która będzie scentralizowanym miejscem docelowym dla partnerów, którzy będą zdobywać zachęty w ramach zakupów i etapów cyklu życia klienta.

- **Nowe podejście do zachęt**  Nowe oferty zachęt i inwestycji będą nadal dodawane do Microsoft Commerce Incentives programie. W celu uproszczenia obsługi partnerów firma Microsoft skonsolidowa przewodniki programu zachęt w jeden dokument hostowany w Partner Center.

### <a name="next-steps"></a>Następne kroki

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Uruchamianie ofert opartych na stanowiskoch w celu zintegrowanego testowania piaskownicy

- Jeśli Organizacja aprowizowała zintegrowane środowisko piaskownicy, nie jest wymagana żadna akcja. Jeśli Twoja organizacja nie ma zintegrowanego środowiska piaskownicy, wykonaj następujące [kroki,](/partner-center/develop/indirect-provider-sandbox-capabilities) aby je utworzyć.
- Zapoznaj się z przewodnikiem operacyjnym programu [CSP](https://partner.microsoft.com/resources/detail/operating-guide-new-commerce-experience-for-csp-seat-based-offers-pdf) dla usług Microsoft 365, Dynamics 365, Power Platform i Windows 365 w nowym miejscu handlu, aby dowiedzieć się więcej o funkcjach, zasadach biznesowych i instrukcjach krok po kroku dotyczących tej wersji. Regularnie sprawdzaj przewodnik obsługi, ponieważ będzie okresowo aktualizowany.
- Zapoznaj się z zasobami opisanymi na [mapie gotowości.](https://partner.microsoft.com/resources/detail/readiness-map-new-commerce-experienceseat-based-offers-pdf)
- Przejrzyj folder [dokumentacji interfejsu API](https://partner.microsoft.com/resources/collection/api-documentation#/).
- Aby uzyskać pomoc techniczną, należy rejestrować bilet pomocy technicznej lub publikować wiadomości w konwersacjach w grupie usługi zestaw SDK Centrum partnerskiego i api [Yammer,](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=6589502)gdzie prezentacje i nagrania funkcji będą publikowane w ciągu września.

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Przypomnienie dotyczące nadchodzących wywołań CSP Q&A we wrześniu

- Zarejestruj się, aby 15 lub 16 września [2016 r&A Community CSP Q.](https://globalpbocomm.eventbuilder.com/GlobalCSP)
- Przejrzyj nowe środowisko handlowe dla kolekcji ofert opartych na stanowiskoch CSP [dla](https://partner.microsoft.com/resources/collection/new-commerce-experience-for-csp-seat-based-offers#/) tego uruchomienia.
- Weź udział w CSP Q&A Community Call i zadawaj pytania dotyczące nowego doświadczenia handlowego dla usług Microsoft 365, Dynamics 365, Power Platform i Windows 365 na podstawie miejsca na szerokość.

#### <a name="microsoft-commerce-incentive-program"></a>Program Microsoft Commerce Incentive

- Przejrzyj komunikację w nadchodzącym rozszerzonym doświadczeniu partnerów w [kolekcji Microsoft Commerce Incentives zasobów.](https://partner.microsoft.com/asset/collection/microsoft-commerce-incentive-resources#/)
- Przejrzyj zaktualizowane przewodniki zachęt dla partnerów FY22 w [portalu Zachęty dla partnerów.](https://microsoft.sharepoint.com/teams/PartnerIncentivesPortal)

### <a name="questions"></a>Masz pytania?

Jeśli masz dodatkowe pytania dotyczące tych ofert, sprawdź swoje Yammer społeczności.

_____________

## <a name="view-this-months-product-launches-and-offers"></a><a name="2"></a>Wyświetlanie ofert i uruchomień produktów w tym miesiącu

### <a name="summary"></a>Podsumowanie

Kalendarz uruchamiania produktów z września 2021 r. został opublikowany.

### <a name="categories"></a>Kategorie

- Data: 2021-09-01
- Rozwój firmy

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)

### <a name="details"></a>Szczegóły

Kalendarz uruchamiania produktów z [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) września 2021 r. jest teraz dostępny w galerii zasobów Gotowości na operacje. Zobacz nadchodzące wprowadzenie produktu i oferty tutaj.

### <a name="next-steps"></a>Następne kroki

Przejrzyj kalendarz [uruchamiania produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)i udostępnij informacje odpowiednim uczestnikom projektu w organizacji.  

### <a name="questions"></a>Masz pytania?

Jeśli masz dodatkowe pytania dotyczące tych ofert, sprawdź swoje Yammer społeczności.

_____________

## <a name="software-in-microsoft-china-cloud-solution-provider-program-mccl-csp-to-start-transactions-from-august-12"></a><a name="1"></a>Software in Microsoft China Dostawca rozwiązań w chmurze Program (MCCL CSP) to start transactions from August 12 (Oprogramowanie w Chinach firmy Microsoft do uruchamiania transakcji od 12 sierpnia)

### <a name="summary"></a>Podsumowanie

W ramach aktualizacji z 3 sierpnia oprogramowanie w programie MCCL CSP rozpocznie transakcje od 12 sierpnia 2021 r.

### <a name="categories"></a>Kategorie

- Data: 2021-09-01
- Rozwój firmy

### <a name="impacted-audience"></a>Odbiorcy, na które ma to wpływ

Partnerzy programu MCCL CSP

### <a name="details"></a>Szczegóły

#### <a name="mccl-csp-transaction-start"></a>Uruchomienie transakcji MCCL CSP

- 12 sierpnia 2021 r. firma MCCL CSP rozpocznie transakcje dla klientów w Chinach.

- Klienci mogą nadal kupować licencje na oprogramowanie za pomocą partnera w programie Licencjonowanie otwarte do 31 grudnia 2021 r. Licencje bezterminowe będą dostępne zarówno w programie MCCL CSP, jak i w programach licencjonowania Open do czasu jego końca.

#### <a name="open-license-program-deprecation"></a>Cofanie pracy z programem Licencjonowanie Open

- Od 1 stycznia 2022 r. klienci nie mogą już kupować ani odnawiać licencji na oprogramowanie za pośrednictwem programu Microsoft Open License.

- Klienci mogą nadal mieć pełne prawa i dostęp do wszystkich bezterminowych licencji na oprogramowanie nabytych w ramach programu Licencjonowanie Open nawet po jego zakończeniu. Nadal mogą również uzyskać dostęp do Centrum usługi licencjonowania zbiorowego, aby zarządzać tymi licencjami i usługami.

#### <a name="software-assurance-sa-purchases"></a>pakiet Software Assurance (SA)

- Oferty skojarów zabezpieczeń z licencją Open License (L&SA) pozostaną nadal dostępne w ramach subskrypcji Open Value (OV) i Open Value Subscription (OVS). Jednak ani SA, ani L&SA nie są dostępne w programie CSP MCCL, ponieważ nie ma planu zaoferowania tego w programie MCCL CSP.

- Korzyści z skojaśnień zabezpieczeń będą kontynuowane do momentu wygaśnięcia okresu skoja stycznia 2022 r., nawet jeśli wygaśnięcie wygaśnie po 1 stycznia 2022 r.

- Program OV firmy Microsoft jest zalecany w przypadku przyszłych zakupów, które obejmują sa sa.

>[!NOTE]
>Nie ma planów zmiany programów OV i OVS.

#### <a name="partner-change-management"></a>Zarządzanie zmianami partnerów

- Istniejący dystrybutorzy programu Microsoft Open są dołączani jako dostawcy pośredni DOSTAWCY CSP firmy MCCL.

- Dostawcy pośredni i wybrani odsprzedawcy pośredni zostaną zaproszeni do przeprowadzenia testów środowiska produkcyjnego w sierpniu w celu zapewnienia funkcji transakcji.

- Warsztaty dotyczące gotowości dla partnerów pośrednich rozpocząły się w lipcu i będą kontynuowane do grudnia 2021 r.

### <a name="next-steps"></a>Następne kroki

Przygotuj się na tę zmianę za pomocą następujących zasobów:

- [Co to jest nowy handel?](https://partner.microsoft.com/resources/detail/new-commerce-experience-introduction)
- [Podręcznik dostawcy pośredniego dostawcy CSP MCCL](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EeWi5axiZ_RCkTbxa-brE-sBGYdLJ5idpnZvFt2MFiTLWw?e=6itfqY)
- [Podręcznik odsprzedawcy pośredniego w programie MCCL CSP](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EY-csVS7lFdKpwkRqeJJ4hkBPGWv4qkfINictqVrwKVLxQ?e=9G6ZY1)

Należy pamiętać, że te zmiany dotyczą tylko programu MCCL CSP i nie mają wpływu na 21 vianet CSP.

### <a name="questions"></a>Masz pytania?

Jeśli masz jakieś dodatkowe pytania, porozmawiaj z menedżerem ds. rozwoju partnera lokalnego.
