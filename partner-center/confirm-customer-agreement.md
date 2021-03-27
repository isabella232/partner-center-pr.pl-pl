---
title: Jak potwierdzić, że klient zaakceptował umowę klienta firmy Microsoft do programu CSP
description: Partnerzy dostawcy rozwiązań w chmurze (CSP) muszą potwierdzić akceptację przez klienta umowy klienta firmy Microsoft przed zamawianiem usług firmy Microsoft dla klientów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633782"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="d353b-103">Jak potwierdzić, że klient zaakceptował umowę klienta firmy Microsoft do programu CSP</span><span class="sxs-lookup"><span data-stu-id="d353b-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="d353b-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="d353b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d353b-105">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="d353b-105">Admin agent</span></span>
- <span data-ttu-id="d353b-106">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="d353b-106">Sales agent</span></span>


<span data-ttu-id="d353b-107">Klienci mogą korzystać z dwóch opcji zaakceptowania umowy klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="d353b-108">**Opcja 1**: zaświadczanie partnera dotyczącego akceptacji przez klienta może potwierdzić akceptację klienta przy użyciu interfejsu API/zestawu SDK Centrum partnerskiego lub pulpitu nawigacyjnego Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="d353b-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="d353b-109">**Opcja 2**: klient bezpośredni akceptacji — partner może zaprosić klienta za pośrednictwem adresu URL w celu przejrzenia i zaakceptowania umowy w centrum administracyjnym Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="d353b-110">Dostęp do szablonu umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="d353b-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="d353b-111">Możesz ręcznie pobrać najnowszą wersję szablonu umowy klienta firmy Microsoft z tego [miejsca](https://aka.ms/customeragreement).</span><span class="sxs-lookup"><span data-stu-id="d353b-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="d353b-112">Umowa dla klientów firmy Microsoft jest specyficzna dla kraju.</span><span class="sxs-lookup"><span data-stu-id="d353b-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="d353b-113">Podczas żądania szablonu umowy klienta firmy Microsoft upewnij się, że wybrano właściwy kraj na podstawie lokalizacji klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="d353b-114">Opcja 1: potwierdzenie akceptacji przez klienta w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="d353b-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="d353b-115">Bezpośredni partnerzy Bill mogą potwierdzić akceptację klienta umowy klienta firmy Microsoft w centrum partnerskim dla nowych i istniejących klientów.</span><span class="sxs-lookup"><span data-stu-id="d353b-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="d353b-116">Pośredni odsprzedawcy nie mogą zaświadczać swoich klientów i muszą współpracować z dostawcami pośrednimi w celu uzyskania zaświadczania.</span><span class="sxs-lookup"><span data-stu-id="d353b-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="d353b-117">Potwierdź akceptację klienta dla nowych klientów</span><span class="sxs-lookup"><span data-stu-id="d353b-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="d353b-118">Podczas tworzenia nowej dzierżawy klienta w centrum partnerskim wykonaj następujące kroki, aby potwierdzić akceptację umowy klienta firmy Microsoft przez klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d353b-119">Aby wykonać te kroki, musisz być agentem administracyjnym lub agentem sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="d353b-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="d353b-120">Wybierz pozycję **klienci**, a następnie **Nowy klient**.</span><span class="sxs-lookup"><span data-stu-id="d353b-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="d353b-121">W obszarze **Informacje o koncie** wprowadź informacje dotyczące firmy i jej głównej osoby kontaktowej.</span><span class="sxs-lookup"><span data-stu-id="d353b-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="d353b-122">W obszarze **Umowa Microsoft** wybierz pole, aby zatwierdzić, że klient zaakceptował umowę klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="d353b-123">W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="d353b-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d353b-124">Nie można ustawić tej wartości na datę przyszłą.</span><span class="sxs-lookup"><span data-stu-id="d353b-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="d353b-125">Upewnij się, że wyświetlane informacje kontaktowe użytkownika podstawowego są poprawne.</span><span class="sxs-lookup"><span data-stu-id="d353b-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="d353b-126">Jeśli jest to nieprawidłowe, wybierz pozycję **Aktualizuj** i wprowadź dokładne informacje dla osoby, która zaakceptował umowę.</span><span class="sxs-lookup"><span data-stu-id="d353b-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="d353b-127">Wybierz pozycję **dalej** , aby kontynuować tworzenie dzierżawy klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nowy klient":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="d353b-129">Potwierdzenie akceptacji przez klienta dla istniejących klientów</span><span class="sxs-lookup"><span data-stu-id="d353b-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="d353b-130">Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży:</span><span class="sxs-lookup"><span data-stu-id="d353b-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="d353b-131">Wybierz pozycję **Klienci**.</span><span class="sxs-lookup"><span data-stu-id="d353b-131">Select **Customers**.</span></span> <span data-ttu-id="d353b-132">Znajdź i wybierz klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-132">Find and select the customer.</span></span>

2. <span data-ttu-id="d353b-133">Wybierz pozycję **Informacje o koncie**.</span><span class="sxs-lookup"><span data-stu-id="d353b-133">Select **Account info**.</span></span>

3. <span data-ttu-id="d353b-134">W obszarze **Umowa klienta firmy Microsoft** wybierz pozycję **Aktualizuj**.</span><span class="sxs-lookup"><span data-stu-id="d353b-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="d353b-135">Wprowadź **imię** i **nazwisko, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) osoby, która zaakceptował umowę.</span><span class="sxs-lookup"><span data-stu-id="d353b-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="d353b-136">W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="d353b-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d353b-137">Nie można ustawić tej wartości na datę przyszłą.</span><span class="sxs-lookup"><span data-stu-id="d353b-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="d353b-138">Wybierz pozycję **Zapisz** i Kontynuuj.</span><span class="sxs-lookup"><span data-stu-id="d353b-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Istniejący klient":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="d353b-140">Pobierz potwierdzenie akceptacji klienta</span><span class="sxs-lookup"><span data-stu-id="d353b-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="d353b-141">Aby uzyskać potwierdzenie, że istniejący klient zaakceptował umowę klienta firmy Microsoft, wykonaj następujące czynności.</span><span class="sxs-lookup"><span data-stu-id="d353b-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="d353b-142">Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="d353b-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d353b-143">Wybierz pozycję **klienci**, a następnie Znajdź i wybierz klienta, który ma zostać wyświetlony.</span><span class="sxs-lookup"><span data-stu-id="d353b-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="d353b-144">Wybierz pozycję **Informacje o koncie**.</span><span class="sxs-lookup"><span data-stu-id="d353b-144">Select **Account info**.</span></span>

3. <span data-ttu-id="d353b-145">W obszarze **Umowa klienta firmy Microsoft** Sprawdź, czy jest to potwierdzenie czy nie zostało dostarczone przez tego klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="d353b-146">Potwierdzenie akceptacji klienta przy użyciu interfejsu API/zestawu SDK Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="d353b-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="d353b-147">Za pomocą interfejsu API/zestawu SDK Centrum partnerskiego można potwierdzić akceptację umowy klienta firmy Microsoft przez klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d353b-148">Aby uzyskać szczegółowe informacje na temat interfejsu API/SDK, zobacz:</span><span class="sxs-lookup"><span data-stu-id="d353b-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="d353b-149">Pobieranie metadanych umowy dla umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="d353b-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="d353b-150">Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="d353b-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="d353b-151">Pobieranie potwierdzenia akceptacji przez klienta umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="d353b-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="d353b-152">Pobierz link do pobierania dla szablonu umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="d353b-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="d353b-153">Opcja 2: akceptacja klienta w centrum administracyjnym Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d353b-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="d353b-154">Partnerzy mogą zapraszać nowych i istniejących klientów za pośrednictwem adresu URL, aby przejrzeć i zaakceptować umowę w centrum administracyjnym Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="d353b-155">W następnych sekcjach pokazano, jak:</span><span class="sxs-lookup"><span data-stu-id="d353b-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="d353b-156">Utwórz nowego klienta i zaproś klienta o sprawdzenie i zaakceptowanie umowy.</span><span class="sxs-lookup"><span data-stu-id="d353b-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="d353b-157">Zaproś nowego klienta o sprawdzenie i zaakceptowanie relacji odsprzedawcy oraz umowy.</span><span class="sxs-lookup"><span data-stu-id="d353b-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="d353b-158">Zaproś istniejącego klienta o sprawdzenie i zaakceptowanie umowy.</span><span class="sxs-lookup"><span data-stu-id="d353b-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="d353b-159">Możesz użyć [interfejsu API/SDK Centrum partnerskiego](/partner-center/develop/get-direct-sign-status-of-customer-agreement) , aby uzyskać stan bezpośredniej akceptacji umowy klienta firmy Microsoft przez klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="d353b-160">Utwórz nowego klienta i zaproś klienta o sprawdzenie i zaakceptowanie umowy</span><span class="sxs-lookup"><span data-stu-id="d353b-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="d353b-161">Wykonaj następujące kroki, aby utworzyć nowego klienta w centrum partnerskim, a następnie Zaproś go o sprawdzenie i zaakceptowanie umowy klienta firmy Microsoft w centrum administracyjnym Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="d353b-162">Na karcie **klienci** w centrum partnerskim wybierz pozycję **Dodaj klienta**.</span><span class="sxs-lookup"><span data-stu-id="d353b-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="d353b-163">W obszarze **Informacje o koncie** wprowadź informacje o nowym kliencie we wszystkich wymaganych polach, w tym nazwę firmy klienta i kontakt podstawowy.</span><span class="sxs-lookup"><span data-stu-id="d353b-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="d353b-164">W obszarze **Umowa klienta** wybierz pozycję **klient z prośbą o zaakceptowanie umowy klienta firmy Microsoft w centrum administracyjnym Microsoft 365**.</span><span class="sxs-lookup"><span data-stu-id="d353b-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="d353b-165">Wypełnij wszystkie inne wymagane pola na stronie.</span><span class="sxs-lookup"><span data-stu-id="d353b-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="d353b-166">Wybierz pozycję **Dalej: Przejrzyj** następnie kontynuuj kroki, aby utworzyć dzierżawę klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="d353b-167">Nowi klienci nie mogą dokonać zakupu, dopóki nie zaakceptują umowy klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Utwórz nowego klienta":::

5. <span data-ttu-id="d353b-169">Po dojściu do ekranu **potwierdzenia** w nowym przepływie pracy klienta Zapisz poświadczenia klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="d353b-170">Musisz podać te poświadczenia klientom później.</span><span class="sxs-lookup"><span data-stu-id="d353b-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="d353b-171">Na zewnątrz Centrum partnerskiego Utwórz i Wyślij wiadomość e-mail z zaproszeniem klienta, aby zatwierdzić umowę klienta firmy Microsoft w centrum administracyjnym Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="d353b-172">Upewnij się, że te elementy zostały uwzględnione w wiadomości e-mail:</span><span class="sxs-lookup"><span data-stu-id="d353b-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="d353b-173">Link do tego [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (wymagane logowanie)</span><span class="sxs-lookup"><span data-stu-id="d353b-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="d353b-174">Poświadczenia klienta zapisane w kroku 5.</span><span class="sxs-lookup"><span data-stu-id="d353b-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="d353b-175">Klient otrzyma wiadomość e-mail z zaproszeniem od partnera i wybierze [adres URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="d353b-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="d353b-176">Klient loguje się do centrum administracyjnego Microsoft 365 przy użyciu podanych poświadczeń klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="d353b-177">Klient sprawdza pole, aby zaakceptować umowę klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="d353b-178">Zaproś nowego klienta o sprawdzenie i zaakceptowanie relacji odsprzedawcy oraz umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="d353b-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="d353b-179">Wykonaj następujące kroki, aby zaprosić nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy oraz umowy klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="d353b-180">Na karcie **klienci** w centrum partnerskim wybierz pozycję **Żądaj linku relacji odsprzedawcy** .</span><span class="sxs-lookup"><span data-stu-id="d353b-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="d353b-181">Zostanie wygenerowany automatyczny szablon wiadomości e-mail, w tym tekst i sparametryzowany adres URL kierujący klienta do centrum administracyjnego Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="d353b-182">Można dostosować automatycznie wygenerowany szablon wiadomości e-mail, a następnie wybrać opcję **Kopiuj do schowka** lub **otworzyć w wiadomości e-mail**.</span><span class="sxs-lookup"><span data-stu-id="d353b-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="d353b-183">Ten szablon wiadomości e-mail zaprasza klienta, aby akceptował żądanie dotyczące **relacji odsprzedawcy** oraz **umowę klienta firmy Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="d353b-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="d353b-184">(Uwaga: w wiadomości e-mail z zaproszeniem upewnij się, że partner zawiera również adres URL, który został podany automatycznie, oraz poświadczenia klienta, które zostały ostatnio utworzone).</span><span class="sxs-lookup"><span data-stu-id="d353b-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Utwórz relację":::

5. <span data-ttu-id="d353b-186">Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika sparametryzowany adres URL.</span><span class="sxs-lookup"><span data-stu-id="d353b-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="d353b-187">Klient korzysta z poświadczeń podanych w wiadomości e-mail w celu zalogowania się do centrum administracyjnego Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="d353b-188">Klient sprawdza pole, aby zaakceptować **relację odsprzedawcy** oraz **umowę klienta firmy Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="d353b-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="d353b-189">W ramach tego samego adresu URL klient może zobaczyć skonsolidowaną listę różnych partnerów, z którymi pracują.</span><span class="sxs-lookup"><span data-stu-id="d353b-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="d353b-190">Mogą wybrać partnera, aby wyświetlić szczegóły.</span><span class="sxs-lookup"><span data-stu-id="d353b-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Zaakceptowanie umowy":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="d353b-192">Zaproś istniejącego klienta o sprawdzenie i zaakceptowanie umowy</span><span class="sxs-lookup"><span data-stu-id="d353b-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="d353b-193">Wykonaj następujące kroki, aby zaprosić istniejącego klienta do przejrzenia i zaakceptowania umowy klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="d353b-194">Utwórz adres e-mail klienta z osadzonym adresem URL, który zaprasza klienta, aby zaakceptował umowę klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="d353b-195">Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika [adres URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="d353b-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="d353b-196">Klient wprowadza swoje poświadczenia do centrum administracyjnego Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="d353b-197">Klient sprawdza pole, aby zaakceptować umowę klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="d353b-198">W ramach tego samego adresu URL klient może zobaczyć skonsolidowaną listę różnych partnerów, z którymi pracują.</span><span class="sxs-lookup"><span data-stu-id="d353b-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="d353b-199">Mogą wybrać partnera, aby wyświetlić szczegóły.</span><span class="sxs-lookup"><span data-stu-id="d353b-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Dział":::

>[!NOTE]
><span data-ttu-id="d353b-201">W niektórych scenariuszach klienci mogą nie być w stanie bezpośrednio zaakceptować umowy klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d353b-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d353b-202">Aby dowiedzieć się więcej na temat tych sytuacji, przeczytaj dwa scenariusze, w których musisz zalogować się w imieniu klienta poniżej.</span><span class="sxs-lookup"><span data-stu-id="d353b-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="d353b-203">Dwa scenariusze, w których należy zaświadczać o swoim imieniu klienta</span><span class="sxs-lookup"><span data-stu-id="d353b-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="d353b-204">Istnieją dwa scenariusze, w których klienci mogą nie być w stanie bezpośrednio zaakceptować umowy klienta firmy Microsoft w centrum administracyjnym Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d353b-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="d353b-205">**Scenariusz 1**: istniejący klient kupił dowolne z następujących elementów za pomocą istniejącej relacji partnera: oferty, oprogramowania lub subskrypcji oprogramowania, wystąpień zarezerwowanych lub planu platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="d353b-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="d353b-206">Klient próbuje teraz dokonać nowego zakupu (z wyjątkiem autoodnawiania).</span><span class="sxs-lookup"><span data-stu-id="d353b-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="d353b-207">Gdy klient kliknie ten adres URL, otrzyma komunikat "Skontaktuj się z partnerem w celu potwierdzenia akceptacji umowy klienta firmy Microsoft".</span><span class="sxs-lookup"><span data-stu-id="d353b-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="d353b-208">**Aby rozwiązać ten problem**: należy zaświadczać o imieniu klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Zrzut ekranu przedstawiający stronę centrum administracyjnego Microsoft 365 z prośbą o skontaktowanie się z partnerem w celu potwierdzenia akceptacji umowy klienta firmy Microsoft.":::

<span data-ttu-id="d353b-210">**Scenariusz 2**. istniejący klient zakupił jedną z następujących ofert, subskrypcji oprogramowania i oprogramowania, wystąpień zarezerwowanych oraz planu platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="d353b-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="d353b-211">Klient podejmie teraz próbę dokonania nowego zakupu u nowego partnera.</span><span class="sxs-lookup"><span data-stu-id="d353b-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="d353b-212">Gdy klient kliknie adres URL, aby Microsoft 365 centrum administracyjnego w celu zaakceptowania nowej relacji partnera i umowy, otrzyma komunikat "Skontaktuj się z partnerem w celu potwierdzenia akceptacji umowy klienta firmy Microsoft".</span><span class="sxs-lookup"><span data-stu-id="d353b-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="d353b-213">**Aby rozwiązać ten problem**: należy zaświadczać o imieniu klienta.</span><span class="sxs-lookup"><span data-stu-id="d353b-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="d353b-214">Potwierdź, że klient zaakceptował umowę</span><span class="sxs-lookup"><span data-stu-id="d353b-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="d353b-215">Jeśli spróbujesz utworzyć nowe zamówienie dla istniejącego klienta, który nie został wcześniej potwierdzony, zostanie wyświetlony monit o ukończenie potwierdzenia.</span><span class="sxs-lookup"><span data-stu-id="d353b-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="d353b-216">Użyj poniższej procedury w tym celu.</span><span class="sxs-lookup"><span data-stu-id="d353b-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="d353b-217">Wprowadź **imię** **, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) użytkownika, który zaakceptował umowę.</span><span class="sxs-lookup"><span data-stu-id="d353b-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="d353b-218">W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="d353b-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d353b-219">Nie można ustawić tej wartości na datę przyszłą.</span><span class="sxs-lookup"><span data-stu-id="d353b-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="d353b-220">Wybierz przycisk **Zapisz i kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="d353b-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="d353b-221">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="d353b-221">Next steps</span></span>

- [<span data-ttu-id="d353b-222">Weryfikowanie lub aktualizowanie informacji o profilu firmy</span><span class="sxs-lookup"><span data-stu-id="d353b-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="d353b-223">Umowy z Klientem Microsoft (według regionu, języka)</span><span class="sxs-lookup"><span data-stu-id="d353b-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
