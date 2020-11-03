---
title: Korzystanie z plików uzgadniania
ms.topic: article
ms.date: 06/08/2020
description: Dowiedz się więcej na temat plików uzgadniania w centrum partnerskim i interpretacji szczegółowych widoków elementów wierszy opłat dla danego cyklu rozliczeniowego.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529854"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="655ac-103">Dowiedz się, jak odczytywać elementy wiersza w plikach uzgadniania Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="655ac-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="655ac-104">Dotyczy:</span><span class="sxs-lookup"><span data-stu-id="655ac-104">Applies to:</span></span>

- <span data-ttu-id="655ac-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="655ac-105">Partner Center</span></span>
- <span data-ttu-id="655ac-106">Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA</span><span class="sxs-lookup"><span data-stu-id="655ac-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="655ac-107">Pliki uzgadniania można pobrać z Centrum partnerskiego, aby wyświetlić szczegółowy widok elementu z każdą opłatą w cyklu rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="655ac-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="655ac-108">Szczegóły elementu wiersza obejmują opłaty dla każdej subskrypcji klienta i szczegółowe zdarzenia (na przykład dodatkowe Dodawanie licencji do subskrypcji).</span><span class="sxs-lookup"><span data-stu-id="655ac-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="655ac-109">Odpowiednie role:</span><span class="sxs-lookup"><span data-stu-id="655ac-109">Appropriate roles:</span></span>

- <span data-ttu-id="655ac-110">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="655ac-110">Billing admin</span></span>
- <span data-ttu-id="655ac-111">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="655ac-111">Global admin</span></span>

