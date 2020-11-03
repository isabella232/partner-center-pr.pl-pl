---
title: Ustalanie rozmiarów maszyn wirtualnych Azure na potrzeby maksymalnego użycia rezerwacji
description: Dowiedz się, jak zmienić rozmiar maszyny wirtualnej (VM) na potrzeby obliczeniowe klientów w przypadku zakupu Microsoft Azurech dla nich rezerwacji.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529902"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Ustalanie rozmiarów maszyn wirtualnych Microsoft Azure na potrzeby maksymalnego użycia rezerwacji

**Dotyczy**

- Centrum partnerskie
- Azure Portal
- Partnerzy w programie CSP
 
> [!NOTE]
> Ten artykuł ma zastosowanie tylko do partnerów w programie Cloud Solution Provider (CSP). Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Określanie rozmiaru maszyny wirtualnej dla rezerwacji platformy Azure dla klienta

Podczas kupowania Microsoft Azurech rezerwacji w imieniu klientów należy wybrać rozmiar maszyny wirtualnej (VM), aby spełnić potrzeby obliczeniowe klienta. Te informacje można znaleźć za pomocą jednej z następujących metod:

- Interfejs API użycia platformy Azure
- Witryna Azure Portal
- Azure PowerShell
- Interfejs API Azure Resource Manager (ARM)

Poniżej przedstawiono instrukcje dotyczące korzystania z każdej z tych metod. Po zakupieniu rezerwacji rabat rezerwacji jest automatycznie stosowany do maszyn wirtualnych, które pasują do atrybutów i ilości rezerwacji. Nie musisz przypisywać rezerwacji do maszyny wirtualnej.

>[!NOTE]
>Rabaty rezerwacji nie mają zastosowania do klasycznych ani promocyjnych maszyn wirtualnych.

>[!IMPORTANT]
>Aby poprawnie określić typ i rozmiar maszyny wirtualnej do zakupu w imieniu klienta, należy użyć jednej z metod opisanych poniżej, ponieważ typ serii maszyn wirtualnych nie jest prawidłowo wyświetlany w plikach uzgadniania Centrum partnerskiego.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Uzyskiwanie informacji o rozmiarach maszyn wirtualnych za pomocą interfejsu API użycia platformy Azure

1. Użyj atrybutu Value dla ServiceType z additionalInfo w odpowiedzi interfejsu API w celu zidentyfikowania rozmiaru maszyny wirtualnej do zakupu.

