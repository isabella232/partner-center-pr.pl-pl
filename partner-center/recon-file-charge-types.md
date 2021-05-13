---
title: Typy opłat za pliki uzgodnień
ms.topic: article
ms.date: 06/05/2020
description: Zapoznaj się z typami opłat (na przykład opartymi na licencjach, opartymi na użyciu i jednym czasem), kredytami i rabatami w Partner Center uzgadniania.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855883"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="24de5-103">Opis różnych typów opłat w plikach Partner Center uzgodnień</span><span class="sxs-lookup"><span data-stu-id="24de5-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="24de5-104">**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="24de5-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="24de5-105">**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="24de5-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="24de5-106">W tym artykule opisano mapowania między sekcją faktury i skojarzonymi typami opłat, które mogą być w pliku uzgodnień.</span><span class="sxs-lookup"><span data-stu-id="24de5-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="24de5-107">Faktura zawiera podsumowanie opłat.</span><span class="sxs-lookup"><span data-stu-id="24de5-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="24de5-108">Plik uzgodnień zawiera szczegółowy podział transakcji elementów wiersza, w tym typy opłat.</span><span class="sxs-lookup"><span data-stu-id="24de5-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="24de5-109">Aby uzyskać więcej informacji na temat plików uzgodnień, zobacz [jak używać plików uzgodnień](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="24de5-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="24de5-110">Zarówno [pliki uzgodnień oparte na](usage-based-recon-files.md) użyciu, jak i pliki uzgodnień oparte na licencjach pokazują tylko transakcje i opłaty związane z użyciem (zużyte jednostki i powiązane opłaty). [](license-based-recon-files.md)</span><span class="sxs-lookup"><span data-stu-id="24de5-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="24de5-111">Środki, rabaty lub zwroty, które są  wyświetlane na fakturze jako Korekty, nie są wyświetlane w pliku uzgodnień.</span><span class="sxs-lookup"><span data-stu-id="24de5-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="24de5-112">Mapowanie typów opłat na opłaty na podstawie faktur</span><span class="sxs-lookup"><span data-stu-id="24de5-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="24de5-113">Aby odwoływać się do kwot opłat między fakturą i plikiem uzgodnień, użyj opcji filtrowania w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="24de5-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="24de5-114">Filtruj według typów opłat w pliku uzgodnień, aby zamapować opłaty na zestaw podziałów opłat w pliku uzgodnień.</span><span class="sxs-lookup"><span data-stu-id="24de5-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="24de5-115">Opłaty na podstawie licencji</span><span class="sxs-lookup"><span data-stu-id="24de5-115">License-based charges</span></span>

