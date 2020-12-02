---
title: Migrowanie systemu Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zapoznaj się z tematem, jak przeprowadzić migrację do wersji kwalifikowanej systemu Dynamics 365 Business Edition, zanim wygasną.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529278"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="c3ced-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Migrowanie ofert usługi Dynamics 365 Business Edition do nowszych wersji)</span><span class="sxs-lookup"><span data-stu-id="c3ced-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="c3ced-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="c3ced-104">**Applies to**</span></span>

- <span data-ttu-id="c3ced-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="c3ced-105">Partner Center</span></span>

<span data-ttu-id="c3ced-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="c3ced-106">**Appropriate roles**</span></span>
- <span data-ttu-id="c3ced-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="c3ced-107">Global admin</span></span>
- <span data-ttu-id="c3ced-108">Administrator użytkowników</span><span class="sxs-lookup"><span data-stu-id="c3ced-108">User admin</span></span>
- <span data-ttu-id="c3ced-109">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="c3ced-109">Admin agent</span></span>
- <span data-ttu-id="c3ced-110">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="c3ced-110">Sales agent</span></span>

<span data-ttu-id="c3ced-111">Od 1 stycznia 2019 klienci korzystający z subskrypcji Dynamics 365 Business Edition nie mogą już odnowiać tych starszych ofert; istniejące subskrypcje nie będą odnawiane automatycznie po ich wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="c3ced-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="c3ced-112">Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "wygasa w dniu [Date]" z "autonews w dniu [Date]".</span><span class="sxs-lookup"><span data-stu-id="c3ced-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="c3ced-113">Aby zapewnić ciągłość dla klientów, należy przenieść te osoby z wygasanymi subskrypcjami do obsługiwanej opcji, wymienione poniżej.</span><span class="sxs-lookup"><span data-stu-id="c3ced-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="c3ced-114">Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="c3ced-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="c3ced-115">W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można wyszukać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false.</span><span class="sxs-lookup"><span data-stu-id="c3ced-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="c3ced-116">W przypadku tej subskrypcji zostanie ustawiona wartość autorenew = false 1 stycznia 2019.</span><span class="sxs-lookup"><span data-stu-id="c3ced-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="c3ced-117">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="c3ced-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="c3ced-118">Wycofywane wersje systemu Dynamics 365 Business</span><span class="sxs-lookup"><span data-stu-id="c3ced-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="c3ced-119">Dynamics 365 dla finansów i operacji, wersja Business</span><span class="sxs-lookup"><span data-stu-id="c3ced-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="c3ced-120">Dynamics 365 dla członków zespołu, wersja Business</span><span class="sxs-lookup"><span data-stu-id="c3ced-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="c3ced-121">Dynamics Business Central — wersja Dynamics 365 Business Edition — nowe oferty</span><span class="sxs-lookup"><span data-stu-id="c3ced-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="c3ced-122">Nowe oferty usługi Dynamics Business Central umożliwiają klientom łączenie ich finansów, sprzedaży, usług i operacji w celu usprawnienia procesów biznesowych, poprawy interakcji z klientami oraz podejmowania lepszych decyzji.</span><span class="sxs-lookup"><span data-stu-id="c3ced-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="c3ced-123">Usługa Dynamics 365 Business Central jest oparta na chmurze i dostępna za pośrednictwem partnerów programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="c3ced-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="c3ced-124">Klienci korzystający z systemu Dynamics 365 Business Edition mogą otrzymywać obniżone ceny za okresy przejściowe dla nowych ofert w ramach usługi Business Central do 30 czerwca 2020.</span><span class="sxs-lookup"><span data-stu-id="c3ced-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c3ced-125">Przejście klientów do nowych planów produktu</span><span class="sxs-lookup"><span data-stu-id="c3ced-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="c3ced-126">Przeniesienie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących kroków w tej kolejności:</span><span class="sxs-lookup"><span data-stu-id="c3ced-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="c3ced-127">Kup nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="c3ced-127">Purchase the new subscription</span></span>
- <span data-ttu-id="c3ced-128">Ponowne przypisanie bieżących licencji użytkownika</span><span class="sxs-lookup"><span data-stu-id="c3ced-128">Reassign current user licenses</span></span>
- <span data-ttu-id="c3ced-129">Anuluj starą subskrypcję</span><span class="sxs-lookup"><span data-stu-id="c3ced-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="c3ced-130">Kup nowy plan dla klienta</span><span class="sxs-lookup"><span data-stu-id="c3ced-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="c3ced-131">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz klienta, który ma zostać przeniesiony do nowej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="c3ced-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="c3ced-132">Wybierz pozycję **Dodaj subskrypcję**.</span><span class="sxs-lookup"><span data-stu-id="c3ced-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="c3ced-133">Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="c3ced-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="c3ced-134">Klient będzie miał teraz zarówno starą subskrypcję, jak i nową.</span><span class="sxs-lookup"><span data-stu-id="c3ced-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="c3ced-135">Następnym krokiem jest ponowne przypisanie licencji do użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="c3ced-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="c3ced-136">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="c3ced-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c3ced-137">Wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="c3ced-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="c3ced-138">Aby ponownie przypisać licencję do użytkownika, wybierz użytkownika, a następnie wybierz pozycję **Zarządzaj licencjami**.</span><span class="sxs-lookup"><span data-stu-id="c3ced-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="c3ced-139">Na stronie **Zarządzanie licencjami** Usuń zaznaczenie pola wyboru Dynamics 365 for Sales/Customer Engagement from Basic (kwalifikowana oferta), a następnie wybierz nowy plan usługi dla subskrypcji, do której będzie przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="c3ced-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="c3ced-140">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="c3ced-140">Select **Submit**.</span></span> <span data-ttu-id="c3ced-141">Należy to zrobić dla każdego użytkownika, który potrzebuje nowej licencji.</span><span class="sxs-lookup"><span data-stu-id="c3ced-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="c3ced-142">Po przeniesieniu licencji do nowej subskrypcji można anulować starą subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="c3ced-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="c3ced-143">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="c3ced-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c3ced-144">Na stronie Szczegóły subskrypcji Ustaw starą subskrypcję na **zawieszoną** i wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="c3ced-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="c3ced-145">Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="c3ced-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="c3ced-146">Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach.</span><span class="sxs-lookup"><span data-stu-id="c3ced-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c3ced-147">Klient nie będzie miał dodatkowych kosztów dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="c3ced-147">Your customer will incur no additional costs for the old subscription.</span></span>
