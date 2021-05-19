---
title: Migrowanie usługi Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przeprowadzić migrację kwalifikowanych ofert usługi Dynamics 365 Business Edition do nowszej wersji, zanim wygasną.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151529"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="16d23-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Migrowanie ofert usługi Dynamics 365 Business Edition do nowszych wersji)</span><span class="sxs-lookup"><span data-stu-id="16d23-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="16d23-104">**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="16d23-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="16d23-105">Od 1 stycznia 2019 r. klienci z subskrypcjami usługi Dynamics 365 Business Edition nie mogą już odnawiać tych starszych ofert. Istniejące subskrypcje nie będą odnawiane automatycznie po wygaśnięciu.</span><span class="sxs-lookup"><span data-stu-id="16d23-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="16d23-106">Na stronie szczegółów subskrypcji stan subskrypcji zmieni się na "Wygasa [data]" z "Automatyczne odnowienie [data]".</span><span class="sxs-lookup"><span data-stu-id="16d23-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="16d23-107">Aby zapewnić ciągłość działania klientów, należy przejść te z wygasających subskrypcji do obsługiwanej opcji wymienionej poniżej.</span><span class="sxs-lookup"><span data-stu-id="16d23-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="16d23-108">Zalecamy przeniesienie klientów do nowych subskrypcji przed datą zakończenia subskrypcji w roku, aby uniknąć jakichkolwiek outages usługi dla klientów.</span><span class="sxs-lookup"><span data-stu-id="16d23-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="16d23-109">Jeśli używasz interfejsu API (CREST lub Partner Center), wygasające subskrypcje możesz znaleźć, oceniając datę zakończenia subskrypcji wraz z właściwością automatycznego odnawiania = False.</span><span class="sxs-lookup"><span data-stu-id="16d23-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="16d23-110">1 stycznia 2019 r. dla określonych subskrypcji zostanie ustawiona opcja automatycznego odnawiania=Fałsz.</span><span class="sxs-lookup"><span data-stu-id="16d23-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="16d23-111">Klientów można przenieść do nowego planu w dowolnym momencie.</span><span class="sxs-lookup"><span data-stu-id="16d23-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="16d23-112">Wycofane wersje usługi Dynamics 365 Business</span><span class="sxs-lookup"><span data-stu-id="16d23-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="16d23-113">Dynamics 365 for Finance and Operations, wersja Business</span><span class="sxs-lookup"><span data-stu-id="16d23-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="16d23-114">Dynamics 365 for Team Members, wersja Business</span><span class="sxs-lookup"><span data-stu-id="16d23-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="16d23-115">Dynamics Business Central — nowe oferty usługi Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="16d23-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="16d23-116">Dzięki nowym ofertom usługi Dynamics Business Central klienci mogą łączyć swoje finanse, sprzedaż, usługi i operacje, aby usprawnić procesy biznesowe, usprawnić interakcje z klientami i podejmować lepsze decyzje.</span><span class="sxs-lookup"><span data-stu-id="16d23-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="16d23-117">Usługa Dynamics 365 Business Central jest oparta na chmurze i jest dostępna tylko za pośrednictwem Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="16d23-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="16d23-118">Klienci usługi Dynamics 365 Business Edition są uprawnieni do otrzymania cennika przejścia z rabatem dla nowych ofert usługi Business Central do 30 czerwca 2020 r.</span><span class="sxs-lookup"><span data-stu-id="16d23-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="16d23-119">Przechodzenie klientów do nowych planów produktów</span><span class="sxs-lookup"><span data-stu-id="16d23-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="16d23-120">Przenoszenie klientów z wycofanych do nowszej jednostki SKU wymaga następujących kroków w tej kolejności:</span><span class="sxs-lookup"><span data-stu-id="16d23-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="16d23-121">Kupowanie nowej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="16d23-121">Purchase the new subscription</span></span>
- <span data-ttu-id="16d23-122">Ponowne przypisanie bieżących licencji użytkowników</span><span class="sxs-lookup"><span data-stu-id="16d23-122">Reassign current user licenses</span></span>
- <span data-ttu-id="16d23-123">Anulowanie starej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="16d23-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="16d23-124">Zakup nowego planu dla klienta</span><span class="sxs-lookup"><span data-stu-id="16d23-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="16d23-125">Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, którego chcesz przenieść do nowej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="16d23-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="16d23-126">Wybierz **pozycję Dodaj subskrypcję.**</span><span class="sxs-lookup"><span data-stu-id="16d23-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="16d23-127">Wybierz subskrypcję, którą chcesz kupić z katalogu (w tym przypadku jedną z powyższych opcji), wprowadź liczbę licencji, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="16d23-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="16d23-128">Klient będzie teraz miał starą i nową subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="16d23-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="16d23-129">Następnym krokiem jest ponowne przypisanie licencji do użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="16d23-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="16d23-130">Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, który przenosisz.</span><span class="sxs-lookup"><span data-stu-id="16d23-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="16d23-131">Wybierz **pozycję Użytkownicy i licencje.**</span><span class="sxs-lookup"><span data-stu-id="16d23-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="16d23-132">Aby ponownie przypisać licencję do użytkownika, wybierz użytkownika, a następnie wybierz pozycję **Zarządzaj licencjami.**</span><span class="sxs-lookup"><span data-stu-id="16d23-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="16d23-133">Na stronie Zarządzanie **licencjami** wyczyść pole wyboru Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license (Plan usługi Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) (Plan usługi Dynamics 365 for Sales/ Customer Engagement plan from Basic (Qualified Offer) (Plan usługi Dynamics 365 for Sales/Customer Engagement z licencji Podstawowej (kwalifikowana oferta) i wybierz nowy plan usługi dla subskrypcji, do których klient jest przenoszący.</span><span class="sxs-lookup"><span data-stu-id="16d23-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="16d23-134">Wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="16d23-134">Select **Submit**.</span></span> <span data-ttu-id="16d23-135">Zrobisz to dla każdego użytkownika, który potrzebuje nowej licencji.</span><span class="sxs-lookup"><span data-stu-id="16d23-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="16d23-136">Po przeniesionej licencji do nowej subskrypcji możesz anulować starą subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="16d23-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="16d23-137">Wybierz **pozycję Klienci** w lewym okienku, a następnie wybierz klienta, który przenosisz.</span><span class="sxs-lookup"><span data-stu-id="16d23-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="16d23-138">Na stronie szczegółów subskrypcji ustaw starą subskrypcję na **wstrzymaną i** wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="16d23-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="16d23-139">Stara subskrypcja została wstrzymana, a nowa subskrypcja jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="16d23-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="16d23-140">Wstrzymana subskrypcja zostanie automatycznie anulowana po upływie 120 dni.</span><span class="sxs-lookup"><span data-stu-id="16d23-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="16d23-141">Klient nie poniesie żadnych dodatkowych kosztów dla starej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="16d23-141">Your customer will incur no additional costs for the old subscription.</span></span>
