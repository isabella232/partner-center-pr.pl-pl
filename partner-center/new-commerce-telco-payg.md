---
title: Nowa płatność za usługi telekomunikacyjne w handlu zgodnie z modelem
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o nowych doświadczeniach handlowych w zakresie zakupów ofert, które umożliwiają płacenie zgodnie z zatygnieciem.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f934b8d858c1fc30d0140d19fb0697ba6bd9001
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959751"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Wprowadzenie: Nowa nadgorę handlowa dla płatności telekomunikacyjnych zgodnie z modelem pracy

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży
- Administrator globalny

> [!Note] 
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Niektóre produkty oparte na licencjach obejmują usługi z przydzielonymi planami połączeń. Te plany połączeń zwykle mają alokację na licencję na minuty miesięcznie, zazwyczaj 120 na licencję. 

W tradycyjnych scenariuszach partnerskich opartych na licencjach nie było możliwości włączenia użycia usług poza comiesięczne limity. Klienci potrzebują więcej niż 120 minut na zakup środków komunikacyjnych lub *comm bezpośrednio* od firmy Microsoft.  Te środki na komunikację nie były oferowane w Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Korzystanie z nowego programu telekomunikacyjnego do płatności zgodnie z użyciem ##

To ograniczenie zostało rozwiązane w nowym handlu, dzięki czemu partner może włączyć możliwości obsługi overage dla usług, które na to zezwalają. Partnerzy mogą kupować oferty, które obejmują możliwości w zakresie nadkupienia. Te oferty są identyfikowane w kolumnie tagów cennika *includeOverage*. SKU katalogu zawiera również właściwość, aby określić, że SKU obsługuje możliwość przesłonić. Partnerzy po prostu kupują oferty, a system konfiguruje subskrypcję i subskrypcję za nadliczbę, która nie jest kosztem i jest naliczana tylko wtedy, gdy użytkownicy klienta zasłanią przydzielone miesięczne minuty rozmów telefonicznych, które są dostępne wraz z zakupioną ofertą. 

Partnerzy mogą śledzić użycie overage, przechodząc do Azure Portal i korzystając z funkcji i możliwości zarządzania kosztami. Partnerzy mogą również w dowolnym momencie ustawić  na wartość Brak nadgoręć, jeśli chcą wyłączyć lub wyłączyć overage w dowolnym momencie.

Partnerzy mogą określić, które produkty obejmują możliwości obsługi nadwyrówek, wyświetlając jednostki SKU produktów w katalogu centrum partnerskiego. 

Partnerzy, którzy kupują produkty z nadaną  opłatą, umożliwiają uzyskanie dostępu do strony Zarządzanie nadgorą na stronie Zarządzanie subskrypcjami. Umożliwi to partnerowi aktywowanie opłat za nadsieć i przypisanie żądanej subskrypcji zużycia, do których będą przepływać opłaty za nadsieć. W dowolnym momencie partner może wyłączyć overage, przypisując subskrypcję zużycie do *wartości Brak.* 

Partnerzy przypiszą lub wyłączą je za pomocą funkcji *Zarządzanie opłatami za* nadgorętami na liście subskrypcji. Będzie ona dostępna tylko wtedy, gdy partner ma subskrypcje, które umożliwiają przesłonić. Miesięczne opłaty za nadsieć będą naliczane dla przypisanej subskrypcji i będą identyfikowane w pliku uzgodnień partnerów. Partnerzy mogą śledzić użycie overage, odwiedzając możliwości zarządzania kosztami platformy Azure w Azure Portal. 

## <a name="important-details-about-overage"></a>Ważne szczegóły dotyczące nadgorętowych danych ##

Zakup produktu sku, który umożliwia przesłonić, automatycznie zapewni, że klient partnera jest ustawiony do przepływu nadgoręć. Obejmuje to utworzenie bezpłatnego planu platformy Azure, skojarzonej domyślnej subskrypcji platformy Azure i subskrypcji przeznaczonej specjalnie na potrzeby użycia opłat za korzystanie z zasobów. Partnerzy mogą zobaczyć i przypisać subskrypcję, w ramach której mają być naliczane opłaty za nadsieć, w skrypcie Zarządzanie opłatami.

Przypisanie overage jest określane przez *pierwszą regułę.* Jeśli partner kupi usługę E5 z planami połączeń dla nowego klienta, ten partner będzie miał naduzycie przypisane do subskrypcji zużycia. Jeśli drugi partner zakupi kolejną kopię E5 z planami połączeń, system będzie przestrzegać zakupu i przypisania pierwszego partnera. Partnerzy mogą zawsze *zarządzać nadgorą* na stronie subskrypcji, aby ją wyłączyć lub wyłączyć, przypisując ją do *opcji Brak.*

Ustawienia overage są dostępne dla 1 usługi na klienta. Jeśli klient ma te same usługi opłat za nadsieć od różnych partnerów, w tym samym czasie można przypisać tylko jedną subskrypcję overage. Jeśli trzeba zmienić overage z jednego partnera na innego, trzy zaangażowane strony muszą najpierw wyrazić zgodę. Gdy istniejący partner będzie miał zgodę, może po prostu ustawić dla istniejącego partnera wartość *Brak,* co umożliwia drugiemu partnerowi ustawienie opłat za nadsieć na subskrypcję.

Obsługa interfejsu API dla funkcji płatności za telekomunikacyjne zgodnie z jenem obejmuje:

- Właściwości SKU, aby pomóc partnerowi w identyfikować, czy sku umożliwia przesłonić
- Nowy interfejs API do przypisywania opłat za nadsieć do istniejącej subskrypcji lub do ustawienia nadgoręt na *wartość Brak*
