---
title: Ustalanie rozmiarów maszyn wirtualnych Azure na potrzeby maksymalnego użycia rezerwacji
description: Dowiedz się, jak rozmiarować maszynę wirtualną do potrzeb obliczeniowych klientów podczas zakupu Microsoft Azure rezerwacji dla nich.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510197"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Ustalanie rozmiarów maszyn wirtualnych Microsoft Azure na potrzeby maksymalnego użycia rezerwacji

**Odpowiednie role:** Agent administracyjny | Agent sprzedaży

W tym artykule wyjaśniono, jak rozmiar maszyny wirtualnej (VM) do potrzeb obliczeniowych klientów podczas zakupu Microsoft Azure rezerwacji.
 
> [!NOTE]
> Ten artykuł dotyczy tylko partnerów w programie Dostawca rozwiązań w chmurze (CSP). Klienci korzystający z innych typów subskrypcji (takich jak subskrypcje z płatnością zgodnie z użyciem, indywidualne, Umowa z Klientem Microsoft lub Enterprise Agreement) powinni zamiast tego przeczytać tę dokumentację rezerwacji platformy [Azure.](/azure/cost-management-billing/reservations)

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Określanie rozmiaru maszyny wirtualnej dla rezerwacji platformy Azure klienta

Podczas Microsoft Azure rezerwacji w imieniu klientów należy wybrać maszynę wirtualną o rozmiarze, aby spełnić potrzeby obliczeniowe klienta. Te informacje można znaleźć przy użyciu jednej z tych metod:

- Interfejs API wykorzystania platformy Azure
- Witryna Azure Portal
- Azure PowerShell
- Interfejs API Azure Resource Manager (ARM)

Instrukcje dotyczące korzystania z każdej z tych metod znajdują się poniżej. Po zakupie rezerwacji rabat za rezerwację jest stosowany automatycznie do maszyn wirtualnych pasujących do atrybutów i ilości rezerwacji. Nie musisz przypisywać rezerwacji do maszyny wirtualnej.

>[!NOTE]
>Rabaty na rezerwacje nie mają zastosowania do klasycznych ani promocyjnych maszyn wirtualnych.

>[!IMPORTANT]
>Aby poprawnie zidentyfikować typ i rozmiar maszyny wirtualnej do kupienia w imieniu klienta, należy użyć jednej z metod opisanych poniżej, ponieważ typ serii maszyn wirtualnych nie jest poprawnie wyświetlany w plikach uzgodnień Partner Center maszyn wirtualnych.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu interfejsu API użycia platformy Azure

1. Użyj wartości atrybutu ServiceType z additionalInfo w odpowiedzi interfejsu API, aby zidentyfikować rozmiar maszyny wirtualnej do kupienia.

