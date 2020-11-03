---
title: Rezerwacje platformy Azure & subskrypcje serwera
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o możliwościach dostawcy rozwiązań w chmurze, aby uzyskać, zainicjować i zarządzać rezerwacjami platformy Azure oraz subskrypcjami serwera dla klientów.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529908"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="0fbcc-103">Pozyskiwanie, Inicjowanie obsługi & Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych platformy Azure (RI) i subskrypcjami serwera dla klientów</span><span class="sxs-lookup"><span data-stu-id="0fbcc-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="0fbcc-104">Dotyczy:</span><span class="sxs-lookup"><span data-stu-id="0fbcc-104">Applies to:</span></span>

- <span data-ttu-id="0fbcc-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="0fbcc-105">Partner Center</span></span>

<span data-ttu-id="0fbcc-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="0fbcc-106">**Appropriate roles**</span></span>

- <span data-ttu-id="0fbcc-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="0fbcc-107">Admin agent</span></span>
- <span data-ttu-id="0fbcc-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="0fbcc-108">Global admin</span></span>
- <span data-ttu-id="0fbcc-109">Agent pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="0fbcc-109">Helpdesk agent</span></span>
- <span data-ttu-id="0fbcc-110">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="0fbcc-110">Sales agent</span></span>
- <span data-ttu-id="0fbcc-111">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="0fbcc-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="0fbcc-112">Ten artykuł ma zastosowanie tylko do partnerów w programie Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="0fbcc-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="0fbcc-113">Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="0fbcc-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="0fbcc-114">Co to jest Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="0fbcc-114">What are Azure Reservations?</span></span>

<span data-ttu-id="0fbcc-115">Azure Reservations pomóc zaoszczędzić pieniądze przez przedpłatę za rok lub trzy lata maszyny wirtualnej, SQL Database pojemność obliczeniowa, Azure Cosmos DB przepływność lub inne zasoby platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="0fbcc-116">Funkcja przedpłaty umożliwia uzyskanie rabatu za zasoby, których używasz.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="0fbcc-117">Rezerwacje mogą znacząco obniżyć swoją maszynę wirtualną, obliczenia w usłudze SQL Database, Azure Cosmos DB i inne koszty zasobów do 72% w porównaniu z cenami z płatność zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="0fbcc-118">Rezerwacje umożliwiają skorzystanie z rabatu na rozliczenia i nie mają wpływu na stan środowiska uruchomieniowego Twoich zasobów.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="0fbcc-119">Aby uzyskać więcej informacji, zobacz [co to są Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="0fbcc-120">Dlaczego klienci kupują rezerwację?</span><span class="sxs-lookup"><span data-stu-id="0fbcc-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="0fbcc-121">W przypadku klientów z maszynami wirtualnymi, Azure Cosmos DB lub baz danych SQL, które są uruchamiane przez długi czas, zakup rezerwacji daje im największą opłacalną opcję.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="0fbcc-122">Na przykład jeśli klient ciągle uruchamia cztery wystąpienia usługi bez rezerwacji, opłaty są naliczone według stawek płatność zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="0fbcc-123">Jeśli kupią rezerwację dla tych zasobów, natychmiast uzyskają rabat rezerwacji.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="0fbcc-124">Zasoby nie będą już obciążane opłatami według stawek płatności zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="0fbcc-125">Atrakcyjna nowa oferta platformy Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="0fbcc-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="0fbcc-126">Dzięki dołączeniu Azure Reservations i subskrypcji serwera do swojego programu CSP firma Microsoft lepiej umożliwia swoim partnerom rozwiązywanie problemów z coraz większym popytem w celu uzyskania bardziej ekonomicznych rozwiązań do obsługi wysoce przewidywalnych, trwałych obciążeń w chmurze.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="0fbcc-127">Program CSP umożliwia partnerom pozyskiwanie, Inicjowanie obsługi i zarządzanie subskrypcjami Azure Reservations i serwera w imieniu klientów komercyjnych za pośrednictwem Centrum partnerskiego firmy Microsoft i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="0fbcc-128">Oferujemy również partnerów w naszym programie CSP, w których można kupować rezerwacje platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="0fbcc-129">Partnerzy programu CSP mogą [kupować rezerwacje platformy Azure w imieniu klienta](azure-reservations-buying.md) lub mogą [zezwolić klientowi na kupowanie własnych rezerwacji](give-customers-permission.md) w ramach wcześniejszej subskrypcji platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="0fbcc-130">Azure Reservations zapewnić klientom elastyczność wirtualizacji dla szerokiego zakresu rozwiązań obliczeniowych, w tym tworzenia i testowania, uruchamiania aplikacji oraz rozszerzania centrum danych.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="0fbcc-131">W [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) na przykład komercyjni klienci mogą teraz zaoszczędzić do 72%, a w przeciwieństwie do cen maszyn wirtualnych z systemem Azure — po prostu przy zakupie lub "obsłużeniu" — w przypadku okresu 1-lub 3-letniego.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="0fbcc-132">Klienci korzystający z systemu Windows Server z Korzyść użycia hybrydowego platformy Azure, dostępną w ramach programu Software Assurance, będą mogli zaoszczędzić do 80% w porównaniu z cenami zgodnie z rzeczywistym użyciem.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="0fbcc-133">W przypadku niedopasowanej kombinacji atrakcyjnych cen i niedopasowanej elastyczności wdrożenia klienci będą widzieli najlepszą ogólną wartość, wybierając Azure Reservations:</span><span class="sxs-lookup"><span data-stu-id="0fbcc-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="0fbcc-134">Rezerwacje platformy Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-134">Azure reservations</span></span>

- <span data-ttu-id="0fbcc-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="0fbcc-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="0fbcc-136">Rezerwacje bazy danych SQL</span><span class="sxs-lookup"><span data-stu-id="0fbcc-136">SQL DB Reservations</span></span>
- <span data-ttu-id="0fbcc-137">Wystąpienie zarządzane SQL</span><span class="sxs-lookup"><span data-stu-id="0fbcc-137">SQL Managed Instance</span></span>
- <span data-ttu-id="0fbcc-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0fbcc-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="0fbcc-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="0fbcc-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="0fbcc-140">App Services</span><span class="sxs-lookup"><span data-stu-id="0fbcc-140">App Services</span></span>
- <span data-ttu-id="0fbcc-141">Azure Databricks rezerwacji jednostek</span><span class="sxs-lookup"><span data-stu-id="0fbcc-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="0fbcc-142">Dysk zarządzany</span><span class="sxs-lookup"><span data-stu-id="0fbcc-142">Managed Disk</span></span>
- <span data-ttu-id="0fbcc-143">Blokowy obiekt blob</span><span class="sxs-lookup"><span data-stu-id="0fbcc-143">Block blob</span></span>
- <span data-ttu-id="0fbcc-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="0fbcc-144">MySQL</span></span>
- <span data-ttu-id="0fbcc-145">Eksplorator danych platformy Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-145">Azure Data explorer</span></span>
- <span data-ttu-id="0fbcc-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="0fbcc-146">MariaDB</span></span>
- <span data-ttu-id="0fbcc-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="0fbcc-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="0fbcc-148">Subskrypcje serwera</span><span class="sxs-lookup"><span data-stu-id="0fbcc-148">Server subscriptions</span></span>

- <span data-ttu-id="0fbcc-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="0fbcc-149">Windows Server</span></span>
- <span data-ttu-id="0fbcc-150">Licencje CAL na Usługi pulpitu zdalnego (RDS)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="0fbcc-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="0fbcc-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="0fbcc-152">Subskrypcje roczne niezależnego dostawcy oprogramowania Linux</span><span class="sxs-lookup"><span data-stu-id="0fbcc-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="0fbcc-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="0fbcc-153">SUSE Linux</span></span>
- <span data-ttu-id="0fbcc-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="0fbcc-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="0fbcc-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="0fbcc-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="0fbcc-156">Subskrypcje roczne niezależnego dostawcy oprogramowania</span><span class="sxs-lookup"><span data-stu-id="0fbcc-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="0fbcc-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="0fbcc-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="0fbcc-158">Wprowadzenie</span><span class="sxs-lookup"><span data-stu-id="0fbcc-158">Getting started</span></span>

<span data-ttu-id="0fbcc-159">Aby zrozumieć, w jaki sposób można określić, Azure Reservations z klientami oraz jak najszybciej rozpocząć pracę, zalecamy następujące podejście do przeglądu materiałów gotowości:</span><span class="sxs-lookup"><span data-stu-id="0fbcc-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="0fbcc-160">Przejrzyj prezentacje przeglądowe i powiązane seminaria internetowe na potrzeby pozycji i pozycjonowania wartości klienta</span><span class="sxs-lookup"><span data-stu-id="0fbcc-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="0fbcc-161">Przejrzyj i zapoznaj się z współczesnym przewodnikiem operacyjnym handlu</span><span class="sxs-lookup"><span data-stu-id="0fbcc-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="0fbcc-162">Zapoznaj się z tematem często zadawanych subskrypcji na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="0fbcc-163">Informacje o aktualizacjach dla Azure Reservations i subskrypcji serwera w [interfejsie API Centrum partnerskiego (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="0fbcc-164">Zasoby</span><span class="sxs-lookup"><span data-stu-id="0fbcc-164">Resources</span></span>

<span data-ttu-id="0fbcc-165">Poniżej znajduje się kompleksowa Lista zasobów, które ułatwiają szybkie dołączanie do Azure Reservations transakcyjnych w centrum partnerskim:</span><span class="sxs-lookup"><span data-stu-id="0fbcc-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="0fbcc-166">Gotowość do sprzedaży</span><span class="sxs-lookup"><span data-stu-id="0fbcc-166">Sales readiness</span></span>

- [<span data-ttu-id="0fbcc-167">Azure Reservations i subskrypcje serwera z omówieniem Korzyść użycia hybrydowego platformy Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="0fbcc-168">Arkusz sprzedaży</span><span class="sxs-lookup"><span data-stu-id="0fbcc-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="0fbcc-169">Często zadawane pytania dla partnerów Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="0fbcc-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="0fbcc-170">Często zadawane pytania dla partnerów dotyczące Azure Reservations i bazy danych SQL</span><span class="sxs-lookup"><span data-stu-id="0fbcc-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="0fbcc-171">Licencja dostępu klienta (CAL) Usługi pulpitu zdalnego (RDS) (anons)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="0fbcc-172">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="0fbcc-173">Subskrypcje serwera</span><span class="sxs-lookup"><span data-stu-id="0fbcc-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="0fbcc-174">Baza danych SQL na platformie Azure — omówienie</span><span class="sxs-lookup"><span data-stu-id="0fbcc-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="0fbcc-175">Rezerwacje bazy danych SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="0fbcc-176">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="0fbcc-177">Wystąpienie zarządzane SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="0fbcc-178">SUSE i Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="0fbcc-179">Red Hat Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="0fbcc-180">SUSE Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="0fbcc-181">System Linux na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="0fbcc-182">Przegląd cen platformy Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="0fbcc-183">Kalkulator cen platformy Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="0fbcc-184">Azure Databricks rezerwacji jednostek</span><span class="sxs-lookup"><span data-stu-id="0fbcc-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="0fbcc-185">Cennik dostawcy usług kryptograficznych **Microsoft Azure: listy zarezerwowanych wystąpień** i cennika usługi **subskrypcje oprogramowania** są dostępne na stronie [& oferty](https://partner.microsoft.com/pcv/sales) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="0fbcc-186">Szkolenia</span><span class="sxs-lookup"><span data-stu-id="0fbcc-186">Training</span></span>

<span data-ttu-id="0fbcc-187">Zarejestruj się, aby wyświetlić [seminaria internetowe gotowości do licencjonowania komercyjnego](https://commercial-licensing.eventbuilder.com/FY2019_ALL) oraz zdarzenia na żądanie.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="0fbcc-188">Zdarzenia gotowości do licencjonowania na żądanie obejmują tematy takie jak:</span><span class="sxs-lookup"><span data-stu-id="0fbcc-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="0fbcc-189">Usługi CSP online, dostawcy CSP Azure i ogólne aktualizacje licencjonowania, w tym Azure (listopad 2018)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="0fbcc-190">Zarezerwowana pojemność bazy danych SQL & elastyczność rozmiaru wystąpienia (sierpień 2018)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="0fbcc-191">Subskrypcje serwera w programie CSP (lipiec 2018)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="0fbcc-192">Przegląd Azure Reservations w programie CSP (2018 maja)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="0fbcc-193">Inne przydatne szkolenia obejmują [moduł licencjonowania platformy Azure na Uniwersytecie dla partnerów](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="0fbcc-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="0fbcc-194">Operacje</span><span class="sxs-lookup"><span data-stu-id="0fbcc-194">Operations</span></span>

- <span data-ttu-id="0fbcc-195">[Współczesny Przewodnik dotyczący operacji handlowych](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (zaktualizowany): kompleksowy przewodnik dotyczący najważniejszych zasad i aspektów operacyjnych, takich jak umowy, porządkowanie przez centrum partnerskie, faktury, szczegóły cennika, zachęty, plik uzgodnienia, interfejs API/zestaw SDK, piaskownica i udostępnione usługi partnera platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="0fbcc-196">Współczesne oferty dotyczące dostępności kraju i waluty klienta</span><span class="sxs-lookup"><span data-stu-id="0fbcc-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="0fbcc-197">Sprzedaj Microsoft Azure wystąpienia zarezerwowane</span><span class="sxs-lookup"><span data-stu-id="0fbcc-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="0fbcc-198">Kup rezerwacje Microsoft Azure w imieniu klientów</span><span class="sxs-lookup"><span data-stu-id="0fbcc-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="0fbcc-199">Zarządzanie rezerwacjami platformy Azure w imieniu klientów</span><span class="sxs-lookup"><span data-stu-id="0fbcc-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="0fbcc-200">Rozliczenia dla rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="0fbcc-201">Rozmiar maszyny wirtualnej dla maksymalnego użycia zastrzeżenia</span><span class="sxs-lookup"><span data-stu-id="0fbcc-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="0fbcc-202">Interfejs API Centrum partnerskiego (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="0fbcc-203">Usługi pulpitu zdalnego</span><span class="sxs-lookup"><span data-stu-id="0fbcc-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="0fbcc-204">Korzyść użycia hybrydowego platformy Azure</span><span class="sxs-lookup"><span data-stu-id="0fbcc-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="0fbcc-205">[Korzyść użycia hybrydowego platformy Azure](https://azure.microsoft.com/pricing/hybrid-benefit) pomaga uzyskać więcej wartości z licencji systemu Windows Server i zaoszczędzić do \* 47 procent na maszynach wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="0fbcc-206">Możesz korzystać z korzyści z licencji systemu Windows Server Datacenter i Standard Edition, które są objęte programem Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="0fbcc-207">W zależności od wersji można przekonwertować licencje lub użyć ich ponownie w celu uruchomienia maszyn wirtualnych z systemem Windows Server na platformie Azure i zaliczyć niższą podstawową stawkę obliczeniową (stawki za maszyny wirtualne z systemem Linux).</span><span class="sxs-lookup"><span data-stu-id="0fbcc-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="0fbcc-208">Zobacz również [korzyść użycia hybrydowego platformy Azure często zadawane pytania](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="0fbcc-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="0fbcc-209">\* Rzeczywiste oszczędności mogą różnić się w zależności od regionu, typu wystąpienia lub użycia.</span><span class="sxs-lookup"><span data-stu-id="0fbcc-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
