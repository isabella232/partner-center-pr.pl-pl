---
title: Migrowanie subskrypcji pakietu Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition zostanie wycofana od 7 kwietnia 2017. Dowiedz się, jak migrować subskrypcje klientów do nowszych wersji pakietu Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/03/2020
ms.locfileid: "92529177"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="cadfc-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions (Migrowanie subskrypcji usługi Office 365 E4 do nowszych wersji usługi Office 365)</span><span class="sxs-lookup"><span data-stu-id="cadfc-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="cadfc-105">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="cadfc-105">**Applies to**</span></span>

-  <span data-ttu-id="cadfc-106">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="cadfc-106">Partner Center</span></span>

<span data-ttu-id="cadfc-107">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="cadfc-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="cadfc-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="cadfc-108">Global admin</span></span>
-   <span data-ttu-id="cadfc-109">Administrator użytkowników</span><span class="sxs-lookup"><span data-stu-id="cadfc-109">User admin</span></span>
-   <span data-ttu-id="cadfc-110">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="cadfc-110">Admin agent</span></span>
-   <span data-ttu-id="cadfc-111">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="cadfc-111">Sales agent</span></span>

<span data-ttu-id="cadfc-112">Plan programu Office 365 Enterprise E4 został wycofany, obowiązuje 7 kwietnia 2017.</span><span class="sxs-lookup"><span data-stu-id="cadfc-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="cadfc-113">Nie można już kupić nowych subskrypcji programu Office 365 E4 po tej dacie, a istniejące subskrypcje E4 nie będą odnawiane automatycznie po ich wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="cadfc-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="cadfc-114">Po zakończeniu subskrypcji E4 zostaną one anulowane.</span><span class="sxs-lookup"><span data-stu-id="cadfc-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="cadfc-115">Aby zapewnić ciągłość dla klientów, należy przejść do klientów z wygasaniem subskrypcji E4 do obsługiwanej opcji jednostki SKU wymienionej poniżej.</span><span class="sxs-lookup"><span data-stu-id="cadfc-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="cadfc-116">Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="cadfc-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="cadfc-117">Pakiety SKU komercyjnego i rządowego programu Office 365 Enterprise E4 zostały wycofane.</span><span class="sxs-lookup"><span data-stu-id="cadfc-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="cadfc-118">Na stronie szczegółów subskrypcji stan subskrypcji E4 został zmieniony na "wygasa w dniu [Date]" z "autonews w dniu [Date]".</span><span class="sxs-lookup"><span data-stu-id="cadfc-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="cadfc-119">W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można odkrywać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false.</span><span class="sxs-lookup"><span data-stu-id="cadfc-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="cadfc-120">Dla subskrypcji E4 zostanie ustawiona wartość autorenew = false w 7 kwietnia 2017.</span><span class="sxs-lookup"><span data-stu-id="cadfc-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="cadfc-121">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="cadfc-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="cadfc-122">Plany wymiany pakietu Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="cadfc-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="cadfc-123">Możesz korzystać z tych samych funkcji z E4 lub korzystać z nowszych funkcji w pakietach Office 365 i Skype dla firm Online.</span><span class="sxs-lookup"><span data-stu-id="cadfc-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="cadfc-124">Szczegóły cennika znajdują się na liście cen i macierzy list oferty w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="cadfc-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="cadfc-125">Bezpieczny produkt Enterprise w wersji E3 lub bezpieczna produktywność w przedsiębiorstwie E5 można zastąpić następującymi opcjami odpowiednio dla pakietu Office 365 Enterprise E3 lub pakietu Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="cadfc-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="cadfc-126">Opcja 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="cadfc-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="cadfc-127">Opcja 2: Office 365 Enterprise E3 + Skype dla firm — PBX</span><span class="sxs-lookup"><span data-stu-id="cadfc-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="cadfc-128">Opcja 3: Office 365 Enterprise E3 + Skype dla firm Plus CAL (cena i funkcjonalność z parzystością)</span><span class="sxs-lookup"><span data-stu-id="cadfc-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="cadfc-129">Opcja 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="cadfc-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="cadfc-130">Cechy</span><span class="sxs-lookup"><span data-stu-id="cadfc-130">Feature</span></span> | <span data-ttu-id="cadfc-131">Opcja 1</span><span class="sxs-lookup"><span data-stu-id="cadfc-131">Option 1</span></span> | <span data-ttu-id="cadfc-132">Opcja 2</span><span class="sxs-lookup"><span data-stu-id="cadfc-132">Option 2</span></span> | <span data-ttu-id="cadfc-133">Opcja 3</span><span class="sxs-lookup"><span data-stu-id="cadfc-133">Option 3</span></span> | <span data-ttu-id="cadfc-134">Opcja 4</span><span class="sxs-lookup"><span data-stu-id="cadfc-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="cadfc-135">Pobrać wszystkie funkcje zawarte w pakiecie Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="cadfc-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="cadfc-136">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-136">Yes</span></span> | <span data-ttu-id="cadfc-137">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-137">Yes</span></span> | <span data-ttu-id="cadfc-138">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-138">Yes</span></span> | <span data-ttu-id="cadfc-139">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-139">No</span></span> |
| <span data-ttu-id="cadfc-140">Numery telefonów zarządzane w pakiecie Office 365?</span><span class="sxs-lookup"><span data-stu-id="cadfc-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="cadfc-141">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-141">Yes</span></span> | <span data-ttu-id="cadfc-142">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-142">Yes</span></span> | <span data-ttu-id="cadfc-143">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-143">No</span></span> | <span data-ttu-id="cadfc-144">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-144">No</span></span> |
| <span data-ttu-id="cadfc-145">Numery telefonów zarządzane zarówno lokalnie, jak i w pakiecie Office 365 (wdrożenie hybrydowe)?</span><span class="sxs-lookup"><span data-stu-id="cadfc-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="cadfc-146">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-146">Yes</span></span> | <span data-ttu-id="cadfc-147">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-147">Yes</span></span> | <span data-ttu-id="cadfc-148">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-148">No</span></span> | <span data-ttu-id="cadfc-149">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-149">No</span></span> |
| <span data-ttu-id="cadfc-150">Czy można dodać plan rozmowy głosowej PSTN?</span><span class="sxs-lookup"><span data-stu-id="cadfc-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="cadfc-151">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-151">Yes</span></span> | <span data-ttu-id="cadfc-152">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-152">Yes</span></span> | <span data-ttu-id="cadfc-153">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-153">No</span></span> | <span data-ttu-id="cadfc-154">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-154">No</span></span> |
| <span data-ttu-id="cadfc-155">Konferencje PSTN?</span><span class="sxs-lookup"><span data-stu-id="cadfc-155">PSTN Conferencing?</span></span> | <span data-ttu-id="cadfc-156">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-156">Yes</span></span> | <span data-ttu-id="cadfc-157">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-157">No</span></span> | <span data-ttu-id="cadfc-158">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-158">No</span></span> | <span data-ttu-id="cadfc-159">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-159">No</span></span> |
| <span data-ttu-id="cadfc-160">Zaawansowane narzędzia do współpracy, analizy i zabezpieczeń?</span><span class="sxs-lookup"><span data-stu-id="cadfc-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="cadfc-161">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-161">Yes</span></span> | <span data-ttu-id="cadfc-162">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-162">No</span></span> | <span data-ttu-id="cadfc-163">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-163">No</span></span> | <span data-ttu-id="cadfc-164">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-164">No</span></span> |
| <span data-ttu-id="cadfc-165">Interaktywne raporty, pulpity nawigacyjne i wizualizacje danych?</span><span class="sxs-lookup"><span data-stu-id="cadfc-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="cadfc-166">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-166">Yes</span></span> | <span data-ttu-id="cadfc-167">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-167">No</span></span> | <span data-ttu-id="cadfc-168">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-168">No</span></span> | <span data-ttu-id="cadfc-169">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-169">No</span></span> | 
| <span data-ttu-id="cadfc-170">Większą kontrolę nad bezpieczeństwem danych i zgodnością z wbudowaną ochroną prywatności, przezroczystością i udoskonalonymi kontrolkami użytkowników?</span><span class="sxs-lookup"><span data-stu-id="cadfc-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="cadfc-171">Tak</span><span class="sxs-lookup"><span data-stu-id="cadfc-171">Yes</span></span> | <span data-ttu-id="cadfc-172">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-172">No</span></span> | <span data-ttu-id="cadfc-173">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-173">No</span></span> | <span data-ttu-id="cadfc-174">Nie</span><span class="sxs-lookup"><span data-stu-id="cadfc-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="cadfc-175">Przejście klientów do nowych planów produktu</span><span class="sxs-lookup"><span data-stu-id="cadfc-175">Transition customers to new product plans</span></span>

