---
title: Definicje danych analiz
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokument zawiera listę różnych raportów i ich definicji danych, które można pobrać ze strony Pobieranie raportu szczegółowych informacji.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 721caed2d8b0e24940e7adedeb90cc689a82d2e7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152838"
---
# <a name="export--data-definitions"></a>Eksportowanie — definicje danych 

**Odpowiednie role:** Przeglądarka raportów | Przeglądarka raportów dla kierownictwa

## <a name="introduction"></a>Wprowadzenie 

Za pomocą centrum Pobierz raporty na pulpicie nawigacyjnym szczegółowych informacji można wyeksportować nieprzetworzone zestawy danych. 

Różne raporty, które można pobrać wraz z ich definicjami danych, są wymienione w następujących tabelach: 

### <a name="partner-profile-report"></a>**Raport profilu partnera**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| MpNId | Identyfikator Microsoft Partner Network (MPN) | 
| PartnerName | Nazwa partnera | 
| PGA_MPNId | Identyfikator mpn konta globalnego partnera | 
| PGA_PartnerName | Nazwa konta globalnego partnera | 
| City (Miasto) | Lokalizacja miasta partnera | 
| Kraj | Lokalizacja kraju partnera | 
| HierarchyLevel (Poziom hierarchii) | Wskazuje, czy jest to globalny identyfikator MPN, czy identyfikator MPN lokalizacji | 

### <a name="customer-details-report"></a>**Raport Szczegóły klienta**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| CustomerSegment | Segment klientów | 
| CustomerMarket | Rynek geograficzny klienta | 
| CustomerStatus (Statystyka klienta) | Stan klienta (aktywny lub nieaktywny) | 
| Produkt | Produkt sprzedawany klientowi za pomocą programu MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI lub Microsoft Azure | 
| SKU | Product SKU | 
| Month (Miesiąc) | Miesiąc, dla którego raportuje się użycie i przychód | 
| MpNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| Lokalizacja partnera | Lokalizacja geograficzna partnera | 
| Typ PartnerAttributionType | Typ przypisania partnera | 
| SalesChannel | Kanał sprzedaży | 
| Dostępne opcje | Dostępne stanowiska | 
| RevenueUSD | Przychód w dolarach amerykańskich | 

### <a name="reseller-performance-report"></a>**Raport wydajności odsprzedawcy**

> [!Note]
> Przychód i dane ACR są dostępne tylko dla użytkowników, którzy są osobami przeglądacy raportów kierownictwa.

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| ResellerMPNid | Identyfikator Microsoft Partner Network odsprzedawcy | 
| ResellerName (Nazwa odsprzedawcy) | Nazwa odsprzedawcy | 
| ResellerMarket | Reseller country of market (Kraj odsprzedawcy na rynku) | 
| IndirectProviderMPNId | Identyfikator dostawcy pośredniego Microsoft Partner Network | 
| IndirectProviderName | Nazwa dostawcy pośredniego | 
| Month (Miesiąc) | Miesiąc, dla którego jest zgłaszane użycie i przychód | 
| Produkt | Nazwa produktu | 
| Subscriptionid | Identyfikator subskrypcji | 
| DostępneSeats | Liczba dostępnych stanowisk | 
| PrzypisaneSeats | Liczba przypisanych stanowisk | 
| BilledRevenueUSD | Rozliczany przychód w dolarach amerykańskich | 
| CustomerName | Nazwa klienta | 
| CustomerTPid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| CustomerSegment | Segment klientów | 
| CustomerMarket | Rynek geograficzny klienta | 
| ResellerStatus (Statystyka odsprzedawcy) | Stan odsprzedawcy | 

### <a name="subscription-details-report"></a>**Raport szczegóły subskrypcji**

>[!Note]
>Dane revenue i ACR są dostępne tylko dla użytkowników, którzy są osobami przeglądających raporty kierownictwa.

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data zakończenia subskrypcji | 
| SubscriptionState | Stan subskrypcji (aktywna lub zerowana) | 
| Month (Miesiąc) | Miesiąc, dla którego raportuje się użycie i przychód | 
| IsAutoRenew | Wskazuje, czy subskrypcja jest autorejezysowa (Tak, czy Nie) | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator GUID klienta | 
| CustomerTpid | Identyfikator nadrzędny najwyższego klienta | 
| CustomerSegment | Segment rynku klienta | 
| CustomerMarket | Geograficzny rynek klienta | 
| Produkt | Produkt sprzedawany klientowi przez partnera | 
| SKU | SKU produktu | 
| MpNId | Microsoft Partner Network partnera | 
| PartnerName | Nazwa partnera | 
| Lokalizacja partnera | Lokalizacja geograficzna partnera | 
| Typ PartnerAttributionType | Typ przypisania dla subskrypcji | 
| SalesChannel | Kanał sprzedaży — bezpośredni, CSP (Dostawca rozwiązań w chmurze) i tak dalej | 
| DostępneSeats | Bieżące dostępne stanowisko | 
| RevenueUSD | Przychód w dolarach amerykańskich | 
| Identyfikator rejestracji | Identyfikator rejestracji subskrypcji | 

### <a name="azure-usage-report"></a>**Raport użycia platformy Azure**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data zakończenia subskrypcji | 
| SubscriptionState | Bieżący stan subskrypcji (otwartej, zamkniętej, aktywnej lub w okresie prolongaty) | 
| Month (Miesiąc) | Data zagregowana według miesiąca | 
| ServiceName | Nazwa usługi platformy Azure | 
| MeterCategory | Nazwa kategorii miernika | 
| UsageUnits | Liczba jednostek używanych w cyklu rozliczeniowym | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędny najwyższego klienta | 
| CustomerSegment | Segment klienta | 
| CustomerMarket | Geograficzny rynek klienta | 
| MpNId | Microsoft Partner Network klienta | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Geograficzna lokalizacja kraju partnera | 
| Typ PartnerAttributionType | Typ przypisania partnera | 
| SalesChannel | Kanał sprzedaży (Direct/CSP, Indirect/CSP, Direct i tak dalej) | 
| ACR_USD | Przychody zużyte przez platformę Azure (ACR) w dolarach amerykańskich | 
| Identyfikator rejestracji | Identyfikator rejestracji subskrypcji platformy Azure | 

