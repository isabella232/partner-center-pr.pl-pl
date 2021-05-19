---
title: Wymuszanie limitu środków
ms.topic: how-to
ms.date: 05/11/2021
description: Dowiedz się więcej na temat limitu środków i sposobu jego obliczania. Zawiera często zadawane pytania.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148112"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="66b12-104">Wymuszanie limitu środków (CLE)</span><span class="sxs-lookup"><span data-stu-id="66b12-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="66b12-105">**Odpowiednie role:** Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="66b12-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="66b12-106">Limit środków i sposób jego działania</span><span class="sxs-lookup"><span data-stu-id="66b12-106">Your credit limit and how it works</span></span>

<span data-ttu-id="66b12-107">Limit środków to maksymalna kwota (w dolarach amerykańskich), którą partner może wydać na zakup produktów lub subskrypcji w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="66b12-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="66b12-108">W przypadku przekroczenia limitu środków nie będzie można dokonać nowych zakupów, dopóki nie zostanie dokonana wystarczająca płatność.</span><span class="sxs-lookup"><span data-stu-id="66b12-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="66b12-109">Istniejące subskrypcje będą nadal nieprzerwane.</span><span class="sxs-lookup"><span data-stu-id="66b12-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="66b12-110">Limity środków mają zastosowanie do ofert w planie platformy Azure, rezerwacjach platformy Azure, oprogramowaniu, witrynie Marketplace, produktach Azure 145 P, Office i Dynamics.</span><span class="sxs-lookup"><span data-stu-id="66b12-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="66b12-111">Limity środków nie mają zastosowania do odnawiania i bieżącego użycia.</span><span class="sxs-lookup"><span data-stu-id="66b12-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="66b12-112">Przypisujemy Limit środków na poziomie dzierżawy w okresie dołączania.</span><span class="sxs-lookup"><span data-stu-id="66b12-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="66b12-113">Opieramy go na prognozowanych przychodach, zakupach i historii płatności.</span><span class="sxs-lookup"><span data-stu-id="66b12-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="66b12-114">Następnie użyjemy następującej formuły do obliczenia dostępnego salda:</span><span class="sxs-lookup"><span data-stu-id="66b12-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="66b12-115">**[Limit środków — (zakup przychodzący + zaległe niezapłacone faktury + nierozlicone opłaty — nadpłata)]**</span><span class="sxs-lookup"><span data-stu-id="66b12-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="66b12-116">Często zadawane pytania</span><span class="sxs-lookup"><span data-stu-id="66b12-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="66b12-117">Czy limit środków został ustawiony na poziomie dzierżawy, czy na poziomie globalnym?</span><span class="sxs-lookup"><span data-stu-id="66b12-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="66b12-118">Poziom dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="66b12-118">The tenant level.</span></span> <span data-ttu-id="66b12-119">Załóżmy na przykład, że prowadzisz działalność w Stanach Zjednoczonych, Kanadzie i Japonii.</span><span class="sxs-lookup"><span data-stu-id="66b12-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="66b12-120">Jeśli dzierżawa w Kanadzie osiągnie limit środków, ta dzierżawa otrzyma powiadomienie, gdy spróbuje dokonać zakupu w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="66b12-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="66b12-121">Nie będzie to mieć wpływu na pozostałe dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="66b12-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="66b12-122">Jeśli przekroczą limit środków, czy mogę kontynuować obsługę istniejących klientów i subskrypcji z pełnym dostępem?</span><span class="sxs-lookup"><span data-stu-id="66b12-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="66b12-123">Tak.</span><span class="sxs-lookup"><span data-stu-id="66b12-123">Yes.</span></span> <span data-ttu-id="66b12-124">Istniejące subskrypcje klientów będą kontynuowane bez zakłóceń.</span><span class="sxs-lookup"><span data-stu-id="66b12-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="66b12-125">Nie można jednak kupić nowych subskrypcji dla klientów.</span><span class="sxs-lookup"><span data-stu-id="66b12-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="66b12-126">Czy CLE ma zastosowanie zarówno do partnerów rozliczanych bezpośrednio, jak i dostawców pośrednich?</span><span class="sxs-lookup"><span data-stu-id="66b12-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="66b12-127">Tak, dotyczy to obu tych sytuacji.</span><span class="sxs-lookup"><span data-stu-id="66b12-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="66b12-128">Kiedy mogę kupić więcej subskrypcji po przesłaniu płatności w celu przywrócenia konta?</span><span class="sxs-lookup"><span data-stu-id="66b12-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="66b12-129">Powinno być możliwe wznowienie zakupu w ciągu 24 godzin od płatności przy założeniu, że firma Microsoft otrzymała wszystkie wymagania dotyczące kontynuowania procesu sprawdzania środków.</span><span class="sxs-lookup"><span data-stu-id="66b12-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="66b12-130">Jak sprawdzić limit środków?</span><span class="sxs-lookup"><span data-stu-id="66b12-130">How can I check my credit limit?</span></span>

<span data-ttu-id="66b12-131">Skontaktuj się [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) z nami, aby wyświetlić limit środków i uzyskać informacje o ostatnich zakupach.</span><span class="sxs-lookup"><span data-stu-id="66b12-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="66b12-132">Czy faktury, które są w sporze, są wliczane do limitu środków?</span><span class="sxs-lookup"><span data-stu-id="66b12-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="66b12-133">Tak.</span><span class="sxs-lookup"><span data-stu-id="66b12-133">Yes.</span></span> <span data-ttu-id="66b12-134">Możesz jednak skontaktować się z firmą Microsoft na stronie , [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) aby rozwiązać ten problem.</span><span class="sxs-lookup"><span data-stu-id="66b12-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="66b12-135">Jak szybko usłyszę ponownie, jeśli napiszę do ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="66b12-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="66b12-136">Odpowiedź powinna być wyższa niż 24 godziny.</span><span class="sxs-lookup"><span data-stu-id="66b12-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="66b12-137">Jakie kryteria są stosowane przez firmę Microsoft do ustawiania limitu środków partnera?</span><span class="sxs-lookup"><span data-stu-id="66b12-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="66b12-138">Limit środków określamy na podstawie prognozowanych przychodów, zakupów i historii płatności.</span><span class="sxs-lookup"><span data-stu-id="66b12-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="66b12-139">Czy limit środków jest obecnie wymuszany w nowym doświadczeniu handlowym?</span><span class="sxs-lookup"><span data-stu-id="66b12-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="66b12-140">Tak.</span><span class="sxs-lookup"><span data-stu-id="66b12-140">Yes.</span></span> <span data-ttu-id="66b12-141">Limity środków mają zastosowanie do wszystkich programów i produktów CSP w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="66b12-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="66b12-142">Kto otrzyma powiadomienie, gdy moja organizacja zbliża się do limitu środków?</span><span class="sxs-lookup"><span data-stu-id="66b12-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="66b12-143">Powiadomienie powinno zostać otrzymać osoba kontaktowa ds. należności dla konta finansowego Twojej organizacji.</span><span class="sxs-lookup"><span data-stu-id="66b12-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="66b12-144">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="66b12-144">Next steps</span></span>

[<span data-ttu-id="66b12-145">Billing basics (Podstawowe informacje dotyczące rozliczeń)</span><span class="sxs-lookup"><span data-stu-id="66b12-145">Billing basics</span></span>](./billing-basics.md)
