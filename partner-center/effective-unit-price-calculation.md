---
title: Efektywne obliczanie ceny jednostkowej
ms.topic: how-to
ms.date: 11/10/2020
description: Dowiedz się więcej na temat efektywnej jednostki cenowej i sposobu jej obliczania. Zawiera przykładowe obliczanie.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/11/2020
ms.locfileid: "94499150"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="7fbc3-104">Efektywne Obliczanie cen jednostkowych dla użycia planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="7fbc3-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="7fbc3-105">Obowiązująca cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="7fbc3-105">The effective unit price</span></span>

<span data-ttu-id="7fbc3-106">Obowiązująca cena jednostkowa jest obliczana na poziomie licznika (w przeciwieństwie do poziomu zasobów) i jest dostosowywana codziennie zgodnie z użyciem licznika.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="7fbc3-107">Obliczamy obowiązującą cenę jednostkową przy użyciu następujących trzech czynników:</span><span class="sxs-lookup"><span data-stu-id="7fbc3-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="7fbc3-108">Użycie, które jest monitorowane codziennie w całym cyklu rozliczeniowym</span><span class="sxs-lookup"><span data-stu-id="7fbc3-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="7fbc3-109">Koszt do rozliczenia dla miernika</span><span class="sxs-lookup"><span data-stu-id="7fbc3-109">Billable cost for the meter</span></span>
- <span data-ttu-id="7fbc3-110">Obsługa warstw (jeśli dotyczy)</span><span class="sxs-lookup"><span data-stu-id="7fbc3-110">Tiering (if applicable)</span></span>

<span data-ttu-id="7fbc3-111">Ze względu na to, że Twoje użycie jest monitorowane codziennie w całym cyklu rozliczeniowym, obowiązująca cena jednostkowa ulegnie zmianie.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="7fbc3-112">Końcowa cena danego cyklu rozliczeniowego będzie dostępna po zatrzymaniu obliczeń zużycia i zamknięciu okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="7fbc3-113">Przed czwartym lub piątym miejscem dziesiętnym zobaczysz większość zmian w zużyciu.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="7fbc3-114">Dowiedz się, czy licznik używa cen warstwowych</span><span class="sxs-lookup"><span data-stu-id="7fbc3-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="7fbc3-115">Jeśli nie wiesz, czy licznik używa cen warstwowych, Skorzystaj z poniższej procedury, aby dowiedzieć się.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="7fbc3-116">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7fbc3-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="7fbc3-117">Wybierz pozycję **Sprzedaj** , wybierz pozycję **Cennik i oferty** , a następnie wybierz pozycję **Cennik planu platformy Azure**.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="7fbc3-118">Znajdź swój licznik według identyfikatora, a następnie Pobierz dane cennika.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="7fbc3-119">Przykładowe Obliczanie</span><span class="sxs-lookup"><span data-stu-id="7fbc3-119">Sample calculation</span></span>

<span data-ttu-id="7fbc3-120">W poniższej tabeli przedstawiono przykład sposobu obliczania efektywnej ceny jednostkowej w okresie otwartym.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="7fbc3-121">W tabeli są stosowane następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="7fbc3-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="7fbc3-122">W **górę** = cena jednostkowa zasobu/godziny = 0,868</span><span class="sxs-lookup"><span data-stu-id="7fbc3-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="7fbc3-123">**Bcu** = jednostka zużycia do rozliczenia dla miernika</span><span class="sxs-lookup"><span data-stu-id="7fbc3-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="7fbc3-124">**BC** = koszt płatny dla licznika = bcu \* w górę \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="7fbc3-125">Odzwierciedla to korektę dla rabatu PEC o 15%.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="7fbc3-126">Następnie użyjemy dolnego limitu funkcji, aby ograniczyć wartość do dwóch cyfr po przecinku dziesiętnym, aby obciążać kwotę minimalną.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="7fbc3-127">**Efektywna cena jednostkowa** = bcu/BC</span><span class="sxs-lookup"><span data-stu-id="7fbc3-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="7fbc3-128">Uwaga: licznik w tym przykładzie nie ma warstw w cenniku.</span><span class="sxs-lookup"><span data-stu-id="7fbc3-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="7fbc3-129">Data</span><span class="sxs-lookup"><span data-stu-id="7fbc3-129">Date</span></span> | <span data-ttu-id="7fbc3-130">BCU (jednostka zużycia do rozliczania)</span><span class="sxs-lookup"><span data-stu-id="7fbc3-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="7fbc3-131">BC (koszt płatny)</span><span class="sxs-lookup"><span data-stu-id="7fbc3-131">BC (Billable cost)</span></span> | <span data-ttu-id="7fbc3-132">Efektywna cena jednostkowa</span><span class="sxs-lookup"><span data-stu-id="7fbc3-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="7fbc3-133">3 — sie</span><span class="sxs-lookup"><span data-stu-id="7fbc3-133">3-Aug</span></span> | <span data-ttu-id="7fbc3-134">29</span><span class="sxs-lookup"><span data-stu-id="7fbc3-134">29</span></span> | <span data-ttu-id="7fbc3-135">21,39</span><span class="sxs-lookup"><span data-stu-id="7fbc3-135">21.39</span></span> | <span data-ttu-id="7fbc3-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="7fbc3-136">0.737586206896552</span></span> |
| <span data-ttu-id="7fbc3-137">10-sie</span><span class="sxs-lookup"><span data-stu-id="7fbc3-137">10-Aug</span></span> | <span data-ttu-id="7fbc3-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="7fbc3-138">210.950039</span></span> | <span data-ttu-id="7fbc3-139">155,63</span><span class="sxs-lookup"><span data-stu-id="7fbc3-139">155.63</span></span> | <span data-ttu-id="7fbc3-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="7fbc3-140">0.737757626107858</span></span> |
| <span data-ttu-id="7fbc3-141">25-sie</span><span class="sxs-lookup"><span data-stu-id="7fbc3-141">25-Aug</span></span> | <span data-ttu-id="7fbc3-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="7fbc3-142">555.950039</span></span> | <span data-ttu-id="7fbc3-143">410,17</span><span class="sxs-lookup"><span data-stu-id="7fbc3-143">410.17</span></span> | <span data-ttu-id="7fbc3-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="7fbc3-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="7fbc3-145">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="7fbc3-145">Next steps</span></span>

- [<span data-ttu-id="7fbc3-146">Rozliczenia i podatki</span><span class="sxs-lookup"><span data-stu-id="7fbc3-146">Billing and taxes</span></span>](billing.md)
