---
title: Kup rezerwacje Microsoft Azure dla klientów
description: Dowiedz się, jak kupować i kupować rezerwacje platformy Azure w imieniu klientów w centrum partnerskim. Zawiera również listę rynków, w których rezerwacje platformy Azure są niedostępne.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 0e81a9561f3749aab281bb4ebd7cd0c38540ff31
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534611"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Kup rezerwacje Microsoft Azure w imieniu klientów w centrum partnerskim

**Odpowiednie role**

- Agent administracyjny
- Administrator globalny
- Agent pomocy technicznej
- Agent sprzedaży
- Administrator zarządzania użytkownikami

W tym artykule wyjaśniono, jak kupić lub zakupić rezerwacje platformy Azure w imieniu klientów w centrum partnerskim. Identyfikuje także rynki, w których rezerwacje platformy Azure są niedostępne.
 
> [!NOTE]
> Ten artykuł ma zastosowanie tylko do partnerów w programie Cloud Solution Provider (CSP). Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).

## <a name="before-you-begin"></a>Przed rozpoczęciem

Zapoznaj się z poniższymi informacjami poniżej przed zakupem rezerwacji platformy Azure w imieniu klientów. (Czy chcesz, aby klienci mogli kupować własne rezerwacje platformy Azure od poprzedniej subskrypcji platformy Azure, która została zakupiona? Zobacz [nadawanie klientom uprawnień do kupowania własnych rezerwacji platformy Azure](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).

- Jeśli i gdy klient zarejestruje nową umowę klienta firmy Microsoft (patrz [potwierdzenie akceptacji klienta przez umowę klienta firmy Microsoft](confirm-customer-agreement.md)), należy zakupić rezerwacje platformy Azure w ramach planu platformy Azure. Aby uzyskać więcej informacji, zapoznaj się z artykułem [zakup planu platformy Azure](purchase-azure-plan.md).

- Klienci muszą mieć już aktywną subskrypcję platformy Azure, aby można było zakupić rezerwacje w ich imieniu
  
- Koszty subskrypcji oprogramowania, takie jak SQL Database lub oprogramowanie SUSE Linux nie są uwzględnione w cenach rezerwacji platformy Azure

- Komercyjne ceny firmy Microsoft nie obejmują podatków, chyba że lokalizacja to Brazylia. Jeśli Twoja lokalizacja to Brazylia, Cena handlowa obejmuje odpowiednie podatki

- Agenci sprzedaży i pomocy technicznej potrzebują jawnego dostępu do subskrypcji platformy Azure, dzięki czemu mogą oni kupować i zarządzać nimi w Azure Portal i żądania pomocy technicznej dotyczącej plików, w tym za wymianę i zwroty w imieniu klienta  

- Jeśli jesteś dostawcą pośrednim i kupisz rezerwacje platformy Azure za pośrednictwem Azure Portal, partner rekordu (pośredni odsprzedawca) jest Dziedziczony z wybranej subskrypcji platformy Azure CSP.

- Nie można zmienić typu po zakupie partnera rekordu dla rezerwacji platformy Azure. Istnieje możliwość anulowania istniejącej rezerwacji i zakupu nowego partnera z nowym partnerem rekordów.

- Jeśli klient chce przenieść subskrypcję platformy Azure z bezpośredniego lub EA do dostawcy usług kryptograficznych, rezerwacje nie zostaną przesłane.

## <a name="azure-reservations-unavailable-markets"></a>Platforma Azure zastrzega niedostępne rynki

> [!IMPORTANT]
> Rezerwacje platformy Azure **nie są** dostępne na następujących rynkach:  
>  
> **Dostępne rynki (w porządku alfabetycznym)**
>
> |A do gi   | Gr do PAL  | PAP do Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Wyspy Åland     | Grenlandia     | Papua Nowa Gwinea     |
> | Samoa Amerykańskie     | Grenada     | Wyspy Pitcairn     |
> | Andora     | Gwadelupa     | Reunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktyda     | Guernsey     | Saint Barthélemy   |
> | Antigua i Barbuda       | Gwinea     | Saint Lucia   |
> | Aruba       | Gwinea Bissau     | Saint-Martin   |
> | Azerbejdżan       | Gujana     | Saint-Pierre i Miquelon   |
> | Benin     | Haiti       | Saint Vincent i Grenadyny     |
> | Bhutan     | Wyspy Heard i McDonald       | Samoa     |
> | Bonaire     | Wyspa Man     | San Marino     |
> | Wyspa Bouveta     | Jan Mayen     | Wyspy Świętego Tomasza i Książęca   |
> | Brytyjskie Terytorium Oceanu Indyjskiego       | Jersey     | Seszele   |
> | Brytyjskie Wyspy Dziewicze     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosowo     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Kambodża     | Lesotho     | Wyspy Salomona     |
> | Republika Środkowoafrykańska     | Liberia     | Somalia     |
> | Czad     | Madagaskar     | Wyspy Georgia Południowa i Sandwich Południowy     |
> | Chiny     | Malawi     | Sudan Południowy     |
> | Wyspa Bożego Narodzenia     | Malediwy     | Święta Helena, Wyspa Wniebowstąpienia, Tristan da Cunha     |
> | Wyspy Kokosowe (Keelinga)     | Mali     | Surinam     |
> | Komory     | Wyspy Marshalla     | Svalbard     |
> | Kongo     | Martynika     | Suazi     |
> | Kongo (DRK)     | Mauretania     | Timor-Leste   |
> | Wyspy Cooka     | Wyspa Majotta     | Togo   |
> | Dżibuti     | Mikronezja     | Tokelau   |
> | Dominika     | Montserrat     | Tonga   |
> | Gwinea Równikowa     | Mozambik     | Wyspy Turks i Caicos   |
> | Erytrea     | Myanmar     | Tuvalu   |
> | Falklandy     | Nauru     | Stany Zjednoczone — Dalekie Wyspy Mniejsze   |
> | Gujana Francuska     | Nowa Kaledonia     | Vanuatu   |
> | Polinezja Francuska     | Niger     | Watykan   |
> | Francuskie Terytoria Południowe i Antarktyczne     | Niue     | Wallis i Futuna   |
> | Gabon     | Norfolk     | Jemen   |
> | Gambia     | Mariany Północne     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Kup rezerwacje platformy Azure

Postępuj zgodnie z poniższymi instrukcjami, aby zakupić Microsoft Azure rezerwacje w imieniu klientów w centrum partnerskim. (Czy chcesz, aby klienci mogli kupować własne rezerwacje platformy Azure od poprzedniej subskrypcji platformy Azure, która została zakupiona? Zobacz [nadawanie klientom uprawnień do kupowania własnych rezerwacji platformy Azure](give-customers-permission.md).

1. Wybierz pozycję **klienci** z menu Centrum partnerskiego.  

2. Na stronie **klienci** Znajdź klienta, który chce zakupić rezerwacje platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć wiersz klienta.  

3. Wybierz pozycję **Dodaj produkty** , a następnie wybierz pozycję **Azure**. 

    a. Wybierz segment rynku klienta z listy **segmentów** .

    b. Wybierz **rezerwacje** z listy **Typ** produktu.

    c. Wybierz typ rezerwacji, którą chce klient z listy **typów rezerwacji** .

4. Rezerwacje platformy Azure muszą być skojarzone z aktywną subskrypcją platformy Azure. Wybierz subskrypcję klienta, do której chcesz dodać rezerwacje platformy Azure, z listy **subskrypcja klienta** . 

   >[!IMPORTANT]
   >Jeśli klient nie ma jeszcze aktywnej subskrypcji platformy Azure, wybierz pozycję **Azure** , aby dodać ją teraz. 

5. Użyj filtrów, aby znaleźć rezerwacje platformy Azure na maszynach wirtualnych spełniających wymagania klienta.  

6. Po znalezieniu rezerwacji, które chcesz kupić, wprowadź liczbę wystąpień zarezerwowanych, których klient będzie potrzebować **, a następnie** wybierz pozycję **Dodaj do koszyka**.  

7. Powtórz kroki 5 i 6, dopóki wszystkie elementy niezbędne do zamówienia nie zostaną dodane. Wybierz pozycję **Przegląd** , aby sprawdzić, czy zamówienie jest poprawne.  

8. Na stronie **Przejrzyj zamówienia** możesz: 

    - Sprawdź lub Zmień liczbę wystąpień zarezerwowanych.

    - Wybierz zakres rezerwacji. Zakres rezerwacji może obejmować jedną subskrypcję lub wiele subskrypcji (zakres udostępniony). W przypadku określania zakresu rezerwacji w ramach jednej subskrypcji rabat zostanie zastosowany tylko do tej subskrypcji. W przypadku wybrania opcji udostępnione rabat zostanie zastosowany do wszystkich subskrypcji w kontekście rozliczeń klienta. 

      >[!NOTE] 
      >Jeśli zdecydujesz się ograniczyć zakres rezerwacji do pojedynczej subskrypcji platformy Azure, może być konieczne zwiększenie limitu przydziału vCPU subskrypcji. Aby zwiększyć limit przydziału vCPU subskrypcji, należy utworzyć żądanie pomocy technicznej w Azure Portal. Postępuj zgodnie z instrukcjami [w tym temacie](/azure/azure-supportability/resource-manager-core-quotas-request) , aby utworzyć żądanie. 

      >[!NOTE]   
      >Jeśli klient jest objęty planem platformy Azure, **zakres**  zostanie ustawiony na wartość **udostępnione**. 

    - Jeśli jesteś partnerem dostawcy, wybierz odsprzedawcy, który ma zostać skojarzony z produktem.
    
    - Jeśli rezerwacja platformy Azure obsługuje opcję planu rozliczania, możesz wybrać częstotliwość rozliczeń jako miesięcznie z menu rozwijanego. 
    - Jeśli rezerwacja platformy Azure nie obsługuje opcji planu rozliczania, domyślna częstotliwość rozliczeń to jednorazowe rozliczanie. 

9. Wybierz pozycję **Kup** , aby kupić zamówienie. Szczegóły zamówienia, w tym numer zamówienia, są wyświetlane na stronie **Potwierdź** . Wybierz pozycję **gotowe** , aby przejść do strony **Historia zamówień** . 

10. Aby zarządzać rezerwacją klienta w Azure Portal, Znajdź klienta na stronie **klientów** , a następnie wybierz strzałkę w dół, aby rozwinąć wiersz klienta. Wybierz **Portal zarządzania Microsoft Azure** , aby otworzyć rekord klienta w Azure Portal.

## <a name="next-steps"></a>Następne kroki

|**Aby uzyskać informacje na temat**   |**Przeczytaj to**    |
|:-----------------------------|:-----------------|
|Omówienie rezerwacji platformy Azure w programie CSP  | [Sprzedaj Microsoft Azure wystąpienia zarezerwowane](azure-reservations.md) |
|Zarządzanie rezerwacjami platformy Azure w centrum partnerskim | [Zarządzanie rezerwacjami platformy Azure w centrum partnerskim](azure-reservations-manage.md)
|Określ prawidłowy rozmiar maszyny wirtualnej i Sprawdź użycie maszyny wirtualnej klienta   |[Rozmiar maszyny wirtualnej dla maksymalnego użycia zastrzeżenia platformy Azure](azure-usage.md)   |
|Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Centrum partnerskiego | [Zakup Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji dla deweloperów Centrum partnerskiego   |
|Przyznanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure  | [Przyznaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure](give-customers-permission.md)  |