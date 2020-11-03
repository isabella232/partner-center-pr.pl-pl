---
title: Przypisywanie ról & uprawnień użytkownikom
ms.topic: article
ms.date: 09/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, które role najlepiej nadają się użytkownikom firmy, którzy zarządzają komercyjnymi transakcjami, odwołaniami, bodźcami lub członkostwem MPN w centrum partnerskim.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 32df86887ccbea5d18d1bd8c7c34add2b1ab60e4
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530261"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Przypisywanie ról i uprawnień użytkowników dla użytkowników firmy, którzy chcą korzystać z Centrum partnerskiego

**Odpowiednie role**

- Administrator globalny
- Administrator użytkowników
- Administrator partnerski MPN

Skonfigurowano Profil partnera, w tym imię i nazwisko oraz adres, szczegóły pomocy technicznej, zwolnienia podatkowe plików, informacje o banku oraz kontakt podstawowy firmy. Następny krok: Poproś użytkowników o skonfigurowanie haseł i ról, aby mogli zacząć pracę w centrum partnerskim.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Konfigurowanie pracowników do pracy w centrum partnerskim

Należy określić typy dostępu użytkowników do Centrum partnerskiego według ról i uprawnień. Role są powiązane z programami, w których działa Twoja firma. Na przykład jeśli Twoja firma jest firmą z dostawcą rozwiązań w chmurze (CSP), nie będziesz mieć tylko standardowych ról zarządzania dzierżawcą Azure Active Directory, takich jak Administrator globalny, ale będą potrzebować ról specyficznych dla programu CSP. Każdy program ma odpowiednie role.

>[!Note]
> Azure Active Directory ról dzierżawy należą do roli Administrator globalny, administrator użytkowników i dostawca usług kryptograficznych. Role spoza usługi Azure-Active-Directory to role, które nie zarządzają dzierżawcą. obejmują one MPN administratora, administratora profilu biznesowego, administratora odwołań, administratora zachęty i użytkownika zachęty. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Zarządzanie transakcjami komercyjnymi w centrum partnerskim (role usługi Azure AD i CSP)

|**Role**|**Co można zrobić**|**Dowiedz się więcej**|
|----------------------------------|---|:---------------------------------|
|Administrator globalny|* Może uzyskać dostęp do wszystkich konto Microsoft/usług z pełnymi uprawnieniami|[Zarządzanie kontem w portalu Partner Center](partner-center-account-setup.md)
|      |* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej
||* Wyświetlanie umów, cenników i ofert
||* Wyświetlanie, tworzenie i zarządzanie użytkownikami partnerskimi|
||  Wyświetlanie, tworzenie i Zarządzanie rozliczeniami, fakturami i plikami Rekonesans
|Administrator zarządzania użytkownikami   | * Wyświetlanie, tworzenie i zarządzanie użytkownikami|[Zarządzaj korzyściami z członkostwa w Microsoft Partner Network i ofertami w centrum partnerskim](manage-your-partner-network-benefits.md)
||* Wyświetl wszystkie profile partnerów
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej
|Administrator rozliczeń | — Wyświetlanie, tworzenie i Zarządzanie rozliczeniami, fakturami i plikami Rekonesans|[Read your bill (Odczytywanie rachunku)](billing.md)
||* Wyświetl Cennik
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej
|Użytkownik domyślny|  Wyświetl mój profil   |[Resetowanie hasła](reset-my-pasword.md)
|Agent administracyjny | * Zarządzanie klientami|[Nawiązywanie połączenia z klientami](connect-with-your-customers.md)
||* Dodaj listę urządzeń do Centrum partnerskiego
||* Tworzenie i stosowanie profilów na urządzeniach
||* Zarządzanie subskrypcjami
||* Żądania dotyczące kondycji usług i usług dla klientów
||* Żądaj uprawnień administratora delegowanego
||* Wyświetl Cennik i oferty
||* Rozliczenia
||* Administruj w imieniu klienta
||* Rejestracja odsprzedawcy o wartości dodanej
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej|
|Agent sprzedaży | * Zarządzanie klientami|[Zapewnij klientom pomoc techniczną dotyczącą rozliczeń i udziel odpowiedzi na pytania dotyczące rozliczeń](provide-billing-support.md)
||* Dodaj listę urządzeń do Centrum partnerskiego
||* Zarządzanie subskrypcjami
||* Wyświetlanie biletów pomocy technicznej
||* Zażądaj relacji z klientem
||* Wyświetl Cennik i oferty
||* Zarządzanie potencjalnymi klientami klienta
||* Wyświetl umowę klienta
||* Rejestracja odsprzedawcy o wartości dodanej
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej|
|Agent pomocy technicznej| * Wyszukiwanie i wyświetlanie klienta|[Eskalacja problemów do firmy Microsoft i Dowiedz się, które problemy są bardziej odpowiednie dla eskalacji firmy Microsoft](escalate-problems-to-microsoft.md)
||* Edytuj szczegóły klienta
||* Pomoc w rozwiązywaniu problemów klientów związanych z rozliczeniami i zarządzaniem subskrypcjami
||* Prośba o pomoc techniczną w imieniu klientów 
||* Zarządzanie subskrypcjami i problemami z rozliczeniami w imieniu klientów
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Dostawca panelu sterowania (CPV). (Rola CSP i rola spoza usługi Azure AD)

CPVs opracowywać aplikacje do użycia przez partnerów dostawcy rozwiązań w chmurze (CSP), aby umożliwić im integrację systemów z interfejsami API Centrum partnerskiego. 

