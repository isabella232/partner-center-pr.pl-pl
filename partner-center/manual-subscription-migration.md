---
title: Migrowanie kwalifikowanych subskrypcji usługi Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przeprowadzić migrację z kwalifikowanych, podstawowych subskrypcji usługi Dynamics 365 do nowej subskrypcji przed wygaśnięciem istniejących subskrypcji.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151648"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="ad0cb-103">Migrowanie usługi Dynamics 365 i planu Customer Engagement Plan z warstwy Podstawowa (zakwalifikowane oferty) do nowszych wersji</span><span class="sxs-lookup"><span data-stu-id="ad0cb-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="ad0cb-104">**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="ad0cb-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="ad0cb-105">Od 1 stycznia 2019 r. klienci z subskrypcjami usługi Dynamics 365 for Sales/Customer Engagement z subskrypcji Podstawowa (kwalifikowane oferty) nie mogą już odnawiać tych starszych ofert. Istniejące subskrypcje nie będą odnawiane automatycznie po wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="ad0cb-106">Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "Wygasa [data]" z "Automatyczne odnowienie [data]".</span><span class="sxs-lookup"><span data-stu-id="ad0cb-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="ad0cb-107">Aby zapewnić ciągłość działania klientów, należy przejść te z wygasających subskrypcji do obsługiwanej opcji wymienionej poniżej.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="ad0cb-108">Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w roku, aby uniknąć jakichkolwiek błędów w usłudze dla klientów.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ad0cb-109">Jeśli używasz interfejsu API (CREST lub Partner Center), wygasające subskrypcje możesz znaleźć, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="ad0cb-110">1 stycznia 2019 r. dla określonych subskrypcji zostanie ustawiona wartość auto renew=False.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="ad0cb-111">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="ad0cb-112">Oferty usługi Dynamics 365 są wy wycofane</span><span class="sxs-lookup"><span data-stu-id="ad0cb-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="ad0cb-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-114">Dynamics 365 for Sales Enterprise Edition CRMOL — podstawowa (oferta kwalifikowana) dla nauczycieli</span><span class="sxs-lookup"><span data-stu-id="ad0cb-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad0cb-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kwalifikowana oferta) dla uczniów</span><span class="sxs-lookup"><span data-stu-id="ad0cb-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad0cb-116">Dynamics 365 for Sales Enterprise Edition (ceny dla instytucji rządowych) CRMOL — podstawowa (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="ad0cb-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad0cb-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="ad0cb-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad0cb-120">Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) od skoja września 2017 r. dla crm (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana) dla nauczycieli i wykładowców</span><span class="sxs-lookup"><span data-stu-id="ad0cb-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad0cb-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana) dla uczniów</span><span class="sxs-lookup"><span data-stu-id="ad0cb-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad0cb-124">Dynamics 365 for Sales Enterprise Edition (cennik dla instytucji rządowych) dla Add-On crm (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (ceny dla instytucji rządowych) CRMOL — podstawowa (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Oferta kwalifikowana) dla uczniów</span><span class="sxs-lookup"><span data-stu-id="ad0cb-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad0cb-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (oferta kwalifikowana) dla nauczycieli i wykładowców</span><span class="sxs-lookup"><span data-stu-id="ad0cb-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad0cb-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Kwalifikowana oferta)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (cennik dla instytucji rządowych) z skoja stycznia 2017 r. dla crm (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="ad0cb-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad0cb-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="ad0cb-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad0cb-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (ceny dla instytucji rządowych) Add-On crm Basic (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Oferta kwalifikowana) dla uczniów</span><span class="sxs-lookup"><span data-stu-id="ad0cb-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad0cb-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (oferta kwalifikowana) dla nauczycieli i wykładowców</span><span class="sxs-lookup"><span data-stu-id="ad0cb-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="ad0cb-137">Plan usługi Dynamics 365 for Sales/Customer Engagement z planów zastępczych w podstawową (kwalifikowanych ofertach)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="ad0cb-138">**Wycofane oferty**</span><span class="sxs-lookup"><span data-stu-id="ad0cb-138">**Retired offers**</span></span>   

