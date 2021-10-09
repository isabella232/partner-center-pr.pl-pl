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
ms.openlocfilehash: 44e999987021ca450da1eb24cbd310a3e35b0873
ms.sourcegitcommit: cf73ea8967a285cc14b281e7b938962c02b18e67
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/08/2021
ms.locfileid: "129689704"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Wprowadzenie: Nowa nadgorę handlowa dla programu Telco z płatnością zgodnie z ty

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży
- Administrator globalny

> [!NOTE]
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Niektóre produkty oparte na licencjach obejmują usługi z przydzielonymi planami połączeń, które zwykle obejmują alokację na licencję na minuty miesięcznie, zwykle 120 na licencję. 

W tradycyjnych scenariuszach z partnerami opartymi na licencjach nie było możliwości włączenia użycia usługi poza miesięczne limity. Klienci potrzebują więcej niż 120 minut na zakup środków komunikacyjnych lub *comm samych* środków bezpośrednio od firmy Microsoft.  Te środki na komunikację nie były oferowane w Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Korzystanie z nowego programu telekomunikacyjnego do płatności zgodnie z użyciem

To ograniczenie zostało rozwiązane w nowym handlu, dzięki czemu partner może włączyć możliwości obsługi nadsyłania dla usług, które na to zezwalają. Partnerzy mogą kupować oferty, które obejmują możliwości w zakresie nadkupienia. Te oferty są identyfikowane w kolumnie tagów cennika *includeOverage*. SKU katalogu zawiera również właściwość, aby określić, czy SKU obsługuje możliwość przesłonić. Partnerzy po prostu kupują oferty, a system konfiguruje subskrypcję z opłatami za nadliczbowe, która nie jest kosztem i jest naliczana tylko wtedy, gdy użytkownicy klienta zajmą przydzielone miesięczne minuty połączeń, które są dostępne wraz z zakupioną ofertą. 

Partnerzy mogą określić, które jednostki SKU produktu obejmują możliwości dotyczące nadwyżeń według 

- Wyświetlanie jednostki SKU produktów w katalogu centrum partnerskiego
- Filtrowanie nowego cennika handlowego według **includesOverage** w kolumnie tagów

Partnerzy, którzy kupują produkty z nadkupieniami, mogą to umożliwić, korzystając z strony Zarządzanie **nadkupiami** na stronie Zarządzanie subskrypcjami. Interfejs zarządzania opłatami za nadsieć umożliwia partnerowi aktywowanie i przypisanie subskrypcji platformy Azure, do której będą przepływać opłaty za nadsieć. W dowolnym momencie partner może wyłączyć zasypkę, przypisując subskrypcję zużycia do wartości *Brak.* 

> [!NOTE]
> Zarządzanie nadgorętami wymaga możliwości utworzenia planu platformy Azure. Domyślnie partnerzy nie mogą aprowizować planów platformy Azure przy użyciu kont piaskownicy. Partnerzy, którzy muszą to zrobić za pomocą konta piaskownicy, muszą złożyć wniosek o dostęp. Więcej informacji można znaleźć w dokumentacji [piaskownicy planu platformy Azure.](/partner-center/develop/test-and-debug#azure-plan)

Partnerzy przypiszą lub wyłączą je za pomocą funkcji *Zarządzanie opłatami za* nadgorę na liście subskrypcji. Będzie ona dostępna tylko wtedy, gdy partner ma subskrypcje, które umożliwiają przesłonić. Miesięczne opłaty za nadsieć będą naliczane w ramach przypisanej subskrypcji i będą identyfikowane w pliku uzgodnień partnerów. Partnerzy mogą śledzić użycie usług overage, odwiedzając możliwości zarządzania kosztami platformy Azure w Azure Portal. 

Partnerzy mogą śledzić użycie usług, przechodząc do Azure Portal i korzystając z funkcji i możliwości zarządzania kosztami. 

## <a name="pricing-and-margins"></a>Ceny i marginesy

Opłaty za korzystanie z usługi Telco zgodnie z użyciem są naliczane na podstawie miesięcznego użycia, gdy klient używa przydzielonej ilości minut wywołania dla posiadanych planów. Partnerzy mogą odnaleźć i pobrać cennik tych opłat w witrynie [Microsoft Teams Telefon i calling.](https://www.microsoft.com/microsoft-teams/voice-calling) Partnerzy mogą przejść do strony **Zobacz stawki** dla miejsca, w którym chcesz dzwonić na tej stronie, aby pobrać i wyświetlić stawki dla różnych planów połączeń telefonicznych. 

Ceny i opłaty za za korzystanie z planu wywołań nie są specyficzne ani mniejsze dla odbiorców programu CSP, są niezależne od kanału. Nie ma żadnych rabatów ani marży dla opłat za korzystanie z usług WSP. 

## <a name="important-details-about-overage"></a>Ważne szczegóły dotyczące nadgoręt

- Zakup opartego na licencji produktu SKU, który obejmuje możliwości przekupienia, spowoduje zakup tylko produktu opartego na licencjach. Partnerzy będą musieli po zakupie zrobić kolejny krok, aby włączyć nadpłacanie, przechodząc do strony zarządzania subskrypcjami i klikając pozycję **Zarządzaj nadkupami**
- Tylko agenci administracyjni dla partnera transakcji mogą włączyć najem na podstawie licencji. 
- Włączenie użycia overage spowoduje utworzenie bezpłatnego planu platformy Azure i skojarzonej domyślnej subskrypcji platformy Azure **Subskrypcji 1** przeznaczonej specjalnie na potrzeby użycia opłat za korzystanie z usług. Jeśli plan platformy Azure już istnieje, włączenie opłat za korzystanie z usług spowoduje utworzenie nowej subskrypcji w ramach istniejącego planu platformy Azure. Partnerzy mogą zawsze wyświetlać lub ponownie przypisać najechane na inne subskrypcje w **skrypcie Zarządzanie opłatami za nadsieć.** Klienci, którzy nie mają jeszcze planu platformy Azure (starszej wersji platformy Azure), będą musieli przejść do planu platformy Azure, zanim będą oni w stanie włączyć naduzycie.

Przypisanie overage jest określane przez *pierwszą regułę.* Jeśli partner zakupi subskrypcję E5 z planami połączeń dla nowego klienta, ten partner będzie miał nadsyłanie przypisane do subskrypcji zużycia. Jeśli drugi partner zakupi kolejną kopię planu E5 z planami połączeń, system będzie przestrzegać zakupów i przypisań pierwszego partnera. Partnerzy mogą zawsze *zarządzać nadgorą na* stronie subskrypcji, aby wyłączyć tę funkcję, przypisując jej do opcji *Brak.*

Ustawienia nadsyłania są na usługę na klienta. W tym samym czasie można przypisać tylko jedną subskrypcję z opłatami za nadsieć. Jeśli trzeba zmienić overage z jednego partnera na innego, trzy zaangażowane strony muszą najpierw wyrazić zgodę. Po wyrażania zgody istniejący partner może po prostu ustawić na wartość Brak na wartość *Brak,* co umożliwia drugiemu partnerowi ustawienie opłat za nadsieć na subskrypcję.

## <a name="telco-pay-as-you-go-apis"></a>Telco — interfejsy API z płatnością zgodnie z ty-

- [Właściwości SKU obejmują](/partner-center/develop/product-resources#sku) właściwość *consumptionType,* która pomaga partnerowi określić, czy w przypadku użycia naduzytkowego w jej przypadku jest włączana wartość SKU
- [Uzyskaj informacje o nadpłacie,](/partner-center/develop/get-subscription-overage) aby dowiedzieć się, czy jakieś naduzycie jest obecnie ustawione dla klienta
- [Aktualizowanie nadgorętowych](/partner-center/develop/update-subscription-overage) zasobów w celu zaktualizowania opłat za korzystanie z usług klienta do subskrypcji platformy Azure lub ustawienia jej na wartość *Brak*
