---
title: Kupowanie Microsoft Azure rezerwacji dla klientów
description: Dowiedz się, jak kupować lub kupować rezerwacje platformy Azure w imieniu klientów w Partner Center. Wyświetla również rynki, na których rezerwacje platformy Azure są niedostępne.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: cd8a78edab25b94e678aafd61ca96e61a625fb07
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149540"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Kupowanie Microsoft Azure rezerwacji w imieniu klientów w Partner Center

**Odpowiednie role:** Agent administracyjny | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży | Administrator zarządzania użytkownikami

W tym artykule wyjaśniono, jak kupować lub kupować rezerwacje platformy Azure w imieniu klientów w Partner Center. Identyfikuje również rynki, na których rezerwacje platformy Azure są niedostępne.
 
> [!NOTE]
> Ten artykuł dotyczy tylko partnerów w programie Dostawca rozwiązań w chmurze (CSP). Klienci korzystający z innych typów subskrypcji (takich jak subskrypcje z płatnością zgodnie z użyciem, indywidualne, Umowa z Klientem Microsoft lub Enterprise Agreement) powinni zamiast tego przeczytać tę dokumentację rezerwacji platformy [Azure.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Zanim rozpoczniesz

Przed zakupem rezerwacji platformy Azure w imieniu klientów zapoznaj się z ważnymi informacjami poniżej. (Czy chcesz, aby klienci mogli kupować własne rezerwacje platformy Azure w ramach poprzedniej zakupionej dla nich subskrypcji platformy Azure? Zobacz [Temat Nadaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure).](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Jeśli i kiedy klient podpisze nową Umowa z Klientem Microsoft (zobacz Potwierdzanie akceptacji klienta [Umowa z Klientem Microsoft),](confirm-customer-agreement.md)musisz zakupić rezerwacje platformy Azure w ramach planu platformy Azure. Aby uzyskać więcej informacji, przeczytaj [Zakup planu platformy Azure.](purchase-azure-plan.md)

- Klienci muszą już mieć aktywną subskrypcję platformy Azure, aby można było kupić rezerwacje w ich imieniu
  
- Koszty subskrypcji oprogramowania, takie jak SQL Database lub oprogramowanie SUSE Linux, nie są uwzględniane w cenach rezerwacji platformy Azure

- Ceny komercyjne firmy Microsoft dla Ciebie nie obejmują podatków, chyba że Twoja lokalizacja to Brazylia. Jeśli Twoja lokalizacja to Brazylia, cena komercyjna uwzględnia odpowiednie podatki

- Agenci działu sprzedaży i pomocy technicznej potrzebują jawnego dostępu do subskrypcji platformy Azure Portal Azure, aby można było ją kupić lub zarządzać nimi w imieniu klienta, w tym w przypadku wymiany i zwrotów kosztów, w imieniu klienta  

- Jeśli jesteś dostawcą pośrednim i kupujesz rezerwacje platformy Azure za pośrednictwem usługi Azure Portal, partner rekordu (odsprzedawca pośredni) jest dziedziczony z wybranej Azure CSP subskrypcji.

- Partnera rekordów rezerwacji platformy Azure nie można zmienić po zakupie. Możesz anulować istniejącą rezerwację i zakupić nową rezerwację u nowego partnera rekordów.

- Jeśli klient chce przenieść subskrypcję platformy Azure z programu Direct lub EA do programu CSP, rezerwacje nie są przenoszone.

## <a name="azure-reservations-unavailable-markets"></a>Rezerwacje platformy Azure są niedostępne na rynkach

> [!IMPORTANT]
> Rezerwacje platformy Azure **nie są** dostępne na następujących rynkach:  
>  
> **Niedostępne rynki (w kolejności alfabetycznej)**
>
> |A do Gi   | Gr do Pal  | Pap–Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Wyspy alandzkie     | Grenlandia     | Papua Nowa Gwinea     |
> | Samoa Amerykańskie     | Grenada     | Wyspy Pitcairn     |
> | Andora     | Gwadelupa     | Reunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktyda     | Guernsey     | Saint Barthélemy   |
> | Antigua i Barbuda       | Gwinea     | Saint Lucia   |
> | Aruba       | Gwinea Bissau     | Saint-Martin   |
> | Azerbejdżan       | Gujana     | Saint Pierre i Miquelon   |
> | Benin     | Haiti       | Saint Vincent i Grenadyny     |
> | Bhutan     | Wyspy Heard i McDonalda       | Samoa     |
> | Bonaire     | Wyspa Man     | San Marino     |
> | Wyspa Bouveta     | Jan Mayen     | São Tomé i Prüncipe   |
> | Brytyjskie Terytorium Oceanu Indyjskiego       | Jersey     | Seszele   |
> | Brytyjskie Wyspy Dziewicze     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosowo     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Kambodża     | Lesotho     | Wyspy Salomona     |
> | Republika Środkowoafrykańska     | Liberia     | Somalia     |
> | Czad     | Madagaskar     | Georgia Południowa i Sandwich Południowy     |
> | Chiny     | Malawi     | Sudan Południowy     |
> | Wyspa Bożego Narodzenia     | Malediwy     | St Stana, Ascension, Tristan da Cunha     |
> | Wyspy Kokosowe (Keelinga)     | Mali     | Surinam     |
> | Komory     | Wyspy Marshalla     | Svalbard     |
> | Kongo     | Martynika     | Suazi     |
> | Kongo (DRK)     | Mauretania     | Timor-Leste   |
> | Wyspy Cooka     | Wyspa Majotta     | Togo   |
> | Dżibuti     | Mikronezja     | Tokelau   |
> | Dominika     | Montserrat     | Tonga   |
> | Gwinea Równikowa     | Mozambik     | Wyspy Turks i Caicos   |
> | Erytrea     | Myanmar     | Tuvalu   |
> | Falklandy     | Nauru     | Stany Zjednoczone Odlying Islands   |
> | Gujana Francuska     | Nowa Kaledonia     | Vanuatu   |
> | Polinezja Francuska     | Niger     | Watykan   |
> | Francuskie Terytoria Południowe i Antarktyczne     | Niue     | Wallis i Futuna   |
> | Gabon     | Norfolk     | Jemen   |
> | Gambia     | Mariany Północne     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Zakup rezerwacji platformy Azure

Wykonaj poniższe kroki, aby kupić Microsoft Azure rezerwacje w imieniu klientów w Partner Center. (Czy chcesz, aby klienci mogli kupować własne rezerwacje platformy Azure w ramach poprzedniej zakupionej dla nich subskrypcji platformy Azure? Zobacz [Temat Nadaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure).](give-customers-permission.md)

1. Wybierz **pozycję Klienci** z Partner Center menu.  

2. Na stronie **Klienci** znajdź klienta, który chce kupić rezerwacje platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć wiersz klienta.  

3. Wybierz **pozycję Dodaj produkty,** a następnie wybierz pozycję **Azure.** 

    a. Wybierz segment rynku klienta z **listy Segment.**

    b. Wybierz **pozycję Rezerwacje** z **listy Typ** produktu.

    c. Wybierz typ rezerwacji, który klient chce wybrać z **listy Typ rezerwacji.**

4. Rezerwacje platformy Azure muszą być skojarzone z aktywną subskrypcją platformy Azure. Wybierz subskrypcję klienta, do której chcesz dodać rezerwacje platformy Azure, z **listy Subskrypcja klienta.** 

   >[!IMPORTANT]
   >Jeśli klient nie ma jeszcze aktywnej subskrypcji platformy Azure, wybierz pozycję **Azure,** aby dodać ją teraz. 

5. Użyj filtrów, aby znaleźć rezerwacje platformy Azure na maszynach wirtualnych, które spełniają wymagania klienta.  

6. Po odnalezieniu rezerwacji, które chcesz kupić, wprowadź liczbę wystąpień zarezerwowanych, których klient będzie potrzebować w **Quantity,** a następnie wybierz pozycję **Dodaj do koszyka**.  

7. Powtarzaj kroki 5 i 6 do momentu dodania wszystkich niezbędnych elementów do zamówienia. Wybierz **pozycję Przejrzyj,** aby sprawdzić, czy zamówienie jest prawidłowe.  

8. Na **stronie Przeglądanie zamówień** możesz: 

    - Sprawdź lub zmień ilość wystąpień zarezerwowanych.

    - Wybierz zakres rezerwacji. Zakres rezerwacji może obejmować jedną subskrypcję lub wiele subskrypcji (zakres udostępniony). Jeśli zakres rezerwacji wynosi jedną subskrypcję, rabat za rezerwację jest stosowany tylko do tej subskrypcji. Jeśli wybierzesz opcję Udostępnione, rabat za rezerwację zostanie zastosowany do wszystkich subskrypcji w kontekście rozliczeń klienta. 

      >[!NOTE] 
      >Jeśli zdecydujesz się ograniczyć zakres rezerwacji do pojedynczej subskrypcji platformy Azure, może być konieczne zwiększenie limitu przydziału procesorów wirtualnych subskrypcji. Aby zwiększyć limit przydziału procesorów wirtualnych subskrypcji, musisz utworzyć żądanie obsługi w Azure Portal. Postępuj zgodnie z [instrukcjami w tym temacie,](/azure/azure-supportability/resource-manager-core-quotas-request) aby utworzyć żądanie. 

      >[!NOTE]   
      >Jeśli klient jest w ramach planu platformy Azure, **dla ustawienia Zakres**  zostanie ustawiona wartość **Udostępnione**. 

    - Jeśli jesteś partnerem dostawcy, wybierz odsprzedawcę, którego chcesz skojarzyć z produktem.
    
    - Jeśli rezerwacja platformy Azure obsługuje opcję Plan rozliczeniowy, z menu rozwijanego możesz wybrać częstotliwość rozliczeń jako miesięczną. 
    - Jeśli rezerwacja platformy Azure nie obsługuje opcji Plan rozliczeniowy, częstotliwość rozliczeń jest domyślnie rozliczeniowa. 

9. Wybierz **pozycję Kup,** aby kupić zamówienie. Szczegóły zamówienia, w tym numer zamówienia, są wyświetlane na **stronie Potwierdzanie.** Wybierz **pozycję Gotowe,** aby przejść do **strony Historii** zamówień. 

10. Aby zarządzać rezerwacją klienta w Azure Portal, znajdź klienta  na stronie Klienci, a następnie wybierz strzałkę w dół, aby rozwinąć wiersz klienta. Wybierz **Portal zarządzania Microsoft Azure,** aby otworzyć rekord klienta w Azure Portal.

## <a name="next-steps"></a>Następne kroki

|**Aby uzyskać informacje o**   |**Przeczytaj to**    |
|:-----------------------------|:-----------------|
|Rezerwacje platformy Azure w programie CSP — omówienie  | [Sprzedaż Microsoft Azure wystąpień zarezerwowanych](azure-reservations.md) |
|Zarządzanie rezerwacjami platformy Azure w usłudze Partner Center | [Zarządzanie rezerwacjami platformy Azure w usłudze Partner Center](azure-reservations-manage.md)
|Określanie prawidłowego rozmiaru maszyny wirtualnej i weryfikowanie użycia maszyny wirtualnej klienta   |[Rozmiar maszyny wirtualnej dla maksymalnego użycia rezerwacji platformy Azure](azure-usage.md)   |
|Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Partner Center API | [Informacje Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji Partner Center deweloperów   |
|Udzielanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure  | [Nadaj klientom uprawnienia do zakupu własnych rezerwacji platformy Azure](give-customers-permission.md)  |