---
title: Migrowanie subskrypcji do nowego handlu
ms.topic: article
ms.date: 10/04/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących migrowania subskrypcji.
author: iragulati1
ms.author: iragulati
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bad50c36cd0e0523fe70115e0b39d88e0e68ab68
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/05/2021
ms.locfileid: "129454668"
---
# <a name="introduction-migrate-subscriptions-to-new-commerce"></a>Wprowadzenie: Migrowanie subskrypcji do nowego handlu

**Odpowiednie role:** Agent administracyjny | Agent sprzedaży | Administrator globalny

> [!NOTE]
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.
Partnerzy mogą migrować subskrypcje do nowego handlu, jeśli subskrypcja spełnia kryteria uprawnień i jest dostępna oferta, na przykład do polubień.

## <a name="ineligible-subscriptions"></a>Subskrypcje, które nie są kwalifikowane ##

Nie wszystkie subskrypcje będą kwalifikować się do migracji w tej chwili. Obecnie nie są kwalifikowane następujące kategorie subskrypcji: 

- Nieaktywne subskrypcje (jeśli subskrypcja jest nieaktywna, nie zostaną wprowadzone żadne zmiany w usłudze) 

- Subskrypcje wersji próbnej (bez korzyści pieniężnych ani implikacji; oczekiwanie będzie, aby wersje próbne działały w starszej wersji) 

- Subskrypcje z promocjami (promocje w NCE są niezależne od tych promocji w starszej wersji) 

- Subskrypcje z dodatki (migracja subskrypcji z dodatki zostanie włączona później; w tej chwili nie możemy obsługiwać migracji współterminowej) 

- Subskrypcje dla odbiorców z organizacji gov, Edu lub Nonprofit (mapowanie kwalifikowanych ofert ze starszej wersji na NCE nie jest obsługiwane) 

- Wycofane lub przestarzałe subskrypcje (w przypadku tych subskrypcji nie będzie można polubić oferty istniejącej w nowym handlu) 

Migracje powyższych subskrypcji są obecnie poza zakresem tej funkcji. Ponadto pojedyncza subskrypcja będzie jednostką migracji, a nie partiami subskrypcji. 

## <a name="suspending-a-legacy-subscription-during-migration"></a>Zawieszanie starszej subskrypcji podczas migracji ##

Starsza subskrypcja zostanie wstrzymana tylko po pomyślnej ścieżce do nowego handlu aprowizowana dla subskrypcji. Ta funkcja zapobiegnie utracie usługi w przypadku jakichkolwiek blokad po zainicjowaniu migracji subskrypcji przez partnera. Ponadto w przypadku starszej i nowej subskrypcji handlowej nie będą występować żadne podwójne rozliczenia. Po zainicjowaniu migracji rozliczenia dla starszej subskrypcji zostaną zatrzymane, aby zapobiec nakładaniu się na rozliczenia dla subskrypcji NCE.

## <a name="billing-term-and-frequency"></a>Okres rozliczeniowy i częstotliwość ##

Okres rozliczeniowy i częstotliwość rozliczeń migrowanych subskrypcji pozostaną takie same jak okres rozliczeniowy i częstotliwość rozliczeń dla starszej subskrypcji. data zakończenia okresu pozostanie taka sama.

## <a name="new-commerce-promotions"></a>Nowe promocje handlowe ##

Subskrypcje w starszej wersji z promocjami nie kwalifikują się do migracji. Zmigrowane subskrypcje mogą kwalifikować się do nowych promocji wprowadzających do handlu. Promocje będą proporcjonalnie do pozostałej części okresu subskrypcji w punkcie migracji. 

## <a name="cancelling-subscriptions-or-decreasing-licenses"></a>Anulowanie subskrypcji lub zmniejszenie liczby licencji ##

Po migracji istnieje 72-godzinne okno anulowania. W ciągu tych 72 godzin partnerzy mogą anulować subskrypcję lub zmniejszyć liczbę licencji w tym oknie. Po 24-godzinnym okresie od ukończenia migracji anulowanie subskrypcji lub licencji będzie proporcjonalnie do jednego dnia użytkowania; po 48-godzinnym okresie od ukończenia migracji anulowanie subskrypcji lub licencji będzie proporcjonalnie do użycia przez dwa dni. 

## <a name="migration-history"></a>Historia migracji ##

Za pośrednictwem interfejsów API można uzyskać dostęp do szczegółów dotyczących historii migracji, takich jak terminy rozpoczęcia i zakończenia migracji, przy użyciu nowego pola GetMigration API i MigrationID. W interfejsie użytkownika identyfikator subskrypcji, z którego została zmigrowana nowa subskrypcja NCE, będzie widoczny w górnej części strony szczegółów, do której dostęp jest uzyskiwany po kliknięciu elementu wiersza subskrypcji na stronie "Subskrypcje" klienta. 

## <a name="apis"></a>Interfejsy API ##

W przypadku migracji subskrypcji podobnych do podobnych zostaną wydane 3 nowe interfejsy API REST. Pierwszy interfejs API "CheckMigration" sprawdzi uprawnienia do migracji dla subskrypcji. Drugi interfejs API "CreateMigration" utworzy migrację, jeśli subskrypcja kwalifikuje się. Trzeci interfejs API "GetMigration" umożliwi partnerom sprawdzanie stanu migracji. 
