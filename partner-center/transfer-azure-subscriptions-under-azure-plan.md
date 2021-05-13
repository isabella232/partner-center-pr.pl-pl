---
title: Przenoszenie subskrypcji platformy Azure w ramach planu platformy Azure do innego partnera CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak Dostawca rozwiązań w chmurze programu partnerskiego skojarzonego z subskrypcjami platformy Azure klienta w ramach planu platformy Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856053"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="257c8-103">Przenoszenie subskrypcji planu platformy Azure klienta do innego partnera</span><span class="sxs-lookup"><span data-stu-id="257c8-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="257c8-104">**Odpowiednie role:** Administrator konta | Agent sprzedaży | Agent rozliczeń</span><span class="sxs-lookup"><span data-stu-id="257c8-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="257c8-105">W tym artykule opisano, jak klient może przełączać swoje subskrypcje platformy Azure w ramach planu platformy Azure z jednego Dostawca rozwiązań w chmurze (CSP) na inny.</span><span class="sxs-lookup"><span data-stu-id="257c8-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="257c8-106">Aby przełączyć subskrypcje platformy Azure klienta z innego partnera, wykonaj następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="257c8-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="257c8-107">Zarówno partner, jak i klient mają kroki do wykonania.</span><span class="sxs-lookup"><span data-stu-id="257c8-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="257c8-108">Tylko partnerzy z bezpośrednią relacją rozliczeń z firmą Microsoft mogą uzyskać dostęp do narzędzi przejścia.</span><span class="sxs-lookup"><span data-stu-id="257c8-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="257c8-109">Odsprzedawcy pośredni muszą współpracować z dostawcami pośrednimi, aby korzystać z tego narzędzia przejściowego.</span><span class="sxs-lookup"><span data-stu-id="257c8-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="257c8-110">Przed rozpoczęciem tego narzędzia klient musi być w rozmowie z partnerami (bieżącymi i przyszłymi).</span><span class="sxs-lookup"><span data-stu-id="257c8-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="257c8-111">Konwersacja w trybie offline musi wymagać uniknięcia nieporozumień i rezygnacji.</span><span class="sxs-lookup"><span data-stu-id="257c8-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="257c8-112">Ponadto partnerzy i klienci powinni zrozumieć te zagadnienia i wymagania wstępne przed zainicjowanie przejścia:</span><span class="sxs-lookup"><span data-stu-id="257c8-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="257c8-113">**Najważniejsze kwestie do rozważenia:**</span><span class="sxs-lookup"><span data-stu-id="257c8-113">**Key considerations:**</span></span>

- <span data-ttu-id="257c8-114">Rezerwacje platformy Azure nie zostaną przeniesiene z subskrypcją do przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="257c8-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="257c8-115">Cennik programu CSP dla usług platformy Azure w ramach bieżącego partnera nie zostanie przejściowy</span><span class="sxs-lookup"><span data-stu-id="257c8-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="257c8-116">Obowiązki pomocy technicznej dla klienta przejdą do przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="257c8-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="257c8-117">Rozliczenia i fakturowanie zostaną przeniesieni do przyszłego partnera w momencie przeniesienia</span><span class="sxs-lookup"><span data-stu-id="257c8-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="257c8-118">Transfer Role-Based Access Control nie ma wpływu na usługę Azure Role-Based Access Control (RBAC)</span><span class="sxs-lookup"><span data-stu-id="257c8-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="257c8-119">Administrator w imieniu (AOBO) nie zostanie przyznany domyślnie przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="257c8-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="257c8-120">Produkty innych firm na platformie handlowej zostaną przesłonene, o ile produkty przejdą weryfikację uprawnień do korzystania z witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="257c8-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="257c8-121">Nie ma żadnych specjalnych rabatów ani ograniczeń regionalnych</span><span class="sxs-lookup"><span data-stu-id="257c8-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="257c8-122">Produkty nie są oparte na subskrypcji</span><span class="sxs-lookup"><span data-stu-id="257c8-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="257c8-123">Przyszły partner powinien współpracować z wydawcą, aby upewnić się, że jest na liście zezwalania na wdrożenie produktu</span><span class="sxs-lookup"><span data-stu-id="257c8-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="257c8-124">Jeśli nie wszystkie te warunki zostaną spełnione w celu przeniesienia produktów z witryny Marketplace, zostaną anulowane, subskrypcje platformy Azure zostaną przeniesione, a następnie ponownie wykup produktów z witryny Marketplace u nowego partnera</span><span class="sxs-lookup"><span data-stu-id="257c8-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="257c8-125">**Wymagania wstępne:**</span><span class="sxs-lookup"><span data-stu-id="257c8-125">**Prerequisites:**</span></span>

