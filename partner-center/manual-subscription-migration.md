---
title: Migrowanie kwalifikowanych subskrypcji systemu Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przeprowadzić migrację z kwalifikowanych, podstawowych subskrypcji Dynamics 365 do nowej subskrypcji przed wygaśnięciem istniejących subskrypcji.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529281"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrowanie usługi Dynamics 365 i planu Customer Engagement Plan z warstwy Podstawowa (zakwalifikowane oferty) do nowszych wersji

**Dotyczy**

-  Centrum partnerskie

**Odpowiednie role**
-   Administrator globalny
-   Administrator użytkowników
-   Agent administracyjny
-   Agent sprzedaży

Od 1 stycznia 2019 klienci z planem Dynamics 365 for Sales/Customer Engagement z subskrypcji Basic (z ofertami kwalifikowanymi) nie mogą już odnowiać tych starszych ofert; istniejące subskrypcje nie będą odnawiane automatycznie po ich wygaśnięciu. Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "wygasa w dniu [Date]" z "autonews w dniu [Date]". 

Aby zapewnić ciągłość dla klientów, należy przenieść te osoby z wygasanymi subskrypcjami do obsługiwanej opcji, wymienione poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.

W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można wyszukać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false. W przypadku tej subskrypcji zostanie ustawiona wartość autorenew = false 1 stycznia 2019. Klientów można przenieść do nowego planu w dowolnym momencie. 

### <a name="the-dynamics-365-offers-being-retired"></a>Oferty dla systemu Dynamics 365 są wycofywane

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla wykładowców
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Oferta kwalifikowana) dla studentów
- Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) CRMOL Basic (kwalifikowana oferta)
- Dynamics 365 for Sales Enterprise Edition od wersji SA dla programu CRM Basic (kwalifikowana oferta)
- Dynamics 365 for Sales Enterprise Edition od wersji SA dla programu CRM Basic (kwalifikowana oferta) dla wykładowców
- Dynamics 365 for Sales Enterprise Edition od wersji SA for CRM Basic (Oferta kwalifikowana) dla studentów
- Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) z programu SA for CRM Basic (kwalifikowana oferta)
- Dynamics 365 for Sales Enterprise Edition Add-On dla programu CRM Basic (kwalifikowana oferta)
- Dynamics 365 for Sales Enterprise Edition Add-On dla programu CRM Basic (kwalifikowana oferta) dla wykładowców
- Dynamics 365 for Sales Enterprise Edition Add-On dla programu CRM Basic (Oferta kwalifikowana) dla studentów
- Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) Add-On dla programu CRM Basic (kwalifikowana oferta)
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kwalifikowana oferta)
- Dynamics 365 Customer Engagement plan Enterprise Edition (cennik dla instytucji rządowych) CRMOL Basic (kwalifikowana oferta)
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla studentów
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla wykładowców
- Dynamics 365 Customer Engagement plan Enterprise Edition od wersji SA dla programu CRM Basic (Oferta kwalifikowana)
- Dynamics 365 Customer Engagement plan Enterprise Edition (cennik dla instytucji rządowych) od SA for CRM Basic (kwalifikowana oferta)
- Dynamics 365 Customer Engagement plan Enterprise Edition from SA for CRM Basic (Oferta kwalifikowana) dla studentów
- Dynamics 365 Customer Engagement plan Enterprise Edition from SA for CRM Basic (Oferta kwalifikowana) dla nauczycieli lub wykładowców
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (Oferta kwalifikowana)
- Dynamics 365 Customer Engagement plan Enterprise Edition (cennik dla instytucji rządowych) Add-On dla programu CRM Basic (Oferta kwalifikowana)
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (Oferta kwalifikowana) dla studentów
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kwalifikowana oferta) dla wykładowców



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Plan "Dynamics 365 for Sales/Customer Engagement" z podstawowych (kwalifikowanych ofert) planów zastępczych

**Wycofane oferty**   

- Dynamics 365 for Sales z programu CRM Basic lub CRMOL Basic (kwalifikowana oferta)
- Plan zaangażowania klienta Dynamics 365 z programu CRM Basic lub CRMOL Basic (kwalifikowana oferta)

**Opcje zamiany**
- Dynamics 365 for Sales Professional (NOWOŚĆ)
- Dynamics 365 for Sales Professional (NOWOŚĆ)
- Dynamics 365 for Customer Service
- Plan zaangażowania klientów w usłudze Dynamics 365 lub
- Członkowie zespołu Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Przejście klientów do nowych planów produktu

Przeniesienie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących kroków w tej kolejności:

- Kup nową subskrypcję
- Ponowne przypisanie bieżących licencji użytkownika
- Anuluj starą subskrypcję

## <a name="purchase-the-new-plan-for-your-customer"></a>Kup nowy plan dla klienta

1. Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz klienta, który ma zostać przeniesiony do nowej subskrypcji.
2. Wybierz pozycję **Dodaj subskrypcję**.
3. Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**. 

Klient będzie miał teraz zarówno starą subskrypcję, jak i nową. Następnym krokiem jest ponowne przypisanie licencji do użytkowników klienta.

1. Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.
2. Wybierz pozycję **Użytkownicy i licencje**.
3. Aby ponownie przypisać licencję do użytkownika, wybierz użytkownika, a następnie wybierz pozycję **Zarządzaj licencjami**. 
4. Na stronie **Zarządzanie licencjami** Usuń zaznaczenie pola wyboru Dynamics 365 for Sales/Customer Engagement from Basic (kwalifikowana oferta), a następnie wybierz nowy plan usługi dla subskrypcji, do której będzie przenoszony klient. 
5. Wybierz pozycję **Prześlij**. Należy to zrobić dla każdego użytkownika, który potrzebuje nowej licencji. 

Po przeniesieniu licencji do nowej subskrypcji można anulować starą subskrypcję. 

1. Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.
2. Na stronie Szczegóły subskrypcji Ustaw starą subskrypcję na **zawieszoną** i wybierz pozycję **Prześlij**.

Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna. Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach. Klient nie będzie miał dodatkowych kosztów dla starej subskrypcji.
 

 



