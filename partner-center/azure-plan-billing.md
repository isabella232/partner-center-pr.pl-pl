---
title: Azure plan rozliczania — faktury & pliki Rekonesans
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak uzyskać dostęp do struktury plików faktur i uzgodnień uzgadniania dla planu platformy Azure i zrozumieć ją.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 1dc683c194de158dc7a4dac541b37631f3be1f1e
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534696"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="b6aa9-103">Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b6aa9-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="b6aa9-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="b6aa9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b6aa9-105">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="b6aa9-105">Admin agent</span></span>
- <span data-ttu-id="b6aa9-106">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="b6aa9-106">Billing admin</span></span>
- <span data-ttu-id="b6aa9-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="b6aa9-107">Global admin</span></span>

<span data-ttu-id="b6aa9-108">W tym artykule wyjaśniono, jak uzyskać dostęp do struktury pliku faktury i uzgodnienia dotyczącej rozliczeń dla planu platformy Azure i zrozumieć ją.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="b6aa9-109">Rozliczenia zgodnie z planem platformy Azure to uproszczone środowisko rozliczeniowe korzystające z wyrównanej pojedynczej daty rozliczania i okresu rozliczeniowego w kalendarzu.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="b6aa9-110">Podsumowanie podstawy rozliczeń</span><span class="sxs-lookup"><span data-stu-id="b6aa9-110">Summary of billing essentials</span></span>

- <span data-ttu-id="b6aa9-111">**Data faktury**: plik faktury i uzgodnienia będą dostępne na pulpicie nawigacyjnym/interfejsie API Centrum partnerskiego przez 8 (północy czasu UTC).</span><span class="sxs-lookup"><span data-stu-id="b6aa9-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="b6aa9-112">**Okres rozliczeniowy faktury**: okres rozliczeniowy faktury jest wyrównany do miesiąca kalendarzowego, na przykład 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="b6aa9-113">**Opłaty za okresy usługi**: opłaty zostaną wyrównane do miesiąca kalendarzowego.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="b6aa9-114">Na przykład jeśli Partner rozliczeń dodaje usługi platformy Azure w ramach planu platformy Azure w dniu 10/15, a klient zacznie zużywać usługi platformy Azure w dniu 10/15, wówczas rozliczenia partner otrzymają faktury/Rekonesans na 11/8 w celu użycia przez klienta okresu usługi 10/15-10/31.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="b6aa9-115">Faktury w następnym miesiącu, które mają zostać wygenerowane w dniu 12/8, zawierają wszystkie opłaty za okres usługi 11/1-11/31.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="b6aa9-116">**Termin płatności faktury**: NET 60 dni.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="b6aa9-117">**Waluta faktury**: partnerzy będą nadal rozliczani w country'sej walucie klienta.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="b6aa9-118">Na przykład jeśli Partner rozliczy jest w Irlandii z klientami w Wielkiej Brytanii, Norwegii i Niemczech, wówczas rozliczka będzie otrzymywać GBP, NOK i fakturę w EUR/rekonesans.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="b6aa9-119">**Zachęty dla partnerów**: płatne 45 dni od końca miesiąca faktury.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="b6aa9-120">Uzyskiwanie dostępu do faktur i plików uzgadniania</span><span class="sxs-lookup"><span data-stu-id="b6aa9-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="b6aa9-121">Administrator globalny lub administrator rozliczeń dla Twojej firmy otrzyma wiadomość e-mail, gdy faktura będzie gotowa do wyświetlenia.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="b6aa9-122">Aby uzyskać dostęp do pliku faktury i uzgodnienia:</span><span class="sxs-lookup"><span data-stu-id="b6aa9-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="b6aa9-123">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b6aa9-124">W menu Centrum partnerskiego wybierz pozycję **rozliczenia**.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="b6aa9-125">Wybierz kartę **cykliczną** i **jednorazową** oraz daną walutę.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="godzin":::

4. <span data-ttu-id="b6aa9-127">Wybierz pozycję **Faktura** lub **plik uzgadniania**.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="b6aa9-128">Aby wyświetlić historyczne faktury i pliki Rekonesans, rozwiń wiersz historia rozliczeń poniżej.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="b6aa9-129">Informacje o użyciu</span><span class="sxs-lookup"><span data-stu-id="b6aa9-129">Understanding usage data</span></span> 

1. <span data-ttu-id="b6aa9-130">Azure plan to główny lub najwyższego poziomu kontenera do użycia.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="b6aa9-131">Całe użycie jest powiązane z powrotem z jednym planem platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="b6aa9-132">W ramach planu będzie co najmniej jedna subskrypcja platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="b6aa9-133">Są to kontenery używane do zarządzania zasobami i ich wdrażania.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="b6aa9-134">W ramach subskrypcji grupy zasobów dodają do zasobów grupy.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="b6aa9-135">Każdy zasób jest wdrażany w jednej grupie zasobów.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="b6aa9-136">Przykłady zasobów obejmują maszyny wirtualne i konta magazynu.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="b6aa9-137">Liczniki emisji zasobów: Liczniki są pomiary zużycia zasobu, a jeden zasób może emitować użycie dla wielu liczników.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="b6aa9-138">Liczniki są identyfikowane przez ProductId, identyfikatora skuId i AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="b6aa9-139">Hierarchia grup zasobów i pomiarów subskrypcji</span><span class="sxs-lookup"><span data-stu-id="b6aa9-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="b6aa9-140">**Konto platformy Azure (dzierżawca)**</span><span class="sxs-lookup"><span data-stu-id="b6aa9-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="b6aa9-141">Subskrypcja A</span><span class="sxs-lookup"><span data-stu-id="b6aa9-141">Subscription A</span></span>
    - <span data-ttu-id="b6aa9-142">Przesourceing 1</span><span class="sxs-lookup"><span data-stu-id="b6aa9-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="b6aa9-143">Maszyna wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="b6aa9-144">Licznik obliczeń</span><span class="sxs-lookup"><span data-stu-id="b6aa9-144">Compute meter</span></span>
        - <span data-ttu-id="b6aa9-145">Sieć wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="b6aa9-146">Brak licznika rozliczeń</span><span class="sxs-lookup"><span data-stu-id="b6aa9-146">No billing meter</span></span>

    - <span data-ttu-id="b6aa9-147">Przesourceing 2</span><span class="sxs-lookup"><span data-stu-id="b6aa9-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="b6aa9-148">Maszyna wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="b6aa9-149">Licznik komputera</span><span class="sxs-lookup"><span data-stu-id="b6aa9-149">Computer meter</span></span>
        - <span data-ttu-id="b6aa9-150">Dysk zarządzany przez SSD w warstwie Premium (zasób)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="b6aa9-151">Licznik pojemności magazynu</span><span class="sxs-lookup"><span data-stu-id="b6aa9-151">Storage capacity meter</span></span>
            - <span data-ttu-id="b6aa9-152">Licznik operacji magazynu</span><span class="sxs-lookup"><span data-stu-id="b6aa9-152">Storage operations meter</span></span>

- <span data-ttu-id="b6aa9-153">Subskrypcja B — resourceing 1 — Azure SQL (Resource) — metry jednostek DTU-VPN Gateway (zasób) — licznik bramy sieci VPN</span><span class="sxs-lookup"><span data-stu-id="b6aa9-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="b6aa9-154">Przesourceing 2</span><span class="sxs-lookup"><span data-stu-id="b6aa9-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="b6aa9-155">Interfejs Virtual Network (zasób)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="b6aa9-156">Brak licznika rozliczeń</span><span class="sxs-lookup"><span data-stu-id="b6aa9-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="b6aa9-157">Przeczytaj fakturę</span><span class="sxs-lookup"><span data-stu-id="b6aa9-157">Read the invoice</span></span>

1. <span data-ttu-id="b6aa9-158">Faktura będzie dostępna nie później niż w ciągu każdego miesiąca.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="b6aa9-159">Partnerzy mają 60 dni, aby przekazać płatność.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="b6aa9-160">Okres rozliczeniowy będzie obejmować dany miesiąc kalendarzowy, na przykład 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="b6aa9-161">Opłaty są naliczane za liczbę netto korekt (kwota to netto za "Partner".</span><span class="sxs-lookup"><span data-stu-id="b6aa9-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="b6aa9-162">Aby uzyskać dodatkowe informacje dotyczące rozliczeń, zapoznaj się z plikiem faktury Rekonesans i dzienną oceną plików użycia.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="faktury":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="b6aa9-164">Przeczytaj plik uzgadniania faktur</span><span class="sxs-lookup"><span data-stu-id="b6aa9-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="b6aa9-165">Każda kombinacja planu i licznika platformy Azure może mieć do dwóch wierszy rozliczeń w pliku rekonesans.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="b6aa9-166">Jeśli licznik zakwalifikowany dla dowolnego typu rabatu lub kredytu (na przykład rabaty warstwowe lub środki uzyskane przez partnera dla usług zarządzanych) w całym miesiącu kalendarzowym, plik Rekonesans będzie zawierać tylko jedną linię rozliczenia.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="b6aa9-167">Kolumna **PriceAdjusmentDescription** będzie odwoływać się do rabatu lub środków uzyskanych z tytułu uznania.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="b6aa9-168">Jeśli nie ma zasobów dla określonego licznika, które kwalifikują się do rabatu lub dla partnerów, plik Rekonesans będzie zawierać tylko jedną linię rozliczeniową, a obowiązująca cena jednostkowa to cena detaliczna (czyli cena jednostkowa).</span><span class="sxs-lookup"><span data-stu-id="b6aa9-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="b6aa9-169">Jeśli licznik lub wszystkie zasoby emitujące Ten licznik są zakwalifikowane dla partnerów w ramach **usług zarządzanych** przez część miesiąca, plik Rekonesans będzie zawierać dwa wiersze rozliczania.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="b6aa9-170">Jeden wiersz będzie reprezentować dni kwalifikowane, a drugi wiersz będzie reprezentować dni, w których licznik nie kwalifikuje się.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="b6aa9-171">Przeczytaj plik dziennego użycia</span><span class="sxs-lookup"><span data-stu-id="b6aa9-171">Read the daily usage file</span></span>

- <span data-ttu-id="b6aa9-172">Liczniki subskrypcji w ramach planu platformy Azure są klasyfikowane i są skumulowane w ujęciu dziennym.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="b6aa9-173">Środki na korzystanie z **usług zarządzanych przez partnerów** są określane i stosowane codziennie.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="b6aa9-174">Każdy miernik subskrypcji będzie miał wiersz na każdy dzień miesiąca, w którym wystąpiło zużycie.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="b6aa9-175">W poniższym przykładzie:</span><span class="sxs-lookup"><span data-stu-id="b6aa9-175">In the example below:</span></span>

  - <span data-ttu-id="b6aa9-176">Zliczanie środków zakwalifikowanych dla **partnerów uzyskano środki dla usług zarządzanych** przez 7/1-7/3 (Zwróć uwagę na to, że obowiązująca cena jednostkowa to cena detaliczna pomniejszona o środki</span><span class="sxs-lookup"><span data-stu-id="b6aa9-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="b6aa9-177">Licznik nie kwalifikuje się do uzyskania środków w wysokości dla **partnerów zarządzanych** przez 7/4-7/7 (Zwróć uwagę na to, że obowiązująca cena jednostkowa to cena detaliczna).</span><span class="sxs-lookup"><span data-stu-id="b6aa9-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="b6aa9-178">Zliczanie środków zakwalifikowanych dla **partnerów w przypadku usług zarządzanych** przez 7/8-7/31 (Zwróć uwagę na to, że obowiązująca cena jednostkowa to cena detaliczna pomniejszona o środki na partnerów</span><span class="sxs-lookup"><span data-stu-id="b6aa9-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="b6aa9-180">Faktura w walucie klienta</span><span class="sxs-lookup"><span data-stu-id="b6aa9-180">Invoice in customer currency</span></span>

<span data-ttu-id="b6aa9-181">Opłaty za usługi platformy Azure za pomocą planu platformy Azure są naliczane w USD i rozliczone w walucie klienta przypisanej do kraju.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="b6aa9-182">Jeśli waluta rozliczeń jest niezerowa, na ostatniej stronie faktury zostanie wyświetlona stawka obcej wymiany (FX).</span><span class="sxs-lookup"><span data-stu-id="b6aa9-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="b6aa9-183">Stawki FX są określane co miesiąc i stosowane do poniższej faktury.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="b6aa9-184">Aby zapoznać się z pełną listą walut krajów, zapoznaj się z tematem [dostępność nowych ofert handlowych i macierzami walutowymi klientów](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="b6aa9-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="b6aa9-185">Firma Microsoft będzie używać Thomson firmy Reuters do określenia stawek FX używanych do określania waluty cenowej do konwersji waluty rozliczeniowej.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-185">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="b6aa9-186">Stawki FX będą odświeżane i dostępne w dniu przed pierwszym miesiącem, dla którego mają zastosowanie.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-186">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="b6aa9-187">**Przykład**: opłaty za użycie za okres usługi od 1 sierpnia do 31 sierpnia będą naliczane przy użyciu kursu FX opublikowanego w dniu 31 lipca.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-187">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="b6aa9-188">Opłaty zostaną wyświetlone na fakturze z września, a stawka FX zostanie zanotowana na ostatniej stronie faktury.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-188">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="b6aa9-189">Rezerwacje platformy Azure</span><span class="sxs-lookup"><span data-stu-id="b6aa9-189">Azure reservations</span></span>


<span data-ttu-id="b6aa9-190">W przypadku kupowania [rezerwacji platformy Azure](azure-reservations.md) za pomocą planu platformy Azure można wybrać jednorazowe lub comiesięczne rozliczanie.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-190">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="b6aa9-191">Wydatki na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="b6aa9-191">Azure spending</span></span>

<span data-ttu-id="b6aa9-192">Istniejące środowisko wydatków platformy Azure zostanie zaktualizowane, aby obsługiwało nowe rozliczenia planu platformy Azure w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-192">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="b6aa9-193">Dzięki temu partnerzy mogą:</span><span class="sxs-lookup"><span data-stu-id="b6aa9-193">This enables partners to:</span></span>

- <span data-ttu-id="b6aa9-194">Wyświetlanie i odbieranie alertów dotyczących zestawu budżetu na poziomie klienta oraz zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="b6aa9-194">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="b6aa9-195">Wyświetl łączne szacowane wydatki w planie platformy Azure (podzielone według zasobów i poziomów licznika)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-195">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="b6aa9-196">Ze względu na to, że model rozliczeń dla usług platformy Azure w ramach planu platformy Azure jest zużyciem po płatności, aby uniknąć wyższego rachunku niż przewidywane, partnerzy mogą stosować miesięczny budżet i śledzić procent użycia.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-196">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="b6aa9-197">Budżet można zastosować jednocześnie do jednego klienta lub wielu klientów.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-197">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Wydatki na platformie Azure":::

## <a name="next-steps"></a><span data-ttu-id="b6aa9-199">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="b6aa9-199">Next steps</span></span>

- <span data-ttu-id="b6aa9-200">Zobacz, w jaki sposób jest naliczany kredyt uzyskany przez partnera (PEC).</span><span class="sxs-lookup"><span data-stu-id="b6aa9-200">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="b6aa9-201">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego i Znajdź dostępną listę cenową.</span><span class="sxs-lookup"><span data-stu-id="b6aa9-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="b6aa9-202">Dowiedz się więcej o [kupowaniu planu platformy Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-202">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="b6aa9-203">Zobacz cennik [dla nowego środowiska handlowego w programie CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="b6aa9-203">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
