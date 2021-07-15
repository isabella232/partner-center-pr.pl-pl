---
title: Typy opłat za pliki uzgodnień
ms.topic: article
ms.date: 06/05/2020
description: Informacje o typach opłat (takich jak opłaty oparte na licencjach, na podstawie użycia i jeden raz), środki i rabaty w Partner Center uzgadniania.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989778"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="50ccd-103">Opis różnych typów opłat w plikach Partner Center uzgodnień</span><span class="sxs-lookup"><span data-stu-id="50ccd-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="50ccd-104">**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="50ccd-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="50ccd-105">**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="50ccd-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="50ccd-106">W tym artykule opisano mapowania między sekcją faktury i skojarzonymi typami opłat, które mogą być w pliku uzgodnień.</span><span class="sxs-lookup"><span data-stu-id="50ccd-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="50ccd-107">Faktura zawiera podsumowanie opłat.</span><span class="sxs-lookup"><span data-stu-id="50ccd-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="50ccd-108">Plik uzgodnień zawiera szczegółowy podział transakcji elementów wiersza, w tym typy opłat.</span><span class="sxs-lookup"><span data-stu-id="50ccd-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="50ccd-109">Aby uzyskać więcej informacji na temat plików uzgodnień, zobacz [jak używać plików uzgodnień](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="50ccd-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="50ccd-110">Zarówno [pliki uzgodnień oparte na](usage-based-recon-files.md) użyciu, jak i pliki uzgodnień oparte na licencjach pokazują tylko transakcje i opłaty związane z użyciem (zużyte jednostki i powiązane opłaty). [](license-based-recon-files.md)</span><span class="sxs-lookup"><span data-stu-id="50ccd-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="50ccd-111">Środki, rabaty lub zwroty, które są  wyświetlane na fakturze jako Korekty, nie są wyświetlane w pliku uzgodnień.</span><span class="sxs-lookup"><span data-stu-id="50ccd-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="50ccd-112">Mapowanie typów opłat na opłaty na podstawie faktur</span><span class="sxs-lookup"><span data-stu-id="50ccd-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="50ccd-113">Aby odwoływać się do kwot opłat między fakturą i plikiem uzgodnień, użyj opcji filtrowania w Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="50ccd-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="50ccd-114">Filtruj według typów opłat w pliku uzgodnień, aby zamapować opłaty na faktury na zestaw podziałów opłat w pliku uzgodnień.</span><span class="sxs-lookup"><span data-stu-id="50ccd-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="50ccd-115">Opłaty na podstawie licencji</span><span class="sxs-lookup"><span data-stu-id="50ccd-115">License-based charges</span></span>