2. Aby uzyskać więcej informacji, zobacz artykuł [pobieranie rekordów użycia klienta na platformie Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) w [interfejsie API Centrum partnerskiego](/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Uzyskiwanie informacji o rozmiarach maszyn wirtualnych przy użyciu Microsoft Azure Portal

1. W centrum partnerskim przejdź do strony **klientów** .

2. Znajdź klienta, który chce kupić rezerwacje maszyn wirtualnych platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie. Wybierz **Portal zarządzania Microsoft Azure** , aby otworzyć rekord klienta w Azure Portal.

3. Wybierz pozycję **maszyny wirtualne** z menu Portal, a następnie wybierz maszynę wirtualną, dla której chcesz kupić rezerwację.

4. Na stronie Szczegóły maszyny wirtualnej Znajdź informacje o rozmiarze i regionie, jak pokazano poniżej, i Skorzystaj z tych informacji, aby kupić rezerwację w centrum partnerskim.  

   :::image type="content" source="images/usage1.png" alt-text="Informacje o rozmiarze i regionie na stronie szczegółów":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Uzyskaj informacje o zmianie rozmiarów maszyny wirtualnej za pomocą Microsoft Azure PowerShell

Użyj informacji z poniższej ilustracji, aby pobrać lokalizację i rozmiar maszyny wirtualnej, dla której chcesz kupić rezerwację. 

:::image type="content" source="images/usage2.png" alt-text="Lokalizacja i rozmiar maszyny wirtualnej":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Uzyskiwanie informacji o wymiarze maszyny wirtualnej za pomocą interfejsu API Azure Resource Manager (ARM)

1. Korzystając z ARMClient lub interfejsów API ARM, wywołaj klienta ARM dla maszyny wirtualnej, dla której chcesz kupić rezerwację.

2. /subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.COMPUTE/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01

3. Wywołanie zwraca wartości dla **vmSize** i **lokalizacji** , jak pokazano poniżej.

    :::image type="content" source="images/usage3.png" alt-text="vmSize wartość":::
    :::image type="content" source="images/usage4.png" alt-text="wartość lokalizacji":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Weryfikowanie użycia maszyn wirtualnych platformy Azure i rabatu rezerwacji

Po zakupie wystąpienia zarezerwowanych maszyn wirtualnych platformy Azure w imieniu klienta rabat na płatność za miejsce maszyny wirtualnej jest automatycznie stosowany do maszyn wirtualnych, które pasują do atrybutów i liczby rezerwacji klienta.

Można sprawdzić użycie rezerwacji przez klienta i sprawdzić, do których maszyn wirtualnych są stosowane rabaty rezerwacji, korzystając z jednej z następujących metod:

- Witryna Azure Portal
- Interfejs API użycia platformy Azure

Poniżej przedstawiono instrukcje dotyczące korzystania z każdej z tych metod.

>[!NOTE]
>Tylko interfejs API użycia platformy Azure wskazuje maszynę wirtualną, do której jest naliczany rabat.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Sprawdź użycie rezerwacji klienta w Microsoft Azure Portal

1. W centrum partnerskim przejdź do strony **klientów** .

2. Znajdź klienta, którego rabat rezerwacji i użycie chcesz zweryfikować, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie. Wybierz **Portal zarządzania Microsoft Azure** , aby otworzyć rekord klienta w Azure Portal.
3. Wybierz pozycję **rezerwacje** z menu portalu, a następnie wybierz rezerwację, dla której chcesz sprawdzić użycie.
4. Na stronie **Przegląd** sprawdź wykres użycia zastrzeżenia, który pokazuje, jak część rezerwacji została zastosowana do maszyn wirtualnych.

    >[!NOTE]
    >Dane użycia mogą być opóźnione o maksymalnie 8 godzin.

    a. Jeśli użycie rezerwacji wynosi 100%, klient uzyskuje wszystkie możliwe oszczędności, jakie może zapewnić zakup rezerwacji.
    b. Jeśli użycie rezerwacji wynosi 0%, Rabat nie zostanie zastosowany do żadnej maszyny wirtualnej.
    c. Jeśli użycie rezerwacji ma wartość z zakresu od 1% do 99%, istnieją nieużywane korzyści.

5. Aby uniknąć tej sytuacji, należy określić prawidłowy rozmiar maszyny wirtualnej, aby obsługiwać potrzeby obliczeniowe klienta przed dokonaniem zakupu.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Weryfikowanie użycia rezerwacji klienta przy użyciu interfejsu API użycia platformy Azure

>[!NOTE]
>Tylko interfejs API użycia platformy Azure wskazuje maszynę wirtualną, do której jest naliczany rabat.  

Dane użycia rezerwacji można uzyskać za pomocą interfejsu API użycia platformy Azure, aby sprawdzić, czy klient pobiera rabat rezerwacji i czy można sprawdzić, które maszyny wirtualne są stosowane do rabatu. Porównaj przykład A na przykład B, aby zobaczyć, jak zweryfikować użycie rezerwacji przez klienta.

:::image type="content" source="images/usage5.png" alt-text="Przykłady użycia zastrzeżenia":::

- ReservationId identyfikuje rezerwację platformy Azure, która została użyta do zastosowania rabatu do maszyny wirtualnej.
- consumptionMeter to MeterId dla maszyny wirtualnej, do której zastosowano rabat rezerwacji.
- ReservationMeter pokazuje $0 koszt od momentu zastosowania rabatu rezerwacji.

Aby uzyskać więcej informacji, zobacz artykuł [pobieranie rekordów użycia klienta na platformie Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) w [interfejsie API Centrum partnerskiego](/partner-center/develop/).

>[!IMPORTANT]
>Koszty oprogramowania, takie jak Microsoft Windows Server, nie są obecnie uwzględniane w cenie rezerwacji maszyny wirtualnej i będą wyświetlane jako osobne elementy wiersza w rekordzie zamówienia i na fakturze. Jeśli jednak klient ma korzyść z używania hybrydowej platformy Azure, koszty oprogramowania nie zostaną zastosowane. Aby uzyskać więcej informacji, zobacz [koszty oprogramowania systemu Windows, które nie są dołączone do wystąpień zarezerwowanych](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Zasoby rezerwacji platformy Azure

|**Aby uzyskać informacje na temat**   |**Przeczytaj to**    |
|:-----------------------------|:-----------------|
|Omówienie rezerwacji platformy Azure w programie CSP  | [Sprzedaj Microsoft Azure zarezerwowane wystąpienia maszyn wirtualnych](azure-reservations.md)
|Kupowanie rezerwacji platformy Azure dla klientów w centrum partnerskim   | [Kupowanie rezerwacji platformy Azure](azure-reservations-buying.md)
|Zarządzanie rezerwacjami platformy Azure w centrum partnerskim | [Zarządzanie rezerwacjami platformy Azure w centrum partnerskim](azure-reservations-manage.md)
|Kupowanie rezerwacji platformy Azure w Azure Portal | [Przedpłata za maszyny wirtualne z Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) w pomocy systemu Azure |
|Zarządzanie rezerwacjami platformy Azure w Azure Portal   | [Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych](/azure/billing/billing-manage-reserved-vm-instance) w pomocy systemu Azure  |
|Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Centrum partnerskiego | [Zakup Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji dla deweloperów Centrum partnerskiego   |
|Przyznanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure z subskrypcji, która została zakupiona. | [Przyznaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure](give-customers-permission.md)   |