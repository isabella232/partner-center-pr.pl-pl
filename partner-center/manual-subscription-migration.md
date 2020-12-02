---
title: Migrowanie kwalifikowanych subskrypcji systemu Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przeprowadzić migrację z kwalifikowanych, podstawowych subskrypcji Dynamics 365 do nowej subskrypcji przed wygaśnięciem istniejących subskrypcji.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529281"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="1d6b3-103">Migrowanie usługi Dynamics 365 i planu Customer Engagement Plan z warstwy Podstawowa (zakwalifikowane oferty) do nowszych wersji</span><span class="sxs-lookup"><span data-stu-id="1d6b3-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="1d6b3-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="1d6b3-104">**Applies to**</span></span>

-  <span data-ttu-id="1d6b3-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="1d6b3-105">Partner Center</span></span>

<span data-ttu-id="1d6b3-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="1d6b3-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="1d6b3-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="1d6b3-107">Global admin</span></span>
-   <span data-ttu-id="1d6b3-108">Administrator użytkowników</span><span class="sxs-lookup"><span data-stu-id="1d6b3-108">User admin</span></span>
-   <span data-ttu-id="1d6b3-109">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="1d6b3-109">Admin agent</span></span>
-   <span data-ttu-id="1d6b3-110">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="1d6b3-110">Sales agent</span></span>

<span data-ttu-id="1d6b3-111">Od 1 stycznia 2019 klienci z planem Dynamics 365 for Sales/Customer Engagement z subskrypcji Basic (z ofertami kwalifikowanymi) nie mogą już odnowiać tych starszych ofert; istniejące subskrypcje nie będą odnawiane automatycznie po ich wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="1d6b3-112">Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "wygasa w dniu [Date]" z "autonews w dniu [Date]".</span><span class="sxs-lookup"><span data-stu-id="1d6b3-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="1d6b3-113">Aby zapewnić ciągłość dla klientów, należy przenieść te osoby z wygasanymi subskrypcjami do obsługiwanej opcji, wymienione poniżej.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="1d6b3-114">Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="1d6b3-115">W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można wyszukać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="1d6b3-116">W przypadku tej subskrypcji zostanie ustawiona wartość autorenew = false 1 stycznia 2019.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="1d6b3-117">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="1d6b3-118">Oferty dla systemu Dynamics 365 są wycofywane</span><span class="sxs-lookup"><span data-stu-id="1d6b3-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="1d6b3-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla wykładowców</span><span class="sxs-lookup"><span data-stu-id="1d6b3-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="1d6b3-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Oferta kwalifikowana) dla studentów</span><span class="sxs-lookup"><span data-stu-id="1d6b3-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="1d6b3-122">Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) CRMOL Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-123">Dynamics 365 for Sales Enterprise Edition od wersji SA dla programu CRM Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-124">Dynamics 365 for Sales Enterprise Edition od wersji SA dla programu CRM Basic (kwalifikowana oferta) dla wykładowców</span><span class="sxs-lookup"><span data-stu-id="1d6b3-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="1d6b3-125">Dynamics 365 for Sales Enterprise Edition od wersji SA for CRM Basic (Oferta kwalifikowana) dla studentów</span><span class="sxs-lookup"><span data-stu-id="1d6b3-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="1d6b3-126">Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) z programu SA for CRM Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-127">Dynamics 365 for Sales Enterprise Edition Add-On dla programu CRM Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-128">Dynamics 365 for Sales Enterprise Edition Add-On dla programu CRM Basic (kwalifikowana oferta) dla wykładowców</span><span class="sxs-lookup"><span data-stu-id="1d6b3-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="1d6b3-129">Dynamics 365 for Sales Enterprise Edition Add-On dla programu CRM Basic (Oferta kwalifikowana) dla studentów</span><span class="sxs-lookup"><span data-stu-id="1d6b3-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="1d6b3-130">Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) Add-On dla programu CRM Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-131">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-132">Dynamics 365 Customer Engagement plan Enterprise Edition (cennik dla instytucji rządowych) CRMOL Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-133">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla studentów</span><span class="sxs-lookup"><span data-stu-id="1d6b3-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="1d6b3-134">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla wykładowców</span><span class="sxs-lookup"><span data-stu-id="1d6b3-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="1d6b3-135">Dynamics 365 Customer Engagement plan Enterprise Edition od wersji SA dla programu CRM Basic (Oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-136">Dynamics 365 Customer Engagement plan Enterprise Edition (cennik dla instytucji rządowych) od SA for CRM Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-137">Dynamics 365 Customer Engagement plan Enterprise Edition from SA for CRM Basic (Oferta kwalifikowana) dla studentów</span><span class="sxs-lookup"><span data-stu-id="1d6b3-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="1d6b3-138">Dynamics 365 Customer Engagement plan Enterprise Edition from SA for CRM Basic (Oferta kwalifikowana) dla nauczycieli lub wykładowców</span><span class="sxs-lookup"><span data-stu-id="1d6b3-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="1d6b3-139">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (Oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-140">Dynamics 365 Customer Engagement plan Enterprise Edition (cennik dla instytucji rządowych) Add-On dla programu CRM Basic (Oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-141">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (Oferta kwalifikowana) dla studentów</span><span class="sxs-lookup"><span data-stu-id="1d6b3-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="1d6b3-142">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kwalifikowana oferta) dla wykładowców</span><span class="sxs-lookup"><span data-stu-id="1d6b3-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="1d6b3-143">Plan "Dynamics 365 for Sales/Customer Engagement" z podstawowych (kwalifikowanych ofert) planów zastępczych</span><span class="sxs-lookup"><span data-stu-id="1d6b3-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="1d6b3-144">**Wycofane oferty**</span><span class="sxs-lookup"><span data-stu-id="1d6b3-144">**Retired offers**</span></span>   