<span data-ttu-id="50ccd-116">Aby zamapować te opłaty na podstawie licencji na fakturę, zsuń **kolumnę Amount** (Kwota) z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="50ccd-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="50ccd-117">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="50ccd-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="50ccd-118">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="50ccd-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="50ccd-119">Opłata za aktywację</span><span class="sxs-lookup"><span data-stu-id="50ccd-119">Activation fee</span></span> | <span data-ttu-id="50ccd-120">Kwota naliczana klientowi podczas korzystania z subskrypcji po zakupie.</span><span class="sxs-lookup"><span data-stu-id="50ccd-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="50ccd-121">Anulowanie opłaty</span><span class="sxs-lookup"><span data-stu-id="50ccd-121">Cancel fee</span></span> | <span data-ttu-id="50ccd-122">Naliczane proporcjonalnie opłaty są zwracane klientowi po zmianie skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="50ccd-123">Anulowanie prorate wystąpienia</span><span class="sxs-lookup"><span data-stu-id="50ccd-123">Cancel instance prorate</span></span> | <span data-ttu-id="50ccd-124">Opłaty proporcjonalnie anulowane, gdy klient z subskrypcją miesięczną ma wstrzymaną subskrypcję i skojarzone licencje zmieniły się w ciągu tego samego miesiąca.</span><span class="sxs-lookup"><span data-stu-id="50ccd-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="50ccd-125">Opłata za cykl</span><span class="sxs-lookup"><span data-stu-id="50ccd-125">Cycle fee</span></span> | <span data-ttu-id="50ccd-126">Okresowe opłaty za subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="50ccd-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="50ccd-127">Cykl rozwoju wystąpienia</span><span class="sxs-lookup"><span data-stu-id="50ccd-127">Cycle instance prorate</span></span> | <span data-ttu-id="50ccd-128">Naliczane proporcjonalnie opłaty naliczane od klienta w przypadku zmiany skojarzonych licencji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="50ccd-129">Naliczanie opłat po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="50ccd-129">Prorate fees when cancel</span></span> | <span data-ttu-id="50ccd-130">Proporcjonalny zwrot za nieużywaną część usługi po anulowaniu.</span><span class="sxs-lookup"><span data-stu-id="50ccd-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="50ccd-131">Naliczanie opłat w przypadku konwersji z bieżącej oferty</span><span class="sxs-lookup"><span data-stu-id="50ccd-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="50ccd-132">Opłaty naliczane proporcjonalnie po konwersji z bieżącej miesięcznej subskrypcji na subskrypcję roczną.</span><span class="sxs-lookup"><span data-stu-id="50ccd-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="50ccd-133">Naliczanie opłat podczas konwersji na nową ofertę</span><span class="sxs-lookup"><span data-stu-id="50ccd-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="50ccd-134">Opłaty naliczane proporcjonalnie po przekonwertowaniu miesięcznej subskrypcji na nową roczną subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="50ccd-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="50ccd-135">Naliczanie opłat podczas zakupu</span><span class="sxs-lookup"><span data-stu-id="50ccd-135">Prorate fees when purchase</span></span> | <span data-ttu-id="50ccd-136">Typ opłaty za subskrypcję w przypadku korzystania z rozliczeń miesięcznych lub rocznych.</span><span class="sxs-lookup"><span data-stu-id="50ccd-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="50ccd-137">Opłata prorate podczas odnawiania</span><span class="sxs-lookup"><span data-stu-id="50ccd-137">Prorate fee when renew</span></span> | <span data-ttu-id="50ccd-138">Opłaty naliczane proporcjonalnie po odnowieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="50ccd-139">Odnawianie opłaty</span><span class="sxs-lookup"><span data-stu-id="50ccd-139">Renew fee</span></span> | <span data-ttu-id="50ccd-140">Opłata za odnowienie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="50ccd-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="50ccd-141">Naliczanie opłat po aktywowaniu</span><span class="sxs-lookup"><span data-stu-id="50ccd-141">Prorate fees when activate</span></span> | <span data-ttu-id="50ccd-142">Opłaty proporcjonalnie od aktywacji do końca okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="50ccd-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="50ccd-143">Opłaty terminowe</span><span class="sxs-lookup"><span data-stu-id="50ccd-143">One-time charges</span></span>

<span data-ttu-id="50ccd-144">Aby zamapować te opłaty raz na fakturę, zsuń **kolumnę Amount** (Kwota) z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="50ccd-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="50ccd-145">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="50ccd-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="50ccd-146">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="50ccd-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="50ccd-147">new</span><span class="sxs-lookup"><span data-stu-id="50ccd-147">new</span></span> | <span data-ttu-id="50ccd-148">Używany podczas tworzenia nowego zakupu.</span><span class="sxs-lookup"><span data-stu-id="50ccd-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="50ccd-149">odnawianie</span><span class="sxs-lookup"><span data-stu-id="50ccd-149">renew</span></span> | <span data-ttu-id="50ccd-150">Używany, gdy subskrypcja zostanie odnowiona po zakończeniu okresu.</span><span class="sxs-lookup"><span data-stu-id="50ccd-150">Used when a subscription is renewed after the end of the term.</span></span> |
| <span data-ttu-id="50ccd-151">addQuantity</span><span class="sxs-lookup"><span data-stu-id="50ccd-151">addQuantity</span></span> | <span data-ttu-id="50ccd-152">Używane zarówno w przypadku zwrotu pierwotnego zakupu, jak i nowej ilości po zwiększeniu.</span><span class="sxs-lookup"><span data-stu-id="50ccd-152">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="50ccd-153">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="50ccd-153">removeQuantity</span></span> | <span data-ttu-id="50ccd-154">Używane zarówno w przypadku zwrotu oryginalnego zakupu, jak i nowej ilości po spadku.</span><span class="sxs-lookup"><span data-stu-id="50ccd-154">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="50ccd-155">cancelImmediate</span><span class="sxs-lookup"><span data-stu-id="50ccd-155">cancelImmediate</span></span> | <span data-ttu-id="50ccd-156">Używane po anulowaniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-156">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="50ccd-157">konwertowanie</span><span class="sxs-lookup"><span data-stu-id="50ccd-157">convert</span></span> | <span data-ttu-id="50ccd-158">Używany podczas uaktualnienia licencji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-158">Used when a license is upgraded.</span></span> |
| <span data-ttu-id="50ccd-159">customerCredit</span><span class="sxs-lookup"><span data-stu-id="50ccd-159">customerCredit</span></span> | <span data-ttu-id="50ccd-160">Używane, gdy środki (np. na platformę Azure, umowa SLA itp.) są podawane względem transakcji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-160">Used when credits (e.g., Azure, SLA, etc.) are given against a transaction.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="50ccd-161">Opłaty za zużycie</span><span class="sxs-lookup"><span data-stu-id="50ccd-161">Usage charges</span></span>

