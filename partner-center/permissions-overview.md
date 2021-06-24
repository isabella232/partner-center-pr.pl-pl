---
title: Przypisywanie ról & uprawnień do użytkowników
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, które role są najlepsze dla użytkowników firmy, którzy zarządzają transakcjami komercyjnymi, poleceniami, zachętami lub członkostwem w programie MPN Partner Center.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 582fdc98617be7d82c0bc61a0bf46ceb662954d3
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565087"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Przypisywanie ról i uprawnień użytkowników w firmie, którzy muszą pracować w Partner Center

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Administrator partnera MPN

Profil partnera, w tym nazwę i adres prawna, szczegóły pomocy technicznej, informacje o zwolnieniach z podatku, informacje o banku i podstawowy kontakt dla twojej firmy. Następny krok: Skonfigurowanie użytkowników przy użyciu haseł i ról w celu rozpoczęcia pracy Partner Center z Tobem.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Konfigurowanie pracowników do pracy w Partner Center

Typy dostępu użytkowników, które muszą być Partner Center, określa się na podstawie ról i uprawnień, które im nadaj. Role są związane z programami, w które bierze udział Twoja firma. Jeśli na przykład Twoja firma jest firmą Dostawca rozwiązań w chmurze (CSP), będziesz mieć nie tylko standardowe role zarządzania dzierżawą usługi Azure Active Directory (Azure AD), takie jak administrator globalny, ale także role specyficzne dla programu CSP. Każdy program ma specyficzne role.

>[!Note]
> Role dzierżawy usługi Azure AD obejmują role administratora globalnego, administratora użytkowników i roli CSP. Role inne niż role usługi Azure AD to role, które nie zarządzają dzierżawą i obejmują administratora partnera MPN (Microsoft Partner Network), administratora profilu biznesowego, administratora poleceń, administratora zachęt i użytkownika zachęt. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Zarządzanie transakcjami komercyjnymi w Partner Center (role usługi Azure AD i CSP)

|**Role**|**Co mogą zrobić**|**Dowiedz się więcej**|
|----------------------------------|---|:---------------------------------|
|Administrator globalny|* Może uzyskać dostęp do wszystkich konto Microsoft/usług z pełnymi uprawnieniami|[Zarządzanie kontem w portalu Partner Center](partner-center-account-setup.md)
|      |* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera
||* Wyświetlanie umów, cenników i ofert
||* Wyświetlanie i tworzenie użytkowników partnerów oraz zarządzanie nimi|
||  Wyświetlanie, tworzenie i zarządzanie rozliczeniami, fakturami i plikami ponownego tworzenia
|Administrator zarządzania użytkownikami   | * Wyświetlanie i tworzenie użytkowników oraz zarządzanie nimi|[Zarządzanie korzyściami Microsoft Partner Network i ofertami członkostwa w programie Partner Center](manage-your-partner-network-benefits.md)
||* Wyświetl wszystko profilów partnerów
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera
|Administrator rozliczeń | — Wyświetlanie, tworzenie i zarządzanie rozliczeniami, fakturami i plikami ponownego tworzenia|[Read your bill (Odczytywanie rachunku)](billing.md)
||* Wyświetl cennik
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera
|Użytkownik domyślny|  Wyświetl Mój profil   |[Resetowanie hasła](reset-my-pasword.md)
|Agent administracyjny | * Zarządzanie klientami|[Nawiązywanie relacji z klientami](connect-with-your-customers.md)
||* Dodaj listę urządzeń do Partner Center
||* Tworzenie i stosowanie profilów do urządzeń
||* Zarządzanie subskrypcjami
||* Kondycja usługi i żądania obsługi dla klientów
||* Żądanie delegowanych uprawnień administratora
||* Wyświetlanie cen i ofert
||* Rozliczenia
||* Administrowanie w imieniu klienta
||* Rejestrowanie odsprzedawcy dodanej wartości
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera|
|Agent sprzedaży | * Zarządzanie klientami|[Zapewnianie pomocy technicznej dotyczącej rozliczeń dla klientów i pomaganie w odpowiadania na ich pytania dotyczące rozliczeń](provide-billing-support.md)
||* Dodaj listę urządzeń do Partner Center
||* Zarządzanie subskrypcjami
||* Wyświetlanie biletów pomocy technicznej
||* Żądanie relacji z klientem
||* Wyświetlanie cen i ofert
||* Zarządzanie potencjalnymi klientami
||* Wyświetlanie umowy klienta
||* Rejestrowanie odsprzedawcy dodanej wartości
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera|
|Agent pomocy technicznej| * Wyszukiwanie i wyświetlanie klienta|[Eskalowanie problemów do firmy Microsoft i dowiedz się, które problemy są bardziej odpowiednie do eskalacji firmy Microsoft](escalate-problems-to-microsoft.md)
||* Edytowanie szczegółów klienta
||* Pomoc w rozwiązywaniu problemów klientów z zarządzaniem rozliczeniami lub subskrypcjami
||* Żądanie pomocy technicznej w imieniu klientów 
||* Zarządzanie subskrypcjami i problemami z rozliczeniami w imieniu klientów
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Panel sterowania Vendor (CPV). (Rola CSP i rola spoza usługi Azure AD)

