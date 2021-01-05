---
title: Przenoszenie subskrypcji platformy Azure w ramach planu platformy Azure do innego partnera CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak zmienić partnera programu Cloud Solution Provider skojarzonego z subskrypcjami platformy Azure klienta w ramach planu platformy Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893210"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="6869d-103">Przenoszenie subskrypcji planu platformy Azure klienta na innego partnera</span><span class="sxs-lookup"><span data-stu-id="6869d-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="6869d-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="6869d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="6869d-105">Partnerzy w programie dostawcy rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="6869d-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="6869d-106">W tym artykule opisano, jak klient może przełączyć swoje subskrypcje platformy Azure w ramach planu platformy Azure z jednego dostawcy rozwiązań w chmurze (CSP) na inny.</span><span class="sxs-lookup"><span data-stu-id="6869d-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="6869d-107">Aby przełączyć subskrypcje platformy Azure klienta z innego partnera, wykonaj następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="6869d-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="6869d-108">Zarówno partner, jak i klient mają kroki do wykonania.</span><span class="sxs-lookup"><span data-stu-id="6869d-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="6869d-109">Tylko partnerzy z bezpośrednią relacją rozliczeniową z firmą Microsoft mogą uzyskać dostęp do narzędzi przejścia.</span><span class="sxs-lookup"><span data-stu-id="6869d-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="6869d-110">Pośrednicy odsprzedawcy muszą współpracować z dostawcami pośrednimi, aby korzystać z tego narzędzia przejścia.</span><span class="sxs-lookup"><span data-stu-id="6869d-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="6869d-111">Klient musi znajdować się w konwersacji z partnerami (bieżący i przyszły) przed użyciem tego narzędzia.</span><span class="sxs-lookup"><span data-stu-id="6869d-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="6869d-112">Konwersacja w trybie offline musi mieć na celu uniknięcie pomyłek i zmian.</span><span class="sxs-lookup"><span data-stu-id="6869d-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="6869d-113">Ponadto partnerzy i klienci powinni zrozumieć te zagadnienia i wymagania wstępne przed zainicjowaniem przejścia:</span><span class="sxs-lookup"><span data-stu-id="6869d-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="6869d-114">**Kluczowe zagadnienia:**</span><span class="sxs-lookup"><span data-stu-id="6869d-114">**Key considerations:**</span></span>

- <span data-ttu-id="6869d-115">Azure Reservations nie zostanie przeniesiona z subskrypcją do przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="6869d-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="6869d-116">Cennik CSP dla usług platformy Azure w ramach bieżącego partnera nie zostanie przenoszony</span><span class="sxs-lookup"><span data-stu-id="6869d-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="6869d-117">Odpowiedzialność za pomoc techniczną dla klienta przejdzie do przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="6869d-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="6869d-118">Rozliczanie i fakturowanie będzie przenoszone do przyszłego partnera w czasie transferu</span><span class="sxs-lookup"><span data-stu-id="6869d-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="6869d-119">Transfer nie ma wpływ na usługę Azure Role-Based Access Control (RBAC)</span><span class="sxs-lookup"><span data-stu-id="6869d-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="6869d-120">Administrator w imieniu (AOBO) nie zostanie domyślnie udzielony dla przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="6869d-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="6869d-121">Produkty z witryny Marketplace innych firm zostaną przetransferowane, o ile produkty przechodzą przez sprawdzanie uprawnień witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6869d-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="6869d-122">Nie ma specjalnych rabatów ani ograniczeń regionalnych</span><span class="sxs-lookup"><span data-stu-id="6869d-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="6869d-123">Produkty nie są oparte na subskrypcji</span><span class="sxs-lookup"><span data-stu-id="6869d-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="6869d-124">W przyszłości Partner powinien współpracować z wydawcą, aby upewnić się, że znajdują się na liście dozwolonych dla wdrożenia produktu</span><span class="sxs-lookup"><span data-stu-id="6869d-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="6869d-125">Jeśli nie wszystkie te warunki zostaną spełnione, aby można było przenieść produkty z portalu Marketplace, przetransferowane subskrypcje platformy Azure, a następnie zakupione produkty Marketplace z nowym partnerem</span><span class="sxs-lookup"><span data-stu-id="6869d-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="6869d-126">**Wymagania wstępne:**</span><span class="sxs-lookup"><span data-stu-id="6869d-126">**Prerequisites:**</span></span>