### <a name="office-365-license-usage-report"></a>**Raport użycia licencji usługi Office 365**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędny najwyższego klienta | 
| Nazwa_obciążenia | Skype dla firm, Teams, Exchange Online | 
| Month (Miesiąc) | Miesiąc, dla którego jest zgłaszane użycie | 
| PaidAvailableUnits | Liczba płatnych dostępnych jednostek | 
| MonthlyActiveUsers | Liczba aktywnych użytkowników miesięcznie | 
| CustomerName | Nazwa klienta | 
| CustomerMarket | Geograficzna lokalizacja kraju rynku klienta | 
| CustomerSegment | Segment klientów | 
| MpNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerLocation | Lokalizacja geograficzna partnera | 
| PartnerAttributionType | Typ przypisania partnera | 

### <a name="enterprise-mobility-license-usage-report"></a>**Raport użycia licencji pakietu Enterprise Mobility**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędny najwyższego klienta | 
| Nazwa_obciążenia | Nazwa obciążenia Enterprise Mobility + Security (EMS) | 
| Month (Miesiąc) | Miesiąc, dla którego jest zgłaszane użycie | 
| PaidAvailableUnits | Liczba płatnych dostępnych jednostek | 
| MonthlyActiveUsers | Liczba aktywnych użytkowników miesięcznie | 
| CustomerName | Nazwa klienta | 
| CustomerMarket | Geograficzna lokalizacja kraju na rynku klienta | 
| CustomerSegment | Segment klientów | 
| MpNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| Lokalizacja partnera | Lokalizacja geograficzna partnera | 
| Typ PartnerAttributionType | Typ przypisania partnera | 

### <a name="dynamics-365-license-usage-report"></a>**Raport użycia licencji usługi Dynamics 365**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data zakończenia subskrypcji | 
| SubscriptionStatus | Stan subskrypcji | 
| Month (Miesiąc) | Miesiąc, dla którego jest zgłaszane użycie | 
| RevSumDivisionName | Nazwa dzielenia sumy rev | 
| RevSumCategoryName | Nazwa kategorii sumy rev | 
| SKU | SKU produktu | 
| SKUId | Identyfikator SKU produktu | 
| FreeVsPaidSKU | Wskazuje, czy jest to bezpłatna, czy płatna sku | 
| SalesModel | Kanał sprzedaży używany do sprzedaży subskrypcji | 
| DetailedSalesModel | Szczegółowy model sprzedaży dla subskrypcji | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator GUID dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędny najwyższego klienta | 
| CustomerSegment | Segment rynku klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| MpNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| Lokalizacja partnera | Lokalizacja geograficzna kraju partnera | 
| Typ PartnerAttachType | Typ przypisania dla subskrypcji | 
| DostępneSeats | Bieżące dostępne stanowisko | 
| PrzypisaneSeats | Aktualnie przypisane stanowisko | 
| ActiveSeats | Bieżące aktywne stanowiska | 
| DeploymentOpportunity | Możliwość bieżącego wdrożenia | 
| ActiveUsagePercent | Bieżąca wartość procentowa aktywnego użycia | 

### <a name="power-bi-license-usage-report"></a>**Power BI użycia licencji**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| SubscriptionId | Identyfikator GUID subskrypcji | 
| SubscriptionStartDate | Data rozpoczęcia subskrypcji | 
| SubscriptionEndDate | Data zakończenia subskrypcji | 
| SubscriptionStatus | Stan subskrypcji (aktywny, nieaktywny lub w okresie prolongaty) | 
| Month (Miesiąc) | Data zagregowana według miesiąca | 
| SKU | SKU produktu | 
| SKUId | Identyfikator SKU produktu | 
| FreeVsPaidSKU | Free or paid SKU differentiator (Bezpłatna lub płatna różnicz SKU) | 
| SalesModel | Model sprzedaży używany do sprzedaży subskrypcji | 
| DetailedSalesModel | Szczegółowy model sprzedaży dla subskrypcji | 
| CustomerName | Nazwa klienta | 
| CustomerTenantId | Identyfikator GUID dzierżawy klienta | 
| CustomerTpid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| CustomerSegment | Segment rynku klienta | 
| CustomerMarket | Rynek geograficzny klienta | 
| MpNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| Lokalizacja partnera | Lokalizacja geograficzna kraju partnera | 
| Typ PartnerAttachType | Typ przypisania dla subskrypcji | 
| DostępneSeats | Bieżące dostępne stanowiska | 
| PrzypisaneSeats | Aktualnie przypisane stanowiska | 
| ActiveSeats | Bieżące aktywne stanowiska | 
| DeploymentOpportunity | Możliwość bieżącego wdrożenia | 
| ActiveUsagePercent | Bieżąca wartość procentowa aktywnego użycia | 

### <a name="teams-meetings-and-calls-report"></a>**Raport o spotkaniach i połączeniach zespołów**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędnego klienta | 
| Month (Miesiąc) | Miesiąc, dla którego jest zgłaszane użycie | 
| Podsieć | Podsieć, dla której jest zgłaszane użycie (spotkania, połączenia lub systemy telefoniczne) | 
| Liczba spotkań | Liczba spotkań | 
| Czas trwania spotkania | Łączny czas trwania spotkania w godzinach | 

### <a name="teams-monthly-usage-report"></a>**Miesięczny raport użycia dla zespołów**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator najwyższego elementu nadrzędnego klienta | 
| Month (Miesiąc) | Miesiąc, dla którego jest zgłaszane użycie | 
| Podsieć | Podciążanie, dla którego jest zgłaszane użycie (spotkania, połączenia lub systemy telefoniczne) | 
| Użytkownicy pulpitu | Liczba użytkowników korzystających z aplikacji Teams na pulpicie | 
| Użytkownicy mobilni | Liczba użytkowników korzystających z aplikacji Teams na urządzeniach przenośnych | 
| Użytkownicy sieci Web | Liczba użytkowników, którzy korzystają z aplikacji Teams w Internecie | 
| AllUpParticipants | Liczba unikatowych użytkowników aplikacji Teams w miesiącu | 