CpV opracowywać aplikacje do użytku przez partnerów CSP, aby umożliwić im integrowanie ich systemów z Partner Center API. 

|**Role**   |**Co możesz zrobić**|**Dowiedz się więcej**|
|------------------------------|:----------------------------|----|
|Administrator globalny| Wyświetlanie profilu dostawcy Panel sterowania (CPV) i zarządzanie nimi|[Zarejestruj się jako dostawca Panel sterowania, aby pomóc w integracji systemów partnerskich CSP z Partner Center API](enroll-as-cpv.md)
||Wyświetlanie użytkowników, którzy potrzebują dostępu do funkcji CPV, i zarządzanie nimi|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Użytkownik-gość (musi zostać dodany do dzierżawy usługi Azure AD)

|**Użytkownik-gość**   | **Role**|
|---------------------------|:--------------------|
||Administrator partnera MPN|
||Administrator profilu biznesowego|
||Administrator poleceń|


## <a name="manage-mpn-membership-and-your-company"></a>Zarządzanie członkostwem w programie MPN i firmą 

Te role nie są rolami usługi Azure AD. Te role zarządzają firmą, a nie dzierżawą.

|**Role** | **Co możesz zrobić**|**Dowiedz się więcej**|
|----------------------------|:----------------------------|-----|
|Administrator partnera MPN|* Wyświetlanie i tworzenie żądań obsługi partnerów oraz zarządzanie nimi|[Kupowanie lub odnawianie subskrypcji programu Microsoft Action Pack i kompetencji Gold](mpn-get-action-pack.md)
||* Wyświetlanie profilów prawnych, firmowych, biznesowych i MPN
||* Wyświetlanie szczegółów użytkownika i jego danych umiejętności
||* Wyświetlanie kompetencji
||* Wyświetlanie korzyści i zarządzanie nimi
||* Wyświetlanie i kupowanie ofert MPN
||* Wyświetlanie historii zamówień i faktur w ofertach MPN
||* Wyświetlanie danych wskaźnika udziału partnera
||* Może działać w narzędziu do weryfikacji walidowania walidowania w|
||* Wyświetlanie analizy danych klientów
||* Wyświetlanie innych ról użytkowników w firmie, ale nie można przypisywać ról
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera
|Administrator konta| Dodawanie lokalizacji|[Zarządzanie lokalizacjami](manage-locations.md)
|| Zarządzanie profilami związanymi z kontami, dla których jesteś administratorem 
||* Przypisywanie ról dla użytkowników w dzierżawie do ról spoza usługi Azure AD 
||* Rejestrowanie lokalizacji w programach
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera

## <a name="manage-referrals"></a>Zarządzanie poleceniami

