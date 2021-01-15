---
title: Jak odczytać rozliczenie & pliku Rekonesans
ms.topic: article
ms.date: 06/05/2020
description: Dowiedz się więcej na temat faktury & pliki uzgadniania. Na rachunku są naliczane opłaty za centrum partnerskie w ramach programu, produktów i klientów w danym okresie miesięcznym.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43c2605d750d35bc2e0095b1fed413ed91a1a28e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215819"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a><span data-ttu-id="7c8ac-104">Zapoznaj się z plikiem rachunku i rozliczeniami — Dowiedz się, jak je znaleźć w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="7c8ac-104">Understand your bill and reconciliation file - learn how to find them in Partner Center</span></span>


<span data-ttu-id="7c8ac-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="7c8ac-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7c8ac-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="7c8ac-106">Global admin</span></span>
- <span data-ttu-id="7c8ac-107">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="7c8ac-107">Billing admin</span></span>
- <span data-ttu-id="7c8ac-108">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="7c8ac-108">Admin agent</span></span>


<span data-ttu-id="7c8ac-109">**Faktura** to **Podsumowanie wszystkich opłat za centrum partnerskie** (w ramach programu, wszystkich produktów i wszystkich klientów).</span><span class="sxs-lookup"><span data-stu-id="7c8ac-109">Your **invoice** is a **summary of all your Partner Center charges** (across the program, all products, and all customers).</span></span> 

## <a name="invoice-types"></a><span data-ttu-id="7c8ac-110">Typy faktur</span><span class="sxs-lookup"><span data-stu-id="7c8ac-110">Invoice types</span></span>

<span data-ttu-id="7c8ac-111">Firma Microsoft będzie wydawać jedną fakturę za wszelkie opłaty za licencje (takie jak Office 365) i opłaty za użycie (na przykład platformę Azure) oraz oddzielne faktury za jednorazowe opłaty (takie jak Azure — RI, Marketplace lub Azure plan).</span><span class="sxs-lookup"><span data-stu-id="7c8ac-111">Microsoft will issue one invoice for any license-based charges (such as Office 365) and usage-based charges (such as Azure) and a separate invoice for one-time charges (such as Azure RI, Marketplace, or Azure plan).</span></span>

<span data-ttu-id="7c8ac-112">Na przykład</span><span class="sxs-lookup"><span data-stu-id="7c8ac-112">For example,</span></span>  

<span data-ttu-id="7c8ac-113">**Scenariusz 1 [pojedyncza waluta]**: partner ma zakupy dla ofert 145P i licencji usługi O365,</span><span class="sxs-lookup"><span data-stu-id="7c8ac-113">**Scenario 1 [Single Currency]**: Partner has purchases for 145P offer and O365 licenses,</span></span>  

- <span data-ttu-id="7c8ac-114">Partner otrzyma jedną fakturę PDF i 2 pliki uzgadniania obejmujące opłaty dla usług O365 i Azure (145p).</span><span class="sxs-lookup"><span data-stu-id="7c8ac-114">Partner will get one invoice PDF and 2 reconciliation files covering the charges for both O365 and Azure (145p).</span></span>  

<span data-ttu-id="7c8ac-115">**Scenariusz 2 [pojedyncza waluta]**: partner kupił zakupy na platformie Azure, na rynku i/lub na platformie Azure, a także za pomocą 145p zakupów.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-115">**Scenario 2 [Single Currency]**: Partner has purchases for Azure RI, Marketplace and/or Azure plan along with 145p purchases.</span></span>

- <span data-ttu-id="7c8ac-116">Partner otrzyma jedną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure (145p).</span><span class="sxs-lookup"><span data-stu-id="7c8ac-116">Partner will get one invoice PDF and a reconciliation file covering the charges for Azure (145p).</span></span> 

- <span data-ttu-id="7c8ac-117">Partner otrzyma kolejną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure RI, Marketplace, plan platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-117">Partner will receive another invoice PDF and a reconciliation file covering their charges for Azure RI, Marketplace, Azure plan.</span></span> 