<span data-ttu-id="24de5-116">Aby zamapować te opłaty na podstawie licencji na fakturę, zsuń **kolumnę Amount** (Kwota) z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="24de5-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="24de5-117">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="24de5-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24de5-118">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="24de5-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24de5-119">Opłata za aktywację</span><span class="sxs-lookup"><span data-stu-id="24de5-119">Activation fee</span></span> | <span data-ttu-id="24de5-120">Kwota naliczana klientowi podczas korzystania z subskrypcji po zakupie.</span><span class="sxs-lookup"><span data-stu-id="24de5-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="24de5-121">Anulowanie opłaty</span><span class="sxs-lookup"><span data-stu-id="24de5-121">Cancel fee</span></span> | <span data-ttu-id="24de5-122">Naliczane proporcjonalnie opłaty są zwracane klientowi po zmianie skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="24de5-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="24de5-123">Anulowanie prorate wystąpienia</span><span class="sxs-lookup"><span data-stu-id="24de5-123">Cancel instance prorate</span></span> | <span data-ttu-id="24de5-124">Opłaty proporcjonalnie anulowane, gdy klient z subskrypcją miesięczną ma wstrzymaną subskrypcję i skojarzone licencje zmieniły się w ciągu tego samego miesiąca.</span><span class="sxs-lookup"><span data-stu-id="24de5-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="24de5-125">Opłata za cykl</span><span class="sxs-lookup"><span data-stu-id="24de5-125">Cycle fee</span></span> | <span data-ttu-id="24de5-126">Okresowe opłaty za subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="24de5-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="24de5-127">Cykl prorate wystąpienia</span><span class="sxs-lookup"><span data-stu-id="24de5-127">Cycle instance prorate</span></span> | <span data-ttu-id="24de5-128">Naliczane proporcjonalnie opłaty naliczane od klienta w przypadku zmiany skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="24de5-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="24de5-129">Naliczanie opłat po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="24de5-129">Prorate fees when cancel</span></span> | <span data-ttu-id="24de5-130">Proporcjonalny zwrot za nieużywaną część usługi po anulowaniu.</span><span class="sxs-lookup"><span data-stu-id="24de5-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="24de5-131">Naliczanie opłat w przypadku konwersji poza bieżącą ofertę</span><span class="sxs-lookup"><span data-stu-id="24de5-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="24de5-132">Opłaty naliczane proporcjonalnie po konwersji z bieżącej miesięcznej subskrypcji na roczną subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="24de5-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="24de5-133">Naliczanie opłat w przypadku konwersji na nową ofertę</span><span class="sxs-lookup"><span data-stu-id="24de5-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="24de5-134">Opłaty naliczane proporcjonalnie po przekonwertowaniu miesięcznej subskrypcji na nową roczną subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="24de5-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="24de5-135">Naliczanie opłat podczas zakupu</span><span class="sxs-lookup"><span data-stu-id="24de5-135">Prorate fees when purchase</span></span> | <span data-ttu-id="24de5-136">Typ opłaty za subskrypcję w przypadku korzystania z rozliczeń miesięcznych lub rocznych.</span><span class="sxs-lookup"><span data-stu-id="24de5-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="24de5-137">Opłata prorate podczas odnawiania</span><span class="sxs-lookup"><span data-stu-id="24de5-137">Prorate fee when renew</span></span> | <span data-ttu-id="24de5-138">Opłaty proporcjonalnie po odnowieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="24de5-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="24de5-139">Odnawianie opłaty</span><span class="sxs-lookup"><span data-stu-id="24de5-139">Renew fee</span></span> | <span data-ttu-id="24de5-140">Opłata za odnowienie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="24de5-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="24de5-141">Naliczanie opłat po aktywowaniu</span><span class="sxs-lookup"><span data-stu-id="24de5-141">Prorate fees when activate</span></span> | <span data-ttu-id="24de5-142">Opłaty naliczane proporcjonalnie od aktywacji do końca okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="24de5-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="24de5-143">Opłaty terminowe</span><span class="sxs-lookup"><span data-stu-id="24de5-143">One-time charges</span></span>

<span data-ttu-id="24de5-144">Aby zamapować te opłaty raz na fakturę, zsuń **kolumnę Amount** (Kwota) z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="24de5-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="24de5-145">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="24de5-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24de5-146">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="24de5-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24de5-147">Nowy</span><span class="sxs-lookup"><span data-stu-id="24de5-147">New</span></span> | <span data-ttu-id="24de5-148">Używany podczas tworzenia nowego zakupu.</span><span class="sxs-lookup"><span data-stu-id="24de5-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="24de5-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="24de5-149">addQuantity</span></span> | <span data-ttu-id="24de5-150">Używane zarówno w przypadku zwrotu pierwotnego zakupu, jak i nowej ilości po zwiększeniu.</span><span class="sxs-lookup"><span data-stu-id="24de5-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="24de5-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="24de5-151">removeQuantity</span></span> | <span data-ttu-id="24de5-152">Używane zarówno w przypadku zwrotu pierwotnego zakupu, jak i nowej ilości po zmniejszeniu.</span><span class="sxs-lookup"><span data-stu-id="24de5-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="24de5-153">Anuluj</span><span class="sxs-lookup"><span data-stu-id="24de5-153">Cancel</span></span> | <span data-ttu-id="24de5-154">Używane po anulowaniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="24de5-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="24de5-155">Convert</span><span class="sxs-lookup"><span data-stu-id="24de5-155">Convert</span></span> | <span data-ttu-id="24de5-156">Używany podczas uaktualnienia licencji, ale liczba licencji pozostaje niezmieniona.</span><span class="sxs-lookup"><span data-stu-id="24de5-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="24de5-157">Opłaty za zużycie</span><span class="sxs-lookup"><span data-stu-id="24de5-157">Usage charges</span></span>

