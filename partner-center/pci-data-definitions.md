---
title: Szczegółowe definicje danych
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokument zawiera listę różnych raportów i definicje danych poszczególnych raportów, które można pobrać z strony raportu pobieranie szczegółowych informacji.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2020
ms.locfileid: "97502131"
---
# <a name="export--data-definitions"></a>Eksportowanie — definicje danych 

 **Odpowiednie role** 

- Podgląd raportów 
- Executive — Podgląd raportów 

## <a name="introduction"></a>Wprowadzenie 

Centrum pobierania raportów na pulpicie nawigacyjnym usługi Insights umożliwia eksportowanie zestawów danych pierwotnych.  

Różne raporty, które można pobrać wraz z definicją danych, są następujące: 

**Profil partnera**: definicje danych różnych pól raportu profilu są następujące: 


| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|MPNId|Identyfikator Microsoft Partner Network|
|PartnerName|Nazwa partnera |
|PGA_MPNId|IDENTYFIKATOR MPN konta globalnego partnera|
|PGA_PartnerName|Nazwa konta globalnego partnera|
|City (Miasto)|Lokalizacja miasta partnera |
|Kraj|Lokalizacja kraju partnera |
|HierarchyLevel|Wskazuje, czy jest to globalny identyfikator MPN, czy lokalizacja MPN identyfikator|

**Szczegóły klienta**: definicje danych różnych pól raportu szczegóły klienta są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CustomerName|Nazwa klienta |
|CustomerTenantId|Identyfikator dzierżawy klienta |
|CustomerTpid|Górny identyfikator elementu nadrzędnego klienta |
|CustomerSegment|Segment klienta |
|CustomerMarket|Rynek geograficzny klienta  |
|CustomerStatus|Stan klienta (Active/inactive) |
|Produkt|Produkt został sprzedany klientowi przez MPN. Jest to jedna z usług O365, D365, Enterprise Mobility, Power BI, Microsoft Azure.|
|SKU|   Jednostka SKU produktu|
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie i przychód|
|MPNId| Identyfikator Microsoft Partner Network|
|PartnerName|   Nazwa partnera|
|PartnerLocation|   Lokalizacja geograficzna partnera|
|PartnerAttributionType|    Typ elementu partnera|
|SalesChannel|  Kanał sprzedaży|
|AvailableSeats|    Dostępne stanowiska| 
|RevenueUSD|    Przychód w USD|

**Wydajność odsprzedawcy**: definicje danych różnych pól raportów o wydajności odsprzedawcy są następujące:

> [!Note]
> Dane dotyczące przychodów i ACR są dostępne tylko dla użytkowników, którzy są użytkownikami programu Executive w raportach.

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|ResellerMpnid|Identyfikator Microsoft Partner Network odsprzedawcy| 
|ResellerName (Nazwa odsprzedawcy)|Nazwa odsprzedawcy|
|ResellerMarket|Kraj odsprzedawcy| 
|IndirectProviderMPNId|Identyfikator Microsoft Partner Network dostawcy pośredniego|
|IndirectProviderName|Nazwa dostawcy pośredniego|
|Month (Miesiąc)|Miesiąc, dla którego zgłaszane jest użycie i przychód|
|Produkt|Nazwa produktu|
|Identyfikator|Identyfikator subskrypcji|
|AvailableSeats|Liczba dostępnych stanowisk|
|AssignedSeats|Liczba przypisanych stanowisk|
|BilledRevenueUSD|Przychód rozliczany (w $)|
|CustomerName|Nazwa klienta| 
|CustomerTPid|Górny identyfikator elementu nadrzędnego klienta| 
|CustomerSegment|Segment klienta |
|CustomerMarket|Rynek geograficzny klienta |
|ResellerStatus|Stan odsprzedawcy| 

**Szczegóły subskrypcji**: definicje danych różnych pól raportu szczegóły subskrypcji są następujące:

>[!Note]
>Dane dotyczące przychodów i ACR są dostępne tylko dla użytkowników, którzy są użytkownikami programu Executive raportów

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|SubscriptionId|    Identyfikator GUID subskrypcji|
|SubscriptionStartDate| Data rozpoczęcia subskrypcji|
|SubscriptionEndDate|   Data końcowa subskrypcji|
|SubscriptionState| Stan subskrypcji (aktywny lub zmieniony)|
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie i przychód|
|IsAutoRenew|   Wskazuje, czy subskrypcja jest autoodnawiana, czy nie (t/N)|
|CustomerName|  Nazwa klienta| 
|CustomerTenantId|  Identyfikator GUID klienta|
|CustomerTpid|  Górny identyfikator elementu nadrzędnego klienta| 
|CustomerSegment|   Segment rynku klienta| 
|CustomerMarket|    Rynek geograficzny klienta|
|Produkt|   Produkt sprzedawany klientowi przez partnera| 
|SKU|   Jednostka SKU produktu |
|MPNId| Identyfikator Microsoft Partner Network partnera |
|PartnerName|   Nazwa partnera |
|PartnerLocation|   Lokalizacja geograficzna partnera |
|PartnerAttributionType|    Typ przypisywania dla subskrypcji|
|SalesChannel|  Kanał sprzedaży (Direct/CSP itp.) |
|AvailableSeats|    Bieżące dostępne stanowisko|
|RevenueUSD|    Przychód w USD|
|Identyfikator rejestracji| Identyfikator rejestracji subskrypcji|

