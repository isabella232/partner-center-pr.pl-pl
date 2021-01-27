---
title: Definicje danych analiz
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: W dokumencie wymieniono różne raporty i ich definicje, które można pobrać z strony raportu pobieranie szczegółowych informacji.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861397"
---
# <a name="export--data-definitions"></a>Eksportowanie — definicje danych 

 **Odpowiednie role** 

- Podgląd raportów 
- Executive — Podgląd raportów 

## <a name="introduction"></a>Wprowadzenie 

Za pomocą Centrum raportów pobierania na pulpicie nawigacyjnym usługi Insights można wyeksportować pierwotne zestawy danych. 

Różne raporty, które można pobrać wraz z ich definicjami danych, są wymienione w następujących tabelach: 

### <a name="partner-profile-report"></a>**Raport profilu partnera**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| MPNId | Identyfikator Microsoft Partner Network (MPN) | 
| PartnerName | Nazwa partnera | 
| PGA_MPNId | Identyfikator konta globalnego partnera MPN | 
| PGA_PartnerName | Nazwa konta globalnego partnera | 
| City (Miasto) | Lokalizacja miasta partnera | 
| Country (Kraj) | Lokalizacja kraju partnera | 
| HierarchyLevel | Wskazuje, czy jest to globalny identyfikator MPN, czy lokalizacja MPN | 

### <a name="customer-details-report"></a>**Raport szczegóły klienta**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| CustomerSegment | Segment klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| CustomerStatus | Stan klienta (aktywny lub nieaktywny) | 
| Produkt | Produkt sprzedawany klientowi przez MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI lub Microsoft Azure | 
| SKU | Jednostka SKU produktu | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie i przychód | 
| MPNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja geograficzna partnera | 
| PartnerAttributionType | Typ przypisania partnera | 
| SalesChannel | Kanał sprzedaży | 
| AvailableSeats | Dostępne stanowiska | 
| RevenueUSD | Przychód w dolarach amerykańskich | 

### <a name="reseller-performance-report"></a>**Raport o wydajności odsprzedawcy**

> [!Note]
> Dane dotyczące przychodów i ACR są dostępne tylko dla użytkowników, którzy są użytkownikami programu Executive w raportach.

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| ResellerMPNid | Identyfikator Microsoft Partner Network odsprzedawcy | 
| ResellerName (Nazwa odsprzedawcy) | Nazwa odsprzedawcy | 
| ResellerMarket | Kraj odsprzedawcy | 
| IndirectProviderMPNId | Identyfikator Microsoft Partner Network dostawcy pośredniego | 
| IndirectProviderName | Nazwa dostawcy pośredniego | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie i przychód | 
| Produkt | Nazwa produktu | 
| Identyfikator | Identyfikator subskrypcji | 
| AvailableSeats | Liczba dostępnych stanowisk | 
| AssignedSeats | Liczba przypisanych stanowisk | 
| BilledRevenueUSD | Przychód rozliczany w dolarach amerykańskich | 
| CustomerName | Nazwa klienta | 
| CustomerTPid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| CustomerSegment | Segment klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| ResellerStatus | Stan odsprzedawcy | 

### <a name="subscription-details-report"></a>**Raport szczegóły subskrypcji**

>[!Note]
>Dane dotyczące przychodów i ACR są dostępne tylko dla użytkowników, którzy są użytkownikami programu Executive w raportach.

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data końcowa subskrypcji | 
| SubscriptionState | Stan subskrypcji (aktywny lub zmieniony) | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie i przychód | 
| IsAutoRenew | Wskazuje, czy subskrypcja jest autoodnawiana (tak lub nie) | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator GUID klienta | 
| CustomerTpid | Górny identyfikator elementu nadrzędnego klienta | 
| CustomerSegment | Segment rynku klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| Produkt | Produkt sprzedawany klientowi przez partnera | 
| SKU | Jednostka SKU produktu | 
| MPNId | Identyfikator Microsoft Partner Network partnera | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja geograficzna partnera | 
| PartnerAttributionType | Typ przypisywania dla subskrypcji | 
| SalesChannel | Kanał dostawcy rozwiązań Sales-Direct, CSP (w chmurze) i tak dalej | 
| AvailableSeats | Bieżące dostępne stanowisko | 
| RevenueUSD | Przychód w dolarach amerykańskich | 
| Identyfikator rejestracji | Identyfikator rejestracji subskrypcji | 

### <a name="azure-usage-report"></a>**Raport użycia platformy Azure**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data końca subskrypcji | 
| SubscriptionState | Bieżący stan subskrypcji (otwarty, zamknięty, aktywny lub w okresie prolongaty) | 
| Month (Miesiąc) | Data agregowana według miesiąca | 
| ServiceName | Nazwa usługi platformy Azure | 
| MeterCategory | Nazwa kategorii miernika | 
| UsageUnits | Liczba jednostek, które są używane w cyklu rozliczeniowym | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędnego elementu klienta | 
| CustomerSegment | Segment klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| MPNId | Identyfikator Microsoft Partner Network klienta | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja regionu geograficznego partnera | 
| PartnerAttributionType | Typ przypisania partnera | 
| SalesChannel | Kanał sprzedaży (Direct/CSP, pośredni/CSP, Direct itd.) | 
| ACR_USD | Przychód zużyty na platformie Azure (ACR) w dolarach amerykańskich | 
| Identyfikator rejestracji | Identyfikator rejestracji subskrypcji platformy Azure | 