<span data-ttu-id="50ccd-162">Aby zamapować te opłaty za użycie na fakturę, zsuń kolumnę **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="50ccd-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="50ccd-163">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="50ccd-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="50ccd-164">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="50ccd-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="50ccd-165">Ocenianie opłaty za użycie po anulowaniu</span><span class="sxs-lookup"><span data-stu-id="50ccd-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="50ccd-166">Uzyskaj dostęp do opłaty za użycie po anulowaniu niezapłaconego użycia w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="50ccd-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="50ccd-167">Ocena opłaty za użycie dla bieżącego cyklu</span><span class="sxs-lookup"><span data-stu-id="50ccd-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="50ccd-168">Dostęp do opłaty za użycie w bieżącym okresie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="50ccd-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="50ccd-169">Środki</span><span class="sxs-lookup"><span data-stu-id="50ccd-169">Credits</span></span>

<span data-ttu-id="50ccd-170">Aby zamapować te środki na fakturę:</span><span class="sxs-lookup"><span data-stu-id="50ccd-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="50ccd-171">**Zsumuj wartość TotalForCustomer** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="50ccd-172">**Zsuń kolumnę PostTaxTotal** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="50ccd-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="50ccd-173">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="50ccd-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="50ccd-174">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="50ccd-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="50ccd-175">Przesunięcie elementu wiersza</span><span class="sxs-lookup"><span data-stu-id="50ccd-175">Offset a line item</span></span> | <span data-ttu-id="50ccd-176">Częściowy lub cały zwrot do pozycji, w tym podatków.</span><span class="sxs-lookup"><span data-stu-id="50ccd-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="50ccd-177">Rabaty na podstawie użycia</span><span class="sxs-lookup"><span data-stu-id="50ccd-177">Usage-based discounts</span></span>

<span data-ttu-id="50ccd-178">Aby zamapować te rabaty na podstawie użycia na fakturę, zsuń kolumnę **PretaxCharges** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="50ccd-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="50ccd-179">Opis opłaty (kolumna ChargeType w pliku uzgodnień)</span><span class="sxs-lookup"><span data-stu-id="50ccd-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="50ccd-180">Wyjaśnienie opłaty</span><span class="sxs-lookup"><span data-stu-id="50ccd-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="50ccd-181">Rabat na aktywację</span><span class="sxs-lookup"><span data-stu-id="50ccd-181">Activation discount</span></span> | <span data-ttu-id="50ccd-182">Rabat stosowany po aktywowaniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="50ccd-183">Rabat na cykl</span><span class="sxs-lookup"><span data-stu-id="50ccd-183">Cycle discount</span></span> | <span data-ttu-id="50ccd-184">Rabat zastosowany do okresowych opłat.</span><span class="sxs-lookup"><span data-stu-id="50ccd-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="50ccd-185">Odnawianie rabatu</span><span class="sxs-lookup"><span data-stu-id="50ccd-185">Renew discount</span></span> | <span data-ttu-id="50ccd-186">Rabat stosowany po odnowieniu subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="50ccd-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="50ccd-187">Anulowanie rabatu</span><span class="sxs-lookup"><span data-stu-id="50ccd-187">Cancel discount</span></span> | <span data-ttu-id="50ccd-188">Opłaty naliczane po anulowaniu rabatów.</span><span class="sxs-lookup"><span data-stu-id="50ccd-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="50ccd-189">Rabaty oparte na licencjach</span><span class="sxs-lookup"><span data-stu-id="50ccd-189">License-based discounts</span></span>

<span data-ttu-id="50ccd-190">Aby zamapować rabaty na podstawie licencji na fakturę, zsumuj kolumnę **TotalOtherDiscount** z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="50ccd-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="50ccd-191">*Rabaty oparte na licencjach mogą być stosowane do wielu typów opłat.*</span><span class="sxs-lookup"><span data-stu-id="50ccd-191">*License-based discounts may be applied to multiple charge types.*</span></span>
