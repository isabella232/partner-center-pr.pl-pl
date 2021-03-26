---
title: Typy opłat za pliki uzgodnień
ms.topic: article
ms.date: 06/05/2020
description: Wykrywaj typy opłat (takie jak oparte na licencji, oparte na użyciu i jednorazowe), kredyty i rabaty w plikach uzgadniania Centrum partnerskiego.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549230"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="0b808-103">Informacje o różnych typach opłat w plikach uzgadniania Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="0b808-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="0b808-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="0b808-104">**Applies to**</span></span>

- <span data-ttu-id="0b808-105">Centrum partnerskie w chmurze firmy Microsoft dla instytucji rządowych</span><span class="sxs-lookup"><span data-stu-id="0b808-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="0b808-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="0b808-106">**Appropriate roles**</span></span>

- <span data-ttu-id="0b808-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="0b808-107">Admin agent</span></span>
- <span data-ttu-id="0b808-108">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="0b808-108">Billing admin</span></span>
- <span data-ttu-id="0b808-109">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="0b808-109">Global admin</span></span>

<span data-ttu-id="0b808-110">W tym artykule opisano mapowania między sekcją faktury i skojarzonymi typami opłat, które mogą znajdować się w pliku uzgadniania.</span><span class="sxs-lookup"><span data-stu-id="0b808-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="0b808-111">Faktura zawiera podsumowanie opłat.</span><span class="sxs-lookup"><span data-stu-id="0b808-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="0b808-112">Plik uzgadniania zawiera szczegółowy podział transakcji elementu wiersza, w tym typów opłat.</span><span class="sxs-lookup"><span data-stu-id="0b808-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="0b808-113">Aby uzyskać więcej informacji dotyczących plików uzgadniania, zobacz [jak używać plików uzgadniania](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="0b808-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="0b808-114">W przypadku [plików uzgadniania opartych na użyciu](usage-based-recon-files.md) i [plików uzgadniania opartych na licencji](license-based-recon-files.md) są wyświetlane tylko transakcje związane z użyciem i opłaty (zużyte jednostki i powiązane opłaty).</span><span class="sxs-lookup"><span data-stu-id="0b808-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="0b808-115">Kredyty jednorazowe, zniżki lub zwroty, które są wyświetlane na fakturze, jako **korekty** nie są wyświetlane w pliku uzgadniania.</span><span class="sxs-lookup"><span data-stu-id="0b808-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="0b808-116">Mapuj typy opłat na faktury</span><span class="sxs-lookup"><span data-stu-id="0b808-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="0b808-117">Aby uzyskać informacje o opłatach za odwołania między fakturą i plikiem uzgadniania, użyj opcji filtru w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="0b808-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="0b808-118">Filtruj według typów opłat w pliku uzgadniania, aby zamapować opłaty za faktury na zestaw podziałów opłat w pliku uzgadniania.</span><span class="sxs-lookup"><span data-stu-id="0b808-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="0b808-119">Opłaty oparte na licencji</span><span class="sxs-lookup"><span data-stu-id="0b808-119">License-based charges</span></span>

