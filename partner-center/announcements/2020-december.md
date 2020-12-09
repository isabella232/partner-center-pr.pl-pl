---
title: Ogłoszenia z grudnia 2020 r.
description: Ogłoszenia 2020 w grudniu dla Centrum partnerskiego, w tym nowe możliwości, promocje, oferty, rynki lub zmiany w istniejących ofertach.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 12/02/2020
ms.openlocfilehash: 1341e60fd9914f421fd59335a8f037f3d915b72f
ms.sourcegitcommit: bc44a6e0c5ef048cda6e882fdb543c13c5b64912
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "96869303"
---
# <a name="december-2020-announcements"></a>Ogłoszenia z grudnia 2020 r.

Na tej stronie znajdują się szczegółowe informacje o anonsach programu Microsoft Partner Center dla listopada 2020.

2020 anonse: od [kwietnia](2020-april.md)do  |  [May](2020-may.md)  |  [czerwca](2020-june.md),  |  [July](2020-july.md)  |  [August](2020-august.md)  |  [wrzesień](2020-september.md),  |  [październik](2020-October.md)  |  [listopad](2020-november.md) | Grudzień

______________

## <a name="sdk-release-on-net-standard-v1163"></a><a name="4"></a>Wersja zestawu SDK na .NET Standard (v 1.16.3)

### <a name="categories"></a>Kategorie

- Data: 2020-12-8
- Możliwości

### <a name="impacted-audience"></a>Odbiorcy, których dotyczy problem

Bezpośredni partnerzy rozliczeń i dostawcy pośredniemu uczestniczący w programie CSP, którzy korzystają z zestawu SDK platformy .NET dla usługi Partner Center.

### <a name="details"></a>Szczegóły