- <span data-ttu-id="6869d-127">Klient angażuje bieżącego partnera CSP w celu przejścia</span><span class="sxs-lookup"><span data-stu-id="6869d-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="6869d-128">W przyszłości partner CSP współpracuje z klientem w celu zapewnienia, że potrzeby klientów mogą być spełnione</span><span class="sxs-lookup"><span data-stu-id="6869d-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="6869d-129">W przyszłości partner CSP nawiązuje relację z klientem i kupuje plan platformy Azure przed rozpoczęciem przejścia</span><span class="sxs-lookup"><span data-stu-id="6869d-129">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="6869d-130">Klient musi podpisać umowę klienta firmy Microsoft, korzystając z przyszłego partnera CSP</span><span class="sxs-lookup"><span data-stu-id="6869d-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="6869d-131">W przyszłości partner CSP musi mieć podpisaną umowę partner firmy Microsoft, aby móc korzystać z tego narzędzia</span><span class="sxs-lookup"><span data-stu-id="6869d-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="6869d-132">Zadania klienta do ukończenia</span><span class="sxs-lookup"><span data-stu-id="6869d-132">Customer tasks to be completed</span></span>

<span data-ttu-id="6869d-133">Aby przenieść subskrypcję platformy Azure w ramach planu platformy Azure, klient musi rozpocząć proces, kontaktując się z bieżącym partnerem.</span><span class="sxs-lookup"><span data-stu-id="6869d-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="6869d-134">Powinny one zbierać nazwę firmy i domenę bieżącego partnera, aby w przyszłości wszyscy partnerzy mogli zakończyć formularz żądania przeniesienia w ich imieniu.</span><span class="sxs-lookup"><span data-stu-id="6869d-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="6869d-135">Klient musi także zidentyfikować subskrypcje, które chcą przenieść z bieżącego partnera.</span><span class="sxs-lookup"><span data-stu-id="6869d-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="6869d-136">Nie można zmienić partnerów dla pakietów Office 365, Enterprise Mobility Suite ani Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="6869d-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="6869d-137">W przyszłości jest odpowiedzialny za wykonanie formularza żądania przeniesienia, który inicjuje proces transferu.</span><span class="sxs-lookup"><span data-stu-id="6869d-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="6869d-138">Firma Microsoft nie może interweniować w imieniu klienta lub bieżącego partnera.</span><span class="sxs-lookup"><span data-stu-id="6869d-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="6869d-139">Klient powinien zaplanować ścisłą pracę z przyszłymi i bieżącymi partnerami, aby zapewnić płynność przejścia.</span><span class="sxs-lookup"><span data-stu-id="6869d-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="6869d-140">Przyszłe zadania partnerskie do ukończenia</span><span class="sxs-lookup"><span data-stu-id="6869d-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="6869d-141">Przyszły partner subskrypcji musi ukończyć formularz żądania przeniesienia z Centrum partnerskiego, aby zażądać przeniesienia subskrypcji:</span><span class="sxs-lookup"><span data-stu-id="6869d-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="6869d-142">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta, który ma zostać ukończony w formularzu żądania przeniesienia w imieniu.</span><span class="sxs-lookup"><span data-stu-id="6869d-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="6869d-143">W menu Klient wybierz pozycję **subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="6869d-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="6869d-144">Wybierz sekcję **żądanie przeniesienia** .</span><span class="sxs-lookup"><span data-stu-id="6869d-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="6869d-145">W **sekcji żądanie transferu** wybierz pozycję **Dodaj nowe żądanie**.</span><span class="sxs-lookup"><span data-stu-id="6869d-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sekcja Transfers":::