|**Role** | **Co możesz zrobić**|**Dowiedz się więcej**
|------------------------------|:-------------------------|---|
|Administrator poleceń|Tworzenie wszystkich danych i zarządzanie nimi na karcie Polecenia w Partner Center|[Zarządzanie możliwościami wspólnej sprzedaży](manage-co-sell-opportunities.md)
||    Może wyświetlać i edytować wszystkie szanse sprzedaży i potencjalnych klientów
||    Może przypisywać członków zespołu do transakcji
||    Może wyświetlać i edytować profile biznesowe
||    Może wyświetlać i rejestrować transakcje dla szans sprzedaży oznaczonych jako wygrane i uprawnione do rejestracji transakcji
||    Może tworzyć i wyświetlać bilety pomocy technicznej
|Użytkownik poleceń|Tworzenie możliwości współpracy sprzedaży i zarządzanie nimi tylko wtedy, gdy są one częścią zespołu |[Zarządzanie możliwościami wspólnej sprzedaży](manage-co-sell-opportunities.md)
||    Może tworzyć możliwości współpracy sprzedaży dla lokalizacji, w których przypisano im rolę.
||    Może wyświetlać i rejestrować transakcje dla szans sprzedaży oznaczonych jako wygrane i uprawnione do rejestracji transakcji, jeśli są członkami zespołu.
||    Może tworzyć i wyświetlać bilety pomocy technicznej
|Administrator profilu biznesowego|Tworzenie profilów biznesowych i zarządzanie nimi | [Zarządzanie profilami biznesowymi](create-a-marketing-profile.md)
||    Może tworzyć i wyświetlać bilety pomocy technicznej

Wraz z nową rolą użytkownika poleceń wprowadzamy również zakres lokalizacji dla transakcji. W poniższej tabeli wyjaśniono dostęp do transakcji na podstawie lokalizacji.

|**Zakres** | **Co możesz zrobić** |
|------------------------------|:-------------------------|
|Cała firma | Zarówno administratorzy, jak i użytkownicy mają dostęp do tworzenia transakcji dla dowolnej lokalizacji w swojej firmie|
|| Administrator poleceń ma dostęp do wyświetlania i edytowania wszystkich transakcji |
|| Użytkownicy poleceń mają dostęp do wyświetlania i edytowania wszystkich transakcji tylko wtedy, gdy są częścią zespołu |
|Co najmniej jedna lokalizacja | Zarówno administratorzy, jak i użytkownicy mają dostęp do tworzenia transakcji dla przypisanej lokalizacji w swojej firmie|
|| Administrator poleceń ma dostęp do wyświetlania i edytowania wszystkich transakcji należących do przypisanych lokalizacji|
|| Użytkownicy poleceń mają dostęp do wyświetlania i edytowania wszystkich transakcji należących do przypisanych lokalizacji, jeśli są częścią zespołu|

## <a name="manage-incentives"></a>Zarządzanie zachętami

|**Role** | **Co możesz zrobić**|**Dowiedz się więcej**
|------------------------------|:-------------------------|---|
|Administrator zachęt|* Inicjuje zachęty i zarządza nimi |[Użyj tych zasobów, aby rozpocząć pracę z zachętami](incentives-get-started-intro.md)
||* Może wyświetlać i edytować wszystkie aspekty programów zachęt
||* Może wyświetlać i edytować dane bankowe i podatkowe
||* Wyświetlanie zarobków dla chętnych i współzałożycieli
||* Obsługa dostępu
||* Spory dotyczące płatności zachęt|
|Zachęty użytkownika|* Może wyświetlać programy zachęt
||* Może wyświetlać i inicjować roszczenia dotyczące zachęt
||* Wyświetlanie zarobków dla chętnych i współzałożycieli
||* Tworzenie biletów pomocy technicznej dla Partner Center
||* Wyświetlanie tworzyć biletów pomocy technicznej partnera

## <a name="view-partner-center-insights-data"></a>Wyświetlanie Partner Center szczegółowych informacji

|**Role** | **Co możesz zrobić**|**Dowiedz się więcej**|
|------------------------------|:-------------------------|---|
|Przeglądarka raportów dla kierownictwa|Dostęp do wszystkich zestawów danych raportowania, tworzenie biletów pomocy technicznej partnera, wyświetlanie tworzyć biletów pomocy technicznej partnera|[Omówienie raportów pulpitu nawigacyjnego dostępnych w u Partner Center Insights](pci-overview-report.md)
|Przeglądarka raportów|Dostęp do raportów danych z wyjątkiem danych osobowych dotyczących przychodów oraz danych osobowych klientów i pracowników, tworzenie biletów pomocy technicznej partnera, wyświetlanie tworzyć biletów pomocy technicznej partnera|

## <a name="next-steps"></a>Następne kroki

- [Tworzenie kont użytkowników i przypisywanie ról oraz uprawnień](create-user-accounts-and-set-permissions.md)
- [Weryfikowanie informacji o koncie podczas rejestrowania w nowym Partner Center programie](verification-responses.md)
