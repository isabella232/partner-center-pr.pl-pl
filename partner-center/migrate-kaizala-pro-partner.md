---
title: Migrowanie subskrypcji Kaizala Pro na platformę Microsoft 365
description: Dowiedz się, jak migrować subskrypcje usługi Kaizala Pro do Microsoft 365 usługi Office 365. Przeczytaj ten artykuł, aby uzyskać więcej informacji na temat przechodzenia klientów.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146429"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="c5d45-104">Migrowanie autonomicznych subskrypcji usługi Kaizala Pro Microsoft 365 wersji usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="c5d45-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="c5d45-105">**Odpowiednie role:** Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="c5d45-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="c5d45-106">Od 1 lipca 2020 r. firma Microsoft kończy sprzedaż autonomicznej usługi Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="c5d45-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="c5d45-107">Klienci nie będą już mogli kupować nowych subskrypcji usługi Kaizala Pro po tej dacie, a istniejące subskrypcje usługi Kaizala Pro nie będą odnawiane automatycznie po wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="c5d45-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="c5d45-108">Aby zapewnić ciągłość działania klientów, należy przejść klientów z wygasającą autonomiczną subskrypcją usługi Kaizala Pro do obsługiwanej opcji jednostki SKU wymienionej poniżej.</span><span class="sxs-lookup"><span data-stu-id="c5d45-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="c5d45-109">Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w ciągu roku, aby uniknąć jakichkolwiek błędów usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="c5d45-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="c5d45-110">Jeśli używasz interfejsu API (CREST lub Partner Center), możesz wykryć wygasające subskrypcje, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania ustawioną na wartość false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="c5d45-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="c5d45-111">Subskrypcje E4 zostaną ustawione `auto renew=False` na 1 lipca 2020 r.</span><span class="sxs-lookup"><span data-stu-id="c5d45-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="c5d45-112">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="c5d45-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="c5d45-113">Plany zastępcze autonomicznej aplikacji Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="c5d45-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="c5d45-114">Dzięki nowym planom klienci mogą korzystać z nowszej funkcjonalności w Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c5d45-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="c5d45-115">Szczegóły cennika znajdują się w cenniku i macierzy listy ofert w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c5d45-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="c5d45-116">[**Microsoft 365 for Business,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)w tym:</span><span class="sxs-lookup"><span data-stu-id="c5d45-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="c5d45-117">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="c5d45-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="c5d45-118">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="c5d45-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="c5d45-119">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c5d45-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="c5d45-120">[**Microsoft 365 dla frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)w tym:</span><span class="sxs-lookup"><span data-stu-id="c5d45-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="c5d45-121">Microsoft 365 F3 (wcześniej Microsoft 365 F1) i Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="c5d45-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="c5d45-122">[**Microsoft 365 for Enterprise, w**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)tym:</span><span class="sxs-lookup"><span data-stu-id="c5d45-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="c5d45-123">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="c5d45-123">Office 365 E1</span></span>
   - <span data-ttu-id="c5d45-124">Microsoft 365 E3 i Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="c5d45-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="c5d45-125">Microsoft 365 E5 i Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="c5d45-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="c5d45-126">[**Microsoft 365 for Education, w**](https://www.microsoft.com/education/buy-license/microsoft365)tym:</span><span class="sxs-lookup"><span data-stu-id="c5d45-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="c5d45-127">Microsoft 365 A1 i Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="c5d45-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="c5d45-128">Microsoft 365 A3 i Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="c5d45-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="c5d45-129">Microsoft 365 A5 i Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="c5d45-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c5d45-130">Przechodzenie klientów do nowych planów produktów</span><span class="sxs-lookup"><span data-stu-id="c5d45-130">Transition customers to new product plans</span></span>

<span data-ttu-id="c5d45-131">Firma Microsoft stale oferuje naszym partnerom nowe produkty i usługi.</span><span class="sxs-lookup"><span data-stu-id="c5d45-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="c5d45-132">W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub zmigrowanie ich subskrypcji z jednostki SKU, które ostatecznie zostaną zamknięte.</span><span class="sxs-lookup"><span data-stu-id="c5d45-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="c5d45-133">Migrowanie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków:</span><span class="sxs-lookup"><span data-stu-id="c5d45-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="c5d45-134">A.</span><span class="sxs-lookup"><span data-stu-id="c5d45-134">A.</span></span> <span data-ttu-id="c5d45-135">Kupowanie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="c5d45-135">Purchase the new subscription</span></span>

<span data-ttu-id="c5d45-136">B.</span><span class="sxs-lookup"><span data-stu-id="c5d45-136">B.</span></span> <span data-ttu-id="c5d45-137">Ponowne przypisanie bieżących licencji użytkowników</span><span class="sxs-lookup"><span data-stu-id="c5d45-137">Reassign current user licenses</span></span>

<span data-ttu-id="c5d45-138">C.</span><span class="sxs-lookup"><span data-stu-id="c5d45-138">C.</span></span> <span data-ttu-id="c5d45-139">Anulowanie starej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="c5d45-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="c5d45-140">Migrowanie klientów do nowych planów</span><span class="sxs-lookup"><span data-stu-id="c5d45-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="c5d45-141">A.</span><span class="sxs-lookup"><span data-stu-id="c5d45-141">A.</span></span> <span data-ttu-id="c5d45-142">Kupowanie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="c5d45-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="c5d45-143">Aby kupić nową subskrypcję, z menu **Partner Center** wybierz pozycję **Klienci,** wybierz klienta, którego chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="c5d45-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="c5d45-144">Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="c5d45-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="c5d45-145">Klient powinien teraz mieć zarówno starą, jak i nową subskrypcję, starą autonomiczną subskrypcję usługi Kaizala Pro i nową "docelową" subskrypcję, na przykład opcja 1 — Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="c5d45-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="c5d45-146">B.</span><span class="sxs-lookup"><span data-stu-id="c5d45-146">B.</span></span> <span data-ttu-id="c5d45-147">Ponowne przypisanie bieżących licencji użytkowników</span><span class="sxs-lookup"><span data-stu-id="c5d45-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="c5d45-148">Aby ponownie przypisać licencje użytkowników klienta, z menu usługi Partner Center wybierz pozycję **Klienci,** wybierz klienta, który przenosisz, **a** następnie wybierz pozycję Użytkownicy i **licencje.**</span><span class="sxs-lookup"><span data-stu-id="c5d45-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="c5d45-149">Zostanie otwarta strona Użytkownicy i licencje klienta.</span><span class="sxs-lookup"><span data-stu-id="c5d45-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="c5d45-150">Aby ponownie przypisać licencję użytkownika, wybierz użytkownika do ponownego przypisania, a następnie wybierz pozycję **Zarządzaj licencjami.**</span><span class="sxs-lookup"><span data-stu-id="c5d45-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="c5d45-151">Na stronie **Manage licenses (Zarządzanie** licencjami) wyczyść pole wyboru Kaizala Pro Standalone license (Licencja autonomiczna usługi Kaizala Pro) i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący.</span><span class="sxs-lookup"><span data-stu-id="c5d45-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="c5d45-152">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="c5d45-152">Select **Submit**.</span></span> <span data-ttu-id="c5d45-153">Strona potwierdzenia zawiera listę nowych przypisań licencji.</span><span class="sxs-lookup"><span data-stu-id="c5d45-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="c5d45-154">Kontynuuj ten sam proces dla innych użytkowników, którzy potrzebują przypisań licencji.</span><span class="sxs-lookup"><span data-stu-id="c5d45-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="c5d45-155">C.</span><span class="sxs-lookup"><span data-stu-id="c5d45-155">C.</span></span> <span data-ttu-id="c5d45-156">Anulowanie starej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="c5d45-156">Cancel old subscription</span></span>

<span data-ttu-id="c5d45-157">Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie klienta.</span><span class="sxs-lookup"><span data-stu-id="c5d45-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="c5d45-158">Z menu **Partner Center** wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="c5d45-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="c5d45-159">Wybierz klienta, którego subskrypcję anulujesz.</span><span class="sxs-lookup"><span data-stu-id="c5d45-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="c5d45-160">Na stronie szczegółów subskrypcji ustaw dla subskrypcji wartość **Wstrzymano**.</span><span class="sxs-lookup"><span data-stu-id="c5d45-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="c5d45-161">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="c5d45-161">Select **Submit**.</span></span>

<span data-ttu-id="c5d45-162">Stara subskrypcja zostanie wstrzymana, a nowa subskrypcja będzie aktywna.</span><span class="sxs-lookup"><span data-stu-id="c5d45-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="c5d45-163">Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni.</span><span class="sxs-lookup"><span data-stu-id="c5d45-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c5d45-164">Klient nie ponosi żadnych dodatkowych kosztów dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="c5d45-164">The customer incurs no additional costs for the old subscription.</span></span>
