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
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528562"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="80ac4-104">Obliczanie efektywnej ceny jednostkowej dla użycia planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="80ac4-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="80ac4-105">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="80ac4-105">The effective unit price</span></span>

<span data-ttu-id="80ac4-106">Efektywna cena jednostkowa jest obliczana na poziomie miernika (w przeciwieństwie do poziomu zasobu) i jest dostosowywana codziennie zgodnie z użyciem miernika.</span><span class="sxs-lookup"><span data-stu-id="80ac4-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="80ac4-107">Efektywną cenę jednostkową obliczamy przy użyciu następujących trzech czynników:</span><span class="sxs-lookup"><span data-stu-id="80ac4-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="80ac4-108">Zużycie, które jest monitorowane codziennie w całym cyklu rozliczeniowym</span><span class="sxs-lookup"><span data-stu-id="80ac4-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="80ac4-109">Rozliczany koszt miernika</span><span class="sxs-lookup"><span data-stu-id="80ac4-109">Billable cost for the meter</span></span>
- <span data-ttu-id="80ac4-110">Warstwy (jeśli dotyczy)</span><span class="sxs-lookup"><span data-stu-id="80ac4-110">Tiering (if applicable)</span></span>

<span data-ttu-id="80ac4-111">Ponieważ monitorujemy dzienne zużycie w całym cyklu rozliczeniowym, efektywna cena jednostkowa będzie się zmieniać.</span><span class="sxs-lookup"><span data-stu-id="80ac4-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="80ac4-112">Końcowa cena dla danego cyklu rozliczeniowego będzie dostępna po zatrzymaniu obliczania zużycia i zamknięciu okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="80ac4-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="80ac4-113">Większość zmian zużycia zobaczysz po czwartym lub piątym miejscu dziesiętnym.</span><span class="sxs-lookup"><span data-stu-id="80ac4-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="80ac4-114">Dowiedz się, czy miernik korzysta z cen warstwowych</span><span class="sxs-lookup"><span data-stu-id="80ac4-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="80ac4-115">Jeśli nie wiesz, czy twój miernik korzysta z cen warstwowych, skorzystaj z poniższej procedury, aby się tego dowiedzieć.</span><span class="sxs-lookup"><span data-stu-id="80ac4-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="80ac4-116">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="80ac4-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="80ac4-117">Wybierz **pozycję Sell**(Sprzedawaj), wybierz pozycję Pricing and offers **(Ceny** i oferty), a następnie wybierz **pozycję Azure plan pricing (Cennik planu platformy Azure).**</span><span class="sxs-lookup"><span data-stu-id="80ac4-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="80ac4-118">Znajdź miernik według identyfikatora, a następnie pobierz dane dotyczące cen.</span><span class="sxs-lookup"><span data-stu-id="80ac4-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="80ac4-119">Przykładowe obliczenie</span><span class="sxs-lookup"><span data-stu-id="80ac4-119">Sample calculation</span></span>

<span data-ttu-id="80ac4-120">W poniższej tabeli przedstawiono przykład sposobu obliczania efektywnej ceny jednostkowej w otwartym okresie.</span><span class="sxs-lookup"><span data-stu-id="80ac4-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="80ac4-121">W tabeli mają zastosowanie następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="80ac4-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="80ac4-122">**UP** = cena jednostkowa zasobu/godziny = 0,868</span><span class="sxs-lookup"><span data-stu-id="80ac4-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="80ac4-123">**BCU** = rozliczana jednostka zużycia dla miernika</span><span class="sxs-lookup"><span data-stu-id="80ac4-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="80ac4-124">**BC** = rozliczany koszt miernika = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="80ac4-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="80ac4-125">Odzwierciedla to korektę rabatu 15% rabatu PEC.</span><span class="sxs-lookup"><span data-stu-id="80ac4-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="80ac4-126">Następnie używamy dolnego limitu funkcji, aby ograniczyć wartość do dwóch cyfr po przecinku dziesiętnym, aby naliczyć minimalną kwotę.</span><span class="sxs-lookup"><span data-stu-id="80ac4-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="80ac4-127">**Efektywna cena jednostkowa** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="80ac4-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="80ac4-128">Uwaga: Miernik w tym przykładzie nie ma warstw cenowych ani innych rabatów — współczynnik efektywnej ceny jednostkowej ma wartość procentową rabatu i inne korekty.</span><span class="sxs-lookup"><span data-stu-id="80ac4-128">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="80ac4-129">Date (Data)</span><span class="sxs-lookup"><span data-stu-id="80ac4-129">Date</span></span> | <span data-ttu-id="80ac4-130">BCU (rozliczana jednostka zużycia)</span><span class="sxs-lookup"><span data-stu-id="80ac4-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="80ac4-131">BC (koszt rozliczany)</span><span class="sxs-lookup"><span data-stu-id="80ac4-131">BC (Billable cost)</span></span> | <span data-ttu-id="80ac4-132">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="80ac4-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="80ac4-133">3 sierpnia</span><span class="sxs-lookup"><span data-stu-id="80ac4-133">3-Aug</span></span> | <span data-ttu-id="80ac4-134">29</span><span class="sxs-lookup"><span data-stu-id="80ac4-134">29</span></span> | <span data-ttu-id="80ac4-135">21.39</span><span class="sxs-lookup"><span data-stu-id="80ac4-135">21.39</span></span> | <span data-ttu-id="80ac4-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="80ac4-136">0.737586206896552</span></span> |
| <span data-ttu-id="80ac4-137">10 sierpnia</span><span class="sxs-lookup"><span data-stu-id="80ac4-137">10-Aug</span></span> | <span data-ttu-id="80ac4-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="80ac4-138">210.950039</span></span> | <span data-ttu-id="80ac4-139">155.63</span><span class="sxs-lookup"><span data-stu-id="80ac4-139">155.63</span></span> | <span data-ttu-id="80ac4-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="80ac4-140">0.737757626107858</span></span> |
| <span data-ttu-id="80ac4-141">25 sierpnia</span><span class="sxs-lookup"><span data-stu-id="80ac4-141">25-Aug</span></span> | <span data-ttu-id="80ac4-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="80ac4-142">555.950039</span></span> | <span data-ttu-id="80ac4-143">410.17</span><span class="sxs-lookup"><span data-stu-id="80ac4-143">410.17</span></span> | <span data-ttu-id="80ac4-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="80ac4-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="80ac4-145">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="80ac4-145">Next steps</span></span>

- [<span data-ttu-id="80ac4-146">Rozliczenia i podatki</span><span class="sxs-lookup"><span data-stu-id="80ac4-146">Billing and taxes</span></span>](billing.md)
