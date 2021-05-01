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
ms.openlocfilehash: 12afa751d2e7cb6b6ef0cd7308f09746a8a43b52
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284506"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="b9498-103">Przenoszenie subskrypcji planu platformy Azure klienta do innego partnera</span><span class="sxs-lookup"><span data-stu-id="b9498-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="b9498-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="b9498-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b9498-105">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="b9498-105">Account admin</span></span>
- <span data-ttu-id="b9498-106">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="b9498-106">Sales agent</span></span>
- <span data-ttu-id="b9498-107">Agent rozliczeń</span><span class="sxs-lookup"><span data-stu-id="b9498-107">Billing agent</span></span>

<span data-ttu-id="b9498-108">W tym artykule opisano, jak klient może przełączać swoje subskrypcje platformy Azure w ramach planu platformy Azure z jednego Dostawca rozwiązań w chmurze (CSP) na inny.</span><span class="sxs-lookup"><span data-stu-id="b9498-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="b9498-109">Aby przełączyć subskrypcje platformy Azure klienta z innego partnera, wykonaj następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="b9498-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="b9498-110">Zarówno partner, jak i klient mają kroki do wykonania.</span><span class="sxs-lookup"><span data-stu-id="b9498-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="b9498-111">Tylko partnerzy z bezpośrednią relacją rozliczeń z firmą Microsoft mogą uzyskać dostęp do narzędzi przejścia.</span><span class="sxs-lookup"><span data-stu-id="b9498-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="b9498-112">Odsprzedawcy pośredni muszą współpracować z dostawcami pośrednimi, aby korzystać z tego narzędzia przejściowego.</span><span class="sxs-lookup"><span data-stu-id="b9498-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="b9498-113">Przed rozpoczęciem tego narzędzia klient musi być w rozmowie z partnerami (bieżącymi i przyszłymi).</span><span class="sxs-lookup"><span data-stu-id="b9498-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="b9498-114">Konwersacja w trybie offline musi wymagać uniknięcia nieporozumień i rezygnacji.</span><span class="sxs-lookup"><span data-stu-id="b9498-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="b9498-115">Ponadto partnerzy i klienci powinni zrozumieć te zagadnienia i wymagania wstępne przed zainicjowanie przejścia:</span><span class="sxs-lookup"><span data-stu-id="b9498-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="b9498-116">**Najważniejsze kwestie do rozważenia:**</span><span class="sxs-lookup"><span data-stu-id="b9498-116">**Key considerations:**</span></span>

- <span data-ttu-id="b9498-117">Rezerwacje platformy Azure nie zostaną przeniesiene z subskrypcją do przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="b9498-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="b9498-118">Cennik programu CSP dla usług platformy Azure w ramach bieżącego partnera nie zostanie przejściowy</span><span class="sxs-lookup"><span data-stu-id="b9498-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="b9498-119">Obowiązki pomocy technicznej dla klienta przejdą do przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="b9498-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="b9498-120">Rozliczenia i fakturowanie zostaną przeniesieni do przyszłego partnera w momencie przeniesienia</span><span class="sxs-lookup"><span data-stu-id="b9498-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="b9498-121">Transfer Role-Based Access Control nie ma wpływu na usługę Azure Role-Based Access Control (RBAC)</span><span class="sxs-lookup"><span data-stu-id="b9498-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="b9498-122">Administrator w imieniu (AOBO) nie zostanie przyznany domyślnie przyszłego partnera</span><span class="sxs-lookup"><span data-stu-id="b9498-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="b9498-123">Produkty innych firm na platformie handlowej będą transferowe, o ile produkty przejdą weryfikację uprawnień do korzystania z witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="b9498-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="b9498-124">Nie ma żadnych specjalnych rabatów ani ograniczeń regionalnych</span><span class="sxs-lookup"><span data-stu-id="b9498-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="b9498-125">Produkty nie są oparte na subskrypcji</span><span class="sxs-lookup"><span data-stu-id="b9498-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="b9498-126">Przyszły partner powinien współpracować z wydawcą, aby upewnić się, że jest na liście zezwalania na wdrożenie produktu</span><span class="sxs-lookup"><span data-stu-id="b9498-126">The future partner should work with the publisher to make sure they are on the allowlist for deployment of the product</span></span>
    - <span data-ttu-id="b9498-127">Jeśli nie wszystkie te warunki zostaną spełnione w celu przeniesienia produktów z witryny Marketplace, zostaną anulowane, subskrypcje platformy Azure zostaną przeniesione, a następnie ponownie wykup produktów z witryny Marketplace u nowego partnera</span><span class="sxs-lookup"><span data-stu-id="b9498-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="b9498-128">**Wymagania wstępne:**</span><span class="sxs-lookup"><span data-stu-id="b9498-128">**Prerequisites:**</span></span>