<span data-ttu-id="7c8ac-118">**Scenariusz 3 [wiele walut]**: partner kupił zakupy dla platformy Azure w walucie DKK i plan platformy Azure w EUR i 145p zakupy w euro.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-118">**Scenario 3 [Multi-Currency]**: Partner has purchases for Azure RI in DKK and Azure plan in EUR along with 145p purchases in EUR.</span></span>

- <span data-ttu-id="7c8ac-119">Partner otrzyma jedną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure RI w DKK.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-119">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure RI in DKK.</span></span> 

- <span data-ttu-id="7c8ac-120">Partner otrzyma jedną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure plan w EUR.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-120">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure plan in EUR.</span></span> 

- <span data-ttu-id="7c8ac-121">Partner otrzyma kolejną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę 145p w EUR (lub w walucie rozliczeniowej partnera).</span><span class="sxs-lookup"><span data-stu-id="7c8ac-121">Partner will receive another invoice PDF and a reconciliation file covering their charges for 145p offer in EUR (or partner billing currency).</span></span> 

## <a name="find-your-bill"></a><span data-ttu-id="7c8ac-122">Znajdowanie rachunku</span><span class="sxs-lookup"><span data-stu-id="7c8ac-122">Find your bill</span></span> 

<span data-ttu-id="7c8ac-123">Fakturę można znaleźć na stronie rozliczenia pulpitu nawigacyjnego w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-123">You can find your invoice on the Billing page of the dashboard in Partner Center.</span></span> <span data-ttu-id="7c8ac-124">Możesz również znaleźć historię rozliczeń, trendy wydatków i pliki uzgadniania na tej stronie.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-124">You can also find your billing history, spending trends, and reconciliation files on this page.</span></span> 

1. <span data-ttu-id="7c8ac-125">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-125">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span> 

2. <span data-ttu-id="7c8ac-126">W menu po lewej stronie wybierz pozycję **rozliczenia**.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-126">In the left-hand menu, select **Billing**.</span></span> 

3. <span data-ttu-id="7c8ac-127">Na stronie rozliczenia wybierz fakturę, którą chcesz pobrać.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-127">On the Billing page, select the invoice you want to download.</span></span> 

<span data-ttu-id="7c8ac-128">Możesz znaleźć link do najnowszej faktury w górnej części strony w obszarze saldo konta na podstawie daty ostatniej faktury.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-128">You can find a link to your latest invoice at the top of the page under Account balance as of last invoice date.</span></span> 

<span data-ttu-id="7c8ac-129">Poprzednie faktury można znaleźć w sekcji Historia rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-129">You can find previous invoices in the Billing history section.</span></span> <span data-ttu-id="7c8ac-130">Wybierz odpowiedni rok, a następnie wybierz strzałkę listy rozwijanej obok odpowiedniego okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-130">Choose the appropriate year, then select the drop-down arrow next to the appropriate Billing period.</span></span> <span data-ttu-id="7c8ac-131">Wybierz łącze obok pozycji faktury (PDF), aby pobrać fakturę tego okresu.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-131">Select the link next to Invoices (.pdf) to download that period's invoice.</span></span> 

## <a name="understanding-invoice-pdf"></a><span data-ttu-id="7c8ac-132">Informacje o dokumencie PDF faktury</span><span class="sxs-lookup"><span data-stu-id="7c8ac-132">Understanding invoice PDF</span></span> 

<span data-ttu-id="7c8ac-133">**Faktury za użycie i opłaty oparte na licencji**: faktury za opłaty za usługi, takie jak Office 365 i Azure, będą dostępne w ciągu dwóch (2) dni od wybranej daty rozliczenia [UTC].</span><span class="sxs-lookup"><span data-stu-id="7c8ac-133">**Invoices for Usage and license-based charges**: Invoices for charges for services such as Office 365 and Azure will be available within two (2) days of your selected billing date [UTC].</span></span>  

<span data-ttu-id="7c8ac-134">**Faktury za jednorazowej i opłaty cykliczne**: faktury dla usług takich jak Azure RI, Azure plan i Marketplace będą dostępne nie później niż w ciągu każdego miesiąca.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-134">**Invoices for onetime and recurring charges**: Invoices for charges for services such as Azure RI, Azure plan, Marketplace will be available not later than 8th of every month.</span></span>  

