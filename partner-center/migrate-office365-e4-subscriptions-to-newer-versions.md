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
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132625"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="2edd8-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions (Migrowanie subskrypcji usługi Office 365 E4 do nowszych wersji usługi Office 365)</span><span class="sxs-lookup"><span data-stu-id="2edd8-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="2edd8-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="2edd8-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2edd8-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="2edd8-106">Global admin</span></span>
- <span data-ttu-id="2edd8-107">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="2edd8-107">User management admin</span></span>
- <span data-ttu-id="2edd8-108">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="2edd8-108">Admin agent</span></span>
- <span data-ttu-id="2edd8-109">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="2edd8-109">Sales agent</span></span>

<span data-ttu-id="2edd8-110">Plan programu Office 365 Enterprise E4 został wycofany, obowiązuje 7 kwietnia 2017.</span><span class="sxs-lookup"><span data-stu-id="2edd8-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="2edd8-111">Nie można już kupić nowych subskrypcji programu Office 365 E4 po tej dacie, a istniejące subskrypcje E4 nie będą odnawiane automatycznie po ich wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="2edd8-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="2edd8-112">Po zakończeniu subskrypcji E4 zostaną one anulowane.</span><span class="sxs-lookup"><span data-stu-id="2edd8-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="2edd8-113">Aby zapewnić ciągłość dla klientów, należy przejść do klientów z wygasaniem subskrypcji E4 do obsługiwanej opcji jednostki SKU wymienionej poniżej.</span><span class="sxs-lookup"><span data-stu-id="2edd8-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="2edd8-114">Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="2edd8-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="2edd8-115">Pakiety SKU komercyjnego i rządowego programu Office 365 Enterprise E4 zostały wycofane.</span><span class="sxs-lookup"><span data-stu-id="2edd8-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="2edd8-116">Na stronie szczegółów subskrypcji stan subskrypcji E4 został zmieniony na "wygasa w dniu [Date]" z "autonews w dniu [Date]".</span><span class="sxs-lookup"><span data-stu-id="2edd8-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="2edd8-117">W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można odkrywać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false.</span><span class="sxs-lookup"><span data-stu-id="2edd8-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="2edd8-118">Dla subskrypcji E4 zostanie ustawiona wartość autorenew = false w 7 kwietnia 2017.</span><span class="sxs-lookup"><span data-stu-id="2edd8-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="2edd8-119">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="2edd8-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="2edd8-120">Plany wymiany pakietu Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="2edd8-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="2edd8-121">Możesz korzystać z tych samych funkcji z E4 lub korzystać z nowszych funkcji w pakietach Office 365 i Skype dla firm Online.</span><span class="sxs-lookup"><span data-stu-id="2edd8-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="2edd8-122">Szczegóły cennika znajdują się na liście cen i macierzy list oferty w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="2edd8-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="2edd8-123">Bezpieczny produkt Enterprise w wersji E3 lub bezpieczna produktywność w przedsiębiorstwie E5 można zastąpić następującymi opcjami odpowiednio dla pakietu Office 365 Enterprise E3 lub pakietu Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2edd8-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="2edd8-124">Opcja 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="2edd8-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="2edd8-125">Opcja 2: Office 365 Enterprise E3 + Skype dla firm — PBX</span><span class="sxs-lookup"><span data-stu-id="2edd8-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="2edd8-126">Opcja 3: Office 365 Enterprise E3 + Skype dla firm Plus CAL (cena i funkcjonalność z parzystością)</span><span class="sxs-lookup"><span data-stu-id="2edd8-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="2edd8-127">Opcja 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="2edd8-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="2edd8-128">Cecha</span><span class="sxs-lookup"><span data-stu-id="2edd8-128">Feature</span></span> | <span data-ttu-id="2edd8-129">Opcja 1</span><span class="sxs-lookup"><span data-stu-id="2edd8-129">Option 1</span></span> | <span data-ttu-id="2edd8-130">Opcja 2</span><span class="sxs-lookup"><span data-stu-id="2edd8-130">Option 2</span></span> | <span data-ttu-id="2edd8-131">Opcja 3</span><span class="sxs-lookup"><span data-stu-id="2edd8-131">Option 3</span></span> | <span data-ttu-id="2edd8-132">Opcja 4</span><span class="sxs-lookup"><span data-stu-id="2edd8-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="2edd8-133">Pobrać wszystkie funkcje zawarte w pakiecie Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="2edd8-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="2edd8-134">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-134">Yes</span></span> | <span data-ttu-id="2edd8-135">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-135">Yes</span></span> | <span data-ttu-id="2edd8-136">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-136">Yes</span></span> | <span data-ttu-id="2edd8-137">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-137">No</span></span> |
| <span data-ttu-id="2edd8-138">Numery telefonów zarządzane w pakiecie Office 365?</span><span class="sxs-lookup"><span data-stu-id="2edd8-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="2edd8-139">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-139">Yes</span></span> | <span data-ttu-id="2edd8-140">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-140">Yes</span></span> | <span data-ttu-id="2edd8-141">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-141">No</span></span> | <span data-ttu-id="2edd8-142">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-142">No</span></span> |
| <span data-ttu-id="2edd8-143">Numery telefonów zarządzane zarówno lokalnie, jak i w pakiecie Office 365 (wdrożenie hybrydowe)?</span><span class="sxs-lookup"><span data-stu-id="2edd8-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="2edd8-144">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-144">Yes</span></span> | <span data-ttu-id="2edd8-145">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-145">Yes</span></span> | <span data-ttu-id="2edd8-146">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-146">No</span></span> | <span data-ttu-id="2edd8-147">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-147">No</span></span> |
| <span data-ttu-id="2edd8-148">Czy można dodać plan rozmowy głosowej PSTN?</span><span class="sxs-lookup"><span data-stu-id="2edd8-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="2edd8-149">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-149">Yes</span></span> | <span data-ttu-id="2edd8-150">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-150">Yes</span></span> | <span data-ttu-id="2edd8-151">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-151">No</span></span> | <span data-ttu-id="2edd8-152">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-152">No</span></span> |
| <span data-ttu-id="2edd8-153">Konferencje PSTN?</span><span class="sxs-lookup"><span data-stu-id="2edd8-153">PSTN Conferencing?</span></span> | <span data-ttu-id="2edd8-154">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-154">Yes</span></span> | <span data-ttu-id="2edd8-155">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-155">No</span></span> | <span data-ttu-id="2edd8-156">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-156">No</span></span> | <span data-ttu-id="2edd8-157">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-157">No</span></span> |
| <span data-ttu-id="2edd8-158">Zaawansowane narzędzia do współpracy, analizy i zabezpieczeń?</span><span class="sxs-lookup"><span data-stu-id="2edd8-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="2edd8-159">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-159">Yes</span></span> | <span data-ttu-id="2edd8-160">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-160">No</span></span> | <span data-ttu-id="2edd8-161">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-161">No</span></span> | <span data-ttu-id="2edd8-162">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-162">No</span></span> |
| <span data-ttu-id="2edd8-163">Interaktywne raporty, pulpity nawigacyjne i wizualizacje danych?</span><span class="sxs-lookup"><span data-stu-id="2edd8-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="2edd8-164">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-164">Yes</span></span> | <span data-ttu-id="2edd8-165">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-165">No</span></span> | <span data-ttu-id="2edd8-166">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-166">No</span></span> | <span data-ttu-id="2edd8-167">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-167">No</span></span> | 
| <span data-ttu-id="2edd8-168">Większą kontrolę nad bezpieczeństwem danych i zgodnością z wbudowaną ochroną prywatności, przezroczystością i udoskonalonymi kontrolkami użytkowników?</span><span class="sxs-lookup"><span data-stu-id="2edd8-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="2edd8-169">Tak</span><span class="sxs-lookup"><span data-stu-id="2edd8-169">Yes</span></span> | <span data-ttu-id="2edd8-170">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-170">No</span></span> | <span data-ttu-id="2edd8-171">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-171">No</span></span> | <span data-ttu-id="2edd8-172">Nie</span><span class="sxs-lookup"><span data-stu-id="2edd8-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2edd8-173">Przejście klientów do nowych planów produktu</span><span class="sxs-lookup"><span data-stu-id="2edd8-173">Transition customers to new product plans</span></span>