- <span data-ttu-id="257c8-126">Klient kontaktuje się z bieżącym partnerem CSP w sprawie zamiaru przejścia</span><span class="sxs-lookup"><span data-stu-id="257c8-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="257c8-127">Przyszły partner CSP współpracuje z klientem w celu zapewnienia, że można spełnić potrzeby klientów</span><span class="sxs-lookup"><span data-stu-id="257c8-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="257c8-128">Przyszły partner CSP ustanawia relację z klientem i kupuje plan platformy Azure przed rozpoczęciem przejścia</span><span class="sxs-lookup"><span data-stu-id="257c8-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="257c8-129">Klient musi podpisać umowę Umowa z Klientem Microsoft z przyszłym partnerem CSP</span><span class="sxs-lookup"><span data-stu-id="257c8-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="257c8-130">Przyszły partner CSP musi mieć podpisaną Microsoft Partner Agreement, aby korzystać z tego narzędzia</span><span class="sxs-lookup"><span data-stu-id="257c8-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="257c8-131">Zadania klienta do wykonania</span><span class="sxs-lookup"><span data-stu-id="257c8-131">Customer tasks to be completed</span></span>

<span data-ttu-id="257c8-132">Aby przenieść subskrypcję platformy Azure w ramach planu platformy Azure, klient musi rozpocząć proces, kontaktując się ze swoim bieżącym partnerem.</span><span class="sxs-lookup"><span data-stu-id="257c8-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="257c8-133">Powinni zebrać nazwę firmy i domenę bieżącego partnera, aby przyszły partner może wypełnić formularz żądania przeniesienia w jego imieniu.</span><span class="sxs-lookup"><span data-stu-id="257c8-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="257c8-134">Klient musi również zidentyfikować subskrypcje, które chce przenieść od bieżącego partnera.</span><span class="sxs-lookup"><span data-stu-id="257c8-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="257c8-135">Nie można zmienić partnerów dla subskrypcji usługi Office 365, pakietu Enterprise Mobility Suite ani subskrypcji usługi Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="257c8-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="257c8-136">Przyszła odpowiedzialność partnera za ukończenie formularza żądania przeniesienia, który inicjuje proces transferu.</span><span class="sxs-lookup"><span data-stu-id="257c8-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="257c8-137">Firma Microsoft nie może interweniować w imieniu klienta ani bieżącego partnera.</span><span class="sxs-lookup"><span data-stu-id="257c8-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="257c8-138">Klient powinien zaplanować ścisłą współpracę ze swoim przyszłym i bieżącym partnerem, aby przejście przebiegało bezproblemowo.</span><span class="sxs-lookup"><span data-stu-id="257c8-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="257c8-139">Przyszłe zadania partnerów do wykonania</span><span class="sxs-lookup"><span data-stu-id="257c8-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="257c8-140">Przyszły partner subskrypcji musi wypełnić formularz żądania przeniesienia z Partner Center żądania przeniesienia subskrypcji:</span><span class="sxs-lookup"><span data-stu-id="257c8-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="257c8-141">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, dla których chcesz wypełnić formularz żądania przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="257c8-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="257c8-142">W menu Customer (Klient) wybierz **pozycję Subscriptions (Subskrypcje).**</span><span class="sxs-lookup"><span data-stu-id="257c8-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="257c8-143">Wybierz **sekcję Żądanie przeniesienia.**</span><span class="sxs-lookup"><span data-stu-id="257c8-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="257c8-144">W **sekcji Żądanie przeniesienia wybierz** **pozycję Dodaj nowe żądanie.**</span><span class="sxs-lookup"><span data-stu-id="257c8-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sekcja Transfery":::