<span data-ttu-id="0b808-120">Aby zmapować opłaty na podstawie licencji na fakturę, należy zsumować **wartość kolumny kwota** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="0b808-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="0b808-121">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="0b808-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="0b808-122">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="0b808-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="0b808-123">Opłata za aktywację</span><span class="sxs-lookup"><span data-stu-id="0b808-123">Activation fee</span></span> | <span data-ttu-id="0b808-124">Kwota naliczana dla klienta w przypadku korzystania z subskrypcji po zakupie.</span><span class="sxs-lookup"><span data-stu-id="0b808-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="0b808-125">Opłata za anulowanie</span><span class="sxs-lookup"><span data-stu-id="0b808-125">Cancel fee</span></span> | <span data-ttu-id="0b808-126">Opłata naliczana proporcjonalnie do klienta po zmianie skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="0b808-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="0b808-127">Anuluj częstotliwość wystąpień</span><span class="sxs-lookup"><span data-stu-id="0b808-127">Cancel instance prorate</span></span> | <span data-ttu-id="0b808-128">Opłata naliczana proporcjonalnie do liczby dni, gdy klient z subskrypcją miesięczną ma zawieszoną subskrypcję, a skojarzone licencje zmieniają się w tym samym miesiącu.</span><span class="sxs-lookup"><span data-stu-id="0b808-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="0b808-129">Opłata za cykl</span><span class="sxs-lookup"><span data-stu-id="0b808-129">Cycle fee</span></span> | <span data-ttu-id="0b808-130">Opłaty okresowe za subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="0b808-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="0b808-131">Tempo wystąpienia cyklu</span><span class="sxs-lookup"><span data-stu-id="0b808-131">Cycle instance prorate</span></span> | <span data-ttu-id="0b808-132">Opłata naliczana proporcjonalnie do liczby opłat naliczanych od klienta po zmianie skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="0b808-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="0b808-133">Oceń opłaty po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="0b808-133">Prorate fees when cancel</span></span> | <span data-ttu-id="0b808-134">Naoprocentowanie proporcjonalnie do nieużywanej części usługi po anulowaniu.</span><span class="sxs-lookup"><span data-stu-id="0b808-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="0b808-135">Opłata proporcjonalna za konwersję z bieżącej oferty</span><span class="sxs-lookup"><span data-stu-id="0b808-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="0b808-136">Naliczanie opłat naliczane po przeprowadzeniu konwersji z bieżącej subskrypcji miesięcznej na roczną subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="0b808-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="0b808-137">Opłaty naliczane za konwersję na nową ofertę</span><span class="sxs-lookup"><span data-stu-id="0b808-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="0b808-138">Opłaty naliczane proporcjonalnie po przeprowadzeniu konwersji miesięcznej subskrypcji na nową roczną subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="0b808-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="0b808-139">Opłata proporcjonalna przy zakupie</span><span class="sxs-lookup"><span data-stu-id="0b808-139">Prorate fees when purchase</span></span> | <span data-ttu-id="0b808-140">Typ opłaty dla subskrypcji w przypadku comiesięcznego lub rocznego rozliczania.</span><span class="sxs-lookup"><span data-stu-id="0b808-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="0b808-141">Opłata proporcjonalna przy odnowieniu</span><span class="sxs-lookup"><span data-stu-id="0b808-141">Prorate fee when renew</span></span> | <span data-ttu-id="0b808-142">Opłata naliczana proporcjonalnie przy odnowieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="0b808-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="0b808-143">Odnawianie opłaty</span><span class="sxs-lookup"><span data-stu-id="0b808-143">Renew fee</span></span> | <span data-ttu-id="0b808-144">Opłata za odnowienie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="0b808-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="0b808-145">Oceń opłaty przy aktywacji</span><span class="sxs-lookup"><span data-stu-id="0b808-145">Prorate fees when activate</span></span> | <span data-ttu-id="0b808-146">Opłata naliczana proporcjonalnie od aktywacji do końca okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="0b808-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="0b808-147">Opłaty jednorazowe</span><span class="sxs-lookup"><span data-stu-id="0b808-147">One-time charges</span></span>

<span data-ttu-id="0b808-148">Aby zmapować te jednorazowe opłaty na fakturę, należy zsumować **wartość kolumny kwota** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="0b808-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="0b808-149">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="0b808-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="0b808-150">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="0b808-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="0b808-151">Nowy</span><span class="sxs-lookup"><span data-stu-id="0b808-151">New</span></span> | <span data-ttu-id="0b808-152">Używany podczas tworzenia nowego zakupu.</span><span class="sxs-lookup"><span data-stu-id="0b808-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="0b808-153">addilooć</span><span class="sxs-lookup"><span data-stu-id="0b808-153">addQuantity</span></span> | <span data-ttu-id="0b808-154">Używany w refund oryginalnego zakupu i nowej ilości po zwiększeniu.</span><span class="sxs-lookup"><span data-stu-id="0b808-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="0b808-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="0b808-155">removeQuantity</span></span> | <span data-ttu-id="0b808-156">Używany w refund oryginalnego zakupu i nowej ilości po zmniejszeniu.</span><span class="sxs-lookup"><span data-stu-id="0b808-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="0b808-157">Anuluj</span><span class="sxs-lookup"><span data-stu-id="0b808-157">Cancel</span></span> | <span data-ttu-id="0b808-158">Używany, gdy subskrypcja została anulowana.</span><span class="sxs-lookup"><span data-stu-id="0b808-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="0b808-159">Convert</span><span class="sxs-lookup"><span data-stu-id="0b808-159">Convert</span></span> | <span data-ttu-id="0b808-160">Używany podczas uaktualniania licencji, ale liczba licencji pozostaje niezmieniona.</span><span class="sxs-lookup"><span data-stu-id="0b808-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="0b808-161">Opłaty za zużycie</span><span class="sxs-lookup"><span data-stu-id="0b808-161">Usage charges</span></span>

