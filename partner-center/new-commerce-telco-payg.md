---
title: Nowe telekomunikacyjne telekomunikacyjne opłaty zgodnie z jenem
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących kupowania ofert, które umożliwiają płacenie zgodnie z nadkupią.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f934b8d858c1fc30d0140d19fb0697ba6bd9001
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/03/2021
ms.locfileid: "123458293"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Wprowadzenie: Nowe opłaty za nadgorę handlową za telekomunikacyjną płatność zgodnie z jenem

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży
- Administrator globalny

> [!Note] 
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Niektóre produkty oparte na licencjach obejmują usługi z przydzielonymi planami połączeń. Te plany połączeń zwykle mają alokację na licencję na minuty miesięcznie, zwykle 120 na licencję. 

W tradycyjnych scenariuszach z partnerami opartymi na licencjach nie było możliwości włączenia użycia usług poza comiesięczne limity. Klienci potrzebują więcej niż 120 minut na zakup środków komunikacyjnych lub *comm samych* środków bezpośrednio od firmy Microsoft.  Te środki na komunikację nie były oferowane w Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Korzystanie z nowego programu telekomunikacyjnego do handlu w przypadku płatności zgodnie z ich użyciem ##

To ograniczenie zostało rozwiązane w nowym handlu, dzięki czemu partner może włączyć możliwości obsługi nadsyłania dla usług, które na to zezwalają. Partnerzy mogą kupować oferty, które obejmują możliwości w zakresie nadkupienia. Te oferty są identyfikowane w kolumnie tagów cennika *includeOverage*. SKU katalogu zawiera również właściwość, aby określić, czy SKU obsługuje możliwość przesłonić. Partnerzy po prostu kupują oferty, a system konfiguruje i subskrypcję opłat za nadliczbowych, które nie są kosztami i są naliczane tylko wtedy, gdy użytkownicy klienta zajmą przydzielone miesięczne minuty połączeń, które są dostępne wraz z zakupioną ofertą. 

Partnerzy mogą śledzić użycie zasobów, przechodząc do Azure Portal i korzystając z funkcji i możliwości zarządzania kosztami. Partnerzy mogą również w dowolnym momencie ustawić  na wartość Brak nadgoręć, jeśli chcą wyłączyć lub wyłączyć nadgorę w dowolnym momencie.

Partnerzy mogą określić, które produkty obejmują możliwości obsługi nadwyżeń, wyświetlając jednostki SKU produktów katalogu partnerów. 

Partnerzy, którzy kupują produkty z nadkupikami, włączyli najechanie na zamówienie, korzystając z strony Zarządzanie nadkupiami na stronie Zarządzanie subskrypcjami.  Umożliwi to partnerowi aktywowanie opłat za korzystanie z usług i przypisanie żądanej subskrypcji zużycia, do których będą przepływać opłaty za nadsieć. W dowolnym momencie partner może wyłączyć zamówienie, przypisując subskrypcję zużycia do wartości *Brak.* 

Partnerzy przypiszą lub wyłączą je za pomocą funkcji *Zarządzanie opłatami za* nadgorę na liście subskrypcji. Będzie ona dostępna tylko wtedy, gdy partner ma subskrypcje, które umożliwiają przesłonić. Miesięczne opłaty za nadsieć będą naliczane w ramach przypisanej subskrypcji i będą identyfikowane w pliku uzgodnień partnerów. Partnerzy mogą śledzić użycie opłat za użycie overage, odwiedzając możliwości zarządzania kosztami platformy Azure w Azure Portal. 

## <a name="important-details-about-overage"></a>Ważne szczegóły dotyczące naddatki ##

Zakup produktu sku, który umożliwia naduzycie, automatycznie zapewni, że klient partnera jest ustawiony do obsługi przepływu za dużo pracy. Obejmuje to utworzenie bezpłatnego planu platformy Azure, skojarzonej domyślnej subskrypcji platformy Azure i subskrypcji przeznaczonej specjalnie do użycia opłat za korzystanie z opłat za korzystanie z usług. Partnerzy mogą zobaczyć i przypisać subskrypcję, w ramach której mają być naliczane opłaty za nad służące do zarządzania opłatami.

Przypisanie nadsyłania jest określane przez *pierwszą regułę.* Jeśli partner zakupi subskrypcję E5 z planami połączeń dla nowego klienta, ten partner będzie miał nadsyłanie przypisane do subskrypcji zużycia. Jeśli drugi partner zakupi kolejną kopię planu E5 z planami połączeń, system będzie przestrzegać zakupów i przypisań pierwszego partnera. Partnerzy mogą zawsze *zarządzać nadgorą na* stronie subskrypcji, aby wyłączyć tę funkcję, przypisując jej do opcji *Brak.*

Ustawienia nadsyłania są na usługę na klienta. Jeśli klient ma te same usługi opłat za nadanych przez różnych partnerów, w tym samym czasie można przypisać tylko jedną subskrypcję. Jeśli trzeba zmienić overage z jednego partnera na innego, trzy strony muszą najpierw wyrazić zgodę. Po wyrażania zgody istniejący partner może po prostu ustawić na wartość Brak na wartość *Brak,* co umożliwia drugiemu partnerowi ustawienie opłat za nadsieć na subskrypcję.

Obsługa interfejsu API dla funkcji telco pay as you go obejmuje:

- Właściwości SKU, które ułatwiają partnerowi określenie, czy taku umożliwia przesłonić
- Nowy interfejs API do przypisywania opłat za nadsieć do istniejącej subskrypcji lub do ustawienia opłat za nadgorę na *wartość Brak*
