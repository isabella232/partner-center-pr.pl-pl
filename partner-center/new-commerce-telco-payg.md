---
title: Nowy sklep telekomunikacyjny z płatnością zgodnie z ty
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących zakupów ofert, które umożliwiają płacenie zgodnie z modelem płatności zgodnie z modelem użytkowania.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6abf0a837758819fba8c3a584ba68216657a2b9
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593246"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Wprowadzenie: Nowa nadgorę handlowa dla programu Telco z płatnością zgodnie z ty

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży
- Administrator globalny

> [!NOTE]
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Niektóre produkty oparte na licencjach obejmują usługi z przydzielonymi planami połączeń, które zwykle obejmują alokację na licencję na minuty miesięcznie, zazwyczaj 120 na licencję. 

W tradycyjnych scenariuszach partnerskich opartych na licencjach nie było możliwości włączenia użycia usług poza comiesięczne limity. Klienci potrzebują więcej niż 120 minut na zakup środków komunikacyjnych lub *comm bezpośrednio* od firmy Microsoft.  Te środki na komunikację nie były oferowane w Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Korzystanie z nowego programu telekomunikacyjnego z płatnością zgodnie z użyciem

To ograniczenie zostało rozwiązane w nowym handlu, dzięki czemu partner może włączyć możliwości obsługi overage dla usług, które na to zezwalają. Partnerzy mogą kupować oferty, które obejmują możliwości w zakresie nadkupienia. Te oferty są identyfikowane w kolumnie tagów cennika *IncludeOverage*. SKU wykazu zawiera również właściwość, aby określić, że SKU obsługuje możliwość przesłonić. Partnerzy po prostu kupują oferty, a system konfiguruje subskrypcję overage, która nie jest kosztem i jest naliczana tylko wtedy, gdy użytkownicy klienta zasłanią przydzielone miesięczne minuty rozmów telefonicznych, które są dostępne wraz z zakupioną ofertą. 

Partnerzy mogą określić, które jednostki SKU produktu obejmują możliwości dotyczące przesłoni 

- Wyświetlanie jednostki SKU produktów w katalogu centrum partnerskiego
- Filtrowanie nowego cennika handlowego według **wartości includesOverage w** kolumnie tagów

Partnerzy, którzy kupują produkty z nadaną opłatą, mogą to umożliwić, korzystając z strony Zarządzanie opłatami za nadgorę **na** stronie Zarządzanie subskrypcjami. Interfejs zarządzania opłatami za nadsieć umożliwia partnerowi aktywowanie i przypisanie subskrypcji platformy Azure, do której będą przepływać opłaty za za korzystanie z opłat za korzystanie z usług. W dowolnym momencie partner może wyłączyć overage, przypisując subskrypcję zużycie do *wartości Brak.* 

> [!NOTE]
> Zarządzanie overage wymaga możliwości utworzenia planu platformy Azure. Domyślnie partnerzy nie mogą aprowizować planów platformy Azure przy użyciu kont piaskownicy. Partnerzy, którzy muszą to zrobić za pomocą konta piaskownicy, muszą złożyć wniosek o dostęp. Więcej informacji o infrastrukturze można znaleźć w dokumentacji piaskownicy [planu platformy Azure.](/partner-center/develop/test-and-debug#azure-plan)

Partnerzy przypiszą lub wyłączą je za pomocą funkcji *Zarządzanie opłatami za* nadgorętami na liście subskrypcji. Będzie ona dostępna tylko wtedy, gdy partner ma subskrypcje, które umożliwiają przesłonić. Miesięczne opłaty za nadsieć będą naliczane dla przypisanej subskrypcji i będą identyfikowane w pliku uzgodnień partnerów. Partnerzy mogą śledzić użycie overage, odwiedzając możliwości zarządzania kosztami platformy Azure w Azure Portal. 

Partnerzy mogą śledzić użycie nadgorętowe, przechodząc do Azure Portal i korzystając z funkcji i możliwości zarządzania kosztami. 

## <a name="important-details-about-overage"></a>Ważne szczegóły dotyczące nadgoręt

- Zakup opartego na licencji produktu SKU, który obejmuje możliwości przesłoni, spowoduje zakup tylko produktu opartego na licencjach. Partnerzy będą musieli po zakupie zrobić kolejny krok, aby włączyć overage, przechodząc do strony zarządzania subskrypcjami i klikając pozycję **Zarządzaj przesłoną**
- Tylko agenci administracyjni dla partnera transakcji mogą włączyć obsługę overage po zakupie opartym na licencjach. 
- Włączenie nadsyłania spowoduje utworzenie bezpłatnego planu platformy Azure i skojarzonej domyślnej subskrypcji platformy Azure **Subskrypcji 1** przeznaczonej specjalnie na potrzeby użycia opłat za korzystanie z zasobów. Jeśli plan platformy Azure już istnieje, włączenie opłat za korzystanie z zasobów spowoduje utworzenie nowej subskrypcji w ramach istniejącego planu platformy Azure. Partnerzy mogą zawsze wyświetlać lub ponownie przypisać nadgorę do innych subskrypcji w **skrypcie Zarządzanie przesłoną.** Klienci, którzy nie mają jeszcze planu platformy Azure (starszej wersji platformy Azure), będą musieli przejść do planu platformy Azure, zanim będą oni w stanie włączyć przesłoną.

Przypisanie overage jest określane przez *pierwszą regułę.* Jeśli partner kupi usługę E5 z planami połączeń dla nowego klienta, ten partner będzie miał naduzycie przypisane do subskrypcji zużycia. Jeśli drugi partner zakupi kolejną kopię E5 z planami połączeń, system będzie przestrzegać zakupu i przypisania pierwszego partnera. Partnerzy mogą zawsze *zarządzać nadgorą na* stronie subskrypcji, aby ją wyłączyć lub wyłączyć, przypisując ją do *opcji Brak.*

Ustawienia dotyczące nadgorętowania są dostępne dla 1 usługi na klienta. W tym samym czasie można przypisać tylko jedną subskrypcję z opłatami za nadsieć. Jeśli trzeba zmienić overage z jednego partnera na innego, trzy zaangażowane strony muszą najpierw wyrazić zgodę. Gdy istniejący partner będzie miał zgodę, może po prostu ustawić dla istniejącego partnera wartość *Brak,* co umożliwia drugiemu partnerowi ustawienie opłat za nadsieć na subskrypcję.

## <a name="telco-pay-as-you-go-apis"></a>Interfejsy API programu Telco z płatnością zgodnie z ty

- [Właściwości SKU](/partner-center/develop/product-resources#sku) obejmują właściwość *consumptionType,* która ułatwia partnerowi określenie, czy ta wartość umożliwia przesuniecie
- [Uzyskaj informacje o nadpłacie,](/partner-center/develop/get-subscription-overage) aby dowiedzieć się, czy jakieś zasypki są obecnie ustawione dla klienta
- [Aktualizowanie nadgorętowych](/partner-center/develop/update-subscription-overage) zasobów w celu zaktualizowania opłat za nadsieć klienta do subskrypcji platformy Azure lub ustawienia jej na wartość *Brak*
