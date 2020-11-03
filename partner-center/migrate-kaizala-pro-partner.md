---
title: Migrowanie subskrypcji usługi kaizala Pro do Microsoft365
description: Dowiedz się, jak migrować subskrypcje usługi kaizala Pro do wersji Microsoft365 lub pakietu Office 365. Przeczytaj ten artykuł, aby uzyskać więcej informacji na temat przechodzenia do klientów.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530519"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="93c92-104">Migrowanie subskrypcji autonomicznych usługi kaizala Pro do wersji Microsoft365 lub pakietu Office 365</span><span class="sxs-lookup"><span data-stu-id="93c92-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="93c92-105">Począwszy od 1 lipca 2020, firma Microsoft kończy sprzedaż usługi autonomicznej usługi kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="93c92-105">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="93c92-106">Klienci nie będą już mogli kupować nowych subskrypcji usługi kaizala Pro po tej dacie, a istniejące subskrypcje usługi kaizala Pro nie będą odnawiane automatycznie po ich wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="93c92-106">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="93c92-107">Aby zapewnić ciągłość dla klientów, należy przejść do klientów z wygaśnienymi subskrypcjami usługi kaizala Pro do obsługiwanej jednostki SKU wymienionej poniżej.</span><span class="sxs-lookup"><span data-stu-id="93c92-107">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="93c92-108">Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="93c92-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="93c92-109">W przypadku korzystania z interfejsu API (z końcówką lub Centrum partnerskiego) można odkrywać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew ustawioną na wartość false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="93c92-109">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="93c92-110">Dla subskrypcji E4 zostanie ustawiona wartość `auto renew=False` 1 lipca 2020.</span><span class="sxs-lookup"><span data-stu-id="93c92-110">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="93c92-111">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="93c92-111">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="93c92-112">Autonomiczne plany zastępcze usługi kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="93c92-112">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="93c92-113">Dzięki nowym planom klienci mogą korzystać z nowszych funkcji i funkcji w Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="93c92-113">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="93c92-114">Szczegóły cennika znajdują się na liście cen i macierzy list oferty w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="93c92-114">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="93c92-115">[**Microsoft 365 dla firm**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), w tym:</span><span class="sxs-lookup"><span data-stu-id="93c92-115">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="93c92-116">Microsoft 365 Business podstawowa</span><span class="sxs-lookup"><span data-stu-id="93c92-116">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="93c92-117">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="93c92-117">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="93c92-118">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="93c92-118">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="93c92-119">[**Microsoft 365 teraźniejszości, w**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)tym:</span><span class="sxs-lookup"><span data-stu-id="93c92-119">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="93c92-120">Microsoft 365 F3 (dawniej Microsoft 365 F1) i Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="93c92-120">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="93c92-121">[**Microsoft 365 dla przedsiębiorstw**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), w tym:</span><span class="sxs-lookup"><span data-stu-id="93c92-121">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="93c92-122">Pakiet Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="93c92-122">Office 365 E1</span></span>
   - <span data-ttu-id="93c92-123">Microsoft 365 E3 i pakiet Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="93c92-123">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="93c92-124">Microsoft 365 E5 i Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="93c92-124">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="93c92-125">[**Microsoft 365 dla edukacji**](https://www.microsoft.com/education/buy-license/microsoft365), w tym:</span><span class="sxs-lookup"><span data-stu-id="93c92-125">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="93c92-126">Microsoft 365 a1 i Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="93c92-126">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="93c92-127">Microsoft 365 A3 i Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="93c92-127">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="93c92-128">Microsoft 365 A5 i Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="93c92-128">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="93c92-129">Przejście klientów do nowych planów produktu</span><span class="sxs-lookup"><span data-stu-id="93c92-129">Transition customers to new product plans</span></span>

<span data-ttu-id="93c92-130">Firma Microsoft ciągle oferuje swoim partnerom nowe produkty i usługi.</span><span class="sxs-lookup"><span data-stu-id="93c92-130">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="93c92-131">W takich przypadkach może być konieczne uaktualnienie klientów do nowych usług lub przeprowadzenie migracji swoich subskrypcji z jednostek SKU, które ostatecznie zostaną zamknięte.</span><span class="sxs-lookup"><span data-stu-id="93c92-131">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="93c92-132">Migrowanie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="93c92-132">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="93c92-133">A.</span><span class="sxs-lookup"><span data-stu-id="93c92-133">A.</span></span> <span data-ttu-id="93c92-134">Kup nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="93c92-134">Purchase the new subscription</span></span>

<span data-ttu-id="93c92-135">B.</span><span class="sxs-lookup"><span data-stu-id="93c92-135">B.</span></span> <span data-ttu-id="93c92-136">Ponowne przypisanie bieżących licencji użytkownika</span><span class="sxs-lookup"><span data-stu-id="93c92-136">Reassign current user licenses</span></span>

<span data-ttu-id="93c92-137">C.</span><span class="sxs-lookup"><span data-stu-id="93c92-137">C.</span></span> <span data-ttu-id="93c92-138">Anuluj starą subskrypcję</span><span class="sxs-lookup"><span data-stu-id="93c92-138">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="93c92-139">Migrowanie klientów do nowych planów</span><span class="sxs-lookup"><span data-stu-id="93c92-139">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="93c92-140">A.</span><span class="sxs-lookup"><span data-stu-id="93c92-140">A.</span></span> <span data-ttu-id="93c92-141">Kup nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="93c92-141">Purchase the new subscription</span></span>

1. <span data-ttu-id="93c92-142">Aby kupić nową subskrypcję, w menu **Centrum partnerskiego** wybierz pozycję **klienci** , wybierz klienta, który chcesz przenieść, a następnie wybierz pozycję **Dodaj subskrypcje** .</span><span class="sxs-lookup"><span data-stu-id="93c92-142">To purchase the new subscription, from the **Partner Center** menu, select **Customers** , select the customer you want to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="93c92-143">Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="93c92-143">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

<span data-ttu-id="93c92-144">Klient powinien mieć teraz zarówno stare, jak i nowe subskrypcje, starszą subskrypcję autonomiczną usługi kaizala Pro i nową subskrypcję "target", na przykład opcję 1-Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="93c92-144">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="93c92-145">B.</span><span class="sxs-lookup"><span data-stu-id="93c92-145">B.</span></span> <span data-ttu-id="93c92-146">Ponowne przypisanie bieżących licencji użytkownika</span><span class="sxs-lookup"><span data-stu-id="93c92-146">Reassign current user licenses</span></span>

1. <span data-ttu-id="93c92-147">Aby ponownie przypisać licencje użytkowników klienta, w menu **Centrum partnerskiego** wybierz pozycję **klienci** , wybierz przenoszony klient, a następnie wybierz pozycję **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="93c92-147">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers** , select the customer you are moving, and then select **Users and licenses** .</span></span> <span data-ttu-id="93c92-148">Zostanie otwarta strona użytkownicy i licencje klienta.</span><span class="sxs-lookup"><span data-stu-id="93c92-148">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="93c92-149">Aby ponownie przypisać licencję użytkownika, wybierz użytkownika, którego chcesz przypisać ponownie, a następnie wybierz pozycję **Zarządzaj licencjami** .</span><span class="sxs-lookup"><span data-stu-id="93c92-149">To reassign user license, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="93c92-150">Na stronie **Zarządzanie licencjami** wyczyść pole wyboru licencja autonomiczna usługi kaizala Pro, a następnie wybierz nowy plan usługi dla subskrypcji, do której jest przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="93c92-150">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="93c92-151">Wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="93c92-151">Select **Submit** .</span></span> <span data-ttu-id="93c92-152">Na stronie potwierdzenia wyświetlane są nowe przypisania licencji.</span><span class="sxs-lookup"><span data-stu-id="93c92-152">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="93c92-153">Kontynuuj ten sam proces dla innych użytkowników, którzy potrzebują przypisań licencji.</span><span class="sxs-lookup"><span data-stu-id="93c92-153">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="93c92-154">C.</span><span class="sxs-lookup"><span data-stu-id="93c92-154">C.</span></span> <span data-ttu-id="93c92-155">Anuluj starą subskrypcję</span><span class="sxs-lookup"><span data-stu-id="93c92-155">Cancel old subscription</span></span>

<span data-ttu-id="93c92-156">Po przeniesieniu licencji użytkownika do nowej usługi możesz bezpiecznie anulować wycofaną subskrypcję na poziomie klienta.</span><span class="sxs-lookup"><span data-stu-id="93c92-156">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="93c92-157">W menu **Centrum partnerskiego** wybierz pozycję **Customers** .</span><span class="sxs-lookup"><span data-stu-id="93c92-157">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="93c92-158">Wybierz klienta, którego subskrypcję chcesz anulować.</span><span class="sxs-lookup"><span data-stu-id="93c92-158">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="93c92-159">Na stronie Szczegóły subskrypcji Ustaw subskrypcję na **zawieszone** .</span><span class="sxs-lookup"><span data-stu-id="93c92-159">In the subscription detail page, set the subscription to **Suspended** .</span></span>

3.  <span data-ttu-id="93c92-160">Wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="93c92-160">Select **Submit** .</span></span>

<span data-ttu-id="93c92-161">Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="93c92-161">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="93c92-162">Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach.</span><span class="sxs-lookup"><span data-stu-id="93c92-162">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="93c92-163">Klient nie wiąże się z żadnymi dodatkowymi kosztami dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="93c92-163">The customer incurs no additional costs for the old subscription.</span></span>
