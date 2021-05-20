---
title: Rozliczenia planu platformy Azure — pliki & ponownego rozliczania
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak uzyskać dostęp do struktury pliku faktur i uzgodnień związanej z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 757383ee264e58e7b4dc8ffefafe213cb49acb79
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149795"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="72575-103">Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="72575-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="72575-104">**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="72575-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="72575-105">W tym artykule wyjaśniono, jak uzyskać dostęp do struktury plików faktur i uzgodnień związanych z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć.</span><span class="sxs-lookup"><span data-stu-id="72575-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="72575-106">Rozliczenia w ramach planu platformy Azure to uproszczone środowisko rozliczeniowe korzystające ze dostosowanej pojedynczej daty rozliczeniowej i okresu rozliczeniowego opartego na miesiącu kalendarzowym.</span><span class="sxs-lookup"><span data-stu-id="72575-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="72575-107">Podsumowanie podstawowych informacji o rozliczeniach</span><span class="sxs-lookup"><span data-stu-id="72575-107">Summary of billing essentials</span></span>

- <span data-ttu-id="72575-108">**Data faktury:** faktura i plik uzgodnień będą dostępne na Partner Center nawigacyjnym/interfejsie API do 8 .00 (północ czasu UTC).</span><span class="sxs-lookup"><span data-stu-id="72575-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="72575-109">**Okres rozliczeniowy** faktury: okres rozliczeniowy faktury jest dopasowany do miesiąca kalendarzowego, na przykład 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="72575-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="72575-110">**Okresy obsługi opłat:** Opłaty będą zgodne z miesiącem kalendarzowym.</span><span class="sxs-lookup"><span data-stu-id="72575-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="72575-111">Jeśli na przykład rozliczany partner dodaje usługi platformy Azure za pośrednictwem planu platformy Azure w dniu 10/15 i klient rozpocznie korzystanie z usług platformy Azure 10/15, wówczas rozliczany partner otrzyma fakturę/rekonesję w dniu 8.11.01. za zużycie przez klienta w okresie 10/15–10/31.</span><span class="sxs-lookup"><span data-stu-id="72575-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="72575-112">Faktura za następny miesiąc, która zostanie wygenerowana w dniu 8.12.2018, zawiera wszystkie opłaty za okres 11/1– 11/31.</span><span class="sxs-lookup"><span data-stu-id="72575-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="72575-113">**Termin płatności faktury:** 60 dni netto.</span><span class="sxs-lookup"><span data-stu-id="72575-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="72575-114">Waluta **faktury:** od 28 stycznia 2021 r. partnerzy w regionie UNII EUROPEJSKIEJ/EFTA i Zjednoczonego Królestwa, którzy mają nowych klientów i istniejących klientów programu CSP, którzy kupują nowe oferty handlowe po raz pierwszy, których dzierżawy zostały utworzone przed 11 maja 2020 r., będą rozliczani za te zakupy w walucie lokalizacji partnera.</span><span class="sxs-lookup"><span data-stu-id="72575-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="72575-115">Partnerzy znajdujący się poza regionem Unii Europejskiej/EFTA i Zjednoczonego Królestwa będą nadal rozliczani w walucie lokalizacji partnera.</span><span class="sxs-lookup"><span data-stu-id="72575-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="72575-116">**Zachęty dla partnerów:** Zapłacono 45 dni od końca miesiąca na fakturze.</span><span class="sxs-lookup"><span data-stu-id="72575-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="72575-117">Uzyskiwanie dostępu do faktur i plików uzgodnień</span><span class="sxs-lookup"><span data-stu-id="72575-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="72575-118">Administrator globalny lub administrator rozliczeń w firmie otrzyma wiadomość e-mail, gdy faktura będzie gotowa do wyświetlenia.</span><span class="sxs-lookup"><span data-stu-id="72575-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="72575-119">Aby uzyskać dostęp do pliku faktury i uzgodnień:</span><span class="sxs-lookup"><span data-stu-id="72575-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="72575-120">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="72575-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="72575-121">Z menu Partner Center wybierz pozycję **Rozliczenia.**</span><span class="sxs-lookup"><span data-stu-id="72575-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="72575-122">Wybierz kartę **Cykliczne** i **Jednorazowa** oraz walutę, która Cię interesuje.</span><span class="sxs-lookup"><span data-stu-id="72575-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="billing":::

4. <span data-ttu-id="72575-124">Wybierz **pozycję Plik** faktury lub **uzgodnień.**</span><span class="sxs-lookup"><span data-stu-id="72575-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="72575-125">Aby wyświetlić faktury historyczne i ponownie rozbudować pliki, rozwiń wiersz Historia rozliczeń poniżej.</span><span class="sxs-lookup"><span data-stu-id="72575-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="72575-126">Informacje o danych użycia</span><span class="sxs-lookup"><span data-stu-id="72575-126">Understanding usage data</span></span> 

1. <span data-ttu-id="72575-127">Plan platformy Azure jest kontenerem głównym lub najwyższego poziomu do użycia.</span><span class="sxs-lookup"><span data-stu-id="72575-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="72575-128">Całe użycie jest powiązane z pojedynczym planem platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="72575-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="72575-129">W ramach planu będzie co najmniej jedna subskrypcja platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="72575-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="72575-130">Są to kontenery używane do zarządzania zasobami i ich wdrażania.</span><span class="sxs-lookup"><span data-stu-id="72575-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="72575-131">W ramach subskrypcji grupy zasobów są dodawania do zasobów grupy.</span><span class="sxs-lookup"><span data-stu-id="72575-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="72575-132">Każdy zasób jest wdrażany w jednej grupie zasobów.</span><span class="sxs-lookup"><span data-stu-id="72575-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="72575-133">Przykłady zasobów obejmują maszyny wirtualne i konta magazynu.</span><span class="sxs-lookup"><span data-stu-id="72575-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="72575-134">Mierniki emisji zasobów: mierniki to pomiary zużycia zasobu, a jeden zasób może emitować użycie dla wielu mierników.</span><span class="sxs-lookup"><span data-stu-id="72575-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="72575-135">Mierniki są identyfikowane przez productId, SKUId i AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="72575-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="72575-136">Hierarchia grup zasobów subskrypcji i pomiary</span><span class="sxs-lookup"><span data-stu-id="72575-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="72575-137">**Konto platformy Azure (dzierżawa)**</span><span class="sxs-lookup"><span data-stu-id="72575-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="72575-138">Subskrypcja A</span><span class="sxs-lookup"><span data-stu-id="72575-138">Subscription A</span></span>
    - <span data-ttu-id="72575-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="72575-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="72575-140">Maszyna wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="72575-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="72575-141">Miernik obliczeniowy</span><span class="sxs-lookup"><span data-stu-id="72575-141">Compute meter</span></span>
        - <span data-ttu-id="72575-142">Sieć wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="72575-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="72575-143">Brak miernika rozliczeń</span><span class="sxs-lookup"><span data-stu-id="72575-143">No billing meter</span></span>

    - <span data-ttu-id="72575-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="72575-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="72575-145">Maszyna wirtualna (zasób)</span><span class="sxs-lookup"><span data-stu-id="72575-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="72575-146">Miernik komputera</span><span class="sxs-lookup"><span data-stu-id="72575-146">Computer meter</span></span>
        - <span data-ttu-id="72575-147">SSD w warstwie Premium dysku zarządzanego (zasób)</span><span class="sxs-lookup"><span data-stu-id="72575-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="72575-148">Miernik pojemności magazynu</span><span class="sxs-lookup"><span data-stu-id="72575-148">Storage capacity meter</span></span>
            - <span data-ttu-id="72575-149">Miernik operacji magazynu</span><span class="sxs-lookup"><span data-stu-id="72575-149">Storage operations meter</span></span>

- <span data-ttu-id="72575-150">Subskrypcja B — ResourceGroup 1 — Azure SQL (zasób) — miernik jednostek DTU — VPN Gateway (zasób) — miernik bramy sieci VPN</span><span class="sxs-lookup"><span data-stu-id="72575-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="72575-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="72575-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="72575-152">Virtual Network interfejs (zasób)</span><span class="sxs-lookup"><span data-stu-id="72575-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="72575-153">Brak miernika rozliczeń</span><span class="sxs-lookup"><span data-stu-id="72575-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="72575-154">Odczytywanie faktury</span><span class="sxs-lookup"><span data-stu-id="72575-154">Read the invoice</span></span>

1. <span data-ttu-id="72575-155">Faktura będzie dostępna nie później niż ósmą część każdego miesiąca.</span><span class="sxs-lookup"><span data-stu-id="72575-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="72575-156">Partnerzy mają 60 dni na odmówienie płatności.</span><span class="sxs-lookup"><span data-stu-id="72575-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="72575-157">Okres rozliczeniowy będzie obejmować dany miesiąc kalendarzowy, na przykład 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="72575-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="72575-158">Opłaty są naliczane bez korekt (kwota jest netto "środki uzyskane przez partnerów dla zarządzanych usług").</span><span class="sxs-lookup"><span data-stu-id="72575-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="72575-159">Przejrzyj plik rekonesji faktury i plik dziennego użycia z ocenami, aby uzyskać dodatkowe szczegóły rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="72575-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktury":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="72575-161">Odczytywanie pliku uzgodnień faktur</span><span class="sxs-lookup"><span data-stu-id="72575-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="72575-162">Każda kombinacja planu i miernika platformy Azure może zawierać maksymalnie dwa wiersze rozliczeń w pliku rekonesfigurowania.</span><span class="sxs-lookup"><span data-stu-id="72575-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="72575-163">Jeśli miernik kwalifikował się do dowolnego typu rabatu lub środków (takich jak rabaty warstwowe lub środki uzyskane przez partnera dla usług zarządzanych) w całym miesiącu kalendarzowym, plik rekonesfiguracji będzie zawierać tylko jedną linię rozliczeniową.</span><span class="sxs-lookup"><span data-stu-id="72575-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="72575-164">Kolumna **PriceAdjusmentDescription** będzie odwoływać się do rabatu lub środków zdobytych.</span><span class="sxs-lookup"><span data-stu-id="72575-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="72575-165">Jeśli nie ma żadnych zasobów dla określonego miernika, który kwalifikował się do rabatu lub środków uzyskane przez partnera, plik rekonescji będzie zawierać tylko jedną linię rozliczeniową, a efektywną ceną jednostkową będzie cena detaliczna (czyli cena jednostkowa).</span><span class="sxs-lookup"><span data-stu-id="72575-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="72575-166">Jeśli miernik lub jakiekolwiek zasoby emitujące ten  licznik kwalifikowały się do środków uzyskane przez partnera dla usług zarządzanych przez część miesiąca, plik rekonescji będzie zawierać dwa wiersze rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="72575-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="72575-167">Jeden wiersz będzie reprezentować dni, w których miernik został zakwalifikowany, a drugi wiersz będzie reprezentować dni, w których miernik nie kwalifikował się.</span><span class="sxs-lookup"><span data-stu-id="72575-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="72575-168">Odczytywanie pliku dziennego użycia</span><span class="sxs-lookup"><span data-stu-id="72575-168">Read the daily usage file</span></span>

- <span data-ttu-id="72575-169">Mierniki subskrypcji w ramach planu platformy Azure są codziennie oceniane i skumulowane.</span><span class="sxs-lookup"><span data-stu-id="72575-169">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="72575-170">**Środków uzyskane przez partnerów na usługi zarządzane** są określane i stosowane codziennie.</span><span class="sxs-lookup"><span data-stu-id="72575-170">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="72575-171">Każdy licznik subskrypcji będzie miał wiersz dla każdego dnia miesiąca, w którym było zużycie.</span><span class="sxs-lookup"><span data-stu-id="72575-171">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="72575-172">W poniższym przykładzie:</span><span class="sxs-lookup"><span data-stu-id="72575-172">In the example below:</span></span>

  - <span data-ttu-id="72575-173">Miernik zakwalifikowany do środków **uzyskane** przez partnerów dla usług zarządzanych w okresie od 7/1 do 7/3 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniejsza niż kredyt uzyskane przez partnera.</span><span class="sxs-lookup"><span data-stu-id="72575-173">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="72575-174">Miernik nie kwalifikował  się do środków uzyskane przez partnerów na usługi zarządzane w okresie od 7/4 do 7/7 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna).</span><span class="sxs-lookup"><span data-stu-id="72575-174">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="72575-175">Miernik zakwalifikowany do środków **uzyskane** przez partnerów dla usług zarządzanych w okresie od 7/8 do 7/31 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniejsza niż kredyt uzyskane przez partnera).</span><span class="sxs-lookup"><span data-stu-id="72575-175">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="72575-177">Faktura w walucie klienta</span><span class="sxs-lookup"><span data-stu-id="72575-177">Invoice in customer currency</span></span>

