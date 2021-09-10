---
title: Analizowanie subskrypcji i licencji
description: Dowiedz się, jak używać metryk na stronie analizy subskrypcji i licencji, aby zidentyfikować swoje sukcesy i obszary, które wymagają większej uwagi.
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: amitravat
ms.author: amrava
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 03/31/2021
ms.openlocfilehash: 393f0ee6c49cbbdf814a823f732bb4b92d4deb2e
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957982"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a>Analizowanie subskrypcji i licencji w celu podejmowania decyzji biznesowych i nowych celów

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży

Dane wpływają na decyzje biznesowe. Użyj metryk na stronie analizy **subskrypcji** i licencji, aby zidentyfikować swoje sukcesy i obszary, które wymagają większej uwagi. Użyj tych informacji podczas planowania nowych celów biznesowych.

**CSP TTM Revenue (USD)**: Ta metryka reprezentuje zagregowany przychód rozliczany w programie CSP (USD) dla ostatnich 12 miesięcy (TTM) dla kont lokalizacji partnera i globalnego konta partnera (PGA), z którym jest skojarzone to konto CSP. Jeśli masz inne konta CSP z innym programem PGA, musisz zalogować się do każdego z nich, aby wyświetlić odpowiednie zagregowane przychody z TTM.  Kliknij link szczegółów pobierania, aby uzyskać podział przychodu z TTM (USD) na identyfikator MPN.

>[!NOTE]
>Lokalne ceny walut (Legacy Commerce FX) w wersji komercyjnej są zarządzane w granicach +/-5% dolarów amerykańskich. Starszy kurs wymiany handlowej (FX) różni się od rozliczeń stawek FX używanych przez platformę Azure w nowoczesnym handlu. Stawki FX dla nowoczesnego handlu są oparte na stawkach MICROSOFT P&L (Reuters FX rates from Treasury Feed). Starsze stawki handlowe FX są poufne firmy Microsoft.


Pozostała część raportu może być przestawna w oparciu o następujące produkty:

 - **Dynamics 365:** dane usługi Dynamics 365  
 - **EMS:** Enterprise management Services  
 - **Microsoft 365:** Microsoft 365 danych  
 - **Office 365:** Office 365 danych  


## <a name="types-of-subscription-and-license-metrics-you-can-view"></a>Typy metryk subskrypcji i licencji, które można wyświetlić

Śledzimy następujące metryki:

**Podsumowanie**  
 - **Sprzedane subskrypcje:** liczba subskrypcji utworzonych w określonym przedziale czasu  
  
 - **Sprzedane licencje:** liczba sprzedanych licencji w określonym przedziale czasu  
  
 - **Subskrypcje odnawiane w ciągu 30** dni: liczba subskrypcji, w których stan jest aktywny w określonym przedziale czasu i gdzie **Autorenew** ma wartość true
 
 - **Aktywne subskrypcje:** subskrypcje, w których stan to **Aktywne**  
 
 - **Wstrzymane subskrypcje:** liczba zawieszonych subskrypcji, brak filtru daty  

**Podział produktów**
  
 - **Liczba subskrypcji:** 5 najliczbszych produktów posortowanych według sprzedanych subskrypcji  
 
 - **Liczba licencji:** 5 najlepiej sprzedawanych produktów według posortowanych licencji

**Przechowywanie subskrypcji**

 - **Odnowione subskrypcje:** subskrypcje odnawiane w ciągu ostatnich 30 dni  

**Rezygnacja z subskrypcji**  
 - **Nowe subskrypcje:** liczba nowych subskrypcji w tym okresie, z wyłączeniem ofert wersji próbnej  
 
 - **Anulowane aprowizowane subskrypcje:** liczba subskrypcji, dla których anulowano aprowizę lub które zostały wstrzymane według daty  

**Wstrzymane subskrypcje** 
 
 - Lista wszystkich subskrypcji ze stanem Wstrzymano **,** z wyjątkiem ofert wersji próbnej  
  
**Aktywne subskrypcje**

 - Lista wszystkich aktywnych subskrypcji  

**Konwersje subskrypcji w wersji próbnej**  

 - **Konwersja próbna:** liczba wszystkich aktywnych **subskrypcji,** w których nastąpiła konwersja wersji próbnej na konwersję w określonym przedziale czasu  

**Subskrypcje wersji próbnej kończące się w ciągu 30 dni**  

 - Lista wersji próbnych, które zostały rozpoczęte, gdzie data zakończenia wynosi w ciągu 30 dni, a z subskrypcją nie jest skojarzona żadna płatna data rozpoczęcia  



## <a name="next-steps"></a>Następne kroki

- [Analizowanie wydajności odsprzedawców pośrednich](analyze-indirect-resellers.md)