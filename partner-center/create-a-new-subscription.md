---
title: Tworzenie subskrypcji klientów w Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak sprzedawać klientom subskrypcje produktów publikowanych przez firmę Microsoft oraz produktów SaaS publikowanych przez zewnętrznych isvów.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201412"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="a27b1-103">Tworzenie, zawieszanie lub anulowanie subskrypcji klientów</span><span class="sxs-lookup"><span data-stu-id="a27b1-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="a27b1-104">**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="a27b1-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="a27b1-105">**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="a27b1-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="a27b1-106">Po utworzeniu rekordu klienta w katalogu Partner Center można sprzedawać im subskrypcje produktów w katalogu.</span><span class="sxs-lookup"><span data-stu-id="a27b1-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="a27b1-107">Dotyczy to produktów publikowanych przez firmę Microsoft oraz produktów SaaS (Software as a Service) publikowanych przez niezależnych dostawców oprogramowania (ISV) innych firm na [platformie handlowej.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="a27b1-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="a27b1-108">Niektóre oferty są ograniczone do jednej subskrypcji na klienta.</span><span class="sxs-lookup"><span data-stu-id="a27b1-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="a27b1-109">Aby wyświetlić listę ofert ograniczonych, odwiedź stronę Partner Center Cennik i oferty.</span><span class="sxs-lookup"><span data-stu-id="a27b1-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="a27b1-110">Jako partner w programie CSP  możesz kupić oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a27b1-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="a27b1-111">Oznacza to, że  możesz kupić dowolną opartą na licencjach lub mierzoną [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) ofertę **SaaS,** która została Ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp.</span><span class="sxs-lookup"><span data-stu-id="a27b1-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="a27b1-112">Aby kupić inne, komercyjne oferty platformy handlowej od isvs (np. ofert opartych na użyciu obejmujących aplikacje platformy Azure, kontenery lub maszyny wirtualne) lub zarządzać nimi, musisz przejść do witryny [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="a27b1-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="a27b1-113">Wszystkie daty i godziny w Partner Center są podane w standardzie czasu uniwersalnego (UTC).</span><span class="sxs-lookup"><span data-stu-id="a27b1-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="a27b1-114">Może się to różnić nawet o 24 godziny od czasu lokalnego.</span><span class="sxs-lookup"><span data-stu-id="a27b1-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="a27b1-115">Tworzenie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a27b1-115">Create a new subscription</span></span>

1. <span data-ttu-id="a27b1-116">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="a27b1-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a27b1-117">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="a27b1-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a27b1-118">Wybierz **pozycję Dodaj subskrypcję.**</span><span class="sxs-lookup"><span data-stu-id="a27b1-118">Select **Add subscription**.</span></span> <span data-ttu-id="a27b1-119">Na **karcie Usługi online** będą wyświetlane wszystkie dostępne oferty SaaS w witrynie Marketplace.</span><span class="sxs-lookup"><span data-stu-id="a27b1-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="a27b1-120">Aby wyświetlić tylko niektóre typy subskrypcji, należy dokonać wyboru w dostępnych filtrach:</span><span class="sxs-lookup"><span data-stu-id="a27b1-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="a27b1-121">**Wydawca:** wybierz **firmę Microsoft,** aby  wyświetlić tylko oferty firmy Microsoft lub partnera, aby wyświetlić produkty platformy handlowej opublikowane przez isVs.</span><span class="sxs-lookup"><span data-stu-id="a27b1-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="a27b1-122">**Typ rozliczeń:** wybierz typ rozliczeń subskrypcji, których chcesz użyć: **Licencja** lub **Użycie.**</span><span class="sxs-lookup"><span data-stu-id="a27b1-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="a27b1-123">Zobacz [Rozliczenia oparte na licencjach,](license-based-billing.md) aby uzyskać informacje, które pomogą Ci zdecydować, czy jest to miesięczna, czy roczna częstotliwość rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="a27b1-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="a27b1-124">**Kategoria:** wybierz **pozycję Przedsiębiorstwo,** **Małe firmy** lub Wersja **próbna.**</span><span class="sxs-lookup"><span data-stu-id="a27b1-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="a27b1-125">Aby uzyskać informacje na temat subskrypcji w wersji próbnej, zobacz Offer your customers trial of Microsoft products (Oferować [klientom wersje próbne produktów firmy Microsoft).](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="a27b1-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="a27b1-126">Wybierz subskrypcje produktów, które chcesz kupić dla klienta.</span><span class="sxs-lookup"><span data-stu-id="a27b1-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="a27b1-127">Produkty, które widzisz, zależą od typu segmentu klientów (edukacja, administracja rządowa itp.) i zastosowanych filtrów.</span><span class="sxs-lookup"><span data-stu-id="a27b1-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="a27b1-128">Niektóre oferty wyświetlane w witrynie Marketplace nie zawsze mogą być dostępne dla określonego klienta lub określonego partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="a27b1-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="a27b1-129">Może to być spowodowane:</span><span class="sxs-lookup"><span data-stu-id="a27b1-129">This can be because:</span></span>

   - <span data-ttu-id="a27b1-130">Klient ma już subskrypcję tego produktu i może korzystać tylko z jednej</span><span class="sxs-lookup"><span data-stu-id="a27b1-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="a27b1-131">Subskrypcja klienta może zostać wstrzymana (w tym przypadku możesz ponownie aktywować subskrypcję, zamiast kupować nową).</span><span class="sxs-lookup"><span data-stu-id="a27b1-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="a27b1-132">W przypadku ofert SaaS dla isv może być kilka powodów, dla których oferta nie jest dostępna do zakupu: isv may not support the customer's billing country or region; IsV may have chosen not to make the offer available through the CSP program; lub, isv may have made the offer exclusive to only certain CSP partners.or, the ISV may have made the [offer exclusive to](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) only certain CSP partners.</span><span class="sxs-lookup"><span data-stu-id="a27b1-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="a27b1-133">Oferta isv (isv) może również nie być transakcji za pośrednictwem Partner Center (na przykład kontenerów lub niektórych ofert opartych na użyciu).</span><span class="sxs-lookup"><span data-stu-id="a27b1-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="a27b1-134">Dla każdej subskrypcji, którą chcesz dodać, wprowadź liczbę licencji (w razie potrzeby) i wybierz **pozycję Dodaj do koszyka.**</span><span class="sxs-lookup"><span data-stu-id="a27b1-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="a27b1-135">Po zakończeniu dodawania subskrypcji wybierz pozycję **Przejrzyj** i przejrzyj zamówienie.</span><span class="sxs-lookup"><span data-stu-id="a27b1-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="a27b1-136">Po przejrzenia zamówień i przygotowaniu się do zakupu tych subskrypcji wybierz pozycję **Kup**.</span><span class="sxs-lookup"><span data-stu-id="a27b1-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="a27b1-137">Po zakupie subskrypcji dla klienta wystąpią następujące zdarzenia:</span><span class="sxs-lookup"><span data-stu-id="a27b1-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="a27b1-138">Możesz przejrzeć lub edytować subskrypcję, wybierając nazwę subskrypcji na stronie **Subskrypcje tego** klienta.</span><span class="sxs-lookup"><span data-stu-id="a27b1-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="a27b1-139">W tym miejscu możesz wybrać licencje dodatków, jeśli są dostępne, zmienić liczbę licencji lub wstrzymać subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="a27b1-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="a27b1-140">**W przypadku subskrypcji SAAS isv (opartych na licencjach i mierzonych):**</span><span class="sxs-lookup"><span data-stu-id="a27b1-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="a27b1-141">Otrzymasz link do witryny wydawcy isv.</span><span class="sxs-lookup"><span data-stu-id="a27b1-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="a27b1-142">Ten link powinien ułatwić ukończenie wdrażania lub konfigurowania konta subskrypcji klienta.</span><span class="sxs-lookup"><span data-stu-id="a27b1-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="a27b1-143">Ani Ty, ani Klient nie otrzymacie wiadomości e-mail z instrukcjami dotyczącymi ukończenia procesu skonfigurowania/aprowizowania konta dla tego typu subskrypcji isv.</span><span class="sxs-lookup"><span data-stu-id="a27b1-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="a27b1-144">Jeśli Twoja subskrypcja zawiera 30-dniową bezpłatną wersję próbną, bezpłatny okres próbny zostanie zastosowany automatycznie.</span><span class="sxs-lookup"><span data-stu-id="a27b1-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="a27b1-145">Jako partner w programie CSP nie możesz zrezygnować z okresu bezpłatnej wersji próbnej ofert zakupu dla klientów.</span><span class="sxs-lookup"><span data-stu-id="a27b1-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="a27b1-146">Po zakończeniu okresu bezpłatnej wersji próbnej okres subskrypcji rozpocznie się, a subskrypcja zostanie przekształcona w stan płatny.</span><span class="sxs-lookup"><span data-stu-id="a27b1-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="a27b1-147">Subskrypcja zostanie następnie automatycznie odnowiona zgodnie z tym samym harmonogramem.</span><span class="sxs-lookup"><span data-stu-id="a27b1-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="a27b1-148">Aktualizowanie subskrypcji z dodatkami</span><span class="sxs-lookup"><span data-stu-id="a27b1-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="a27b1-149">Aby kupić dodatek, klient musi najpierw mieć aktywną subskrypcję podstawową.</span><span class="sxs-lookup"><span data-stu-id="a27b1-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="a27b1-150">Nie można kupować dodatków za pomocą wykazu.</span><span class="sxs-lookup"><span data-stu-id="a27b1-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="a27b1-151">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="a27b1-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a27b1-152">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="a27b1-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a27b1-153">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="a27b1-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="a27b1-154">Poniżej sekcji **Stan** znajduje się lista dostępnych dodatków dla subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="a27b1-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="a27b1-155">Zaktualizuj liczbę licencji dla każdego wymaganego dodatku.</span><span class="sxs-lookup"><span data-stu-id="a27b1-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="a27b1-156">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="a27b1-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="a27b1-157">Możliwość zakupu dodatków za pośrednictwem usługi Partner Center jest dostępna tylko dla dostawców bezpośrednich i pośrednich.</span><span class="sxs-lookup"><span data-stu-id="a27b1-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="a27b1-158">Tylko kwalifikujące się dodatki są wyświetlane na podstawie podstawowych wymagań i dostępności regionalnej.</span><span class="sxs-lookup"><span data-stu-id="a27b1-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="a27b1-159">Aby uzyskać więcej informacji na temat cen i ofert, zapoznaj się z macierzą ofert odsprzedawcy chmury.</span><span class="sxs-lookup"><span data-stu-id="a27b1-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="a27b1-160">Wstrzymanie subskrypcji podstawowej spowoduje również wstrzymanie wszystkich skojarzonych dodatków.</span><span class="sxs-lookup"><span data-stu-id="a27b1-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="a27b1-161">Daty rozpoczęcia dla dodatków są dopasowywane do podstawowej subskrypcji, a opłaty są obliczane na podstawie daty rozpoczęcia i zakończenia naliczania opłat z opłatami proporcjonalnymi na pierwszej fakturze.</span><span class="sxs-lookup"><span data-stu-id="a27b1-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="a27b1-162">Aby uzyskać dodatkowe informacje, zobacz [Rozliczenia oparte na licencjach.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="a27b1-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="a27b1-163">Wstrzymywanie lub anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a27b1-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="a27b1-164">Partnerzy mogą wstrzymać lub anulować subskrypcję na żądanie klienta lub w przypadku niepłacenia lub oszustwa.</span><span class="sxs-lookup"><span data-stu-id="a27b1-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="a27b1-165">Zawieszenie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a27b1-165">Suspend a subscription</span></span>

<span data-ttu-id="a27b1-166">Jeśli zmienisz stan subskrypcji na Wstrzymano, użytkownicy nie będą mogli logować się ani uzyskać dostępu do usług.</span><span class="sxs-lookup"><span data-stu-id="a27b1-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="a27b1-167">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="a27b1-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a27b1-168">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="a27b1-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a27b1-169">Wybierz subskrypcję, którą chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="a27b1-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="a27b1-170">W sekcji **Stan** wybierz pozycję **Wstrzymano**.</span><span class="sxs-lookup"><span data-stu-id="a27b1-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="a27b1-171">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="a27b1-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="a27b1-172">Wszystkie dane zostaną usunięte, chyba że subskrypcja zostanie ponownie aktywowana w ciągu 90 dni lub 90 dni plus liczba dni między otwarciem konta a pierwszym okresem rozliczeniowym (maksymalnie 120 dni).</span><span class="sxs-lookup"><span data-stu-id="a27b1-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="a27b1-173">Po wstrzymaniu subskrypcji data, która zostanie wyświetlony poniżej przycisku **Wstrzymano,** wskazuje, kiedy subskrypcja automatycznie wygaśnie, jeśli subskrypcja nie zostanie ponownie aktywowana.</span><span class="sxs-lookup"><span data-stu-id="a27b1-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="a27b1-174">Subskrypcje CSP nie mają wygasłego okresu (w jaki działają subskrypcje bezpośrednie w sieci Web), w którym usługi nadal działają, ale subskrypcja nie generuje żadnych opłat rozliczeniowych.</span><span class="sxs-lookup"><span data-stu-id="a27b1-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="a27b1-175">Subskrypcje CSP są aktywne lub wstrzymane (albo całkowicie usunięte).</span><span class="sxs-lookup"><span data-stu-id="a27b1-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="a27b1-176">Anulowanie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a27b1-176">Cancel a subscription</span></span>

<span data-ttu-id="a27b1-177">Subskrypcje SaaS oparte na licencjach można anulować od zewnętrznych wydawców isV w ramach Partner Center [platformy handlowej.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="a27b1-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="a27b1-178">Dopóki anulujesz subskrypcję w okresie anulowania, otrzymasz pełny zwrot kosztów.</span><span class="sxs-lookup"><span data-stu-id="a27b1-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="a27b1-179">W przypadku ofert isv offers billed monthly:</span><span class="sxs-lookup"><span data-stu-id="a27b1-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="a27b1-180">Jeśli anulujesz zamówienie po upływie mniej niż 24 godzin, otrzymasz pełne środków na następnej fakturze.</span><span class="sxs-lookup"><span data-stu-id="a27b1-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="a27b1-181">Jeśli anulujesz subskrypcję po upływie 24 godzin od złożonego zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.</span><span class="sxs-lookup"><span data-stu-id="a27b1-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="a27b1-182">W przypadku ofert rozliczanych rocznie:</span><span class="sxs-lookup"><span data-stu-id="a27b1-182">For offers billed annually:</span></span>

- <span data-ttu-id="a27b1-183">Jeśli anulujesz zamówienie po upływie mniej niż 14 dni, otrzymasz pełne środków na następnej fakturze.</span><span class="sxs-lookup"><span data-stu-id="a27b1-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="a27b1-184">Jeśli anulujesz subskrypcję później niż 14 dni od zamówienia, anulowanie zostanie zaplanowane podczas odnawiania.</span><span class="sxs-lookup"><span data-stu-id="a27b1-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="a27b1-185">Po zakończeniu tych okresów nie będzie już dostępna opcja anulowania subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="a27b1-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="a27b1-186">Oparte na użyciu i mierzone usługi innych firm isv (które na przykład korzystają z maszyn wirtualnych lub kontenerów) nie kwalifikują się do zwrotu.</span><span class="sxs-lookup"><span data-stu-id="a27b1-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="a27b1-187">Usługi oparte na użyciu można anulować.</span><span class="sxs-lookup"><span data-stu-id="a27b1-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="a27b1-188">Ponieważ opłaty są naliczane po użyciu, te usługi nie kwalifikują się do zwrotu.</span><span class="sxs-lookup"><span data-stu-id="a27b1-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="a27b1-189">Aby anulować opartą na licencji subskrypcję SaaS uzyskaną od wydawcy niezależnego dostawcy oprogramowania, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="a27b1-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="a27b1-190">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="a27b1-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a27b1-191">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="a27b1-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a27b1-192">Znajdź subskrypcję, którą chcesz anulować.</span><span class="sxs-lookup"><span data-stu-id="a27b1-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="a27b1-193">W kolumnie **Stan** wybierz pozycję **Anuluj.**</span><span class="sxs-lookup"><span data-stu-id="a27b1-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="a27b1-194">Następnie **prześlij** zmiany.</span><span class="sxs-lookup"><span data-stu-id="a27b1-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="a27b1-195">Jeśli zostanie wyświetlone okno dialogowe, wypełnij odpowiednie szczegóły, a następnie wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="a27b1-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="a27b1-196">Aby potwierdzić anulowanie, wybierz pozycję **Tak, anuluj .**</span><span class="sxs-lookup"><span data-stu-id="a27b1-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="a27b1-197">Możesz również anulować subskrypcję usługi Azure Marketplace przy użyciu interfejsów API.</span><span class="sxs-lookup"><span data-stu-id="a27b1-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="a27b1-198">Aby to zrobić, zobacz [Anulowanie Azure Marketplace subskrypcji.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="a27b1-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="a27b1-199">Wybierz, czy subskrypcja platformy handlowej ma być odnawiana automatycznie</span><span class="sxs-lookup"><span data-stu-id="a27b1-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="a27b1-200">Domyślnie aktywne subskrypcje są ustawione na automatyczne odnawianie po upływie okresu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="a27b1-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="a27b1-201">W [przypadku subskrypcji produktów platformy handlowej](csp-commercial-marketplace-overview.md)możesz opcjonalnie zdecydować, aby nie odnawiać subskrypcji automatycznie.</span><span class="sxs-lookup"><span data-stu-id="a27b1-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="a27b1-202">Aby zatrzymać automatyczne odnawianie aktywnej subskrypcji platformy handlowej:</span><span class="sxs-lookup"><span data-stu-id="a27b1-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="a27b1-203">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="a27b1-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a27b1-204">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="a27b1-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a27b1-205">Wybierz pozycję **Subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="a27b1-205">Select **Subscriptions**.</span></span> <span data-ttu-id="a27b1-206">Zawiera listę wszystkich subskrypcji opartych na licencjach zakupionych dla klienta.</span><span class="sxs-lookup"><span data-stu-id="a27b1-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="a27b1-207">W kolumnie **Subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.</span><span class="sxs-lookup"><span data-stu-id="a27b1-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="a27b1-208">Na stronie szczegółów subskrypcji znajdź sekcję **Stan** i usuń zaznaczenie pola **Automatycznie odnawiaj.**</span><span class="sxs-lookup"><span data-stu-id="a27b1-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="a27b1-209">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="a27b1-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a27b1-210">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="a27b1-210">Next steps</span></span>

- [<span data-ttu-id="a27b1-211">Kupowanie produktów na platformie handlowej dla klientów</span><span class="sxs-lookup"><span data-stu-id="a27b1-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="a27b1-212">Zarządzanie produktami platformy handlowej dla klientów</span><span class="sxs-lookup"><span data-stu-id="a27b1-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="a27b1-213">Omówienie komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="a27b1-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)