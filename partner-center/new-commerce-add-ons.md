---
title: Nowe dodatki handlowe
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o nowych doświadczeniach handlowych dotyczących zakupów dodatków.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 355c7ae3d4832764f6201613c040eebca998c3b6
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249336"
---
# <a name="introduction-new-commerce-add-ons"></a>Wprowadzenie: Nowe dodatki handlowe

**Odpowiednie role:** Agent administracyjny | Agent sprzedaży | Administrator globalny

> [!NOTE]
> Nowe zmiany w oknie handlowym są obecnie dostępne tylko dla partnerów, którzy są częścią nowego Microsoft 365/Dynamics 365 w wersji Technical Preview.

Partnerzy mogą kupować dodatki w nowym handlu, aby umożliwić innym usługom uzupełnienie wcześniej zakupionego produktu. Niektóre przykłady dodatków to wywoływanie planów, więcej miejsca na dysku lub inne funkcje, które można dodać, jeśli klient ma podstawowe usługi.

## <a name="add-ons-in-new-commerce"></a>Dodatki w nowym handlu

Nowe dodatki handlowe obejmują podobne koncepcje jak tradycyjne dodatki oparte na licencjach. Nowe dodatki handlowe, takie jak tradycyjne oparte na licencjach, obejmują koncepcję wymagań wstępnych. Wymagania wstępne to jednostki SKU produktu, które klient musi mieć, aby dodatek działał prawidłowo. Wymagania wstępne dodatku można znaleźć w interfejsach API wykazu dla danej sku i w interfejsie użytkownika Partner Center katalogu. Dodatki do zakupu wymagają, aby w dzierżawie klienta istniał co najmniej jeden z wymagań wstępnych.

Podstawowa różnica między tradycyjnymi i nowymi dodatkimi handlowymi polega na tym, **jak** są one kupowane. Partnerzy stosują dodatek do subskrypcji oferty podstawowej w tradycyjnych scenariuszach opartych na licencjach. Partner kupuje nowe dodatki handlowe z samego katalogu. To środowisko zakupu dopasowuje możliwości odnajdywania dodatków do oferty podstawowej, co ułatwia znajdowanie i kupowanie dodatków.

Wiele pojęć dotyczących sposobu działania dodatków z perspektywy usług pozostaje prawdziwych w tradycyjnym i nowym handlu. Zarówno tradycyjne, jak i nowe transakcje handlowe rejestrowały i aprowizowały usługi dodatku, aprowizowanie odbywa się w ten sam sposób w obu przypadkach. Ponadto usługi pojedynczego dodatku mogą uzupełniać więcej niż jedną podstawową bazę SKU produktu, z pomocą których ten dodatek jest przeznaczony.

## <a name="identifying-add-ons"></a>Identyfikowanie dodatków

Partnerzy mogą identyfikować dodatki i uzyskać listy wymagań wstępnych, przeglądając szczegóły jednostki SKU podczas uzyskiwania jednostki SKU za pośrednictwem interfejsu API. Dodatki są również identyfikowane na nowym cenniku opartym na licencjach handlowych w kolumnie Tagi. Macierz oferty zawiera listę wymagań wstępnych dla każdej dodatku sku produktu.

## <a name="purchasing-add-ons"></a>Dodatki do zakupów

Dodatki istnieją zarówno w tradycyjnych, opartych na licencjach, jak i w nowych usługach handlowych. Kluczową różnicą jest sposób, w jaki dodatki są odnalezione. Nowe dodatki handlowe są odnalezione i kupowane z katalogu, w tym samym miejscu, w którym znajdują się podstawowe oferty lub wymagania wstępne. Tradycyjne dodatki oparte na licencjach można odnajdywać i dodawać tylko po dodaniu ich do strony szczegółów subskrypcji oferty podstawowej. 

Dodatki nowego typu do obsługi handlu są odnalezione i zakupione w samym katalogu. Partnerzy mogą filtrować według nowych dodatków handlowych, wybierając menu rozwijane typu produktu. Produkty dodatku są identyfikowane przez ikonę informacji obok nazwy SKU produktu. Partnerzy mogą kliknąć tę ikonę, aby uzyskać więcej informacji na temat wymagań wstępnych dodatku.

Partnerzy mogą uzyskać więcej szczegółów na temat wymaganych  produktów dla dodatku, klikając pozycję Wyświetl zgodne podstawowe subskrypcje produktów, aby wyświetlić listę jednostki SKU produktu, które muszą istnieć, aby partner zakupił dany dodatek.

## <a name="add-on-enforcement"></a>Wymuszanie dodatków

Partnerzy zobaczą przydatne informacje na temat dodatków podczas próby zakupu nowego produktu dodatku handlowego, gdy klient nie ma wymagań wstępnych. Partnerzy mogą sprawdzać, czy wymagania wstępne dodatku istnieją w katalogu Partner Center i przeglądać strony. Jeśli dodatek nie ma wymagań wstępnych pomocy technicznej, interfejs użytkownika wyświetli komunikat "Dodatek nie jest dostępny bez zgodnego produktu podstawowego". Partnerzy korzystający z interfejsu API CreateCart zobaczą błąd w pozycji koszyka, jeśli dodatek nie ma wymaganych jednostki SKU produktu. Kod błędu zostanie 400041 z opisem "Dodatek nie jest dostępny do zakupu bez zgodnego produktu podstawowego".

## <a name="important-details-when-purchasing-add-ons"></a>Ważne szczegóły dotyczące zakupu dodatków

Dodatki są kupowane jako odrębne jednostki SKU produktów, jeśli klient spełnia wymagania wstępne. Subskrypcje dodatków mają własne odrębne dopasowanie terminu. Partnerzy, którzy kupią dodatki, zauważą termin i skojarzoną datę zakończenia mogą nie być takie same jak wymaganie wstępne. Tak długo, jak obie subskrypcje będą automatycznie odnawiać nowe warunki, wymagania wstępne i dodatki będą nadal działać prawidłowo. Jeśli partner zdecyduje się zakończyć okres wymagań wstępnych, nie odnawiając go automatycznie, dodatek powinien również zostać zaktualizowany, aby nie był automatycznie odnawiany na koniec okresu dodatku, jeśli partner stwierdzi, że nie jest już potrzebny.  Partnerzy konwertują produktową sku na wyższą wartość SKU, która ma już usługi dodatku, mogą złożyć żądanie obsługi z pomocą techniczną, aby wyłączyć dodatek.

Partnerzy muszą zarządzać terminami zakończenia dla dodatków, które pozyskują, aby zapewnić dopasowanie do podstawowych ofert zgodnie z potrzebami.
