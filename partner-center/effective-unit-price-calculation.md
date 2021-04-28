---
title: Obliczanie obowiązującej ceny jednostkowej
ms.topic: how-to
ms.date: 04/02/2021
description: Dowiedz się więcej na temat efektywnej ceny jednostkowej i sposobu jej obliczania. Ten artykuł zawiera również przykładowe obliczenia.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172221"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="76b68-104">Obliczanie efektywnej ceny jednostkowej dla użycia planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="76b68-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="76b68-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="76b68-105">**Appropriate roles**</span></span>

- <span data-ttu-id="76b68-106">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="76b68-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="76b68-107">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="76b68-107">The effective unit price</span></span>

<span data-ttu-id="76b68-108">Efektywna cena jednostkowa jest obliczana na poziomie miernika (w przeciwieństwie do poziomu zasobu) i jest dostosowywana codziennie zgodnie z użyciem miernika.</span><span class="sxs-lookup"><span data-stu-id="76b68-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="76b68-109">Efektywną cenę jednostkową obliczamy przy użyciu następujących trzech czynników:</span><span class="sxs-lookup"><span data-stu-id="76b68-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="76b68-110">Zużycie, które jest monitorowane codziennie w całym cyklu rozliczeniowym</span><span class="sxs-lookup"><span data-stu-id="76b68-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="76b68-111">Rozliczany koszt miernika</span><span class="sxs-lookup"><span data-stu-id="76b68-111">Billable cost for the meter</span></span>
- <span data-ttu-id="76b68-112">Warstwy (jeśli dotyczy)</span><span class="sxs-lookup"><span data-stu-id="76b68-112">Tiering (if applicable)</span></span>

<span data-ttu-id="76b68-113">Ponieważ monitorujemy dzienne zużycie w całym cyklu rozliczeniowym, efektywna cena jednostkowa będzie się zmieniać.</span><span class="sxs-lookup"><span data-stu-id="76b68-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="76b68-114">Końcowa cena dla danego cyklu rozliczeniowego będzie dostępna po zatrzymaniu obliczenia użycia i zamknięciu okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="76b68-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="76b68-115">Większość zmian w zużyciu zobaczysz po czwartym lub piątym miejscu dziesiętnym.</span><span class="sxs-lookup"><span data-stu-id="76b68-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="76b68-116">Dowiedz się, czy miernik korzysta z cen warstwowych</span><span class="sxs-lookup"><span data-stu-id="76b68-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="76b68-117">Jeśli nie wiesz, czy miernik korzysta z cen warstwowych, skorzystaj z poniższej procedury, aby się tego dowiedzieć.</span><span class="sxs-lookup"><span data-stu-id="76b68-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="76b68-118">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="76b68-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="76b68-119">Wybierz **pozycję Sell**(Sprzedawaj), wybierz pozycję Pricing and offers (Ceny i **oferty),** a następnie wybierz **pozycję Azure plan pricing (Cennik planu platformy Azure).**</span><span class="sxs-lookup"><span data-stu-id="76b68-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="76b68-120">Znajdź miernik według identyfikatora, a następnie pobierz dane cennika.</span><span class="sxs-lookup"><span data-stu-id="76b68-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="76b68-121">Przykładowe obliczenie</span><span class="sxs-lookup"><span data-stu-id="76b68-121">Sample calculation</span></span>

<span data-ttu-id="76b68-122">W poniższej tabeli przedstawiono przykład sposobu obliczania efektywnej ceny jednostkowej w okresie otwarcia.</span><span class="sxs-lookup"><span data-stu-id="76b68-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="76b68-123">W tabeli mają zastosowanie następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="76b68-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="76b68-124">**UP** = cena jednostkowa zasobu/godziny = 0,868</span><span class="sxs-lookup"><span data-stu-id="76b68-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="76b68-125">**BCU** = rozliczana jednostka zużycia dla miernika</span><span class="sxs-lookup"><span data-stu-id="76b68-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="76b68-126">**BC** = rozliczany koszt miernika = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="76b68-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="76b68-127">Odzwierciedla to korektę rabatu 15% PEC.</span><span class="sxs-lookup"><span data-stu-id="76b68-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="76b68-128">Następnie używamy dolnego limitu funkcji, aby ograniczyć wartość do dwóch cyfr po przecinku dziesiętnym, aby nalicować minimalną kwotę.</span><span class="sxs-lookup"><span data-stu-id="76b68-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="76b68-129">**Efektywna cena jednostkowa** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="76b68-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="76b68-130">Uwaga: Miernik w tym przykładzie nie ma warstw cenowych ani innych rabatów — współczynniki efektywnej ceny jednostkowej w procentach rabatów i innych korektach.</span><span class="sxs-lookup"><span data-stu-id="76b68-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="76b68-131">Date (Data)</span><span class="sxs-lookup"><span data-stu-id="76b68-131">Date</span></span> | <span data-ttu-id="76b68-132">BCU (rozliczana jednostka zużycia)</span><span class="sxs-lookup"><span data-stu-id="76b68-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="76b68-133">BC (koszt rozliczany)</span><span class="sxs-lookup"><span data-stu-id="76b68-133">BC (Billable cost)</span></span> | <span data-ttu-id="76b68-134">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="76b68-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="76b68-135">3 sierpnia</span><span class="sxs-lookup"><span data-stu-id="76b68-135">3-Aug</span></span> | <span data-ttu-id="76b68-136">29</span><span class="sxs-lookup"><span data-stu-id="76b68-136">29</span></span> | <span data-ttu-id="76b68-137">21.39</span><span class="sxs-lookup"><span data-stu-id="76b68-137">21.39</span></span> | <span data-ttu-id="76b68-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="76b68-138">0.737586206896552</span></span> |
| <span data-ttu-id="76b68-139">10 sierpnia</span><span class="sxs-lookup"><span data-stu-id="76b68-139">10-Aug</span></span> | <span data-ttu-id="76b68-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="76b68-140">210.950039</span></span> | <span data-ttu-id="76b68-141">155.63</span><span class="sxs-lookup"><span data-stu-id="76b68-141">155.63</span></span> | <span data-ttu-id="76b68-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="76b68-142">0.737757626107858</span></span> |
| <span data-ttu-id="76b68-143">25 sierpnia</span><span class="sxs-lookup"><span data-stu-id="76b68-143">25-Aug</span></span> | <span data-ttu-id="76b68-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="76b68-144">555.950039</span></span> | <span data-ttu-id="76b68-145">410.17</span><span class="sxs-lookup"><span data-stu-id="76b68-145">410.17</span></span> | <span data-ttu-id="76b68-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="76b68-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="76b68-147">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="76b68-147">Next steps</span></span>

- [<span data-ttu-id="76b68-148">Rozliczenia i podatki</span><span class="sxs-lookup"><span data-stu-id="76b68-148">Billing and taxes</span></span>](billing.md)
