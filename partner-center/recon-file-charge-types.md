---
title: Typy opłat za pliki uzgadniania
ms.topic: article
ms.date: 06/05/2020
description: Wykrywaj typy opłat (takie jak oparte na licencji, oparte na użyciu i jednorazowe), kredyty i rabaty w plikach uzgadniania Centrum partnerskiego.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/31/2020
ms.locfileid: "92529389"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="5a270-103">Informacje o różnych typach opłat w plikach uzgadniania Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="5a270-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="5a270-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="5a270-104">**Applies to**</span></span>

- <span data-ttu-id="5a270-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="5a270-105">Partner Center</span></span>
- <span data-ttu-id="5a270-106">Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA</span><span class="sxs-lookup"><span data-stu-id="5a270-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="5a270-107">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="5a270-107">**Appropriate roles**</span></span>

- <span data-ttu-id="5a270-108">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="5a270-108">Admin agent</span></span>
- <span data-ttu-id="5a270-109">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="5a270-109">Billing admin</span></span>
- <span data-ttu-id="5a270-110">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="5a270-110">Global admin</span></span>

<span data-ttu-id="5a270-111">W tym temacie opisano mapowania między sekcją faktury i skojarzonymi typami opłat, które mogą znajdować się w pliku uzgadniania.</span><span class="sxs-lookup"><span data-stu-id="5a270-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="5a270-112">Faktura zawiera podsumowanie opłat.</span><span class="sxs-lookup"><span data-stu-id="5a270-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="5a270-113">Plik uzgadniania zawiera szczegółowy podział transakcji elementu wiersza, w tym typów opłat.</span><span class="sxs-lookup"><span data-stu-id="5a270-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="5a270-114">Aby uzyskać więcej informacji dotyczących plików uzgadniania, zobacz [jak używać plików uzgadniania](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="5a270-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="5a270-115">W przypadku [plików uzgadniania opartych na użyciu](usage-based-recon-files.md) i [plików uzgadniania opartych na licencji](license-based-recon-files.md) są wyświetlane tylko transakcje związane z użyciem i opłaty (zużyte jednostki i powiązane opłaty).</span><span class="sxs-lookup"><span data-stu-id="5a270-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="5a270-116">Kredyty jednorazowe, zniżki lub zwroty, które są wyświetlane na fakturze, jako **korekty** nie są wyświetlane w pliku uzgadniania.</span><span class="sxs-lookup"><span data-stu-id="5a270-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="5a270-117">Mapuj typy opłat na faktury</span><span class="sxs-lookup"><span data-stu-id="5a270-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="5a270-118">Aby uzyskać informacje o opłatach za odwołania między fakturą i plikiem uzgadniania, użyj opcji filtru w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="5a270-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="5a270-119">Filtruj według typów opłat w pliku uzgadniania, aby zamapować opłaty za faktury na zestaw podziałów opłat w pliku uzgadniania.</span><span class="sxs-lookup"><span data-stu-id="5a270-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="5a270-120">Opłaty oparte na licencji</span><span class="sxs-lookup"><span data-stu-id="5a270-120">License-based charges</span></span>

