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
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147126"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="cd8d7-104">Obliczanie efektywnej ceny jednostkowej dla użycia planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="cd8d7-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="cd8d7-105">**Odpowiednie role:** Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="cd8d7-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="cd8d7-106">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="cd8d7-106">The effective unit price</span></span>

<span data-ttu-id="cd8d7-107">Efektywna cena jednostkowa jest obliczana na poziomie miernika (w przeciwieństwie do poziomu zasobu) i jest dostosowywana codziennie zgodnie z użyciem miernika.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="cd8d7-108">Efektywną cenę jednostkową obliczamy przy użyciu następujących trzech czynników:</span><span class="sxs-lookup"><span data-stu-id="cd8d7-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="cd8d7-109">Zużycie, które jest monitorowane codziennie w całym cyklu rozliczeniowym</span><span class="sxs-lookup"><span data-stu-id="cd8d7-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="cd8d7-110">Rozliczany koszt miernika</span><span class="sxs-lookup"><span data-stu-id="cd8d7-110">Billable cost for the meter</span></span>
- <span data-ttu-id="cd8d7-111">Warstwy (jeśli dotyczy)</span><span class="sxs-lookup"><span data-stu-id="cd8d7-111">Tiering (if applicable)</span></span>

<span data-ttu-id="cd8d7-112">Ponieważ monitorujemy dzienne zużycie w całym cyklu rozliczeniowym, efektywna cena jednostkowa będzie się zmieniać.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="cd8d7-113">Końcowa cena dla danego cyklu rozliczeniowego będzie dostępna po zatrzymaniu obliczenia zużycia i zamknięciu okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="cd8d7-114">Większość zmian w zużyciu zobaczysz po czwartym lub piątym miejscu dziesiętnym.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="cd8d7-115">Dowiedz się, czy miernik korzysta z cen warstwowych</span><span class="sxs-lookup"><span data-stu-id="cd8d7-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="cd8d7-116">Jeśli nie wiesz, czy miernik korzysta z cen warstwowych, skorzystaj z poniższej procedury, aby się tego dowiedzieć.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="cd8d7-117">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="cd8d7-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="cd8d7-118">Wybierz **pozycję Sell**(Sprzedawaj), wybierz pozycję Pricing and offers **(Ceny i oferty),** a następnie wybierz **pozycję Azure plan pricing (Cennik planu platformy Azure).**</span><span class="sxs-lookup"><span data-stu-id="cd8d7-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="cd8d7-119">Znajdź miernik według identyfikatora, a następnie pobierz dane cennika.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="cd8d7-120">Przykładowe obliczenie</span><span class="sxs-lookup"><span data-stu-id="cd8d7-120">Sample calculation</span></span>

<span data-ttu-id="cd8d7-121">W poniższej tabeli przedstawiono przykład sposobu obliczania efektywnej ceny jednostkowej w okresie otwarcia.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="cd8d7-122">W tabeli mają zastosowanie następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="cd8d7-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="cd8d7-123">**UP** = cena jednostkowa zasobu/godziny = 0,868</span><span class="sxs-lookup"><span data-stu-id="cd8d7-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="cd8d7-124">**BCU** = rozliczana jednostka zużycia dla miernika</span><span class="sxs-lookup"><span data-stu-id="cd8d7-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="cd8d7-125">**BC** = rozliczany koszt miernika = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="cd8d7-126">Odzwierciedla to korektę rabatu 15% PEC.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="cd8d7-127">Następnie używamy dolnego limitu funkcji, aby ograniczyć wartość do dwóch cyfr po przecinku dziesiętnym, aby nalicować minimalną kwotę.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="cd8d7-128">**Efektywna cena jednostkowa** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="cd8d7-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="cd8d7-129">Uwaga: Miernik w tym przykładzie nie ma warstw cenowych ani innych rabatów — współczynniki Efektywne ceny jednostkowej w procentach rabatów i innych korektach.</span><span class="sxs-lookup"><span data-stu-id="cd8d7-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="cd8d7-130">Date (Data)</span><span class="sxs-lookup"><span data-stu-id="cd8d7-130">Date</span></span> | <span data-ttu-id="cd8d7-131">BCU (rozliczana jednostka zużycia)</span><span class="sxs-lookup"><span data-stu-id="cd8d7-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="cd8d7-132">BC (koszt rozliczany)</span><span class="sxs-lookup"><span data-stu-id="cd8d7-132">BC (Billable cost)</span></span> | <span data-ttu-id="cd8d7-133">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="cd8d7-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="cd8d7-134">3 sierpnia</span><span class="sxs-lookup"><span data-stu-id="cd8d7-134">3-Aug</span></span> | <span data-ttu-id="cd8d7-135">29</span><span class="sxs-lookup"><span data-stu-id="cd8d7-135">29</span></span> | <span data-ttu-id="cd8d7-136">21.39</span><span class="sxs-lookup"><span data-stu-id="cd8d7-136">21.39</span></span> | <span data-ttu-id="cd8d7-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="cd8d7-137">0.737586206896552</span></span> |
| <span data-ttu-id="cd8d7-138">10 sierpnia</span><span class="sxs-lookup"><span data-stu-id="cd8d7-138">10-Aug</span></span> | <span data-ttu-id="cd8d7-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="cd8d7-139">210.950039</span></span> | <span data-ttu-id="cd8d7-140">155.63</span><span class="sxs-lookup"><span data-stu-id="cd8d7-140">155.63</span></span> | <span data-ttu-id="cd8d7-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="cd8d7-141">0.737757626107858</span></span> |
| <span data-ttu-id="cd8d7-142">25 sierpnia</span><span class="sxs-lookup"><span data-stu-id="cd8d7-142">25-Aug</span></span> | <span data-ttu-id="cd8d7-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="cd8d7-143">555.950039</span></span> | <span data-ttu-id="cd8d7-144">410.17</span><span class="sxs-lookup"><span data-stu-id="cd8d7-144">410.17</span></span> | <span data-ttu-id="cd8d7-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="cd8d7-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="cd8d7-146">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cd8d7-146">Next steps</span></span>

- [<span data-ttu-id="cd8d7-147">Rozliczenia i podatki</span><span class="sxs-lookup"><span data-stu-id="cd8d7-147">Billing and taxes</span></span>](billing.md)