5.  <span data-ttu-id="257c8-146">Wypełnij formularz **Nowe żądanie przeniesienia.**</span><span class="sxs-lookup"><span data-stu-id="257c8-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="257c8-147">Wybierz **pozycję Wyślij żądanie przeniesienia**  >  **Wyślij**.</span><span class="sxs-lookup"><span data-stu-id="257c8-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Pełny formularz żądania przeniesienia":::

7.  <span data-ttu-id="257c8-149">Przegląd potwierdzenia żądania przeniesienia</span><span class="sxs-lookup"><span data-stu-id="257c8-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Przegląd oczekujących transferów":::

    >[!Note]
    ><span data-ttu-id="257c8-151">Przyszły partner może anulować żądanie przeniesienia, wybierając pozycję **Anuluj** żądanie w prawym górnym rogu tylko wtedy, gdy żądanie przeniesienia ma stan "oczekujące".</span><span class="sxs-lookup"><span data-stu-id="257c8-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="257c8-152">Gdy stan żądania przeniesienia będzie "w toku" lub "ukończony", anulowanie nie będzie możliwe.</span><span class="sxs-lookup"><span data-stu-id="257c8-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="257c8-153">Bieżące zadania partnerów do wykonania</span><span class="sxs-lookup"><span data-stu-id="257c8-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="257c8-154">Agent administracyjny bieżącego partnera klienta otrzyma wiadomość e-mail z żądaniem przeniesienia subskrypcji przez klienta:</span><span class="sxs-lookup"><span data-stu-id="257c8-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Przegląd":::

<span data-ttu-id="257c8-156">Przejrzyj i zaakceptuj formularz żądania przeniesienia od Partner Center, aby ukończyć przenoszenie subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="257c8-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="257c8-157">Jeśli bieżący partner nie zostanie podjęty w ciągu 30 dni, żądanie wygaśnie, a przyszły partner będzie miał żądanie utworzenia nowego żądania przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="257c8-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="257c8-158">Wybierz **pozycję Przejrzyj żądanie przeniesienia z** wiadomości e-mail LUB</span><span class="sxs-lookup"><span data-stu-id="257c8-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="257c8-159">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, w imieniu których przesłano żądanie przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="257c8-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="257c8-160">W menu Customer (Klient) wybierz **pozycję Subscriptions (Subskrypcje).**</span><span class="sxs-lookup"><span data-stu-id="257c8-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="257c8-161">Wybierz **sekcję Żądanie przeniesienia.**</span><span class="sxs-lookup"><span data-stu-id="257c8-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="257c8-162">Rozwiń informacje o transferze, wybierając **wybrany identyfikator żądania przeniesienia w** obszarze **Odebrane żądania**</span><span class="sxs-lookup"><span data-stu-id="257c8-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Żądanie przeniesienia przeglądów źródła":::

5.  <span data-ttu-id="257c8-164">Przejrzyj żądanie przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="257c8-164">Review transfer request.</span></span> <span data-ttu-id="257c8-165">Wybierz żądane subskrypcje platformy Azure do przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="257c8-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="257c8-166">Przed przystąpieniem pamiętaj: nie będziesz już mieć dostępu do wybranych subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="257c8-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="257c8-167">Dalsze użycie nie zostanie zafakturowane.</span><span class="sxs-lookup"><span data-stu-id="257c8-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="257c8-168">Rezerwacje platformy Azure nie są transferowe z subskrypcjami.</span><span class="sxs-lookup"><span data-stu-id="257c8-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="257c8-169">Następnie wybierz **pozycję Zaakceptuj i przenieś,** aby zakończyć proces przenoszenia.</span><span class="sxs-lookup"><span data-stu-id="257c8-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Wybieranie subskrypcji do przeniesienia w ramach planów platformy Azure":::