### <a name="office-365-license-usage-report"></a>**Raport użycia licencji pakietu Office 365**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędnego elementu klienta | 
| Nr obciążenia | Skype dla firm, zespoły, Exchange Online | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie | 
| PaidAvailableUnits | Liczba płatnych jednostek | 
| MonthlyActiveUsers | Liczba aktywnych użytkowników miesięcznie | 
| CustomerName | Nazwa klienta | 
| CustomerMarket | Geograficzna lokalizacja kraju klienta | 
| CustomerSegment | Segment klienta | 
| MPNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja geograficzna partnera | 
| PartnerAttributionType | Typ przypisania partnera | 

### <a name="enterprise-mobility-license-usage-report"></a>**Raport użycia licencji pakietu Enterprise Mobility**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędnego elementu klienta | 
| Nr obciążenia | Nazwa obciążenia Enterprise Mobility + Securityowego (EMS) | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie | 
| PaidAvailableUnits | Liczba płatnych jednostek | 
| MonthlyActiveUsers | Liczba aktywnych użytkowników miesięcznie | 
| CustomerName | Nazwa klienta | 
| CustomerMarket | Geograficzna lokalizacja kraju klienta | 
| CustomerSegment | Segment klienta | 
| MPNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja geograficzna partnera | 
| PartnerAttributionType | Typ przypisania partnera | 

### <a name="dynamics-365-license-usage-report"></a>**Raport użycia licencji systemu Dynamics 365**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data końcowa subskrypcji | 
| SubscriptionStatus | Stan subskrypcji | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie | 
| RevSumDivisionName | Nazwa podziału sumy Rev. | 
| RevSumCategoryName | Nazwa kategorii sum Rev | 
| SKU | Jednostka SKU produktu | 
| Identyfikatora skuId | Identyfikator jednostki SKU produktu | 
| FreeVsPaidSKU | Wskazuje, czy jest to bezpłatna czy płatna jednostka SKU | 
| SalesModel | Kanał sprzedaży używany do sprzedaży subskrypcji | 
| DetailedSalesModel | Szczegółowy model sprzedaży dla subskrypcji | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator GUID dzierżawy klienta | 
| CustomerTpid | Górny identyfikator elementu nadrzędnego klienta | 
| CustomerSegment | Segment rynku klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| MPNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja regionu geograficznego partnera | 
| PartnerAttachType | Typ przypisywania dla subskrypcji | 
| AvailableSeats | Bieżące dostępne stanowisko | 
| AssignedSeats | Bieżące przypisane miejsce | 
| ActiveSeats | Bieżące aktywne stanowiska | 
| DeploymentOpportunity | Bieżąca szansa sprzedaży wdrożenia | 
| ActiveUsagePercent | Bieżące aktywne procenty użycia | 

### <a name="power-bi-license-usage-report"></a>**Raport użycia licencji Power BI**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data końcowa subskrypcji | 
| SubscriptionStatus | Stan subskrypcji (aktywny, nieaktywny lub w okresie prolongaty) | 
| Month (Miesiąc) | Data agregowana według miesiąca | 
| SKU | Jednostka SKU produktu | 
| Identyfikatora skuId | Identyfikator jednostki SKU produktu | 
| FreeVsPaidSKU | Bezpłatny lub płatny rozróżnienie jednostki SKU | 
| SalesModel | Model sprzedaży używany do sprzedaży subskrypcji | 
| DetailedSalesModel | Szczegółowy model sprzedaży dla subskrypcji | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator GUID dzierżawy klienta | 
| CustomerTpid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| CustomerSegment | Segment rynku klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| MPNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja regionu geograficznego partnera | 
| PartnerAttachType | Typ przypisywania dla subskrypcji | 
| AvailableSeats | Bieżące dostępne stanowiska | 
| AssignedSeats | Aktualnie przypisane stanowiska | 
| ActiveSeats | Bieżące aktywne stanowiska | 
| DeploymentOpportunity | Bieżąca szansa sprzedaży wdrożenia | 
| ActiveUsagePercent | Bieżące aktywne procenty użycia | 

### <a name="teams-meetings-and-calls-report"></a>**Raporty dotyczące spotkań i wywołań zespołów**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie | 
| Obciążanie | Obciążanie, dla którego zgłaszane jest użycie (spotkania, wywołania lub systemy telefoniczne) | 
| Liczba spotkań | Liczba spotkań | 
| Czas trwania spotkania | Łączny czas trwania spotkań w godzinach | 

### <a name="teams-monthly-usage-report"></a>**Raport dotyczący miesięcznego użycia zespołów**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie | 
| Obciążanie | Obciążanie, dla którego zgłaszane jest użycie (spotkania, wywołania lub systemy telefoniczne) | 
| Użytkownicy komputerów stacjonarnych | Liczba użytkowników, którzy korzystają z zespołów na komputerze | 
| Użytkownicy mobilni | Liczba użytkowników, którzy korzystają z zespołów na urządzeniach przenośnych | 
| Użytkownicy sieci Web | Liczba użytkowników, którzy korzystają z zespołów w sieci Web | 
| AllUpParticipants | Liczba unikatowych użytkowników zespołów w miesiącu | 