<span data-ttu-id="cadfc-176">Firma Microsoft ciągle oferuje swoim partnerom nowe produkty i usługi.</span><span class="sxs-lookup"><span data-stu-id="cadfc-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="cadfc-177">W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub przeprowadzenie migracji swoich subskrypcji z jednostek SKU, które ostatecznie zostaną zamknięte.</span><span class="sxs-lookup"><span data-stu-id="cadfc-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="cadfc-178">Migrowanie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="cadfc-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="cadfc-179">Kup nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="cadfc-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="cadfc-180">Ponowne przypisanie bieżących licencji użytkownika</span><span class="sxs-lookup"><span data-stu-id="cadfc-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="cadfc-181">Anuluj starą subskrypcję</span><span class="sxs-lookup"><span data-stu-id="cadfc-181">Cancel the old subscription</span></span>

<span data-ttu-id="cadfc-182">Wykonaj następujące kroki, aby zmigrować subskrypcję pakietu Office 365 Enterprise E4 klienta do jednej z opcji w powyższej tabeli.</span><span class="sxs-lookup"><span data-stu-id="cadfc-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="cadfc-183">Krok 1 — kupowanie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="cadfc-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="cadfc-184">W menu **Centrum partnerskiego** wybierz pozycję **klienci** , wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-184">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="cadfc-185">Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

   <span data-ttu-id="cadfc-186">Klient powinien mieć teraz zarówno stare, jak i nowe subskrypcje, starszą subskrypcję pakietu Office 365 Enterprise E4 i nową subskrypcję "target", na przykład opcję 1 — pakiet Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="cadfc-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="cadfc-187">Krok 2. przypisanie licencji użytkownika klienta</span><span class="sxs-lookup"><span data-stu-id="cadfc-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="cadfc-188">W menu **Centrum partnerskiego** wybierz pozycję **klienci** , wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-188">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Users and licenses** .</span></span> <span data-ttu-id="cadfc-189">Zostanie otwarta strona użytkownicy i licencje klienta.</span><span class="sxs-lookup"><span data-stu-id="cadfc-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="cadfc-190">Aby ponownie przypisać licencje użytkowników, wybierz użytkownika, który ma zostać przypisana, a następnie wybierz pozycję **Zarządzaj licencjami** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="cadfc-191">Na stronie **Zarządzanie licencjami** wyczyść pole wyboru licencja **Office 365 Enterprise E4** , a następnie wybierz nowy plan usługi dla subskrypcji, do której będzie przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="cadfc-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="cadfc-192">Wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-192">Select **Submit** .</span></span> <span data-ttu-id="cadfc-193">Na stronie potwierdzenia wyświetlane są nowe przypisania licencji.</span><span class="sxs-lookup"><span data-stu-id="cadfc-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="cadfc-194">Kontynuuj te same kroki dla wszystkich innych użytkowników klienta, którzy potrzebują ponownego przypisania licencji.</span><span class="sxs-lookup"><span data-stu-id="cadfc-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="cadfc-195">Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie najwyższego poziomu klienta.</span><span class="sxs-lookup"><span data-stu-id="cadfc-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="cadfc-196">Krok 3. Anulowanie starej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="cadfc-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="cadfc-197">W menu **Centrum partnerskiego** wybierz pozycję **Customers** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-197">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="cadfc-198">Wybierz klienta, który chcesz przenieść, a następnie wybierz subskrypcję, którą chcesz anulować.</span><span class="sxs-lookup"><span data-stu-id="cadfc-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="cadfc-199">Na stronie Szczegóły subskrypcji Ustaw stan subskrypcji na **zawieszone** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-199">In the subscription details page, set the subscription status to **Suspended** .</span></span>

3. <span data-ttu-id="cadfc-200">Wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="cadfc-200">Select **Submit** .</span></span>

<span data-ttu-id="cadfc-201">Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="cadfc-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="cadfc-202">Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach.</span><span class="sxs-lookup"><span data-stu-id="cadfc-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="cadfc-203">Klient nie wiąże się z żadnymi dodatkowymi kosztami dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="cadfc-203">The customer incurs no additional costs for the old subscription.</span></span>



 