### <a name="teams-usage-3p-apps-report"></a>**Raport aplikacji 3P użycia aplikacji Teams**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CustomerTenantId | Identyfikator dzierżawy klienta | 
| CustomerTpid | Identyfikator nadrzędny najwyższego klienta | 
| Month (Miesiąc) | Miesiąc, dla którego jest zgłaszane użycie | 
| Nazwa aplikacji 3P | Nazwa aplikacji Teams | 
| Liczba użytkowników | Liczba użytkowników aplikacji | 


### <a name="training-details-report"></a>**Raport Szczegóły szkolenia**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| TrainingActivityId | Identyfikator szkolenia | 
| TrainingTitle | Tytuł szkolenia | 
| TrainingType | Typ szkolenia (certyfikacja lub egzamin) | 
| IndividualFirstName | Imię klienta | 
| IndividualLastName | Nazwisko klienta | 
| E-mail | Osobisty identyfikator e-mail klienta | 
| Poczta firmowa | Identyfikator e-mail klienta pakietu Office | 
| TrainingCompletionDate | Data ukończenia szkolenia | 
| Month (Miesiąc) | Miesiąc, dla którego są zgłaszane dane | 
| IcMCP | Wskazuje, czy użytkownik jest specjalistą Microsoft Certified Professional (MCP) | 
| Identyfikator MCPID | Identyfikator MCP użytkownika | 
| MpNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| PartnerCityLocation | Lokalizacja geograficzna miasta partnera | 
| PartnerCountryLocation | Lokalizacja geograficzna kraju partnera | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn raportu**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Nazwa użytkownika | Nazwa użytkownika | 
| UserId | Identyfikator GUID użytkownika | 
| TrainingName (Nazwa szkolenia) | Nazwa szkolenia | 
| TrainingType | Typ szkolenia (moduł lub ścieżka szkoleniowa) | 
| Produkty | Produkt, którego dotyczy moduł uczenia | 
| Role | Odpowiednie role szkolenia | 
| CompletionDate | Data ukończenia szkolenia | 
| MpNId | Identyfikator Microsoft Partner Network | 
| PartnerName | Nazwa partnera | 
| Kraj | Geograficzna lokalizacja kraju partnera | 

### <a name="competency-summary-and-history-report"></a>**Podsumowanie kompetencji i raport historii**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CompetencyName | Nazwa kompetencji | 
| CompetencyLevel | Poziom kompetencji (Gold lub Silver) | 
| CompetencyStatus | Bieżący stan kompetencji (aktywny, nieaktywny lub w okresie prolongaty) | 
| CompetencyStartDate | Data rozpoczęcia kompetencji | 
| CompetencyEndDate | Data zakończenia kompetencji | 