<span data-ttu-id="72575-178">Opłaty za usługi platformy Azure w ramach planu platformy Azure będą naliczane w USD i rozliczane w walucie przypisanej do kraju klienta.</span><span class="sxs-lookup"><span data-stu-id="72575-178">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="72575-179">Jeśli waluta rozliczeniowa nie jest w USD, używany kurs wymiany walut (FX) będzie wyświetlany na ostatniej stronie faktury.</span><span class="sxs-lookup"><span data-stu-id="72575-179">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="72575-180">Stawki FX są określane co miesiąc i stosowane do poniższej faktury.</span><span class="sxs-lookup"><span data-stu-id="72575-180">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="72575-181">Aby uzyskać pełną listę walut krajów, zapoznaj się z nową ofertą handlową dla dostępności [kraju i macierzą walut klientów.](https://go.microsoft.com/fwlink/?linkid=2112354)</span><span class="sxs-lookup"><span data-stu-id="72575-181">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="72575-182">Firma Microsoft obserwuje giełdę w Londynie w celu konwersji.</span><span class="sxs-lookup"><span data-stu-id="72575-182">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="72575-183">Używamy kursu wymiany, który jest równy kursowi wymiany przechwyconej w ostatniej sekundzie ostatniego dnia biznesowego miesiąca na giełdzie w Londynie.</span><span class="sxs-lookup"><span data-stu-id="72575-183">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="72575-184">Stawki FX zostaną odświeżone i udostępnione w dniu przed pierwszym miesiącem, dla którego mają zastosowanie.</span><span class="sxs-lookup"><span data-stu-id="72575-184">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="72575-185">Rezerwacje platformy Azure</span><span class="sxs-lookup"><span data-stu-id="72575-185">Azure reservations</span></span>


<span data-ttu-id="72575-186">Jeśli kupujesz [rezerwacje platformy Azure](azure-reservations.md) za pośrednictwem planu platformy Azure, możesz wybrać rozliczenia godzinowe lub miesięczne.</span><span class="sxs-lookup"><span data-stu-id="72575-186">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="72575-187">Wydatki na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="72575-187">Azure spending</span></span>

<span data-ttu-id="72575-188">Istniejące środowisko wydatków na platformę Azure jest aktualizowane w celu obsługi nowych rozliczeń planu platformy Azure w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="72575-188">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="72575-189">Dzięki temu partnerzy mogą:</span><span class="sxs-lookup"><span data-stu-id="72575-189">This enables partners to:</span></span>

- <span data-ttu-id="72575-190">Wyświetlanie i odbieranie alertów dotyczących budżetu ustawionego na poziomie klienta oraz zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="72575-190">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="72575-191">Wyświetlanie łącznych szacowanych wydatków w ramach planu platformy Azure (podzielone według poziomu zasobu i miernika)</span><span class="sxs-lookup"><span data-stu-id="72575-191">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="72575-192">Ponieważ model rozliczeń dla usług platformy Azure za pośrednictwem planu platformy Azure to użycie po płatności, aby uniknąć większego rachunku, niż oczekiwano, partnerzy mogą zastosować miesięczny budżet i śledzić procent użycia.</span><span class="sxs-lookup"><span data-stu-id="72575-192">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="72575-193">Budżet można zastosować do jednego klienta lub wielu klientów jednocześnie.</span><span class="sxs-lookup"><span data-stu-id="72575-193">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Wydatki na platformie Azure":::

## <a name="next-steps"></a><span data-ttu-id="72575-195">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="72575-195">Next steps</span></span>

- <span data-ttu-id="72575-196">Zobacz, jak są obliczane punkty uzyskane przez partnera.</span><span class="sxs-lookup"><span data-stu-id="72575-196">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="72575-197">Zaloguj się do Partner Center [pulpitu nawigacyjnego i](https://partner.microsoft.com/dashboard/) znajdź dostępny cennik.</span><span class="sxs-lookup"><span data-stu-id="72575-197">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="72575-198">Dowiedz się więcej [o zakupie planu platformy Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="72575-198">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="72575-199">Zobacz cennik nowego doświadczenia handlowego w [programie CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="72575-199">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
