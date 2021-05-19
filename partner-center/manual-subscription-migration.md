---
title: Migrowanie kwalifikowanych subskrypcji usługi Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przeprowadzić migrację z kwalifikowanych, podstawowych subskrypcji usługi Dynamics 365 do nowej subskrypcji przed wygaśnięciem istniejących subskrypcji.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151648"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrowanie usługi Dynamics 365 i planu Customer Engagement Plan z warstwy Podstawowa (zakwalifikowane oferty) do nowszych wersji

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży

Od 1 stycznia 2019 r. klienci z subskrypcjami usługi Dynamics 365 for Sales/Customer Engagement z subskrypcji Podstawowa (kwalifikowane oferty) nie mogą już odnawiać tych starszych ofert. Istniejące subskrypcje nie będą odnawiane automatycznie po wygaśnięciu. Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "Wygasa [data]" z "Automatyczne odnowienie [data]". 

Aby zapewnić ciągłość działania klientów, należy przejść te z wygasających subskrypcji do obsługiwanej opcji wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w roku, aby uniknąć jakichkolwiek błędów w usłudze dla klientów.

Jeśli używasz interfejsu API (CREST lub Partner Center), wygasające subskrypcje możesz znaleźć, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False. 1 stycznia 2019 r. dla określonych subskrypcji zostanie ustawiona wartość auto renew=False. Klientów można przenieść do nowego planu w dowolnym momencie. 

### <a name="the-dynamics-365-offers-being-retired"></a>Oferty usługi Dynamics 365 są wy wycofane

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta)
- Dynamics 365 for Sales Enterprise Edition CRMOL — podstawowa (oferta kwalifikowana) dla nauczycieli
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla uczniów
- Dynamics 365 for Sales Enterprise Edition (ceny dla instytucji rządowych) CRMOL — podstawowa (oferta kwalifikowana)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Kwalifikowana oferta)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students
- Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) od skoja września 2017 r. dla crm (oferta kwalifikowana)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana) dla nauczycieli i wykładowców
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana) dla uczniów
- Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) dla Add-On crm (oferta kwalifikowana)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (oferta kwalifikowana)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (ceny dla instytucji rządowych) CRMOL — podstawowa (oferta kwalifikowana)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Oferta kwalifikowana) dla uczniów
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (oferta kwalifikowana) dla nauczycieli i wykładowców
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Kwalifikowana oferta)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (cennik dla instytucji rządowych) z skoja stycznia 2017 r. dla crm (oferta kwalifikowana)
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (ceny dla instytucji rządowych) Add-On crm Basic (oferta kwalifikowana)
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Oferta kwalifikowana) dla uczniów
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana) dla nauczycieli i wykładowców



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Plan usługi Dynamics 365 for Sales/Customer Engagement z planów zastępczych w podstawową (kwalifikowanych ofertach)

**Wycofane oferty**   

- Dynamics 365 for Sales z usługi CRM Basic lub CRMOL Basic (oferta kwalifikowana)
- Dynamics 365 Customer Engagement Plan from CRM Basic lub CRMOL Basic (Oferta kwalifikowana)

**Opcje zamiany**
- Dynamics 365 for Sales Professional (NOWOŚĆ)
- Dynamics 365 for Sales Professional (NOWOŚĆ)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement Plan lub
- Członkowie zespołu usługi Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Przechodzenie klientów do nowych planów produktów

Przenoszenie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków w tej kolejności:

- Kupowanie nowej subskrypcji
- Ponowne przypisanie bieżących licencji użytkowników
- Anulowanie starej subskrypcji

## <a name="purchase-the-new-plan-for-your-customer"></a>Zakup nowego planu dla klienta

1. Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, którego chcesz przenieść do nowej subskrypcji.
2. Wybierz **pozycję Dodaj subskrypcję.**
3. Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**. 

Klient będzie teraz miał starą i nową subskrypcję. Następnym krokiem jest ponowne przypisanie licencji do użytkowników klienta.

1. Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, który przenosisz.
2. Wybierz **pozycję Użytkownicy i licencje.**
3. Aby ponownie przypisać licencję do użytkownika, wybierz użytkownika, a następnie wybierz pozycję **Zarządzaj licencjami.** 
4. Na stronie Zarządzanie **licencjami** wyczyść pole wyboru Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license (Plan usługi Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) (Plan usługi Dynamics 365 for Sales/ Customer Engagement plan from Basic (Qualified Offer) (Plan usługi Dynamics 365 for Sales/Customer Engagement z licencji Podstawowej (kwalifikowana oferta) i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący. 
5. Wybierz pozycję **Prześlij**. Zrobisz to dla każdego użytkownika, który potrzebuje nowej licencji. 

Po przeniesioniu licencji do nowej subskrypcji możesz anulować starą subskrypcję. 

1. Wybierz **pozycję Klienci** w lewym okienku nav, a następnie wybierz klienta, który przenosisz.
2. Na stronie szczegółów subskrypcji ustaw starą subskrypcję na wartość **Wstrzymano** i wybierz pozycję **Prześlij.**

Stara subskrypcja została wstrzymana, a nowa subskrypcja jest aktywna. Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni. Klient nie poniesie żadnych dodatkowych kosztów dla starej subskrypcji.
 

 



