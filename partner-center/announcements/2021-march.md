---
title: Ogłoszenia z marca 2021 r.
description: Ogłoszenia dotyczące platformy Microsoft Partner Center z marca 2021 r., w tym nowe możliwości, promocje, oferty, rynki lub zmiany istniejących ofert.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328070"
---
# <a name="march-2021-announcements"></a>Ogłoszenia z marca 2021 r.

Ta strona zawiera ogłoszenia dotyczące platformy Microsoft Partner Center na marzec 2021 r.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Gotowość: zmiany interfejsu API weryfikacji adresu Dostawca rozwiązań w chmurze (CSP) zostaną wprowadzone w czerwcu; Funkcja testowania jest teraz dostępna

### <a name="categories"></a>Kategorie

- Data: 2021-04-30
- Gotowość

### <a name="summary"></a>Podsumowanie

Aby pomóc partnerom i klientom w prowadzenia działalności w oparciu o zaufanie, będziemy zapraszać partnerów do testowania zmian w interfejsie API weryfikowania adresów dla wszystkich krajów na całym świecie.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy tworzą nowych lub aktualizują istniejących klientów, rozsyłają szczegółowe informacje.

### <a name="details"></a>Szczegóły

Firma Microsoft działa w oparciu o zaufanie. Dokładamy starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji adresu klienta na potrzeby transakcji subskrypcji klientów w programie CSP. Od 31 marca 2021 r. wprowadziliśmy zmiany w interfejsie API weryfikowania adresu, które zaprosiliśmy partnerów do testowania przed wprowadzeniem zmian w czerwcu 2021 r.

Zmiany mają wpływ tylko na interfejs API weryfikacji adresu. Nie ma to wpływu na interfejsy API tworzenia klienta i aktualizowania profilu rozliczeniowego.

Odpowiedź zwróci jeden z następujących komunikatów o stanie:

| Stan     | Opis |    Liczba zwróconych sugerowanych adresów |
|-------|---------------|-------------------|
|Zweryfikowana wysyłka | Adres jest weryfikowany i można go wysłać. | Pojedynczy |
|Sprawdzonych | Adres jest weryfikowany. | Pojedynczy |
|Wymagana interakcja | Sugerowany adres został znacząco zmieniony i wymaga potwierdzenia przez użytkownika. | Pojedynczy |
|Część częściowa ulicy | Podana ulica w adresie jest częściowa i wymaga więcej informacji. | Wiele — maksymalnie trzy |
|Część lokalna | Dane lokalne (numer budynku, numer pakietu i inne) są częściowe i wymagają więcej informacji. | Wiele — maksymalnie trzy |
|Wiele | Istnieje wiele pól, które są częściowo w adresie (potencjalnie również częściowe ulice i część lokalna). | Wiele — maksymalnie trzy |
|Brak | Adres jest niepoprawny. | Brak |
|Nie sprawdzono | Nie można wysłać adresu w procesie walidacji. | Brak |

Kody pocztowe w USA zwracają dodatkowe 4 cyfry i łącznik — na przykład 12345-6789.

Po przesłaniu adresu do weryfikacji za pośrednictwem interfejsu API weryfikacji adresu zostanie zwrócony następujący schemat odpowiedzi:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Przyjrzyj się tej przykładowej odpowiedzi. Pamiętaj, że w przypadku Stanów Zjednoczonych odpowiedź zwróci dodatkowy czterocyfrowy sufiks dla wiersza kodu pocztowego, jeśli wprowadzasz tylko pięć cyfr dla kodu pocztowego.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Następne kroki

- Udostępnij swój identyfikator dzierżawy piaskownicy ekspertowi w tej dziedzinie (Ali Ichki), który zostanie uwzględniony w teście testowym, aby rozpocząć przygotowywanie do aktualizacji.

- Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.

### <a name="questions"></a>Masz pytania?

Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych przez firmę Microsoft, swiązyj się z grupą usługi Yammer pomocy technicznej partnera.

### <a name="change-log"></a>Dziennik zmian:

- 31 marca 2020 r.: oryginalna publikacja

- 30 kwietnia 2021 r.: aktualizacje przykładowej odpowiedzi i szczegółów kodu pocztowego

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Nowe środowisko centrum administracyjnego programu Exchange (EAC)

### <a name="categories"></a>Kategorie

- Data: 2021-03-29
- Możliwości

### <a name="summary"></a>Podsumowanie

Od 27 kwietnia 2021 r. w centrum administracyjnym programu Exchange (EAC) zostanie wdane nowe środowisko, które poprawi wydajność pracy użytkowników.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Administratorzy delegowani uzyskiwania dostępu do programu Exchange za pośrednictwem Partner Center

### <a name="details"></a>Szczegóły

Od 27 kwietnia 2021 r. partnerzy, którzy przejdą do programu Exchange za pośrednictwem programu Partner Center, zostaną przekierowani do nowego konta EAC.

To nowe środowisko jest obecnie dostępne w wersji zapoznawczej, a administratorzy mogą aktywować to środowisko, wybierając przełącznik w prawym górnym rogu klasycznej funkcji EAC. Mogą również przejść do nowej EAC, wybierając baner "Wypróbuj teraz", który jest wyświetlany na wszystkich stronach.

Nowe funkcje EAC mają następujące zalety:

- Dodano szczegółowe informacje, raporty i mechanizmy alertów dotyczące problemów związanych z przepływem poczty e-mail. 

- Spersonalizowane pulpity nawigacyjne zwiększające produktywność.