**Użycie platformy Azure**: definicje danych różnych pól raportu użycia platformy Azure są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|SubscriptionId|    Identyfikator GUID subskrypcji|
|SubscriptionStartDate| Data rozpoczęcia subskrypcji.|
|SubscriptionEndDate|   Data zakończenia subskrypcji.|
|SubscriptionState| Bieżący stan subskrypcji (otwarty/zamknięty/aktywny/okres prolongaty)|
|Month (Miesiąc)| Data agregowana według miesiąca |
|ServiceName|   Nazwa usługi platformy Azure|
|MeterCategory| Nazwa kategorii miernika|
|UsageUnits|    Liczba jednostek używanych w trakcie cyklu rozliczeniowego. |
|CustomerName|  Nazwa klienta |
|CustomerTenantId|  Identyfikator dzierżawy klienta |
|CustomerTpid|  Identyfikator nadrzędnego elementu klienta |
|CustomerSegment|   Segment klienta |
|CustomerMarket|    Rynek geograficzny klienta |
|MPNId  |Identyfikator Microsoft Partner Network klienta |
|PartnerName|   Nazwa partnera |
|PartnerLocation    |Lokalizacja regionu geograficznego partnera |
|PartnerAttributionType |Typ elementu partnera|
|SalesChannel|  Kanał sprzedaży (bezpośredni/CSP pośredni/CSP Direct itp.) |
|ACR_USD|   Przychód zużyty przez platformę Azure w USD|
|Identyfikator rejestracji| Identyfikator rejestracji subskrypcji platformy Azure|

**Office 365 — użycie licencji**: definicje danych różnych pól raportu użycia licencji pakietu Office 365:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CustomerTenantId|  Identyfikator dzierżawy klienta| 
|CustomerTpid|  Identyfikator nadrzędnego elementu klienta |
|Nr obciążenia|  SFB, zespoły, EXO |
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie|
|PaidAvailableUnits|    Liczba płatnych jednostek|
|MonthlyActiveUsers|    Liczba aktywnych użytkowników miesięcznie|
|CustomerName|  Nazwa klienta|
|CustomerMarket|    Geograficzna lokalizacja kraju klienta |
|CustomerSegment|   Segment klienta |
|MPNId| Identyfikator Microsoft Partner Network|
|PartnerName|   Nazwa partnera|
|PartnerLocation|   Lokalizacja geograficzna partnera|
|PartnerAttributionType|    Typ elementu partnera|

**Enterprise Mobility — użycie licencji**: definicja danych różnych pól raportu dotyczącego użycia licencji pakietu EMS:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CustomerTenantId|  Identyfikator dzierżawy klienta| 
|CustomerTpid|  Identyfikator nadrzędnego elementu klienta |
|Nr obciążenia|  Nazwa obciążenia EMS |
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie|
|PaidAvailableUnits|    Liczba płatnych jednostek|
|MonthlyActiveUsers|    Liczba aktywnych użytkowników miesięcznie|
|CustomerName|  Nazwa klienta|
|CustomerMarket|Geograficzna lokalizacja kraju klienta |
|CustomerSegment|   Segment klienta |
|MPNId| Identyfikator Microsoft Partner Network|
|PartnerName|   Nazwa partnera|
|PartnerLocation|   Lokalizacja geograficzna partnera|
|PartnerAttributionType|    Typ elementu partnera|

**Dynamics 365 — użycie licencji**: definicja danych różnych pól raportu Dynamics 365 — użycie licencji to:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|SubscriptionId|Identyfikator GUID subskrypcji|
|SubscriptionStartDate| Data rozpoczęcia subskrypcji|
|SubscriptionEndDate|   Data końcowa subskrypcji|
|SubscriptionStatus|    Stan subskrypcji |
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie|
|RevSumDivisionName|    Nazwa podziału sumy Rev.|
|RevSumCategoryName|    Nazwa kategorii sum Rev|
|SKU|   Jednostka SKU produktu |
|Identyfikatora skuId| Identyfikator jednostki SKU produktu |
|FreeVsPaidSKU| Wskazuje, czy jest to bezpłatna czy płatna jednostka SKU |
|SalesModel|    Kanał sprzedaży używany do sprzedaży subskrypcji|
|DetailedSalesModel|    Szczegółowy model sprzedaży dla subskrypcji|
|CustomerName|  Nazwa klienta |
|CustomerTenantId|  Identyfikator GUID dzierżawy klienta |
|CustomerTpid|  Górny identyfikator elementu nadrzędnego klienta |
|CustomerSegment|   Segment rynku klienta |
|CustomerMarket|    Rynek geograficzny klienta |
|MPNId| Identyfikator sieci partnera firmy Microsoft |
|PartnerName|   Nazwa partnera |
|PartnerLocation|   Lokalizacja regionu geograficznego partnera |
|PartnerAttachType| Typ przypisywania dla subskrypcji|
|AvailableSeats|    Bieżące dostępne stanowisko|
|AssignedSeats| Bieżące przypisane miejsce |
|ActiveSeats|   Bieżące aktywne stanowiska |
|DeploymentOpportunity| Bieżąca szansa sprzedaży wdrożenia|
|ActiveUsagePercent|    Bieżące aktywne procenty użycia|
 
