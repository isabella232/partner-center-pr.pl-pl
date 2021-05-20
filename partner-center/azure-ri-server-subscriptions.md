---
title: Rezerwacje platformy Azure & subskrypcji serwera
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się Dostawca rozwiązań w chmurze możliwości pozyskiwania i aprowizowania rezerwacji platformy Azure oraz subskrypcji serwera dla klientów oraz zarządzania nimi.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 79175fc7e67fdcdc3195b33859f3609c4caf942f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149421"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="9514a-103">Uzyskaj, aprowizuj i & wystąpieniami zarezerwowanymi maszyn wirtualnych platformy Azure i subskrypcjami serwerów dla klientów</span><span class="sxs-lookup"><span data-stu-id="9514a-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="9514a-104">**Odpowiednie role:** Administrator | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży | Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="9514a-104">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="9514a-105">Co to jest Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="9514a-105">What are Azure Reservations?</span></span>

<span data-ttu-id="9514a-106">Rezerwacje platformy Azure pomagają zaoszczędzić pieniądze, płacąc z przedpłaty za maszynę wirtualną przez rok lub trzy lata, SQL Database obliczeniową, przepływność Azure Cosmos DB lub inne zasoby platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="9514a-106">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="9514a-107">Przedpłaty umożliwiają uzyskiwanie rabatu na zasoby, których używasz.</span><span class="sxs-lookup"><span data-stu-id="9514a-107">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="9514a-108">Rezerwacje mogą znacznie obniżyć koszty zasobów maszyn wirtualnych, zasobów obliczeniowych usługi SQL Database, zasobów Azure Cosmos DB i innych— nawet o 72% w porównaniu z cenami z płatnością zgodnie z potrzebami.</span><span class="sxs-lookup"><span data-stu-id="9514a-108">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="9514a-109">Rezerwacje umożliwiają skorzystanie z rabatu na rozliczenia i nie mają wpływu na stan środowiska uruchomieniowego Twoich zasobów.</span><span class="sxs-lookup"><span data-stu-id="9514a-109">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="9514a-110">Aby uzyskać więcej informacji, [zobacz Co to są rezerwacje platformy Azure?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="9514a-110">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="9514a-111">Dlaczego klienci powinni kupić rezerwację?</span><span class="sxs-lookup"><span data-stu-id="9514a-111">Why should customers buy a reservation?</span></span>

<span data-ttu-id="9514a-112">Jeśli klienci mają maszyny wirtualne, Azure Cosmos DB baz danych SQL, które działają przez długi czas, zakup rezerwacji jest najbardziej opłacalnym rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="9514a-112">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="9514a-113">Jeśli na przykład klient stale uruchamia cztery wystąpienia usługi bez rezerwacji, opłaty są naliczane zgodnie z płatnością zgodnie z użyciem.</span><span class="sxs-lookup"><span data-stu-id="9514a-113">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="9514a-114">Jeśli zakupią rezerwację dla tych zasobów, natychmiast uzyskają rabat na rezerwację.</span><span class="sxs-lookup"><span data-stu-id="9514a-114">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="9514a-115">Zasoby nie będą już obciążane opłatami według stawek płatności zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="9514a-115">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="9514a-116">Atrakcyjna nowa oferta platformy Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="9514a-116">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="9514a-117">Przenosząc rezerwacje platformy Azure i subskrypcje serwerów do programu CSP, firma Microsoft lepiej umożliwia swoim partnerom obsługę szybko rosnącego zapotrzebowania klientów na bardziej ekonomiczne rozwiązania do obsługi wysoce przewidywalnych, trwałych obciążeń w chmurze.</span><span class="sxs-lookup"><span data-stu-id="9514a-117">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="9514a-118">Program CSP umożliwia partnerom pozyskiwanie rezerwacji platformy Azure i subskrypcji serwera oraz zarządzanie nimi w imieniu klientów komercyjnych za pośrednictwem usług Microsoft Partner Center i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="9514a-118">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="9514a-119">Dajemy partnerom w naszym programie CSP możliwość wyboru sposobu zakupu rezerwacji platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="9514a-119">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="9514a-120">Partnerzy programu CSP mogą kupić rezerwacje platformy Azure [](give-customers-permission.md) w [imieniu](azure-reservations-buying.md) klienta lub mogą zezwolić klientowi na zakup własnych rezerwacji w ramach poprzedniej subskrypcji platformy Azure zakupionej przez partnera.</span><span class="sxs-lookup"><span data-stu-id="9514a-120">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="9514a-121">Rezerwacje platformy Azure zapewniają klientom elastyczność wirtualizacji dla szerokiego zakresu rozwiązań obliczeniowych, w tym tworzenia i testowania, uruchamiania aplikacji i rozszerzania centrum danych.</span><span class="sxs-lookup"><span data-stu-id="9514a-121">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="9514a-122">Na [](https://azure.microsoft.com/pricing/reserved-vm-instances/) Azure Reserved VM Instances klienci komercyjni mogą teraz zaoszczędzić do 72% w porównaniu z cenami maszyn wirtualnych platformy Azure z płatnością zgodnie z potrzebami, po prostu kupując lub "rezerwując" maszynę wirtualną na okres 1 roku lub 3 lat.</span><span class="sxs-lookup"><span data-stu-id="9514a-122">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="9514a-123">Klienci z systemem Windows Server Korzyść użycia hybrydowego platformy Azure z systemem pakiet Software Assurance będą mogli zaoszczędzić do 80% w porównaniu z płatnością zgodnie z cennikiem.</span><span class="sxs-lookup"><span data-stu-id="9514a-123">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="9514a-124">Dzięki niedopasowanej kombinacji atrakcyjnych cen i niedopasowanych elastyczności wdrażania klienci zobaczą najlepszą ogólną wartość po wybraniu rezerwacji platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="9514a-124">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="9514a-125">Zobacz [Kupowanie rezerwacji](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) w witrynie Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="9514a-125">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="9514a-126">Zobacz cennik komercyjnych wystąpień zarezerwowanych platformy **Azure RI** w [](https://partner.microsoft.com/dashboard/sell/pricingandoffers) kategorii wystąpienia zarezerwowane usługi **Microsoft Azure** na stronie Ceny i oferty w usłudze Partner Center dla subskrypcji oprogramowania i corocznych subskrypcji isv systemu Linux.</span><span class="sxs-lookup"><span data-stu-id="9514a-126">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="9514a-127">**Roczne subskrypcje dla isv isv systemu Linux**</span><span class="sxs-lookup"><span data-stu-id="9514a-127">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="9514a-128">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="9514a-128">SUSE Linux</span></span>
- <span data-ttu-id="9514a-129">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="9514a-129">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="9514a-130">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="9514a-130">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="9514a-131">**Roczne subskrypcje isv**</span><span class="sxs-lookup"><span data-stu-id="9514a-131">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="9514a-132">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="9514a-132">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="9514a-133">Wprowadzenie</span><span class="sxs-lookup"><span data-stu-id="9514a-133">Getting started</span></span>

<span data-ttu-id="9514a-134">Aby dowiedzieć się, jak można pozycjonować rezerwacje platformy Azure u klientów i jak najszybciej rozpocząć działanie operacyjne, zalecamy następujące podejście, aby przejrzeć materiały dotyczące gotowości:</span><span class="sxs-lookup"><span data-stu-id="9514a-134">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="9514a-135">Zapoznaj się z nowym [przewodnikiem Partner Center operacji handlowych i zapoznaj się z tym przewodnikiem.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)</span><span class="sxs-lookup"><span data-stu-id="9514a-135">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="9514a-136">Informacje o aktualizacjach rezerwacji platformy Azure i subskrypcji serwera w interfejsie [API Partner Center API (interfejs API/zestaw SDK).](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="9514a-136">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="9514a-137">Gotowość do sprzedaży</span><span class="sxs-lookup"><span data-stu-id="9514a-137">Sales readiness</span></span>

- [<span data-ttu-id="9514a-138">Usługi pulpitu zdalnego (RDS) Client Access License (CAL) (anons)</span><span class="sxs-lookup"><span data-stu-id="9514a-138">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="9514a-139">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="9514a-139">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="9514a-140">Subskrypcje serwera</span><span class="sxs-lookup"><span data-stu-id="9514a-140">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="9514a-141">Rezerwacje bazy danych SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="9514a-141">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="9514a-142">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="9514a-142">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="9514a-143">SQL Managed Instance (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="9514a-143">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="9514a-144">SUSE i Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="9514a-144">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="9514a-145">System Red Hat Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="9514a-145">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="9514a-146">System SUSE Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="9514a-146">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="9514a-147">System Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="9514a-147">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="9514a-148">Omówienie cennika platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9514a-148">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="9514a-149">Kalkulator cen platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9514a-149">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="9514a-150">Azure Databricks rezerwacje jednostek</span><span class="sxs-lookup"><span data-stu-id="9514a-150">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="9514a-151">Szkolenie</span><span class="sxs-lookup"><span data-stu-id="9514a-151">Training</span></span>

<span data-ttu-id="9514a-152">Zarejestruj się, aby [wyświetlić seminaria internetowe dotyczące gotowości na licencjonowanie komercyjne](https://commercial-licensing.eventbuilder.com/FY2019_ALL) i wydarzenia na żądanie.</span><span class="sxs-lookup"><span data-stu-id="9514a-152">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="9514a-153">Zarejestrowane wcześniej zdarzenia gotowości licencjonowania na żądanie obejmują następujące tematy:</span><span class="sxs-lookup"><span data-stu-id="9514a-153">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="9514a-154">CSP Online Services, CSP Azure i ogólne aktualizacje licencjonowania, w tym azure (listopad 2018)</span><span class="sxs-lookup"><span data-stu-id="9514a-154">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="9514a-155">Pojemność zarezerwowana usługi SQL DB & elastyczność rozmiaru wystąpienia (sierpień 2018 r.)</span><span class="sxs-lookup"><span data-stu-id="9514a-155">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="9514a-156">Subskrypcje serwera w programie CSP (lipiec 2018 r.)</span><span class="sxs-lookup"><span data-stu-id="9514a-156">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="9514a-157">Omówienie rezerwacji platformy Azure w programie CSP (maj 2018 r.)</span><span class="sxs-lookup"><span data-stu-id="9514a-157">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="9514a-158">Operacje</span><span class="sxs-lookup"><span data-stu-id="9514a-158">Operations</span></span>

<span data-ttu-id="9514a-159">[Partner Center](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)operacji handlowych: kompleksowy przewodnik obejmujący kluczowe zasady i aspekty operacyjne, takie jak umowy, zamawianie za pośrednictwem usługi Partner Center, faktura, szczegóły cennika, zachęty, plik uzgodnień, interfejs API/zestaw SDK, piaskownica i Azure Partner Shared Services.</span><span class="sxs-lookup"><span data-stu-id="9514a-159">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="9514a-160">Korzyść użycia hybrydowego platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9514a-160">Azure Hybrid Benefit</span></span>

<span data-ttu-id="9514a-161">Usługa [Korzyść użycia hybrydowego platformy Azure jest](https://azure.microsoft.com/pricing/hybrid-benefit) korzyścią cenową dla klientów, którzy mają licencje usługi pakiet Software Assurance, co pomaga zmaksymalizować wartość istniejących lokalnych inwestycji w system Windows Server i/lub SQL Server licencji podczas migracji na platformę Azure.</span><span class="sxs-lookup"><span data-stu-id="9514a-161">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="9514a-162">Uprawnieni klienci mogą zaoszczędzić do 40%\* na platformie Azure Virtual Machines (infrastruktura jako usługa lub IaaS) i zaoszczędzić do 55% na usługach Azure SQL Database (platforma jako usługa lub PaaS) i SQL Server na platformie Azure Virtual Machines (IaaS) z usługą Korzyść użycia hybrydowego platformy Azure, co w połączeniu z wystąpieniami zarezerwowanym platformy Azure zwiększa się do 80%.</span><span class="sxs-lookup"><span data-stu-id="9514a-162">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9514a-163">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="9514a-163">Next steps</span></span>

- [<span data-ttu-id="9514a-164">Często zadawane pytania dotyczące korzyści użycia hybrydowego platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9514a-164">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="9514a-165">\*Rzeczywiste oszczędności mogą się różnić w zależności od regionu, typu wystąpienia lub użycia.</span><span class="sxs-lookup"><span data-stu-id="9514a-165">\*Actual savings may vary based on region, instance type, or usage.</span></span>