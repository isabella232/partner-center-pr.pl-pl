---
title: Nowe dodatki handlowe
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących zakupów dodatków.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 01644e5d2dd2fe2057d223b62f1f4e9d6f9cd101
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/16/2021
ms.locfileid: "127876955"
---
# <a name="introduction-new-commerce-add-ons"></a>Wprowadzenie: Nowe dodatki handlowe

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży
- Administrator globalny

> [!Note] 
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Partnerzy mogą kupować dodatki w nowym handlu, aby umożliwić innym usługom uzupełnienie wcześniej zakupionego produktu. Niektóre przykłady to wywoływanie planów, więcej miejsca na dysku lub inne funkcje, które można dodać, jeśli klient ma usługi podstawowe.



## <a name="add-ons-in-new-commerce"></a>Dodatki w nowym handlu ## 

Nowe dodatki handlowe zawierają podobne pojęcia jak tradycyjne dodatki oparte na licencjach. Nowe dodatki handlowe, takie jak tradycyjne oparte na licencjach, obejmują koncepcję wymagań wstępnych. Są to jednostki SKU produktów, które klient musi mieć, aby dodatek działał poprawnie. Wymagania wstępne dotyczące dodatku można znaleźć w interfejsach API wykazu dla danej sku i w interfejsie użytkownika Partner Center katalogu. Dodatki do zakupów wymagają, aby w dzierżawie klienta istniał co najmniej jeden z wymagań wstępnych.
 
Główna różnica w zakupie dodatków między tradycyjnymi opartymi na licencjach i nowymi modelami handlu polega na *tym,* jak są one kupowane. W tradycyjnych opartych na licencjach partner stosuje dodatek do istniejącej subskrypcji oferty podstawowej. W przypadku nowego handlu partnerzy kupują dodatki z samego katalogu, nie mają już dwukierunkowego doświadczenia zakupowego dla podstawowych ofert i dodatków— wszystko znajduje się w katalogu w nowym handlu.

Wiele pojęć dotyczących sposobu działania dodatków, z perspektywy usług, pozostaje prawdziwych w tradycyjnym i nowym handlu. Zarówno rejestrowanie, jak i aprowizowanie usług dodatków nie różni się od tego, jak odbywa się aprowizowanie. Ponadto usługi pojedynczego dodatku mogą uzupełniać więcej niż jedną podstawową bazę SKU produktu, z pomocą których ten dodatek jest przeznaczony.

## <a name="identifying-add-ons"></a>Identyfikowanie dodatków ##

Partnerzy mogą identyfikować dodatki i uzyskać listy wymagań wstępnych, przeglądając szczegóły jednostki SKU podczas uzyskiwania jednostki SKU za pośrednictwem interfejsu API. Dodatki są również identyfikowane w nowym cenniku opartym na licencjach handlowych w kolumnie Tagi. Macierz oferty zawiera listę wymagań wstępnych dla każdej dodatku sku produktu.

## <a name="purchasing-add-ons"></a>Dodatki do zakupów ##

Dodatki istnieją zarówno w tradycyjnych, opartych na licencjach, jak i w nowych doświadczeniach handlowych. Kluczową różnicą jest to, że nowy handel umożliwia odnajdywanie i kupowanie z katalogu, w tym samym miejscu, w którym znajdują się podstawowe oferty lub wymagania wstępne. Tradycyjne dodatki oparte na licencjach można odnajdywać i kupować tylko, przechodząc na stronę szczegółów subskrypcji oferty podstawowej. Gdy dodatek zostanie tam wymieniony, partner stosuje odpowiedni dodatek.


Nowe dodatki do obsługi handlu są odnalezione i zakupione w samym katalogu. Partnerzy mogą filtrować według nowych dodatków handlowych, wybierając menu rozwijane typu produktu. Produkty dodatku są również łatwe do zobaczenia, ponieważ obok nich znajduje się ikona informacji, co objaśnia ich stan i znaczenie dodatku.


Partnerzy mogą uzyskać więcej szczegółów na temat wymaganych  produktów dla dodatku, klikając pozycję Wyświetl zgodne podstawowe subskrypcje produktów, aby wyświetlić listę jednostki SKU produktu, które muszą istnieć, aby partner zakupił dany dodatek.


## <a name="add-on-enforcement"></a>Wymuszanie dodatku ##

Partnerzy zobaczą błędy podczas próby zakupu nowego produktu dodatku handlowego, gdy klient nie ma żadnego z wymagań wstępnych. Partnerzy mogą zweryfikować, czy klient spełnia wymagania wstępne, wywołując interfejs API validateAddon w Centrum partnerskim.

## <a name="important-details-when-purchasing-add-ons"></a>Ważne szczegóły dotyczące zakupów dodatków ##

Dodatki są kupowane jako odrębne jednostki SKU produktów, jeśli klient spełnia wymagania wstępne. Subskrypcje dodatków mają własne odrębne dopasowanie terminu. Partnerzy, którzy kupią dodatki, zauważą termin i skojarzoną datę zakończenia mogą nie być takie same, jak w przypadku wymagań wstępnych. Tak długo, jak obie subskrypcje będą automatycznie odnawiane na nowe warunki, wymagania wstępne i dodatki będą działać prawidłowo. Jeśli partner zdecyduje się zakończyć okres wymagań wstępnych, nie odnawiając go automatycznie, dodatek powinien zostać zaktualizowany tak, aby nie był automatycznie odnawiany na końcu okresu dodatku, jeśli partner stwierdzi, że nie jest już potrzebny.  Partnerzy konwertują produktową sku na wyższą wartość SKU, która ma już usługi dodatku, mogą złożyć żądanie obsługi z pomocą techniczną, aby wyłączyć dodatek.

Partnerzy muszą zarządzać terminami zakończenia dla dodatków, które pozyskują, aby upewnić się, że istnieje dopasowanie do podstawowych ofert zgodnie z potrzebami.

