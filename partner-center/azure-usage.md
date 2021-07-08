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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="1ea41-103">Ustalanie rozmiarów maszyn wirtualnych Microsoft Azure na potrzeby maksymalnego użycia rezerwacji</span><span class="sxs-lookup"><span data-stu-id="1ea41-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="1ea41-104">**Odpowiednie role:** Agent administracyjny | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="1ea41-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="1ea41-105">W tym artykule wyjaśniono, jak rozmiar maszyny wirtualnej (VM) do potrzeb obliczeniowych klientów podczas zakupu Microsoft Azure rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="1ea41-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="1ea41-106">Ten artykuł dotyczy tylko partnerów w programie Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="1ea41-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="1ea41-107">Klienci korzystający z innych typów subskrypcji (takich jak subskrypcje z płatnością zgodnie z użyciem, indywidualne, Umowa z Klientem Microsoft lub Enterprise Agreement) powinni zamiast tego przeczytać tę dokumentację rezerwacji platformy [Azure.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="1ea41-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="1ea41-108">Określanie rozmiaru maszyny wirtualnej dla rezerwacji platformy Azure klienta</span><span class="sxs-lookup"><span data-stu-id="1ea41-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="1ea41-109">Podczas Microsoft Azure rezerwacji w imieniu klientów należy wybrać maszynę wirtualną o rozmiarze, aby spełnić potrzeby obliczeniowe klienta.</span><span class="sxs-lookup"><span data-stu-id="1ea41-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="1ea41-110">Te informacje można znaleźć przy użyciu jednej z tych metod:</span><span class="sxs-lookup"><span data-stu-id="1ea41-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="1ea41-111">Interfejs API wykorzystania platformy Azure</span><span class="sxs-lookup"><span data-stu-id="1ea41-111">Azure utilization API</span></span>
- <span data-ttu-id="1ea41-112">Witryna Azure Portal</span><span class="sxs-lookup"><span data-stu-id="1ea41-112">The Azure portal</span></span>
- <span data-ttu-id="1ea41-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="1ea41-113">Azure PowerShell</span></span>
- <span data-ttu-id="1ea41-114">Interfejs API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="1ea41-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="1ea41-115">Instrukcje dotyczące korzystania z każdej z tych metod znajdują się poniżej.</span><span class="sxs-lookup"><span data-stu-id="1ea41-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="1ea41-116">Po zakupie rezerwacji rabat za rezerwację jest stosowany automatycznie do maszyn wirtualnych pasujących do atrybutów i ilości rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="1ea41-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="1ea41-117">Nie musisz przypisywać rezerwacji do maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="1ea41-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="1ea41-118">Rabaty na rezerwacje nie mają zastosowania do klasycznych ani promocyjnych maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="1ea41-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="1ea41-119">Aby poprawnie zidentyfikować typ i rozmiar maszyny wirtualnej do kupienia w imieniu klienta, należy użyć jednej z metod opisanych poniżej, ponieważ typ serii maszyn wirtualnych nie jest poprawnie wyświetlany w plikach uzgodnień Partner Center maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="1ea41-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="1ea41-120">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu interfejsu API użycia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="1ea41-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="1ea41-121">Użyj wartości atrybutu ServiceType z additionalInfo w odpowiedzi interfejsu API, aby zidentyfikować rozmiar maszyny wirtualnej do kupienia.</span><span class="sxs-lookup"><span data-stu-id="1ea41-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="1ea41-122">Aby uzyskać więcej informacji, zobacz [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the Partner Center API (Uzyskiwanie rekordów wykorzystania platformy Azure przez klienta w [interfejsie API Partner Center API).](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="1ea41-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="1ea41-123">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="1ea41-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="1ea41-124">W Partner Center przejdź do strony **Customers** (Klienci).</span><span class="sxs-lookup"><span data-stu-id="1ea41-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="1ea41-125">Znajdź klienta, który chce kupić rezerwacje maszyn wirtualnych platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie.</span><span class="sxs-lookup"><span data-stu-id="1ea41-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="1ea41-126">Wybierz **Microsoft Azure portal zarządzania,** aby otworzyć rekord klienta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1ea41-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="1ea41-127">Wybierz **pozycję Maszyny wirtualne** z menu portalu, a następnie wybierz maszynę wirtualną, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="1ea41-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="1ea41-128">Na stronie szczegółów maszyny wirtualnej znajdź informacje o rozmiarze i regionie, jak pokazano poniżej, i użyj tych informacji do zakupu rezerwacji w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1ea41-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informacje o rozmiarze i regionie na stronie szczegółów.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="1ea41-130">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="1ea41-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="1ea41-131">Skorzystaj z informacji na poniższej ilustracji, aby uzyskać lokalizację i rozmiar maszyny wirtualnej, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="1ea41-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Lokalizacja i rozmiar maszyny wirtualnej.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="1ea41-133">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu interfejsu API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="1ea41-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="1ea41-134">Korzystając z klienta ARMClient lub interfejsów API ARM, wywołaj klienta ARM dla maszyny wirtualnej, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="1ea41-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="1ea41-135">Wywołanie zwraca wartości parametrów **vmSize** i **location**, jak pokazano poniżej.</span><span class="sxs-lookup"><span data-stu-id="1ea41-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="wartość vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="wartość lokalizacji.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="1ea41-138">Weryfikowanie użycia maszyny wirtualnej platformy Azure i rabatu na rezerwację</span><span class="sxs-lookup"><span data-stu-id="1ea41-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="1ea41-139">Po zakupie wystąpienia zarezerwowanego maszyny wirtualnej platformy Azure w imieniu klienta rabat za opłacenie miejsca maszyny wirtualnej jest automatycznie stosowany do maszyn wirtualnych, które pasują do atrybutów i ilości rezerwacji klienta.</span><span class="sxs-lookup"><span data-stu-id="1ea41-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="1ea41-140">Możesz sprawdzić użycie rezerwacji klienta i sprawdzić, do których maszyn wirtualnych są stosowane rabaty za rezerwację, korzystając z jednej z następujących metod:</span><span class="sxs-lookup"><span data-stu-id="1ea41-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="1ea41-141">Witryna Azure Portal</span><span class="sxs-lookup"><span data-stu-id="1ea41-141">The Azure portal</span></span>
- <span data-ttu-id="1ea41-142">Interfejs API wykorzystania platformy Azure</span><span class="sxs-lookup"><span data-stu-id="1ea41-142">Azure utilization API</span></span>

<span data-ttu-id="1ea41-143">Instrukcje dotyczące korzystania z każdej z tych metod znajdują się poniżej.</span><span class="sxs-lookup"><span data-stu-id="1ea41-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="1ea41-144">Tylko interfejs API wykorzystania platformy Azure pokazuje, do której maszyny wirtualnej jest stosowany rabat.</span><span class="sxs-lookup"><span data-stu-id="1ea41-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="1ea41-145">Weryfikowanie użycia rezerwacji klienta w portalu Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="1ea41-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="1ea41-146">W Partner Center przejdź do strony **Customers** (Klienci).</span><span class="sxs-lookup"><span data-stu-id="1ea41-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="1ea41-147">Znajdź klienta, którego rabat na rezerwację i użycie chcesz zweryfikować, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie.</span><span class="sxs-lookup"><span data-stu-id="1ea41-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="1ea41-148">Wybierz **Microsoft Azure portal zarządzania,** aby otworzyć rekord klienta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1ea41-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="1ea41-149">Wybierz **pozycję Rezerwacje** z menu portalu, a następnie wybierz rezerwację, dla której chcesz sprawdzić użycie.</span><span class="sxs-lookup"><span data-stu-id="1ea41-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="1ea41-150">Na stronie **Przegląd** sprawdź wykres wykorzystania rezerwacji, który pokazuje, jaka część rezerwacji została zastosowana do maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="1ea41-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="1ea41-151">Dane użycia mogą być opóźnione o maksymalnie 8 godzin.</span><span class="sxs-lookup"><span data-stu-id="1ea41-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="1ea41-152">a.</span><span class="sxs-lookup"><span data-stu-id="1ea41-152">a.</span></span> <span data-ttu-id="1ea41-153">Jeśli wykorzystanie rezerwacji wynosi 100%, klient może uzyskać wszystkie możliwe oszczędności, które może zapewnić zakup rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="1ea41-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="1ea41-154">b.</span><span class="sxs-lookup"><span data-stu-id="1ea41-154">b.</span></span> <span data-ttu-id="1ea41-155">Jeśli użycie rezerwacji wynosi 0%, rabat nie jest stosowany do żadnej maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="1ea41-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="1ea41-156">c.</span><span class="sxs-lookup"><span data-stu-id="1ea41-156">c.</span></span> <span data-ttu-id="1ea41-157">Jeśli użycie rezerwacji wynosi od 1% do 99%, istnieją nieużywane korzyści.</span><span class="sxs-lookup"><span data-stu-id="1ea41-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="1ea41-158">Aby uniknąć tej sytuacji, przed dokonaniem zakupu określ maszynę wirtualną o prawidłowym rozmiarze, która będzie obsługiwać potrzeby obliczeniowe klienta.</span><span class="sxs-lookup"><span data-stu-id="1ea41-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="1ea41-159">Weryfikowanie użycia rezerwacji klienta za pomocą interfejsu API wykorzystania platformy Azure</span><span class="sxs-lookup"><span data-stu-id="1ea41-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="1ea41-160">Tylko interfejs API wykorzystania platformy Azure pokazuje, do której maszyny wirtualnej jest stosowany rabat.</span><span class="sxs-lookup"><span data-stu-id="1ea41-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="1ea41-161">Dane użycia rezerwacji można uzyskać za pomocą interfejsu API wykorzystania platformy Azure, aby sprawdzić, czy klient otrzyma rabat na rezerwację i sprawdzić, do których maszyn wirtualnych jest stosowany rabat.</span><span class="sxs-lookup"><span data-stu-id="1ea41-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="1ea41-162">Porównaj przykład A z przykładem B, aby zobaczyć, jak zweryfikować użycie rezerwacji klienta.</span><span class="sxs-lookup"><span data-stu-id="1ea41-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Przykłady użycia rezerwacji.":::

- <span data-ttu-id="1ea41-164">Identyfikator reservationId identyfikuje rezerwację platformy Azure, która została użyta do zastosowania rabatu do maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="1ea41-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="1ea41-165">consumptionMeter to identyfikator MeterId maszyny wirtualnej, do których zastosowano rabat na rezerwację.</span><span class="sxs-lookup"><span data-stu-id="1ea41-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="1ea41-166">Wartość ReservationMeter pokazuje koszt 0 USD od momentu zastosowania rabatu na rezerwację.</span><span class="sxs-lookup"><span data-stu-id="1ea41-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="1ea41-167">Aby uzyskać więcej informacji, zobacz [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the Partner Center API (Uzyskiwanie rekordów wykorzystania platformy Azure przez klienta w [interfejsie API Partner Center API).](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="1ea41-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="1ea41-168">Koszty oprogramowania, takie jak microsoft Windows Server, nie są obecnie uwzględniane w cenie rezerwacji maszyny wirtualnej i będą wyświetlane jako oddzielne pozycje w rekordzie zamówienia i na fakturze.</span><span class="sxs-lookup"><span data-stu-id="1ea41-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="1ea41-169">Jeśli jednak klient ma korzyść użycia hybrydowego platformy Azure, koszty oprogramowania nie zostaną zastosowane.</span><span class="sxs-lookup"><span data-stu-id="1ea41-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="1ea41-170">Aby uzyskać więcej informacji, [zobacz Windows oprogramowania nieujmowane w wystąpieniach zarezerwowanych.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="1ea41-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="1ea41-171">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="1ea41-171">Next steps</span></span>

|<span data-ttu-id="1ea41-172">**Aby uzyskać informacje o**</span><span class="sxs-lookup"><span data-stu-id="1ea41-172">**For information about**</span></span>   |<span data-ttu-id="1ea41-173">**Przeczytaj to**</span><span class="sxs-lookup"><span data-stu-id="1ea41-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="1ea41-174">Rezerwacje platformy Azure w programie CSP — omówienie</span><span class="sxs-lookup"><span data-stu-id="1ea41-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="1ea41-175">Sprzedaż Microsoft Azure wystąpień zarezerwowanych maszyn wirtualnych</span><span class="sxs-lookup"><span data-stu-id="1ea41-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="1ea41-176">Kupowanie rezerwacji platformy Azure dla klientów w Partner Center</span><span class="sxs-lookup"><span data-stu-id="1ea41-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="1ea41-177">Kupowanie rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="1ea41-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="1ea41-178">Zarządzanie rezerwacjami platformy Azure w Partner Center</span><span class="sxs-lookup"><span data-stu-id="1ea41-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="1ea41-179">Zarządzanie rezerwacjami platformy Azure w Partner Center</span><span class="sxs-lookup"><span data-stu-id="1ea41-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="1ea41-180">Kupowanie rezerwacji platformy Azure w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="1ea41-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="1ea41-181">Prepay for virtual machines with Azure Reserved VM Instances in the Azure Help [(Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help (Prepay for virtual machines with Azure Reserved VM Instances in the Azure Help</span><span class="sxs-lookup"><span data-stu-id="1ea41-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="1ea41-182">Zarządzanie rezerwacjami platformy Azure w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="1ea41-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="1ea41-183">[Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych w](/azure/billing/billing-manage-reserved-vm-instance) pomocy platformy Azure</span><span class="sxs-lookup"><span data-stu-id="1ea41-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="1ea41-184">Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Partner Center API</span><span class="sxs-lookup"><span data-stu-id="1ea41-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="1ea41-185">[Informacje Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji Partner Center dewelopera</span><span class="sxs-lookup"><span data-stu-id="1ea41-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="1ea41-186">Udzielanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure w ramach zakupionej dla nich subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="1ea41-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="1ea41-187">Nadaj klientom uprawnienia do zakupu własnych rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="1ea41-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |