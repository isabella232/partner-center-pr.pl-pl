---
title: Tworzenie subskrypcji klientów w Partner Center
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak sprzedawać klientom subskrypcje produktów publikowanych przez firmę Microsoft oraz produktów SaaS publikowanych przez zewnętrznych isvs.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148205"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="11c2d-103">Tworzenie, zawieszanie lub anulowanie subskrypcji klientów</span><span class="sxs-lookup"><span data-stu-id="11c2d-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="11c2d-104">**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="11c2d-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="11c2d-105">**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="11c2d-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="11c2d-106">Po utworzeniu rekordu klienta w katalogu Partner Center można sprzedawać im subskrypcje produktów w katalogu.</span><span class="sxs-lookup"><span data-stu-id="11c2d-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="11c2d-107">Dotyczy to produktów publikowanych przez firmę Microsoft oraz produktów SaaS (Software as a Service) publikowanych przez niezależnych dostawców oprogramowania (ISV) innych firm na [platformie handlowej.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="11c2d-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="11c2d-108">Niektóre oferty są ograniczone do jednej subskrypcji na klienta.</span><span class="sxs-lookup"><span data-stu-id="11c2d-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="11c2d-109">Aby wyświetlić listę ofert, które są ograniczone, odwiedź stronę Partner Center Cennik i oferty.</span><span class="sxs-lookup"><span data-stu-id="11c2d-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="11c2d-110">Jako partner w programie CSP  możesz kupować oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11c2d-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="11c2d-111">Oznacza to, że  możesz kupić dowolną ofertę **SaaS** opartą na licencjach lub taryfowej, która została ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp. [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)</span><span class="sxs-lookup"><span data-stu-id="11c2d-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="11c2d-112">Aby kupić lub zarządzać innymi, komercyjnymi ofertami platformy handlowej od isvs (takimi jak oferty oparte na użyciu obejmujące aplikacje platformy Azure, kontenery lub maszyny wirtualne), musisz przejść do witryny [Azure Portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="11c2d-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="11c2d-113">Tworzenie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="11c2d-113">Create a new subscription</span></span>

1. <span data-ttu-id="11c2d-114">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="11c2d-114">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="11c2d-115">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="11c2d-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="11c2d-116">Wybierz **pozycję Dodaj subskrypcję.**</span><span class="sxs-lookup"><span data-stu-id="11c2d-116">Select **Add subscription**.</span></span> <span data-ttu-id="11c2d-117">Na **karcie Usługi online** będą wyświetlane wszystkie dostępne oferty SaaS w witrynie Marketplace.</span><span class="sxs-lookup"><span data-stu-id="11c2d-117">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="11c2d-118">Aby wyświetlić tylko niektóre typy subskrypcji, należy dokonać wyboru w dostępnych filtrach:</span><span class="sxs-lookup"><span data-stu-id="11c2d-118">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="11c2d-119">**Wydawca:** wybierz **firmę Microsoft,** aby  wyświetlić tylko oferty firmy Microsoft lub partnera, aby wyświetlić produkty platformy handlowej opublikowane przez isVs.</span><span class="sxs-lookup"><span data-stu-id="11c2d-119">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="11c2d-120">**Typ rozliczeń:** wybierz typ rozliczeń subskrypcji, których chcesz użyć: **Licencja** lub **Użycie.**</span><span class="sxs-lookup"><span data-stu-id="11c2d-120">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="11c2d-121">Zobacz [Rozliczenia oparte na licencjach,](license-based-billing.md) aby uzyskać informacje, które pomogą Ci wybrać miesięczną i roczną częstotliwość rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="11c2d-121">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="11c2d-122">**Kategoria:** wybierz **enterprise,** **małe firmy** lub wersję **próbną.**</span><span class="sxs-lookup"><span data-stu-id="11c2d-122">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="11c2d-123">Aby uzyskać informacje o subskrypcjach w wersji próbnej, zobacz [Temat Offer your customers trial of Microsoft products (Oferuj klientom wersje próbne produktów firmy Microsoft).](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="11c2d-123">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="11c2d-124">Wybierz subskrypcje produktów, które chcesz kupić dla klienta.</span><span class="sxs-lookup"><span data-stu-id="11c2d-124">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="11c2d-125">Produkty, które widzisz, zależą od typu segmentu klientów (edukacja, administracja rządowa itp.) i zastosowanych filtrów.</span><span class="sxs-lookup"><span data-stu-id="11c2d-125">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="11c2d-126">Niektóre oferty wyświetlane w witrynie Marketplace mogą nie być zawsze dostępne dla określonego klienta lub określonego partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="11c2d-126">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="11c2d-127">Może to być spowodowane:</span><span class="sxs-lookup"><span data-stu-id="11c2d-127">This can be because:</span></span>

   - <span data-ttu-id="11c2d-128">Klient ma już subskrypcję tego produktu i ma tylko jedną z nich</span><span class="sxs-lookup"><span data-stu-id="11c2d-128">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="11c2d-129">Subskrypcja klienta może zostać wstrzymana (w tym przypadku możesz ponownie aktywować subskrypcję, zamiast kupować nową).</span><span class="sxs-lookup"><span data-stu-id="11c2d-129">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="11c2d-130">W przypadku ofert SaaS dla isv może być kilka powodów, dla których oferta nie jest dostępna do zakupu: isv may not support the customer's billing country or region; IsV may have chosen not make the offer available through the CSP program; lub, isv may have made the offer [exclusive to only](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) certain CSP partners.or, the ISV may have made the offer exclusive to only certain CSP partners.</span><span class="sxs-lookup"><span data-stu-id="11c2d-130">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="11c2d-131">Oferta isv (isv) może być również nie do transakcji za pośrednictwem Partner Center (na przykład kontenerów lub niektórych ofert opartych na użyciu).</span><span class="sxs-lookup"><span data-stu-id="11c2d-131">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="11c2d-132">Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby) i wybierz **pozycję Dodaj do koszyka.**</span><span class="sxs-lookup"><span data-stu-id="11c2d-132">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="11c2d-133">Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj zamówienie.</span><span class="sxs-lookup"><span data-stu-id="11c2d-133">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="11c2d-134">Po przejrzenia zamówień i przygotowaniu się do zakupu tych subskrypcji wybierz pozycję **Kup**.</span><span class="sxs-lookup"><span data-stu-id="11c2d-134">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="11c2d-135">Po zakupie subskrypcji dla klienta wystąpią następujące zdarzenia:</span><span class="sxs-lookup"><span data-stu-id="11c2d-135">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="11c2d-136">Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji na stronie **Subskrypcje tego** klienta.</span><span class="sxs-lookup"><span data-stu-id="11c2d-136">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="11c2d-137">W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="11c2d-137">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="11c2d-138">**W przypadku subskrypcji SAAS isv (opartych na licencjach i mierzonych):**</span><span class="sxs-lookup"><span data-stu-id="11c2d-138">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="11c2d-139">Otrzymasz link do witryny wydawcy isv.</span><span class="sxs-lookup"><span data-stu-id="11c2d-139">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="11c2d-140">Ten link powinien pomóc w ukończeniu wdrażania lub konfigurowania konta subskrypcji klienta.</span><span class="sxs-lookup"><span data-stu-id="11c2d-140">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="11c2d-141">Ani Ty, ani Klient nie otrzymacie wiadomości e-mail z instrukcjami dotyczącymi ukończenia procesu skonfigurowania/aprowizowania konta dla tego typu subskrypcji isv).</span><span class="sxs-lookup"><span data-stu-id="11c2d-141">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="11c2d-142">Jeśli Twoja subskrypcja zawiera 30-dniową bezpłatną wersję próbną, bezpłatny okres próbny zostanie zastosowany automatycznie.</span><span class="sxs-lookup"><span data-stu-id="11c2d-142">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="11c2d-143">Jako partner w programie CSP nie możesz zrezygnować z okresu bezpłatnej wersji próbnej ofert zakupu dla klientów.</span><span class="sxs-lookup"><span data-stu-id="11c2d-143">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="11c2d-144">Po zakończeniu okresu bezpłatnej wersji próbnej okres subskrypcji rozpocznie się, a subskrypcja zostanie przekształcona w stan płatny.</span><span class="sxs-lookup"><span data-stu-id="11c2d-144">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="11c2d-145">Subskrypcja zostanie następnie automatycznie odnowiona zgodnie z tym samym harmonogramem.</span><span class="sxs-lookup"><span data-stu-id="11c2d-145">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="11c2d-146">Aktualizowanie subskrypcji z dodatkami</span><span class="sxs-lookup"><span data-stu-id="11c2d-146">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="11c2d-147">Aby kupić dodatek, klient musi najpierw mieć aktywną subskrypcję podstawową.</span><span class="sxs-lookup"><span data-stu-id="11c2d-147">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="11c2d-148">Nie można kupować dodatków za pomocą wykazu.</span><span class="sxs-lookup"><span data-stu-id="11c2d-148">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="11c2d-149">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="11c2d-149">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="11c2d-150">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="11c2d-150">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="11c2d-151">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="11c2d-151">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="11c2d-152">Poniżej sekcji **Stan** znajduje się lista dostępnych dodatków dla subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="11c2d-152">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="11c2d-153">Zaktualizuj liczbę licencji dla każdego wymaganego dodatku.</span><span class="sxs-lookup"><span data-stu-id="11c2d-153">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="11c2d-154">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="11c2d-154">Then **Submit** your changes.</span></span>

<span data-ttu-id="11c2d-155">Możliwość zakupu dodatków za pośrednictwem usługi Partner Center jest dostępna tylko dla dostawców bezpośrednich i pośrednich.</span><span class="sxs-lookup"><span data-stu-id="11c2d-155">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="11c2d-156">Tylko kwalifikujące się dodatki są wyświetlane na podstawie podstawowych wymagań i dostępności regionalnej.</span><span class="sxs-lookup"><span data-stu-id="11c2d-156">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="11c2d-157">Aby uzyskać więcej informacji na temat cen i ofert, zapoznaj się z macierzą ofert odsprzedawcy chmury.</span><span class="sxs-lookup"><span data-stu-id="11c2d-157">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="11c2d-158">Wstrzymanie subskrypcji podstawowej spowoduje również wstrzymanie wszystkich skojarzonych dodatków.</span><span class="sxs-lookup"><span data-stu-id="11c2d-158">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="11c2d-159">Daty rozpoczęcia dla dodatków są dopasowywane do podstawowej subskrypcji, a opłaty są obliczane na podstawie daty rozpoczęcia i zakończenia naliczania opłat z opłatami proporcjonalnymi na pierwszej fakturze.</span><span class="sxs-lookup"><span data-stu-id="11c2d-159">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="11c2d-160">Aby uzyskać dodatkowe informacje, zobacz [Rozliczenia oparte na licencjach.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="11c2d-160">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="11c2d-161">Wstrzymywanie lub anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="11c2d-161">Suspend or cancel a subscription</span></span>

<span data-ttu-id="11c2d-162">Partnerzy mogą wstrzymać lub anulować subskrypcję na żądanie klienta lub w przypadku niepłacenia lub oszustwa.</span><span class="sxs-lookup"><span data-stu-id="11c2d-162">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="11c2d-163">Zawieszenie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="11c2d-163">Suspend a subscription</span></span>

<span data-ttu-id="11c2d-164">Jeśli zmienisz stan subskrypcji na Wstrzymano, użytkownicy nie będą mogli logować się ani uzyskać dostępu do usług.</span><span class="sxs-lookup"><span data-stu-id="11c2d-164">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="11c2d-165">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="11c2d-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="11c2d-166">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="11c2d-166">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="11c2d-167">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="11c2d-167">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="11c2d-168">W sekcji **Stan** wybierz pozycję **Wstrzymano**.</span><span class="sxs-lookup"><span data-stu-id="11c2d-168">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="11c2d-169">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="11c2d-169">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="11c2d-170">Wszystkie dane zostaną usunięte, chyba że subskrypcja zostanie ponownie aktywowana w ciągu 90 dni lub 90 dni plus liczba dni między otwarciem konta a pierwszym okresem rozliczeniowym (maksymalnie 120 dni).</span><span class="sxs-lookup"><span data-stu-id="11c2d-170">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="11c2d-171">Po wstrzymaniu subskrypcji data, która  zostanie wyświetlony poniżej przycisku Wstrzymano, wskazuje, kiedy subskrypcja automatycznie wygaśnie, jeśli subskrypcja nie zostanie ponownie aktywowana.</span><span class="sxs-lookup"><span data-stu-id="11c2d-171">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="11c2d-172">Subskrypcje programu CSP nie mają wygasłego okresu (w jaki działają subskrypcje bezpośrednie w sieci Web), w którym usługi nadal działają, ale subskrypcja nie generuje żadnych opłat rozliczeniowych.</span><span class="sxs-lookup"><span data-stu-id="11c2d-172">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="11c2d-173">Subskrypcje CSP są aktywne lub wstrzymane (albo całkowicie usunięte).</span><span class="sxs-lookup"><span data-stu-id="11c2d-173">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="11c2d-174">Anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="11c2d-174">Cancel a subscription</span></span>

<span data-ttu-id="11c2d-175">Subskrypcje SaaS oparte na licencjach można anulować od zewnętrznych wydawców isV w ramach Partner Center [platformy handlowej.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="11c2d-175">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="11c2d-176">Dopóki anulujesz subskrypcję w okresie anulowania, otrzymasz pełny zwrot kosztów.</span><span class="sxs-lookup"><span data-stu-id="11c2d-176">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="11c2d-177">W przypadku ofert isv offers billed monthly:</span><span class="sxs-lookup"><span data-stu-id="11c2d-177">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="11c2d-178">Jeśli anulujesz zamówienie po upływie mniej niż 24 godzin, otrzymasz pełne środków na następnej fakturze.</span><span class="sxs-lookup"><span data-stu-id="11c2d-178">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="11c2d-179">Jeśli anulujesz subskrypcję po upływie 24 godzin od złożonego zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.</span><span class="sxs-lookup"><span data-stu-id="11c2d-179">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="11c2d-180">W przypadku ofert rozliczanych rocznie:</span><span class="sxs-lookup"><span data-stu-id="11c2d-180">For offers billed annually:</span></span>

- <span data-ttu-id="11c2d-181">Jeśli anulujesz zamówienie po upływie mniej niż 14 dni, otrzymasz pełne środków na następnej fakturze.</span><span class="sxs-lookup"><span data-stu-id="11c2d-181">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="11c2d-182">Jeśli anulujesz subskrypcję później niż 14 dni od zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.</span><span class="sxs-lookup"><span data-stu-id="11c2d-182">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="11c2d-183">Po zakończeniu tych okresów nie będzie już dostępna opcja anulowania subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="11c2d-183">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="11c2d-184">Oparte na użyciu i mierzone usługi innych firm isv (na przykład które używają maszyn wirtualnych lub kontenerów) nie kwalifikują się do zwrotu.</span><span class="sxs-lookup"><span data-stu-id="11c2d-184">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="11c2d-185">Usługi oparte na użyciu można anulować.</span><span class="sxs-lookup"><span data-stu-id="11c2d-185">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="11c2d-186">Ponieważ opłaty są naliczane po użyciu, te usługi nie kwalifikują się do zwrotu kosztów.</span><span class="sxs-lookup"><span data-stu-id="11c2d-186">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="11c2d-187">Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="11c2d-187">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="11c2d-188">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="11c2d-188">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="11c2d-189">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="11c2d-189">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="11c2d-190">Znajdź subskrypcję, którą chcesz anulować.</span><span class="sxs-lookup"><span data-stu-id="11c2d-190">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="11c2d-191">W kolumnie **Stan** wybierz pozycję **Anuluj.**</span><span class="sxs-lookup"><span data-stu-id="11c2d-191">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="11c2d-192">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="11c2d-192">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="11c2d-193">Jeśli zostanie wyświetlone okno dialogowe, wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="11c2d-193">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="11c2d-194">Aby potwierdzić anulowanie, wybierz pozycję **Tak, anuluj .**</span><span class="sxs-lookup"><span data-stu-id="11c2d-194">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="11c2d-195">Możesz również anulować subskrypcję usługi Azure Marketplace przy użyciu interfejsów API.</span><span class="sxs-lookup"><span data-stu-id="11c2d-195">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="11c2d-196">Aby to zrobić, zobacz [Anulowanie Azure Marketplace subskrypcji.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="11c2d-196">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="11c2d-197">Wybierz, czy subskrypcja platformy handlowej ma być odnawiana automatycznie</span><span class="sxs-lookup"><span data-stu-id="11c2d-197">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="11c2d-198">Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="11c2d-198">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="11c2d-199">W [przypadku subskrypcji produktów platformy handlowej](csp-commercial-marketplace-overview.md)możesz opcjonalnie zdecydować, aby nie odnawiać subskrypcji automatycznie.</span><span class="sxs-lookup"><span data-stu-id="11c2d-199">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="11c2d-200">Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji platformy handlowej:</span><span class="sxs-lookup"><span data-stu-id="11c2d-200">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="11c2d-201">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="11c2d-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="11c2d-202">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="11c2d-202">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="11c2d-203">Wybierz pozycję **Subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="11c2d-203">Select **Subscriptions**.</span></span> <span data-ttu-id="11c2d-204">Zawiera listę wszystkich subskrypcji opartych na licencjach zakupionych dla klienta.</span><span class="sxs-lookup"><span data-stu-id="11c2d-204">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="11c2d-205">W kolumnie **Subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.</span><span class="sxs-lookup"><span data-stu-id="11c2d-205">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="11c2d-206">Na stronie szczegółów subskrypcji znajdź sekcję **Stan** i usuń zaznaczenie pola **Automatycznie odnawiaj.**</span><span class="sxs-lookup"><span data-stu-id="11c2d-206">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="11c2d-207">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="11c2d-207">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="11c2d-208">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="11c2d-208">Next steps</span></span>

- [<span data-ttu-id="11c2d-209">Kupowanie produktów na platformie handlowej dla klientów</span><span class="sxs-lookup"><span data-stu-id="11c2d-209">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="11c2d-210">Zarządzanie produktami na platformie handlowej dla klientów</span><span class="sxs-lookup"><span data-stu-id="11c2d-210">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="11c2d-211">Omówienie komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="11c2d-211">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)