Od grudnia 08 2020 partnerzy mogą rozpocząć pobieranie wersji [MicrosoftPartnerCenter. NETSDK (Galeria NuGet | Microsoft. Store. PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3), wraz z zaktualizowanymi [przykładami](https://github.com/Microsoft/Partner-Center-DotNet-Samples)z zestawu SDK usługi Public Partner Center. Ta wersja obejmuje następujące aktualizacje:
 
**SelfServePolicies — dodano nowe funkcje**

- [GetSelfServePolicies](/partner-center/develop/get-a-self-serve-policy-by-id.md)
- [GetListOfSelfServicePolicies](/partner-center/develop/get-a-list-of-self-serve-policies.md)
- [CreateSelfServePolicies](/partner-center/develop/create-a-self-serve-policy.md)
- [UpdateSelfServePolicies](/partner-center/develop/update-a-self-serve-policy.md)
- [DeleteSelfServePolicies](/partner-center/develop/delete-a-self-serve-policy.md)
 
**Profil firmy dla klientów**

- Dodano [OrganizationRegistrationNumber](/partner-center/develop/create-a-customer.md)
 
**CustomerBillingProfile.DefaultAddress**

- Dodano MiddleName
 
### <a name="next-steps"></a>Następne kroki

- Pobierz najnowszą wersję [MicrosoftPartnerCenter. NETSDK (Galeria NuGet | Microsoft. Store. PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3)
- Pobierz i przejrzyj przykłady w witrynie [GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

______________

## <a name="december-2020-license-based-price-list-release-notes"></a><a name="3"></a>Informacje o wersji cennika na podstawie licencji z grudnia 2020

### <a name="categories"></a>Kategorie

- Data: 2020-12-8
- Oferty/rynki

### <a name="summary"></a>Podsumowanie 

Na cenniku z cennikiem z grudnia 2020 i cennikiem listy oferty występuje kilka problemów.

### <a name="impacted-audience"></a>Odbiorcy, których dotyczy problem 

Wszyscy partnerzy przeprowadzają Operacje transakcyjne przez program Cloud Solution Provider (CSP)

### <a name="details"></a>Szczegóły

Listy cen na podstawie licencji w grudniu i pliki macierzy list oferty zawierają kilka anomalii. Te problemy dotyczą tylko plików cennika opartych na licencji i należy je skorygować w aktualizacjach z stycznia 2021.

#### <a name="incorrect-offers-in-the-license-based-price-list"></a>Nieprawidłowe oferty na liście cen na podstawie licencji

Listy cen na podstawie licencji w grudniu zawierają poniższe oferty, które nie powinny znajdować się na listach cen. Oferty te zostały wcześniej uwzględnione na liście cen i nie powinny zostać opublikowane. Nie ma harmonogramu od momentu, w którym mogą być dostępne. W przyszłości, jeśli zostaną dodane z powrotem, zostaną one wyświetlone jako dodatki w przyszłych cennikach w wersji zapoznawczej.

   |**Nazwa oferty**|**Identyfikator oferty**|
   |-------------------|:------|
   |Zasoby ludzkie Dynamics 365 (cennik dla niedochodowych)|1596fa61-7da1-4263-98f8-b27dfa4cfbb5|
   |Zasoby ludzkie Dynamics 365 dołączone do kwalifikującej oferty Dynamics 365 Base (cennik dla niedochodowych)|8bf0b826-e05b-45aa-9cd1-9a9f742f7731|
   |Zasoby ludzkie Dynamics 365 dołączone do kwalifikującej oferty Dynamics 365 Base (cennik dla niedochodowych) (Oferta kwalifikująca)|f906435d-9dc9-42ba-bea6-2a2b08ca60db|
   |Obszar piaskownicy zasobów ludzkich systemu Dynamics 365 (cennik dla niedochodowych)|079ec5ba-d726-4384-95af-62d135c210d2|
   |Dynamics 365 Human Resources (ceny niedochodowe)|931acecc-34c3-4f83-913e-c7fdbfd7e2a1|
   |Operacje na Dynamics 365 — kolejność wierszy (cennik dla cen niedochodowych)|7dd6b78a-3d53-47f8-8a64-bd84609a9a70|
   
#### <a name="incorrect-offers-in-the-offer-list-matrix"></a>Nieprawidłowe oferty w macierzy listy ofert
   
Poniższe oferty znajdowały się w macierzy z listą ofert z błędem. Nie są one dostępne, a jeszcze nie wprowadzono daty docelowej dla dostępności. Partnerzy powinni je zignorować.

   |**Nazwa oferty**|**Identyfikator oferty**|
   |-------------------|:------|
   |Operacje systemu Dynamics 365 — wydajność bazy danych (cenniki dotyczące niedochodowych)|1d3f4d81-89b9-419e-a880-31b2c50b8d66|
   |Operacje związane z systemem Dynamics 365 — pojemność plików (cennik dla niedochodowych)|dc173a86-285b-444c-881e-3ece531f67da|

#### <a name="powerapps-offer"></a>Oferta usługi powerapps

Ta oferta została uwzględniona w macierzy z listą ofert, ale nie z cennikiem z grudnia. Oferta jest dostępna i Cennik można znaleźć w pliku z cennikiem w poprzednim miesiącu. Tę ofertę należy dodać z powrotem do cennika stycznia.

   |**Nazwa oferty**|**Identyfikator oferty**|
   |-------------------|:------|
   |Aplikacje zaawansowane na plan aplikacji|5e1087b6-246B-4503-b88a-b60bdf0b3840|

### <a name="next-steps"></a>Następne kroki

Sprawdź informacje o wersji często, gdy inne problemy nie zostaną odkryte, zostaną dołączone do tego anonsu.

### <a name="last-updated"></a>Ostatnia aktualizacja

8 grudnia 2020 r.

______________

## <a name="an-update-of-the-us-microsoft-365-business-voice-with-calling-plan-offer-is-coming-soon"></a><a name="2"></a>Wkrótce zostanie udostępniona aktualizacja Microsoft 365 Business głosu z ofertą planu wywołującego

### <a name="categories"></a>Kategorie

- Data: 2020-12-3
- Oferty/rynki

### <a name="summary"></a>Podsumowanie 

Od 1 stycznia 2021 firma Microsoft rozpocznie przechodzenie przez partnerów i klientów z nami do nowego Microsoft 365 Business głosu z ofertą planu wywoływania. Nie jest wymagane wykonanie jakiejkolwiek akcji partnerskiej.

### <a name="impacted-audience"></a>Odbiorcy, których dotyczy problem 

Wszyscy partnerzy przeprowadzają Operacje transakcyjne przez program Cloud Solution Provider (CSP)

### <a name="details"></a>Szczegóły

Firma Microsoft zamieni istniejący głos biznesowy za pomocą oferty planu wywołującego w Stanach Zjednoczonych z nową ofertą, która będzie obsługiwać wewnętrzne wymagania dotyczące produktów odpływ. Nowa oferta będzie mieć ten sam zestaw funkcji i Cennik. Zmiany oferty są wewnętrzne dla firmy Microsoft i nie mają wpływu na sposób, w jaki partnerzy CSP na rynku, sprzedawać ani nie obsługują głosu biznesowego z ofertą planu wywoływania. Zmiana zostanie zastosowana tylko do tej oferty.

W przypadku nowej sprzedaży będziesz używać nowej oferty od 1 stycznia 2021. Stara oferta zostanie zastąpiona nową ofertą na cenniku.

Istniejący klienci zostaną automatycznie przeniesieni do nowej oferty w dniu ich odnowienia. Od partnerów nie jest wymagana żadna akcja i odnowienie klientów.


* * Szczegóły nowej oferty
 
   |**Nazwa oferty**|**Identyfikator oferty**|**Identyfikator materiału**|
   |-------------------|:------|:------|
   |Microsoft 365 Business Voice (US)|86713ec1-ad33-42cf-a1ce-8397d4d875fe|PZW-00023|
   
* * Szczegóły oferty

   |**Nazwa oferty**|**Identyfikator oferty**|**Identyfikator materiału**|
   |-------------------|:------|:------|
   |Microsoft 365 Business Voice (US)|9f9f2c7b-c961-402b-9421-8e3c9207eeb3|PZW-00009|

### <a name="next-steps"></a>Następne kroki

Zapoznaj się z cennikiem i Udostępnij te informacje wszystkim odpowiednim kontaktom w organizacji.

______________

## <a name="now-live-partner-center-api-updates-and-user-interface-enhancements-for-the-education-customer-validation-process"></a><a name="1"></a>Teraz na żywo: aktualizacje interfejsu API Centrum partnerskiego i ulepszenia interfejsu użytkownika dla procesu weryfikacji klienta edukacyjnego

### <a name="categories"></a>Kategorie

- Data: 2020-12-3
- Możliwości

### <a name="impacted-audience"></a>Odbiorcy, których dotyczy problem 

Partnerzy sprzedający oferty akademickie za pomocą programu Cloud Solution Provider

### <a name="summary"></a>Podsumowanie 

Firma Microsoft uruchamia się na zaufaniu. Firma Microsoft dokłada starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji klienta dla ofert akademickich transakcji w programie dostawcy rozwiązań w chmurze. W ramach tego zobowiązania wprowadzamy udoskonalenia interfejsu API Centrum partnerskiego oraz usprawnienia interfejsów użytkownika, które będą dodawać przejrzystość i wgląd w proces przed sprawdzeniem klienta, a także możliwość wprowadzania dokładniejszych danych, które pozwolą na lepsze pomyślne przed sprawdzeniem klientów. 

**Ulepszenia Centrum partnerskiego** 

- Nowe interfejsy API pobierania i OGŁASZAnia kwalifikacji do obsługi dokładnego wprowadzania danych i ulepszania procesu sprawdzania poprawności przez klienta edukacji przez firmę Microsoft. 

- Rozszerzenia interfejsu użytkownika do obsługi dokładnego wprowadzania danych i ulepszania procesu sprawdzania poprawności przez klienta edukacji przez firmę Microsoft. 

**Wycofanie istniejących interfejsów API uzyskiwania i UMIESZCZAnia kwalifikacji** 

Istniejące interfejsy API uzyskiwania i UMIESZCZAnia kwalifikacji zostaną wycofane **przed końcem lutego 2021**. W takim przypadku konieczne będzie przejście do nowego interfejsu API pobierania i publikowania Centrum partnerskiego, aby można było zakupić oferty szkoleniowe.  

**Testowanie** 

Aby lepiej zrozumieć interfejsy API i wpis danych wymagane do pomyślnej weryfikacji klienta, partnerzy mogą przetestować te ulepszenia. Partnerzy, którzy chcą uczestniczyć w testowaniu powinni pobrać [Przewodnik testowania klienta edukacyjnego Centrum partnerskiego](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf) , aby zapoznać się z instrukcjami dotyczącymi sposobu przygotowania, rejestracji i uzyskiwania informacji o tym, czego można oczekiwać w fazie testowania.

**Klienci biblioteki i muzeów** 

Oprócz powyższych ulepszeń firma Microsoft przyjemnością się z ogłoszeniem, że firma Microsoft oferuje oferty o cenie akademickiej dla klientów korzystających z bibliotek i Muzeówów, rozszerzając klientów edukacyjnych, którzy będą mogli korzystać z funkcji Transact CSP. 

Firma Microsoft zastrzega sobie prawo do przeglądania statusu dowolnego klienta lub proponowanego klienta jako wykwalifikowanych użytkowników edukacyjnych. Aby uzyskać szczegółowe informacje, zobacz [wymagania dotyczące użytkowników z wykwalifikowanymi](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7) wersjami edukacyjnymi. 

### <a name="next-stepsadditional-resources"></a>Następne kroki/dodatkowe zasoby

- Zapoznaj się z nowym interfejsem użytkownika Centrum partnerskiego, zmianami interfejsu API i przewodniku w zasobach gotowości do działania: usprawnienia procesu [weryfikacji klienta edukacyjnego w centrum partnerskim](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/) 

- Upewnij się, że Twoja organizacja ma zaznajomienie się z [wymaganiami edukacyjnymi dla użytkowników edukacyjnych](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7). 

- Podziel się tymi informacjami z odpowiednimi zespołami w organizacji oraz z odsprzedawcami, aby ułatwić im przygotowanie się do tych zmian. 

### <a name="change-log"></a>Dziennik zmian 

31 sierpnia 2020: Oryginalna publikacja 

- 25 września 2020: dodano aktualizację okna testowego 

- 4 października 2020: przypomnienie dotyczące rejestracji na potrzeby testowania 

- 10 listopada 2020: przypomnienie dotyczące rejestracji w celu testowania 

- 3 grudnia 2020: aktualizacje interfejsu API na żywo 