<span data-ttu-id="5a270-121">Aby zmapować opłaty na podstawie licencji na fakturę, należy zsumować **wartość kolumny kwota** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="5a270-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="5a270-122">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="5a270-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5a270-123">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="5a270-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5a270-124">Opłata za aktywację</span><span class="sxs-lookup"><span data-stu-id="5a270-124">Activation fee</span></span> | <span data-ttu-id="5a270-125">Kwota naliczana dla klienta w przypadku korzystania z subskrypcji po zakupie.</span><span class="sxs-lookup"><span data-stu-id="5a270-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="5a270-126">Opłata za anulowanie</span><span class="sxs-lookup"><span data-stu-id="5a270-126">Cancel fee</span></span> | <span data-ttu-id="5a270-127">Opłata naliczana proporcjonalnie do klienta po zmianie skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="5a270-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="5a270-128">Anuluj częstotliwość wystąpień</span><span class="sxs-lookup"><span data-stu-id="5a270-128">Cancel instance prorate</span></span> | <span data-ttu-id="5a270-129">Opłata naliczana proporcjonalnie do liczby dni, gdy klient z subskrypcją miesięczną ma zawieszoną subskrypcję, a skojarzone licencje zmieniają się w tym samym miesiącu.</span><span class="sxs-lookup"><span data-stu-id="5a270-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="5a270-130">Opłata za cykl</span><span class="sxs-lookup"><span data-stu-id="5a270-130">Cycle fee</span></span> | <span data-ttu-id="5a270-131">Opłaty okresowe za subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="5a270-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="5a270-132">Tempo wystąpienia cyklu</span><span class="sxs-lookup"><span data-stu-id="5a270-132">Cycle instance prorate</span></span> | <span data-ttu-id="5a270-133">Opłata naliczana proporcjonalnie do liczby opłat naliczanych od klienta po zmianie skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="5a270-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="5a270-134">Oceń opłaty po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="5a270-134">Prorate fees when cancel</span></span> | <span data-ttu-id="5a270-135">Naoprocentowanie proporcjonalnie do nieużywanej części usługi po anulowaniu.</span><span class="sxs-lookup"><span data-stu-id="5a270-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="5a270-136">Opłata proporcjonalna za konwersję z bieżącej oferty</span><span class="sxs-lookup"><span data-stu-id="5a270-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="5a270-137">Naliczanie opłat naliczane po przeprowadzeniu konwersji z bieżącej subskrypcji miesięcznej na roczną subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="5a270-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="5a270-138">Opłaty naliczane za konwersję na nową ofertę</span><span class="sxs-lookup"><span data-stu-id="5a270-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="5a270-139">Opłaty naliczane proporcjonalnie po przeprowadzeniu konwersji miesięcznej subskrypcji na nową roczną subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="5a270-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="5a270-140">Opłata proporcjonalna przy zakupie</span><span class="sxs-lookup"><span data-stu-id="5a270-140">Prorate fees when purchase</span></span> | <span data-ttu-id="5a270-141">Typ opłaty dla subskrypcji w przypadku comiesięcznego lub rocznego rozliczania.</span><span class="sxs-lookup"><span data-stu-id="5a270-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="5a270-142">Opłata proporcjonalna przy odnowieniu</span><span class="sxs-lookup"><span data-stu-id="5a270-142">Prorate fee when renew</span></span> | <span data-ttu-id="5a270-143">Opłata naliczana proporcjonalnie przy odnowieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="5a270-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="5a270-144">Odnawianie opłaty</span><span class="sxs-lookup"><span data-stu-id="5a270-144">Renew fee</span></span> | <span data-ttu-id="5a270-145">Opłata za odnowienie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="5a270-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="5a270-146">Oceń opłaty przy aktywacji</span><span class="sxs-lookup"><span data-stu-id="5a270-146">Prorate fees when activate</span></span> | <span data-ttu-id="5a270-147">Opłata naliczana proporcjonalnie od aktywacji do końca okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="5a270-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="5a270-148">Opłaty jednorazowe</span><span class="sxs-lookup"><span data-stu-id="5a270-148">One-time charges</span></span>

<span data-ttu-id="5a270-149">Aby zmapować te jednorazowe opłaty na fakturę, należy zsumować **wartość kolumny kwota** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="5a270-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="5a270-150">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="5a270-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5a270-151">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="5a270-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5a270-152">Nowy</span><span class="sxs-lookup"><span data-stu-id="5a270-152">New</span></span> | <span data-ttu-id="5a270-153">Używany podczas tworzenia nowego zakupu.</span><span class="sxs-lookup"><span data-stu-id="5a270-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="5a270-154">addilooć</span><span class="sxs-lookup"><span data-stu-id="5a270-154">addQuantity</span></span> | <span data-ttu-id="5a270-155">Używany w refund oryginalnego zakupu i nowej ilości po zwiększeniu.</span><span class="sxs-lookup"><span data-stu-id="5a270-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="5a270-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="5a270-156">removeQuantity</span></span> | <span data-ttu-id="5a270-157">Używany w refund oryginalnego zakupu i nowej ilości po zmniejszeniu.</span><span class="sxs-lookup"><span data-stu-id="5a270-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="5a270-158">Anuluj</span><span class="sxs-lookup"><span data-stu-id="5a270-158">Cancel</span></span> | <span data-ttu-id="5a270-159">Używany, gdy subskrypcja została anulowana.</span><span class="sxs-lookup"><span data-stu-id="5a270-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="5a270-160">Convert</span><span class="sxs-lookup"><span data-stu-id="5a270-160">Convert</span></span> | <span data-ttu-id="5a270-161">Używany podczas uaktualniania licencji, ale liczba licencji pozostaje niezmieniona.</span><span class="sxs-lookup"><span data-stu-id="5a270-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="5a270-162">Opłaty za zużycie</span><span class="sxs-lookup"><span data-stu-id="5a270-162">Usage charges</span></span>

