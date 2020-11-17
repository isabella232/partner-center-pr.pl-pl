---
title: Rezerwacje platformy Azure & subskrypcje serwera
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o możliwościach dostawcy rozwiązań w chmurze, aby uzyskać, zainicjować i zarządzać rezerwacjami platformy Azure oraz subskrypcjami serwera dla klientów.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0434ad2e6494f5efc1b1e5e2aa003dc6587d7b4e
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691354"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="adbf6-103">Pozyskiwanie, Inicjowanie obsługi & Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych platformy Azure (RI) i subskrypcjami serwera dla klientów</span><span class="sxs-lookup"><span data-stu-id="adbf6-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="adbf6-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="adbf6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="adbf6-105">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="adbf6-105">Admin agent</span></span>
- <span data-ttu-id="adbf6-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="adbf6-106">Global admin</span></span>
- <span data-ttu-id="adbf6-107">Agent pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="adbf6-107">Helpdesk agent</span></span>
- <span data-ttu-id="adbf6-108">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="adbf6-108">Sales agent</span></span>
- <span data-ttu-id="adbf6-109">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="adbf6-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="adbf6-110">Co to jest Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="adbf6-110">What are Azure Reservations?</span></span>

<span data-ttu-id="adbf6-111">Azure Reservations pomóc zaoszczędzić pieniądze przez przedpłatę za rok lub trzy lata maszyny wirtualnej, SQL Database pojemność obliczeniowa, Azure Cosmos DB przepływność lub inne zasoby platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="adbf6-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="adbf6-112">Funkcja przedpłaty umożliwia uzyskanie rabatu za zasoby, których używasz.</span><span class="sxs-lookup"><span data-stu-id="adbf6-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="adbf6-113">Rezerwacje mogą znacząco obniżyć swoją maszynę wirtualną, obliczenia w usłudze SQL Database, Azure Cosmos DB i inne koszty zasobów do 72% w porównaniu z cenami z płatność zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="adbf6-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="adbf6-114">Rezerwacje umożliwiają skorzystanie z rabatu na rozliczenia i nie mają wpływu na stan środowiska uruchomieniowego Twoich zasobów.</span><span class="sxs-lookup"><span data-stu-id="adbf6-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="adbf6-115">Aby uzyskać więcej informacji, zobacz [co to są Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="adbf6-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="adbf6-116">Dlaczego klienci kupują rezerwację?</span><span class="sxs-lookup"><span data-stu-id="adbf6-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="adbf6-117">W przypadku klientów z maszynami wirtualnymi, Azure Cosmos DB lub baz danych SQL, które są uruchamiane przez długi czas, zakup rezerwacji daje im największą opłacalną opcję.</span><span class="sxs-lookup"><span data-stu-id="adbf6-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="adbf6-118">Na przykład jeśli klient ciągle uruchamia cztery wystąpienia usługi bez rezerwacji, opłaty są naliczone według stawek płatność zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="adbf6-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="adbf6-119">Jeśli kupią rezerwację dla tych zasobów, natychmiast uzyskają rabat rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="adbf6-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="adbf6-120">Zasoby nie będą już obciążane opłatami według stawek płatności zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="adbf6-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="adbf6-121">Atrakcyjna nowa oferta platformy Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="adbf6-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="adbf6-122">Dzięki dołączeniu Azure Reservations i subskrypcji serwera do swojego programu CSP firma Microsoft lepiej umożliwia swoim partnerom rozwiązywanie problemów z coraz większym popytem w celu uzyskania bardziej ekonomicznych rozwiązań do obsługi wysoce przewidywalnych, trwałych obciążeń w chmurze.</span><span class="sxs-lookup"><span data-stu-id="adbf6-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="adbf6-123">Program CSP umożliwia partnerom pozyskiwanie, Inicjowanie obsługi i zarządzanie subskrypcjami Azure Reservations i serwera w imieniu klientów komercyjnych za pośrednictwem Centrum partnerskiego firmy Microsoft i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="adbf6-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="adbf6-124">Oferujemy również partnerów w naszym programie CSP, w których można kupować rezerwacje platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="adbf6-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="adbf6-125">Partnerzy programu CSP mogą [kupować rezerwacje platformy Azure w imieniu klienta](azure-reservations-buying.md) lub mogą [zezwolić klientowi na kupowanie własnych rezerwacji](give-customers-permission.md) w ramach wcześniejszej subskrypcji platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="adbf6-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="adbf6-126">Azure Reservations zapewnić klientom elastyczność wirtualizacji dla szerokiego zakresu rozwiązań obliczeniowych, w tym tworzenia i testowania, uruchamiania aplikacji oraz rozszerzania centrum danych.</span><span class="sxs-lookup"><span data-stu-id="adbf6-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="adbf6-127">W [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) na przykład komercyjni klienci mogą teraz zaoszczędzić do 72%, a w przeciwieństwie do cen maszyn wirtualnych z systemem Azure — po prostu przy zakupie lub "obsłużeniu" — w przypadku okresu 1-lub 3-letniego.</span><span class="sxs-lookup"><span data-stu-id="adbf6-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="adbf6-128">Klienci korzystający z systemu Windows Server z Korzyść użycia hybrydowego platformy Azure, dostępną w ramach programu Software Assurance, będą mogli zaoszczędzić do 80% w porównaniu z cenami zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="adbf6-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="adbf6-129">W przypadku niedopasowanej kombinacji atrakcyjnych cen i niedopasowanej elastyczności wdrożenia klienci będą widzieli najlepszą ogólną wartość, wybierając Azure Reservations.</span><span class="sxs-lookup"><span data-stu-id="adbf6-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="adbf6-130">Zobacz [zakupy rezerwacji](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) w witrynie Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="adbf6-130">See [Purchase Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="adbf6-131">Zapoznaj się z **Microsoft Azure** **listą komercyjnych cen dostawcy usług kryptograficznych (CSP) na platformie Azure** na stronie [ceny i oferty](https://partner.microsoft.com/dashboard/sell/pricingandoffers) w centrum partnerskim dla subskrypcji oprogramowania i rocznych subskrypcji systemu Linux.</span><span class="sxs-lookup"><span data-stu-id="adbf6-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="adbf6-132">**Subskrypcje roczne niezależnego dostawcy oprogramowania Linux**</span><span class="sxs-lookup"><span data-stu-id="adbf6-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="adbf6-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="adbf6-133">SUSE Linux</span></span>
- <span data-ttu-id="adbf6-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="adbf6-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="adbf6-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="adbf6-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="adbf6-136">**Subskrypcje roczne niezależnego dostawcy oprogramowania**</span><span class="sxs-lookup"><span data-stu-id="adbf6-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="adbf6-137">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="adbf6-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="adbf6-138">Wprowadzenie</span><span class="sxs-lookup"><span data-stu-id="adbf6-138">Getting started</span></span>

<span data-ttu-id="adbf6-139">Aby zrozumieć, w jaki sposób można określić, Azure Reservations z klientami oraz jak najszybciej rozpocząć pracę, zalecamy następujące podejście do przeglądu materiałów gotowości:</span><span class="sxs-lookup"><span data-stu-id="adbf6-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="adbf6-140">Przejrzyj i zapoznaj się z [nowym przewodnikiem obsługi handlu w centrum partnerskim](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span><span class="sxs-lookup"><span data-stu-id="adbf6-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="adbf6-141">Informacje na temat aktualizacji Azure Reservations i subskrypcji serwera w [interfejsie API Centrum partnerskiego (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="adbf6-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="adbf6-142">Gotowość do sprzedaży</span><span class="sxs-lookup"><span data-stu-id="adbf6-142">Sales readiness</span></span>

- [<span data-ttu-id="adbf6-143">Licencja dostępu klienta (CAL) Usługi pulpitu zdalnego (RDS) (anons)</span><span class="sxs-lookup"><span data-stu-id="adbf6-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="adbf6-144">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="adbf6-144">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="adbf6-145">Subskrypcje serwera</span><span class="sxs-lookup"><span data-stu-id="adbf6-145">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)

- [<span data-ttu-id="adbf6-146">Rezerwacje bazy danych SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="adbf6-146">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="adbf6-147">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="adbf6-147">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="adbf6-148">Wystąpienie zarządzane SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="adbf6-148">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="adbf6-149">SUSE i Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="adbf6-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="adbf6-150">Red Hat Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="adbf6-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="adbf6-151">SUSE Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="adbf6-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="adbf6-152">System Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="adbf6-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="adbf6-153">Przegląd cen platformy Azure</span><span class="sxs-lookup"><span data-stu-id="adbf6-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="adbf6-154">Kalkulator cen platformy Azure</span><span class="sxs-lookup"><span data-stu-id="adbf6-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="adbf6-155">Azure Databricks rezerwacji jednostek</span><span class="sxs-lookup"><span data-stu-id="adbf6-155">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="adbf6-156">Szkolenia</span><span class="sxs-lookup"><span data-stu-id="adbf6-156">Training</span></span>

<span data-ttu-id="adbf6-157">Zarejestruj się, aby wyświetlić [seminaria internetowe gotowości do licencjonowania komercyjnego](https://commercial-licensing.eventbuilder.com/FY2019_ALL) oraz zdarzenia na żądanie.</span><span class="sxs-lookup"><span data-stu-id="adbf6-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="adbf6-158">Wcześniej zarejestrowane zdarzenia gotowości licencjonowania obejmują następujące tematy:</span><span class="sxs-lookup"><span data-stu-id="adbf6-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="adbf6-159">Usługi CSP online, dostawcy CSP Azure i ogólne aktualizacje licencjonowania, w tym Azure (listopad 2018)</span><span class="sxs-lookup"><span data-stu-id="adbf6-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="adbf6-160">Zarezerwowana pojemność bazy danych SQL & elastyczność rozmiaru wystąpienia (sierpień 2018)</span><span class="sxs-lookup"><span data-stu-id="adbf6-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="adbf6-161">Subskrypcje serwera w programie CSP (lipiec 2018)</span><span class="sxs-lookup"><span data-stu-id="adbf6-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="adbf6-162">Przegląd Azure Reservations w programie CSP (2018 maja)</span><span class="sxs-lookup"><span data-stu-id="adbf6-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="adbf6-163">Operacje</span><span class="sxs-lookup"><span data-stu-id="adbf6-163">Operations</span></span>

<span data-ttu-id="adbf6-164">[Centrum partnerskie — nowy Przewodnik operacji handlowych](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): kompleksowy przewodnik dotyczący najważniejszych zasad i aspektów operacyjnych, takich jak umowy, porządkowanie przez centrum partnerskie, faktury, szczegóły cennika, zachęty, plik uzgadniania, interfejs API/zestaw SDK, piaskownica i udostępnione usługi partnerskie platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="adbf6-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="adbf6-165">Korzyść użycia hybrydowego platformy Azure</span><span class="sxs-lookup"><span data-stu-id="adbf6-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="adbf6-166">[Korzyść użycia hybrydowego platformy Azure](https://azure.microsoft.com/pricing/hybrid-benefit) to korzyść cenowa dla klientów korzystających z licencji z programem Software Assurance, która pomaga zmaksymalizować wartość istniejących inwestycji w system Windows Server i/lub SQL Server licencje licencyjne podczas migracji na platformę Azure.</span><span class="sxs-lookup"><span data-stu-id="adbf6-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="adbf6-167">Uprawnieni klienci mogą zaoszczędzić do 40% \* na platformie Azure Virtual Machines (infrastruktura jako usługa lub IaaS) i zaoszczędzić do 55% na Azure SQL Database (platforma jako usługa lub PaaS) i SQL Server na platformie Azure Virtual Machines (IaaS) z Korzyść użycia hybrydowego platformy Azure, które zwiększają się do 80% w połączeniu z wystąpieniami zarezerwowanymi platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="adbf6-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="adbf6-168">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="adbf6-168">Next steps</span></span>

- [<span data-ttu-id="adbf6-169">Często zadawane pytania dotyczące korzyści użycia hybrydowego platformy Azure</span><span class="sxs-lookup"><span data-stu-id="adbf6-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="adbf6-170">\* Rzeczywiste oszczędności mogą różnić się w zależności od regionu, typu wystąpienia lub użycia.</span><span class="sxs-lookup"><span data-stu-id="adbf6-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>
