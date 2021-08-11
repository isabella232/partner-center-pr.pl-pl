---
title: Analizowanie subskrypcji i licencji
description: Dowiedz się, jak używać metryk na stronie analizy subskrypcji i licencji, aby identyfikować sukcesy i obszary, które wymagają większej uwagi.
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: amitravat
ms.author: amrava
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 03/31/2021
ms.openlocfilehash: 3ab138c1159304542b78faa20da635ce85cd97bdbba84b016b860632c537509e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115684854"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a>Analizowanie subskrypcji i licencji w celu podejmowania decyzji biznesowych i nowych celów

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny | Agent sprzedaży

Dane wpływają na decyzje biznesowe. Użyj metryk na stronie **analizy** subskrypcji i licencji, aby zidentyfikować sukcesy i obszary, które wymagają większej uwagi. Użyj tych informacji podczas planowania nowych celów biznesowych.

**CSP TTM Revenue (USD)**: ta metryka reprezentuje zagregowany przychód rozliczany w programie CSP (USD) dla ostatnich 12 miesięcy (TTM) dla kont lokalizacji partnera i globalnego konta partnera (PGA), z którym jest skojarzone to konto CSP. Jeśli masz inne konta CSP z innym pga, musisz zalogować się do każdego z nich, aby wyświetlić odpowiednie zagregowane przychody z TTM.  Kliknij link szczegółów pobierania, aby uzyskać podział przychodu z TTM (USD) na identyfikator MPN.

>[!NOTE]
>Lokalne ceny walut (starsza wersja commerce FX) w wersji komercyjnej są zarządzane w granicach +/-5% dolarów amerykańskich. Starszy kurs wymiany handlowej (FX) różni się od rozliczeń stawek FX używanych przez platformę Azure w nowoczesnym handlu. Stawki FX rozliczeń dla nowoczesnego handlu są oparte na stawkach Microsoft P&L (reuters FX rates from Treasury feed). Starsze stawki handlowe FX są poufne przez firmę Microsoft.


Pozostała część raportu może być przestawna w oparciu o następujące produkty:

 - **Dynamics 365:** dane usługi Dynamics 365  
 - **EMS:** Enterprise danych usług zarządzania  
 - **Microsoft 365:** Microsoft 365 danych  
 - **Office 365:** Office 365 danych  


## <a name="types-of-subscription-and-license-metrics-you-can-view"></a>Typy metryk subskrypcji i licencji, które można wyświetlić

Śledzimy następujące metryki:

**Podsumowanie**  
 - **Sprzedane subskrypcje:** liczba subskrypcji utworzonych w określonym przedziale czasu  
  
 - **Sprzedane licencje:** liczba sprzedanych licencji w określonym przedziale czasu  
  
 - **Subskrypcje odnawiane w ciągu 30** dni: liczba subskrypcji, w których stan jest aktywny przez określony okres i gdzie **autorenew** ma wartość true
 
 - **Aktywne subskrypcje:** subskrypcje, w których stan to **Aktywne**  
 
 - **Wstrzymane subskrypcje:** liczba wstrzymanych subskrypcji, brak filtru daty  

**Podział produktów**
  
 - **Liczba subskrypcji:** 5 najliczbowych produktów posortowanych według sprzedanych subskrypcji  
 
 - **Liczba licencji:** 5 najlepiej sprzedawanych produktów według posortowanych licencji

**Przechowywanie subskrypcji**

 - **Odnowione subskrypcje:** subskrypcje odnawiane w ciągu ostatnich 30 dni  

**Rezygnacja z subskrypcji**  
 - **Nowe subskrypcje:** liczba nowych subskrypcji w okresie z wyłączeniem ofert wersji próbnej  
 
 - **Anulowano aprowizowane subskrypcje:** liczba subskrypcji anulowanych lub zawieszonych według daty  

**Wstrzymane subskrypcje** 
 
 - Lista wszystkich subskrypcji ze stanem **Wstrzymano** z wyłączeniem ofert wersji próbnej  
  
**Aktywne subskrypcje**

 - Lista wszystkich aktywnych subskrypcji  

**Konwersje subskrypcji w wersji próbnej**  

 - **Konwersja wersji** próbnej: liczba wszystkich aktywnych **subskrypcji,** w których nastąpiła konwersja wersji próbnej płatnej w określonym przedziale czasu  

**Subskrypcje wersji próbnej kończące się na 30 dni**  

 - Lista prób, które zostały rozpoczęte, gdzie data zakończenia wynosi w ciągu 30 dni i nie ma płatnej daty rozpoczęcia skojarzonej z subskrypcją  



## <a name="next-steps"></a>Następne kroki

- [Analizowanie wydajności odsprzedawców pośrednich](analyze-indirect-resellers.md)