- <span data-ttu-id="b9498-129">Klient angażuje bieżącego partnera CSP w celu przejścia</span><span class="sxs-lookup"><span data-stu-id="b9498-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="b9498-130">Przyszły partner CSP współpracuje z klientem w celu zapewnienia, że można spełnić potrzeby klientów</span><span class="sxs-lookup"><span data-stu-id="b9498-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="b9498-131">Przyszły partner CSP ustanawia relację z klientem i kupuje plan platformy Azure przed rozpoczęciem przejścia</span><span class="sxs-lookup"><span data-stu-id="b9498-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="b9498-132">Klient musi podpisać Umowa z Klientem Microsoft z przyszłym partnerem CSP</span><span class="sxs-lookup"><span data-stu-id="b9498-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="b9498-133">Przyszły partner CSP musi mieć podpisaną Microsoft Partner Agreement, aby korzystać z tego narzędzia</span><span class="sxs-lookup"><span data-stu-id="b9498-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="b9498-134">Zadania klienta do wykonania</span><span class="sxs-lookup"><span data-stu-id="b9498-134">Customer tasks to be completed</span></span>

<span data-ttu-id="b9498-135">Aby przenieść subskrypcję platformy Azure w ramach planu platformy Azure, klient musi rozpocząć proces, kontaktując się ze swoim bieżącym partnerem.</span><span class="sxs-lookup"><span data-stu-id="b9498-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="b9498-136">Powinni zebrać nazwę firmy i domenę bieżącego partnera, aby przyszła jego partnerka może wypełnić formularz żądania przeniesienia w jego imieniu.</span><span class="sxs-lookup"><span data-stu-id="b9498-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="b9498-137">Klient musi również zidentyfikować subskrypcje, które chce przenieść od bieżącego partnera.</span><span class="sxs-lookup"><span data-stu-id="b9498-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="b9498-138">Nie można zmienić partnerów dla subskrypcji usługi Office 365, pakietu Enterprise Mobility Suite ani subskrypcji usługi Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="b9498-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="b9498-139">Przyszła odpowiedzialność partnera za ukończenie formularza żądania przeniesienia, który inicjuje proces przenoszenia.</span><span class="sxs-lookup"><span data-stu-id="b9498-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="b9498-140">Firma Microsoft nie może interweniować w imieniu klienta ani bieżącego partnera.</span><span class="sxs-lookup"><span data-stu-id="b9498-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="b9498-141">Klient powinien zaplanować ścisłą współpracę ze swoim przyszłym i bieżącym partnerem, aby przejście przebiegało bezproblemowo.</span><span class="sxs-lookup"><span data-stu-id="b9498-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="b9498-142">Przyszłe zadania partnerów do wykonania</span><span class="sxs-lookup"><span data-stu-id="b9498-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="b9498-143">Przyszły partner subskrypcji musi wypełnić formularz żądania przeniesienia od firmy Partner Center zażądać przeniesienia subskrypcji:</span><span class="sxs-lookup"><span data-stu-id="b9498-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="b9498-144">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, dla których chcesz wypełnić formularz żądania przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="b9498-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="b9498-145">W menu Customer (Klient) wybierz **pozycję Subscriptions (Subskrypcje).**</span><span class="sxs-lookup"><span data-stu-id="b9498-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="b9498-146">Wybierz **sekcję Żądanie** przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="b9498-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="b9498-147">W **sekcji Żądanie przeniesienia wybierz** pozycję **Dodaj nowe żądanie.**</span><span class="sxs-lookup"><span data-stu-id="b9498-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sekcja Transfery":::