### <a name="competency-performance-report"></a>**Raport wydajności kompetencji**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| CompetencyName | Nazwa kompetencji | 
| CompetencyAttainmentOptionName | Nazwa opcji poziomu kompetencji | 
| Month (Miesiąc) | Miesiąc, dla którego metryki są zgłaszane | 
| MetricName | Nazwa metryki istotnej dla kompetencji | 
| MetricMonthlyContribution | Miesięczny udział metryki | 
| TTMAggregate | Metryka zagregowana dla ostatnich 12 miesięcy | 
| AnniversaryYearAggregate | Metryka zagregowana dla bieżącego roku rocznicowego | 
| GoldThreshold | Wymaganie dotyczące wydajności w celu spełnienia kompetencji Gold | 
| SilverThreshold | Wymaganie dotyczące wydajności w celu spełnienia kompetencji Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent — Microsoft 365 raport o proporcjonalności**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Microsoft Partner Network identyfikator | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikatora klienta | 
| Numer DUNS | The Dun & Bradstreet (D&B) number of the customer who's scoreded for propensity | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża, do której należy organizacja | 
| Pionowa | Pionowa relacja klienta, który jest osłaniany za pomoc, zidentyfikowana przez firmę Microsoft, D&B i inne standardy branżowe | 
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Podmiot zależny klienta, który jest osądlany do proporcjonalności | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży klienta, który jest osądlany do proporcjonalności | 
| City (Miasto) | Geograficzna lokalizacja miasta organizacji | 
| Stan | Lokalizacja geograficzna stanu organizacji | 
| Postal Code | Kod pocztowy organizacji | 
| Kraj | Geograficzna lokalizacja kraju organizacji | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegment rynku | 
| Podsumowanie typu kontrolera SMC | Typ kontrolera SMC | 
| Najważniejsze niezamaniowane — baza obliczeniowa | Klienci niezamażwani — obliczenia | 
| Najważniejsze niezamaniowane — baza użytkowników | Top unmanaged customers – user | 
| IsNonProfit | Wskazuje, czy organizacja jest organizacją niedochodową (Tak czy Nie) | 
| Włączanie pracy zdalnej — docelowa usługa Exchange Online | Klienci, którzy mają aktywną subskrypcję usługi Exchange Online, odsprzedają Microsoft 365 | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (bieżąca wersja) przy użyciu platformy Cloud Ascent Propensity — +10 licencji | Klient, który ma bieżącego klienta lokalnego pakietu Office lub systemu Windows. Oznacza to, że wersja klienta jest późniejsza niż wersja końca cyklu życia (EOL). Klient ma co najmniej 10 licencji. Klient, który ma ocenę proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (bieżąca wersja) przy użyciu platformy Cloud Ascent Propensity — <10 licencji | Klient, który ma bieżącego klienta lokalnego pakietu Office lub systemu Windows (czyli wersję nowszą niż EOL). Klient ma mniej niż 10 licencji. Klient, który ma ocenę proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (bieżąca wersja) bez zależności od usługi Cloud Ascent — +10 licencji | Klient, który ma bieżącego klienta lokalnego pakietu Office lub systemu Windows (czyli wersję nowszą niż EOL). Klient ma co najmniej 10 licencji. Klient nie ma oceny proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (bieżąca wersja) bez zależności od usługi Cloud Ascent — <10 licencji | Klient, który ma bieżącego klienta lokalnego pakietu Office lub systemu Windows (czyli wersję nowszą niż EOL). Klient ma mniej niż 10 licencji. Klient nie ma oceny proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (wersja EOL) przy użyciu platformy Cloud Ascent Propensity — +10 licencji | Klient, który ma lokalną wersję EOL dla pakietu Office lub klienta systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma co najmniej 10 licencji. Klient ma ocenę proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (wersja EOL) przy użyciu platformy Cloud Ascent Propensity — <10 licencji | Klient, który ma lokalnego klienta EOL pakietu Office lub systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma mniej niż 10 licencji. Klient ma ocenę proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (wersja EOL) bez platformy Cloud Ascent Propensity — +10 licencji | Klient, który ma bieżącego klienta lokalnego pakietu Office lub systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma co najmniej 10 licencji. Klient nie ma wyniku proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — pozyskiwanie lokalne (wersja EOL) bez zależności od usługi Cloud Ascent — <10 licencji | Klient, który ma bieżącego klienta lokalnego pakietu Office lub systemu Windows (czyli wersję EOL lub wcześniejszą). Klient ma mniej niż 10 licencji. Klient nie ma wyniku proporcjonalności. Partner powinien być celem konwersji na Microsoft 365. | 
| Włączanie pracy zdalnej — perspektywa wysokiej Microsoft 365 (Act NowithEvaluate) | Klient potencjalnych klientów z wysoką Microsoft 365 | 
| Włączanie pracy zdalnej — konkuruj (Zoom) z Microsoft 365 | Customer with Zoom and Microsoft 365, target for conversion to Teams | 
| Włączanie pracy zdalnej — konkuruj (Zoom) bez Microsoft 365 | Customer with Zoom, target for conversion to Teams | 
| Zmniejszenie kosztów i zarządzania — Microsoft 365 E3 dla Microsoft 365 E5 | Istniejący klient z Microsoft 365 E3, docelowy dla Microsoft 365 E5 | 
| Zmniejszenie kosztów i zarządzania — Microsoft 365 Business Basic i Business Standard, których celem jest Microsoft 365 Business Premium | Istniejący klienci Microsoft 365 Business Basic i Business Standard, docelowi dla Microsoft 365 Business Premium | 
| Przekształcanie produktywności organizacyjnej — wydajność urządzenia Surface | Klient wykazuje zadowolenie z urządzenia Surface | 
| M365Cluster | Określa, czy klient jest podatny na zakup Microsoft 365. Ustaw jako cel teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal istnieje pojemność po ustawieniu się teraz i ocenienie klientów. | 
| M365Fit | Wewnętrzne i zewnętrzne punkty danych definiujące firmographics. Ocenianie dopasowania używa modelu lookalike do naszych najlepszych małych i średnich firm (SMB), aby porównać klientów i sprawdzić, czy są one potencjalnym rozwiązaniem dla produktów firmy Microsoft w chmurze. Ocenianie dopasowania jest aktualizowane co kwartał. | 
| M365Intent | Sygnały związane z mediami społecznościowymi i zachowaniem online klienta definiują intencję. Ocenianie intencji jest nałogowe na dopasowanie w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| SurfaceCluster | Określa, czy klient jest podatny na zakup urządzenia Surface, konsolidując zalecenia dotyczące dopasowania i intencji w klastrze. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal dostępna jest pojemność po usługach Act Now i Evaluate customers. | 
| SurfaceFit | Wewnętrzne i zewnętrzne punkty danych definiujące firmographics. Ocenianie dopasowania wykorzystuje model lookalike do najlepszych średnich jakości usług, aby porównać klientów i sprawdzić, czy są one potencjalnym rozwiązaniem dla produktów w chmurze firmy Microsoft. Ocenianie dopasowania jest aktualizowane co kwartał. | 
| SurfaceIntent (Urządzenie powierzchniowe) | Sygnały związane z mediami społecznościowymi i zachowaniem online klienta definiują intencję. Ocenianie intencji jest nałogowe na dopasowanie w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| O365Cluster | Określa, czy klient jest w stanie kupić usługę Office 365. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal dostępna jest pojemność po usługach Act Now i Evaluate customers. | 
| O365Fit | Wewnętrzne i zewnętrzne punkty danych definiujące firmographics. Ocenianie dopasowania używa modelu lookalike do naszych najlepszych SMB, aby porównać klientów i sprawdzić, czy są one potencjalnym rozwiązaniem dla produktów w chmurze firmy Microsoft. Ocenianie dopasowania jest aktualizowane co kwartał. | 
| O365Intent | Sygnały związane z mediami społecznościowymi i zachowaniem online klienta definiują intencję. Ocenianie intencji jest nałogowe na dopasowanie w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| M365UpsellCustomer | Określa, czy klient wykazuje wywłaszczalność sprzedaży Microsoft 365 | 
| Ma usługę Google | Określa, czy klient pokazuje sygnały dotyczące konkurencji dotyczące posiadanych produktów Google | 
| Ma usługę AWS | Określa, czy klient pokazuje sygnały dotyczące konkurencji dla produktów Amazon Web Services (AWS) | 
| Ma ea | Określa, czy odnowienie jest umową Enterprise Agreement (EA), czy subskrypcją EA | 
| Ma otwarte | Określa, czy odnawianie jest umową Open, czy Open Value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent — raport o proporcjonalności usługi Dynamics 365**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Microsoft Partner Network identyfikator | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikatora klienta | 
| Numer DUNS | The Dun & Bradstreet number of the customer who's scored for propensity | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża, do której należy organizacja | 
| Pionowa | Pionowa relacja z klientem, który został oznaczony jako klient z poziomem proporcjonalności, identyfikowany przez firmy Microsoft, D&B i inne standardy branżowe
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Podmiot zależny klienta, który jest wyzyscyjnie | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży klienta, który jest wyzyscyjni ze względu na proporcjonalność | 
| City (Miasto) | Lokalizacja geograficzna miasta | 
| Stan | Lokalizacja geograficzna stanu | 
| Postal Code | Kod pocztowy organizacji | 
| Kraj | Lokalizacja geograficzna kraju | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegment rynku | 
| Podsumowanie typu kontrolera SMC | Kategoryzacja klienta: Główne niezamówiene bazy użytkowników to klienci z ponad 300 pracownikami, główne nieza zarządzania bazami obliczeniowymi to klienci z potencjałem 10 000 USD na platformie Azure przez trzy lata, średnie firmy to klienci z co najmniej 25 pracownikami, a małe firmy to klienci z mniej niż 25 pracownikami. | 
| Najważniejsze niezamaniowane — baza obliczeniowa | Klienci niezamażwani — obliczenia | 
| Najważniejsze niezamaniowane — baza użytkowników | Najgorętsi klienci niezamażni — użytkownicy | 
| IsNonProfit | Wskazuje, czy organizacja jest organizacją niedochodową (Tak, czy Nie) | 
| Activate Digital Selling - Microsoft 365 - seat size >= 25 seat (SalesPro propensity model) | Klient bez usługi Dynamics 365. Rozmiar miejsca: 25+. Partner powinien być celem sprzedaży krzyżowej usługi Dynamics 365 SalesPro. | 
| Aktywowanie sprzedaży cyfrowej — dynamics 365 SalesPropensity (działanie teraz lub ocena) | Klienci o wysokiej proporcjonalności bez usługi Dynamics 365. Partner powinien być celem dla usługi Dynamics 365 SalesPro. | 
| Managing Financial Risk & Fraud - Dynamics on-premises install base - Navision (Business Central propensity model) | Istniejący klient z lokalną usługą Navision. Partner powinien być ukierunkowany na usługę Dynamics 365 Business Central. | 
| Zarządzanie ryzykiem finansowym & oszustwem — lokalna baza instalacji usługi Dynamics — Dynamics AX (model proporcjonalności Dynamics 365 Finance + Operations) | Istniejący klient z lokalnym ax. Partner powinien być celem dla usługi Dynamics 365 Finance + Operations. | 
| Zarządzanie ryzykiem finansowym & oszustwem — lokalna baza instalacji usługi Dynamics — Great Plains (model proporcjonalności business central) | Istniejący klient z lokalnym środowiskiem Great Plains. Partner powinien być ukierunkowany na usługę Dynamics 365 Business Central. | 
| Managing Financial Risk & Fraud - Dynamics on-premises install base - Solomon (Business Central propensity model) | Istniejący klient z lokalnym solomonem. Partner powinien być celem usługi Dynamics 365 Business Central. | 
| Zarządzanie ryzykiem finansowym & oszustwem — lokalna baza instalacji usługi Dynamics — inne (model proporcjonalności usługi Business Central) | Istniejący klient z innymi rozwiązaniami lokalnymi, które nie zostały wcześniej wymienione. Partner powinien być celem usługi Dynamics 365 Business Central. | 
| Tworzenie elastycznych procesów biznesowych — baza instalacji lokalnej usługi Dynamics — AX/GP/SL/NAV/Other (model proporcjonalności usługi Dynamics 365) | Tworzenie elastycznych procesów biznesowych — baza instalacji lokalnej usługi Dynamics — AX/GP/SL/NAV/Other (model proporcjonalności usługi Dynamics 365) | 
| Tworzenie elastycznych procesów biznesowych — baza konkurencji Dynamics — Mendix/OutSystems/Salesforce (model proporcjonalności dynamics 365) | Tworzenie elastycznych procesów biznesowych — baza konkurencji Dynamics — Mendix/OutSystems/Salesforce (model proporcjonalności dynamics 365) | 
| Tworzenie elastycznych procesów biznesowych — baza instalacji dynamics 365 Finance + Operations | Istniejący klienci usługi Dynamics 365 Finance + Operations. Partner docelowy Power Apps. | 
| Tworzenie elastycznych procesów biznesowych — baza instalacji usługi Dynamics 365 Business Central | Istniejący klienci usługi Dynamics 365 Business Central. Partner docelowy Power Apps. | 
| Tworzenie elastycznych procesów biznesowych — baza instalacji usługi Dynamics 365 Customer Engagement | Istniejący klienci usługi Dynamics 365 Customer Engagement. Partner docelowy Power Apps. | 
| Tworzenie odpornego łańcucha dostaw — system Windows i aktywowanie pierwszego obciążenia usługi Dynamics 365 jako zarządzania łańcuchem dostaw usługi Dynamics 365 przy użyciu klientów innych niż Oracle lub SAP ERP (planowanie zasobów przedsiębiorstwa) | Klienci docelowi do zarządzania łańcuchem dostaw usługi Dynamics 365 | 
| Tworzenie odpornego łańcucha dostaw — sprzedaż krzyżowa usługi Dynamics 365 — zarządzanie łańcuchem dostaw i/lub handel detaliczny dla istniejących klientów usługi Dynamics 365 Customer Engagement | Istniejący klienci usługi Dynamics 365 Customer Engagement, których celem jest zarządzanie łańcuchem dostaw usługi Dynamics 365 w ramach sprzedaży krzyżowej. | 
| Tworzenie odpornego łańcucha dostaw — sprzedaż krzyżowa usługi Dynamics 365 Supply Chain Management i/lub handlu detalicznego do usług Dynamics 365 Customer Engagement i Oracle lub SAP | Istniejący klienci usługi Dynamics 365 Customer Engagement z bazą danych Oracle lub SAP docelową dla zarządzania łańcuchem dostaw usługi Dynamics 365 | 
| D365BCCluster | Określa, czy klient jest podatny na zakup usługi Dynamics 365 Business Central. Klienci, którzy wykazują swoją proporcjonalność do usługi Business Central, będą w kategorii Średnia i Mała. Ustaw jako cel teraz i Oceń klastry, ponieważ wyniosą one wyższą rentowność. Przekieruj klientów do edukacji tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak zaadeksuj działania teraz i oceń klientów. | 
| D365BCFit | Wewnętrzne i zewnętrzne punkty danych definiujące firmographics. Ocenianie dopasowania wykorzystuje model podobny do naszego najlepszego SMB, aby porównać klientów i sprawdzić, czy są potencjalnie odpowiedni dla produktów firmy Microsoft w chmurze. Ocenianie dopasowania jest aktualizowane co kwartał. | 
| D365BCIntent | Sygnały związane z mediami społecznościowymi i zachowaniem online klienta definiują intencję. Ocenianie intencji jest nałogowe na dopasowanie w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| D365FOCluster | Określa, czy klient jest podatny na zakup usługi Dynamics 365 Finance and Operations. Klienci, którzy wykazują przyczłętość do pracy z operacjami i finansami, będą się chcieć znaleźć w głównych kategoriach nieza zarządzania. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak ustawisz cel Ustaw teraz i Oceń klientów. | 
| D365FOFit | Wewnętrzne i zewnętrzne punkty danych definiujące firmographics. Ocenianie dopasowania wykorzystuje model podobny do naszego najlepszego SMB, aby porównać klientów i sprawdzić, czy są one potencjalnym rozwiązaniem dla produktów w chmurze firmy Microsoft. Ocenianie dopasowania jest aktualizowane co kwartał. | 
| D365FOIntent | Sygnały związane z mediami społecznościowymi i zachowaniem online klienta definiują intencję. Ocenianie intencji jest nałogowe na dopasowanie w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| D365CECluster | Określa zaangażowanie klienta w zakup usługi Dynamics 365 Customer Engagement. Klienci, którzy wykazują zaangażowanie w zaangażowanie klientów, będą w kategoriach Średni i Mały. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak ustawisz cel Ustaw teraz i Oceń klientów. | 
| D365CEFit | Wskazuje dopasowanie do usługi Dynamics 365 Customer Engagement | 
| D365CEIntent | Wskazuje intencję usługi Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Określa, czy klient ma otwarte odnawianie lokalnego programu Dynamics AX lub CRM | 
| M365UpsellCustomer | Określa, czy klient wykazuje wywłaszczalność sprzedaży Microsoft 365 | 
| Ma usługę Google | Określa, czy klient pokazuje sygnały dotyczące konkurencji dotyczące posiadanych produktów Google | 
| Ma usługę AWS | Określa, czy klient pokazuje sygnały dotyczące konkurencji dotyczące posiadanych produktów AWS | 
| Ma ea | Określa, czy odnowienie jest subskrypcją EA, czy ea | 
| Ma otwarte | Określa, czy odnawianie jest umową Open, czy Open Value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent — raport o proporcjonalności do platformy Azure**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Microsoft Partner Network identyfikator | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikatora klienta | 
| Numer DUNS | The Dun & Bradstreet number of the customer who's scored for propensity | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża | 
| Pionowa | Pionowa relacja z klientem, który został oznaczony jako klient z poziomem proporcjonalności, identyfikowany przez firmy Microsoft, D&B i inne standardy branżowe | 
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Podmiot zależny klienta, który jest wyzyscyjnie | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży klienta, który jest wyzyscyjni ze względu na proporcjonalność | 
| City (Miasto) | Lokalizacja geograficzna miasta | 
| Stan | Lokalizacja geograficzna stanu | 
| Postal Code | Kod pocztowy organizacji | 
| Kraj | Lokalizacja geograficzna kraju | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegment rynku | 
| Podsumowanie typu kontrolera SMC | Typ kontrolera SMC | 
| Najważniejsze niezamaniowane — baza obliczeniowa | Klienci niezamażwani — obliczenia | 
| Najważniejsze niezamaniowane — baza użytkowników | Najgorętsi klienci niezamówieni — użytkownicy | 
| IsNonProfit | Wskazuje, czy organizacja jest organizacją niedochodową (Tak, czy Nie) | 
| Migrate - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - 5+ licenses (Migracja — EOL Windows Server IB z proporcjonalnością usługi Cloud Ascent — ponad 5 licencji) | Klient, który ma lokalną wersję EOL systemu Windows Server (czyli wersję EOL lub wcześniejszą). Klient ma co najmniej 5 licencji. Klient, który ma ocenę proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — EOL Windows Server — EOL Windows Server IB with Cloud Ascent propensity — <5 licencji | Klient, który ma lokalną wersję EOL systemu Windows Server (czyli wersję EOL lub wcześniejszą). Klient ma mniej niż 5 licencji. Klient, który ma ocenę proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — EOL Windows Server — EOL Windows Server IB without Cloud Ascent propensity - 5+ licenses | Klient, który ma lokalną wersję EOL systemu Windows Server (czyli wersję EOL lub wcześniejszą). Klient ma więcej niż 5 licencji. Klient nie ma oceny proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — EOL Windows Server — EOL Windows Server IB without Cloud Ascent propensity — <5 licencji | Klient, który ma lokalną wersję EOL systemu Windows Server (czyli wersję EOL lub wcześniejszą). Ma mniej niż 5 licencji. Klient nie ma oceny proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrate - EOL SQL - EOL SQL Server IB with Cloud Ascent Propensity - 5+ licenses (Migracja — EOL SQL — ponad 5 licencji) | Klient, który ma lokalną wersję EOL SQL Server (czyli wersję EOL lub wcześniejszą). Klient ma ponad 5 licencji. Klient ma ocenę proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrate - EOL SQL - EOL SQL Server IB with Cloud Ascent propensity - <5 licenses (Migracja — EOL SQL — 5 licencji) | Klient, który ma lokalną wersję EOL SQL Server (czyli wersję EOL lub wcześniejszą). Ma mniej niż 5 licencji. Klient, który ma ocenę proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrate - EOL SQL - EOL SQL Server IB without Cloud Ascent Propensity - 5+ licenses (Migracja — EOL SQL — ponad 5 licencji) | Klient, który ma lokalną wersję EOL SQL Server (czyli wersję EOL lub wcześniejszą). Klient ma co najmniej 5 licencji. Klient nie ma wyniku proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrate - EOL SQL - EOL SQL Server IB without Cloud Ascent Propensity — <5 licencji | Klient, który ma lokalną wersję EOL SQL Server (czyli wersję EOL lub wcześniejszą). Klient ma mniej niż 5 licencji. Klient nie ma wyniku proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — migrowanie lokalnego systemu Windows Server — bieżący system Windows Server IB z usługą Cloud Ascent Propensity — ponad 5 licencji | Klient z bieżącym lokalnym systemem Windows Server (wersja nowsza niż EOL). Klient ma ponad 5 licencji. Klient ma ocenę proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — migrowanie lokalnego systemu Windows Server — bieżąca wersja systemu Windows Server IB z proporcjonalnością usługi Cloud Ascent — <5 licencji | Klient z bieżącym lokalnym systemem Windows Server (wersja nowsza niż EOL). Klient ma mniej niż 5 licencji. Klient ma ocenę proporcjonalności dla platformy Azure. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — migrowanie lokalnego systemu Windows Server — bieżący system Windows Server IB bez zależności od chmury — ponad 5 licencji | Klient z bieżącym lokalnym systemem Windows Server (wersja nowsza niż EOL). Klient ma ponad 5 licencji. Klient nie ma oceny proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — migrowanie lokalnego systemu Windows Server — bieżący system Windows Server IB bez zależności od chmury — <5 licencji | Klient z bieżącym lokalnym systemem Windows Server (wersja nowsza niż EOL). Klient ma mniej niż 5 licencji. Klient nie ma oceny proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — Azure SQL maszyn wirtualnych SQL — bieżące SQL Server IB z proporcjonalnością usługi Cloud Ascent — ponad 5 licencji | Klient, który ma bieżącą wersję lokalną SQL Server (czyli wersję nowszą niż EOL). Klient ma ponad 5 licencji. Klient ma ocenę proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — Azure SQL maszyn wirtualnych SQL — bieżące SQL Server IB z proporcjonalnością do chmury — <5 licencji | Klient, który ma bieżącą wersję lokalną SQL Server (czyli wersję nowszą niż EOL). Klient ma mniej niż 5 licencji. Klient ma ocenę proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — Azure SQL maszyn wirtualnych SQL — bieżąca SQL Server IB bez platformy Cloud Ascent Propensity — ponad 5 licencji | Klient, który ma bieżącą wersję lokalną SQL Server (czyli wersję nowszą niż EOL). Klient ma ponad 5 licencji. Klient nie ma wyniku proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migracja — migrowanie Azure SQL maszyn wirtualnych SQL — bieżące SQL Server IB bez proporcjonalności do chmury — <5 licencji | Klient, który ma bieżącą wersję lokalną SQL Server (czyli wersję nowszą niż EOL). Klient ma mniej niż 5 licencji. Klient nie ma wyniku proporcjonalności. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — OSS — migrowanie do bazy danych Open Source Szmigrowanie (OSS) | Istniejący klient z dowolnym z następujących produktów konkurują ze sobą: PostgreSQL, MySQL, MariaDB. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — OSS — Linux na platformie Azure | Istniejący klient z systemem Linux. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — SAP — SAP na platformie Azure | Istniejący klient z sap. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — Windows Virtual Desktop — Usługi pulpitu zdalnego IB | Identyfikuje klientów z aktywnymi usługami Usługi pulpitu zdalnego. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrate - Windows Virtual Desktop - Cross Sell Modern Work to Azure/WVD | Identyfikuje klientów za pomocą Microsoft 365 i nie ma platformy Azure. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — VMware IB | Istniejący klient z produktem: VMware. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Migrowanie — Citrix IB | Istniejący klient z produktem: Citrix Systems. Partner powinien zwrócić się do tego klienta o migrację na platformę Azure. | 
| Innowacje — analiza — Power BI IB o wysokiej wydajności platformy Azure | Klienci z subskrypcją i usługą Active Power BI, w tym: Power BI - Standalone Pro, Power BI - Azure Suites, Power BI - Office Suites, Power BI Suites - Microsoft 365 | 
| Włączanie — Metodyka DevOps z usługą GitHub — Visual Studio/MSDN IB | Identyfikuje klientów z aktywnymi Visual Studio wersji | 
| Wersja Standardowa systemu Windows Server | Wyświetla wersję zakupów systemu Windows Server Standard przez klienta | 
| Licencja systemu Windows Server Standard | Wyświetla typ licencji zakupów systemu Windows Server Standard przez klienta | 
| Wersja centrum danych systemu Windows Server | Przedstawia wersję zakupów centrum danych systemu Windows u klienta | 
| Licencja centrum danych systemu Windows Server | Przedstawia typ licencji zakupów centrum danych systemu Windows przez klienta | 
| AzureFit | Wewnętrzne i zewnętrzne punkty danych definiujące firmographics. Ocenianie dopasowania wykorzystuje model podobny do naszego najlepszego SMB, aby porównać klientów i sprawdzić, czy są one potencjalnym rozwiązaniem dla produktów w chmurze firmy Microsoft. Ocenianie dopasowania jest aktualizowane co kwartał. | 
| AzureIntent (Usługa AzureIntent) | Sygnały związane z mediami społecznościowymi i zachowaniem online klienta definiują intencję. Ocenianie intencji jest nałogowe na dopasowanie w celu zdefiniowania klastrów. Ocenianie intencji jest aktualizowane co miesiąc. | 
| AzureCluster | Określa, czy klient jest w stanie zakupić platformę Azure, konsolidując zalecenia dotyczące dopasowania i intencji w klastrze. Ustaw jako cel teraz i Oceń klastry, ponieważ wyniosą one wyższą rentowność. Przekieruj klientów do edukacji tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak zaadeksuj działania teraz i oceń klientów. | 
| WindowsServerDataCenter_HasOpenRenewal | Określa, czy klient ma otwarte odnawianie centrum danych systemu Windows Server | 
| WindowsServerStandard_HasOpenRenewal | Określa, czy klient ma otwarte odnawianie dla systemu Windows Server Standard | 
| AzureUpsellCustomer | Określa, czy klient wykazuje wywłaszczalność sprzedaży na platformie Azure | 
| Ma usługę Google | Określa, czy klient pokazuje sygnały dotyczące konkurencji dotyczące posiadanych produktów Google | 
| Ma usługę AWS | Określa, czy klient pokazuje sygnały konkurencji dotyczące posiadanych produktów AWS | 
| Ma ea | Określa, czy odnawianie jest subskrypcją EA, czy ea | 
| Ma otwarte | Określa, czy odnawianie jest umową open value, czy open value | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent — raport o proporcjonalności do odnowienia umowy**