7.  <span data-ttu-id="257c8-171">Wyświetlanie potwierdzenia akceptacji przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="257c8-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="257c8-172">W tym momencie przyszły partner, klient i bieżący partner zostaną powiadomieni o zaakceptowanym żądaniu przeniesienia za pośrednictwem poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="257c8-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="257c8-173">Po zaakceptowaniu przeniesienia może on pozostać w stanie Oczekujące przez maksymalnie 15 minut podczas aktualizowania systemu.</span><span class="sxs-lookup"><span data-stu-id="257c8-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="257c8-174">Jeśli trwa to dłużej, system będzie próbować przez trzy dni.</span><span class="sxs-lookup"><span data-stu-id="257c8-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="257c8-175">Jeśli stan przeniesienia nadal będzie mieć stan Oczekujące, partner powinien przesłać żądanie obsługi.</span><span class="sxs-lookup"><span data-stu-id="257c8-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="257c8-176">Po zakończeniu przenoszenia subskrypcje uwzględnione w żądaniu będą wyświetlane w planie platformy Azure przyszłego partnera i nie będą już wyświetlane w nim.</span><span class="sxs-lookup"><span data-stu-id="257c8-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="257c8-177">W przypadku dostawców pośrednich: poinformuj odsprzedawcę pośredniego, że żądanie przeniesienia zostało zaakceptowane.</span><span class="sxs-lookup"><span data-stu-id="257c8-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="257c8-178">Zarządzanie przeniesionymi subskrypcjami klientów</span><span class="sxs-lookup"><span data-stu-id="257c8-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="257c8-179">Przejście nie wpływa na dostęp do istniejących użytkowników, grup lub jednostek usługi, które zostały przypisane przy użyciu kontroli dostępu na podstawie ról (RBAC) na platformie Azure.</span><span class="sxs-lookup"><span data-stu-id="257c8-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="257c8-180">Kontrola dostępu oparta na rolach [(RBAC)](/azure/role-based-access-control/overview) na platformie Azure pomaga klientom zarządzać tym, kto ma dostęp do zasobów platformy Azure, co może zrobić z tymi zasobami i do jakich obszarów ma dostęp.</span><span class="sxs-lookup"><span data-stu-id="257c8-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="257c8-181">Jako nowy partner nie masz dostępu RBAC do zasobów klienta po przeniesieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="257c8-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="257c8-182">Poprzedni partner klienta zachowuje dostęp RBAC.</span><span class="sxs-lookup"><span data-stu-id="257c8-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="257c8-183">We współpracy z klientem dowiedz się, kto ma wgląd w swoje subskrypcje i jak wprowadzać dowolne zmiany.</span><span class="sxs-lookup"><span data-stu-id="257c8-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="257c8-184">W związku z tym ważne jest, aby klient usuał dostęp RBAC platformy Azure dla poprzedniego partnera i dodał dostęp dla nowego partnera.</span><span class="sxs-lookup"><span data-stu-id="257c8-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="257c8-185">Aby uzyskać więcej informacji na temat nowego dostępu klienta, zobacz Co to jest kontrola dostępu na podstawie ról [(RBAC) platformy Azure?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="257c8-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="257c8-186">Aby uzyskać więcej informacji na temat usuwania dostępu RBAC poprzedniego partnera przez klienta, zobacz [Usuwanie przypisania roli.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="257c8-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="257c8-187">Ponadto nie uzyskujesz automatycznie dostępu [administratora w imieniu (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) do subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="257c8-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="257c8-188">Usługa AOBO jest niezbędna, aby partner zarządzał subskrypcjami platformy Azure swoich klientów w ich imieniu.</span><span class="sxs-lookup"><span data-stu-id="257c8-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="257c8-189">Aby uzyskać więcej informacji na temat uprawnień platformy Azure, zobacz Uzyskiwanie uprawnień do zarządzania [usługą lub subskrypcją klienta.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="257c8-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="257c8-190">Następne kroki:</span><span class="sxs-lookup"><span data-stu-id="257c8-190">Next steps:</span></span>

- [<span data-ttu-id="257c8-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="257c8-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="257c8-192">Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta.</span><span class="sxs-lookup"><span data-stu-id="257c8-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