<span data-ttu-id="0b808-162">Aby zmapować te opłaty za korzystanie z faktury, należy zsumować kolumny **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="0b808-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="0b808-163">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="0b808-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="0b808-164">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="0b808-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="0b808-165">Oceń opłatę za użycie po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="0b808-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="0b808-166">Uzyskaj dostęp do opłat za użycie w przypadku anulowania Niepłatnego użycia w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="0b808-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="0b808-167">Ocenianie opłaty za użycie dla bieżącego cyklu</span><span class="sxs-lookup"><span data-stu-id="0b808-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="0b808-168">Opłata za użycie w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="0b808-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="0b808-169">Środki</span><span class="sxs-lookup"><span data-stu-id="0b808-169">Credits</span></span>

<span data-ttu-id="0b808-170">Aby zamapować te kredyty na fakturę:</span><span class="sxs-lookup"><span data-stu-id="0b808-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="0b808-171">Zasumuj **TotalForCustomer** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="0b808-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="0b808-172">Suma kolumny **PostTaxTotal** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="0b808-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="0b808-173">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="0b808-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="0b808-174">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="0b808-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="0b808-175">Przesunięcie elementu wiersza</span><span class="sxs-lookup"><span data-stu-id="0b808-175">Offset a line item</span></span> | <span data-ttu-id="0b808-176">Częściowe lub całkowite zwrotne do elementu wiersza, w tym podatki.</span><span class="sxs-lookup"><span data-stu-id="0b808-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="0b808-177">Rabaty oparte na użyciu</span><span class="sxs-lookup"><span data-stu-id="0b808-177">Usage-based discounts</span></span>

<span data-ttu-id="0b808-178">Aby zmapować te rabaty oparte na użyciu na fakturze, należy zsumować kolumny **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="0b808-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="0b808-179">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="0b808-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="0b808-180">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="0b808-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="0b808-181">Rabat aktywacji</span><span class="sxs-lookup"><span data-stu-id="0b808-181">Activation discount</span></span> | <span data-ttu-id="0b808-182">Rabat stosowany po aktywowaniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="0b808-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="0b808-183">Rabat dla cyklu</span><span class="sxs-lookup"><span data-stu-id="0b808-183">Cycle discount</span></span> | <span data-ttu-id="0b808-184">Rabat stosowany do opłat okresowych.</span><span class="sxs-lookup"><span data-stu-id="0b808-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="0b808-185">Odnów rabat</span><span class="sxs-lookup"><span data-stu-id="0b808-185">Renew discount</span></span> | <span data-ttu-id="0b808-186">Rabat stosowany w przypadku odnowienia subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="0b808-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="0b808-187">Anuluj rabat</span><span class="sxs-lookup"><span data-stu-id="0b808-187">Cancel discount</span></span> | <span data-ttu-id="0b808-188">Opłaty są naliczane po anulowaniu rabatów.</span><span class="sxs-lookup"><span data-stu-id="0b808-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="0b808-189">Rabaty na podstawie licencji</span><span class="sxs-lookup"><span data-stu-id="0b808-189">License-based discounts</span></span>

<span data-ttu-id="0b808-190">Aby zmapować rabaty na podstawie licencji na fakturę, należy zsumować kolumny **TotalOtherDiscount** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="0b808-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="0b808-191">*Rabaty oparte na licencjach mogą być stosowane do wielu typów opłat.*</span><span class="sxs-lookup"><span data-stu-id="0b808-191">*License-based discounts may be applied to multiple charge types.*</span></span>