|**Role**   |**Co możesz zrobić**|**Dowiedz się więcej**|
|------------------------------|:----------------------------|----|
|Administrator globalny| Wyświetl swój profil CPV i Zarządzaj nim|[Zarejestruj się jako dostawca panelu sterowania, aby ułatwić integrację systemów partnerskich programu CSP z interfejsami API Centrum partnerskiego](enroll-as-cpv.md)
||Wyświetl wszystkich użytkowników, którzy potrzebują dostępu do funkcji CPV, i zarządzaj nimi|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Użytkownik-Gość (musi zostać dodany do dzierżawy Azure Active Directory)

|**Użytkownik-Gość**   | **Role**|
|---------------------------|:--------------------|
||Administrator partnerski MPN|
||Administrator kont|
||Administrator zachęt|
||Administrator profilu biznesowego|
||Administrator odwołań|


## <a name="manage-mpn-membership-and-your-company"></a>Zarządzanie członkostwem w MPN i firmą 

Role te nie są Azure Active Directory rolami. Role te zarządzają firmową firmą, a nie z dzierżawcą.

|**Role** | **Co możesz zrobić**|**Dowiedz się więcej**|
|----------------------------|:----------------------------|-----|
|Administrator partnerski MPN|* Wyświetlanie i tworzenie żądań obsługi partnerów oraz zarządzanie nimi|[Kupowanie lub odnawianie subskrypcji programu Microsoft Action Pack i kompetencji Gold](mpn-get-action-pack.md)
||* Wyświetl profile prawne, firmowe, biznesowe i MPN
||* Wyświetl szczegóły użytkownika i ich dane dotyczące umiejętności
||* Wyświetl kompetencje
||* Wyświetl korzyści i zarządzaj nimi
||* Oferty dotyczące widoków i zakupów MPN
||* Widok MPN zawiera historię i faktury zamówień
||* Wyświetl dane wskaźnika udziału partnera
||* Można korzystać z narzędzia sprawdzania poprawności załącznika|
||* Przeglądanie analizy danych klienta
||* Wyświetl inne role użytkownika w firmie, ale nie można przypisać ról
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej
|Administrator konta| Dodaj lokalizacje|[Zarządzaj lokalizacjami](manage-locations.md)
|| Zarządzanie profilami związanymi z kontami, dla których jesteś administratorem 
||* Przypisywanie ról dla użytkowników w dzierżawie do ról spoza usługi Azure Active Directory 
||* Rejestrowanie lokalizacji w programach
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej


## <a name="manage-referrals"></a>Zarządzanie odwołaniami 

|**Role**|**Co możesz zrobić**|**Dowiedz się więcej**|
|-----------------------------|:------------------------|---|
|Administrator odwołań       |* Wyświetlanie i tworzenie profilów firmy oraz zarządzanie nimi|[Manage different leads like customer inquiries, marketing-qualified leads, and sales-qualified leads (Zarządzanie różnymi typami potencjalnych klientów: wywodzących się bezpośrednio z klientów, zakwalifikowanych za pośrednictwem kanału marketingowego i zakwalifikowanych przez sprzedawców)](manage-leads.md)
||* Odbierz odwołania i zarządzaj nimi
||* Wyświetlanie i tworzenie odwołań do współsprzedażowych oraz zarządzanie nimi|
||* Wyświetlanie i tworzenie żądań obsługi partnerów oraz zarządzanie nimi
|Administrator profilu biznesowego   |* Wyświetlanie i tworzenie profilu biznesowego oraz zarządzanie nim |[Utwórz profil biznesowy](create-a-marketing-profile.md)
||* Wyświetlanie i tworzenie żądań obsługi partnerów oraz zarządzanie nimi
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej|

## <a name="manage-incentives"></a>Zarządzanie bodźcami 

|**Role** | **Co możesz zrobić**|**Dowiedz się więcej**
|------------------------------|:-------------------------|---|
|Administrator zachęt|* Inicjuje zachęty i zarządza nimi |[Skorzystaj z tych zasobów, aby rozpocząć pracę z zachętami](incentives-get-started-intro.md)
||* Może wyświetlać i edytować wszystkie aspekty programów zachęty
||* Można wyświetlać i edytować szczegóły dotyczące banku i podatku
||* Wyświetlanie zysków z rabatu i współistnienia
||* Pomoc techniczna dotycząca dostępu
||* Płatności zachęcające do rozstrzygania sporów|
|Użytkownik zachęt|* Może wyświetlać programy zachęty
||* Można wyświetlać i inicjować oświadczenia zachęt
||* Wyświetlanie zysków z rabatu i współistnienia
||* Tworzenie biletów pomocy technicznej dla Centrum partnerskiego
||* Przeglądanie utworzonych biletów pomocy technicznej

## <a name="view-partner-center-insights-data"></a>Wyświetlanie danych szczegółowych informacji w centrum partnerskim

|**Role** | **Co możesz zrobić**|**Dowiedz się więcej**|
|------------------------------|:-------------------------|---|
|Executive — Podgląd raportów|Dostęp do wszystkich zestawów danych raportowania, tworzenie biletów pomocy technicznej dla partnerów, wyświetlanie utworzonych biletów pomocy technicznej|[Przegląd raportów pulpitu nawigacyjnego dostępnych w usłudze Partner Center Insights](pci-overview-report.md)
|Podgląd raportów|Dostęp do raportów danych z wyjątkiem dochodów i danych osobowych klientów i pracowników, tworzenie biletów pomocy technicznej dla partnerów, wyświetlanie tworzonych biletów pomocy technicznej|

## <a name="next-steps"></a>Następne kroki

- [Tworzenie kont użytkowników i przypisywanie ról oraz uprawnień](create-user-accounts-and-set-permissions.md)
- [Sprawdź informacje o koncie po zarejestrowaniu się w nowym programie partnerskim centrum](verification-responses.md)