**Power BI użycie licencji**: definicja danych różnych pól raportu Power BI — użycie licencji to:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|SubscriptionId|    Identyfikator GUID subskrypcji|
|SubscriptionStartDate| Data rozpoczęcia subskrypcji|
|SubscriptionEndDate|   Data końcowa subskrypcji|
|SubscriptionStatus|    Stan subskrypcji (aktywny lub In-Active lub okres prolongaty)|
|Month (Miesiąc)| Data agregowana według miesiąca |
|SKU|   Jednostka SKU produktu |
|Identyfikatora skuId| Identyfikator jednostki SKU produktu |
|FreeVsPaidSKU| Bezpłatny lub płatny rozróżnienie jednostki SKU |
|SalesModel|    Model sprzedaży używany do sprzedaży subskrypcji|
|DetailedSalesModel|    Szczegółowy model sprzedaży dla subskrypcji|
|CustomerName|  Nazwa klienta |
|CustomerTenantId|  Identyfikator GUID dzierżawy klienta |
|CustomerTpid|  Górny identyfikator elementu nadrzędnego klienta| 
|CustomerSegment|   Segment rynku klienta |
|CustomerMarket|    Rynek geograficzny klienta |
|MPNId| Identyfikator Microsoft Partner Network |
|PartnerName|   Nazwa partnera |
|PartnerLocation|   Lokalizacja regionu geograficznego partnera |
|PartnerAttachType| Typ przypisywania dla subskrypcji|
|AvailableSeats|    Bieżące dostępne stanowiska|
|AssignedSeats| Aktualnie przypisane stanowiska|
|ActiveSeats|   Bieżące aktywne stanowiska|
|DeploymentOpportunity| Bieżąca szansa sprzedaży wdrożenia|
|ActiveUsagePercent|    Bieżące aktywne procenty użycia|

**Użycie zespołów — spotkania i wywołania**: definicje danych różnych pól są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CustomerTenantId|  Identyfikator dzierżawy klienta |
|CustomerTpid|  Identyfikator nadrzędnego elementu klienta |
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie|
|Obciążanie|   Obciążenie podrzędne, dla którego zgłaszane jest użycie (spotkania, wywołania, systemy telefoniczne)|
|Liczba spotkań| Liczba spotkań|
|Czas trwania spotkania|  Łączny czas trwania spotkań w godzinach|

**Zespoły — szczegóły dotyczące miesięcznego użycia**: definicje danych różnych pól są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CustomerTenantId|  Identyfikator dzierżawy klienta |
|CustomerTpid|  Identyfikator nadrzędnego elementu klienta |
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie|
|Obciążanie|   Obciążenie podrzędne, dla którego zgłaszane jest użycie (spotkania, wywołania, systemy telefoniczne)|
|Użytkownicy komputerów stacjonarnych| Liczba użytkowników korzystających z zespołów na komputerze|
|Użytkownicy mobilni|  Liczba użytkowników korzystających z zespołów na urządzeniach przenośnych|
|Użytkownicy sieci Web| Liczba użytkowników korzystających z zespołów w sieci Web|
|AllUpParticipants| Liczba odrębnych użytkowników zespołów w miesiącu|

**Użycie zespołów — 3P Apps**: definicje danych różnych pól są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CustomerTenantId|  Identyfikator dzierżawy klienta| 
|CustomerTpid|  Identyfikator nadrzędnego elementu klienta |
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane jest użycie|
|Nazwa aplikacji 3P|   Nazwa aplikacji Teams|
|Liczba użytkowników|    Liczba użytkowników aplikacji|


**Szczegóły szkolenia**: definicje danych różnych pól raportu szczegóły szkolenia są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|TrainingActivityId|    Identyfikator szkolenia |
|TrainingTitle| Tytuł szkolenia |
|Szkolenietype|  Typ szkolenia (certyfikacja/egzamin)|
|IndividualFirstName|   Imię klienta| 
|IndividualLastName|    Nazwisko klienta| 
|E-mail| Osobisty identyfikator poczty E-mail klienta|
|CorpEmail| Identyfikator poczty e-mail klienta|
|TrainingCompletionDate|    Data ukończenia szkolenia |
|Month (Miesiąc)| Miesiąc, dla którego są zgłaszane dane|
|IcMCP| Wskazuje, czy użytkownik jest certyfikowanym specjalistą firmy Microsoft|
|MCPID| IDENTYFIKATOR MCP użytkownika|
|MPNId| Identyfikator Microsoft Partner Network |
|PartnerName|   Nazwa partnera |
|PartnerCityLocation|   Lokalizacja geograficzna partnera |
|PartnerCountryLocation|    Lokalizacja regionu geograficznego partnera |

**Microsoft Learn**: definicje danych różnych pól raportu Microsoft Learn są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|Nazwa użytkownika|Nazwa użytkownika| 
|UserId|Identyfikator GUID użytkownika |
|Szkoleniename|Nazwa szkolenia |
|Szkolenietype|Typ szkolenia (ścieżka/Learning modułu)|
|Produkty|Produkt, dla którego ma zastosowanie moduł uczenia|
|Role|Odpowiednie role szkoleniowe |
|CompletionDate|Data ukończenia szkolenia |
|MPNId|Identyfikator Microsoft Partner Network |
|PartnerName|Nazwa partnera |
|Kraj|Lokalizacja regionu geograficznego partnera |

**Podsumowanie kompetencji i historia**: definicja danych różnych pól w raporcie dotyczącym kompetencji i historii jest:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CompetencyName|Nazwa kompetencji |
|CompetencyLevel|Poziom kompetencji (Gold/Silver)|
|CompetencyStatus|Bieżący stan kompetencji (aktywny/nieaktywny/w okresie prolongaty)|
|CompetencyStartDate|Data rozpoczęcia danej kompetencji| 
|CompetencyEndDate|Data zakończenia podanej kompetencji |