- <span data-ttu-id="ad0cb-139">Dynamics 365 for Sales z usługi CRM Basic lub CRMOL Basic (oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad0cb-140">Dynamics 365 Customer Engagement Plan from CRM Basic lub CRMOL Basic (Oferta kwalifikowana)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="ad0cb-141">**Opcje zamiany**</span><span class="sxs-lookup"><span data-stu-id="ad0cb-141">**Replacement options**</span></span>
- <span data-ttu-id="ad0cb-142">Dynamics 365 for Sales Professional (NOWOŚĆ)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ad0cb-143">Dynamics 365 for Sales Professional (NOWOŚĆ)</span><span class="sxs-lookup"><span data-stu-id="ad0cb-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ad0cb-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="ad0cb-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="ad0cb-145">Dynamics 365 Customer Engagement Plan lub</span><span class="sxs-lookup"><span data-stu-id="ad0cb-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="ad0cb-146">Członkowie zespołu usługi Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ad0cb-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ad0cb-147">Przechodzenie klientów do nowych planów produktów</span><span class="sxs-lookup"><span data-stu-id="ad0cb-147">Transition customers to new product plans</span></span>

<span data-ttu-id="ad0cb-148">Przenoszenie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków w tej kolejności:</span><span class="sxs-lookup"><span data-stu-id="ad0cb-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="ad0cb-149">Kupowanie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="ad0cb-149">Purchase the new subscription</span></span>
- <span data-ttu-id="ad0cb-150">Ponowne przypisanie bieżących licencji użytkowników</span><span class="sxs-lookup"><span data-stu-id="ad0cb-150">Reassign current user licenses</span></span>
- <span data-ttu-id="ad0cb-151">Anulowanie starej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="ad0cb-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="ad0cb-152">Zakup nowego planu dla klienta</span><span class="sxs-lookup"><span data-stu-id="ad0cb-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="ad0cb-153">Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, którego chcesz przenieść do nowej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="ad0cb-154">Wybierz **pozycję Dodaj subskrypcję.**</span><span class="sxs-lookup"><span data-stu-id="ad0cb-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="ad0cb-155">Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="ad0cb-156">Klient będzie teraz miał starą i nową subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="ad0cb-157">Następnym krokiem jest ponowne przypisanie licencji do użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="ad0cb-158">Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, który przenosisz.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ad0cb-159">Wybierz **pozycję Użytkownicy i licencje.**</span><span class="sxs-lookup"><span data-stu-id="ad0cb-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="ad0cb-160">Aby ponownie przypisać licencję do użytkownika, wybierz użytkownika, a następnie wybierz pozycję **Zarządzaj licencjami.**</span><span class="sxs-lookup"><span data-stu-id="ad0cb-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="ad0cb-161">Na stronie Zarządzanie **licencjami** wyczyść pole wyboru Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license (Plan usługi Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) (Plan usługi Dynamics 365 for Sales/ Customer Engagement plan from Basic (Qualified Offer) (Plan usługi Dynamics 365 for Sales/Customer Engagement z licencji Podstawowej (kwalifikowana oferta) i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="ad0cb-162">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-162">Select **Submit**.</span></span> <span data-ttu-id="ad0cb-163">Zrobisz to dla każdego użytkownika, który potrzebuje nowej licencji.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="ad0cb-164">Po przeniesioniu licencji do nowej subskrypcji możesz anulować starą subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="ad0cb-165">Wybierz **pozycję Klienci** w lewym okienku nav, a następnie wybierz klienta, który przenosisz.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ad0cb-166">Na stronie szczegółów subskrypcji ustaw starą subskrypcję na wartość **Wstrzymano** i wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="ad0cb-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="ad0cb-167">Stara subskrypcja została wstrzymana, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="ad0cb-168">Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ad0cb-169">Klient nie poniesie żadnych dodatkowych kosztów dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="ad0cb-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



