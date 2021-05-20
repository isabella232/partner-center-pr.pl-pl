---
title: Jak potwierdzić, że klient zaakceptował Umowa z Klientem Microsoft programu CSP
description: Dostawca rozwiązań w chmurze (CSP) partnerzy muszą potwierdzić akceptację przez klienta Umowa z Klientem Microsoft przed zamówieniem usługi firmy Microsoft dla klientów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: c75f129ae5a0755833462138f60901cc7ff36732
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148520"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="5cc32-103">Jak potwierdzić, że klient zaakceptował Umowa z Klientem Microsoft programu CSP</span><span class="sxs-lookup"><span data-stu-id="5cc32-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="5cc32-104">**Odpowiednie role:** Agent administracyjny | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="5cc32-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="5cc32-105">Klienci mają dwie opcje dotyczące sposobu akceptowania Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="5cc32-106">**Opcja 1:** Potwierdzenie akceptacji klienta przez partnera — partner może potwierdzić akceptację klienta przy użyciu interfejsu API lub zestawu SDK Partner Center lub za pośrednictwem pulpitu Partner Center nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="5cc32-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="5cc32-107">**Opcja 2:** Akceptacja bezpośrednia klienta — partner może zaprosić klienta za pośrednictwem adresu URL w celu przejrzenia i zaakceptowania umowy w Microsoft 365 Administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="5cc32-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="5cc32-108">Szablon Umowa z Klientem Microsoft dostępu</span><span class="sxs-lookup"><span data-stu-id="5cc32-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="5cc32-109">Najnowszą wersję szablonu aplikacji można pobrać ręcznie Umowa z Klientem Microsoft [tutaj.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="5cc32-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="5cc32-110">Ta Umowa z Klientem Microsoft jest specyficzna dla kraju.</span><span class="sxs-lookup"><span data-stu-id="5cc32-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="5cc32-111">Podczas żądania Umowa z Klientem Microsoft szablonu należy wybrać właściwy kraj na podstawie lokalizacji klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="5cc32-112">Opcja 1. Potwierdzanie akceptacji przez klientów w Partner Center</span><span class="sxs-lookup"><span data-stu-id="5cc32-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="5cc32-113">Partnerzy rozliczani bezpośrednio mogą potwierdzić akceptację klientów Umowa z Klientem Microsoft w Partner Center dla nowych i istniejących klientów.</span><span class="sxs-lookup"><span data-stu-id="5cc32-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="5cc32-114">Odsprzedawcy pośredni nie mogą poświadczać w imieniu swoich klientów i muszą współpracować ze swoim dostawcą pośrednim, aby uzyskać ukończone zaświadczenia.</span><span class="sxs-lookup"><span data-stu-id="5cc32-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="5cc32-115">Potwierdzanie akceptacji przez klientów dla nowych klientów</span><span class="sxs-lookup"><span data-stu-id="5cc32-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="5cc32-116">Podczas tworzenia nowej dzierżawy klienta w Partner Center, należy wykonać następujące kroki, aby potwierdzić akceptację Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="5cc32-117">Aby wykonać te kroki, musisz być agentem administracyjnym lub agentem sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="5cc32-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="5cc32-118">Wybierz **pozycję Klienci,** a następnie **pozycję Nowy klient.**</span><span class="sxs-lookup"><span data-stu-id="5cc32-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="5cc32-119">W **obszarze Informacje o** koncie wprowadź informacje dotyczące firmy i jej głównej osoby kontaktowej.</span><span class="sxs-lookup"><span data-stu-id="5cc32-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="5cc32-120">W **ramach umowy firmy Microsoft** zaznacz pole wyboru, aby zaświadczyć, że klient zaakceptował Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="5cc32-121">W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5cc32-122">Nie można ustawić tej daty na przyszłą datę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="5cc32-123">Upewnij się, że wyświetlane informacje kontaktowe użytkownika podstawowego są poprawne.</span><span class="sxs-lookup"><span data-stu-id="5cc32-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="5cc32-124">Jeśli jest niepoprawna, wybierz pozycję **Aktualizuj** i wprowadź dokładne informacje dotyczące osoby, która zaakceptowała umowę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="5cc32-125">Wybierz **przycisk Dalej,** aby kontynuować tworzenie dzierżawy klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nowy klient":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="5cc32-127">Potwierdzanie akceptacji przez klientów dla istniejących klientów</span><span class="sxs-lookup"><span data-stu-id="5cc32-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="5cc32-128">Aby to zrobić, musisz być agentem administratora lub agentem sprzedaży:</span><span class="sxs-lookup"><span data-stu-id="5cc32-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="5cc32-129">Wybierz pozycję **Klienci**.</span><span class="sxs-lookup"><span data-stu-id="5cc32-129">Select **Customers**.</span></span> <span data-ttu-id="5cc32-130">Znajdź i wybierz klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-130">Find and select the customer.</span></span>

2. <span data-ttu-id="5cc32-131">Wybierz **pozycję Informacje o koncie.**</span><span class="sxs-lookup"><span data-stu-id="5cc32-131">Select **Account info**.</span></span>

3. <span data-ttu-id="5cc32-132">W **Umowa z Klientem Microsoft** wybierz pozycję **Zaktualizuj**.</span><span class="sxs-lookup"><span data-stu-id="5cc32-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="5cc32-133">Wprowadź **imię,** **nazwisko,** adres **e-mail** i numer telefonu  (opcjonalnie) osoby, która zaakceptowała umowę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="5cc32-134">W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5cc32-135">Nie można ustawić tej daty na przyszłą datę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="5cc32-136">Wybierz **pozycję Zapisz** i kontynuuj.</span><span class="sxs-lookup"><span data-stu-id="5cc32-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Istniejący klient":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="5cc32-138">Pobieranie potwierdzenia akceptacji przez klienta</span><span class="sxs-lookup"><span data-stu-id="5cc32-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="5cc32-139">Aby pobrać potwierdzenie, że istniejący klient zaakceptował Umowa z Klientem Microsoft, należy wykonać następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="5cc32-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="5cc32-140">Aby to zrobić, musisz być agentem administratora lub agentem sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="5cc32-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5cc32-141">Wybierz **pozycję Klienci,** a następnie znajdź i wybierz klienta, którego chcesz wyświetlić.</span><span class="sxs-lookup"><span data-stu-id="5cc32-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="5cc32-142">Wybierz **pozycję Informacje o koncie.**</span><span class="sxs-lookup"><span data-stu-id="5cc32-142">Select **Account info**.</span></span>

3. <span data-ttu-id="5cc32-143">W **ramach umowy klienta firmy Microsoft** sprawdź, czy potwierdzenie nie zostało dostarczone przez tego klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="5cc32-144">Potwierdzanie akceptacji przez klientów przy użyciu Partner Center API/SDK</span><span class="sxs-lookup"><span data-stu-id="5cc32-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="5cc32-145">Możesz użyć Partner Center API/zestawu SDK, aby potwierdzić akceptację przez klienta Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="5cc32-146">Aby uzyskać szczegółowe informacje na temat interfejsu API/zestawu SDK, zobacz:</span><span class="sxs-lookup"><span data-stu-id="5cc32-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="5cc32-147">Pobieranie metadanych umowy dla umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="5cc32-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="5cc32-148">Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="5cc32-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="5cc32-149">Pobieranie potwierdzenia akceptacji przez klienta umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="5cc32-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="5cc32-150">Uzyskiwanie linku pobierania dla szablonu Umowa z Klientem Microsoft szablonu</span><span class="sxs-lookup"><span data-stu-id="5cc32-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="5cc32-151">Opcja 2. Akceptacja klienta w Microsoft 365 administracyjnym</span><span class="sxs-lookup"><span data-stu-id="5cc32-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="5cc32-152">Partnerzy mogą zapraszać nowych i istniejących klientów za pośrednictwem adresu URL do przejrzenia i zaakceptowania umowy w Microsoft 365 Administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="5cc32-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="5cc32-153">W kilku następnych sekcjach podano, jak:</span><span class="sxs-lookup"><span data-stu-id="5cc32-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="5cc32-154">Utwórz nowego klienta i zaproś go do przejrzenia i zaakceptowania umowy.</span><span class="sxs-lookup"><span data-stu-id="5cc32-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="5cc32-155">Zaproś nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i umowy.</span><span class="sxs-lookup"><span data-stu-id="5cc32-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="5cc32-156">Zaproś istniejącego klienta do przejrzenia i zaakceptowania umowy.</span><span class="sxs-lookup"><span data-stu-id="5cc32-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="5cc32-157">Możesz użyć [Partner Center API/zestawu SDK,](/partner-center/develop/get-direct-sign-status-of-customer-agreement) aby uzyskać stan bezpośredniej akceptacji klienta dla Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="5cc32-158">Tworzenie nowego klienta i zapraszanie go do przejrzenia i zaakceptowania umowy</span><span class="sxs-lookup"><span data-stu-id="5cc32-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="5cc32-159">Użyj poniższych kroków, aby utworzyć nowego klienta w Partner Center następnie zaprosić go do przejrzenia i zaakceptowania Umowa z Klientem Microsoft w Microsoft 365 administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="5cc32-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="5cc32-160">Na karcie **Customers (Klienci)** w Partner Center wybierz **pozycję Add customer (Dodaj klienta).**</span><span class="sxs-lookup"><span data-stu-id="5cc32-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="5cc32-161">W **obszarze Informacje o** koncie wprowadź informacje o nowym kliencie we wszystkich wymaganych polach, w tym nazwę firmy klienta i podstawowy kontakt.</span><span class="sxs-lookup"><span data-stu-id="5cc32-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="5cc32-162">W **obszarze Umowa z** Klientem wybierz pozycję Klient zostanie poproszony o **zaakceptowanie Umowa z Klientem Microsoft w Microsoft 365 administracyjnym.**</span><span class="sxs-lookup"><span data-stu-id="5cc32-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="5cc32-163">Wypełnij wszystkie inne wymagane pola na stronie.</span><span class="sxs-lookup"><span data-stu-id="5cc32-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="5cc32-164">Wybierz **pozycję Dalej: Przejrzyj,** a następnie kontynuuj kroki tworzenia dzierżawy klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="5cc32-165">Nowi klienci nie mogą dokonać zakupu, dopóki nie zaakceptują Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Tworzenie nowego klienta":::

5. <span data-ttu-id="5cc32-167">Po osiągnięciu ekranu **Potwierdzenie** w przepływie pracy nowego klienta zapisz poświadczenia klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="5cc32-168">Te poświadczenia trzeba będzie przekazać później klientowi.</span><span class="sxs-lookup"><span data-stu-id="5cc32-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="5cc32-169">Poza Partner Center utwórz i wyślij wiadomość e-mail z zaproszeniem klienta do zaakceptowania Umowa z Klientem Microsoft w Microsoft 365 Administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="5cc32-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="5cc32-170">Pamiętaj, aby uwzględnić następujące elementy w wiadomości e-mail:</span><span class="sxs-lookup"><span data-stu-id="5cc32-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="5cc32-171">Link do tego adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (wymagane jest zalogowanie)</span><span class="sxs-lookup"><span data-stu-id="5cc32-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="5cc32-172">Poświadczenia klienta zapisane w kroku 5.</span><span class="sxs-lookup"><span data-stu-id="5cc32-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="5cc32-173">Klient otrzyma wiadomość e-mail z zaproszeniem od partnera i wybierze adres [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="5cc32-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="5cc32-174">Klient logowania się Microsoft 365 administracyjnym przy użyciu podanych poświadczeń klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="5cc32-175">Klient sprawdza to pole, aby zaakceptować umowę klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="5cc32-176">Zaproś nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i Umowa z Klientem Microsoft</span><span class="sxs-lookup"><span data-stu-id="5cc32-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="5cc32-177">Użyj poniższych kroków, aby zaprosić nowego klienta do przejrzenia i zaakceptowania relacji odsprzedawcy i Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="5cc32-178">Na karcie **Customers (Klienci)** w Partner Center wybierz link **Request a reseller relationship (Zażądaj relacji odsprzedawcy).**</span><span class="sxs-lookup"><span data-stu-id="5cc32-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="5cc32-179">Zostanie wygenerowany automatyczny szablon wiadomości e-mail, w tym tekst i sparametryzowane adresy URL, które kierują klienta do centrum Microsoft 365 administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="5cc32-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="5cc32-180">Możesz dostosować automatycznie wygenerowany szablon wiadomości e-mail, a następnie wybrać pozycję **Kopiuj do schowka** lub **Otwórz w wiadomości e-mail.**</span><span class="sxs-lookup"><span data-stu-id="5cc32-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="5cc32-181">Użyj tego szablonu wiadomości e-mail, aby zaprosić klienta do **zaakceptowania** żądania relacji odsprzedawcy **i Umowa z Klientem Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="5cc32-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="5cc32-182">(Uwaga: w wiadomości e-mail z zaproszeniem upewnij się, że partner zawiera również adres URL, który został automatycznie podany, a także poświadczenia klienta, które zostały ostatnio utworzone).</span><span class="sxs-lookup"><span data-stu-id="5cc32-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="tworzenie relacji":::

5. <span data-ttu-id="5cc32-184">Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika sparametryzowane adresy URL.</span><span class="sxs-lookup"><span data-stu-id="5cc32-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="5cc32-185">Klient używa poświadczeń podanych w wiadomości e-mail, aby zalogować się Microsoft 365 Centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="5cc32-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="5cc32-186">Klient sprawdza pole wyboru, aby zaakceptować relację **odsprzedawcy** **i Umowa z Klientem Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="5cc32-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="5cc32-187">W ramach tego samego adresu URL klient może wyświetlić skonsolidowaną listę różnych partnerów, z których pracuje.</span><span class="sxs-lookup"><span data-stu-id="5cc32-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="5cc32-188">Może wybrać partnera, aby wyświetlić szczegóły.</span><span class="sxs-lookup"><span data-stu-id="5cc32-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Zaakceptowanie umowy":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="5cc32-190">Zapraszanie istniejącego klienta do przejrzenia i zaakceptowania umowy</span><span class="sxs-lookup"><span data-stu-id="5cc32-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="5cc32-191">Skorzystaj z poniższych kroków, aby zaprosić istniejącego klienta do przejrzenia i zaakceptowania Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="5cc32-192">Utwórz wiadomość e-mail klienta z osadzonym adresem URL z zaproszeniem klienta do zaakceptowania Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="5cc32-193">Klient otrzymuje zaproszenie za pośrednictwem poczty e-mail i klika [adres URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="5cc32-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="5cc32-194">Klient wprowadza swoje poświadczenia w Microsoft 365 Administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="5cc32-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="5cc32-195">Klient sprawdza to pole, aby zaakceptować Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="5cc32-196">Pod tym samym adresem URL klient może zobaczyć skonsolidowaną listę różnych partnerów, z których pracuje.</span><span class="sxs-lookup"><span data-stu-id="5cc32-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="5cc32-197">Może wybrać partnera, aby wyświetlić szczegóły.</span><span class="sxs-lookup"><span data-stu-id="5cc32-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Klienta":::

>[!NOTE]
><span data-ttu-id="5cc32-199">W niektórych scenariuszach klienci mogą nie być w stanie bezpośrednio zaakceptować Umowa z Klientem Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cc32-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="5cc32-200">Aby dowiedzieć się więcej na temat tych sytuacji, przeczytaj dwa scenariusze, w których musisz zaświadczyć w imieniu klienta, poniżej.</span><span class="sxs-lookup"><span data-stu-id="5cc32-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="5cc32-201">Dwa scenariusze, w których musisz zaświadczyć w imieniu klienta</span><span class="sxs-lookup"><span data-stu-id="5cc32-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="5cc32-202">Istnieją dwa scenariusze, w których klienci mogą nie być w stanie bezpośrednio zaakceptować Umowa z Klientem Microsoft w Microsoft 365 administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="5cc32-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="5cc32-203">**Scenariusz 1.** Istniejący klient kupił dowolne z następujących produktów w ramach istniejącej relacji partnerskiej: oferty, subskrypcje oprogramowania lub oprogramowania, wystąpienia zarezerwowane lub plan platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="5cc32-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="5cc32-204">Klient próbuje teraz dokonać nowego zakupu (z wyjątkiem automatycznego odnawiania).</span><span class="sxs-lookup"><span data-stu-id="5cc32-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="5cc32-205">Gdy klient kliknie adres URL, otrzyma komunikat "Skontaktuj się z partnerem, aby potwierdzić akceptację Umowa z Klientem Microsoft".</span><span class="sxs-lookup"><span data-stu-id="5cc32-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="5cc32-206">**Aby rozwiązać** ten problem: musisz atestować w imieniu klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Zrzut ekranu Microsoft 365 Centrum administracyjnego z prośbą o sprosenie się z partnerem w celu potwierdzenia akceptacji Umowa z Klientem Microsoft.":::

<span data-ttu-id="5cc32-208">**Scenariusz 2.** Istniejący klient kupił dowolną z następujących ofert, subskrypcji oprogramowania i oprogramowania, wystąpień zarezerwowanych i planu platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="5cc32-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="5cc32-209">Klient próbuje teraz dokonać nowego zakupu u nowego partnera.</span><span class="sxs-lookup"><span data-stu-id="5cc32-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="5cc32-210">Gdy klient kliknie adres URL w centrum administracyjnym Microsoft 365, aby zaakceptować nową relację z partnerem i umowę, otrzyma komunikat "Skontaktuj się z partnerem, aby potwierdzić akceptację Umowa z Klientem Microsoft".</span><span class="sxs-lookup"><span data-stu-id="5cc32-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="5cc32-211">**Aby rozwiązać** ten problem: musisz atestować w imieniu klienta.</span><span class="sxs-lookup"><span data-stu-id="5cc32-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="5cc32-212">Potwierdzanie, że klient zaakceptował umowę</span><span class="sxs-lookup"><span data-stu-id="5cc32-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="5cc32-213">Jeśli spróbujesz utworzyć nowe zamówienie dla istniejącego klienta, który nie został jeszcze potwierdzony, zostanie wyświetlony monit o potwierdzenie.</span><span class="sxs-lookup"><span data-stu-id="5cc32-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="5cc32-214">Użyj poniższej procedury w tym celu.</span><span class="sxs-lookup"><span data-stu-id="5cc32-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="5cc32-215">Wprowadź **imię,** **nazwisko,** adres **e-mail** i **numer** telefonu (opcjonalnie) użytkownika, który zaakceptował umowę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="5cc32-216">W **obszarze Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5cc32-217">Nie można ustawić tej daty na przyszłą datę.</span><span class="sxs-lookup"><span data-stu-id="5cc32-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="5cc32-218">Wybierz przycisk **Zapisz i kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="5cc32-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="5cc32-219">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="5cc32-219">Next steps</span></span>

- [<span data-ttu-id="5cc32-220">Weryfikowanie lub aktualizowanie informacji o profilu firmy</span><span class="sxs-lookup"><span data-stu-id="5cc32-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="5cc32-221">Umowy z Klientem Microsoft (według regionu, języka)</span><span class="sxs-lookup"><span data-stu-id="5cc32-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
