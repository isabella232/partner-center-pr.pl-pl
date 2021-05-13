---
title: Ustawianie budżetu wydatków na platformę Azure dla klientów
ms.topic: how-to
ms.date: 03/17/2021
description: Dowiedz się, jak ustawiać lub usuwać miesięczne budżety wydatków na platformę Azure dla klientów, a także jak wyświetlać dane wydatków na platformie Azure i ustawiać powiadomienia dotyczące budżetu.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855356"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="7e561-103">Ustawianie, sprawdzanie lub usuwanie miesięcznych budżetów wydatków na platformę Azure dla klientów w Partner Center</span><span class="sxs-lookup"><span data-stu-id="7e561-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="7e561-104">**Odpowiednie role:** Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="7e561-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="7e561-105">Możesz ustawić [miesięczny budżet wydatków na platformę Azure dla klientów w](#set-azure-spending-budget) Partner Center.</span><span class="sxs-lookup"><span data-stu-id="7e561-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="7e561-106">Ułatwia to klientom zarządzanie wydatkami na platformę Azure.</span><span class="sxs-lookup"><span data-stu-id="7e561-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="7e561-107">Ta opcja umożliwia porównanie wydatków klientów na platformę Azure z budżetem w ciągu miesiąca.</span><span class="sxs-lookup"><span data-stu-id="7e561-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="7e561-108">Ułatwia to również klientom budżetowanie wydatków na platformę Azure, dzięki czemu ich miesięczne rachunki nie są wyższe niż przewidujesz.</span><span class="sxs-lookup"><span data-stu-id="7e561-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="7e561-109">Ta funkcja nie jest dostępna w piaskownicy ani na kontach Test w środowisku produkcyjnym (TIP).</span><span class="sxs-lookup"><span data-stu-id="7e561-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="7e561-110">Po [skonfigurowaniu budżetu wydatków na platformę Azure](#set-azure-spending-budget)dla klientów możesz również przejrzeć użycie klientów w następujący sposób.</span><span class="sxs-lookup"><span data-stu-id="7e561-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="7e561-111">Te opcje mogą pomóc w wykrywaniu błędnie skonfigurowanych usług lub nietypowych trendów, które mogą sugerować oszustwo.</span><span class="sxs-lookup"><span data-stu-id="7e561-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="7e561-112">Następnie możesz współpracować z klientami, aby zidentyfikować główną przyczynę i zarządzać kosztami.</span><span class="sxs-lookup"><span data-stu-id="7e561-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="7e561-113">W razie potrzeby można również zmienić budżet klienta [na](#set-azure-spending-budget) wyższą kwotę.</span><span class="sxs-lookup"><span data-stu-id="7e561-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="7e561-114">Sprawdzanie bieżących wydatków na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="7e561-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="7e561-115">Włącz powiadomienia e-mail, gdy wydatki klienta zbliża się do limitu budżetu</span><span class="sxs-lookup"><span data-stu-id="7e561-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="7e561-116">Wyświetlanie kosztów pozycji według usługi dla subskrypcji opartych na użyciu</span><span class="sxs-lookup"><span data-stu-id="7e561-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="7e561-117">W dowolnym momencie [możesz również usunąć budżet](#remove-azure-spending-budget) wydatków na platformę Azure dla klientów.</span><span class="sxs-lookup"><span data-stu-id="7e561-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="7e561-118">Dane wydatków na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="7e561-118">Azure spending data</span></span>

<span data-ttu-id="7e561-119">Dane wydatków na platformę Azure są *szacowane,* a *rzeczywiste kwoty rozliczeń mogą się różnić.*</span><span class="sxs-lookup"><span data-stu-id="7e561-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="7e561-120">Wartość danych nie odzwierciedla *podatków,* środków, korekt ani innych opłat, które mogą być naliczane.</span><span class="sxs-lookup"><span data-stu-id="7e561-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="7e561-121">Dane wydatków są *odświeżane raz dziennie.*</span><span class="sxs-lookup"><span data-stu-id="7e561-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="7e561-122">Klienci mogą nadal korzystać z usług i zasobów platformy Azure (za które są naliczane opłaty), chyba że zmienisz ustawienia konta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7e561-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="7e561-123">Ustawianie budżetu wydatków na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="7e561-123">Set Azure spending budget</span></span>

<span data-ttu-id="7e561-124">Możesz ustawić *miesięczny budżet wydatków na platformę Azure dla* wielu klientów w Partner Center:</span><span class="sxs-lookup"><span data-stu-id="7e561-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="7e561-125">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7e561-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7e561-126">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Wydatki na platformę Azure.**</span><span class="sxs-lookup"><span data-stu-id="7e561-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7e561-127">Na stronie **wydatków na** platformę Azure w obszarze **Klienci Microsoft Azure subskrypcjami** wybierz klientów, dla których chcesz ustawić budżet.</span><span class="sxs-lookup"><span data-stu-id="7e561-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="7e561-128">Wprowadź wartość dla budżetu **miesięcznego.**</span><span class="sxs-lookup"><span data-stu-id="7e561-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="7e561-129">Wybierz **pozycję Zastosuj,** aby zapisać zmiany.</span><span class="sxs-lookup"><span data-stu-id="7e561-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="7e561-130">Możesz również *ustawić budżet dla pojedynczego klienta w* ustawieniach subskrypcji:</span><span class="sxs-lookup"><span data-stu-id="7e561-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="7e561-131">Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7e561-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="7e561-132">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Klienci**.</span><span class="sxs-lookup"><span data-stu-id="7e561-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="7e561-133">Na **stronie Klienci** wybierz nazwę firmy **klienta**.</span><span class="sxs-lookup"><span data-stu-id="7e561-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="7e561-134">Na stronie Subskrypcje klienta w **obszarze** Subskrypcja oparta **na użyciu** wybierz pozycję **Zmień budżet.**</span><span class="sxs-lookup"><span data-stu-id="7e561-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="7e561-135">Wprowadź wartość budżetu.</span><span class="sxs-lookup"><span data-stu-id="7e561-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="7e561-136">Wybierz **pozycję Zastosuj,** aby zapisać zmiany.</span><span class="sxs-lookup"><span data-stu-id="7e561-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="7e561-137">Usuwanie budżetu wydatków na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="7e561-137">Remove Azure spending budget</span></span>

<span data-ttu-id="7e561-138">Możesz usunąć *miesięczny budżet wydatków na* platformę Azure dla klientów w Partner Center:</span><span class="sxs-lookup"><span data-stu-id="7e561-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="7e561-139">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7e561-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7e561-140">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Wydatki na platformę Azure.**</span><span class="sxs-lookup"><span data-stu-id="7e561-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7e561-141">Na stronie **wydatków na** platformę Azure w obszarze **Klienci Microsoft Azure subskrypcjami** wybierz klientów, których budżet chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="7e561-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="7e561-142">Wybierz **pozycję Usuń budżet.**</span><span class="sxs-lookup"><span data-stu-id="7e561-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="7e561-143">Sprawdzanie bieżących wydatków na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="7e561-143">Check current Azure spending</span></span>

<span data-ttu-id="7e561-144">Bieżące wydatki *na platformę Azure* i budżety miesięczne klientów można śledzić w dowolnym momencie:</span><span class="sxs-lookup"><span data-stu-id="7e561-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="7e561-145">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7e561-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7e561-146">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Wydatki na platformę Azure.**</span><span class="sxs-lookup"><span data-stu-id="7e561-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7e561-147">Na stronie **wydatków na** platformę Azure w obszarze Klienci z subskrypcjami **Microsoft Azure** można zobaczyć omówienie miesięcznych budżetów klientów, bieżących szacunkowych wydatków i procentowego użytego budżetu.</span><span class="sxs-lookup"><span data-stu-id="7e561-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="7e561-148">Powiadomienia dotyczące limitów budżetu</span><span class="sxs-lookup"><span data-stu-id="7e561-148">Notifications for budget limits</span></span>

<span data-ttu-id="7e561-149">Możesz *włączyć powiadomienia e-mail,* gdy miesięczne wydatki klienta zbliżają się do limitu budżetu.</span><span class="sxs-lookup"><span data-stu-id="7e561-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="7e561-150">Po włączeniu tej opcji będziesz powiadamiany, gdy klienci będą korzystać z co najmniej 80% miesięcznego budżetu.</span><span class="sxs-lookup"><span data-stu-id="7e561-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="7e561-151">Ta opcja pomaga śledzić rachunek za korzystanie z platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="7e561-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="7e561-152">Aby skonfigurować powiadomienia e-mail:</span><span class="sxs-lookup"><span data-stu-id="7e561-152">To configure email notifications:</span></span>

1. <span data-ttu-id="7e561-153">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7e561-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="7e561-154">Przejdź do obszaru **Settings** (Ustawienia).</span><span class="sxs-lookup"><span data-stu-id="7e561-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="7e561-155">Wybierz **pozycję Moje preferencje.**</span><span class="sxs-lookup"><span data-stu-id="7e561-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="7e561-156">Skonfiguruj preferowany adres e-mail, jeśli nie został jeszcze skonfigurowany.</span><span class="sxs-lookup"><span data-stu-id="7e561-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="7e561-157">Skonfiguruj preferowany język powiadomienia.</span><span class="sxs-lookup"><span data-stu-id="7e561-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="7e561-158">Wybierz **kartę CSP** w **sekcji Preferencje** powiadomień.</span><span class="sxs-lookup"><span data-stu-id="7e561-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="7e561-159">Zaznacz opcję Email (Adres e-mail) dla **powiadomienia Azure Spending (Wydatki na** platformę Azure) i save **(Zapisz).**</span><span class="sxs-lookup"><span data-stu-id="7e561-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="7e561-160">Koszty z elementami według usługi</span><span class="sxs-lookup"><span data-stu-id="7e561-160">Itemized costs by service</span></span>

<span data-ttu-id="7e561-161">Możesz wyświetlić *koszty z pozycjami (i szacowane użycie) według usługi dla subskrypcji opartych na użyciu:*</span><span class="sxs-lookup"><span data-stu-id="7e561-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="7e561-162">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7e561-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="7e561-163">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="7e561-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="7e561-164">Na stronie **Klienci** wybierz nazwę firmy **klienta**.</span><span class="sxs-lookup"><span data-stu-id="7e561-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="7e561-165">Na stronie **Subskrypcje klienta** w obszarze **Subskrypcje** oparte na użyciu wybierz nazwę **subskrypcji**.</span><span class="sxs-lookup"><span data-stu-id="7e561-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="7e561-166">Na stronie subskrypcji możesz przejrzeć  koszty ujmowane według usługi i Szacowane użycie **dla** bieżącego miesiąca.</span><span class="sxs-lookup"><span data-stu-id="7e561-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="7e561-167">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="7e561-167">Next steps</span></span>

- [<span data-ttu-id="7e561-168">Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="7e561-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