<span data-ttu-id="24de5-158">Aby zamapować te opłaty za użycie na fakturę, zsuń kolumnę **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="24de5-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="24de5-159">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="24de5-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24de5-160">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="24de5-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24de5-161">Ocenianie opłaty za użycie po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="24de5-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="24de5-162">Uzyskaj dostęp do opłaty za użycie po anulowaniu za niezapłacone użycie w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="24de5-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="24de5-163">Ocena opłaty za użycie dla bieżącego cyklu</span><span class="sxs-lookup"><span data-stu-id="24de5-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="24de5-164">Dostęp do opłaty za użycie w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="24de5-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="24de5-165">Środki</span><span class="sxs-lookup"><span data-stu-id="24de5-165">Credits</span></span>

<span data-ttu-id="24de5-166">Aby zamapować te środki na fakturę:</span><span class="sxs-lookup"><span data-stu-id="24de5-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="24de5-167">**Zsumuj wartość TotalForCustomer** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="24de5-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="24de5-168">Zsuń kolumnę **PostTaxTotal** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="24de5-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="24de5-169">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="24de5-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24de5-170">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="24de5-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24de5-171">Przesunięcie elementu wiersza</span><span class="sxs-lookup"><span data-stu-id="24de5-171">Offset a line item</span></span> | <span data-ttu-id="24de5-172">Częściowy lub cały zwrot do pozycji, w tym podatki.</span><span class="sxs-lookup"><span data-stu-id="24de5-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="24de5-173">Rabaty oparte na użyciu</span><span class="sxs-lookup"><span data-stu-id="24de5-173">Usage-based discounts</span></span>

<span data-ttu-id="24de5-174">Aby zamapować te rabaty na podstawie użycia na fakturę, zsuń kolumnę **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="24de5-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="24de5-175">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="24de5-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24de5-176">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="24de5-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24de5-177">Rabat na aktywację</span><span class="sxs-lookup"><span data-stu-id="24de5-177">Activation discount</span></span> | <span data-ttu-id="24de5-178">Rabat stosowany po aktywowaniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="24de5-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="24de5-179">Rabat na cykl</span><span class="sxs-lookup"><span data-stu-id="24de5-179">Cycle discount</span></span> | <span data-ttu-id="24de5-180">Rabat stosowany do okresowych opłat.</span><span class="sxs-lookup"><span data-stu-id="24de5-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="24de5-181">Odnawianie rabatu</span><span class="sxs-lookup"><span data-stu-id="24de5-181">Renew discount</span></span> | <span data-ttu-id="24de5-182">Rabat stosowany po odnowieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="24de5-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="24de5-183">Anulowanie rabatu</span><span class="sxs-lookup"><span data-stu-id="24de5-183">Cancel discount</span></span> | <span data-ttu-id="24de5-184">Opłaty stosowane w przypadku anulowania rabatów.</span><span class="sxs-lookup"><span data-stu-id="24de5-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="24de5-185">Rabaty oparte na licencjach</span><span class="sxs-lookup"><span data-stu-id="24de5-185">License-based discounts</span></span>

<span data-ttu-id="24de5-186">Aby zamapować rabaty na podstawie licencji na fakturę, zsumuj kolumnę **TotalOtherDiscount** z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="24de5-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="24de5-187">*Rabaty oparte na licencjach mogą być stosowane do wielu typów opłat.*</span><span class="sxs-lookup"><span data-stu-id="24de5-187">*License-based discounts may be applied to multiple charge types.*</span></span>