5.  <span data-ttu-id="6869d-147">Wykonaj **nową formę żądania przeniesienia** .</span><span class="sxs-lookup"><span data-stu-id="6869d-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="6869d-148">Wybierz pozycję **Wyślij żądanie wysłania żądania**  >  .</span><span class="sxs-lookup"><span data-stu-id="6869d-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formularz kończenia żądania przeniesienia":::

7.  <span data-ttu-id="6869d-150">Sprawdź potwierdzenie żądania przeniesienia</span><span class="sxs-lookup"><span data-stu-id="6869d-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Przejrzyj oczekujące przeniesienie":::

    >[!Note]
    ><span data-ttu-id="6869d-152">Przyszły partner może anulować żądanie transferu, wybierając pozycję **Anuluj żądanie** w prawym górnym rogu tylko wtedy, gdy żądanie transferu ma stan "oczekiwanie".</span><span class="sxs-lookup"><span data-stu-id="6869d-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="6869d-153">Gdy żądanie transferu jest w stanie "w toku" lub "ukończone", anulowanie nie będzie możliwe.</span><span class="sxs-lookup"><span data-stu-id="6869d-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="6869d-154">Bieżące zadania partnerskie do ukończenia</span><span class="sxs-lookup"><span data-stu-id="6869d-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="6869d-155">Agent administracyjny bieżącego partnera klienta otrzyma wiadomość e-mail z prośbą o przesłanie subskrypcji przez klienta:</span><span class="sxs-lookup"><span data-stu-id="6869d-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Przegląd":::

<span data-ttu-id="6869d-157">Przejrzyj i zaakceptuj formularz żądania przeniesienia z Centrum partnerskiego, aby ukończyć transfer subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="6869d-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="6869d-158">Jeśli bieżący partner nie podejmie żadnych działań w ciągu 30 dni, żądanie wygaśnie, a w przyszłości Partner będzie musiał utworzyć nowe żądanie transferu.</span><span class="sxs-lookup"><span data-stu-id="6869d-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="6869d-159">Wybierz pozycję **Przejrzyj żądanie przeniesienia** z wiadomości e-mail lub</span><span class="sxs-lookup"><span data-stu-id="6869d-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="6869d-160">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta, w imieniu którego zostało przesłane żądanie transferu.</span><span class="sxs-lookup"><span data-stu-id="6869d-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="6869d-161">W menu Klient wybierz pozycję **subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="6869d-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="6869d-162">Wybierz sekcję **żądanie przeniesienia** .</span><span class="sxs-lookup"><span data-stu-id="6869d-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="6869d-163">Rozwiń węzeł informacje o transferze, wybierając wybrany **Identyfikator żądania transferu** w obszarze **odebrane żądania** .</span><span class="sxs-lookup"><span data-stu-id="6869d-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Żądanie transferu przeglądów źródła":::

5.  <span data-ttu-id="6869d-165">Przejrzyj żądanie transferu.</span><span class="sxs-lookup"><span data-stu-id="6869d-165">Review transfer request.</span></span> <span data-ttu-id="6869d-166">Wybierz żądane subskrypcje platformy Azure do przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="6869d-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="6869d-167">Przed kontynuowaniem Zwróć uwagę: nie będziesz już mieć dostępu do wybranych subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="6869d-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="6869d-168">Nie będzie ono zafakturowane do dalszych zastosowań.</span><span class="sxs-lookup"><span data-stu-id="6869d-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="6869d-169">Rezerwacje platformy Azure nie są transferowane w ramach subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="6869d-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="6869d-170">Następnie wybierz pozycję **Zaakceptuj i Przenieś** , aby zakończyć proces transferu.</span><span class="sxs-lookup"><span data-stu-id="6869d-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Wybierz subskrypcje do przeniesienia w ramach planów platformy Azure":::

