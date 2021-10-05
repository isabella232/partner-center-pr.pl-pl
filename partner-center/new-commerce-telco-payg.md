---
title: Nowy sklep telekomunikacyjny z płatnością zgodnie z ty-
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących kupowania ofert, które umożliwiają płatność zgodnie z modelem płatności zgodnie z modelem użytkowania.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8265cb3ce77183c4919e9b8e4e028bb66e8cd2f7
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/05/2021
ms.locfileid: "129452500"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Wprowadzenie: Nowa nadgorę handlowa dla programu telekomunikacyjnego z płatnością zgodnie z ty

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży
- Administrator globalny

> [!NOTE]
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Niektóre produkty oparte na licencjach obejmują usługi z przydzielonymi planami połączeń, które zwykle obejmują alokację na licencję na minuty miesięcznie, zwykle 120 na licencję. 

W tradycyjnych scenariuszach z partnerami opartymi na licencjach nie było możliwości włączenia użycia usług poza comiesięczne limity. Klienci potrzebują więcej niż 120 minut na zakup środków komunikacyjnych lub *comm samych* środków bezpośrednio od firmy Microsoft.  Te środki na komunikację nie były oferowane w Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Korzystanie z nowego programu telekomunikacyjnego do płatności zgodnie z użyciem

To ograniczenie zostało rozwiązane w nowym handlu, dzięki czemu partner może włączyć możliwości obsługi nadsyłania dla usług, które na to zezwalają. Partnerzy mogą kupować oferty, które obejmują możliwości w zakresie nadkupienia. Te oferty są identyfikowane w kolumnie tagów cennika *includeOverage*. SKU katalogu zawiera również właściwość, aby określić, czy SKU obsługuje możliwość przesłonić. Partnerzy po prostu kupują oferty, a system konfiguruje subskrypcję z opłatami za nadliczbowe, która nie jest kosztem, i nalicza opłaty tylko wtedy, gdy użytkownicy klienta zaćmią przydzielone miesięczne minuty połączenia, które są dostępne wraz z zakupioną ofertą. 

Partnerzy mogą określić, które jednostki SKU produktu obejmują możliwości dotyczące nadwyżeń według 

- Wyświetlanie jednostki SKU produktów w katalogu centrum partnerskiego
- Filtrowanie nowego cennika handlowego według **includesOverage** w kolumnie tagów

Partnerzy, którzy kupują produkty z nadkupieniami, mogą to umożliwić, korzystając z strony Zarządzanie **nadkupiami** na stronie Zarządzanie subskrypcjami. Interfejs zarządzania opłatami za nadsieć umożliwia partnerowi aktywowanie i przypisanie subskrypcji platformy Azure, do której będą przepływać opłaty za nadsieć. W dowolnym momencie partner może wyłączyć opłaty za zużycie, przypisując subskrypcję zużycia do wartości *Brak.* 

Partnerzy przypiszą lub wyłączą je za pomocą funkcji *Zarządzanie opłatami za* nadgorę na liście subskrypcji. Będzie ona dostępna tylko wtedy, gdy partner ma subskrypcje, które umożliwiają przesłonić. Miesięczne opłaty za nadsieć będą naliczane w ramach przypisanej subskrypcji i będą identyfikowane w pliku uzgodnień partnerów. Partnerzy mogą śledzić użycie opłat za użycie zasobów, odwiedzając możliwości zarządzania kosztami platformy Azure w Azure Portal. 

Partnerzy mogą śledzić użycie usług, przechodząc do Azure Portal i korzystając z funkcji i możliwości zarządzania kosztami. 

## <a name="important-details-about-overage"></a>Ważne szczegóły dotyczące naddatki

- Zakup opartego na licencji produktu SKU, który obejmuje możliwości przekupienia, spowoduje zakup tylko produktu opartego na licencjach. Partnerzy będą musieli po zakupie zrobić kolejny krok, aby włączyć nadpłacanie, przechodząc do strony zarządzania subskrypcjami i klikając pozycję **Zarządzaj nadkupami**
- Tylko agenci administracyjni dla partnera transakcji mogą włączyć najem na podstawie licencji. 
- Włączenie użycia overage spowoduje utworzenie bezpłatnego planu platformy Azure i skojarzonej domyślnej subskrypcji platformy Azure **Subskrypcji 1** przeznaczonej specjalnie na potrzeby użycia opłat za korzystanie z usług. Jeśli plan platformy Azure już istnieje, włączenie opłat za korzystanie z usług spowoduje utworzenie nowej subskrypcji w ramach istniejącego planu platformy Azure. Partnerzy mogą zawsze wyświetlać lub ponownie przypisać najechane na inne subskrypcje w **skrypcie Zarządzanie opłatami za nadsieć.** Klienci, którzy nie mają jeszcze planu platformy Azure (starszej wersji platformy Azure), będą musieli przejść do planu platformy Azure, zanim będą oni w stanie włączyć naduzycie.

Przypisanie nadsyłania jest określane przez *pierwszą regułę.* Jeśli partner zakupi subskrypcję E5 z planami połączeń dla nowego klienta, ten partner będzie miał nadsyłanie przypisane do subskrypcji zużycia. Jeśli drugi partner zakupi kolejną kopię planu E5 z planami połączeń, system będzie przestrzegać zakupów i przypisań pierwszego partnera. Partnerzy mogą zawsze *zarządzać nadgorą na* stronie subskrypcji, aby wyłączyć tę funkcję, przypisując jej do opcji *Brak.*

Ustawienia nadsyłania są na usługę na klienta. W tym samym czasie można przypisać tylko jedną subskrypcję z opłatami za nadsieć. Jeśli trzeba zmienić overage z jednego partnera na innego, trzy strony muszą najpierw wyrazić zgodę. Po wyrażania zgody istniejący partner może po prostu ustawić na wartość Brak na wartość *Brak,* co umożliwia drugiemu partnerowi ustawienie opłat za nadsieć na subskrypcję.

## <a name="telco-pay-as-you-go-apis"></a>Interfejsy API programu Telco z płatnością zgodnie z ty-

- [Właściwości SKU obejmują](/partner-center/develop/product-resources#sku) właściwość *consumptionType,* która ułatwia partnerowi określenie, czy w przypadku użycia za pomocą typu SKU
- [Uzyskaj informacje o nadpłacie,](/partner-center/develop/get-subscription-overage) aby dowiedzieć się, czy jakieś naduzycie jest obecnie ustawione dla klienta
- [Aktualizowanie nadgorętowych](/partner-center/develop/update-subscription-overage) zasobów w celu zaktualizowania opłat za korzystanie z usług klienta do subskrypcji platformy Azure lub ustawienia jej na wartość *Brak*
