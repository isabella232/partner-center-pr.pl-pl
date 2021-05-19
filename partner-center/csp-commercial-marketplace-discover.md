---
title: Odnajdywanie ofert — komercyjna platforma handlowa
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak partnerzy programu CSP mogą Partner Center do wyświetlania lub wyszukiwania na platformie handlowej ofert SaaS lub cen od niezależnych dostawców oprogramowania.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147976"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="55708-103">Odnajdywanie ofert i cen na platformie Partner Center platformie handlowej</span><span class="sxs-lookup"><span data-stu-id="55708-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="55708-104">**Odpowiednie role:** Administrator globalny | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="55708-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="55708-105">Gdy niezależni dostawcy oprogramowania (ISV) zdecydują się opublikować ofertę na platformie handlowej, mogą również zdecydować, czy mają być udostępniane w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="55708-105">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="55708-106">Jeśli zdecyduje się sprzedawać ofertę za pośrednictwem programu CSP, partnerzy programu CSP powinni zobaczyć tę ofertę w Partner Center Marketplace.</span><span class="sxs-lookup"><span data-stu-id="55708-106">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="55708-107">Jeśli oferta isV nie jest wyświetlana zgodnie z oczekiwaniami w Partner Center, może to być spowodowane:</span><span class="sxs-lookup"><span data-stu-id="55708-107">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="55708-108">IsV decided not to sell the offer through the CSP program.</span><span class="sxs-lookup"><span data-stu-id="55708-108">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="55708-109">Na przykład niektóre produkty isv mogą zostać udostępnione w innych obszarach platformy handlowej (np. w usługach [Microsoft AppSource](https://appsource.microsoft.com/) i [Azure Marketplace),](https://azuremarketplace.microsoft.com/)ale mogą nie być widoczne dla partnerów w programie CSP na platformie Partner Center Marketplace.</span><span class="sxs-lookup"><span data-stu-id="55708-109">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="55708-110">IsV decided to make the offer exclusive to only a select number of CSP partners.</span><span class="sxs-lookup"><span data-stu-id="55708-110">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="55708-111">Aby uzyskać więcej informacji na temat ofert na wyłączność, zobacz w dalszej części tego tematu pomocy.</span><span class="sxs-lookup"><span data-stu-id="55708-111">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="55708-112">Nie można transakcjiować typu oferty za pośrednictwem Partner Center lub Azure Portal (np. kontenerów lub niektórych ofert opartych na użyciu).</span><span class="sxs-lookup"><span data-stu-id="55708-112">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="55708-113">Kraj rozliczeniowy skojarzonych klientów może nie być obsługiwany dla tej oferty isv.</span><span class="sxs-lookup"><span data-stu-id="55708-113">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="55708-114">Wyświetlanie ofert w witrynie Marketplace w Partner Center</span><span class="sxs-lookup"><span data-stu-id="55708-114">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="55708-115">Aby wyświetlić dostępne oferty platformy handlowej w programie CSP:</span><span class="sxs-lookup"><span data-stu-id="55708-115">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="55708-116">Zaloguj się Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **CSP** z menu nawigacji po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="55708-116">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="55708-117">Wybierz **pozycję Sell (Sprzedawaj),** a następnie **pozycję Marketplace ( Marketplace).**</span><span class="sxs-lookup"><span data-stu-id="55708-117">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="55708-118">Domyślnie zobaczysz produkty wszystkich typów i kategorii.</span><span class="sxs-lookup"><span data-stu-id="55708-118">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="55708-119">Wybierz filtr według typu lub kategorii.</span><span class="sxs-lookup"><span data-stu-id="55708-119">Select a filter by type or category.</span></span> <span data-ttu-id="55708-120">Możesz również użyć funkcji **wyszukiwania,** aby znaleźć określone słowa kluczowe, nazwy ofert lub nazwy wydawców ISV.</span><span class="sxs-lookup"><span data-stu-id="55708-120">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="55708-121">Wybierz z listy określoną ofertę produktu.</span><span class="sxs-lookup"><span data-stu-id="55708-121">Select a specific product offer from the list.</span></span> <span data-ttu-id="55708-122">Spowoduje to przejść do karty Przegląd produktu, na której można dowiedzieć się więcej o ofercie.</span><span class="sxs-lookup"><span data-stu-id="55708-122">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="55708-123">Informacje na tej karcie mogą obejmować:</span><span class="sxs-lookup"><span data-stu-id="55708-123">Information on this tab might include:</span></span> 

    - <span data-ttu-id="55708-124">Opis produktu lub oferty</span><span class="sxs-lookup"><span data-stu-id="55708-124">A description of the product or offer</span></span>

    - <span data-ttu-id="55708-125">Więcej informacji na temat wydawcy isv</span><span class="sxs-lookup"><span data-stu-id="55708-125">More information about the ISV publisher</span></span>

    - <span data-ttu-id="55708-126">Linki do dokumentacji lub materiałów marketingowych przekazanych przez wydawcę ISV</span><span class="sxs-lookup"><span data-stu-id="55708-126">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="55708-127">Inne możliwe kontakty isv w zakresie obsługi klienta, inżynierii lub kontaktu dla programu CSP</span><span class="sxs-lookup"><span data-stu-id="55708-127">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="55708-128">Aby wyświetlić więcej informacji o dostępnych planach, jednostkach SKU lub cenach oferty, wybierz **kartę Plany i** cennik. Na tej karcie są wyświetlane:</span><span class="sxs-lookup"><span data-stu-id="55708-128">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="55708-129">Rynki, na których ta oferta jest dla Ciebie dostępna</span><span class="sxs-lookup"><span data-stu-id="55708-129">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="55708-130">Lista dostępnych dla oferty jednostki SKU lub planów</span><span class="sxs-lookup"><span data-stu-id="55708-130">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="55708-131">Cennik każdej dostępnej wersji SKU lub planu</span><span class="sxs-lookup"><span data-stu-id="55708-131">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="55708-132">Wyświetlanie ofert w witrynie Marketplace za pośrednictwem Partner Center API</span><span class="sxs-lookup"><span data-stu-id="55708-132">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="55708-133">Partnerzy programu CSP mogą również używać interfejsów API do zwracania listy kwalifikujących się ofert.</span><span class="sxs-lookup"><span data-stu-id="55708-133">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="55708-134">Kwalifikujące się oferty będą dotyczyć tylko ofert dostawcy ISV SaaS dostępnych dla partnera do sprzedaży za pośrednictwem Partner Center marketplace.</span><span class="sxs-lookup"><span data-stu-id="55708-134">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="55708-135">W przypadku partnerów korzystających z interfejsów API do identyfikowania ofert w katalogu zapoznaj się ze wskazówkami, aby uzyskać listę ofert [dla rynku.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)</span><span class="sxs-lookup"><span data-stu-id="55708-135">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="55708-136">Zobacz najnowsze ceny ofert witryny Marketplace w Partner Center</span><span class="sxs-lookup"><span data-stu-id="55708-136">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="55708-137">Wykonaj następujące kroki, aby uzyskać najnowsze szczegóły cennika skojarzone z ofertą:</span><span class="sxs-lookup"><span data-stu-id="55708-137">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="55708-138">Zaloguj się do Partner Center [nawigacyjnego,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **CSP** z menu nawigacji po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="55708-138">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="55708-139">Wybierz **pozycję Sell**(Sprzedawaj), a następnie pozycję Pricing and offers **(Ceny i oferty).**</span><span class="sxs-lookup"><span data-stu-id="55708-139">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="55708-140">Przewiń w dół do **sekcji Marketplace,** wybierz lokalizację i pobierz cennik **witryny Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="55708-140">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="55708-141">W ten sposób zostanie wygenerowany arkusz kalkulacyjny z najnowszymi danymi cennika usług SaaS, ofert opartych na licencjach i ofert mierzonych dostępnych od wydawców ISV.</span><span class="sxs-lookup"><span data-stu-id="55708-141">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="55708-142">Niektóre cenniki aplikacji platformy Azure mogą być również wyświetlane tutaj.</span><span class="sxs-lookup"><span data-stu-id="55708-142">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="55708-143">Te informacje są aktualizowane codziennie, więc możesz sprawdzać bieżące ceny tak często, jak chcesz.</span><span class="sxs-lookup"><span data-stu-id="55708-143">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="55708-144">Jeśli produkt isv zawiera bezpłatny okres próbny, arkusz kalkulacyjny wyświetli dwa wiersze dla tego produktu:</span><span class="sxs-lookup"><span data-stu-id="55708-144">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="55708-145">Jeden wiersz zawiera cenę bezpłatnej wersji próbnej o wartości zero.</span><span class="sxs-lookup"><span data-stu-id="55708-145">One row shows the free trial price of zero.</span></span> <span data-ttu-id="55708-146">Oznacza to, że dostępny jest bezpłatny okres próbny.</span><span class="sxs-lookup"><span data-stu-id="55708-146">This means a free trial period is available.</span></span>

    - <span data-ttu-id="55708-147">W drugim wierszu przedstawiono cenę i warunki, które będą stosowane po zakończeniu bezpłatnego okresu próbnego.</span><span class="sxs-lookup"><span data-stu-id="55708-147">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="55708-148">Jako partner programu CSP możesz kwalifikować się do innych zachęt skojarzonych z niektórymi ofertami platformy handlowej.</span><span class="sxs-lookup"><span data-stu-id="55708-148">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="55708-149">Aby uzyskać więcej informacji na temat innych zachęt, zobacz przewodnik zachęt [CSP](https://aka.ms/partnerincentives) (wymaga logowania WSP).</span><span class="sxs-lookup"><span data-stu-id="55708-149">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="55708-150">Dowiedz się więcej o ofertach na wyłączność na platformie handlowej</span><span class="sxs-lookup"><span data-stu-id="55708-150">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="55708-151">IsVs have the option to make their offers available only to specific partners in the CSP program.</span><span class="sxs-lookup"><span data-stu-id="55708-151">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="55708-152">Ta oferta jest znana jako oferta wyłączna.</span><span class="sxs-lookup"><span data-stu-id="55708-152">This is known as an Exclusive offer.</span></span> <span data-ttu-id="55708-153">Wszyscy partnerzy w programie CSP mogą nadal wyświetlać wszystkie oferty isv na platformie handlowej Partner Center, w tym oferty oznaczone jako wyłącznie.</span><span class="sxs-lookup"><span data-stu-id="55708-153">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="55708-154">Jeśli oferta nie **jest** oznaczona jako Wyłączna, wszyscy partnerzy mogą ją zakupić (przy założeniu, że kraj rozliczeniowy wybranego klienta odpowiada dostępności oferty isv w danym kraju).</span><span class="sxs-lookup"><span data-stu-id="55708-154">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="55708-155">Jednak w przypadku każdej oferty oznaczonej jako Wyłączna tylko partnerzy wybrani przez isv będą mogli kupić tę ofertę.</span><span class="sxs-lookup"><span data-stu-id="55708-155">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="55708-156">Jeśli widzisz ofertę oznaczoną jako Wyłączna, która ma być sprzedawana klientom, sproś się bezpośrednio do isv i poproś o zgodę na sprzedaż oferty exclusive.</span><span class="sxs-lookup"><span data-stu-id="55708-156">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="55708-157">Po wyświetleniu szczegółów oferty na wyłączność może zostać wyświetlony link Skontaktuj się z **isv,** który możesz wybrać.</span><span class="sxs-lookup"><span data-stu-id="55708-157">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="55708-158">Aby dowiedzieć się więcej na temat obsługi usługodawców internetowych na platformie handlowej, przeczytaj [temat Cloud Solution Providers (Dostawcy rozwiązań w chmurze).](/azure/marketplace/cloud-solution-providers)</span><span class="sxs-lookup"><span data-stu-id="55708-158">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="55708-159">Aby uzyskać więcej informacji na temat obsługi CSP na platformie handlowej, przeczytaj [omówienie komercyjnej platformy handlowej.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="55708-159">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="55708-160">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="55708-160">Next steps</span></span>

- [<span data-ttu-id="55708-161">Kupowanie ofert komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="55708-161">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)