5.  <span data-ttu-id="b9498-149">Wypełnij formularz **Nowe żądanie przeniesienia.**</span><span class="sxs-lookup"><span data-stu-id="b9498-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="b9498-150">Wybierz **pozycję Wyślij żądanie przeniesienia**  >  **Wyślij**.</span><span class="sxs-lookup"><span data-stu-id="b9498-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Wypełnij formularz żądania przeniesienia":::

7.  <span data-ttu-id="b9498-152">Przegląd potwierdzenia żądania przeniesienia</span><span class="sxs-lookup"><span data-stu-id="b9498-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Przegląd oczekującego przeniesienia":::

    >[!Note]
    ><span data-ttu-id="b9498-154">Przyszły partner może anulować żądanie przeniesienia, wybierając **pozycję** Anuluj żądanie w prawym górnym rogu tylko wtedy, gdy stan żądania przeniesienia to "oczekujące".</span><span class="sxs-lookup"><span data-stu-id="b9498-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="b9498-155">Gdy stan żądania przeniesienia będzie "w toku" lub "ukończony", anulowanie nie będzie możliwe.</span><span class="sxs-lookup"><span data-stu-id="b9498-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="b9498-156">Bieżące zadania partnerów do wykonania</span><span class="sxs-lookup"><span data-stu-id="b9498-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="b9498-157">Agent administratora bieżącego partnera klienta otrzyma wiadomość e-mail z żądaniem przeniesienia subskrypcji przez klienta:</span><span class="sxs-lookup"><span data-stu-id="b9498-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Przegląd":::

<span data-ttu-id="b9498-159">Przejrzyj i zaakceptuj formularz żądania przeniesienia od Partner Center, aby ukończyć przenoszenie subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="b9498-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="b9498-160">Jeśli bieżący partner nie zostanie podjęty w ciągu 30 dni, żądanie wygaśnie, a przyszły partner będzie miał żądanie utworzenia nowego przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="b9498-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="b9498-161">Wybierz pozycję **Przejrzyj żądanie przeniesienia w** wiadomości e-mail LUB</span><span class="sxs-lookup"><span data-stu-id="b9498-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="b9498-162">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, w imieniu których przesłano żądanie przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="b9498-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="b9498-163">W menu Customer (Klient) wybierz **pozycję Subscriptions (Subskrypcje).**</span><span class="sxs-lookup"><span data-stu-id="b9498-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="b9498-164">Wybierz **sekcję Żądanie przeniesienia.**</span><span class="sxs-lookup"><span data-stu-id="b9498-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="b9498-165">Rozwiń pozycję Transferuj informacje, wybierając **identyfikator wybranego żądania przeniesienia w** obszarze **Odebrane żądania**</span><span class="sxs-lookup"><span data-stu-id="b9498-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Żądanie przeniesienia przeglądów źródła":::

5.  <span data-ttu-id="b9498-167">Przejrzyj żądanie przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="b9498-167">Review transfer request.</span></span> <span data-ttu-id="b9498-168">Wybierz żądane subskrypcje platformy Azure do przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="b9498-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="b9498-169">Przed przystąpieniem pamiętaj: nie będziesz już mieć dostępu do wybranych subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="b9498-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="b9498-170">Dalsze użycie nie zostanie zafakturowane.</span><span class="sxs-lookup"><span data-stu-id="b9498-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="b9498-171">Rezerwacje platformy Azure nie są transferowe z subskrypcjami.</span><span class="sxs-lookup"><span data-stu-id="b9498-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="b9498-172">Następnie wybierz **pozycję Zaakceptuj i przenieś,** aby zakończyć proces transferu.</span><span class="sxs-lookup"><span data-stu-id="b9498-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Wybierz subskrypcje do przeniesienia w ramach planów platformy Azure":::

