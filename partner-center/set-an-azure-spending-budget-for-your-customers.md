---
title: Ustawianie budżetu wydatków na platformę Azure dla klientów
ms.topic: how-to
ms.date: 03/17/2021
description: Dowiedz się, jak ustawiać lub usuwać miesięczne budżety wydatków platformy Azure dla klientów, a także wyświetlać dane wydatków platformy Azure i ustawiać powiadomienia związane z budżetem.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712753"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="ff7a9-103">Ustaw, sprawdzaj lub usuwaj miesięczne budżety wydatków platformy Azure dla klientów w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="ff7a9-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="ff7a9-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="ff7a9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ff7a9-105">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="ff7a9-105">Admin agent</span></span>

<span data-ttu-id="ff7a9-106">Możesz [ustawić miesięczny budżet wydatków platformy Azure dla klientów](#set-azure-spending-budget) w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="ff7a9-107">Dzięki temu klienci mogą zarządzać wydatkami na platformę Azure.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="ff7a9-108">Ta opcja umożliwia porównanie wydatków platformy Azure dla klientów z budżetem w danym miesiącu.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="ff7a9-109">Ułatwia ona również klientom budżetowanie wydatków na platformę Azure, dzięki czemu miesięczne rozliczenie nie jest wyższe niż przewidywane.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="ff7a9-110">Ta funkcja jest niedostępna w piaskownicy lub testowaniu na kontach w środowisku produkcyjnym.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="ff7a9-111">Po [ustawieniu budżetu wydatków na platformę Azure dla swoich klientów](#set-azure-spending-budget)można również przejrzeć użycie klienta w następujący sposób.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="ff7a9-112">Te opcje mogą pomóc w określeniu błędnie skonfigurowanych usług lub nietypowych trendów, które mogą sugerować oszustwo.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="ff7a9-113">Następnie możesz współpracować z klientami, aby identyfikować główną przyczynę i zarządzać kosztami.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="ff7a9-114">W razie potrzeby można także [zmienić budżet klienta](#set-azure-spending-budget) na wyższą kwotę.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="ff7a9-115">Sprawdź bieżące wydatki na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="ff7a9-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="ff7a9-116">Włącz powiadomienia e-mail, gdy wydatki klienta zbliżają się do limitu budżetu</span><span class="sxs-lookup"><span data-stu-id="ff7a9-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="ff7a9-117">Wyświetlanie wyszczególnionych kosztów według usługi dla subskrypcji opartych na użyciu</span><span class="sxs-lookup"><span data-stu-id="ff7a9-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="ff7a9-118">W dowolnym momencie możesz również [usunąć budżet wydatków platformy Azure](#remove-azure-spending-budget) dla klientów.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="ff7a9-119">Dane wydatków platformy Azure</span><span class="sxs-lookup"><span data-stu-id="ff7a9-119">Azure spending data</span></span>

<span data-ttu-id="ff7a9-120">Dane wydatków platformy Azure to *oszacowanie* , a *rzeczywiste kwoty rozliczeń mogą się różnić*.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="ff7a9-121">Wartość danych *nie odzwierciedla* podatków, kredytów, korekt lub innych opłat, które mogą być stosowane.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="ff7a9-122">Dane wydatków są *odświeżane raz* dziennie.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="ff7a9-123">Klienci mogą nadal korzystać z usług i zasobów platformy Azure (i być obciążani nimi), chyba że zmienisz ustawienia konta w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="ff7a9-124">Ustaw budżet wydatków na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="ff7a9-124">Set Azure spending budget</span></span>

<span data-ttu-id="ff7a9-125">Możesz *ustawić miesięczny budżet wydatków platformy Azure* dla wielu klientów w centrum partnerskim:</span><span class="sxs-lookup"><span data-stu-id="ff7a9-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="ff7a9-126">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ff7a9-127">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **wydatki na platformę Azure**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ff7a9-128">Na stronie **wydatków platformy Azure** w obszarze **klienci z subskrypcjami Microsoft Azure** wybierz klientów, dla których chcesz ustawić budżet.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="ff7a9-129">Wprowadź wartość dla **miesięcznego budżetu**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="ff7a9-130">Wybierz pozycję **Zastosuj** , aby zapisać zmiany.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="ff7a9-131">Możesz również *ustawić budżet dla pojedynczego klienta* w ustawieniach subskrypcji:</span><span class="sxs-lookup"><span data-stu-id="ff7a9-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="ff7a9-132">Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="ff7a9-133">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **klienci**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="ff7a9-134">Na stronie **klienci** wybierz **nazwę firmy** klienta.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="ff7a9-135">Na stronie **subskrypcje** klienta w obszarze **subskrypcja oparta na użyciu** wybierz pozycję **Zmień budżet**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="ff7a9-136">Wprowadź wartość budżetu.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="ff7a9-137">Wybierz pozycję **Zastosuj** , aby zapisać zmiany.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="ff7a9-138">Usuń budżet wydatków platformy Azure</span><span class="sxs-lookup"><span data-stu-id="ff7a9-138">Remove Azure spending budget</span></span>

<span data-ttu-id="ff7a9-139">Możesz *usunąć miesięczny budżet wydatków platformy Azure* dla klientów w centrum partnerskim:</span><span class="sxs-lookup"><span data-stu-id="ff7a9-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="ff7a9-140">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ff7a9-141">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **wydatki na platformę Azure**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ff7a9-142">Na stronie **wydatków platformy Azure** w obszarze **klienci z subskrypcjami Microsoft Azure** wybierz klientów, których budżet chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="ff7a9-143">Wybierz pozycję **Usuń budżet**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="ff7a9-144">Sprawdź bieżące wydatki na platformę Azure</span><span class="sxs-lookup"><span data-stu-id="ff7a9-144">Check current Azure spending</span></span>

<span data-ttu-id="ff7a9-145">W dowolnym momencie możesz *śledzić bieżące wydatki na korzystanie z platformy Azure i budżety miesięczne klientów* :</span><span class="sxs-lookup"><span data-stu-id="ff7a9-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="ff7a9-146">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ff7a9-147">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **wydatki na platformę Azure**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ff7a9-148">Na stronie **wydatków na platformę Azure** w obszarze **klienci z subskrypcjami Microsoft Azure** można zobaczyć przegląd budżetów miesięcznych klientów, bieżące oszacowania wydatków i procent użycia budżetu.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="ff7a9-149">Powiadomienia dotyczące limitów budżetu</span><span class="sxs-lookup"><span data-stu-id="ff7a9-149">Notifications for budget limits</span></span>

<span data-ttu-id="ff7a9-150">*Powiadomienia e-mail można włączyć* , gdy miesięczne wydatki klienta zbliżają się do limitu budżetu.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="ff7a9-151">Po włączeniu tej opcji użytkownik zostanie powiadomiony, że klienci będą korzystać z co najmniej 80% czasu miesięcznego budżetu.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="ff7a9-152">Ta opcja pomaga zachować oczami na rachunku na korzystanie z platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="ff7a9-153">Aby skonfigurować powiadomienia e-mail:</span><span class="sxs-lookup"><span data-stu-id="ff7a9-153">To configure email notifications:</span></span>

1. <span data-ttu-id="ff7a9-154">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="ff7a9-155">Przejdź do obszaru **Settings** (Ustawienia).</span><span class="sxs-lookup"><span data-stu-id="ff7a9-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="ff7a9-156">Wybierz pozycję **moje preferencje**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="ff7a9-157">Jeśli nie, skonfiguruj preferowany adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="ff7a9-158">Skonfiguruj preferowany język dla powiadomienia.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="ff7a9-159">Wybierz kartę **dostawca CSP** w sekcji **Preferencje powiadomień** .</span><span class="sxs-lookup"><span data-stu-id="ff7a9-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="ff7a9-160">Zaznacz opcję Poczta E-mail dla powiadomienia **wydatków platformy Azure** i **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="ff7a9-161">Wyszczególnione koszty według usługi</span><span class="sxs-lookup"><span data-stu-id="ff7a9-161">Itemized costs by service</span></span>

<span data-ttu-id="ff7a9-162">Można *wyświetlić wyszczególnione koszty (i szacowane użycie) według usługi dla subskrypcji opartych na użyciu*:</span><span class="sxs-lookup"><span data-stu-id="ff7a9-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="ff7a9-163">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="ff7a9-164">W menu po lewej stronie w obszarze **CSP** wybierz pozycję **klienci**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="ff7a9-165">Na stronie **klienci** wybierz **nazwę firmy** klienta.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="ff7a9-166">Na stronie **subskrypcje** klienta w obszarze **subskrypcje na podstawie użycia** wybierz nazwę **subskrypcji**.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="ff7a9-167">Na stronie subskrypcja można przejrzeć **koszty wyszczególnione** według usługi i **szacowane użycie** w bieżącym miesiącu.</span><span class="sxs-lookup"><span data-stu-id="ff7a9-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="ff7a9-168">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="ff7a9-168">Next steps</span></span>

- [<span data-ttu-id="ff7a9-169">Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="ff7a9-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
