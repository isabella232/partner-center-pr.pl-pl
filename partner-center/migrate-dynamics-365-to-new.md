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
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132642"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="94f35-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Migrowanie ofert usługi Dynamics 365 Business Edition do nowszych wersji)</span><span class="sxs-lookup"><span data-stu-id="94f35-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="94f35-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="94f35-104">**Appropriate roles**</span></span>

- <span data-ttu-id="94f35-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="94f35-105">Global admin</span></span>
- <span data-ttu-id="94f35-106">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="94f35-106">User management admin</span></span>
- <span data-ttu-id="94f35-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="94f35-107">Admin agent</span></span>
- <span data-ttu-id="94f35-108">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="94f35-108">Sales agent</span></span>

<span data-ttu-id="94f35-109">Od 1 stycznia 2019 klienci korzystający z subskrypcji Dynamics 365 Business Edition nie mogą już odnowiać tych starszych ofert; istniejące subskrypcje nie będą odnawiane automatycznie po ich wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="94f35-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="94f35-110">Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "wygasa w dniu [Date]" z "autonews w dniu [Date]".</span><span class="sxs-lookup"><span data-stu-id="94f35-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="94f35-111">Aby zapewnić ciągłość dla klientów, należy przenieść te osoby z wygasanymi subskrypcjami do obsługiwanej opcji, wymienione poniżej.</span><span class="sxs-lookup"><span data-stu-id="94f35-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="94f35-112">Zalecamy przeniesienie klientów do nowych subskrypcji przed roczną datą końcową subskrypcji, aby uniknąć przerwy w działaniu usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="94f35-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="94f35-113">W przypadku korzystania z interfejsu API (SZCZYTu lub Centrum partnerskiego) można wyszukać wygasające subskrypcje, oceniając datę końcową subskrypcji wraz z właściwością autorenew = false.</span><span class="sxs-lookup"><span data-stu-id="94f35-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="94f35-114">Dla podanych subskrypcji zostanie ustawiona wartość autorenew = false 1 stycznia 2019.</span><span class="sxs-lookup"><span data-stu-id="94f35-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="94f35-115">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="94f35-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="94f35-116">Wycofywane wersje systemu Dynamics 365 Business</span><span class="sxs-lookup"><span data-stu-id="94f35-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="94f35-117">Dynamics 365 dla finansów i operacji, wersja Business</span><span class="sxs-lookup"><span data-stu-id="94f35-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="94f35-118">Dynamics 365 dla członków zespołu, wersja Business</span><span class="sxs-lookup"><span data-stu-id="94f35-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="94f35-119">Dynamics Business Central — wersja Dynamics 365 Business Edition — nowe oferty</span><span class="sxs-lookup"><span data-stu-id="94f35-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="94f35-120">Nowe oferty usługi Dynamics Business Central umożliwiają klientom łączenie ich finansów, sprzedaży, usług i operacji w celu usprawnienia procesów biznesowych, poprawy interakcji z klientami oraz podejmowania lepszych decyzji.</span><span class="sxs-lookup"><span data-stu-id="94f35-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="94f35-121">Usługa Dynamics 365 Business Central jest oparta na chmurze i dostępna za pośrednictwem partnerów programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="94f35-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="94f35-122">Klienci korzystający z systemu Dynamics 365 Business Edition mogą otrzymywać obniżone ceny za okresy przejściowe dla nowych ofert w ramach usługi Business Central do 30 czerwca 2020.</span><span class="sxs-lookup"><span data-stu-id="94f35-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="94f35-123">Przejście klientów do nowych planów produktu</span><span class="sxs-lookup"><span data-stu-id="94f35-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="94f35-124">Przeniesienie klientów z wycofanych jednostek SKU do nowszych wersji wymaga wykonania następujących kroków w tej kolejności:</span><span class="sxs-lookup"><span data-stu-id="94f35-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="94f35-125">Kup nową subskrypcję</span><span class="sxs-lookup"><span data-stu-id="94f35-125">Purchase the new subscription</span></span>
- <span data-ttu-id="94f35-126">Ponowne przypisanie bieżących licencji użytkownika</span><span class="sxs-lookup"><span data-stu-id="94f35-126">Reassign current user licenses</span></span>
- <span data-ttu-id="94f35-127">Anuluj starą subskrypcję</span><span class="sxs-lookup"><span data-stu-id="94f35-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="94f35-128">Kup nowy plan dla klienta</span><span class="sxs-lookup"><span data-stu-id="94f35-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="94f35-129">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz klienta, który ma zostać przeniesiony do nowej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="94f35-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="94f35-130">Wybierz pozycję **Dodaj subskrypcję**.</span><span class="sxs-lookup"><span data-stu-id="94f35-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="94f35-131">Wybierz subskrypcję, którą chcesz kupić z wykazu (w tym przypadku jedną z opcji powyżej), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="94f35-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="94f35-132">Klient będzie miał teraz zarówno starą subskrypcję, jak i nową.</span><span class="sxs-lookup"><span data-stu-id="94f35-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="94f35-133">Następnym krokiem jest ponowne przypisanie licencji do użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="94f35-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="94f35-134">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="94f35-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="94f35-135">Wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="94f35-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="94f35-136">Aby ponownie przypisać licencję do użytkownika, wybierz użytkownika, a następnie wybierz pozycję **Zarządzaj licencjami**.</span><span class="sxs-lookup"><span data-stu-id="94f35-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="94f35-137">Na stronie **Zarządzanie licencjami** Usuń zaznaczenie pola wyboru Dynamics 365 for Sales/Customer Engagement from Basic (kwalifikowana oferta), a następnie wybierz nowy plan usługi dla subskrypcji, do której będzie przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="94f35-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="94f35-138">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="94f35-138">Select **Submit**.</span></span> <span data-ttu-id="94f35-139">Należy to zrobić dla każdego użytkownika, który potrzebuje nowej licencji.</span><span class="sxs-lookup"><span data-stu-id="94f35-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="94f35-140">Po przeniesieniu licencji do nowej subskrypcji można anulować starą subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="94f35-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="94f35-141">Wybierz pozycję **klienci** na lewym panelu nawigacyjnym, a następnie wybierz przenoszony klient.</span><span class="sxs-lookup"><span data-stu-id="94f35-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="94f35-142">Na stronie Szczegóły subskrypcji Ustaw starą subskrypcję na **zawieszoną** i wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="94f35-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="94f35-143">Stara subskrypcja jest zawieszona, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="94f35-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="94f35-144">Zawieszona subskrypcja zostanie cofnięta automatycznie po 120 dniach.</span><span class="sxs-lookup"><span data-stu-id="94f35-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="94f35-145">Klient nie będzie miał dodatkowych kosztów dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="94f35-145">Your customer will incur no additional costs for the old subscription.</span></span>