| Nazwa kolumny | Opis danych | 
| :--------- | :--------- | 
| Identyfikator MPN | Microsoft Partner Network identyfikator | 
| Nazwa partnera | Nazwa partnera | 
| Customer ID | Numer identyfikatora klienta | 
| Numer DUNS | The Dun & Bradstreet number of the customer who's scored for propensity | 
| Nazwa konta | Nazwa konta | 
| Domena | Domena konta | 
| Rozmiar organizacji | Rozmiar organizacji | 
| Branża | Branża | 
| Pionowa | Pionowa relacja z klientem, który został oznaczony jako klient z poziomem proporcjonalności, identyfikowany przez firmy Microsoft, D&B i inne standardy branżowe | 
| Warstwowy | Obszar geograficzny lokalizacji | 
| Przedstawicielstwo | Podmiot zależny klienta, który jest wyzyscyjnie | 
| Sales Territory (Obszar sprzedaży) | Terytorium sprzedaży klienta, który jest wyzyscyjni ze względu na proporcjonalność | 
| City (Miasto) | Lokalizacja geograficzna miasta | 
| Stan | Lokalizacja geograficzna stanu | 
| Postal Code | Kod pocztowy organizacji | 
| Kraj | Lokalizacja geograficzna kraju | 
| Segment | Segment rynku | 
| Segment podrzędny | Podsegmentowanie rynku | 
| Podsumowanie typu kontrolera SMC | Typ kontrolera SMC | 
| Najważniejsze niezamaniowane — baza obliczeniowa | Najgorętsi klienci niezamażni — obliczenia | 
| Najważniejsze niezamaniowane — baza użytkowników | Najgorętsi klienci niezamażni — użytkownicy | 
| IsNonProfit | Wskazuje, czy organizacja jest organizacją niedochodową (Tak, czy Nie) | 
| Ma usługę Google | Określa, czy klient pokazuje sygnały konkurencji dotyczące posiadanych produktów AWS | 
| Ma usługę AWS | Określa, czy klient pokazuje sygnały konkurencji dotyczące posiadanych produktów AWS | 
| Klaster platformy Azure | Określa, czy klient jest podatny na zakup platformy Azure. Ustaw jako cel teraz i Oceń klastry, ponieważ wyniosą one wyższą rentowność. Przekieruj klientów do edukacji tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak zaadeksuj działania teraz i oceń klientów. | 
| Klaster D365 Finance + Operations | Określa, czy klient jest podatny na zakup usługi Dynamics 365 Finance and Operations. Klienci, którzy wykazują przyzwolenia na usługi Finance + Operations, będą się ująć w główne nieza zarządzania kategoriami. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak ustawisz cel Ustaw teraz i Oceń klientów. | 
| Klaster D365 CE | Określa zaangażowanie klienta w zakup usługi Dynamics 365 Customer Engagement. Klienci, którzy wykazują zaangażowanie w zaangażowanie klientów, będą w kategoriach Średni i Mały. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak ustawisz cel Ustaw teraz i Oceń klientów. | 
| Klaster D365 BC | Określa, czy klient jest w stanie kupić usługę Dynamics 365 Business Central. Klienci, którzy będą mieć poziom proporcjonalny do usługi Business Central, będą w kategorii Średni i Mały. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak ustawisz cel Ustaw teraz i Oceń klientów. | 
| Microsoft 365 klastra | Określa, czy klient jest podatny na zakup Microsoft 365. Ustaw jako cel ustaw teraz i oceń klastry, ponieważ wyniosą one wyższą rentowność. Należy kierować działania do klientów i edukować ich tylko wtedy, gdy nadal będzie dostępna pojemność po tym, jak ustawisz cel Ustaw teraz i Oceń klientów. | 
| Program licencjonowania | Określa typ programu licencjonowania do odnowienia | 
| Identyfikator umowy | Identyfikator umowy | 
| Data zakończenia umowy | Data zakończenia umowy | 
| Typ wygaśnięcia | Typ wygaśnięcia | 
| Wygasający przychód | Przychód skojarzony z wygasającą subskrypcją | 
| Ma ea | Określa, czy odnowienie jest subskrypcją EA, czy ea | 
| Ma otwarte | Określa, czy odnawianie jest umową Open, czy Open Value | 
| Klient usługi Azure Upsell | Określa, czy klient wykazuje wywłaszczalność sprzedaży na platformie Azure | 
| Microsoft 365 upsell customer | Określa, czy klient wykazuje wywłaszczalność sprzedaży Microsoft 365 | 
| RevSumDivisionName | Identyfikuje produkt, który można odnowić | 

## <a name="next-steps"></a>Następne kroki

Aby uzyskać więcej informacji, zobacz [Pobieranie raportów](pci-download-reports.md).