<span data-ttu-id="2edd8-174">Firma Microsoft ciągle oferuje swoim partnerom nowe produkty i usługi.</span><span class="sxs-lookup"><span data-stu-id="2edd8-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="2edd8-175">W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub przeprowadzenie migracji swoich subskrypcji z jednostek SKU, które ostatecznie zostaną zamknięte.</span><span class="sxs-lookup"><span data-stu-id="2edd8-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="2edd8-176">Migrowanie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="2edd8-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="2edd8-177">Kup nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="2edd8-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="2edd8-178">Ponowne przypisanie bieżących licencji użytkownika</span><span class="sxs-lookup"><span data-stu-id="2edd8-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="2edd8-179">Anuluj starą subskrypcję</span><span class="sxs-lookup"><span data-stu-id="2edd8-179">Cancel the old subscription</span></span>

<span data-ttu-id="2edd8-180">Wykonaj następujące kroki, aby zmigrować subskrypcję pakietu Office 365 Enterprise E4 klienta do jednej z opcji w powyższej tabeli.</span><span class="sxs-lookup"><span data-stu-id="2edd8-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="2edd8-181">Krok 1 — kupowanie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="2edd8-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="2edd8-182">W menu **Centrum partnerskiego** wybierz pozycję **klienci**, wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="2edd8-183">Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="2edd8-184">Klient powinien mieć teraz zarówno stare, jak i nowe subskrypcje, starszą subskrypcję pakietu Office 365 Enterprise E4 i nową subskrypcję "target", na przykład opcję 1 — pakiet Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2edd8-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="2edd8-185">Krok 2. przypisanie licencji użytkownika klienta</span><span class="sxs-lookup"><span data-stu-id="2edd8-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="2edd8-186">W menu **Centrum partnerskiego** wybierz pozycję **klienci**, wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="2edd8-187">Zostanie otwarta strona użytkownicy i licencje klienta.</span><span class="sxs-lookup"><span data-stu-id="2edd8-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="2edd8-188">Aby ponownie przypisać licencje użytkownika, wybierz użytkownika, którego chcesz przypisać ponownie, a następnie wybierz pozycję **Zarządzaj licencjami**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="2edd8-189">Na stronie **Zarządzanie licencjami** wyczyść pole wyboru licencja **Office 365 Enterprise E4** , a następnie wybierz nowy plan usługi dla subskrypcji, do której będzie przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="2edd8-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="2edd8-190">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-190">Select **Submit**.</span></span> <span data-ttu-id="2edd8-191">Na stronie potwierdzenia wyświetlane są nowe przypisania licencji.</span><span class="sxs-lookup"><span data-stu-id="2edd8-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="2edd8-192">Kontynuuj te same kroki dla wszystkich innych użytkowników klienta, którzy potrzebują ponownego przypisania licencji.</span><span class="sxs-lookup"><span data-stu-id="2edd8-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="2edd8-193">Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie najwyższego poziomu klienta.</span><span class="sxs-lookup"><span data-stu-id="2edd8-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="2edd8-194">Krok 3. Anulowanie starej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="2edd8-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="2edd8-195">W menu **Centrum partnerskiego** wybierz pozycję **Customers**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2edd8-196">Wybierz klienta, który chcesz przenieść, a następnie wybierz subskrypcję, którą chcesz anulować.</span><span class="sxs-lookup"><span data-stu-id="2edd8-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="2edd8-197">Na stronie Szczegóły subskrypcji Ustaw stan subskrypcji na **zawieszone**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="2edd8-198">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="2edd8-198">Select **Submit**.</span></span>

<span data-ttu-id="2edd8-199">Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="2edd8-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="2edd8-200">Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach.</span><span class="sxs-lookup"><span data-stu-id="2edd8-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2edd8-201">Klient nie wiąże się z żadnymi dodatkowymi kosztami dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="2edd8-201">The customer incurs no additional costs for the old subscription.</span></span>



 