**Wydajność kompetencji**: definicje danych różnych pól raportu wydajności dotyczącej kompetencji są następujące:

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|CompetencyName|    Nazwa kompetencji |
|CompetencyAttainmentOptionName|    Nazwa opcji uzyskania kompetencji|
|Month (Miesiąc)| Miesiąc, dla którego zgłaszane są metryki|
|MetricName|    Nazwa metryki związanej z kompetencją|
|MetricMonthlyContribution| Miesięczny udział w metryce|
|TTMAggregate|  Zagregowana Metryka na końcowe 12 miesięcy|
|AnniversaryYearAggregate|  Zagregowana Metryka dla bieżącego roku rocznicowego|
|GoldThreshold| Wymagania dotyczące wydajności w celu spełnienia wymagań w zakresie złota|
|SilverThreshold|   Wymagania dotyczące wydajności w celu spełnienia kompetencji Silver|

**DoM365nie do chmury**: definicje danych różnych pól raportu "wzniesienie-M365":

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|Identyfikator MPN|    Identyfikator Microsoft Partner Network|
|Nazwa partnera|  Nazwa partnera|
|Customer ID|   Numer identyfikacyjny klienta |
|Numer DUNS|   & Dun Bradstreet numer klienta ocenianego dla pozostałej części|
|Nazwa konta|  Nazwa konta |
|Domena|    Domena konta|
|Rozmiar organizacji|  Rozmiar organizacji|
|Branża|  Branża  |
|Pionowa|  Pionowy klient, którego wynikiem jest ocena, zgodnie z opisem przez firmę Microsoft i inne standardy branżowe (D&B)|
|Obszar|  Obszar geograficzny lokalizacji|
|Przedstawicielstwo|    Dotacja dla klienta będącego wynikiem oceny|
|Sales Territory (Obszar sprzedaży)|   Terytorium sprzedaży dla tego klienta jest oceniane|
|City (Miasto)|  Lokalizacja geograficzna |
|Stan| Lokalizacja stanu geograficznego|
|Postal Code|   Postal Code|
|Kraj|   Lokalizacja kraju geograficznego |
|Segment|   Segment rynku |
|Segment podrzędny|   Segment podrzędny rynku |
|Podsumowanie typu SMC|  Typ SMC |
|Najwyższe niezarządzane — podstawa obliczeń|  Najlepsi niezarządzani klienci — obliczenia|
|Najważniejsze niezarządzane — baza użytkowników| Główni niezarządzani klienci — użytkownik|
|IsNonProfit|   Czy zysk (tak/nie) (tak/nie)|
|Włącz zdalną służbę — docelowa usługa Exchange Online|   Klienci z aktywną subskrypcją usługi Exchange Online, która jest sprzedawana do M365|
|Włącz zdalne pozyskiwanie Premium (aktualna wersja) przy użyciu CLAS-+ 10 licencji|Klient, który ma aktualne Premium Office lub win Client (czyli wersje, które są po EOS produktów). Klient ma co najmniej 10 licencji. Klient, który ma wynik propióra. Partnerzy powinni kierować do M365.|
|Włącz zdalne pozyskiwanie Premium (bieżąca wersja) z proCLASami — licencje na <10|Klient, który ma aktualne Premium Office lub win Client (czyli wersje, które są po EOS produktów). Klient ma mniej niż 10 licencji. Klient, który ma wynik propióra. Partnerzy powinni kierować do M365.|
|Włącz zdalne pozyskiwanie Premium (aktualna wersja) bez CLAS-+ 10 licencji| Klient, który ma aktualne Premium Office lub win Client (czyli wersje, które są po EOS produktów). Klient ma co najmniej 10 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować do M365.|
|Włącz zdalne pozyskiwanie Premium (bieżąca wersja) bez poCLAS — licencje na <10| Klient, który ma aktualne Premium Office lub win Client (czyli wersje, które są po EOS produktów). Klient ma mniej niż 10 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować do M365.|
|Włącz zdalne pozyskiwanie Premium (EOS) z CLAS propiórami-+ 10|Klient, który ma EOS na Premium Office lub win Client (czyli wersje, które są starsze niż i obejmują produkty EOS. Klient ma co najmniej 10 licencji. Klient ma wynik. Partnerzy powinni kierować do M365.|
|Włącz zdalne pozyskiwanie Premium (EOS) z CLAS propiórem — licencje na <10|Klient, który ma EOS na Premium Office lub win Client (czyli wersje, które są starsze niż i obejmują produkty EOS. Klient ma mniej niż 10 licencji. Klient ma wynik. Partnerzy powinni kierować do M365.|
|Włącz zdalne pozyskiwanie Premium (EOS) bez CLAS-+ 10 licencji| Klient, który ma aktualne Premium Office lub win Client (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma co najmniej 10 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować do M365.|
|Włącz zdalne pozyskiwanie Premium (EOS) bez CLAS propióra — licencje na <10| Klient, który ma aktualne Premium Office lub win Client (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma mniej niż 10 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować do M365.|
|Włącz zdalną służbę — duży perspektywa dla M365 (wykonaj teraz/Oceń)| Potencjalni klienci z wysoką perspektywą dla M365.|
|Włącz zdalną współpracę — konkurowanie (powiększanie) za pomocą M365| Klienci z powiększaniem i M365, celem konwersji na zespoły|
|Włącz zdalną współpracę — konkurowanie (powiększanie) bez M365|  Klienci z powiększeniem, celem konwersji na zespoły|
|Obniżanie kosztów i zarządzanie-M365 E3 dla M365 E5| Istniejący klient z M365 E3, cel dla M365 E5|
|Obniżanie kosztów i zarządzanie klientami M365 BB i BS przeznaczonymi dla M365 BP|    Istniejący M365 BB i BS klienci mają do nich miejsce dla M365 BP|
|Przekształcanie produktywności organizacyjnej — pióra powierzchni|    Klient pokazuje pokazywanie pióra powierzchni.|
|M365Cluster|Określa proM365i klienta do zakupu.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|M365Fit|   Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowywanie oceniania przy użyciu modelu podobny do najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne dla Microsoft Cloud produktów. Punktacja jest aktualizowana kwartalnie.|
|M365Intent|    Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie intencji jest nadmiarowe w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc.|
|SurfaceCluster|    Umożliwia to zidentyfikowanie promiaru klientów w celu zakupu powierzchni przez skonsolidowanie zaleceń dotyczących dopasowania i celu do klastra.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|SurfaceFit|    Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowywanie oceniania przy użyciu modelu podobny do najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne dla Microsoft Cloud produktów. Punktacja jest aktualizowana kwartalnie.|
|SurfaceIntent| Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie intencji jest nadmiarowe w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc.|
|O365Cluster|   Umożliwia to zidentyfikowanie klienta w celu zakupienia usługi O365.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|O365Fit|   Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowywanie oceniania przy użyciu modelu podobny do najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne dla Microsoft Cloud produktów. Punktacja jest aktualizowana kwartalnie.|
|O365Intent|    Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie intencji jest nadmiarowe w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc.|
|M365UpsellCustomer|    Ta wartość określa, czy klient pokazuje niesprzedawaną M365|
|Ma Google|    Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów firmy Google|
|Ma AWS|   Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów AWS|
|Ma EA|    Ta wartość określa, czy odnowienie jest umową Enterprise Agreement (EA), czy z subskrypcją EA|
|Ma otwarte|  Wskazuje to, czy odnowienie jest umową Open Value, czy otwartą|

**DoD365nie do chmury**: definicje danych różnych pól raportu "wzniesienie-D365":

| **Nazwa kolumny** | **Opis danych** |
|---------|:---------|
|Identyfikator MPN|    Identyfikator Microsoft Partner Network|
|Nazwa partnera|  Nazwa partnera|
|Customer ID|   Numer identyfikacyjny klienta |
|Numer DUNS|   & Dun Bradstreet numer klienta ocenianego dla pozostałej części|
|Nazwa konta|  Nazwa konta |
|Domena|    Domena konta|
|Rozmiar organizacji|  Rozmiar organizacji|
|Branża|  Branża  |
|Pionowa|  Pionowy klient, którego wynikiem jest ocena, zgodnie z opisem przez firmę Microsoft i inne standardy branżowe (D&B)
|Obszar|  Obszar geograficzny lokalizacji|
|Przedstawicielstwo|    Dotacja dla klienta będącego wynikiem oceny|
|Sales Territory (Obszar sprzedaży)|   Sales Territory (Obszar sprzedaży)|
|City (Miasto)|  Lokalizacja geograficzna |
|Stan| Lokalizacja stanu geograficznego|
|Postal Code|   Postal Code|
|Kraj|   Lokalizacja kraju geograficznego |
|Segment|   Segment rynku |
|Segment podrzędny|   Segment podrzędny rynku |
|Podsumowanie typu SMC|  Kategoryzacja klienta: najważniejsze niezarządzane bazy użytkowników są klientami z 300 i pracownikami, a największa niezarządzana baza obliczeniowa to klienci z $10-letnim potencjałem platformy Azure, średnia firma to klienci z 25 pracownikami lub większymi, niewielkie firmy to klienci z mniej niż 25 pracownikami|
|Najwyższe niezarządzane — podstawa obliczeń   |Najlepsi niezarządzani klienci — obliczenia|
|Najważniejsze niezarządzane — baza użytkowników| Główni niezarządzani klienci — użytkownicy|
|IsNonProfit|   Czy zysk (tak/nie) (tak/nie)|
|Aktywuj sprzedawanie cyfrowe — rozmiar M365 >= 25 siedzeń (model SalesPro propozycji)|   Klient bez D365. Rozmiar miejsca: 25 i. Partnerzy powinni kierować do D365 Salespro|
|Aktywuj sprzedawanie cyfrowe — D365 SalesPro (wykonaj teraz/Oceń) |Klienci z dużą piórem bez D365.  Partnerzy powinni kierować do D365 SalesPro.|
|Zarządzanie ryzykiem finansowym & oszustw-Dynamics on-Premium Install Base-Navision (model BC)|Istniejący klient z systemem Navision lokalnego.  Partner powinien kierować do D365 BC|
|Zarządzanie ryzykiem finansowym & oszustw-Dynamics on-Premium Install Base-AX (model za F&O)    |Istniejący klient z systemem lokalnego AX.  Partner powinien kierować do D365 F&O|
|Zarządzanie ryzykiem finansowym & oszustw-Dynamics on-Premium Install Base-Great Plains (model Pro BC)|  Istniejący klient z lokalnego Great Plains.  Partner powinien kierować do D365 BC|
|Zarządzanie ryzykiem finansowym & oszustw-Dynamics on-Premium Install Base-Salomona (model BC)|Istniejący klient z lokalnego Wyspy Salomona.  Partner powinien kierować do D365 BC|
|Zarządzanie ryzykiem finansowym & oszustw-Dynamics on-Premium Install Base-others (model: BC) |Istniejący klient z innymi rozwiązaniami lokalnego, które nie są wymienione powyżej.  Partner powinien kierować do D365 BC|
|Tworzenie procesów biznesowych Agile — Dynamics on-Premium Install Base-AX/GP/SL/NAV/Other (D365 model Pro)|   Tworzenie procesów biznesowych Agile — Dynamics on-Premium Install Base-AX/GP/SL/NAV/Other (D365 model Pro)|
|Tworzenie procesów biznesowych Agile — podstawy konkurowania — Mendix/Systems/Salesforce (model D365 Pro")| Tworzenie procesów biznesowych Agile — podstawy konkurowania — Mendix/Systems/Salesforce (model D365 Pro")|
|Kompiluj procesy biznesowe Agile — baza instalacji D365 F&O |Istniejący klienci D365 F&O.  Partner na aplikacje docelowe.|
|Kompiluj procesy biznesowe Agile — baza instalacji D365 BC| Istniejący klienci D365 BC. Partner na aplikacje docelowe.|
|Kompiluj procesy biznesowe Agile — baza instalacji D365 CE| Istniejący klienci D365 CE. Partner na aplikacje docelowe.|
|Twórz odporny na błędy łańcuchy dostaw — Wykorzystaj i aktywuj pierwsze obciążenie D365 jako łańcuch dostaw D365 z klientami z systemami innym niż Oracle/SAP ERP|  Kierowanie klientów do łańcucha dostaw D365.|
|Twórz odporny łańcuchy dostaw — transsprzedażowy łańcuch dostaw D365 i/lub handel detaliczny do istniejących klientów D365 CE |Istniejący klienci D365 CE mają do sprzedaży krzyżowego łańcucha dostaw D365|
|Utwórz odporny na awarie łańcuch dostaw — D365 SUP. Łańcuch i/lub handel detaliczny/handel do D365 CE i (Oracle lub SAP)| Istniejący klienci usługi D365 CE z oprogramowaniem Oracle lub SAP, który jest przeznaczony dla łańcucha dostaw D365|
|D365BCCluster| Umożliwia to zidentyfikowanie proD365ów klienta do zakupu programu Business Central.  Klienci, którzy wyświetlają pióro dla BC, będą w średnich i małych kategoriach.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|D365BCFit| Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowywanie oceniania przy użyciu modelu podobny do najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne dla Microsoft Cloud produktów. Punktacja jest aktualizowana kwartalnie.|
|D365BCIntent|  Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie intencji jest nadmiarowe w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc.|
|D365FOCluster| Umożliwia to zidentyfikowanie proD365ości klienta w celu zakupienia finansów i operacji.  Klienci, którzy wyświetlają sugestie dotyczące języka F&O, będą znajdować się w najważniejszych niezarządzanych kategoriach. Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|D365FOFit| Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowywanie oceniania przy użyciu modelu podobny do najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne dla Microsoft Cloud produktów. Punktacja jest aktualizowana kwartalnie.|
|D365FOIntent|  Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie intencji jest nadmiarowe w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc.|
|D365CECluster| Pozwala to zidentyfikować proD365 klienta w celu zakupu.  Klienci, którzy wyświetlają pióro dla CE, będą w średnich i małych kategoriach.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|D365CEFit| Dopasuj do D365 CE|
|D365CEIntent|  Zamierzenie dla D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Wskazuje, czy klient ma otwarte odnowienie dla usługi Dynamics on-Premium AX lub CRM.|
|M365UpsellCustomer|    Ta wartość określa, czy klient pokazuje niesprzedawaną M365|
|Ma Google|    Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów firmy Google|
|Ma AWS|   Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów AWS|
|Ma EA |Ta wartość określa, czy odnowienie jest umową Enterprise Agreement (EA), czy z subskrypcją EA|
|Ma otwarte|  Wskazuje to, czy odnowienie jest umową Open Value, czy otwartą|

Poszczególni **Ascent-Azure w chmurze**: definicje danych różnych pól w programie Cloud Ascent-Azure raport o zamiarach:

|**Nazwa kolumny** |**Opis danych** |
|---------|:---------|
|Identyfikator MPN|    Identyfikator Microsoft Partner Network|
|Nazwa partnera|  Nazwa partnera|
|Customer ID|   Numer identyfikacyjny klienta |
|Numer DUNS|   & Dun Bradstreet numer klienta ocenianego dla pozostałej części|
|Nazwa konta|  Nazwa konta |
|Domena|    Domena konta|
|Rozmiar organizacji|  Rozmiar organizacji|
|Branża|  Branża  |
|Pionowa|  Pionowy klient, którego wynikiem jest ocena, zgodnie z opisem przez firmę Microsoft i inne standardy branżowe (D&B)|
|Obszar|  Obszar geograficzny lokalizacji|
|Przedstawicielstwo|    Dotacja dla klienta będącego wynikiem oceny|
|Sales Territory (Obszar sprzedaży)|   Sales Territory (Obszar sprzedaży)|
|City (Miasto)|  Lokalizacja geograficzna |
|Stan| Lokalizacja stanu geograficznego|
|Postal Code|   Postal Code|
|Kraj|   Lokalizacja kraju geograficznego |
|Segment|   Segment rynku |
|Segment podrzędny|   Segment podrzędny rynku |
|Podsumowanie typu SMC|  Typ SMC |
|Najwyższe niezarządzane — podstawa obliczeń|  Najlepsi niezarządzani klienci — obliczenia|
|Najważniejsze niezarządzane — baza użytkowników| Główni niezarządzani klienci — użytkownicy|
|IsNonProfit|   Czy zysk (tak/nie) (tak/nie)|
|Migrowanie-EOS win Server-EOS systemu Windows Server IB z CLAS Pro-5 + licencje|   Klient, który ma EOS na Premium serwera Windows (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma co najmniej 5 licencji. Klient, który ma wynik propióra.  Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie-EOS win Server-EOS systemu Windows Server IB z <CLAS Pro 5 licencji|   Klient, który ma EOS (koniec usługi) na serwerze Premium z systemem Windows (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma mniej niż 5 licencji. Klient, który ma wynik propióra.  Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — EOS win Server-EOS Windows Server IB bez CLAS |Klient, który ma EOS na Premium serwera Windows (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma więcej niż 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — EOS win Server-EOS Windows Server IB bez CLAS — <5 licencji|    Klient, który ma EOS na Premium serwera Windows (czyli wersje, które są starsze niż i obejmują produkty EOS). Ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie-EOS SQL-EOS SQL Server IB z CLAS Pro-5 licencji|  Klient, który ma EOS na Premium SQL Server (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma 5 licencji. Klient ma wynik.  Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie-EOS SQL-EOS SQL Server IB z CLAS propiórą — <5 licencji|  Klient, który ma EOS na Premium SQL Server (czyli wersje, które są starsze niż i obejmują produkty EOS). Ma mniej niż 5 licencji. Klient, który ma wynik propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie-EOS SQL-EOS SQL Server IB bez CLAS|   Klient, który ma EOS na Premium SQL Server (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma co najmniej 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie-EOS SQL-EOS SQL Server IB bez CLAS — <5 licencji|   Klient, który ma EOS na Premium SQL Server (czyli wersje, które są starsze niż i obejmują produkty EOS). Klient ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie na serwerze Premium win — bieżący system Windows Server IB z CLAS propiórami-5 + licencje|   Klient, który ma bieżący Premium serwer win, czyli wersje, które są po EOS produktów. Klient ma 5 licencji. Klient ma wynik. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie na serwerze Premium z programem Windows Server — bieżący serwer IB z CLAS Pro<5 licencji|   Klient, który ma bieżący Premium serwer win, czyli wersje, które są po EOS produktów. Klient ma mniej niż 5 licencji. Klient ma ocenę dla systemu Azure. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie na serwerze Premium win — bieżący system Windows Server IB bez CLAS Pro-5 licencji|    Klient, który ma bieżący Premium serwer win, czyli wersje, które są po EOS produktów. Klient ma 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie na serwerze Premium win — bieżący system Windows Server IB bez CLAS <5 licencji |Klient, który ma bieżący Premium serwer win, czyli wersje, które są po EOS produktów. Klient ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL — bieżąca SQL Server IB z CLASością-5 + licencje|  Klient, który ma bieżące Premium SQL Server (czyli wersje, które są po EOS produktów). Klient ma 5 licencji. Klient ma wynik. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL — bieżąca SQL Server IB z CLAS propiórem — <5 licencji|  Klient, który ma bieżące Premium SQL Server (czyli wersje, które są po EOS produktów). Klient ma mniej niż 5 licencji. Klient ma wynik. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL — bieżąca SQL Server IB bez poCLASów-5 licencji|   Klient, który ma bieżące Premium SQL Server (czyli wersje, które są po EOS produktów). Klient ma 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL — bieżąca SQL Server IB bez poCLASch — <5 licencji|   Klient, który ma bieżące Premium SQL Server (czyli wersje, które są po EOS produktów). Klient ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — OSS — Migrowanie do usługi OSS DB| Istniejący klient z jednym z następujących produktów konkurencyjnych: PostgreSQL, MySQL, MariaDB. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — OSS-Linux na platformie Azure |Istniejący klient z produktem: Linux. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie oprogramowania SAP — SAP na platformie Azure|  Istniejący klient z produktem: SAP. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie-WVD-RDS IB |Identyfikuje klientów z aktywnym Usługi pulpitu zdalnego systemu Windows. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — WVD — sprzedaż w wielu różnych firmach do platformy Azure/WVD|   Identyfikuje klientów w programie M365 i nie ma platformy Azure. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — VMware IB|   Istniejący klient z produktem: VMware. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Migrowanie — Citrix IB|   Istniejący klient z produktem: Citrix Systems. Partnerzy powinni kierować tych klientów do migracji na platformę Azure.|
|Innowacje-Analytics-Power BI IB z/wysoką prozach platformy Azure|   Klienci z subskrypcją usługi Power BI i aktywnymi subskrypcjami, w tym: Power BI — Autonomiczne pakiety Pro, Power BI-Azure, Power BI-Office Suite, Power BI Suites-M365|
|Enable-DevOps z usługą GitHub-VisualStudio/MSDN IB|    Zidentyfikowani klienci z aktywną wizualizacją Studios|
|System Windows Server w wersji Standard|   Spowoduje to wyświetlenie wersji systemu Windows Server Standard zakupy przez klienta|
|Licencja systemu Windows Server Standard|   W tym polu jest wyświetlany typ licencji zakupu systemu Windows Server Standard dla klienta|
|Wersja centrum danych systemu Windows Server|    Spowoduje to wyświetlenie wersji programu Windows Data Center zakupy przez klienta|
|Licencja na centrum danych systemu Windows Server| W tym polu jest wyświetlany typ licencji dla zakupów centrum danych systemu Windows przez klienta|
|AzureFit|  Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowywanie oceniania przy użyciu modelu podobny do najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne dla Microsoft Cloud produktów. Punktacja jest aktualizowana kwartalnie.|
|AzureIntent|   Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie intencji jest nadmiarowe w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc.|
|AzureCluster|  Pozwala to zidentyfikować prowidoczność klienta w celu zakupu platformy Azure, konsolidując zalecenia dotyczące dopasowania i celu do klastra.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|WindowsServerDataCenter_HasOpenRenewal|    Wskazuje, czy klient ma otwarte odnowienie dla centrum danych systemu Windows Server|
|WindowsServerStandard_HasOpenRenewal|  Wskazuje, czy klient ma otwarte odnowienie dla systemu Windows Server Standard|
|AzureUpsellCustomer|   Wskazuje to, czy klient pokazuje niesprzedażowe pióro dla platformy Azure|
|Ma Google|    Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów firmy Google|
|Ma AWS|   Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów AWS|
|Ma EA |Ta wartość określa, czy odnowienie jest umową Enterprise Agreement (EA), czy z subskrypcją EA|
|Ma otwarte|  Wskazuje to, czy odnowienie jest umową Open Value, czy otwartą|

Liczba **Odnowień Ascent-Agreement w chmurze**: definicje danych różnych pól w ramach umowy dotyczącej wzwyższego poziomu w chmurze:

|**Nazwa kolumny** |**Opis danych** |
|---------|:---------|
|Identyfikator MPN|    Identyfikator Microsoft Partner Network|
|Nazwa partnera|  Nazwa partnera|
|Customer ID|   Numer identyfikacyjny klienta |
|Numer DUNS|   & Dun Bradstreet numer klienta ocenianego dla pozostałej części|
|Nazwa konta|  Nazwa konta |
|Domena|    Domena konta|
|Rozmiar organizacji|  Rozmiar organizacji|
|Branża|  Branża  |
|Pionowa|  Pionowy klient, którego wynikiem jest ocena, zgodnie z opisem przez firmę Microsoft i inne standardy branżowe (D&B)|
|Obszar|  Obszar geograficzny lokalizacji|
|Przedstawicielstwo|    Dotacja dla klienta będącego wynikiem oceny|
|Sales Territory (Obszar sprzedaży)|   Sales Territory (Obszar sprzedaży)|
|City (Miasto)|  Lokalizacja geograficzna |
|Stan| Lokalizacja stanu geograficznego|
|Postal Code|   Postal Code|
|Kraj|   Lokalizacja kraju geograficznego |
|Segment|   Segment rynku |
|Segment podrzędny|   Segment podrzędny rynku |
|Podsumowanie typu SMC|  Typ SMC |
|Najwyższe niezarządzane — podstawa obliczeń|  Najlepsi niezarządzani klienci — obliczenia|
|Najważniejsze niezarządzane — baza użytkowników| Główni niezarządzani klienci — użytkownicy|
|IsNonProfit|Czy zysk (tak/nie) (tak/nie)|
|Ma Google|Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów AWS|
|Ma AWS|Ta flaga określa, czy klient przedstawia sygnały konkurencyjne dla produktów AWS|
|Klaster platformy Azure|Umożliwia to zidentyfikowanie prowiedzy o zakupie klienta platformy Azure.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|Klaster D365 F&O|  Umożliwia to zidentyfikowanie proD365ości klienta w celu zakupienia finansów i operacji.  Klienci, którzy wyświetlają sugestie dotyczące języka F&O, będą znajdować się w najważniejszych niezarządzanych kategoriach.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|Klaster D365 CE|   Pozwala to zidentyfikować proD365 klienta w celu zakupu.  Klienci, którzy wyświetlają pióro dla CE, będą w średnich i małych kategoriach.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|Klaster D365 BC|   Umożliwia to zidentyfikowanie proD365ów klienta do zakupu programu Business Central.  Klienci, którzy wyświetlają pióro dla BC, będą w średnich i małych kategoriach.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|Klaster M365|  Umożliwia to zidentyfikowanie proM365ów klienta do zakupu.  Klastry działają teraz i powinny być przeznaczone do produkcji, gdy będą one miały wyższy plon.  Informacyjna i informowanie klientów powinna być ukierunkowana tylko w przypadku, gdy istnieje jeszcze możliwość wykonania działania i ocenienia klientów.|
|Program licencjonowania|   Identyfikuje typ programu licencjonowania dla odnowienia|
|Identyfikator umowy|  Identyfikator umowy|
|Data zakończenia umowy|    Data zakończenia umowy |
|Typ wygaśnięcia|   Typ wygaśnięcia|
|Przychód z tytułu wygaśnięcia|  Przychód skojarzony z wygasanymi subskrypcjami|
|Ma EA|    Ta wartość określa, czy odnowienie jest umową Enterprise Agreement (EA), czy z subskrypcją EA|
|Ma otwarte|  Wskazuje to, czy odnowienie jest umową Open Value, czy otwartą|
|Klient do sprzedaży na platformie Azure| Wskazuje to, czy klient pokazuje niesprzedażowe pióro dla platformy Azure|
|M365 klienta|  Ta wartość określa, czy klient pokazuje niesprzedawaną M365|
|RevSumDivisionName|    Identyfikuje produkt, który jest przeznaczony do odnowienia|

## <a name="next-steps"></a>Następne kroki

Raporty znajdują się w temacie [Download Reports](pci-download-reports.md).
