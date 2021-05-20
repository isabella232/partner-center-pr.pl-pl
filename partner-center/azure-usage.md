---
title: Ustalanie rozmiarów maszyn wirtualnych Azure na potrzeby maksymalnego użycia rezerwacji
description: Dowiedz się, jak do rozmiaru maszyny wirtualnej (VM) do potrzeb obliczeniowych klientów, gdy kupujesz Microsoft Azure rezerwacje dla nich.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149455"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="b13f9-103">Ustalanie rozmiarów maszyn wirtualnych Microsoft Azure na potrzeby maksymalnego użycia rezerwacji</span><span class="sxs-lookup"><span data-stu-id="b13f9-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="b13f9-104">**Odpowiednie role:** Agent administracyjny | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="b13f9-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="b13f9-105">W tym artykule wyjaśniono, jak rozmiar maszyny wirtualnej (VM) do potrzeb obliczeniowych klientów podczas zakupu Microsoft Azure dla nich rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="b13f9-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="b13f9-106">Ten artykuł dotyczy tylko partnerów w programie Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="b13f9-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="b13f9-107">Klienci korzystający z innych typów subskrypcji (takich jak subskrypcje z płatnością zgodnie z użyciem, indywidualny, Umowa z Klientem Microsoft lub Enterprise Agreement) powinni zamiast tego przeczytać tę dokumentację rezerwacji platformy [Azure.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="b13f9-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="b13f9-108">Określanie rozmiaru maszyny wirtualnej dla rezerwacji platformy Azure klienta</span><span class="sxs-lookup"><span data-stu-id="b13f9-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="b13f9-109">Podczas Microsoft Azure rezerwacji w imieniu klientów należy wybrać maszynę wirtualną o rozmiarze spełniającym potrzeby obliczeniowe klienta.</span><span class="sxs-lookup"><span data-stu-id="b13f9-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="b13f9-110">Te informacje można znaleźć przy użyciu jednej z tych metod:</span><span class="sxs-lookup"><span data-stu-id="b13f9-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="b13f9-111">Interfejs API wykorzystania platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b13f9-111">Azure utilization API</span></span>
- <span data-ttu-id="b13f9-112">Witryna Azure Portal</span><span class="sxs-lookup"><span data-stu-id="b13f9-112">The Azure portal</span></span>
- <span data-ttu-id="b13f9-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b13f9-113">Azure PowerShell</span></span>
- <span data-ttu-id="b13f9-114">Interfejs API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="b13f9-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="b13f9-115">Instrukcje dotyczące korzystania z każdej z tych metod znajdują się poniżej.</span><span class="sxs-lookup"><span data-stu-id="b13f9-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="b13f9-116">Po zakupie rezerwacji rabat za rezerwację jest stosowany automatycznie do maszyn wirtualnych pasujących do atrybutów i ilości rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="b13f9-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="b13f9-117">Nie musisz przypisywać rezerwacji do maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="b13f9-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="b13f9-118">Rabaty na rezerwacje nie mają zastosowania do klasycznych ani promocyjnych maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="b13f9-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="b13f9-119">Aby poprawnie zidentyfikować typ i rozmiar maszyny wirtualnej do kupienia w imieniu klienta, należy użyć jednej z metod opisanych poniżej, ponieważ typ serii maszyn wirtualnych nie jest poprawnie wyświetlany w plikach uzgodnień Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b13f9-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="b13f9-120">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu interfejsu API wykorzystania platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b13f9-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="b13f9-121">Użyj wartości atrybutu ServiceType z additionalInfo w odpowiedzi interfejsu API, aby zidentyfikować rozmiar maszyny wirtualnej do kupienia.</span><span class="sxs-lookup"><span data-stu-id="b13f9-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="b13f9-122">Aby uzyskać więcej informacji, zobacz [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the Partner Center API (Uzyskiwanie rekordów wykorzystania platformy Azure przez klienta w [interfejsie API Partner Center ).](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="b13f9-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="b13f9-123">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="b13f9-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="b13f9-124">W Partner Center przejdź do **strony Customers (Klienci).**</span><span class="sxs-lookup"><span data-stu-id="b13f9-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="b13f9-125">Znajdź klienta, który chce kupić rezerwacje maszyn wirtualnych platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie.</span><span class="sxs-lookup"><span data-stu-id="b13f9-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="b13f9-126">Wybierz **Portal zarządzania Microsoft Azure,** aby otworzyć rekord klienta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b13f9-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="b13f9-127">Wybierz **pozycję Maszyny wirtualne** z menu portalu, a następnie wybierz maszynę wirtualną, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="b13f9-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="b13f9-128">Na stronie szczegółów maszyny wirtualnej znajdź informacje o rozmiarze i regionie, jak pokazano poniżej, i użyj tych informacji do zakupu rezerwacji w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b13f9-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informacje o rozmiarze i regionie na stronie szczegółów":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="b13f9-130">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b13f9-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="b13f9-131">Skorzystaj z informacji na poniższej ilustracji, aby uzyskać lokalizację i rozmiar maszyny wirtualnej, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="b13f9-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Lokalizacja i rozmiar maszyny wirtualnej":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="b13f9-133">Uzyskiwanie informacji o rozmiarze maszyny wirtualnej przy użyciu interfejsu API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="b13f9-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="b13f9-134">Korzystając z klienta ARMClient lub interfejsów API ARM, wywołaj klienta ARM dla maszyny wirtualnej, dla której chcesz kupić rezerwację.</span><span class="sxs-lookup"><span data-stu-id="b13f9-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="b13f9-135">/subscriptions/ <Subscription ID> /resourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="b13f9-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="b13f9-136">Wywołanie zwraca wartości **vmSize** i **location**, jak pokazano poniżej.</span><span class="sxs-lookup"><span data-stu-id="b13f9-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="Wartość vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="wartość lokalizacji":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="b13f9-139">Weryfikowanie rabatu za użycie maszyny wirtualnej platformy Azure i rezerwację</span><span class="sxs-lookup"><span data-stu-id="b13f9-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="b13f9-140">Po zakupie wystąpienia zarezerwowanego maszyny wirtualnej platformy Azure w imieniu klienta rabat za opłacenie z góry miejsca maszyny wirtualnej jest automatycznie stosowany do maszyn wirtualnych, które pasują do atrybutów i ilości rezerwacji klienta.</span><span class="sxs-lookup"><span data-stu-id="b13f9-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="b13f9-141">Możesz sprawdzić użycie rezerwacji klienta i sprawdzić, do których maszyn wirtualnych są stosowane rabaty za rezerwację, korzystając z jednej z następujących metod:</span><span class="sxs-lookup"><span data-stu-id="b13f9-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="b13f9-142">Witryna Azure Portal</span><span class="sxs-lookup"><span data-stu-id="b13f9-142">The Azure portal</span></span>
- <span data-ttu-id="b13f9-143">Interfejs API wykorzystania platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b13f9-143">Azure utilization API</span></span>

<span data-ttu-id="b13f9-144">Instrukcje dotyczące korzystania z każdej z tych metod znajdują się poniżej.</span><span class="sxs-lookup"><span data-stu-id="b13f9-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="b13f9-145">Tylko interfejs API wykorzystania platformy Azure pokazuje, do której maszyny wirtualnej jest stosowany rabat.</span><span class="sxs-lookup"><span data-stu-id="b13f9-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="b13f9-146">Sprawdź użycie rezerwacji klienta w Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="b13f9-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="b13f9-147">W Partner Center przejdź do strony **Customers** (Klienci).</span><span class="sxs-lookup"><span data-stu-id="b13f9-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="b13f9-148">Znajdź klienta, którego rabat na rezerwację i użycie chcesz zweryfikować, a następnie wybierz strzałkę w dół, aby rozwinąć informacje o kliencie.</span><span class="sxs-lookup"><span data-stu-id="b13f9-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="b13f9-149">Wybierz **Portal zarządzania Microsoft Azure,** aby otworzyć rekord klienta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b13f9-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="b13f9-150">Wybierz **pozycję Rezerwacje** z menu portalu, a następnie wybierz rezerwację, dla której chcesz sprawdzić użycie.</span><span class="sxs-lookup"><span data-stu-id="b13f9-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="b13f9-151">Na stronie **Przegląd** sprawdź wykres wykorzystania rezerwacji, który pokazuje, jaka część rezerwacji została zastosowana do maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="b13f9-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b13f9-152">Dane użycia mogą być opóźnione o maksymalnie 8 godzin.</span><span class="sxs-lookup"><span data-stu-id="b13f9-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="b13f9-153">a.</span><span class="sxs-lookup"><span data-stu-id="b13f9-153">a.</span></span> <span data-ttu-id="b13f9-154">Jeśli wykorzystanie rezerwacji wynosi 100%, klient może uzyskać wszystkie możliwe oszczędności, które może zapewnić zakup rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="b13f9-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="b13f9-155">b.</span><span class="sxs-lookup"><span data-stu-id="b13f9-155">b.</span></span> <span data-ttu-id="b13f9-156">Jeśli użycie rezerwacji wynosi 0%, rabat nie jest stosowany do żadnej maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="b13f9-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="b13f9-157">c.</span><span class="sxs-lookup"><span data-stu-id="b13f9-157">c.</span></span> <span data-ttu-id="b13f9-158">Jeśli użycie rezerwacji wynosi od 1% do 99%, istnieją nieużywane korzyści.</span><span class="sxs-lookup"><span data-stu-id="b13f9-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="b13f9-159">Aby uniknąć tej sytuacji, przed dokonaniem zakupu określ maszynę wirtualną o prawidłowym rozmiarze, która będzie obsługiwać potrzeby obliczeniowe klienta.</span><span class="sxs-lookup"><span data-stu-id="b13f9-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="b13f9-160">Weryfikowanie użycia rezerwacji klienta za pomocą interfejsu API wykorzystania platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b13f9-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="b13f9-161">Tylko interfejs API wykorzystania platformy Azure pokazuje, do której maszyny wirtualnej jest stosowany rabat.</span><span class="sxs-lookup"><span data-stu-id="b13f9-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="b13f9-162">Dane użycia rezerwacji można uzyskać za pomocą interfejsu API wykorzystania platformy Azure, aby sprawdzić, czy klient otrzyma rabat na rezerwację i sprawdzić, do których maszyn wirtualnych jest stosowany rabat.</span><span class="sxs-lookup"><span data-stu-id="b13f9-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="b13f9-163">Porównaj przykład A z przykładem B, aby zobaczyć, jak zweryfikować użycie rezerwacji klienta.</span><span class="sxs-lookup"><span data-stu-id="b13f9-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Przykłady użycia rezerwacji":::

- <span data-ttu-id="b13f9-165">Identyfikator reservationId identyfikuje rezerwację platformy Azure, która została użyta do zastosowania rabatu do maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="b13f9-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="b13f9-166">consumptionMeter to identyfikator MeterId maszyny wirtualnej, do których zastosowano rabat na rezerwację.</span><span class="sxs-lookup"><span data-stu-id="b13f9-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="b13f9-167">Wartość ReservationMeter pokazuje koszt 0 USD od momentu zastosowania rabatu na rezerwację.</span><span class="sxs-lookup"><span data-stu-id="b13f9-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="b13f9-168">Aby uzyskać więcej informacji, zobacz [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the Partner Center API (Uzyskiwanie rekordów wykorzystania platformy Azure przez klienta w [interfejsie API Partner Center API).](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="b13f9-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="b13f9-169">Koszty oprogramowania, takie jak Microsoft Windows Server, nie są obecnie uwzględniane w cenie rezerwacji maszyny wirtualnej i będą wyświetlane jako oddzielne pozycje w rekordzie zamówienia i na fakturze.</span><span class="sxs-lookup"><span data-stu-id="b13f9-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="b13f9-170">Jeśli jednak klient ma korzyść użycia hybrydowego platformy Azure, koszty oprogramowania nie zostaną zastosowane.</span><span class="sxs-lookup"><span data-stu-id="b13f9-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="b13f9-171">Aby uzyskać więcej informacji, zobacz [Koszty oprogramowania systemu Windows nieujmowane w wystąpieniach zarezerwowanych.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="b13f9-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="b13f9-172">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="b13f9-172">Next steps</span></span>

|<span data-ttu-id="b13f9-173">**Aby uzyskać informacje o**</span><span class="sxs-lookup"><span data-stu-id="b13f9-173">**For information about**</span></span>   |<span data-ttu-id="b13f9-174">**Przeczytaj to**</span><span class="sxs-lookup"><span data-stu-id="b13f9-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="b13f9-175">Rezerwacje platformy Azure w programie CSP — omówienie</span><span class="sxs-lookup"><span data-stu-id="b13f9-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="b13f9-176">Sprzedaż Microsoft Azure wystąpień zarezerwowanych maszyn wirtualnych</span><span class="sxs-lookup"><span data-stu-id="b13f9-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="b13f9-177">Kupowanie rezerwacji platformy Azure dla klientów w Partner Center</span><span class="sxs-lookup"><span data-stu-id="b13f9-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="b13f9-178">Kupowanie rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b13f9-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="b13f9-179">Zarządzanie rezerwacjami platformy Azure w Partner Center</span><span class="sxs-lookup"><span data-stu-id="b13f9-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="b13f9-180">Zarządzanie rezerwacjami platformy Azure w Partner Center</span><span class="sxs-lookup"><span data-stu-id="b13f9-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="b13f9-181">Kupowanie rezerwacji platformy Azure w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="b13f9-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="b13f9-182">Prepay for virtual machines with Azure Reserved VM Instances in the Azure Help [(Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help (Prepay for virtual machines with Azure Reserved VM Instances in the Azure Help</span><span class="sxs-lookup"><span data-stu-id="b13f9-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="b13f9-183">Zarządzanie rezerwacjami platformy Azure w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="b13f9-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="b13f9-184">[Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych w](/azure/billing/billing-manage-reserved-vm-instance) pomocy platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b13f9-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="b13f9-185">Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Partner Center API</span><span class="sxs-lookup"><span data-stu-id="b13f9-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="b13f9-186">[Informacje Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji Partner Center dewelopera</span><span class="sxs-lookup"><span data-stu-id="b13f9-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="b13f9-187">Udzielanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure w ramach zakupionej dla nich subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="b13f9-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="b13f9-188">Nadaj klientom uprawnienia do zakupu własnych rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b13f9-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |