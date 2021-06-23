---
title: Rozliczenia planu platformy Azure — pliki & i pliki rekonfigurowane
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak uzyskać dostęp do struktury plików faktur i uzgodnień związanej z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551524"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="95f19-103">Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="95f19-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="95f19-104">**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="95f19-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="95f19-105">W tym artykule wyjaśniono, jak uzyskać dostęp do struktury plików faktur i uzgodnień związanej z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć.</span><span class="sxs-lookup"><span data-stu-id="95f19-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="95f19-106">Rozliczenia w ramach planu platformy Azure to uproszczone środowisko rozliczeniowe korzystające ze dostosowanej pojedynczej daty rozliczeniowej i okresu rozliczeniowego opartego na miesiącu kalendarzowym.</span><span class="sxs-lookup"><span data-stu-id="95f19-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="95f19-107">Podsumowanie podstawowych informacji dotyczących rozliczeń</span><span class="sxs-lookup"><span data-stu-id="95f19-107">Summary of billing essentials</span></span>

- <span data-ttu-id="95f19-108">**Data faktury:** faktura i plik uzgodnień będą dostępne na pulpicie nawigacyjnym Partner Center nawigacyjnym/interfejsie API do 8 dnia (północ czasu UTC).</span><span class="sxs-lookup"><span data-stu-id="95f19-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="95f19-109">**Okres rozliczeniowy** faktury: okres rozliczeniowy faktury jest dopasowany do miesiąca kalendarzowego, na przykład 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="95f19-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="95f19-110">**Okresy obsługi opłat:** opłaty będą zgodne z miesiącem kalendarzowym.</span><span class="sxs-lookup"><span data-stu-id="95f19-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="95f19-111">Jeśli na przykład rozliczany partner dodaje usługi platformy Azure za pośrednictwem planu platformy Azure 10/15 i klient rozpocznie korzystanie z usług platformy Azure 10/15, rozliczany partner otrzyma fakturę/rekonesję w dniu 8.11.2015 r. za zużycie przez klienta w okresie 10/15 – 10/31.</span><span class="sxs-lookup"><span data-stu-id="95f19-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="95f19-112">Faktura za następny miesiąc, która zostanie wygenerowana w dniu 8.12.2018, zawiera wszystkie opłaty za okres 11/1– 11/31.</span><span class="sxs-lookup"><span data-stu-id="95f19-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="95f19-113">**Termin płatności faktury:** 60 dni netto.</span><span class="sxs-lookup"><span data-stu-id="95f19-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="95f19-114">Waluta **faktury:** od 28 stycznia 2021 r. partnerzy w regionie Unii Europejskiej/DSM i Zjednoczonego Królestwa, którzy mają nowych klientów i istniejących klientów programu CSP, którzy po raz pierwszy kupują nowe oferty handlowe, których dzierżawy zostały utworzone przed 11 maja 2020 r., będą rozliczani za te zakupy w walucie lokalizacji partnera.</span><span class="sxs-lookup"><span data-stu-id="95f19-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="95f19-115">Partnerzy znajdujący się poza regionem Unii Europejskiej/DSM i Zjednoczonego Królestwa będą nadal rozliczani w walucie lokalizacji partnera.</span><span class="sxs-lookup"><span data-stu-id="95f19-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="95f19-116">**Zachęty dla partnerów:** Zapłacono 45 dni od końca miesiąca na fakturze.</span><span class="sxs-lookup"><span data-stu-id="95f19-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="95f19-117">Uzyskiwanie dostępu do faktur i plików uzgodnień</span><span class="sxs-lookup"><span data-stu-id="95f19-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="95f19-118">Gdy faktura będzie gotowa do wyświetlenia, administrator globalny lub administrator rozliczeń w firmie otrzyma wiadomość e-mail.</span><span class="sxs-lookup"><span data-stu-id="95f19-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="95f19-119">Aby uzyskać dostęp do pliku faktury i uzgodnień:</span><span class="sxs-lookup"><span data-stu-id="95f19-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="95f19-120">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="95f19-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="95f19-121">Z menu Partner Center wybierz pozycję **Rozliczenia.**</span><span class="sxs-lookup"><span data-stu-id="95f19-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="95f19-122">Wybierz kartę **Cykliczne** **i Jednorazowa** oraz walutę, która Cię interesuje.</span><span class="sxs-lookup"><span data-stu-id="95f19-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="Rozliczeń.":::

4. <span data-ttu-id="95f19-124">Wybierz **pozycję Plik** faktury lub **uzgodnień.**</span><span class="sxs-lookup"><span data-stu-id="95f19-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="95f19-125">Aby wyświetlić historyczne faktury i ponownie rozbudować pliki, rozwiń wiersz Historia rozliczeń poniżej.</span><span class="sxs-lookup"><span data-stu-id="95f19-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="95f19-126">Informacje o danych użycia</span><span class="sxs-lookup"><span data-stu-id="95f19-126">Understanding usage data</span></span> 

1. <span data-ttu-id="95f19-127">Plan platformy Azure to główny lub najwyższego poziomu kontener do użycia.</span><span class="sxs-lookup"><span data-stu-id="95f19-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="95f19-128">Całe użycie jest powiązane z pojedynczym planem platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="95f19-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="95f19-129">W ramach planu będzie co najmniej jedna subskrypcja platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="95f19-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="95f19-130">Są to kontenery używane do zarządzania zasobami i ich wdrażania.</span><span class="sxs-lookup"><span data-stu-id="95f19-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="95f19-131">W ramach subskrypcji grupy zasobów są dodawania do zasobów grupy.</span><span class="sxs-lookup"><span data-stu-id="95f19-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="95f19-132">Każdy zasób jest wdrażany w jednej grupie zasobów.</span><span class="sxs-lookup"><span data-stu-id="95f19-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="95f19-133">Przykłady zasobów obejmują maszyny wirtualne i konta magazynu.</span><span class="sxs-lookup"><span data-stu-id="95f19-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="95f19-134">Mierniki emisji zasobów: mierniki to pomiary zużycia zasobu, a jeden zasób może emitować użycie dla wielu mierników.</span><span class="sxs-lookup"><span data-stu-id="95f19-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="95f19-135">Mierniki są identyfikowane przez productId, SKUId i AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="95f19-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="95f19-136">Hierarchia grup zasobów subskrypcji i pomiary</span><span class="sxs-lookup"><span data-stu-id="95f19-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="95f19-137">**Konto platformy Azure (dzierżawa)**</span><span class="sxs-lookup"><span data-stu-id="95f19-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="95f19-138">Subskrypcja A</span><span class="sxs-lookup"><span data-stu-id="95f19-138">Subscription A</span></span>
    - <span data-ttu-id="95f19-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="95f19-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="95f19-140">Maszyna wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="95f19-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="95f19-141">Miernik zasobów obliczeniowych</span><span class="sxs-lookup"><span data-stu-id="95f19-141">Compute meter</span></span>
        - <span data-ttu-id="95f19-142">Sieć wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="95f19-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="95f19-143">Brak miernika rozliczeń</span><span class="sxs-lookup"><span data-stu-id="95f19-143">No billing meter</span></span>

    - <span data-ttu-id="95f19-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="95f19-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="95f19-145">Maszyna wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="95f19-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="95f19-146">Miernik komputera</span><span class="sxs-lookup"><span data-stu-id="95f19-146">Computer meter</span></span>
        - <span data-ttu-id="95f19-147">SSD w warstwie Premium dysk zarządzany (zasób)</span><span class="sxs-lookup"><span data-stu-id="95f19-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="95f19-148">Miernik pojemności magazynu</span><span class="sxs-lookup"><span data-stu-id="95f19-148">Storage capacity meter</span></span>
            - <span data-ttu-id="95f19-149">Miernik operacji magazynu</span><span class="sxs-lookup"><span data-stu-id="95f19-149">Storage operations meter</span></span>

- <span data-ttu-id="95f19-150">Subskrypcja B — ResourceGroup 1 — Azure SQL (zasób) — miernik jednostek DTU — VPN Gateway (zasób) — miernik bramy sieci VPN</span><span class="sxs-lookup"><span data-stu-id="95f19-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="95f19-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="95f19-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="95f19-152">Virtual Network interfejs (zasób)</span><span class="sxs-lookup"><span data-stu-id="95f19-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="95f19-153">Brak miernika rozliczeń</span><span class="sxs-lookup"><span data-stu-id="95f19-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="95f19-154">Odczytywanie faktury</span><span class="sxs-lookup"><span data-stu-id="95f19-154">Read the invoice</span></span>

1. <span data-ttu-id="95f19-155">Faktura będzie dostępna nie później niż w ósmej części każdego miesiąca.</span><span class="sxs-lookup"><span data-stu-id="95f19-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="95f19-156">Partnerzy mają 60 dni na odmówienie płatności.</span><span class="sxs-lookup"><span data-stu-id="95f19-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="95f19-157">Okres rozliczeniowy będzie obejmować dany miesiąc kalendarzowy, na przykład 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="95f19-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="95f19-158">Opłaty są naliczane netto korekt (kwota wynosi net "Środki uzyskane przez partnerów dla zarządzanych usług").</span><span class="sxs-lookup"><span data-stu-id="95f19-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="95f19-159">Zapoznaj się z plikiem rekonesfiguracji faktury i plikiem dziennego użycia, aby uzyskać dodatkowe szczegóły dotyczące rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="95f19-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktury.":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="95f19-161">Odczytywanie pliku uzgodnień faktur</span><span class="sxs-lookup"><span data-stu-id="95f19-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="95f19-162">Każda kombinacja planu i miernika platformy Azure może zawierać maksymalnie dwa wiersze rozliczeń w pliku rekonesfigurowania.</span><span class="sxs-lookup"><span data-stu-id="95f19-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="95f19-163">Jeśli miernik kwalifikował się do dowolnego typu rabatu lub środków (takich jak rabaty warstwowe lub środki uzyskane przez partnera dla usług zarządzanych) w całym miesiącu kalendarzowym, plik rekonesfiguracji będzie zawierać tylko jedną linię rozliczeniową.</span><span class="sxs-lookup"><span data-stu-id="95f19-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="95f19-164">Kolumna **PriceAdjusmentDescription** będzie odwoływać się do rabatu lub środków zdobytych.</span><span class="sxs-lookup"><span data-stu-id="95f19-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="95f19-165">Jeśli nie ma żadnych zasobów dla określonego miernika, który kwalifikował się do rabatu lub środków uzyskane przez partnera, plik rekonescji będzie zawierać tylko jedną linię rozliczeniową, a efektywną ceną jednostkową będzie cena detaliczna (czyli cena jednostkowa).</span><span class="sxs-lookup"><span data-stu-id="95f19-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="95f19-166">Jeśli miernik lub jakiekolwiek zasoby emitujące ten  licznik kwalifikowały się do środków uzyskane przez partnera dla usług zarządzanych przez część miesiąca, plik rekonescji będzie zawierać dwa wiersze rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="95f19-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="95f19-167">Jeden wiersz będzie reprezentować dni, w których miernik został zakwalifikowany, a drugi wiersz będzie reprezentować dni, w których miernik się nie kwalifikował.</span><span class="sxs-lookup"><span data-stu-id="95f19-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

>[!NOTE]
><span data-ttu-id="95f19-168">Możesz uzgodnić zużycie platformy Azure w pliku ponownego zakupu w ramach jednego zakupu.</span><span class="sxs-lookup"><span data-stu-id="95f19-168">You can reconcile your Azure consumption in your one-time purchase recon file.</span></span> <span data-ttu-id="95f19-169">W tym celu przejdź do pliku z rekonescją dziennego użycia i wyszukaj swój subscriptionID.</span><span class="sxs-lookup"><span data-stu-id="95f19-169">To do this, go to your daily-rated usage recon file and search for your SubscriptionID.</span></span> <span data-ttu-id="95f19-170">Spowoduje to wyświetlenie wszystkich kosztów skojarzonych z identyfikatorem planu platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="95f19-170">This will display all costs associated with your Azure Plan ID.</span></span> <span data-ttu-id="95f19-171">Twoja subskrypcja platformy Azure jest wyświetlana jako entitlementID.</span><span class="sxs-lookup"><span data-stu-id="95f19-171">Your Azure SubscriptionID is shown as the EntitlementID.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="95f19-172">Odczytywanie pliku dziennego użycia</span><span class="sxs-lookup"><span data-stu-id="95f19-172">Read the daily usage file</span></span>

- <span data-ttu-id="95f19-173">Mierniki subskrypcji w ramach planu platformy Azure są codziennie oceniane i skumulowane.</span><span class="sxs-lookup"><span data-stu-id="95f19-173">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="95f19-174">**Środków uzyskane przez partnerów na usługi zarządzane** są określane i stosowane codziennie.</span><span class="sxs-lookup"><span data-stu-id="95f19-174">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="95f19-175">Każdy licznik subskrypcji będzie miał wiersz dla każdego dnia miesiąca, w którym było zużycie.</span><span class="sxs-lookup"><span data-stu-id="95f19-175">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="95f19-176">W poniższym przykładzie:</span><span class="sxs-lookup"><span data-stu-id="95f19-176">In the example below:</span></span>

  - <span data-ttu-id="95f19-177">Miernik zakwalifikowany do środków **uzyskane** przez partnerów dla usług zarządzanych w okresie od 7/1 do 7/3 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniejsza niż kredyt uzyskane przez partnera.</span><span class="sxs-lookup"><span data-stu-id="95f19-177">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="95f19-178">Miernik nie kwalifikował  się do środków uzyskane przez partnerów na usługi zarządzane w okresie od 7/4 do 7/7 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna).</span><span class="sxs-lookup"><span data-stu-id="95f19-178">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="95f19-179">Miernik **zakwalifikowany** do środków uzyskane przez partnerów dla usług zarządzanych w okresie od 7/8 do 7/31 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniejsza niż kredyt uzyskane przez partnera).</span><span class="sxs-lookup"><span data-stu-id="95f19-179">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="95f19-181">Faktura w walucie klienta</span><span class="sxs-lookup"><span data-stu-id="95f19-181">Invoice in customer currency</span></span>

<span data-ttu-id="95f19-182">Opłaty za usługi platformy Azure w ramach planu platformy Azure będą naliczane w USD i rozliczane w walucie przypisanej do kraju klienta.</span><span class="sxs-lookup"><span data-stu-id="95f19-182">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="95f19-183">Jeśli waluta rozliczeniowa nie jest w USD, używany kurs wymiany walut (FX) będzie wyświetlany na ostatniej stronie faktury.</span><span class="sxs-lookup"><span data-stu-id="95f19-183">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="95f19-184">Stawki FX są określane co miesiąc i stosowane do poniższej faktury.</span><span class="sxs-lookup"><span data-stu-id="95f19-184">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="95f19-185">Aby uzyskać pełną listę walut krajów, zapoznaj się z nową ofertą handlową dla dostępności [kraju i macierzą walut klientów.](https://go.microsoft.com/fwlink/?linkid=2112354)</span><span class="sxs-lookup"><span data-stu-id="95f19-185">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="95f19-186">Firma Microsoft stosuje wstępnie określony kurs wymiany do podstawowych cen USD, aby uzyskać łączne opłaty naliczane za usługi platformy Azure zakupione lub zużyte w każdym miesiącu kalendarzowym.</span><span class="sxs-lookup"><span data-stu-id="95f19-186">Microsoft applies a predetermined exchange rate to base USD prices to arrive at total charges incurred for Azure services purchased or consumed each calendar month.</span></span> <span data-ttu-id="95f19-187">Miesięczny kurs wymiany to średni kurs opublikowany przez thomson Reuters (zazwyczaj) dwa dni robocze przed końcem poprzedniego miesiąca o godzinie 16:00 GMT.</span><span class="sxs-lookup"><span data-stu-id="95f19-187">The monthly exchange rate is the mid-rate published by Thomson Reuters (typically) two business days prior to the preceding month-end at 4:00 pm GMT.</span></span> 

<span data-ttu-id="95f19-188">**Na przykład** Grudniowy kurs wymiany firmy Microsoft będzie wartością średniego kursu wymiany Thomson Reuters z 29 listopada lub około 29 listopada dla danej waluty.</span><span class="sxs-lookup"><span data-stu-id="95f19-188">**For example,** Microsoft’s December exchange rate would be the Thomson Reuters mid-rate on or around November 29 for a given currency.</span></span> <span data-ttu-id="95f19-189">Ta stawka będzie stosowana do wszystkich zakupów w tej walucie od 1 grudnia do 31 grudnia.</span><span class="sxs-lookup"><span data-stu-id="95f19-189">That rate will be applied to all purchases in that currency from December 1 to December 31.</span></span> 

## <a name="azure-reservations"></a><span data-ttu-id="95f19-190">Rezerwacje platformy Azure</span><span class="sxs-lookup"><span data-stu-id="95f19-190">Azure reservations</span></span>


<span data-ttu-id="95f19-191">W przypadku zakupu [rezerwacji platformy Azure](azure-reservations.md) za pośrednictwem planu platformy Azure możesz wybrać rozliczenia godzinowe lub miesięczne.</span><span class="sxs-lookup"><span data-stu-id="95f19-191">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="95f19-192">Wydatki na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="95f19-192">Azure spending</span></span>

<span data-ttu-id="95f19-193">Istniejące środowisko wydatków na platformę Azure zostanie zaktualizowane w celu obsługi nowych rozliczeń planu platformy Azure w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="95f19-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="95f19-194">Dzięki temu partnerzy mogą:</span><span class="sxs-lookup"><span data-stu-id="95f19-194">This enables partners to:</span></span>

- <span data-ttu-id="95f19-195">Wyświetlanie i odbieranie alertów dotyczących budżetu ustawionego na poziomie klienta oraz zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="95f19-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="95f19-196">Wyświetlanie łącznych szacowanych wydatków w ramach planu platformy Azure (podzielone według poziomu zasobu i miernika)</span><span class="sxs-lookup"><span data-stu-id="95f19-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="95f19-197">Ponieważ model rozliczeń dla usług platformy Azure za pośrednictwem planu platformy Azure to użycie po płatności, aby uniknąć większego rachunku, niż oczekiwano, partnerzy mogą zastosować miesięczny budżet i śledzić procent użycia.</span><span class="sxs-lookup"><span data-stu-id="95f19-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="95f19-198">Budżet można zastosować do jednego klienta lub wielu klientów jednocześnie.</span><span class="sxs-lookup"><span data-stu-id="95f19-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Wydatki na platformę Azure.":::

## <a name="next-steps"></a><span data-ttu-id="95f19-200">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="95f19-200">Next steps</span></span>

- <span data-ttu-id="95f19-201">Zobacz, jak są obliczane punkty uzyskane przez partnera.</span><span class="sxs-lookup"><span data-stu-id="95f19-201">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="95f19-202">Zaloguj się do Partner Center [pulpitu nawigacyjnego i](https://partner.microsoft.com/dashboard/) znajdź dostępny cennik.</span><span class="sxs-lookup"><span data-stu-id="95f19-202">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="95f19-203">Dowiedz się więcej [o zakupie planu platformy Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="95f19-203">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="95f19-204">Zobacz cennik nowego doświadczenia handlowego w [programie CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="95f19-204">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