7.  <span data-ttu-id="6869d-172">Wyświetl potwierdzenie akceptacji transferu.</span><span class="sxs-lookup"><span data-stu-id="6869d-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="6869d-173">W tym momencie przyszły partner, klient i bieżący partner będą powiadamiani o zaakceptowanym żądaniu transferu za pośrednictwem poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="6869d-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="6869d-174">Po przeprowadzeniu przejścia stan transferu może potrwać do 15 minut, podczas gdy system zostanie zaktualizowany.</span><span class="sxs-lookup"><span data-stu-id="6869d-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="6869d-175">Jeśli trwa dłużej, system będzie ponawiać próbę przez trzy dni.</span><span class="sxs-lookup"><span data-stu-id="6869d-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="6869d-176">Jeśli stan transferu nadal pozostaje w stanie oczekiwania, Partner powinien przesłać żądanie obsługi.</span><span class="sxs-lookup"><span data-stu-id="6869d-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="6869d-177">Po zakończeniu transferu subskrypcje zawarte w żądaniu będą widoczne w planie platformy Azure w przyszłości partnera i nie będą już wyświetlane.</span><span class="sxs-lookup"><span data-stu-id="6869d-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="6869d-178">W przypadku dostawców pośrednich: Powiadom pośredni odsprzedawcę o zaakceptowaniu żądania transferu.</span><span class="sxs-lookup"><span data-stu-id="6869d-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="6869d-179">Zarządzanie przetransferowanymi subskrypcjami klientów</span><span class="sxs-lookup"><span data-stu-id="6869d-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="6869d-180">Przejście nie wpływa na dostęp do istniejących użytkowników, grup lub jednostek usługi, które zostały przypisane przy użyciu kontroli dostępu na podstawie ról (RBAC) na platformie Azure.</span><span class="sxs-lookup"><span data-stu-id="6869d-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="6869d-181">Funkcja kontroli dostępu opartej na rolach [(Azure RBAC)](/azure/role-based-access-control/overview) systemu Azure pomaga klientowi zarządzać dostępem do zasobów platformy Azure, co można zrobić z tymi zasobami i jakie obszary mają do nich dostęp.</span><span class="sxs-lookup"><span data-stu-id="6869d-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="6869d-182">Nowy partner nie otrzymuje dostępu RBAC do zasobów klienta po jego przeniesieniu.</span><span class="sxs-lookup"><span data-stu-id="6869d-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="6869d-183">Poprzedni partner klienta zachowuje dostęp do kontroli dostępu RBAC.</span><span class="sxs-lookup"><span data-stu-id="6869d-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="6869d-184">Skontaktuj się z klientem, aby zrozumieć, kto ma wgląd w swoje subskrypcje i jak wprowadzać niepożądane zmiany.</span><span class="sxs-lookup"><span data-stu-id="6869d-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="6869d-185">W związku z tym ważne jest, aby klient usuwał dostęp do usługi Azure RBAC dla swojego poprzedniego partnera i mógł dodać dostęp dla nowego partnera.</span><span class="sxs-lookup"><span data-stu-id="6869d-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="6869d-186">Aby uzyskać więcej informacji na temat klienta dostarczającego nowy dostęp, zobacz [co to jest kontrola dostępu oparta na rolach (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="6869d-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="6869d-187">Aby uzyskać więcej informacji na temat usuwania przez klienta dostępu RBAC z poprzedniego partnera, zobacz [usuwanie przypisania roli](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="6869d-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="6869d-188">Ponadto nie otrzymujesz automatycznie dostępu [administratora w imieniu (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) do subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="6869d-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="6869d-189">AOBO jest konieczne, aby partner mógł zarządzać subskrypcjami platformy Azure klienta w ich imieniu.</span><span class="sxs-lookup"><span data-stu-id="6869d-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="6869d-190">Aby uzyskać więcej informacji na temat uprawnień platformy Azure, zobacz [Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="6869d-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="6869d-191">Następne kroki:</span><span class="sxs-lookup"><span data-stu-id="6869d-191">Next steps:</span></span>

- [<span data-ttu-id="6869d-192">(RBAC na platformie Azure)</span><span class="sxs-lookup"><span data-stu-id="6869d-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="6869d-193">Uzyskaj uprawnienia do zarządzania usługą lub subskrypcją klienta.</span><span class="sxs-lookup"><span data-stu-id="6869d-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
