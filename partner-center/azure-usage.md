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
ms.openlocfilehash: 226ebd27b4ca4cdef56ce833a58a10bed89f8056
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534951"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="13737-103">Ustalanie rozmiarów maszyn wirtualnych Microsoft Azure na potrzeby maksymalnego użycia rezerwacji</span><span class="sxs-lookup"><span data-stu-id="13737-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="13737-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="13737-104">**Appropriate roles**</span></span>

- <span data-ttu-id="13737-105">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="13737-105">Admin agent</span></span>
- <span data-ttu-id="13737-106">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="13737-106">Sales agent</span></span>

<span data-ttu-id="13737-107">W tym artykule wyjaśniono, jak zmienić rozmiar maszyny wirtualnej (VM) na potrzeby obliczeniowe klientów w przypadku zakupu Microsoft Azure dla nich rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="13737-107">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="13737-108">Ten artykuł ma zastosowanie tylko do partnerów w programie Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="13737-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="13737-109">Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="13737-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="13737-110">Określanie rozmiaru maszyny wirtualnej dla rezerwacji platformy Azure dla klienta</span><span class="sxs-lookup"><span data-stu-id="13737-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="13737-111">Podczas kupowania Microsoft Azurech rezerwacji w imieniu klientów należy wybrać rozmiar maszyny wirtualnej (VM), aby spełnić potrzeby obliczeniowe klienta.</span><span class="sxs-lookup"><span data-stu-id="13737-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="13737-112">Te informacje można znaleźć za pomocą jednej z następujących metod:</span><span class="sxs-lookup"><span data-stu-id="13737-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="13737-113">Interfejs API użycia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="13737-113">Azure utilization API</span></span>
- <span data-ttu-id="13737-114">Witryna Azure Portal</span><span class="sxs-lookup"><span data-stu-id="13737-114">The Azure portal</span></span>
- <span data-ttu-id="13737-115">Program Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="13737-115">Azure PowerShell</span></span>
- <span data-ttu-id="13737-116">Interfejs API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="13737-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="13737-117">Poniżej przedstawiono instrukcje dotyczące korzystania z każdej z tych metod.</span><span class="sxs-lookup"><span data-stu-id="13737-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="13737-118">Po zakupieniu rezerwacji rabat rezerwacji jest automatycznie stosowany do maszyn wirtualnych, które pasują do atrybutów i ilości rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="13737-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="13737-119">Nie musisz przypisywać rezerwacji do maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="13737-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="13737-120">Rabaty rezerwacji nie mają zastosowania do klasycznych ani promocyjnych maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="13737-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="13737-121">Aby poprawnie określić typ i rozmiar maszyny wirtualnej do zakupu w imieniu klienta, należy użyć jednej z metod opisanych poniżej, ponieważ typ serii maszyn wirtualnych nie jest prawidłowo wyświetlany w plikach uzgadniania Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="13737-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="13737-122">Uzyskiwanie informacji o rozmiarach maszyn wirtualnych za pomocą interfejsu API użycia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="13737-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="13737-123">Użyj atrybutu Value dla ServiceType z additionalInfo w odpowiedzi interfejsu API w celu zidentyfikowania rozmiaru maszyny wirtualnej do zakupu.</span><span class="sxs-lookup"><span data-stu-id="13737-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="13737-124">Aby uzyskać więcej informacji, zobacz artykuł [pobieranie rekordów użycia klienta na platformie Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) w [interfejsie API Centrum partnerskiego](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="13737-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="13737-125">Uzyskiwanie informacji o rozmiarach maszyn wirtualnych przy użyciu Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="13737-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="13737-126">W centrum partnerskim przejdź do strony **klientów** .</span><span class="sxs-lookup"><span data-stu-id="13737-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="13737-127">Znajdź klienta, który chce kupić rezerwacje maszyn wirtualnych platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie.</span><span class="sxs-lookup"><span data-stu-id="13737-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="13737-128">Wybierz **Portal zarządzania Microsoft Azure** , aby otworzyć rekord klienta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="13737-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="13737-129">Wybierz pozycję **maszyny wirtualne** z menu Portal, a następnie wybierz maszynę wirtualną, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="13737-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="13737-130">Na stronie Szczegóły maszyny wirtualnej Znajdź informacje o rozmiarze i regionie, jak pokazano poniżej, i Skorzystaj z tych informacji, aby kupić rezerwację w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="13737-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informacje o rozmiarze i regionie na stronie szczegółów":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="13737-132">Uzyskaj informacje o zmianie rozmiarów maszyny wirtualnej za pomocą Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="13737-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="13737-133">Użyj informacji z poniższej ilustracji, aby pobrać lokalizację i rozmiar maszyny wirtualnej, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="13737-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Lokalizacja i rozmiar maszyny wirtualnej":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="13737-135">Uzyskiwanie informacji o wymiarze maszyny wirtualnej za pomocą interfejsu API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="13737-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="13737-136">Korzystając z ARMClient lub interfejsów API ARM, wywołaj klienta ARM dla maszyny wirtualnej, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="13737-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="13737-137">/subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.COMPUTE/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="13737-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="13737-138">Wywołanie zwraca wartości dla **vmSize** i **lokalizacji**, jak pokazano poniżej.</span><span class="sxs-lookup"><span data-stu-id="13737-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize wartość":::
    :::image type="content" source="images/usage4.png" alt-text="wartość lokalizacji":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="13737-141">Weryfikowanie użycia maszyn wirtualnych platformy Azure i rabatu rezerwacji</span><span class="sxs-lookup"><span data-stu-id="13737-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="13737-142">Po zakupie wystąpienia zarezerwowanych maszyn wirtualnych platformy Azure w imieniu klienta rabat na płatność za miejsce maszyny wirtualnej jest automatycznie stosowany do maszyn wirtualnych, które pasują do atrybutów i liczby rezerwacji klienta.</span><span class="sxs-lookup"><span data-stu-id="13737-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="13737-143">Można sprawdzić użycie rezerwacji przez klienta i sprawdzić, do których maszyn wirtualnych są stosowane rabaty rezerwacji, korzystając z jednej z następujących metod:</span><span class="sxs-lookup"><span data-stu-id="13737-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="13737-144">Witryna Azure Portal</span><span class="sxs-lookup"><span data-stu-id="13737-144">The Azure portal</span></span>
- <span data-ttu-id="13737-145">Interfejs API użycia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="13737-145">Azure utilization API</span></span>

<span data-ttu-id="13737-146">Poniżej przedstawiono instrukcje dotyczące korzystania z każdej z tych metod.</span><span class="sxs-lookup"><span data-stu-id="13737-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="13737-147">Tylko interfejs API użycia platformy Azure wskazuje maszynę wirtualną, do której jest naliczany rabat.</span><span class="sxs-lookup"><span data-stu-id="13737-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="13737-148">Sprawdź użycie rezerwacji klienta w Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="13737-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="13737-149">W centrum partnerskim przejdź do strony **klientów** .</span><span class="sxs-lookup"><span data-stu-id="13737-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="13737-150">Znajdź klienta, którego rabat rezerwacji i użycie chcesz zweryfikować, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie.</span><span class="sxs-lookup"><span data-stu-id="13737-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="13737-151">Wybierz **Portal zarządzania Microsoft Azure** , aby otworzyć rekord klienta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="13737-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="13737-152">Wybierz pozycję **rezerwacje** z menu portalu, a następnie wybierz rezerwację, dla której chcesz sprawdzić użycie.</span><span class="sxs-lookup"><span data-stu-id="13737-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="13737-153">Na stronie **Przegląd** sprawdź wykres użycia zastrzeżenia, który pokazuje, jak część rezerwacji została zastosowana do maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="13737-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="13737-154">Dane użycia mogą być opóźnione o maksymalnie 8 godzin.</span><span class="sxs-lookup"><span data-stu-id="13737-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="13737-155">a.</span><span class="sxs-lookup"><span data-stu-id="13737-155">a.</span></span> <span data-ttu-id="13737-156">Jeśli użycie rezerwacji wynosi 100%, klient uzyskuje wszystkie możliwe oszczędności, jakie może zapewnić zakup rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="13737-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="13737-157">b.</span><span class="sxs-lookup"><span data-stu-id="13737-157">b.</span></span> <span data-ttu-id="13737-158">Jeśli użycie rezerwacji wynosi 0%, Rabat nie zostanie zastosowany do żadnej maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="13737-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="13737-159">c.</span><span class="sxs-lookup"><span data-stu-id="13737-159">c.</span></span> <span data-ttu-id="13737-160">Jeśli użycie rezerwacji ma wartość z zakresu od 1% do 99%, istnieją nieużywane korzyści.</span><span class="sxs-lookup"><span data-stu-id="13737-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="13737-161">Aby uniknąć tej sytuacji, należy określić prawidłowy rozmiar maszyny wirtualnej, aby obsługiwać potrzeby obliczeniowe klienta przed dokonaniem zakupu.</span><span class="sxs-lookup"><span data-stu-id="13737-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="13737-162">Weryfikowanie użycia rezerwacji klienta przy użyciu interfejsu API użycia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="13737-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="13737-163">Tylko interfejs API użycia platformy Azure wskazuje maszynę wirtualną, do której jest naliczany rabat.</span><span class="sxs-lookup"><span data-stu-id="13737-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="13737-164">Dane użycia rezerwacji można uzyskać za pomocą interfejsu API użycia platformy Azure, aby sprawdzić, czy klient pobiera rabat rezerwacji i czy można sprawdzić, które maszyny wirtualne są stosowane do rabatu.</span><span class="sxs-lookup"><span data-stu-id="13737-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="13737-165">Porównaj przykład A na przykład B, aby zobaczyć, jak zweryfikować użycie rezerwacji przez klienta.</span><span class="sxs-lookup"><span data-stu-id="13737-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Przykłady użycia zastrzeżenia":::

- <span data-ttu-id="13737-167">ReservationId identyfikuje rezerwację platformy Azure, która została użyta do zastosowania rabatu do maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="13737-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="13737-168">consumptionMeter to MeterId dla maszyny wirtualnej, do której zastosowano rabat rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="13737-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="13737-169">ReservationMeter pokazuje $0 koszt od momentu zastosowania rabatu rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="13737-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="13737-170">Aby uzyskać więcej informacji, zobacz artykuł [pobieranie rekordów użycia klienta na platformie Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) w [interfejsie API Centrum partnerskiego](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="13737-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="13737-171">Koszty oprogramowania, takie jak Microsoft Windows Server, nie są obecnie uwzględniane w cenie rezerwacji maszyny wirtualnej i będą wyświetlane jako osobne elementy wiersza w rekordzie zamówienia i na fakturze.</span><span class="sxs-lookup"><span data-stu-id="13737-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="13737-172">Jeśli jednak klient ma korzyść z używania hybrydowej platformy Azure, koszty oprogramowania nie zostaną zastosowane.</span><span class="sxs-lookup"><span data-stu-id="13737-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="13737-173">Aby uzyskać więcej informacji, zobacz [koszty oprogramowania systemu Windows, które nie są dołączone do wystąpień zarezerwowanych](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="13737-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="13737-174">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="13737-174">Next steps</span></span>

|<span data-ttu-id="13737-175">**Aby uzyskać informacje na temat**</span><span class="sxs-lookup"><span data-stu-id="13737-175">**For information about**</span></span>   |<span data-ttu-id="13737-176">**Przeczytaj to**</span><span class="sxs-lookup"><span data-stu-id="13737-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="13737-177">Omówienie rezerwacji platformy Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="13737-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="13737-178">Sprzedaj Microsoft Azure zarezerwowane wystąpienia maszyn wirtualnych</span><span class="sxs-lookup"><span data-stu-id="13737-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="13737-179">Kupowanie rezerwacji platformy Azure dla klientów w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="13737-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="13737-180">Kupowanie rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="13737-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="13737-181">Zarządzanie rezerwacjami platformy Azure w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="13737-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="13737-182">Zarządzanie rezerwacjami platformy Azure w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="13737-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="13737-183">Kupowanie rezerwacji platformy Azure w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="13737-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="13737-184">[Przedpłata za maszyny wirtualne z Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) w pomocy systemu Azure</span><span class="sxs-lookup"><span data-stu-id="13737-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="13737-185">Zarządzanie rezerwacjami platformy Azure w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="13737-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="13737-186">[Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych](/azure/billing/billing-manage-reserved-vm-instance) w pomocy systemu Azure</span><span class="sxs-lookup"><span data-stu-id="13737-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="13737-187">Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="13737-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="13737-188">[Zakup Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji dla deweloperów Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="13737-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="13737-189">Przyznanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure z subskrypcji, która została zakupiona.</span><span class="sxs-lookup"><span data-stu-id="13737-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="13737-190">Przyznaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="13737-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |