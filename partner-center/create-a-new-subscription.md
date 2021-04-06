---
title: Tworzenie subskrypcji klientów w centrum partnerskim
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak sprzedawać subskrypcje klientom w przypadku produktów opublikowanych przez firmę Microsoft, a także produktów SaaS opublikowanych przez niezależnych dostawców oprogramowania.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502939"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="34fb8-103">Tworzenie, zawieszanie lub anulowanie subskrypcji klientów</span><span class="sxs-lookup"><span data-stu-id="34fb8-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="34fb8-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="34fb8-104">**Applies to**</span></span>

- <span data-ttu-id="34fb8-105">Centrum partnerskie Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="34fb8-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="34fb8-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="34fb8-106">**Appropriate roles**</span></span>

- <span data-ttu-id="34fb8-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="34fb8-107">Admin agent</span></span>
- <span data-ttu-id="34fb8-108">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="34fb8-108">Billing admin</span></span>
- <span data-ttu-id="34fb8-109">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="34fb8-109">Global admin</span></span>
- <span data-ttu-id="34fb8-110">Agent pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="34fb8-110">Helpdesk agent</span></span>
- <span data-ttu-id="34fb8-111">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="34fb8-111">Sales agent</span></span>

<span data-ttu-id="34fb8-112">Po utworzeniu rekordu klienta w centrum partnerskim możesz sprzedawać te subskrypcje do produktów w katalogu.</span><span class="sxs-lookup"><span data-stu-id="34fb8-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="34fb8-113">Obejmuje to produkty opublikowane przez firmę Microsoft i oprogramowanie jako usługa (SaaS) opublikowane przez niezależnych dostawców oprogramowania (ISV) innych firm do [komercyjnej witryny Marketplace](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="34fb8-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="34fb8-114">Niektóre oferty są ograniczone do jednej subskrypcji na klienta.</span><span class="sxs-lookup"><span data-stu-id="34fb8-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="34fb8-115">Aby wyświetlić listę ofert, które są ograniczone, odwiedź stronę ceny i oferty Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="34fb8-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="34fb8-116">Jako partner w programie CSP można zakupić subskrypcje SaaS **oparte na licencjach** lub **naliczanych** od niezależnych dostawców oprogramowania w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="34fb8-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="34fb8-117">Oznacza to, że możesz zakupić dowolną ofertę **opartą na licencji** lub **naliczaną** SaaSą oferowaną przez wydawcę niezależnego dostawcy oprogramowania, w tym [wyłączne oferty](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , do których masz dostęp.</span><span class="sxs-lookup"><span data-stu-id="34fb8-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="34fb8-118">Aby kupić inne, komercyjne oferty rynkowe z niezależnych dostawców oprogramowania (na przykład oferty oparte na użyciu dotyczące aplikacji platformy Azure, kontenerów lub maszyn wirtualnych) i zarządzać nimi, musisz przejść do [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="34fb8-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="34fb8-119">Utwórz nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="34fb8-119">Create a new subscription</span></span>

1. <span data-ttu-id="34fb8-120">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="34fb8-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="34fb8-121">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="34fb8-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="34fb8-122">Wybierz pozycję **Dodaj subskrypcję**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-122">Select **Add subscription**.</span></span> <span data-ttu-id="34fb8-123">Na karcie **usługi online** zostaną wyświetlone wszystkie dostępne oferty SaaS w portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="34fb8-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="34fb8-124">Aby wyświetlić tylko niektóre typy subskrypcji, należy wybrać dostępne filtry:</span><span class="sxs-lookup"><span data-stu-id="34fb8-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="34fb8-125">**Wydawca**: Wybierz **firmę Microsoft** , aby wyświetlić tylko oferty od firmy Microsoft lub **partnera** , aby zobaczyć komercyjne produkty Marketplace opublikowane przez niezależnych dostawców oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="34fb8-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="34fb8-126">**Typ rozliczeń**: Wybierz typ rozliczania subskrypcji, którego chcesz użyć: **licencja** lub **użycie**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="34fb8-127">Informacje, które pomogą w wyborze miesięcznej i rocznej częstotliwości rozliczania, można znaleźć na stronie [rozliczeń opartych na licencji](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="34fb8-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="34fb8-128">**Kategoria**: wybierz pozycję **Enterprise**, **mała firma** lub **wersja próbna**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="34fb8-129">Aby uzyskać informacje na temat subskrypcji wersji próbnej, zobacz artykuł [oferujący klientom wersje próbne produktów firmy Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="34fb8-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="34fb8-130">Wybierz subskrypcje produktu, które chcesz kupić dla klienta.</span><span class="sxs-lookup"><span data-stu-id="34fb8-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="34fb8-131">Widoczne produkty zależą od typu segmentu klienta (edukacja, rząd itp.) oraz filtrów, które zostały zastosowane.</span><span class="sxs-lookup"><span data-stu-id="34fb8-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="34fb8-132">Niektóre oferty prezentowane w portalu Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="34fb8-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="34fb8-133">Może to być spowodowane:</span><span class="sxs-lookup"><span data-stu-id="34fb8-133">This can be because:</span></span>

   - <span data-ttu-id="34fb8-134">Klient ma już subskrypcję tego produktu i jest dozwolony tylko jeden</span><span class="sxs-lookup"><span data-stu-id="34fb8-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="34fb8-135">Subskrypcja klienta mogła zostać zawieszona (w tym przypadku można ponownie aktywować subskrypcję zamiast zakupić nową).</span><span class="sxs-lookup"><span data-stu-id="34fb8-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="34fb8-136">W przypadku ofert SaaS oferowanych przez niezależnych dostawców oprogramowania może istnieć kilka powodów, dla których oferta nie jest dostępna do zakupu: dostawca niezależnego dostawcy oprogramowania może nie obsługiwać kraju lub regionu rozliczeniowego klienta. Dostawca niezależnego dostawcy oprogramowania mógł zrezygnować z udostępnienia oferty za pomocą programu CSP. niezależny dostawca oprogramowania może [również oferować ofertę wyłącznie dla](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) niektórych partnerów CSP.</span><span class="sxs-lookup"><span data-stu-id="34fb8-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="34fb8-137">Oferta niezależnego dostawcy oprogramowania może być również nieobsługiwana w centrum partnerskim (na przykład w przypadku kontenerów lub niektórych ofert opartych na użyciu).</span><span class="sxs-lookup"><span data-stu-id="34fb8-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="34fb8-138">Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby), a następnie wybierz pozycję **Dodaj do koszyka**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="34fb8-139">Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj swoją kolejność.</span><span class="sxs-lookup"><span data-stu-id="34fb8-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="34fb8-140">Po przejrzeniu zamówień i przygotowaniu do zakupu tych subskrypcji wybierz pozycję **Kup**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="34fb8-141">Po zakupieniu subskrypcji dla klienta zostaną wykonane następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="34fb8-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="34fb8-142">Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji ze strony **subskrypcji** tego klienta.</span><span class="sxs-lookup"><span data-stu-id="34fb8-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="34fb8-143">W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="34fb8-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="34fb8-144">**W przypadku subskrypcji niezależnego dostawcy oprogramowania (SaaS):**</span><span class="sxs-lookup"><span data-stu-id="34fb8-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="34fb8-145">Zostanie wyświetlony link do witryny wydawcy niezależnego dostawcy oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="34fb8-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="34fb8-146">Ten link powinien pomóc w zakończeniu konfiguracji wdrożenia lub konta subskrypcji klienta.</span><span class="sxs-lookup"><span data-stu-id="34fb8-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="34fb8-147">Klient nie otrzyma wiadomości e-mail z instrukcjami dotyczącymi ukończenia konfigurowania lub aprowizacji dla tego typu subskrypcji niezależnego dostawcy oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="34fb8-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="34fb8-148">Jeśli subskrypcja obejmuje 30-dniową bezpłatną wersję próbną, zostanie automatycznie zastosowana bezpłatna wersja próbna.</span><span class="sxs-lookup"><span data-stu-id="34fb8-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="34fb8-149">Jako partner w programie CSP nie można zrezygnować z bezpłatnego okresu próbnego w przypadku ofert zakupu dla klientów.</span><span class="sxs-lookup"><span data-stu-id="34fb8-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="34fb8-150">Po zakończeniu okresu bezpłatnej wersji próbnej subskrypcja zostanie rozpoczęta i subskrypcja zostanie przekonwertowana na stan płatny.</span><span class="sxs-lookup"><span data-stu-id="34fb8-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="34fb8-151">Subskrypcja będzie następnie odnawiana ponownie zgodnie z tym samym harmonogramem.</span><span class="sxs-lookup"><span data-stu-id="34fb8-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="34fb8-152">Aktualizowanie subskrypcji z dodatkami</span><span class="sxs-lookup"><span data-stu-id="34fb8-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="34fb8-153">Aby kupić dodatek, klient musi najpierw mieć aktywną subskrypcję podstawową.</span><span class="sxs-lookup"><span data-stu-id="34fb8-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="34fb8-154">Nie można kupować dodatków za pomocą wykazu.</span><span class="sxs-lookup"><span data-stu-id="34fb8-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="34fb8-155">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="34fb8-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="34fb8-156">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="34fb8-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="34fb8-157">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="34fb8-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="34fb8-158">Poniżej sekcji **stan** znajdują się listy dostępnych dodatków dla subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="34fb8-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="34fb8-159">Zaktualizuj liczbę licencji dla każdego wymaganego dodatku.</span><span class="sxs-lookup"><span data-stu-id="34fb8-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="34fb8-160">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="34fb8-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="34fb8-161">Możliwość kupowania dodatków za pośrednictwem Centrum partnerskiego jest dostępna tylko dla dostawców rachunków bezpośrednich i pośrednich.</span><span class="sxs-lookup"><span data-stu-id="34fb8-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="34fb8-162">Tylko kwalifikujące się dodatki są wyświetlane na podstawie podstawowych wymagań i dostępności regionalnej.</span><span class="sxs-lookup"><span data-stu-id="34fb8-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="34fb8-163">Aby uzyskać więcej informacji na temat cen i ofert, zapoznaj się z macierzą oferty odsprzedawcy w chmurze.</span><span class="sxs-lookup"><span data-stu-id="34fb8-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="34fb8-164">Wstrzymanie subskrypcji podstawowej spowoduje również wstrzymanie wszystkich skojarzonych dodatków.</span><span class="sxs-lookup"><span data-stu-id="34fb8-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="34fb8-165">Daty rozpoczęcia dla dodatków są dopasowywane do podstawowej subskrypcji, a opłaty są obliczane na podstawie daty rozpoczęcia i zakończenia naliczania opłat z opłatami proporcjonalnymi na pierwszej fakturze.</span><span class="sxs-lookup"><span data-stu-id="34fb8-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="34fb8-166">Aby uzyskać dodatkowe informacje, zobacz artykuł dotyczący [rozliczeń opartych na licencji](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="34fb8-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="34fb8-167">Wstrzymywanie lub anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="34fb8-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="34fb8-168">Partnerzy mogą wstrzymywać lub anulować subskrypcję, jeśli jest to wymagane przez klienta lub w przypadku braku płatności lub oszustwa.</span><span class="sxs-lookup"><span data-stu-id="34fb8-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="34fb8-169">Zawieszenie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="34fb8-169">Suspend a subscription</span></span>

<span data-ttu-id="34fb8-170">W przypadku zmiany stanu subskrypcji na **zawieszone** użytkownicy nie będą mogli się zalogować ani uzyskiwać dostępu do usług.</span><span class="sxs-lookup"><span data-stu-id="34fb8-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="34fb8-171">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="34fb8-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="34fb8-172">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="34fb8-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="34fb8-173">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="34fb8-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="34fb8-174">W sekcji **Stan** wybierz pozycję **Wstrzymano**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="34fb8-175">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="34fb8-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="34fb8-176">Wszystkie dane zostaną usunięte, chyba że subskrypcja zostanie ponownie aktywowana w ciągu 90 dni lub 90 dni i liczba dni od momentu otwarcia konta oraz pierwszego okresu rozliczeniowego (maksymalnie 120 dni).</span><span class="sxs-lookup"><span data-stu-id="34fb8-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="34fb8-177">W przypadku wstrzymania subskrypcji Data wyświetlana poniżej przycisku **Wstrzymaj** wskazuje, kiedy subskrypcja wygaśnie automatycznie, jeśli nie zostanie ponownie aktywowana.</span><span class="sxs-lookup"><span data-stu-id="34fb8-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="34fb8-178">Anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="34fb8-178">Cancel a subscription</span></span>

<span data-ttu-id="34fb8-179">Subskrypcje SaaS oparte na licencjach można anulować od wydawców niezależnych dostawców oprogramowania w ramach [komercyjnego portalu](csp-commercial-marketplace-overview.md)partnerów.</span><span class="sxs-lookup"><span data-stu-id="34fb8-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="34fb8-180">Po anulowaniu anulowania w okresie anulowania otrzymasz pełny zwrot.</span><span class="sxs-lookup"><span data-stu-id="34fb8-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="34fb8-181">W przypadku niezależnych dostawców oprogramowania oferty są rozliczane miesięcznie:</span><span class="sxs-lookup"><span data-stu-id="34fb8-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="34fb8-182">Jeśli po złożeniu zamówienia zostanie anulowana godzina krótsza niż 24 godziny, otrzymasz pełne środki na następną fakturę.</span><span class="sxs-lookup"><span data-stu-id="34fb8-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="34fb8-183">Jeśli po złożeniu zamówienia zostanie anulowane później niż 24 godziny, anulowanie zostanie zaplanowane na odnowienie.</span><span class="sxs-lookup"><span data-stu-id="34fb8-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="34fb8-184">W przypadku ofert rozliczanych rocznie:</span><span class="sxs-lookup"><span data-stu-id="34fb8-184">For offers billed annually:</span></span>

- <span data-ttu-id="34fb8-185">Jeśli anulujesz subskrypcję poniżej 14 dni, otrzymasz pełne środki na następną fakturę.</span><span class="sxs-lookup"><span data-stu-id="34fb8-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="34fb8-186">Jeśli anulujesz zamówienie później niż 14 dni po jego umieszczeniu, anulowanie zostanie zaplanowane na odnowienie.</span><span class="sxs-lookup"><span data-stu-id="34fb8-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="34fb8-187">Po przekroczeniu tych okresów nie będzie już widoczna opcja anulowania subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="34fb8-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="34fb8-188">W przypadku korzystania z usług niezależnych dostawców oprogramowania (na przykład używanych przez maszyny wirtualne lub kontenery) nie kwalifikują się do powrotu.</span><span class="sxs-lookup"><span data-stu-id="34fb8-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="34fb8-189">Usługi oparte na użyciu mogą być nieobsługiwane jako metoda anulowania.</span><span class="sxs-lookup"><span data-stu-id="34fb8-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="34fb8-190">Ze względu na to, że opłaty są naliczane po użyciu, usługi te nie kwalifikują się do zwrotu pieniędzy.</span><span class="sxs-lookup"><span data-stu-id="34fb8-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="34fb8-191">Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="34fb8-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="34fb8-192">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="34fb8-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="34fb8-193">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="34fb8-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="34fb8-194">Znajdź subskrypcję, którą chcesz anulować.</span><span class="sxs-lookup"><span data-stu-id="34fb8-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="34fb8-195">W kolumnie **stan** wybierz pozycję **Anuluj**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="34fb8-196">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="34fb8-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="34fb8-197">Jeśli zostanie wyświetlone okno dialogowe, Wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="34fb8-198">Aby potwierdzić anulowanie, wybierz pozycję **tak, Anuluj**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="34fb8-199">Możesz również anulować subskrypcję portalu Azure Marketplace przy użyciu interfejsów API.</span><span class="sxs-lookup"><span data-stu-id="34fb8-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="34fb8-200">Aby to zrobić, zobacz sekcję [Anulowanie subskrypcji portalu Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="34fb8-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="34fb8-201">Zdecyduj, czy chcesz automatycznie odnawiać komercyjną subskrypcję portalu Marketplace</span><span class="sxs-lookup"><span data-stu-id="34fb8-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="34fb8-202">Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="34fb8-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="34fb8-203">W przypadku [subskrypcji na komercyjne produkty Marketplace](csp-commercial-marketplace-overview.md)możesz opcjonalnie zrezygnować z automatycznego odnawiania subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="34fb8-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="34fb8-204">Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji komercyjnej witryny Marketplace:</span><span class="sxs-lookup"><span data-stu-id="34fb8-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="34fb8-205">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="34fb8-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="34fb8-206">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="34fb8-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="34fb8-207">Wybierz pozycję **Subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-207">Select **Subscriptions**.</span></span> <span data-ttu-id="34fb8-208">Zawiera listę wszystkich subskrypcji opartych na licencji zakupionych dla klienta.</span><span class="sxs-lookup"><span data-stu-id="34fb8-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="34fb8-209">W kolumnie **subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.</span><span class="sxs-lookup"><span data-stu-id="34fb8-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="34fb8-210">Na stronie Szczegóły subskrypcji Znajdź sekcję **stan** i usuń zaznaczenie pola wyboru **autoodnawianie** .</span><span class="sxs-lookup"><span data-stu-id="34fb8-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="34fb8-211">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="34fb8-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="34fb8-212">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="34fb8-212">Next steps</span></span>

- [<span data-ttu-id="34fb8-213">Kup komercyjne produkty Marketplace dla klientów</span><span class="sxs-lookup"><span data-stu-id="34fb8-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="34fb8-214">Zarządzanie komercyjnymi produktami Marketplace dla klientów</span><span class="sxs-lookup"><span data-stu-id="34fb8-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="34fb8-215">Omówienie komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="34fb8-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)