### <a name="teams-usage-3p-apps-report"></a>**Raport dotyczący użycia zespołów 3P Apps**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędnego elementu klienta | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane jest użycie | 
| Nazwa aplikacji 3P | Nazwa aplikacji Teams | 
| Liczba użytkowników | Liczba użytkowników aplikacji | 


### <a name="training-details-report"></a>**Raport szczegóły szkolenia**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| TrainingActivityId | Identyfikator szkolenia | 
| TrainingTitle | Tytuł szkolenia | 
| Szkolenietype | Typ szkolenia (certyfikacja lub egzamin) | 
| IndividualFirstName | Imię klienta | 
| IndividualLastName | Nazwisko klienta | 
| E-mail | Osobisty identyfikator poczty e-mail klienta | 
| CorpEmail | Identyfikator poczty e-mail klienta | 
| TrainingCompletionDate | Data ukończenia szkolenia | 
| Month (Miesiąc) | Miesiąc, dla którego są zgłaszane dane | 
| IcMCP | Wskazuje, czy użytkownik jest użytkownikiem z certyfikatem Microsoft Certified Professional (MCP) | 
| MCPID | IDENTYFIKATOR MCP użytkownika | 
| MPNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerCityLocation | Lokalizacja geograficzna partnera | 
| PartnerCountryLocation | Lokalizacja regionu geograficznego partnera | 

### <a name="microsoft-learn-report"></a>**Raport Microsoft Learn**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Nazwa użytkownika | Nazwa użytkownika | 
| UserId | Identyfikator GUID użytkownika | 
| Szkoleniename | Nazwa szkolenia | 
| Szkolenietype | Typ szkolenia (ścieżka modułu lub uczenia) | 
| Produkty | Produkt, dla którego ma zastosowanie moduł uczenia | 
| Role | Odpowiednie role szkoleniowe | 
| CompletionDate | Data ukończenia szkolenia | 
| MPNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| Country (Kraj) | Lokalizacja regionu geograficznego partnera | 

### <a name="competency-summary-and-history-report"></a>**Podsumowanie kompetencji i raport historii**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CompetencyName | Nazwa kompetencji | 
| CompetencyLevel | Poziom kompetencji (złoty lub Silver) | 
| CompetencyStatus | Bieżący stan kompetencji (aktywny, nieaktywny lub w okresie prolongaty) | 
| CompetencyStartDate | Data rozpoczęcia kompetencji | 
| CompetencyEndDate | Data końcowa kompetencji | 

