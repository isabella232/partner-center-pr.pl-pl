---
title: Migrowanie systemu Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zapoznaj się z tematem, jak przeprowadzić migrację do wersji kwalifikowanej systemu Dynamics 365 Business Edition, zanim wygasną.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529278"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrate Dynamics 365 Business Edition Offers to newer versions (Migrowanie ofert usługi Dynamics 365 Business Edition do nowszych wersji)

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**
- Administrator globalny
- Administrator użytkowników
- Agent administracyjny
- Agent sprzedaży

Od 1 stycznia 2019 klienci korzystający z subskrypcji Dynamics 365 Business Edition nie mogą już odnowiać tych starszych ofert; istniejące subskrypcje nie będą odnawiane automatycznie po ich wygaśnięciu. Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "wygasa w dniu [Date]" z "autonews w dniu [Date]".

Aby zapewnić ciągłość dla klientów, należy przenieść te osoby z wygasanymi subskrypcjami do obsługiwanej opcji, wymienione poniżej. Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.

W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można wyszukać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false. W przypadku tej subskrypcji zostanie ustawiona wartość autorenew = false 1 stycznia 2019. Klientów można przenieść do nowego planu w dowolnym momencie. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Wycofywane wersje systemu Dynamics 365 Business

- Dynamics 365 dla finansów i operacji, wersja Business
- Dynamics 365 dla członków zespołu, wersja Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central — wersja Dynamics 365 Business Edition — nowe oferty

Nowe oferty usługi Dynamics Business Central umożliwiają klientom łączenie ich finansów, sprzedaży, usług i operacji w celu usprawnienia procesów biznesowych, poprawy interakcji z klientami oraz podejmowania lepszych decyzji. Usługa Dynamics 365 Business Central jest oparta na chmurze i dostępna za pośrednictwem partnerów programu Cloud Solution Provider (CSP).
Klienci korzystający z systemu Dynamics 365 Business Edition mogą otrzymywać obniżone ceny za okresy przejściowe dla nowych ofert w ramach usługi Business Central do 30 czerwca 2020.

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
