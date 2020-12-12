---
title: Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft
description: Dowiedz się, jak potwierdzić akceptację umowy klienta firmy Microsoft przez klienta. Może to być konieczne, aby zamówić produkty i usługi firmy Microsoft dla klientów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354614"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="474ce-104">Zaktualizowano metodę w celu potwierdzenia akceptacji przez klienta umowy klienta firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="474ce-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="474ce-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="474ce-105">**Appropriate roles**</span></span>

- <span data-ttu-id="474ce-106">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="474ce-106">Admin agent</span></span>
- <span data-ttu-id="474ce-107">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="474ce-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="474ce-108">Zasób z umową jest obecnie obsługiwany przez centrum partnerskie tylko w chmurze publicznej firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="474ce-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="474ce-109">Nie dotyczy:</span><span class="sxs-lookup"><span data-stu-id="474ce-109">It is not applicable to:</span></span>
> * <span data-ttu-id="474ce-110">Centrum partnerskie obsługiwane przez firmę 21Vianet</span><span class="sxs-lookup"><span data-stu-id="474ce-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="474ce-111">Centrum partnerskie dla Microsoft Cloud Niemcy</span><span class="sxs-lookup"><span data-stu-id="474ce-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="474ce-112">Centrum partnerskie Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="474ce-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="474ce-113">Od 31 stycznia 2020, wszyscy klienci, istniejące i nowe, muszą podpisać nową umowę klienta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="474ce-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="474ce-114">Aby dowiedzieć się więcej, przeczytaj artykuł [potwierdzenie akceptacji klienta umowy dla klientów firmy Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="474ce-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="474ce-115">Jako partner musisz uzyskać zgodę klienta firmy Microsoft, aby móc zamówić produkty i usługi firmy Microsoft dla tego klienta.</span><span class="sxs-lookup"><span data-stu-id="474ce-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="474ce-116">Aby lepiej pomóc partnerom spełnić wymagania dotyczące zgodności, firma Microsoft prosi partnerów o potwierdzenie akceptacji, dostarczając następujące informacje dotyczące osoby, która zaakceptowali umowę:</span><span class="sxs-lookup"><span data-stu-id="474ce-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="474ce-117">Imię</span><span class="sxs-lookup"><span data-stu-id="474ce-117">First name</span></span>

- <span data-ttu-id="474ce-118">Nazwisko</span><span class="sxs-lookup"><span data-stu-id="474ce-118">Last name</span></span>

- <span data-ttu-id="474ce-119">Adres e-mail</span><span class="sxs-lookup"><span data-stu-id="474ce-119">Email address</span></span>

- <span data-ttu-id="474ce-120">Numer telefonu (opcjonalnie)</span><span class="sxs-lookup"><span data-stu-id="474ce-120">Phone number (optional)</span></span>

- <span data-ttu-id="474ce-121">Data akceptacji</span><span class="sxs-lookup"><span data-stu-id="474ce-121">Date of acceptance</span></span>

<span data-ttu-id="474ce-122">Bezpośredni partnerzy rozliczeń i dostawcy pośredniego muszą potwierdzić akceptację umowy klienta firmy Microsoft przez klienta podczas przeprowadzania transakcji za pośrednictwem usługi Partner Center lub interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="474ce-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="474ce-123">Potwierdzenie jest *obowiązkowe*.</span><span class="sxs-lookup"><span data-stu-id="474ce-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="474ce-124">Jeśli nie podano potwierdzenia dla danego klienta:</span><span class="sxs-lookup"><span data-stu-id="474ce-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="474ce-125">Nie będzie można tworzyć nowych zamówień dla tego klienta.</span><span class="sxs-lookup"><span data-stu-id="474ce-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="474ce-126">Nie będzie można zmienić liczby licencji istniejących subskrypcji opartych na licencji dla tego klienta.</span><span class="sxs-lookup"><span data-stu-id="474ce-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="474ce-127">Potwierdzenie akceptacji klienta można przeprowadzić za pośrednictwem Centrum partnerskiego lub interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="474ce-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="474ce-128">Aby to zrobić za pomocą interfejsu API Centrum partnerskiego, zobacz następujące tematy:</span><span class="sxs-lookup"><span data-stu-id="474ce-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="474ce-129">Uzyskaj potwierdzenie zgody klienta</span><span class="sxs-lookup"><span data-stu-id="474ce-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="474ce-130">Pobierz metadane umowy</span><span class="sxs-lookup"><span data-stu-id="474ce-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="474ce-131">Potwierdź zgodę klienta</span><span class="sxs-lookup"><span data-stu-id="474ce-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="474ce-132">Dotyczy to zarówno środowiska produkcyjnego, jak i piaskownicy.</span><span class="sxs-lookup"><span data-stu-id="474ce-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="474ce-133">Potwierdź akceptację klienta dla nowego klienta</span><span class="sxs-lookup"><span data-stu-id="474ce-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="474ce-134">Poniższa procedura umożliwia potwierdzenie akceptacji klienta podczas tworzenia nowej dzierżawy klienta w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="474ce-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="474ce-135">Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="474ce-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="474ce-136">Wybierz pozycję **klienci**, a następnie **Nowy klient** , a następnie wybierz pozycję **Informacje o koncie**.</span><span class="sxs-lookup"><span data-stu-id="474ce-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="474ce-137">Wprowadź informacje o **firmie** i **kontakcie podstawowym**.</span><span class="sxs-lookup"><span data-stu-id="474ce-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Informacje o firmie":::

3. <span data-ttu-id="474ce-139">W obszarze **Umowa klienta firmy Microsoft** wybierz pozycję **klient zaakceptował najnowszą umowę klienta firmy Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="474ce-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="474ce-140">W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="474ce-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="474ce-141">Nie można ustawić tej wartości na datę przyszłą.</span><span class="sxs-lookup"><span data-stu-id="474ce-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="474ce-142">Wprowadź szczegółowe informacje o użytkowniku, który podał zatwierdzenie.</span><span class="sxs-lookup"><span data-stu-id="474ce-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Dodaj datę przyjęcia":::

   <span data-ttu-id="474ce-144">Domyślnie są wyświetlane podstawowe informacje o użytkowniku kontaktu.</span><span class="sxs-lookup"><span data-stu-id="474ce-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="474ce-145">Jeśli to nie jest poprawne, wybierz pozycję **Aktualizuj** , a następnie wprowadź imię **, nazwisko**, **adres e-mail** i \**numer telefonu* (opcjonalnie) osoby, która zaakceptował umowę.</span><span class="sxs-lookup"><span data-stu-id="474ce-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="474ce-146">Wybierz pozycję **dalej** , aby kontynuować wykonywanie pozostałych kroków w celu utworzenia dzierżawy klienta.</span><span class="sxs-lookup"><span data-stu-id="474ce-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="474ce-147">Potwierdzenie akceptacji przez klienta dla istniejącego klienta</span><span class="sxs-lookup"><span data-stu-id="474ce-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="474ce-148">Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="474ce-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="474ce-149">Wybierz pozycję **klienci**, a następnie Znajdź i wybierz klienta, który ma zostać wyświetlony.</span><span class="sxs-lookup"><span data-stu-id="474ce-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="474ce-150">Wybierz pozycję **Informacje o koncie**.</span><span class="sxs-lookup"><span data-stu-id="474ce-150">Select **Account info**.</span></span>

3. <span data-ttu-id="474ce-151">W obszarze **Umowa klienta firmy Microsoft** wybierz pozycję **Aktualizuj**.</span><span class="sxs-lookup"><span data-stu-id="474ce-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Aktualizowanie":::

4. <span data-ttu-id="474ce-153">Wprowadź **imię** **, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) użytkownika, który zaakceptował umowę.</span><span class="sxs-lookup"><span data-stu-id="474ce-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="474ce-154">W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="474ce-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="474ce-155">Nie można ustawić tej wartości na datę przyszłą.</span><span class="sxs-lookup"><span data-stu-id="474ce-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="474ce-156">Wybierz przycisk **Zapisz i kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="474ce-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="474ce-157">Potwierdź akceptację klienta podczas tworzenia nowego zamówienia dla istniejącego klienta</span><span class="sxs-lookup"><span data-stu-id="474ce-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="474ce-158">Jeśli spróbujesz utworzyć nowe zamówienie dla istniejącego klienta, który nie został wcześniej potwierdzony, zostanie wyświetlony monit o ukończenie potwierdzenia.</span><span class="sxs-lookup"><span data-stu-id="474ce-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="474ce-159">Użyj poniższej procedury w tym celu.</span><span class="sxs-lookup"><span data-stu-id="474ce-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="474ce-160">Wprowadź **imię** **, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) użytkownika, który zaakceptował umowę.</span><span class="sxs-lookup"><span data-stu-id="474ce-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="474ce-161">W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę.</span><span class="sxs-lookup"><span data-stu-id="474ce-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="474ce-162">Nie można ustawić tej wartości na datę przyszłą.</span><span class="sxs-lookup"><span data-stu-id="474ce-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="474ce-163">Wybierz przycisk **Zapisz i kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="474ce-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="474ce-164">Pobierz potwierdzenie akceptacji klienta dla istniejącego klienta</span><span class="sxs-lookup"><span data-stu-id="474ce-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="474ce-165">Potwierdzenie akceptacji klienta dla istniejącego klienta zostało podane wcześniej przy użyciu poniższej procedury.</span><span class="sxs-lookup"><span data-stu-id="474ce-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="474ce-166">Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="474ce-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="474ce-167">Wybierz pozycję **klienci**, a następnie Znajdź i wybierz klienta, który ma zostać wyświetlony.</span><span class="sxs-lookup"><span data-stu-id="474ce-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="474ce-168">Wybierz pozycję **Informacje o koncie**.</span><span class="sxs-lookup"><span data-stu-id="474ce-168">Select **Account info**.</span></span>

3. <span data-ttu-id="474ce-169">W ramach **umowy klienta firmy Microsoft** zobaczysz, czy dla tego klienta podano potwierdzenie.</span><span class="sxs-lookup"><span data-stu-id="474ce-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="474ce-170">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="474ce-170">Next steps</span></span>

- [<span data-ttu-id="474ce-171">Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft w programie partnerskim programu CSP</span><span class="sxs-lookup"><span data-stu-id="474ce-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="474ce-172">Zaświadczenie akceptacji umowy klienta firmy Microsoft w imieniu klienta</span><span class="sxs-lookup"><span data-stu-id="474ce-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)