---
title: Obliczanie obowiązującej ceny jednostkowej
ms.topic: how-to
ms.date: 04/02/2021
description: Dowiedz się więcej na temat efektywnej ceny jednostkowej i sposobu jej obliczania. Ten artykuł zawiera również Przykładowe obliczenia.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374401"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="fb851-104">Efektywne Obliczanie cen jednostkowych dla użycia planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="fb851-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="fb851-105">Obowiązująca cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="fb851-105">The effective unit price</span></span>

<span data-ttu-id="fb851-106">Obowiązująca cena jednostkowa jest obliczana na poziomie licznika (w przeciwieństwie do poziomu zasobów) i jest dostosowywana codziennie zgodnie z użyciem licznika.</span><span class="sxs-lookup"><span data-stu-id="fb851-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="fb851-107">Obliczamy obowiązującą cenę jednostkową przy użyciu następujących trzech czynników:</span><span class="sxs-lookup"><span data-stu-id="fb851-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="fb851-108">Użycie, które jest monitorowane codziennie w całym cyklu rozliczeniowym</span><span class="sxs-lookup"><span data-stu-id="fb851-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="fb851-109">Koszt do rozliczenia dla miernika</span><span class="sxs-lookup"><span data-stu-id="fb851-109">Billable cost for the meter</span></span>
- <span data-ttu-id="fb851-110">Obsługa warstw (jeśli dotyczy)</span><span class="sxs-lookup"><span data-stu-id="fb851-110">Tiering (if applicable)</span></span>

<span data-ttu-id="fb851-111">Ze względu na to, że Twoje użycie jest monitorowane codziennie w całym cyklu rozliczeniowym, obowiązująca cena jednostkowa ulegnie zmianie.</span><span class="sxs-lookup"><span data-stu-id="fb851-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="fb851-112">Końcowa cena danego cyklu rozliczeniowego będzie dostępna po zatrzymaniu obliczeń zużycia i zamknięciu okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="fb851-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="fb851-113">Przed czwartym lub piątym miejscem dziesiętnym zobaczysz większość zmian w zużyciu.</span><span class="sxs-lookup"><span data-stu-id="fb851-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="fb851-114">Dowiedz się, czy licznik używa cen warstwowych</span><span class="sxs-lookup"><span data-stu-id="fb851-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="fb851-115">Jeśli nie wiesz, czy licznik używa cen warstwowych, Skorzystaj z poniższej procedury, aby dowiedzieć się.</span><span class="sxs-lookup"><span data-stu-id="fb851-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="fb851-116">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="fb851-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="fb851-117">Wybierz pozycję **Sprzedaj**, wybierz pozycję **Cennik i oferty**, a następnie wybierz pozycję **Cennik planu platformy Azure**.</span><span class="sxs-lookup"><span data-stu-id="fb851-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="fb851-118">Znajdź swój licznik według identyfikatora, a następnie Pobierz dane cennika.</span><span class="sxs-lookup"><span data-stu-id="fb851-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="fb851-119">Przykładowe Obliczanie</span><span class="sxs-lookup"><span data-stu-id="fb851-119">Sample calculation</span></span>

<span data-ttu-id="fb851-120">W poniższej tabeli przedstawiono przykład sposobu obliczania efektywnej ceny jednostkowej w okresie otwartym.</span><span class="sxs-lookup"><span data-stu-id="fb851-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="fb851-121">W tabeli są stosowane następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="fb851-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="fb851-122">W **górę** = cena jednostkowa zasobu/godziny = 0,868</span><span class="sxs-lookup"><span data-stu-id="fb851-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="fb851-123">**Bcu** = jednostka zużycia do rozliczenia dla miernika</span><span class="sxs-lookup"><span data-stu-id="fb851-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="fb851-124">**BC** = koszt płatny dla licznika = bcu \* w górę \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="fb851-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="fb851-125">Odzwierciedla to korektę dla rabatu PEC o 15%.</span><span class="sxs-lookup"><span data-stu-id="fb851-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="fb851-126">Następnie użyjemy dolnego limitu funkcji, aby ograniczyć wartość do dwóch cyfr po przecinku dziesiętnym, aby obciążać kwotę minimalną.</span><span class="sxs-lookup"><span data-stu-id="fb851-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="fb851-127">**Efektywna cena jednostkowa** = bcu/BC</span><span class="sxs-lookup"><span data-stu-id="fb851-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="fb851-128">Licznik w tym przykładzie nie ma warstw w cenniku.</span><span class="sxs-lookup"><span data-stu-id="fb851-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="fb851-129">Efektywne czynniki cenowe jednostki w procentach rabatu i inne korekty.</span><span class="sxs-lookup"><span data-stu-id="fb851-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="fb851-130">Date (Data)</span><span class="sxs-lookup"><span data-stu-id="fb851-130">Date</span></span> | <span data-ttu-id="fb851-131">BCU (jednostka zużycia do rozliczania)</span><span class="sxs-lookup"><span data-stu-id="fb851-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="fb851-132">BC (koszt płatny)</span><span class="sxs-lookup"><span data-stu-id="fb851-132">BC (Billable cost)</span></span> | <span data-ttu-id="fb851-133">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="fb851-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="fb851-134">3 — sie</span><span class="sxs-lookup"><span data-stu-id="fb851-134">3-Aug</span></span> | <span data-ttu-id="fb851-135">29</span><span class="sxs-lookup"><span data-stu-id="fb851-135">29</span></span> | <span data-ttu-id="fb851-136">21,39</span><span class="sxs-lookup"><span data-stu-id="fb851-136">21.39</span></span> | <span data-ttu-id="fb851-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="fb851-137">0.737586206896552</span></span> |
| <span data-ttu-id="fb851-138">10-sie</span><span class="sxs-lookup"><span data-stu-id="fb851-138">10-Aug</span></span> | <span data-ttu-id="fb851-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="fb851-139">210.950039</span></span> | <span data-ttu-id="fb851-140">155,63</span><span class="sxs-lookup"><span data-stu-id="fb851-140">155.63</span></span> | <span data-ttu-id="fb851-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="fb851-141">0.737757626107858</span></span> |
| <span data-ttu-id="fb851-142">25-sie</span><span class="sxs-lookup"><span data-stu-id="fb851-142">25-Aug</span></span> | <span data-ttu-id="fb851-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="fb851-143">555.950039</span></span> | <span data-ttu-id="fb851-144">410,17</span><span class="sxs-lookup"><span data-stu-id="fb851-144">410.17</span></span> | <span data-ttu-id="fb851-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="fb851-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="fb851-146">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="fb851-146">Next steps</span></span>

- [<span data-ttu-id="fb851-147">Rozliczenia i podatki</span><span class="sxs-lookup"><span data-stu-id="fb851-147">Billing and taxes</span></span>](billing.md)