7.  <span data-ttu-id="b9498-174">Wyświetl potwierdzenie akceptacji transferu.</span><span class="sxs-lookup"><span data-stu-id="b9498-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="b9498-175">W tym momencie przyszły partner, klient i bieżący partner zostanie powiadomiony o zaakceptowanym żądaniu przeniesienia za pośrednictwem poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="b9498-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="b9498-176">Po zaakceptowaniu przeniesienia stan transferu może pozostać Oczekujący przez maksymalnie 15 minut podczas aktualizowania systemu.</span><span class="sxs-lookup"><span data-stu-id="b9498-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="b9498-177">Jeśli trwa to dłużej, system będzie próbować przez trzy dni.</span><span class="sxs-lookup"><span data-stu-id="b9498-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="b9498-178">Jeśli stan przeniesienia nadal pozostaje oczekujący, partner powinien przesłać żądanie obsługi.</span><span class="sxs-lookup"><span data-stu-id="b9498-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="b9498-179">Po zakończeniu przenoszenia subskrypcje uwzględnione w żądaniu pojawią się w planie platformy Azure przyszłego partnera i nie będą już wyświetlane.</span><span class="sxs-lookup"><span data-stu-id="b9498-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="b9498-180">W przypadku dostawców pośrednich: poinformuj odsprzedawcę pośredniego, że żądanie przeniesienia zostało zaakceptowane.</span><span class="sxs-lookup"><span data-stu-id="b9498-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="b9498-181">Zarządzanie przeniesionymi subskrypcjami klientów</span><span class="sxs-lookup"><span data-stu-id="b9498-181">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="b9498-182">Przejście nie wpływa na dostęp do istniejących użytkowników, grup lub jednostek usługi, które zostały przypisane przy użyciu kontroli dostępu na podstawie ról (RBAC) na platformie Azure.</span><span class="sxs-lookup"><span data-stu-id="b9498-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="b9498-183">Kontrola dostępu oparta na rolach [(RBAC)](/azure/role-based-access-control/overview) na platformie Azure ułatwia klientom zarządzanie tym, kto ma dostęp do zasobów platformy Azure, co może zrobić z tymi zasobami i do jakich obszarów ma dostęp.</span><span class="sxs-lookup"><span data-stu-id="b9498-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="b9498-184">Jako nowy partner nie masz dostępu RBAC do zasobów klienta po przeniesieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="b9498-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="b9498-185">Poprzedni partner klienta zachowuje dostęp RBAC.</span><span class="sxs-lookup"><span data-stu-id="b9498-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="b9498-186">We współpracy z klientem dowiedz się, kto ma wgląd w swoje subskrypcje i jak wprowadzać dowolne zmiany.</span><span class="sxs-lookup"><span data-stu-id="b9498-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="b9498-187">W związku z tym ważne jest, aby klient usuał dostęp RBAC platformy Azure dla poprzedniego partnera i dodał dostęp dla nowego partnera.</span><span class="sxs-lookup"><span data-stu-id="b9498-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="b9498-188">Aby uzyskać więcej informacji na temat nowego dostępu klienta, zobacz Co to jest kontrola dostępu na podstawie ról [(RBAC) platformy Azure?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="b9498-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="b9498-189">Aby uzyskać więcej informacji na temat usuwania dostępu RBAC poprzedniego partnera przez klienta, zobacz [Usuwanie przypisania roli](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="b9498-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="b9498-190">Ponadto nie uzyskujesz automatycznie dostępu [administratora w imieniu (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) do subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="b9498-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="b9498-191">AOBO jest niezbędne, aby partner zarządzał subskrypcjami platformy Azure swoich klientów w ich imieniu.</span><span class="sxs-lookup"><span data-stu-id="b9498-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="b9498-192">Aby uzyskać więcej informacji na temat uprawnień platformy Azure, zobacz Uzyskiwanie uprawnień do zarządzania [usługą lub subskrypcją klienta.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="b9498-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9498-193">Następne kroki:</span><span class="sxs-lookup"><span data-stu-id="b9498-193">Next steps:</span></span>

- [<span data-ttu-id="b9498-194">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="b9498-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="b9498-195">Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta.</span><span class="sxs-lookup"><span data-stu-id="b9498-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