<span data-ttu-id="7c8ac-135">Poniżej znajdują się niektóre pola klucza w dokumencie PDF faktury —</span><span class="sxs-lookup"><span data-stu-id="7c8ac-135">Below are some of the key fields on the Invoice PDF document –</span></span>

<span data-ttu-id="7c8ac-136">**Numer faktury**: unikatowy identyfikator dokumentu faktury wygenerowanego dla odpowiedniego okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-136">**Invoice number**: Unique identifier for the invoice document generated for the respective billing period.</span></span> 

<span data-ttu-id="7c8ac-137">**Okres rozliczeniowy**: jest to okres, w którym masz użycie i usługi oparte na licencji.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-137">**Billing period**: This is the period during which you have usages and license-based services.</span></span> 

<span data-ttu-id="7c8ac-138">**Data faktury**: Data rozliczenia lub Data rocznicy, w której jest generowana faktura co miesiąc.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-138">**Invoice date**: The billing date or anniversary date on which your invoice is generated each month.</span></span> 

<span data-ttu-id="7c8ac-139">**Termin płatności**: Data, o którą należy otrzymać płatność.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-139">**Payment due date**: The date by which your payment must be received.</span></span> 

<span data-ttu-id="7c8ac-140">**Opłaty**: kwota należna w walucie rozliczeniowej dla odpowiedniego okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-140">**Charges**: The amount due in your billing currency for the respective billing period.</span></span> 

<span data-ttu-id="7c8ac-141">**Kredyty**: kredyty (takie jak SLA) lub korekty zmian wprowadzonych w subskrypcjach (na przykład zwiększenie lub zmniejszenie licencji).</span><span class="sxs-lookup"><span data-stu-id="7c8ac-141">**Credits**: Credits (such as SLA) or adjustments for changes made to subscriptions (for example, license increases or decreases).</span></span> 

<span data-ttu-id="7c8ac-142">**Instrukcje dotyczące płatności**: Opis sposobu płacenia faktury w zależności od regionu.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-142">**Payment instructions**: Description of how to pay your invoice, based on your region.</span></span> <span data-ttu-id="7c8ac-143">Zawsze pamiętaj o uwzględnieniu numeru faktury podczas dokonywania płatności.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-143">Always be sure to include your invoice number when making a payment.</span></span> 

<span data-ttu-id="7c8ac-144">Aby uzyskać szczegółowy opis wszystkich pól w pliku faktury (w tym pól dla opłat jednorazowych), zobacz [pola pliku faktury](invoice-file.md).</span><span class="sxs-lookup"><span data-stu-id="7c8ac-144">For a detailed description of all the fields in your invoice file (including fields for one-time charges), see [Invoice file fields](invoice-file.md).</span></span> 

## <a name="understand-reconciliation-files"></a><span data-ttu-id="7c8ac-145">Omówienie plików uzgadniania</span><span class="sxs-lookup"><span data-stu-id="7c8ac-145">Understand reconciliation files</span></span>

 <span data-ttu-id="7c8ac-146">Pliki uzgadniania, które udostępniają szczegółowe dane dotyczące szczegółów opłat, są dostępne do pobrania wraz z DOKUMENTem faktury.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-146">Reconciliation files, which provides a drill down/itemized details of your charges, are available to download along with the Invoice PDF.</span></span> <span data-ttu-id="7c8ac-147">Pliki uzgadniania obejmują identyfikatory klientów i identyfikatory subskrypcji, których można użyć do tworzenia faktur klienta.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-147">The reconciliation files include customer identifiers and subscription identifiers that you can use to create customer invoices.</span></span> <span data-ttu-id="7c8ac-148">Zapoznaj się z  [tematem jak używać plików uzgadniania](use-the-reconciliation-files.md) , aby uzyskać więcej szczegółów na temat plików rekonesans.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-148">Please refer to  [How to use the reconciliation files](use-the-reconciliation-files.md) to get more details on the recon files.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7c8ac-149">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="7c8ac-149">Next steps</span></span>

- [<span data-ttu-id="7c8ac-150">Jak używać plików uzgadniania</span><span class="sxs-lookup"><span data-stu-id="7c8ac-150">How to use the reconciliation files</span></span>](use-the-reconciliation-files.md)