2. Aby uzyskać więcej informacji, zobacz [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the Partner Center API (Uzyskiwanie rekordów wykorzystania platformy Azure przez klienta w [interfejsie API Partner Center API).](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu Microsoft Azure portal

1. W Partner Center przejdź do strony **Customers** (Klienci).

2. Znajdź klienta, który chce kupić rezerwacje maszyn wirtualnych platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie. Wybierz **Microsoft Azure portal zarządzania,** aby otworzyć rekord klienta w Azure Portal.

3. Wybierz **pozycję Maszyny wirtualne** z menu portalu, a następnie wybierz maszynę wirtualną, dla której chcesz kupić rezerwację.

4. Na stronie szczegółów maszyny wirtualnej znajdź informacje o rozmiarze i regionie, jak pokazano poniżej, i użyj tych informacji do zakupu rezerwacji w Partner Center.  

   :::image type="content" source="images/usage1.png" alt-text="Informacje o rozmiarze i regionie na stronie szczegółów.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu Microsoft Azure PowerShell

Skorzystaj z informacji na poniższej ilustracji, aby uzyskać lokalizację i rozmiar maszyny wirtualnej, dla której chcesz kupić rezerwację. 

:::image type="content" source="images/usage2.png" alt-text="Lokalizacja i rozmiar maszyny wirtualnej.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu interfejsu API Azure Resource Manager (ARM)

1. Korzystając z klienta ARMClient lub interfejsów API ARM, wywołaj klienta ARM dla maszyny wirtualnej, dla której chcesz kupić rezerwację.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. Wywołanie zwraca wartości parametrów **vmSize** i **location**, jak pokazano poniżej.

    :::image type="content" source="images/usage3.png" alt-text="wartość vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="wartość lokalizacji.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Weryfikowanie użycia maszyny wirtualnej platformy Azure i rabatu na rezerwację

Po zakupie wystąpienia zarezerwowanego maszyny wirtualnej platformy Azure w imieniu klienta rabat za opłacenie miejsca maszyny wirtualnej jest automatycznie stosowany do maszyn wirtualnych, które pasują do atrybutów i ilości rezerwacji klienta.

Możesz sprawdzić użycie rezerwacji klienta i sprawdzić, do których maszyn wirtualnych są stosowane rabaty za rezerwację, korzystając z jednej z następujących metod:

- Witryna Azure Portal
- Interfejs API wykorzystania platformy Azure

Instrukcje dotyczące korzystania z każdej z tych metod znajdują się poniżej.

>[!NOTE]
>Tylko interfejs API wykorzystania platformy Azure pokazuje, do której maszyny wirtualnej jest stosowany rabat.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Weryfikowanie użycia rezerwacji klienta w portalu Microsoft Azure portal

1. W Partner Center przejdź do strony **Customers** (Klienci).

2. Znajdź klienta, którego rabat na rezerwację i użycie chcesz zweryfikować, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie. Wybierz **Microsoft Azure portal zarządzania,** aby otworzyć rekord klienta w Azure Portal.
3. Wybierz **pozycję Rezerwacje** z menu portalu, a następnie wybierz rezerwację, dla której chcesz sprawdzić użycie.
4. Na stronie **Przegląd** sprawdź wykres wykorzystania rezerwacji, który pokazuje, jaka część rezerwacji została zastosowana do maszyn wirtualnych.

    >[!NOTE]
    >Dane użycia mogą być opóźnione o maksymalnie 8 godzin.

    a. Jeśli wykorzystanie rezerwacji wynosi 100%, klient może uzyskać wszystkie możliwe oszczędności, które może zapewnić zakup rezerwacji.
    b. Jeśli użycie rezerwacji wynosi 0%, rabat nie jest stosowany do żadnej maszyny wirtualnej.
    c. Jeśli użycie rezerwacji wynosi od 1% do 99%, istnieją nieużywane korzyści.

5. Aby uniknąć tej sytuacji, przed dokonaniem zakupu określ maszynę wirtualną o prawidłowym rozmiarze, która będzie obsługiwać potrzeby obliczeniowe klienta.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Weryfikowanie użycia rezerwacji klienta za pomocą interfejsu API wykorzystania platformy Azure

>[!NOTE]
>Tylko interfejs API wykorzystania platformy Azure pokazuje, do której maszyny wirtualnej jest stosowany rabat.  

Dane użycia rezerwacji można uzyskać za pomocą interfejsu API wykorzystania platformy Azure, aby sprawdzić, czy klient otrzyma rabat na rezerwację i sprawdzić, do których maszyn wirtualnych jest stosowany rabat. Porównaj przykład A z przykładem B, aby zobaczyć, jak zweryfikować użycie rezerwacji klienta.

:::image type="content" source="images/usage5.png" alt-text="Przykłady użycia rezerwacji.":::

- Identyfikator reservationId identyfikuje rezerwację platformy Azure, która została użyta do zastosowania rabatu do maszyny wirtualnej.
- consumptionMeter to identyfikator MeterId maszyny wirtualnej, do których zastosowano rabat na rezerwację.
- Wartość ReservationMeter pokazuje koszt 0 USD od momentu zastosowania rabatu na rezerwację.

Aby uzyskać więcej informacji, zobacz [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the Partner Center API (Uzyskiwanie rekordów wykorzystania platformy Azure przez klienta w [interfejsie API Partner Center API).](/partner-center/develop/)

>[!IMPORTANT]
>Koszty oprogramowania, takie jak microsoft Windows Server, nie są obecnie uwzględniane w cenie rezerwacji maszyny wirtualnej i będą wyświetlane jako oddzielne pozycje w rekordzie zamówienia i na fakturze. Jeśli jednak klient ma korzyść użycia hybrydowego platformy Azure, koszty oprogramowania nie zostaną zastosowane. Aby uzyskać więcej informacji, [zobacz Windows oprogramowania nieujmowane w wystąpieniach zarezerwowanych.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Następne kroki

|**Aby uzyskać informacje o**   |**Przeczytaj to**    |
|:-----------------------------|:-----------------|
|Rezerwacje platformy Azure w programie CSP — omówienie  | [Sprzedaż Microsoft Azure wystąpień zarezerwowanych maszyn wirtualnych](azure-reservations.md)
|Kupowanie rezerwacji platformy Azure dla klientów w Partner Center   | [Kupowanie rezerwacji platformy Azure](azure-reservations-buying.md)
|Zarządzanie rezerwacjami platformy Azure w Partner Center | [Zarządzanie rezerwacjami platformy Azure w Partner Center](azure-reservations-manage.md)
|Kupowanie rezerwacji platformy Azure w Azure Portal | Prepay for virtual machines with Azure Reserved VM Instances in the Azure Help [(Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help (Prepay for virtual machines with Azure Reserved VM Instances in the Azure Help |
|Zarządzanie rezerwacjami platformy Azure w Azure Portal   | [Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych w](/azure/billing/billing-manage-reserved-vm-instance) pomocy platformy Azure  |
|Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Partner Center API | [Informacje Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji Partner Center dewelopera   |
|Udzielanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure w ramach zakupionej dla nich subskrypcji. | [Nadaj klientom uprawnienia do zakupu własnych rezerwacji platformy Azure](give-customers-permission.md)   |