<span data-ttu-id="655ac-112">Aby uzyskać informacje na temat sposobu odczytywania **faktury** , zobacz [odczytywanie rachunku](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="655ac-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="655ac-113">Informacje o polach plików uzgadniania</span><span class="sxs-lookup"><span data-stu-id="655ac-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="655ac-114">Pola pliku uzgadniania opartego na licencji</span><span class="sxs-lookup"><span data-stu-id="655ac-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="655ac-115">Pola pliku uzgadniania opartego na użyciu</span><span class="sxs-lookup"><span data-stu-id="655ac-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="655ac-116">Pola plików uzgadniania dziennego użycia z oceną</span><span class="sxs-lookup"><span data-stu-id="655ac-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="655ac-117">Informacje o typach opłat w plikach uzgadniania</span><span class="sxs-lookup"><span data-stu-id="655ac-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="655ac-118">Aby zrozumieć typy opłat w plikach uzgadniania (kolumna **opłatatype** ), zobacz temat [typy obciążeń plików uzgadniania](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="655ac-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="655ac-119">Rozwiązywanie problemów z formatowaniem</span><span class="sxs-lookup"><span data-stu-id="655ac-119">Fix formatting issues</span></span>

<span data-ttu-id="655ac-120">Czasami plik uzgadniania może zawierać problemy z formatowaniem.</span><span class="sxs-lookup"><span data-stu-id="655ac-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="655ac-121">Na przykład ten problem może wystąpić, jeśli ustawienia regionalne en-US nie są używane.</span><span class="sxs-lookup"><span data-stu-id="655ac-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="655ac-122">Wykonaj następujące kroki, aby naprawić wszelkie problemy z formatowaniem w plikach uzgadniania:</span><span class="sxs-lookup"><span data-stu-id="655ac-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="655ac-123">Otwórz plik uzgadniania (w formacie CSV) w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="655ac-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="655ac-124">Wybierz pierwszą kolumnę w pliku.</span><span class="sxs-lookup"><span data-stu-id="655ac-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="655ac-125">Otwórz **Kreatora konwersji tekstu na kolumny**.</span><span class="sxs-lookup"><span data-stu-id="655ac-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="655ac-126">Na wstążce wybierz pozycję **dane** , a następnie wybierz pozycję **tekst do kolumn**.</span><span class="sxs-lookup"><span data-stu-id="655ac-126">On the ribbon, select **Data** , then select **Text to Columns**.</span></span>
4. <span data-ttu-id="655ac-127">W kreatorze wybierz pozycję **rozdzielany typ pliku**.</span><span class="sxs-lookup"><span data-stu-id="655ac-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="655ac-128">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="655ac-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="655ac-129">W polu **ograniczników** wybierz **przecinek**.</span><span class="sxs-lookup"><span data-stu-id="655ac-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="655ac-130">(Jeśli **karta** jest już zaznaczona, można opuścić tę opcję). Następnie wybierz przycisk **dalej**.</span><span class="sxs-lookup"><span data-stu-id="655ac-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="655ac-131">W polu **Format danych kolumny** wybierz **datę: MDR**.</span><span class="sxs-lookup"><span data-stu-id="655ac-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="655ac-132">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="655ac-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="655ac-133">W polu **Format danych kolumny** zaznacz opcję **tekst** dla wszystkich kolumn kwoty.</span><span class="sxs-lookup"><span data-stu-id="655ac-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="655ac-134">Następnie wybierz pozycję **Finish** (Zakończ).</span><span class="sxs-lookup"><span data-stu-id="655ac-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="655ac-135">Programowe pobieranie plików uzgadniania</span><span class="sxs-lookup"><span data-stu-id="655ac-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="655ac-136">Pliki uzgadniania mogą być bardzo duże i czasami trudno je pobrać.</span><span class="sxs-lookup"><span data-stu-id="655ac-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="655ac-137">Aby programowo pobrać pliki uzgadniania, zobacz [Pobieranie elementów wiersza faktury](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="655ac-137">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="655ac-138">Podatki mapuje lub VAT</span><span class="sxs-lookup"><span data-stu-id="655ac-138">Map taxes or VAT</span></span>

<span data-ttu-id="655ac-139">Aby zmapować podatki lub podatek VAT na fakturę:</span><span class="sxs-lookup"><span data-stu-id="655ac-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="655ac-140">Suma wartości kolumny **podatkowej** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="655ac-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="655ac-141">Suma kolumny **TaxAmount** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="655ac-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="655ac-142">Itemize pliki uzgodnienia według partnera</span><span class="sxs-lookup"><span data-stu-id="655ac-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="655ac-143">Partnerzy w **modelu pośrednim** mogą używać tych dodatkowych pól w plikach uzgadniania opartych na licencji i użycia, aby itemize pliki przez odsprzedawcę.</span><span class="sxs-lookup"><span data-stu-id="655ac-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="655ac-144">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="655ac-144">MPN ID</span></span> | <span data-ttu-id="655ac-145">Opis</span><span class="sxs-lookup"><span data-stu-id="655ac-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="655ac-146">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="655ac-146">MPN ID</span></span> | <span data-ttu-id="655ac-147">Identyfikator Microsoft Partner Network (MPN) partnera dostawcy rozwiązań w chmurze (bezpośredniego lub pośredniego).</span><span class="sxs-lookup"><span data-stu-id="655ac-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="655ac-148">IDENTYFIKATOR MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="655ac-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="655ac-149">[Identyfikator MPN odsprzedawcy rekordu dla subskrypcji](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="655ac-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="655ac-150">To pole odnosi się do identyfikatora odsprzedawcy wymienionego dla określonej subskrypcji w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="655ac-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="655ac-151">Występuje tylko w przypadku plików uzgadniania dla partnerów w modelu pośrednim.</span><span class="sxs-lookup"><span data-stu-id="655ac-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="655ac-152">IDENTYFIKATOR MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="655ac-152">Reseller MPN ID</span></span>

<span data-ttu-id="655ac-153">Jeśli partner dostawcy usług kryptograficznych sprzedał subskrypcję bezpośrednio do klienta, jego **identyfikator MPN** zostanie wyświetlony dwukrotnie jako **identyfikator MPN** i **identyfikator MPN odsprzedawcy**.</span><span class="sxs-lookup"><span data-stu-id="655ac-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="655ac-154">Jeśli partner CSP ma odsprzedawcę bez **identyfikatora MPN** , ta wartość jest ustawiana na **identyfikator MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="655ac-154">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="655ac-155">Jeśli partner CSP usunie **identyfikator MPN odsprzedawcy** , ta wartość zostanie ustawiona na *-1*.</span><span class="sxs-lookup"><span data-stu-id="655ac-155">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1*.</span></span>

<span data-ttu-id="655ac-156">Aby wyświetlić lub zaktualizować **identyfikator MPN odsprzedawcy** :</span><span class="sxs-lookup"><span data-stu-id="655ac-156">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="655ac-157">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="655ac-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="655ac-158">W menu Centrum partnerskiego wybierz pozycję **Customers**.</span><span class="sxs-lookup"><span data-stu-id="655ac-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="655ac-159">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="655ac-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="655ac-160">W menu Klient wybierz pozycję **subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="655ac-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="655ac-161">Wybierz subskrypcję z listy.</span><span class="sxs-lookup"><span data-stu-id="655ac-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="655ac-162">Wybierz pozycję **Aktualizuj** , aby zmienić **ODSPRZEDAWCA (identyfikator MPN)**.</span><span class="sxs-lookup"><span data-stu-id="655ac-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>