- <span data-ttu-id="1d6b3-145">Dynamics 365 for Sales z programu CRM Basic lub CRMOL Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="1d6b3-146">Plan zaangażowania klienta Dynamics 365 z programu CRM Basic lub CRMOL Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="1d6b3-147">**Opcje zamiany**</span><span class="sxs-lookup"><span data-stu-id="1d6b3-147">**Replacement options**</span></span>
- <span data-ttu-id="1d6b3-148">Dynamics 365 for Sales Professional (NOWOŚĆ)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="1d6b3-149">Dynamics 365 for Sales Professional (NOWOŚĆ)</span><span class="sxs-lookup"><span data-stu-id="1d6b3-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="1d6b3-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="1d6b3-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="1d6b3-151">Plan zaangażowania klientów w usłudze Dynamics 365 lub</span><span class="sxs-lookup"><span data-stu-id="1d6b3-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="1d6b3-152">Członkowie zespołu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1d6b3-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="1d6b3-153">Przejście klientów do nowych planów produktu</span><span class="sxs-lookup"><span data-stu-id="1d6b3-153">Transition customers to new product plans</span></span>

<span data-ttu-id="1d6b3-154">Przeniesienie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących kroków w tej kolejności:</span><span class="sxs-lookup"><span data-stu-id="1d6b3-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="1d6b3-155">Kup nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="1d6b3-155">Purchase the new subscription</span></span>
- <span data-ttu-id="1d6b3-156">Ponowne przypisanie bieżących licencji użytkownika</span><span class="sxs-lookup"><span data-stu-id="1d6b3-156">Reassign current user licenses</span></span>
- <span data-ttu-id="1d6b3-157">Anuluj starą subskrypcję</span><span class="sxs-lookup"><span data-stu-id="1d6b3-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="1d6b3-158">Kup nowy plan dla klienta</span><span class="sxs-lookup"><span data-stu-id="1d6b3-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="1d6b3-159">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz klienta, który ma zostać przeniesiony do nowej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="1d6b3-160">Wybierz pozycję **Dodaj subskrypcję**.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-160">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="1d6b3-161">Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="1d6b3-162">Klient będzie miał teraz zarówno starą subskrypcję, jak i nową.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="1d6b3-163">Następnym krokiem jest ponowne przypisanie licencji do użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="1d6b3-164">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="1d6b3-165">Wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-165">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="1d6b3-166">Aby ponownie przypisać licencję do użytkownika, wybierz użytkownika, a następnie wybierz pozycję **Zarządzaj licencjami**.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-166">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="1d6b3-167">Na stronie **Zarządzanie licencjami** Usuń zaznaczenie pola wyboru Dynamics 365 for Sales/Customer Engagement from Basic (kwalifikowana oferta), a następnie wybierz nowy plan usługi dla subskrypcji, do której będzie przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="1d6b3-168">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-168">Select **Submit**.</span></span> <span data-ttu-id="1d6b3-169">Należy to zrobić dla każdego użytkownika, który potrzebuje nowej licencji.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="1d6b3-170">Po przeniesieniu licencji do nowej subskrypcji można anulować starą subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="1d6b3-171">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="1d6b3-172">Na stronie Szczegóły subskrypcji Ustaw starą subskrypcję na **zawieszoną** i wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="1d6b3-173">Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="1d6b3-174">Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="1d6b3-175">Klient nie będzie miał dodatkowych kosztów dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="1d6b3-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



