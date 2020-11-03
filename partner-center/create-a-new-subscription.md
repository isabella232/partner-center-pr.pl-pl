---
title: Tworzenie subskrypcji klientów w centrum partnerskim
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak sprzedawać subskrypcje klientów do produktów opublikowanych przez firmę Microsoft, a także produktów SaaS opublikowanych przez niezależnych dostawców oprogramowania.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 8c3cfc2a6576029a8fdfb902a7b3889b4ea6c628
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92530009"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="18f35-103">Tworzenie, zawieszanie lub anulowanie subskrypcji klientów</span><span class="sxs-lookup"><span data-stu-id="18f35-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="18f35-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="18f35-104">**Applies to**</span></span>

- <span data-ttu-id="18f35-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="18f35-105">Partner Center</span></span>
- <span data-ttu-id="18f35-106">Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA</span><span class="sxs-lookup"><span data-stu-id="18f35-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="18f35-107">Partnerzy CSP</span><span class="sxs-lookup"><span data-stu-id="18f35-107">CSP partners</span></span>

<span data-ttu-id="18f35-108">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="18f35-108">**Appropriate roles**</span></span>

- <span data-ttu-id="18f35-109">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="18f35-109">Admin agent</span></span>
- <span data-ttu-id="18f35-110">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="18f35-110">Billing admin</span></span>
- <span data-ttu-id="18f35-111">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="18f35-111">Global admin</span></span>
- <span data-ttu-id="18f35-112">Agent pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="18f35-112">Helpdesk agent</span></span>
- <span data-ttu-id="18f35-113">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="18f35-113">Sales agent</span></span>

<span data-ttu-id="18f35-114">Po utworzeniu rekordu klienta w centrum partnerskim możesz sprzedawać te subskrypcje do produktów w katalogu.</span><span class="sxs-lookup"><span data-stu-id="18f35-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="18f35-115">Obejmuje to produkty opublikowane przez firmę Microsoft, a także produkty SaaS (Software as a Service) opublikowane przez niezależnych dostawców oprogramowania (ISV) innych firm do [komercyjnej witryny Marketplace](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="18f35-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="18f35-116">Niektóre oferty są ograniczone do jednej subskrypcji na klienta.</span><span class="sxs-lookup"><span data-stu-id="18f35-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="18f35-117">Aby wyświetlić listę ofert, które są ograniczone, odwiedź stronę ceny i oferty Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="18f35-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="18f35-118">Jako partner w programie CSP można zakupić wyłącznie subskrypcje SaaS **oparte na licencjach** pochodzących od niezależnych dostawców oprogramowania w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="18f35-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="18f35-119">Oznacza to, że możesz zakupić każdą SaaSą z **licencją** , która będzie dostępna dla Ciebie, w tym [wyłączne oferty](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , do których masz dostęp.</span><span class="sxs-lookup"><span data-stu-id="18f35-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="18f35-120">Aby kupić inne, komercyjne oferty rynkowe z niezależnych dostawców oprogramowania ( **na przykład na podstawie użycia** , taryfowych lub opartych na zużyciu obejmujące aplikacje, kontenery i maszyny wirtualne platformy Azure), należy przejść do [portalu zarządzania systemu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="18f35-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based** , metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="18f35-121">Aby uzyskać więcej informacji, zobacz [kupowanie komercyjnych produktów Marketplace](csp-commercial-marketplace-purchase.md).</span><span class="sxs-lookup"><span data-stu-id="18f35-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="18f35-122">Utwórz nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="18f35-122">Create a new subscription</span></span>

1. <span data-ttu-id="18f35-123">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="18f35-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18f35-124">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="18f35-124">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="18f35-125">Wybierz pozycję **Dodaj subskrypcję**.</span><span class="sxs-lookup"><span data-stu-id="18f35-125">Select **Add subscription**.</span></span> <span data-ttu-id="18f35-126">Na karcie **usługi online** zostaną wyświetlone wszystkie dostępne oferty SaaS w portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="18f35-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="18f35-127">Aby wyświetlić tylko niektóre typy subskrypcji, należy wybrać dostępne filtry:</span><span class="sxs-lookup"><span data-stu-id="18f35-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="18f35-128">**Wydawca** : Wybierz **firmę Microsoft** , aby wyświetlić tylko oferty od firmy Microsoft lub **partnera** , aby zobaczyć komercyjne produkty Marketplace opublikowane przez niezależnych dostawców oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="18f35-128">**Publisher** : Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="18f35-129">**Typ rozliczeń** : Wybierz typ rozliczania subskrypcji, którego chcesz użyć: **licencja** lub **użycie**.</span><span class="sxs-lookup"><span data-stu-id="18f35-129">**Billing type** : Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="18f35-130">Informacje, które pomogą w wyborze miesięcznej i rocznej częstotliwości rozliczania, można znaleźć na stronie [rozliczeń opartych na licencji](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="18f35-130">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="18f35-131">**Kategoria** : wybierz pozycję **Enterprise** , **mała firma** lub **wersja próbna**.</span><span class="sxs-lookup"><span data-stu-id="18f35-131">**Category** : Choose **Enterprise** , **Small business** , or **Trial**.</span></span> <span data-ttu-id="18f35-132">Aby uzyskać informacje na temat subskrypcji wersji próbnej, zobacz artykuł [oferujący klientom wersje próbne produktów firmy Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="18f35-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="18f35-133">Wybierz subskrypcje produktu, które chcesz kupić dla klienta.</span><span class="sxs-lookup"><span data-stu-id="18f35-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="18f35-134">Widoczne produkty zależą od typu segmentu klienta (edukacja, rząd itp.) oraz filtrów, które zostały zastosowane.</span><span class="sxs-lookup"><span data-stu-id="18f35-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="18f35-135">Niektóre oferty prezentowane w portalu Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="18f35-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="18f35-136">Może to być spowodowane:</span><span class="sxs-lookup"><span data-stu-id="18f35-136">This can be because:</span></span>

   - <span data-ttu-id="18f35-137">Klient ma już subskrypcję tego produktu i jest dozwolony tylko jeden</span><span class="sxs-lookup"><span data-stu-id="18f35-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="18f35-138">Subskrypcja klienta mogła zostać zawieszona (w tym przypadku można ponownie aktywować subskrypcję zamiast zakupić nową).</span><span class="sxs-lookup"><span data-stu-id="18f35-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="18f35-139">W przypadku ofert SaaS oferowanych przez niezależnych dostawców oprogramowania może istnieć kilka powodów, dla których oferta nie jest dostępna do zakupu: dostawca niezależnego dostawcy oprogramowania może nie obsługiwać kraju lub regionu rozliczeniowego klienta. Dostawca niezależnego dostawcy oprogramowania mógł zrezygnować z udostępnienia oferty za pomocą programu CSP. niezależny dostawca oprogramowania może [również oferować ofertę wyłącznie dla](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) niektórych partnerów CSP.</span><span class="sxs-lookup"><span data-stu-id="18f35-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="18f35-140">Oferta niezależnego dostawcy oprogramowania może być również nieobsługiwana w centrum partnerskim (na przykład w przypadku kontenerów lub niektórych ofert opartych na użyciu).</span><span class="sxs-lookup"><span data-stu-id="18f35-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="18f35-141">Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby), a następnie wybierz pozycję **Dodaj do koszyka**.</span><span class="sxs-lookup"><span data-stu-id="18f35-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="18f35-142">Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj swoją kolejność.</span><span class="sxs-lookup"><span data-stu-id="18f35-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="18f35-143">Po przejrzeniu zamówień i przygotowaniu do zakupu tych subskrypcji wybierz pozycję **Kup**.</span><span class="sxs-lookup"><span data-stu-id="18f35-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="18f35-144">Po zakupieniu subskrypcji dla klienta zostaną wykonane następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="18f35-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="18f35-145">Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji ze strony **subskrypcji** tego klienta.</span><span class="sxs-lookup"><span data-stu-id="18f35-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="18f35-146">W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="18f35-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="18f35-147">**W przypadku subskrypcji niezależnego dostawcy oprogramowania (SaaS):**</span><span class="sxs-lookup"><span data-stu-id="18f35-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="18f35-148">Zostanie wyświetlony link do witryny wydawcy niezależnego dostawcy oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="18f35-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="18f35-149">Ten link powinien pomóc w zakończeniu konfiguracji wdrożenia lub konta subskrypcji klienta.</span><span class="sxs-lookup"><span data-stu-id="18f35-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="18f35-150">Klient nie otrzyma wiadomości e-mail z instrukcjami dotyczącymi ukończenia konfigurowania lub aprowizacji dla tego typu subskrypcji niezależnego dostawcy oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="18f35-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="18f35-151">Jeśli subskrypcja obejmuje 30-dniową bezpłatną wersję próbną, zostanie automatycznie zastosowana bezpłatna wersja próbna.</span><span class="sxs-lookup"><span data-stu-id="18f35-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="18f35-152">Jako partner w programie CSP nie można zrezygnować z bezpłatnego okresu próbnego w przypadku ofert zakupu dla klientów.</span><span class="sxs-lookup"><span data-stu-id="18f35-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="18f35-153">Po zakończeniu okresu bezpłatnej wersji próbnej subskrypcja zostanie rozpoczęta i subskrypcja zostanie przekonwertowana na stan płatny.</span><span class="sxs-lookup"><span data-stu-id="18f35-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="18f35-154">Subskrypcja będzie następnie odnawiana ponownie zgodnie z tym samym harmonogramem.</span><span class="sxs-lookup"><span data-stu-id="18f35-154">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="18f35-155">Aktualizowanie subskrypcji z dodatkami</span><span class="sxs-lookup"><span data-stu-id="18f35-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="18f35-156">Aby kupić dodatek, klient musi mieć aktywną subskrypcję podstawową.</span><span class="sxs-lookup"><span data-stu-id="18f35-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="18f35-157">Nie można kupować dodatków za pomocą wykazu.</span><span class="sxs-lookup"><span data-stu-id="18f35-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="18f35-158">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="18f35-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18f35-159">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="18f35-159">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="18f35-160">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="18f35-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="18f35-161">Poniżej sekcji **stan** znajdują się listy dostępnych dodatków dla subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="18f35-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="18f35-162">Zaktualizuj liczbę licencji dla każdego wymaganego dodatku.</span><span class="sxs-lookup"><span data-stu-id="18f35-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="18f35-163">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="18f35-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="18f35-164">Możliwość kupowania dodatków za pośrednictwem Centrum partnerskiego jest dostępna tylko dla dostawców rachunków bezpośrednich i pośrednich.</span><span class="sxs-lookup"><span data-stu-id="18f35-164">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="18f35-165">Tylko kwalifikujące się dodatki są wyświetlane na podstawie podstawowych wymagań i dostępności regionalnej.</span><span class="sxs-lookup"><span data-stu-id="18f35-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="18f35-166">Aby uzyskać więcej informacji na temat cen i ofert, zapoznaj się z tabelą ofert dla odsprzedawców rozwiązań w chmurze.</span><span class="sxs-lookup"><span data-stu-id="18f35-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="18f35-167">Wstrzymanie subskrypcji podstawowej spowoduje również wstrzymanie wszystkich skojarzonych dodatków.</span><span class="sxs-lookup"><span data-stu-id="18f35-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="18f35-168">Daty rozpoczęcia dla dodatków są dopasowywane do podstawowej subskrypcji, a opłaty są obliczane na podstawie daty rozpoczęcia i zakończenia naliczania opłat z opłatami proporcjonalnymi na pierwszej fakturze.</span><span class="sxs-lookup"><span data-stu-id="18f35-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="18f35-169">Aby uzyskać dodatkowe informacje, zobacz artykuł dotyczący [rozliczeń opartych na licencji](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="18f35-169">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="18f35-170">Wstrzymywanie lub anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="18f35-170">Suspend or cancel a subscription</span></span>

<span data-ttu-id="18f35-171">Partnerzy mogą wstrzymywać lub anulować subskrypcję, jeśli jest to wymagane przez klienta lub w przypadku braku płatności lub oszustwa.</span><span class="sxs-lookup"><span data-stu-id="18f35-171">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="18f35-172">Wstrzymywanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="18f35-172">Suspend a subscription</span></span>

<span data-ttu-id="18f35-173">W przypadku zmiany stanu subskrypcji na **zawieszone** użytkownicy nie będą mogli się zalogować ani uzyskiwać dostępu do usług.</span><span class="sxs-lookup"><span data-stu-id="18f35-173">When you change the status of a subscription to **Suspended** , users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="18f35-174">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="18f35-174">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18f35-175">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="18f35-175">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="18f35-176">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="18f35-176">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="18f35-177">W sekcji **Stan** wybierz pozycję **Wstrzymano**.</span><span class="sxs-lookup"><span data-stu-id="18f35-177">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="18f35-178">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="18f35-178">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="18f35-179">Wszystkie dane zostaną usunięte, chyba że subskrypcja zostanie ponownie aktywowana w ciągu 90 dni lub 90 dni i liczba dni od momentu otwarcia konta oraz pierwszego okresu rozliczeniowego (maksymalnie 120 dni).</span><span class="sxs-lookup"><span data-stu-id="18f35-179">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="18f35-180">W przypadku wstrzymania subskrypcji Data wyświetlana poniżej przycisku **Wstrzymaj** wskazuje, kiedy subskrypcja wygaśnie automatycznie, jeśli nie zostanie ponownie aktywowana.</span><span class="sxs-lookup"><span data-stu-id="18f35-180">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="18f35-181">Anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="18f35-181">Cancel a subscription</span></span>

<span data-ttu-id="18f35-182">Możesz anulować subskrypcje SaaS oparte na licencji od wydawców niezależnych od firmy Microsoft [w centrum](csp-commercial-marketplace-overview.md)partnerskim.</span><span class="sxs-lookup"><span data-stu-id="18f35-182">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="18f35-183">Po anulowaniu anulowania w okresie anulowania otrzymasz pełny zwrot.</span><span class="sxs-lookup"><span data-stu-id="18f35-183">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="18f35-184">W przypadku niezależnych dostawców oprogramowania oferty są rozliczane miesięcznie:</span><span class="sxs-lookup"><span data-stu-id="18f35-184">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="18f35-185">Jeśli po złożeniu zamówienia zostanie anulowana godzina krótsza niż 24 godziny, otrzymasz pełne środki na następną fakturę.</span><span class="sxs-lookup"><span data-stu-id="18f35-185">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="18f35-186">Jeśli po złożeniu zamówienia zostanie anulowane później niż 24 godziny, anulowanie zostanie zaplanowane na odnowienie.</span><span class="sxs-lookup"><span data-stu-id="18f35-186">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="18f35-187">W przypadku ofert rozliczanych rocznie:</span><span class="sxs-lookup"><span data-stu-id="18f35-187">For offers billed annually:</span></span>

- <span data-ttu-id="18f35-188">Jeśli anulujesz subskrypcję poniżej 14 dni, otrzymasz pełne środki na następną fakturę.</span><span class="sxs-lookup"><span data-stu-id="18f35-188">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="18f35-189">Jeśli anulujesz zamówienie później niż 14 dni po jego umieszczeniu, anulowanie zostanie zaplanowane na odnowienie.</span><span class="sxs-lookup"><span data-stu-id="18f35-189">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="18f35-190">Po przekroczeniu tych okresów nie będzie już widoczna opcja anulowania subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="18f35-190">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="18f35-191">W przypadku korzystania z usług niezależnych dostawców oprogramowania (na przykład używanych przez maszyny wirtualne lub kontenery) nie kwalifikują się do powrotu.</span><span class="sxs-lookup"><span data-stu-id="18f35-191">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="18f35-192">Usługi oparte na użyciu mogą być nieobsługiwane jako metoda anulowania.</span><span class="sxs-lookup"><span data-stu-id="18f35-192">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="18f35-193">Ze względu na to, że opłaty są naliczane po użyciu, usługi te nie kwalifikują się do zwrotu pieniędzy.</span><span class="sxs-lookup"><span data-stu-id="18f35-193">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="18f35-194">Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="18f35-194">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="18f35-195">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="18f35-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18f35-196">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="18f35-196">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="18f35-197">Znajdź subskrypcję, którą chcesz anulować.</span><span class="sxs-lookup"><span data-stu-id="18f35-197">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="18f35-198">W kolumnie **stan** wybierz pozycję **Anuluj**.</span><span class="sxs-lookup"><span data-stu-id="18f35-198">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="18f35-199">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="18f35-199">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="18f35-200">Jeśli zostanie wyświetlone okno dialogowe, Wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="18f35-200">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="18f35-201">Aby potwierdzić anulowanie, wybierz pozycję **tak, Anuluj**.</span><span class="sxs-lookup"><span data-stu-id="18f35-201">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="18f35-202">Możesz również anulować subskrypcję portalu Azure Marketplace przy użyciu interfejsów API.</span><span class="sxs-lookup"><span data-stu-id="18f35-202">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="18f35-203">Aby to zrobić, zobacz sekcję [Anulowanie subskrypcji portalu Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="18f35-203">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="18f35-204">Zdecyduj, czy chcesz automatycznie odnawiać komercyjną subskrypcję portalu Marketplace</span><span class="sxs-lookup"><span data-stu-id="18f35-204">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="18f35-205">Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="18f35-205">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="18f35-206">W przypadku [subskrypcji na komercyjne produkty Marketplace](csp-commercial-marketplace-overview.md)możesz opcjonalnie zrezygnować z automatycznego odnawiania subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="18f35-206">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="18f35-207">Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji komercyjnej witryny Marketplace:</span><span class="sxs-lookup"><span data-stu-id="18f35-207">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="18f35-208">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="18f35-208">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="18f35-209">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="18f35-209">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="18f35-210">Wybierz pozycję **Subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="18f35-210">Select **Subscriptions**.</span></span> <span data-ttu-id="18f35-211">Zawiera listę wszystkich subskrypcji opartych na licencji zakupionych dla klienta.</span><span class="sxs-lookup"><span data-stu-id="18f35-211">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="18f35-212">W kolumnie **subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.</span><span class="sxs-lookup"><span data-stu-id="18f35-212">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="18f35-213">Na stronie Szczegóły subskrypcji Znajdź sekcję **stan** i usuń zaznaczenie pola wyboru **autoodnawianie** .</span><span class="sxs-lookup"><span data-stu-id="18f35-213">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="18f35-214">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="18f35-214">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="18f35-215">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="18f35-215">Next steps</span></span>

- [<span data-ttu-id="18f35-216">Kup komercyjne produkty Marketplace dla klientów</span><span class="sxs-lookup"><span data-stu-id="18f35-216">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="18f35-217">Zarządzanie komercyjnymi produktami Marketplace dla klientów</span><span class="sxs-lookup"><span data-stu-id="18f35-217">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="18f35-218">Komercyjne Omówienie portalu Marketplace</span><span class="sxs-lookup"><span data-stu-id="18f35-218">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)