### <a name="competency-performance-report"></a>**Raport o wydajności dotyczącej kompetencji**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CompetencyName | Nazwa kompetencji | 
| CompetencyAttainmentOptionName | Nazwa opcji uzyskania kompetencji | 
| Month (Miesiąc) | Miesiąc, dla którego zgłaszane są metryki | 
| MetricName | Nazwa metryki dotyczącej kompetencji | 
| MetricMonthlyContribution | Miesięczny udział w metryce | 
| TTMAggregate | Zagregowana Metryka na końcowe 12 miesięcy | 
| AnniversaryYearAggregate | Zagregowana Metryka dla bieżącego roku rocznicowego | 
| GoldThreshold | Wymagania dotyczące wydajności w celu spełnienia wymagań w zakresie złota | 
| SilverThreshold | Wymagania dotyczące wydajności w celu spełnienia kompetencji Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Wzniesienie Microsoft 365 w chmurze — raport**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Identyfikator Microsoft Partner Network | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikacyjny klienta | 
| Numer DUNS | Bradstreet Dun & (D&B) numer klienta, który jest przeznaczony do oceny | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża, do której należy organizacja | 
| Pionowa | Pionowy dla klienta, który jest przeznaczony do oceny dla osób, określonych przez firmę Microsoft, D&B i inne standardy branżowe | 
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Oddział klienta, który jest przeznaczony do oceny | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży dla klienta, który jest przeznaczony do oceny | 
| City (Miasto) | Lokalizacja geograficzna organizacji | 
| Stan | Lokalizacja stanu geograficznego organizacji | 
| Postal Code | Kod pocztowy organizacji | 
| Country (Kraj) | Lokalizacja regionu geograficznego organizacji | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegment rynku | 
| Podsumowanie typu SMC | Typ SMC | 
| Najwyższe niezarządzane — podstawa obliczeń | Najlepsi niezarządzani klienci — obliczenia | 
| Najważniejsze niezarządzane — baza użytkowników | Główni niezarządzani klienci — użytkownik | 
| IsNonProfit | Wskazuje, czy organizacja nie ma zysku (tak lub nie) | 
| Włącz zdalną służbę — docelowa usługa Exchange Online | Klienci z aktywną subskrypcją usługi Exchange Online, która jest sprzedawana do Microsoft 365 | 
| Włącz zdalne pozyskiwanie w chmurze (aktualna wersja) z założeniami o wzniesieniu do chmury-+ 10 licencji | Klient, który ma aktualny lokalny pakiet biurowy lub klienta systemu Windows. Oznacza to, że wersja klienta jest późniejsza niż wersja końcowa (EOL). Klient ma co najmniej 10 licencji. Klient, który ma wynik propióra. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalne pozyskiwanie w chmurze (bieżąca wersja) z niezależnością od chmury — <10 licencji | Klient korzystający z bieżącego lokalnego klienta lub systemu Windows (czyli wersji nowszej niż EOL). Klient ma mniej niż 10 licencji. Klient, który ma wynik propióra. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalne pozyskiwanie w miejscu pracy (bieżąca wersja) bez poniesień w chmurze — + 10 licencji | Klient korzystający z bieżącego lokalnego klienta lub systemu Windows (czyli wersji nowszej niż EOL). Klient ma co najmniej 10 licencji. Klient nie ma wyniku propióra. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalne pozyskiwanie w chmurze (aktualna wersja) bez pomieszczeń z założeniami chmury — <10 licencji | Klient korzystający z bieżącego lokalnego klienta lub systemu Windows (czyli wersji nowszej niż EOL). Klient ma mniej niż 10 licencji. Klient nie ma wyniku propióra. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalne pozyskiwanie w chmurze (wersja EOL) z założeniami o wzniesieniu do chmury-+ 10 licencji | Klient, który ma EOL lokalnego lub klienta systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma co najmniej 10 licencji. Klient ma wynik. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalne pozyskiwanie w chmurze (wersja EOL) z niezależnością od chmury — <10 licencji | Klient, który ma EOL lokalnego lub klienta systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma mniej niż 10 licencji. Klient ma wynik. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalne pozyskiwanie w miejscu pracy (wersja EOL) bez poniesień w chmurze — + 10 licencji | Klient korzystający z bieżącego lokalnego klienta lub systemu Windows (czyli wersji EOL lub starszej). Klient ma co najmniej 10 licencji. Klient nie ma wyniku propióra. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalne pozyskiwanie w miejscu pracy (wersja EOL) bez poniesień w chmurze — <10 licencji | Klient korzystający z bieżącego lokalnego klienta lub systemu Windows (czyli wersji EOL lub starszej). Klient ma mniej niż 10 licencji. Klient nie ma wyniku propióra. Partner powinien być celem konwersji do Microsoft 365. | 
| Włącz zdalną i wysoką perspektywę dla Microsoft 365 (ACT NowithEvaluate) | Potencjalni klienci z wysoką perspektywą dla Microsoft 365 | 
| Włącz zdalną współpracę — konkurowanie (powiększanie) za pomocą Microsoft 365 | Klient z powiększaniem i Microsoft 365, cel konwersji na zespoły | 
| Włącz zdalną współpracę — konkurowanie (powiększanie) bez Microsoft 365 | Klient z powiększeniem, cel konwersji na zespoły | 
| Obniżanie kosztów i zarządzanie Microsoft 365 E3 dla Microsoft 365 E5 | Istniejący klient z Microsoft 365 E3, cel dla Microsoft 365 E5 | 
| Obniżanie kosztów i zarządzanie Microsoft 365 Business klientami standardowymi i biznesowymi przeznaczonymi dla Microsoft 365 Business Premium | Istniejący klienci korzystający z usługi Microsoft 365 Business Basic i Business Standard, Target for Microsoft 365 Business Premium | 
| Przekształcanie produktywności organizacyjnej — pióra powierzchni | Klient pokazuje propióra powierzchni | 
| M365Cluster | Pozwala zidentyfikować proMicrosoft 365 klientów w celu zakupu. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko, gdy nadal jest dostępna wydajność i Oceń klientów. | 
| M365Fit | Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Funkcja określania rozmiaru jest zgodna z modelem Lookalike do naszych najlepszych i średnich firm (technologii) w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne w przypadku produktów w chmurze firmy Microsoft. Punktacja jest aktualizowana kwartalnie. | 
| M365Intent | Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie zamiaru jest przełożone w celu dopasowania do definiowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| SurfaceCluster | Określa promyślną ofertę klienta, aby zakupić powierzchnię przez skonsolidowanie zaleceń dotyczących dopasowania i celu do klastra. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko, gdy nadal jest dostępna wydajność i Oceń klientów. | 
| SurfaceFit | Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowanie do oceniania korzysta z modelu Lookalike do naszych najlepszych technologii w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne w przypadku produktów w chmurze firmy Microsoft. Punktacja jest aktualizowana kwartalnie. | 
| SurfaceIntent | Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie zamiaru jest przełożone w celu dopasowania do definiowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| O365Cluster | Określa propióra klienta dotyczące zakupu pakietu Office 365. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko, gdy nadal jest dostępna wydajność i Oceń klientów. | 
| O365Fit | Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowanie do oceniania korzysta z modelu Lookalike do naszych najlepszych technologii w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne w przypadku produktów w chmurze firmy Microsoft. Punktacja jest aktualizowana kwartalnie. | 
| O365Intent | Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie zamiaru jest przełożone w celu dopasowania do definiowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| M365UpsellCustomer | Określa, czy klient ma pokazywanie pozostałej dla Microsoft 365 | 
| Ma Google | Określa, czy klient ma wyświetlać sygnały konkurencyjne dla produktów firmy Google | 
| Ma AWS | Określa, czy klient ma wyświetlać sygnały konkurencyjne na potrzeby produktów Amazon Web Services (AWS) | 
| Ma EA | Określa, czy odnowienie jest umową Enterprise Agreement (EA), czy z subskrypcją EA | 
| Ma otwarte | Określa, czy odnowienie jest umową Open lub Open Value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Doniesienie do chmury — Raport z propióry dla systemu Dynamics 365**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Identyfikator Microsoft Partner Network | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikacyjny klienta | 
| Numer DUNS | & Dun Bradstreet numer klienta, który jest przeznaczony do oceny | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża, do której należy organizacja | 
| Pionowa | Pionowy dla klienta, który jest przeznaczony do oceny dla osób, określonych przez firmę Microsoft, D&B i inne standardy branżowe
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Oddział klienta, który jest przeznaczony do oceny | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży dla klienta, który jest przeznaczony do oceny | 
| City (Miasto) | Lokalizacja geograficzna | 
| Stan | Lokalizacja stanu geograficznego | 
| Postal Code | Kod pocztowy organizacji | 
| Country (Kraj) | Lokalizacja kraju geograficznego | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegment rynku | 
| Podsumowanie typu SMC | Kategoryzacja klienta: najważniejsze niezarządzane bazy użytkowników są klientami z ponad 300 pracownikami, a najwyższe niezarządzane bazy obliczeniowe są klientami z USD10ą, 1000 na platformie Azure. w przypadku małych firm klienci mają 25 pracowników lub więcej, a małe firmy są klientami z mniej niż 25 pracownikami. | 
| Najwyższe niezarządzane — podstawa obliczeń | Najlepsi niezarządzani klienci — obliczenia | 
| Najważniejsze niezarządzane — baza użytkowników | Główni niezarządzani klienci — użytkownicy | 
| IsNonProfit | Wskazuje, czy organizacja nie ma zysku (tak lub nie) | 
| Aktywuj sprzedawanie cyfrowe — rozmiar Microsoft 365 miejsca >= 25 siedzeń (model propozycji SalesPro) | Klient bez systemu Dynamics 365. Rozmiar miejsca: 25 i. Partner powinien mieć miejsce docelowe w przypadku usługi Dynamics 365 SalesPro. | 
| Aktywuj sprzedawanie cyfrowe — Dynamics 365 SalesPro (wykonaj teraz lub Oceń) | Klienci z wysokim poziomem liter bez systemu Dynamics 365. Partner powinien mieć cel dla systemu Dynamics 365 SalesPro. | 
| Zarządzanie ryzykiem finansowym & oszustw — podstawowa instalacja w ramach systemu Dynamics | Istniejący klient z lokalnym systemem Navision. Partner powinien kierować do usługi Dynamics 365 Business Central. | 
| Zarządzanie ryzykiem finansowym & oszustw — lokalna instalacja podstawowa — Dynamics AX (Dynamics 365 finansów + model operacji) | Istniejący klient z lokalnym systemem AX. Partner powinien kierować do usługi Dynamics 365 finanse + Operations. | 
| Zarządzanie ryzykiem finansowym & oszustw — podstawowa instalacja systemu Dynamics — doskonałe zwykłe (model biznesowy) | Istniejący klient z lokalnymi doskonałymi lokalizacjami. Partner powinien kierować do usługi Dynamics 365 Business Central. | 
| Zarządzanie ryzykiem finansowym & oszustw — lokalna instalacja systemu Dynamics (podstawowa) | Istniejący klient z lokalną Wyspyem Salomona. Partner powinien kierować do usługi Dynamics 365 Business Central. | 
| Zarządzanie ryzykiem finansowym & oszustw — podstawowa instalacja w ramach systemu Dynamics | Istniejący klient z innymi rozwiązaniami lokalnymi, które nie zostały wcześniej wymienione. Partner powinien kierować do usługi Dynamics 365 Business Central. | 
| Tworzenie procesów biznesowych Agile — podstawowa instalacja systemu Dynamics AX/GP/SL/Nawigacja/inne (model propióra Dynamics 365) | Tworzenie procesów biznesowych Agile — podstawowa instalacja systemu Dynamics AX/GP/SL/Nawigacja/inne (model propióra Dynamics 365) | 
| Tworzenie procesów biznesowych Agile — podstawy konkurowania — Mendix/Systems/Salesforce (model proości Dynamics 365) | Tworzenie procesów biznesowych Agile — podstawy konkurowania — Mendix/Systems/Salesforce (model proości Dynamics 365) | 
| Tworzenie procesów biznesowych Agile — Dynamics 365 finansów + Operations Base | Istniejący klienci programu Dynamics 365 Finanse i Operations Manager. Partner na aplikacje docelowe. | 
| Kompiluj procesy biznesowe Agile — baza instalacji systemu Dynamics 365 Business Central | Istniejący klienci programu Dynamics 365 Business Central. Partner na aplikacje docelowe. | 
| Kompiluj procesy biznesowe Agile — baza instalacji dla systemu Dynamics 365 klienta | Istniejący klienci korzystający z systemu Dynamics 365. Partner na aplikacje docelowe. | 
| Tworzenie łańcucha dostaw odpornych na awarie — Windows i aktywowanie pierwszego obciążenia Dynamics 365 jako zarządzania łańcuchem dostaw programu Dynamics 365 w przypadku klientów z systemami innym niż Oracle lub SAP ERP (planowanie zasobów przedsiębiorstwa) | Klienci docelowi do zarządzania łańcuchem dostaw w usłudze Dynamics 365 | 
| Twórz odporny na awarie 365 łańcuch dostaw, zarządzanie łańcuchem dostaw i/lub handel detaliczny w usłudze Dynamics 365 | Istniejący klienci w ramach programu Dynamics 365, którzy mają być zaangażowani w zarządzanie łańcuchem dostaw do sprzedaży w ramach usługi Dynamics 365. | 
| Utwórz łańcuch dostaw odporny na sprzedaż w różnych 365 sklepach — Zarządzanie łańcuchem dostaw i/lub handel detaliczny i handlowe w usłudze Dynamics 365 Customer Engagement i Oracle lub SAP | Obecni klienci korzystający z rozwiązania Dynamics 365 dla klientów z oprogramowaniem Oracle lub SAP do celów zarządzania łańcuchem dostaw systemu Dynamics 365 | 
| D365BCCluster | Określa propióra klienta do zakupu Dynamics 365 Business Central. Klienci, którzy wyświetlają propióra dla programu Business Central, będą w średnich i małych kategoriach. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| D365BCFit | Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowanie do oceniania korzysta z modelu Lookalike do naszego najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne w przypadku produktów w chmurze firmy Microsoft. Punktacja jest aktualizowana kwartalnie. | 
| D365BCIntent | Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie zamiaru jest przełożone w celu dopasowania do definiowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| D365FOCluster | Określa propióra klienta do zakupu systemu Dynamics 365 Finanse i operacje. Klienci, którzy wyświetlają propióra dla finansów i operacji, będą znajdować się w najważniejszych niezarządzanych kategoriach. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| D365FOFit | Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowanie do oceniania korzysta z modelu Lookalike do naszego najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne w przypadku produktów w chmurze firmy Microsoft. Punktacja jest aktualizowana kwartalnie. | 
| D365FOIntent | Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie zamiaru jest przełożone w celu dopasowania do definiowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| D365CECluster | Określa propióra klienta dotyczące zakupu programu Dynamics 365 Customer Engagement. Klienci, którzy wyświetlają pióro dla zaangażowania klientów, będą w średnich i małych kategoriach. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| D365CEFit | Wskazuje, że jest to dopasowanie do programu Dynamics 365 Customer Engagement | 
| D365CEIntent | Wskazuje zamiar dla programu Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Wskazuje, czy klient ma otwarte odnowienie dla platformy Dynamics lokalnego systemu AX lub CRM | 
| M365UpsellCustomer | Określa, czy klient ma pokazywanie pozostałej dla Microsoft 365 | 
| Ma Google | Określa, czy klient ma wyświetlać sygnały konkurencyjne dla produktów firmy Google | 
| Ma AWS | Określa, czy klient ma wyświetlać sygnały konkurencyjne dla produktów AWS | 
| Ma EA | Określa, czy odnowienie jest subskrypcją EA lub EA | 
| Ma otwarte | Określa, czy odnowienie jest umową Open lub Open Value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Wzniesienie do chmury — raport dotyczący propiór platformy Azure**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Identyfikator Microsoft Partner Network | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikacyjny klienta | 
| Numer DUNS | & Dun Bradstreet numer klienta, który jest przeznaczony do oceny | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża | 
| Pionowa | Pionowy dla klienta, który jest przeznaczony do oceny dla osób, określonych przez firmę Microsoft, D&B i inne standardy branżowe | 
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Oddział klienta, który jest przeznaczony do oceny | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży dla klienta, który jest przeznaczony do oceny | 
| City (Miasto) | Lokalizacja geograficzna | 
| Stan | Lokalizacja stanu geograficznego | 
| Postal Code | Kod pocztowy organizacji | 
| Country (Kraj) | Lokalizacja kraju geograficznego | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegment rynku | 
| Podsumowanie typu SMC | Typ SMC | 
| Najwyższe niezarządzane — podstawa obliczeń | Najlepsi niezarządzani klienci — obliczenia | 
| Najważniejsze niezarządzane — baza użytkowników | Główni niezarządzani klienci — użytkownicy | 
| IsNonProfit | Wskazuje, czy organizacja nie ma zysku (tak lub nie) | 
| Migrowanie-EOL systemu Windows Server EOL z systemem Windows Server IB z założeniami w chmurze — 5 + licencje | Klient, który ma EOL lokalny serwer systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma co najmniej 5 licencji. Klient, który ma wynik propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-EOL systemu Windows Server EOL z systemem Windows Server IB z założeniami w chmurze — <5 licencji | Klient, który ma EOL lokalny serwer systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma mniej niż 5 licencji. Klient, który ma wynik propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-EOL systemu Windows Server — EOL systemu Windows Server IB bez pozostałej do założenia w chmurze — 5 licencji | Klient, który ma EOL lokalny serwer systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma więcej niż 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-EOL systemu Windows Server-EOL systemu Windows Server IB bez założenia w chmurze — <5 licencji | Klient, który ma EOL lokalny serwer systemu Windows (czyli wersję EOL lub wcześniejszą). Ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-EOL SQL-EOL SQL Server IB z założeniami w chmurze — 5 + licencje | Klient, który ma SQL Server lokalnego (czyli wersję EOL lub wcześniejszą). Klient ma 5 licencji. Klient ma wynik. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-EOL SQL-EOL SQL Server IB z założeniami w chmurze — <5 licencji | Klient, który ma SQL Server lokalnego (czyli wersję EOL lub wcześniejszą). Ma mniej niż 5 licencji. Klient, który ma wynik propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-EOL SQL-EOL SQL Server IB bez ponoszonych pod kątem chmury — 5 licencji | Klient, który ma SQL Server lokalnego (czyli wersję EOL lub wcześniejszą). Klient ma co najmniej 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-EOL SQL-EOL SQL Server IB bez założenia w chmurze — <5 licencji | Klient, który ma SQL Server lokalnego (czyli wersję EOL lub wcześniejszą). Klient ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie lokalnego systemu Windows Server — bieżący system Windows Server IB z założeniami w chmurze — 5 + licencje | Klient, który ma bieżący lokalny serwer systemu Windows (czyli wersję nowszą niż EOL). Klient ma 5 licencji. Klient ma wynik. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie lokalnego systemu Windows Server — bieżący system Windows Server IB z niedołożeniami w chmurze — <5 licencji | Klient, który ma bieżący lokalny serwer systemu Windows (czyli wersję nowszą niż EOL). Klient ma mniej niż 5 licencji. Klient ma ocenę dla systemu Azure. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie lokalnego systemu Windows Server — bieżący system Windows Server IB bez ponoszonych pod kątem chmury — 5 licencji | Klient, który ma bieżący lokalny serwer systemu Windows (czyli wersję nowszą niż EOL). Klient ma 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie lokalnego systemu Windows Server — bieżący system Windows Server IB bez podania z założeniami w chmurze — <5 licencji | Klient, który ma bieżący lokalny serwer systemu Windows (czyli wersję nowszą niż EOL). Klient ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL (VM) — bieżąca SQL Server IB z założeniami w chmurze — 5 + licencje | Klient, który ma bieżącą SQL Server lokalną (czyli wersję późniejszą niż EOL). Klient ma 5 licencji. Klient ma wynik. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL — bieżąca SQL Server IB z założeniami w chmurze — <5 licencji | Klient, który ma bieżącą SQL Server lokalną (czyli wersję późniejszą niż EOL). Klient ma mniej niż 5 licencji. Klient ma wynik. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL — bieżąca SQL Server IB bez ponoszonych z chmury — 5 licencji. | Klient, który ma bieżącą SQL Server lokalną (czyli wersję późniejszą niż EOL). Klient ma 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Migrowanie do usługi Azure SQL lub maszyny wirtualne SQL — bieżąca SQL Server IB bez ponoszonych pod kątem chmury — <5 licencji | Klient, który ma bieżącą SQL Server lokalną (czyli wersję późniejszą niż EOL). Klient ma mniej niż 5 licencji. Klient nie ma wyniku propióra. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie-OSS-Migrowanie do bazy danych open source Szekspira (OSS) | Istniejący klient z jednym z następujących produktów konkurencyjnych: PostgreSQL, MySQL, MariaDB. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — OSS-Linux na platformie Azure | Istniejący klient z systemem Linux. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie oprogramowania SAP — SAP na platformie Azure | Istniejący klient z programem SAP. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — pulpit wirtualny systemu Windows — Usługi pulpitu zdalnego IB | Identyfikuje klientów z aktywnym Usługi pulpitu zdalnego systemu Windows. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — pulpit wirtualny systemu Windows — sprzedaż na wiele firm do platformy Azure/WVD | Identyfikuje klientów, którzy mają Microsoft 365 i nie mają platformy Azure. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — VMware IB | Istniejący klient z produktem: VMware. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Migrowanie — Citrix IB | Istniejący klient z produktem: Citrix Systems. Partner powinien kierować tego klienta na potrzeby migracji na platformę Azure. | 
| Innowacje-Analytics-Power BI IB z wysoką pozostałością platformy Azure | Klienci z subskrypcją usługi Power BI i aktywnymi subskrypcjami, w tym: Power BI — Autonomiczne pakiety Pro, Power BI-Azure, Power BI-Office Suite, Power BI Suite-Microsoft 365 | 
| Enable-DevOps z usługą GitHub — Visual Studio/MSDN IB | Identyfikuje klientów z aktywnymi wersjami programu Visual Studio | 
| Wersja Standard systemu Windows Server | Wyświetla wersję systemu Windows Server Standard zakupy dla klienta | 
| Licencja na system Windows Server Standard | Wyświetla typ licencji systemu Windows Server Standard zakupy dla klienta | 
| Wersja centrum danych systemu Windows Server | Wyświetla wersję zakupów centrum danych systemu Windows przez klienta | 
| Licencja centrum danych systemu Windows Server | Wyświetla typ licencji dla zakupów centrum danych systemu Windows przez klienta | 
| AzureFit | Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics. Dopasowanie do oceniania korzysta z modelu Lookalike do naszego najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne w przypadku produktów w chmurze firmy Microsoft. Punktacja jest aktualizowana kwartalnie. | 
| AzureIntent | Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel. Ocenianie zamiaru jest przełożone w celu dopasowania do definiowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| AzureCluster | Określa prowskazówki klienta dotyczące zakupu platformy Azure, konsolidując zalecenia dotyczące dopasowania i celu do klastra. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| WindowsServerDataCenter_HasOpenRenewal | Wskazuje, czy klient ma otwarte odnowienie dla systemu Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Wskazuje, czy klient ma otwarte odnowienie dla systemu Windows Server Standard | 
| AzureUpsellCustomer | Określa, czy klient ma pokazywanie niesprzedaży dla platformy Azure | 
| Ma Google | Określa, czy klient ma wyświetlać sygnały konkurencyjne dla produktów firmy Google | 
| Ma AWS | Określa, czy klient ma wyświetlać sygnały konkurencyjne dla produktów AWS | 
| Ma EA | Określa, czy odnowienie jest subskrypcją EA lub EA | 
| Ma otwarte | Określa, czy odnowienie jest umową Open lub Open Value | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Założenia w chmurze — raport dotyczący odnowień umowy**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Identyfikator Microsoft Partner Network | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikacyjny klienta | 
| Numer DUNS | & Dun Bradstreet numer klienta, który jest przeznaczony do oceny | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża | 
| Pionowa | Pionowy dla klienta, który jest przeznaczony do oceny dla osób, określonych przez firmę Microsoft, D&B i inne standardy branżowe | 
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Oddział klienta, który jest przeznaczony do oceny | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży dla klienta, który jest przeznaczony do oceny | 
| City (Miasto) | Lokalizacja geograficzna | 
| Stan | Lokalizacja stanu geograficznego | 
| Postal Code | Kod pocztowy organizacji | 
| Country (Kraj) | Lokalizacja kraju geograficznego | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegment rynku | 
| Podsumowanie typu SMC | Typ SMC | 
| Najwyższe niezarządzane — podstawa obliczeń | Najlepsi niezarządzani klienci — obliczenia | 
| Najważniejsze niezarządzane — baza użytkowników | Główni niezarządzani klienci — użytkownicy | 
| IsNonProfit | Wskazuje, czy organizacja nie ma zysku (tak lub nie) | 
| Ma Google | Określa, czy klient ma wyświetlać sygnały konkurencyjne dla produktów AWS | 
| Ma AWS | Określa, czy klient ma wyświetlać sygnały konkurencyjne dla produktów AWS | 
| Klaster platformy Azure | Określa propióra klienta dotyczące zakupu platformy Azure. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| D365 Finanse i klaster operacji | Określa propióra klienta do zakupu systemu Dynamics 365 Finanse i operacje. Klienci, którzy wyświetlają propióra dla finansów i operacji, będą znajdować się w najważniejszych niezarządzanych kategoriach. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| Klaster D365 CE | Określa propióra klienta dotyczące zakupu programu Dynamics 365 Customer Engagement. Klienci, którzy wyświetlają pióro dla zaangażowania klientów, będą w średnich i małych kategoriach. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| Klaster D365 BC | Określa propióra klienta do zakupu Dynamics 365 Business Central. Klienci, którzy wyświetlają propióra dla programu Business Central, będą w średnich i małych kategoriach. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| Klaster Microsoft 365 | Umożliwia zidentyfikowanie prowiedzy dla klienta Microsoft 365. Kierowanie teraz i testowanie klastrów, ponieważ spowoduje to wygenerowanie wyższego plonu. Docelowa informacyjna i informowanie klientów tylko wtedy, gdy masz jeszcze możliwość wykonania działania, a następnie Oceń klientów. | 
| Program licencjonowania | Identyfikuje typ programu licencjonowania dla odnowienia | 
| Identyfikator umowy | Identyfikator umowy | 
| Data zakończenia umowy | Data zakończenia umowy | 
| Typ wygaśnięcia | Typ wygaśnięcia | 
| Przychód z tytułu wygaśnięcia | Przychód skojarzony z wygasanymi subskrypcjami | 
| Ma EA | Określa, czy odnowienie jest subskrypcją EA lub EA | 
| Ma otwarte | Określa, czy odnowienie jest umową Open lub Open Value | 
| Klient do sprzedaży na platformie Azure | Określa, czy klient ma pokazywanie niesprzedaży dla platformy Azure | 
| Microsoft 365 klienta w sprzedaży | Określa, czy klient ma pokazywanie pozostałej dla Microsoft 365 | 
| RevSumDivisionName | Identyfikuje produkt, który jest przeznaczony do odnowienia | 

## <a name="next-steps"></a>Następne kroki

Aby uzyskać więcej informacji, zobacz [pobieranie raportów](pci-download-reports.md).
