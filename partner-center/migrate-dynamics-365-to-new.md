---
title: Migrowanie usługi Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przeprowadzić migrację kwalifikowanych ofert usługi Dynamics 365 Business Edition do nowszej wersji, zanim wygasną.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151529"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrate Dynamics 365 Business Edition Offers to newer versions (Migrowanie ofert usługi Dynamics 365 Business Edition do nowszych wersji)

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży

Od 1 stycznia 2019 r. klienci z subskrypcjami usługi Dynamics 365 Business Edition nie mogą już odnawiać tych starszych ofert. Istniejące subskrypcje nie będą odnawiane automatycznie po wygaśnięciu. Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "Wygasa [data]" z "Automatyczne odnowienie [data]".

Aby zapewnić ciągłość działania klientów, należy przejść te z wygasających subskrypcji do obsługiwanej opcji wymienionej poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w roku, aby uniknąć jakichkolwiek outages usługi dla klientów.

Jeśli używasz interfejsu API (CREST lub Partner Center), wygasające subskrypcje możesz znaleźć, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False. 1 stycznia 2019 r. dla określonych subskrypcji zostanie ustawiona opcja automatycznego odnawiania=Fałsz. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Wycofane wersje usługi Dynamics 365 Business

- Dynamics 365 for Finance and Operations, wersja Business
- Dynamics 365 for Team Members, wersja Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central — nowe oferty usługi Dynamics 365 Business Edition

Dzięki nowym ofertom usługi Dynamics Business Central klienci mogą łączyć swoje finanse, sprzedaż, usługi i operacje, aby usprawnić procesy biznesowe, usprawnić interakcje z klientami i podejmować lepsze decyzje. Usługa Dynamics 365 Business Central jest oparta na chmurze i jest dostępna tylko za pośrednictwem Dostawca rozwiązań w chmurze (CSP).
Klienci usługi Dynamics 365 Business Edition są uprawnieni do otrzymania cennika przejścia z rabatem dla nowych ofert usługi Business Central do 30 czerwca 2020 r.

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

Po przeniesionej licencji do nowej subskrypcji możesz anulować starą subskrypcję. 

1. Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, który przenosisz.
2. Na stronie szczegółów subskrypcji ustaw starą subskrypcję na **wstrzymaną i** wybierz pozycję **Prześlij.**

Stara subskrypcja została wstrzymana, a nowa subskrypcja jest aktywna. Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni. Klient nie poniesie żadnych dodatkowych kosztów dla starej subskrypcji.