Aby ułatwić nawigowanie po nowym środowisko, filmy wideo są dostępne w sekcji **Training & Guide** (Przewodnik szkoleniowy) dotyczącej nowego doświadczenia EAC. Te informacje zapewniają przegląd sposobu najlepszego korzystania z nowego portalu.

>[!NOTE]
>Dzięki tej zmianie klasyczne środowisko funkcji EAC nie będzie przestarzałe. Przed zaimplementowaniem każdej zmiany użytkownik zostanie o tym powiadomiony z dużym wyprzedzeniem.

### <a name="next-steps"></a>Następne kroki

- Zapoznaj się z [zasobami na ten temat,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)gdzie możesz wyświetlać zrzuty ekranu nowego doświadczenia.

- Udostępnij te informacje odpowiednim uczestnikom projektu w organizacji. 

### <a name="questions"></a>Masz pytania?

Jeśli masz pytania dotyczące tych zmian, sprawdź odpowiednie społeczności usługi Yammer.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: Introducing the product launch calendar (Operacje firmy Microsoft: wprowadzenie do kalendarza uruchamiania produktu)

### <a name="categories"></a>Kategorie

- Data: 2021-03-25
- Oferty | Nowoczesne miejsce pracy

### <a name="summary"></a>Podsumowanie

W odpowiedzi na opinie partnerów operacje firmy Microsoft usprawniają komunikację podczas uruchamiania produktów.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Dostawca rozwiązań w chmurze partnerów (CSP)

### <a name="details"></a>Szczegóły

Firma Microsoft dokłada starań, aby stale ulepszać środowisko partnerów. Otrzymaliśmy opinię, że otrzymujesz zbyt wiele komunikatów od firmy Microsoft, w tym zduplikowane ogłoszenia dotyczące startów produktów.

W odpowiedzi na Twoją opinię firma Microsoft usprawniła środowisko gotowości do wprowadzenia nowych i istniejących ofert produktów.

Teraz zapewniamy pojedynczy miesięczny widok uruchomień produktów opublikowany w galerii zasobów gotowości operacji. Ten [comiesięczny widok](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) kalendarza uruchamiania produktu zastąpi komunikację o uruchomieniu poszczególnych produktów w galerii zasobów Gotowości na operacje i w Partner Center o ogłoszeniach.

Możesz również uzyskać dostęp do kalendarza [uruchamiania tego produktu z](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) kolekcji [społeczności,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)widoków [kalendarza](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)i [biuletynów CSP.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) Powiadomimy Cię, gdy opublikujemy kalendarz uruchamiania produktów z każdego miesiąca z ogłoszeniem w galerii zasobów Gotowości na operacje.

Informacje dotyczące nowych i istniejących ofert można nadal znaleźć w dziennikach podglądu cennika i zmian cennika, a także w blogach dotyczących produktów, przewodnikach licencjonowania i stronach marketingowych produktów.

Zmiana będzie dotyczyć startów następujących produktów:

- Lokalna usługa Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Serwer  
- Narzędzia
- Teams i Telco

Będziemy nadal wysyłać konkretne ogłoszenia dotyczące startów produktów, które wymagają szczegółów gotowości operacji.

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.

### <a name="questions"></a>Masz pytania?

Jeśli masz dodatkowe pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Zmiany wymagań dotyczących dołączania klientów do CSP

### <a name="categories"></a>Kategorie

- Data: 2021-03-25
- Możliwości

### <a name="summary"></a>Podsumowanie

W ramach naszego zobowiązania do pomocy partnerom i klientom w zakresie prowadzenia działalności w oparciu o zaufanie poprosimy o dodatkowe informacje o klientach od 25 marca 2021 r.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Dostawca rozwiązań w chmurze (CSP) i dostawcy pośredni, którzy mają nowych lub istniejących klientów w krajach wymienionych w następnej sekcji

### <a name="details"></a>Szczegóły

Firma Microsoft działa w oparciu o zaufanie. Dokładamy starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji klientów na potrzeby transakcji subskrypcji klientów w programie CSP. 25 marca 2021 r. wprowadzimy ulepszenia interfejsu API i interfejsu użytkownika usługi Partner Center, które będą mieć wpływ na partnerów spełniających oba następujące kryteria:

1. Partner ma bezpośrednią relację rozliczeń z firmą Microsoft (co oznacza, że partner jest partnerem z rozliczaniem bezpośrednim lub dostawcą pośrednim).

2. Partner współpracuje z nowymi lub istniejącymi klientami w następujących krajach:

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

Partnerzy spełniający kryteria będą mieli możliwość przesyłania identyfikatora rejestracji firmy **klienta** (znanego także  jako organizacja klienta **), oraz** numeru telefonu podczas dołączania nowych klientów lub modyfikowania istniejących danych klienta. Ci partnerzy mogą również wprowadzić opcjonalne **drugie imię** klienta.

Pamiętaj, że podczas dodawania identyfikatora rejestracji firmy należy użyć identyfikatora podatku od działalności biznesowej, a nie identyfikatora osobistego klienta.

Partnerzy, którzy firma współpracuje z nowymi lub istniejącymi klientami w następujących krajach, są już do dołączani w poprzedniej wersji w listopadzie 2020 r.

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

Partnerzy z klientami na całym świecie będą mieć możliwość wprowadzania identyfikatora rejestracji **firmy,** numeru telefonu i środkowego  imienia i nazwiska klientów w dniu 25 marca 2021 r. jako opcjonalnych szczegółów.

### <a name="next-steps"></a>Następne kroki

- Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.

- Przygotuj się do uwzględnienia zmian przy użyciu Partner Center API i internetowego interfejsu użytkownika. Zestawy API/zestawy SDK będą dostępne do testowania.

- Pamiętaj, aby przesłać dodatkowe dane podczas dołączania nowych klientów lub modyfikowania istniejących danych klienta.

- Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.

### <a name="questions"></a>Masz pytania?

Skontaktuj się z doradcą podatkowym lub lokalnym urzędem podatkowym, jeśli masz pytania związane z identyfikatorem prawna (nazywanym również URZĘDEM podatkowym lub NIP). Firma Microsoft nie może zapewnić wskazówek dotyczących kwestii podatkowych.

Jeśli potrzebujesz pomocy technicznej w operacjach wykonywanych w firmie Microsoft, [otwórz żądanie obsługi](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Korekty wprowadzone do 1 marca 2021 r. bezterminowy cennik oprogramowania

### <a name="categories"></a>Kategorie

- Data: 2021-03-23
- Oferty/rynki

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Dostawcy pośredni i bezpośredni partnerzy rozliczający się bezterminowo w ramach programu Dostawca rozwiązań w chmurze oprogramowania 

### <a name="details"></a>Szczegóły

Cennik oprogramowania bezterminowego opublikowany 1 marca 2021 r. obejmował rynki, które nie powinny tam być. Cennik oprogramowania bezterminowego został zaktualizowany 17 marca 2021 r. o korekty. Te poprawki miały zastosowanie tylko do:

- Identyfikator produktu: DF77X4D43RKT 
- Nazwa produktu: Windows 10 Home do wersji Pro Upgrade for Microsoft 365 Business
- Usunięte lub nieobsługiwane rynki: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, LM, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Te zmiany dotyczą tylko powyższego produktu. Inne produkty nie miały poprawek. 

### <a name="next-steps-and-resources"></a>Następne kroki i zasoby

- Partnerzy, którzy transakcjiują oprogramowanie bezterminowe, powinni pobrać najnowszy cennik oprogramowania bezterminowego.
- Zapoznaj się z [kodami krajów regionów,](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) aby uzyskać przyjazne mapowanie dwuliterowego skrótu na kraje.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> Wersja zestawu SDK w .NET Standard (wersja 1.17.0)

### <a name="categories"></a>Kategorie

- Data: 2021-03-23

- Możliwości
 
### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy z rozliczeniami bezpośrednimi i dostawcy pośredni uczestniczący w programie CSP, którzy Partner Center zestawu SDK platformy .NET.

### <a name="details"></a>Szczegóły

Od 23 marca 2020 r. partnerzy mogą rozpocząć pobieranie wersji pakietu [MicrosoftPartnerCenter.NETSDK (galerii NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)wraz ze zaktualizowanymi publicznymi zestaw SDK Centrum partnerskiego [przykładami usługi GitHub.](https://github.com/Microsoft/Partner-Center-DotNet-Samples) Ta wersja zawiera aktualizacje następujących metod:

#### <a name="audit-updated-new-operation-types"></a>Aktualizacja inspekcji: nowe typy operacji

Dodano [nowe typy operacji,](https://docs.microsoft.com/partner-center/develop/auditing-resources) aby wiedzieć, kiedy klient zatwierdził i zakończył działanie daP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Aktualizacja inspekcji: nowe typy zasobów i operacji

Dodano [nowe typy zasobów i operacji](https://docs.microsoft.com/partner-center/develop/auditing-resources) na potrzeby obsługi scenariusza roli katalogu klienta.

- Nowy typ zasobu "CustomerDirectoryRole"

- Typy operacji "AddUserMember" i "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>Aktualizacje zestawu SDK dla kont klientów

- Obsługa get /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Dodatkowe zmiany

Następujące zmiany są wprowadzane w ramach nowego handlu i są obecnie dostępne na zaproszenie tylko dla partnerów, którzy są częścią nowego doświadczenia handlowego M365/D365 w wersji Technical Preview. Partnerzy, którzy nie są częścią wersji New Commerce Technical Preview, nie powinni zauważyć wpływu i powinni być zgodni z poprzednimi wersjami.

- Zmiany katalogu:

  - GET /products/{product-id}/skus/{sku-id}

- Zakup i zarządzanie:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Następne kroki

- Pobierz najnowszą wersję [microsoftPartnerCenter.NETSDK (Galeria NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Pobieranie i przeglądanie [przykładów usługi GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Oferta komercyjnej platformy handlowej programu CSP i zachęty FY21 CSP dla kwalifikujących się ofert

### <a name="categories"></a>Kategorie

- Data: 2021-03-18
- Możliwości

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Dostawcy pośredni i bezpośredni partnerzy rozliczani w Dostawca rozwiązań w chmurze programie 

### <a name="details"></a>Szczegóły

Dostawcy pośredni i bezpośredni partnerzy rozliczający w programie Dostawca rozwiązań w chmurze mogą sprzedawać oferty innych firm i uzyskać zachętę motywacyjną dla każdej kwalifikującej się oferty innej firmy Partner Center lub Azure Portal. Zachęta będzie mieć formę rachunku za rozliczaną sprzedaż dla kwalifikujących się ofert i będzie dostępna do 30 czerwca **2021 r.**.  

Kontynuuj dalsze informacje na temat tej zachęty oferty komercyjnej platformy handlowej CSP poniżej i skontaktuj się z klientami już dzisiaj, aby zidentyfikować odpowiednie oferty, aby umożliwić ich dalszy sukces i transformację cyfrową.

Współpracujemy z niezależnymi dostawcami oprogramowania (ISV), aby wprowadzić na rynek najnowsze rozwiązania IaaS i SaaS dla klientów firmy Microsoft. Wydawcy isV mają możliwość włączenia sprzedaży swoich ofert za pośrednictwem kanału partnerskiego firmy Microsoft. Nasze oferty kwalifikujące się do zachęt można podzielone na dwie kategorie:

- Wybierz oferty SaaS i IaaS innych firm ze stanem zniechęceń do współscenizacji adresu IP platformy Azure. 

- Aplikacje SaaS zintegrowane z usługą Teams lub co najmniej dwie Microsoft 365 aplikacji zwiększających produktywność, takich jak PowerPoint, Word, Excel, Outlook lub SharePoint.

### <a name="next-steps-and-resources"></a>Następne kroki i zasoby

- Dowiedz się więcej o zarobkach [w programie Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps (Zachęty dla partnerów do sprzedaży kwalifikujących się aplikacji na platformie handlowej). Nowe oferty są dodawane co miesiąc.  
- [Dostawca rozwiązań w chmurze zasobów zachęt dla partnerów rozliczanych bezpośrednio](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Dostawca rozwiązań w chmurze zasobów zachęt dostawcy pośredniego](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Przejrzyj tę [prezentację,](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) aby dowiedzieć się więcej o sprzedaży aplikacji platformy handlowej. Zapoznaj się z dodatkowymi zasobami [tutaj.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) 
- Eksplorowanie katalogu komercyjnej platformy [handlowej w Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) lub [Azure Portal](https://ms.portal.azure.com/#home)
- Integrowanie [aplikacji z](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) firmową platformą handlowa przy użyciu interfejsów API
- Docieranie do isvs you interested in doing business with
- Dostawcy pośredni muszą integrować się przy użyciu interfejsów API i kierować odsprzedawcami aplikacji do sprzedaży

### <a name="questions"></a>Masz pytania?  

Zapoznaj się [z tym artykułem,](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) aby zapoznać się z omówieniem platformy handlowej w Partner Center.

Jeśli potrzebujesz dodatkowej pomocy, możesz utworzyć wniosek o pomoc techniczną w Partner Center. Dowiedz się więcej na stronie [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium oferty nazewnictwa i aktualizacji wymagań wstępnych

### <a name="categories"></a>Kategorie

- Data: 2021-03-18
- Możliwości

### <a name="summary"></a>Podsumowanie

Ostateczny cennik z 1 kwietnia 2021 r. zostanie zaktualizowany w celu zwiększenia przejrzystości nazw i/lub informacji o wymaganiach wstępnych dotyczących Power BI Premium ofert dla 1 użytkownika.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Dostawca rozwiązań w chmurze (CSP) partnerów bezpośrednich i pośrednich

### <a name="details"></a>Szczegóły

Ostateczny cennik z 1 kwietnia 2021 r. zostanie zaktualizowany, aby dodać przejrzystość do nazewnictwa i/lub informacji o wymaganiach wstępnych dotyczących Power BI Premium ofert na użytkownika.

Do momentu zaktualizowania ostatecznego cennika skorzystaj z informacji w tej sekcji, aby upewnić się, że zamówiony jest prawidłowy produkt.

Poniżej przedstawiono szczegóły dotyczące objętej sku i wymagań wstępnych.

| Nazwa wyświetlana oferty w wersji zapoznawczej cennika z 1 marca |  Zaktualizowano nazwę wyświetlaną oferty w ostatecznym cenniku z 1 kwietnia| Identyfikator oferty |
| ------ | ----------- | ----------- |
| Power BI Premium na użytkownika Add-On (cennik dla pracowników organizacji non profit)  |  Power BI Premium na użytkownika Add-On **(Office)** (cennik dla pracowników organizacji non-profit)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Klienci muszą mieć jedno z następujących wymagań wstępnych, aby kupić tę ofertę:

| Nazwa wyświetlana oferty | Identyfikator oferty |
| ------ | ----------- |
| Microsoft 365 E5 (cennik dla pracowników organizacji non profit)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 bez konferencji audio (cennik dla personelu organizacji non profit)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (cennik dla pracowników organizacji non profit)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Wersja próbna usługi Office 365 E5 (cennik dla pracowników organizacji non profit)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 bez konferencji audio (cennik dla pracowników organizacji non-profit)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Do zakupu Power BI Premium wymagana jest następująca oferta usługi:

| Nazwa wyświetlana oferty | Identyfikator oferty |
| ------ | ----------- |
|   Power BI Premium na użytkownika Add-On (cennik dla pracowników non profit)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Klienci muszą mieć następujące wymagania wstępne, aby kupić tę ofertę:

| Nazwa wyświetlana oferty | Identyfikator oferty |
| ------ |----------|
| Power BI Pro (Nonprofit Staff Pricing)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.  

### <a name="questions"></a>Masz pytania?

Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Aktualizacje marcowych cen dla Microsoft 365 F3

### <a name="categories"></a>Kategorie

- Data: 2021-03-16
- Oferty/rynki

### <a name="summary"></a>Podsumowanie

Poprawiono niepoprawne ceny z marca 2021 r. dla waluty Microsoft 365 F3 Funt brytyjskie (GB) i Euro (EUR).

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy kupują Microsoft 365 F3 w GB lub EUR między 1 marca a 17 marca 2021 r. w ramach programu Dostawca rozwiązań w chmurze (CSP).

### <a name="details"></a>Szczegóły

Firma Microsoft rozwiązała problem z nieprawidłowymi cenami Microsoft 365 F3. Nieprawidłowe ceny dotyczyły gb/usd i tylko ofert zakupionych w okresie od 1 marca do 17 marca 2021 r. Poniżej przedstawiono oferty i waluty, których to ma wpływ. 

| Nazwa oferty | Waluta | Identyfikator oferty | Identyfikator materiału |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Wc) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (komercyjne) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Cenniki bazowe licencji w wersji zapoznawczej z marca i kwietnia zostały zaktualizowane 16 marca o godzinie 17:00 czasu pacyficznego.

### <a name="next-steps"></a>Następne kroki

- Partnerzy powinni ponownie pobrać bieżące cenniki oparte na licencjach, zarówno w wersji zapoznawczej z marca, jak i kwietnia, z tymi korektami cen, jeśli ma to zastosowanie.  
- Firma Microsoft skontaktuje się z partnerami, których dotyczy problem, w najbliższych tygodniach za pośrednictwem poczty e-mail, aby poinformować ich o następnych krokach związanych z korygowania transakcji, których dotyczy problem.

### <a name="questions"></a>Masz pytania?

Aby uzyskać więcej pytań, zapoznaj się z odpowiednimi społecznościami usługi Yammer dla CSP.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Aktualizowanie nazwy firmy prawnej za pomocą Partner Center

### <a name="categories"></a>Kategorie

- Data: 2021-03-16
- Wydajność dysków & skalowania

### <a name="summary"></a>Podsumowanie

Od marca 2021 r. partnerzy Microsoft Partner Network (MPN) i odsprzedawcy pośredni Dostawca rozwiązań w chmurze (CSP) mogą aktualizować swoją nazwę firmy prawnej za pośrednictwem Partner Center.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy MPN i odsprzedawcy pośredni w programie CSP (nie dotyczy partnerów rozliczanych bezpośrednio w programie CSP)

### <a name="details"></a>Szczegóły

Od marca 2021 r. partnerzy MPN i odsprzedawcy pośredni w programie CSP mogą aktualizować swoje prawne nazwy firmy za pośrednictwem Partner Center w sposób zgodny i samoobsługowy. Dzięki tej nowej funkcji partnerzy nie będą już musieli przesyłać biletu Partner Center pomocy technicznej, aby zaktualizować nazwę firmy. Pozwoli to zaoszczędzić znaczną ilość czasu dla partnerów podczas wykonywania tych działań. 

Aby dowiedzieć się więcej, zobacz [Aktualizowanie legalnych profilów biznesowych.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Upewnij się, że nazwa firmy w Twoim profilu biznesowym jest bezpłatna od błędów pisowni i skrótów, i dokładnie pasuje do formalnych rekordów rejestracji firmy w firmie. Aby uzyskać więcej informacji na temat aktualizowania profilu organizacji, zobacz [Weryfikowanie profilu organizacji.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Następne kroki

Udostępnij te informacje w organizacji, aby odpowiedni zespół może przeglądać i aktualizować swoje procesy.

### <a name="questions"></a>Masz pytania?

Jeśli masz dodatkowe pytania, sprawdź odpowiednie społeczności CSP w usłudze Yammer.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Aktualizacja ewolucji programu Dostawca rozwiązań w chmurze (CSP) i zmiany programu licencjonowania Open License

### <a name="categories"></a>Kategorie

- Data: 2021-03-15
- Możliwości

### <a name="summary"></a>Podsumowanie

Nowe bezterminowe oferty oprogramowania w sektorze komercyjnym i publicznym będą dostępne w programie licencjonowania Dostawca rozwiązań w chmurze (CSP) wraz ze zmianami w programie licencjonowania Open.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Dystrybutorzy handlowi i odsprzedawcy zarządzani sprzedawani za pośrednictwem programu Licencjonowanie Open, a także wszyscy partnerzy programu CSP, którzy odsprzedają oprogramowanie bezterminowe

### <a name="details"></a>Szczegóły

We wrześniu 2020 r. firma [Microsoft](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) ogłosiła szereg kroków w ramach naszej cyfrowej transformacji w celu rozszerzenia możliwości partnerów w programie CSP, w tym dostępności oprogramowania lokalnego dla partnerów. Te zmiany umożliwiają partnerom rozwój firmy i rozszerzenie zasięgu dzięki wykorzystaniu licencji na oprogramowanie w programie CSP, pozycjonowając ich w celu osiągnięcia sukcesu we współczesnym świecie chmury. Zapewniają one również klientom przejście do chmury i zapewniają partnerom elastyczność potrzebną dla środowisk chmury hybrydowej klienta.

W kontynuacji tej transformacji cyfrowej ogłaszamy następujące zmiany:

- 1 lipca 2021 r.: do cennika programu Licencjonowanie open nie zostaną dodane żadne nowe jednostki SKU, produkty ani promocje.

- 7 lipca 2021 r.: do cennika oprogramowania CSP zostaną dodane dwie oferty komercyjne: Uzyskaj [](./2020-december.md#9)oryginalne systemy Windows i Visual Studio Professional oraz oferty sektora publicznego (dla instytucji rządowych, edukacji i organizacji non profit — zobacz ogłoszenie).  Cennik można znaleźć w sekcji Oprogramowanie na stronie Sell > Pricing & Offers (Ceny & [sprzedaży)](https://partnercenter.microsoft.com/pcv/sales) w Partner Center i zostanie ponownie opublikowany w tym dniu.

Aby uzyskać szczegółowe informacje dotyczące ewolucji programu CSP i zmian programu licencjonowania Open License, zobacz **Następne kroki** poniżej.

### <a name="next-steps"></a>Następne kroki:

- Ewolucja programu CSP: Przejrzyj oprogramowanie [bezterminowe w Dostawca rozwiązań w chmurze gotowość](https://partner.microsoft.com/resources/collection/software-in-csp#/) programu. Użyj tej [mapy gotowości,](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) aby szybko znaleźć odpowiednie informacje dla swojej roli.

- Zmiany programu licencjonowania Open: Przejrzyj materiały dotyczące zmian gotowości programu CSP i [Open License Program.](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) Użyj tej [mapy gotowości,](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) aby szybko znaleźć odpowiednie informacje dla swojej roli.

### <a name="questions"></a>Pytania

Aby uzyskać więcej pytań, zapoznaj się z odpowiednimi społecznościami usługi Yammer dla CSP.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Aktualizacja do poprzedniego anonsu: Premium Assessments , dodatek do Menedżera zgodności

### <a name="categories"></a>Kategorie

- Data: 2021-03-15
- Rozwijanie firmy

### <a name="summary"></a>Podsumowanie

Oferty wersji próbnej nie powinny być wymienione w cenniku i zostaną usunięte.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy inicjujące transakcje za pośrednictwem Dostawca rozwiązań w chmurze

### <a name="details"></a>Szczegóły

Oferty wersji próbnej nie powinny zostać uwzględnione w cenniku. Zostaną one usunięte z cennika z 1 maja 2021 r.

Oryginalne zawiadomienie znajduje się [tutaj.](./2021-february.md#4)

### <a name="additional-resources"></a>Dodatkowe zasoby

- [Microsoft 365 zabezpieczeń i zgodności E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Tworzenie ocen i zarządzanie nimi w Menedżerze zgodności firmy Microsoft — Microsoft 365 Zgodności](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.

### <a name="questions"></a>Masz pytania?

Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrowanie rozwiązań z usługi One Commercial Partner (OCP) do platformy handlowej firmy Microsoft

### <a name="categories"></a>Kategorie

- Data: 2021-03-12
- Możliwości

### <a name="summary"></a>Podsumowanie

Od 29 marca 2021 r. zaczniesz mieć ograniczone możliwości jednego partnera komercyjnego (OCP, One Commercial Partner) go-to-market (GTM). Zachęcamy do migrowania rozwiązań na platformę handlową w Partner Center.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Organizacje sprzedają się razem z rozwiązaniami w OCP GTM

### <a name="details"></a>Szczegóły

W grudniu 2020 r. rozpoczęliśmy podróż od narzędzia Microsoft OCP GTM do platformy handlowej firmy Microsoft w Partner Center. To przejście rozszerza możliwości platformy handlowej, na której można prezentować swoje rozwiązania milionom klientów, dwukierunkowo udostępniać możliwości innym sprzedawcom firmy Microsoft i partnerów oraz wspólnie sprzedawać innowacyjne rozwiązania.

Kolejny kamień milowy w przejściu zostanie miał miejsce 29 marca 2021 r. Właśnie wtedy zaczniesz mieć ograniczone możliwości OCP GTM, a niektóre pola stają się tylko do odczytu. Jeśli obecnie sprzedajesz rozwiązania w OCP GTM, zachęcamy do migrowania rozwiązań na platformę handlową, aby wykorzystać jej możliwości i uprościć środowisko publikowania. 

Przejście na platformę handlową sprawia, Partner Center głównym miejscem docelowym dla publikowania we współpracy sprzedaży. Jest to miejsce, w którym można kontynuować rozwój firmy, łącząc swoje rozwiązania z naszymi wspólnymi klientami za pośrednictwem tych samych kanałów i funkcji w produktach, których używamy dla produktów firmy Microsoft. [Dowiedz się więcej o platformie handlowej](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Następne kroki

- Jeśli rozwiązania nie zostały jeszcze przeniesione, postępuj [](/azure/marketplace/co-sell-solution-migration) zgodnie z instrukcjami podanymi w przewodniku przejścia lub wyświetl samouczek wideo krok po kroku, aby ukończyć wszystkie działania migracji i rozpocząć publikowanie swoich rozwiązań na platformie handlowej. [](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)

- W przypadku pytań dotyczących ograniczonego środowiska możliwości w UCP GTM zobacz wymagania dotyczące współpracy sprzedaży, aby opublikować w artykule Często zadawane pytania dotyczące platformy handlowej [firmy Microsoft.](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) (Zobacz sekcję "Ograniczone możliwości OCP GTM od 29 marca 2021 r.").

### <a name="questions"></a>Masz pytania?

Jeśli [masz pytania](https://partner.microsoft.com/support/?stage=1) lub potrzebujesz więcej informacji, skontaktuj się z pomocą techniczną.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Rozszerzanie nowego doświadczenia handlowego w programie Dostawca rozwiązań w chmurze (CSP) dla platformy Azure na Rosję

### <a name="categories"></a>Kategorie

- Data: 2021-03-10
- Możliwości

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Wszyscy partnerzy w Rosyjskim inicjuje transakcję za pośrednictwem Dostawca rozwiązań w chmurze (CSP).

### <a name="details"></a>Szczegóły

Od 10 marca 2021 r. z przyjemnością ogłaszamy dostępność nowego rozwiązania handlowego w programie CSP dla platformy **Azure w Rosyjskim**. To środowisko usprawni i poprawi sposób, w jaki klienci kupują i zużywają usługi platformy Azure. Zapewni ona również partnerom w programie CSP spójny widok cen platformy Azure w różnych ruchach sprzedaży, cen USD dla globalnej spójności, wyrównania dat rozliczeń i dostępu do Azure Cost Management.

### <a name="next-steps"></a>Następne kroki

Dostępnych jest kilka zasobów wprowadzających nowe środowisko handlowe platformy Azure i udostępniających dodatkowe informacje. Najnowsze często zadawane pytania, talii, wideo i inne informacje można znaleźć w galerii zasobów aktualizacji [programu CSP.](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Partner Center klucza licencji oprogramowania i realizacji pobierania

### <a name="categories"></a>Kategorie

- Data: 2021-03-04
- Możliwości

### <a name="summary"></a>Podsumowanie

Funkcja Partner Center pobierania oprogramowania i realizacji klucza licencji została przywrócona.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Wszyscy Dostawca rozwiązań w chmurze (CSP) w ramach zamówień oprogramowania bezterminowych subskrypcji serwerów za pośrednictwem Partner Center

### <a name="details"></a>Szczegóły

W odpowiedzi na opinie partnerów przywracamy możliwość realizacji Partner Center uzyskiwania kluczy oprogramowania i licencji w przypadku bezterminowych zamówień oprogramowania i zamówień na oprogramowanie subskrypcji serwera. Zostanie on przywrócony do poprzedniego stanu przed usunięciem 19 stycznia 2021 r. (Zobacz [anons).](2020-september.md#17)

Należy pamiętać, że klucze licencji na oprogramowanie i linki pobierania są cennymi i wysoce pożądanymi zasobami własności intelektualnej. W przypadku wycieku mogą one szybko zostać wyczerpane limity aktywacji i spowodować negatywne doświadczenia klientów i partnerów.

### <a name="next-steps"></a>Następne kroki

Zapoznaj się z następującymi zasobami, aby uzyskać instrukcje dotyczące użycia i ważne wskazówki dotyczące dystrybucji kluczy oprogramowania:

- [Sprzedaż oprogramowania lokalnego za pośrednictwem programu CSP](../csp-on-premise-software.md)
- [Partner Center nowego przewodnika operacji handlowych](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (zobacz **sekcję Guidance on Software Key Distribution** (Wskazówki dotyczące dystrybucji kluczy oprogramowania).

### <a name="questions"></a>Masz pytania?

Jeśli masz dodatkowe pytania dotyczące tego powiadomienia, sprawdź odpowiednie społeczności usługi Yammer.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrowanie transakcji z programu Partner Sales Connect (PSC) do Partner Center

### <a name="categories"></a>Kategorie

- Data: 2021-03-04
- Możliwości

### <a name="summary"></a>Podsumowanie

Partner Sales Connect (PSC) będzie miał dostęp tylko do odczytu od 31 marca 2021 r., dlatego zachęcamy do rozpoczęcia migracji twoich transakcji z programu PSC do Partner Center.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Partnerzy z transakcjami w chmurze

### <a name="details"></a>Szczegóły

W ramach naszego wspólnego zobowiązania do rozwoju wspólna sprzedaż z firmą **Microsoft** to ścieżka, którą możesz **odkryć,** dostarczyć swoją wiedzę i rozszerzyć zasięg klientów, aby uzyskać pozytywne wyniki dla klientów. Przy średniej transakcji, która jest **3,5** raza szybsza niż zwykle, zarządzanie doświadczeniem w zakresie współpracy sprzedaży w programie Partner Center umożliwia sprzedaż w kanałach bezpośrednich klientów, partnerów i sprzedawców firmy Microsoft oraz zarządzanie całym potokiem poleceń w jednej lokalizacji.

Od 31  marca **2021** r. program **PSC** będzie miał dostęp tylko do odczytu, dlatego zachęcamy do rozpoczęcia przechodzenia do programu Partner Center i uzyskiwania dostępu do tych ulepszeń możliwości: 

- **Dokładniejszy routing** transakcji, które udostępniasz firmie Microsoft właściwemu sprzedawcy, w zależności od rodzaju potrzebnej pomocy.
- **Weryfikacja uprawnień do** transakcji z góry dla rozwiązań kwalifikujących się do zachęt oraz spełnianie kryteriów programu ISV Connect, upraszczając proces zatwierdzania i ostateczne potwierdzenie wykonania (POE).
- **Bezproblemowe środowisko użytkownika** do zarządzania wszystkimi możliwościami sprzedaży i potencjalnymi klientami zakwalifikowanym do sprzedaży w jednym miejscu.

Niedawno dodaliśmy również nowe funkcje w programie Partner Center, które mogą pomóc w przenoszeniu:

- [Operacje zbiorcze dotyczące możliwości współpracy sprzedaży](../bulk-operations.md)
- [Funkcja migracji transakcji](../psc-to-pc.md) (zobacz **sekcję Migracja transakcji psc).**

Dzięki środowisku współpracy w Partner Center zespoły sprzedaży będą miały więcej czasu na skoncentrowanie się na tworzeniu potencjalnych klientów i szans sprzedaży, zamykaniu transakcji i tworzeniu długotrwałych relacji z klientami.

### <a name="next-steps"></a>Następne kroki

Skorzystaj z Partner Center [przejścia,](../psc-to-pc.md) aby przejść przez kroki migracji transakcji z usługi PSC do Partner Center.

### <a name="questions"></a>Masz pytania?

W przypadku jakichkolwiek dodatkowych pytań skontaktuj się z pomocą [techniczną.](https://partner.microsoft.com/support/?stage=1)

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nowe produkty i oferty usługi Microsoft Dynamics 365 dostępne od 1 kwietnia 2021 r.

### <a name="categories"></a>Kategorie

- Data: 2021-03-04
- Możliwości

### <a name="summary"></a>Podsumowanie

1 kwietnia 2021 r. firma Microsoft uruchomi kilka nowych produktów i ofert dla programu Dostawca rozwiązań w chmurze (CSP).

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)

### <a name="details"></a>Szczegóły

1 kwietnia 2021 r. firma Microsoft będzie wprowadzać następujące nowe produkty i oferty:

- Power BI Premium na użytkownika
- Rozszerzenie segmentów i obszarów geograficznych customer voice and marketing USL

**Power BI Premium na użytkownika**

Firma Microsoft wprowadzi pierwszą ofertę dla użytkowników Power BI Premium użytkowników. Power BI Premium jest obecnie sprzedawane tylko w konstrukcji pojemności. Power BI Premium na użytkownika zapewnia dostęp do funkcji analizy biznesowej (BI) i analizy przedsiębiorstwa. Elastyczne licencjonowanie poszczególnych miejsc jest przeznaczone dla małych i średnich firm.

Przejrzyj szczegóły [Power BI wersji,](/power-platform-release-plan/2020wave2/power-bi/planned-features) aby dowiedzieć się więcej o tej ofercie.


**Szczegóły oferty**

Pamiętaj, że nazwa oferty różni się nieco od wersji zapoznawczej cennika.

| Nazwa oferty | Identyfikator oferty |
| ------ |----------- |
| Power BI Premium na użytkownika | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium na użytkownika dla nauczycieli lub wykładowców | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium na użytkownika dla uczniów | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium na użytkownika (cennik dla pracowników niedochodowych) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium na użytkownika Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium na użytkownika Add-On dla nauczycieli lub wykładowców | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium na użytkownika Add-On dla uczniów | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium na użytkownika Add-On (cennik dla pracowników non profit) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Rozszerzenie segmentów i obszarów geograficznych CUSTOMER Voice and Marketing USL**

W związku z wprowadzeniem w grudniu 2020 r. oferty Dynamics 365 Customer Voice and Marketing USL zostały zmienione w celu dodania nowych krajów oraz bardziej niedochodowych i edukacyjnych jednostki SKU.

| Nazwa oferty | Identyfikator oferty |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (cennik dla pracowników non-profit) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL dla nauczycieli lub wykładowców | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Odwiedź następujące strony, aby dowiedzieć się więcej o tych ofertach:

- [Strona główna usługi Dynamics 365 Customer Service Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Strona główna usługi Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Następne kroki

Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.  

### <a name="questions"></a>Masz pytania?

Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Usługa Microsoft Drukowanie uniwersalne jest teraz dostępna w niektórych pakietach

### <a name="categories"></a>Kategorie

- Data: 2021-03-33
- Możliwości

### <a name="summary"></a>Podsumowanie

Usługa Microsoft Drukowanie uniwersalne będzie dostępna do transakcji w ramach wybranych pakietów Microsoft 365 i jako dodatek autonomiczny od 1 marca 2021 r.

### <a name="impacted-audience"></a>Odbiorcy, których to miało wpływ

Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)

### <a name="details"></a>Szczegóły

[Drukowanie uniwersalne](https://aka.ms/universalprint) to Microsoft 365 drukowania, która nie wymaga lokalnych serwerów wydruku i umożliwia drukowanie na urządzeniach z systemem Windows na drukarkach zarejestrowanych na platformie Azure. Będzie ona dostępna do transakcji od 1 marca 2021 r.

Pracownicy korzystają z drukowania bez sterowników, usprawnionego odnajdywania drukarek opartego na lokalizacji i intuicyjnego drukowania bez uczenia się. Urządzenia przyłączone do usługi Azure Active Directory (Azure AD) używają istniejących poświadczeń usługi Azure AD w celu bezpiecznego drukowania. Administratorzy zarządzają drukowaniem przy użyciu Azure Portal i mogą łatwo łączyć drukarki z natywną obsługą Drukowanie uniwersalne. Drukowanie uniwersalne można wdrożyć za pomocą niezgodnych drukarek przy użyciu łącznik Drukowanie uniwersalne oprogramowania.

Drukowanie uniwersalne zostaną wypełnione podczas startu w systemach Windows E3, A3, E5 i A5 oraz Microsoft 365 BP, F3, E3, A3, E5 i A5.  

**Szczegóły oferty**

Pamiętaj, że nazwa oferty różni się nieco od wersji zapoznawczej cennika.

| Nazwa oferty | Identyfikator oferty | Identyfikator materiału |
| ------ |----------- |----------- |  
| Drukowanie uniwersalne woluminu (500 zadań) — Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Drukowanie uniwersalne (500 zadań) dla nauczycieli lub wykładowców — Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Drukowanie uniwersalne woluminu (500 zadań) — System Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Drukowanie uniwersalne woluminu (500 zadań) dla nauczycieli lub wykładowców — Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Następne kroki

Zapoznaj się z cennikiem i omówieniem [Drukowanie uniwersalne .](/universal-print/fundamentals/universal-print-whatis) Udostępnij te informacje wszystkim odpowiednim kontaktom w twojej organizacji.

### <a name="questions"></a>Masz pytania?

Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.