<span data-ttu-id="5a270-163">Aby zmapować te opłaty za korzystanie z faktury, należy zsumować kolumny **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="5a270-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="5a270-164">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="5a270-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5a270-165">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="5a270-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5a270-166">Oceń opłatę za użycie po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="5a270-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="5a270-167">Uzyskaj dostęp do opłat za użycie w przypadku anulowania Niepłatnego użycia w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="5a270-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="5a270-168">Ocenianie opłaty za użycie dla bieżącego cyklu</span><span class="sxs-lookup"><span data-stu-id="5a270-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="5a270-169">Opłata za użycie w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="5a270-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="5a270-170">Środki</span><span class="sxs-lookup"><span data-stu-id="5a270-170">Credits</span></span>

<span data-ttu-id="5a270-171">Aby zamapować te kredyty na fakturę:</span><span class="sxs-lookup"><span data-stu-id="5a270-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="5a270-172">Zasumuj **TotalForCustomer** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="5a270-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="5a270-173">Suma kolumny **PostTaxTotal** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="5a270-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="5a270-174">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="5a270-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5a270-175">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="5a270-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5a270-176">Przesunięcie elementu wiersza</span><span class="sxs-lookup"><span data-stu-id="5a270-176">Offset a line item</span></span> | <span data-ttu-id="5a270-177">Częściowe lub całkowite zwrotne do elementu wiersza, w tym podatki.</span><span class="sxs-lookup"><span data-stu-id="5a270-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="5a270-178">Rabaty oparte na użyciu</span><span class="sxs-lookup"><span data-stu-id="5a270-178">Usage-based discounts</span></span>

<span data-ttu-id="5a270-179">Aby zmapować te rabaty oparte na użyciu na fakturze, należy zsumować kolumny **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="5a270-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="5a270-180">Opis opłaty (kolumna opłaty) w pliku uzgadniania</span><span class="sxs-lookup"><span data-stu-id="5a270-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5a270-181">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="5a270-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5a270-182">Rabat aktywacji</span><span class="sxs-lookup"><span data-stu-id="5a270-182">Activation discount</span></span> | <span data-ttu-id="5a270-183">Rabat stosowany po aktywowaniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="5a270-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="5a270-184">Rabat dla cyklu</span><span class="sxs-lookup"><span data-stu-id="5a270-184">Cycle discount</span></span> | <span data-ttu-id="5a270-185">Rabat stosowany do opłat okresowych.</span><span class="sxs-lookup"><span data-stu-id="5a270-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="5a270-186">Odnów rabat</span><span class="sxs-lookup"><span data-stu-id="5a270-186">Renew discount</span></span> | <span data-ttu-id="5a270-187">Rabat stosowany w przypadku odnowienia subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="5a270-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="5a270-188">Anuluj rabat</span><span class="sxs-lookup"><span data-stu-id="5a270-188">Cancel discount</span></span> | <span data-ttu-id="5a270-189">Opłaty są naliczane po anulowaniu rabatów.</span><span class="sxs-lookup"><span data-stu-id="5a270-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="5a270-190">Rabaty na podstawie licencji</span><span class="sxs-lookup"><span data-stu-id="5a270-190">License-based discounts</span></span>

<span data-ttu-id="5a270-191">Aby zmapować rabaty na podstawie licencji na fakturę, należy zsumować kolumny **TotalOtherDiscount** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="5a270-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="5a270-192">*Rabaty oparte na licencjach mogą być stosowane do wielu typów opłat.*</span><span class="sxs-lookup"><span data-stu-id="5a270-192">*License-based discounts may be applied to multiple charge types.*</span></span>
