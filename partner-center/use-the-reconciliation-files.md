---
title: Korzystanie z plików uzgadniania
ms.topic: article
ms.date: 03/10/2021
description: Dowiedz się więcej na temat plików uzgadniania w centrum partnerskim i interpretacji szczegółowych widoków elementów wierszy opłat dla danego cyklu rozliczeniowego.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022778"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="eacfd-103">Dowiedz się, jak odczytywać elementy wiersza w plikach uzgadniania Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="eacfd-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="eacfd-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="eacfd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="eacfd-105">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="eacfd-105">Billing admin</span></span>
- <span data-ttu-id="eacfd-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="eacfd-106">Global admin</span></span>

<span data-ttu-id="eacfd-107">Pliki uzgadniania można pobrać z Centrum partnerskiego, aby wyświetlić szczegółowy widok elementu z każdą opłatą w cyklu rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="eacfd-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="eacfd-108">Szczegóły elementu wiersza obejmują opłaty dla każdej subskrypcji klienta i szczegółowe zdarzenia (na przykład dodatkowe Dodawanie licencji do subskrypcji).</span><span class="sxs-lookup"><span data-stu-id="eacfd-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="eacfd-109">Aby uzyskać informacje na temat sposobu odczytywania **faktury**, zobacz [odczytywanie rachunku](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="eacfd-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="eacfd-110">Informacje o polach plików uzgadniania</span><span class="sxs-lookup"><span data-stu-id="eacfd-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="eacfd-111">Pola pliku uzgodnień w oparciu o licencję</span><span class="sxs-lookup"><span data-stu-id="eacfd-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="eacfd-112">Pola pliku uzgodnień w oparciu o użycie</span><span class="sxs-lookup"><span data-stu-id="eacfd-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="eacfd-113">Pola pliku uzgodnień dziennego użycia</span><span class="sxs-lookup"><span data-stu-id="eacfd-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="eacfd-114">Pola pliku uzgadniania jednorazowego zakupu dostawcy usług kryptograficznych</span><span class="sxs-lookup"><span data-stu-id="eacfd-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="eacfd-115">Informacje o typach opłat w plikach uzgadniania</span><span class="sxs-lookup"><span data-stu-id="eacfd-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="eacfd-116">Aby zrozumieć typy opłat w plikach uzgadniania (kolumna **opłatatype** ), zobacz temat [typy obciążeń plików uzgadniania](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="eacfd-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="eacfd-117">Rozwiązywanie problemów z formatowaniem</span><span class="sxs-lookup"><span data-stu-id="eacfd-117">Fix formatting issues</span></span>

<span data-ttu-id="eacfd-118">Czasami plik uzgadniania może zawierać problemy z formatowaniem.</span><span class="sxs-lookup"><span data-stu-id="eacfd-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="eacfd-119">Na przykład ten problem może wystąpić, jeśli ustawienia regionalne en-US nie są używane.</span><span class="sxs-lookup"><span data-stu-id="eacfd-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="eacfd-120">Wykonaj następujące kroki, aby naprawić wszelkie problemy z formatowaniem w plikach uzgadniania:</span><span class="sxs-lookup"><span data-stu-id="eacfd-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="eacfd-121">Otwórz plik uzgadniania (w formacie CSV) w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="eacfd-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="eacfd-122">Wybierz pierwszą kolumnę w pliku.</span><span class="sxs-lookup"><span data-stu-id="eacfd-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="eacfd-123">Otwórz **Kreatora konwersji tekstu na kolumny**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="eacfd-124">Na wstążce wybierz pozycję **dane**, a następnie wybierz pozycję **tekst do kolumn**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="eacfd-125">W kreatorze wybierz pozycję **rozdzielany typ pliku**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="eacfd-126">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="eacfd-127">W polu **ograniczników** wybierz **przecinek**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="eacfd-128">(Jeśli **karta** jest już zaznaczona, można opuścić tę opcję). Następnie wybierz przycisk **dalej**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="eacfd-129">W polu **Format danych kolumny** wybierz **datę: MDR**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="eacfd-130">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="eacfd-131">W polu **Format danych kolumny** zaznacz opcję **tekst** dla wszystkich kolumn kwoty.</span><span class="sxs-lookup"><span data-stu-id="eacfd-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="eacfd-132">Następnie wybierz pozycję **Finish** (Zakończ).</span><span class="sxs-lookup"><span data-stu-id="eacfd-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="eacfd-133">Programowe pobieranie plików uzgadniania</span><span class="sxs-lookup"><span data-stu-id="eacfd-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="eacfd-134">Pliki uzgadniania mogą być bardzo duże i czasami trudno je pobrać.</span><span class="sxs-lookup"><span data-stu-id="eacfd-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="eacfd-135">Aby programowo pobrać pliki uzgadniania, zobacz [Pobieranie elementów wiersza faktury](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="eacfd-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="eacfd-136">Podatki mapuje lub VAT</span><span class="sxs-lookup"><span data-stu-id="eacfd-136">Map taxes or VAT</span></span>

<span data-ttu-id="eacfd-137">Aby zmapować podatki lub podatek VAT na fakturę:</span><span class="sxs-lookup"><span data-stu-id="eacfd-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="eacfd-138">Suma wartości kolumny **podatkowej** z pliku opartego na licencji.</span><span class="sxs-lookup"><span data-stu-id="eacfd-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="eacfd-139">Suma kolumny **TaxAmount** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="eacfd-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="eacfd-140">Itemize pliki uzgodnienia według partnera</span><span class="sxs-lookup"><span data-stu-id="eacfd-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="eacfd-141">Partnerzy w **modelu pośrednim** mogą używać tych dodatkowych pól w plikach uzgadniania opartych na licencji i użycia, aby itemize pliki przez odsprzedawcę.</span><span class="sxs-lookup"><span data-stu-id="eacfd-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="eacfd-142">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="eacfd-142">MPN ID</span></span> | <span data-ttu-id="eacfd-143">Opis</span><span class="sxs-lookup"><span data-stu-id="eacfd-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="eacfd-144">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="eacfd-144">MPN ID</span></span> | <span data-ttu-id="eacfd-145">Identyfikator Microsoft Partner Network (MPN) partnera dostawcy rozwiązań w chmurze (bezpośredniego lub pośredniego).</span><span class="sxs-lookup"><span data-stu-id="eacfd-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="eacfd-146">IDENTYFIKATOR MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="eacfd-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="eacfd-147">[Identyfikator MPN odsprzedawcy rekordu dla subskrypcji](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="eacfd-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="eacfd-148">To pole odnosi się do identyfikatora odsprzedawcy wymienionego dla określonej subskrypcji w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="eacfd-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="eacfd-149">Występuje tylko w przypadku plików uzgadniania dla partnerów w modelu pośrednim.</span><span class="sxs-lookup"><span data-stu-id="eacfd-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="eacfd-150">IDENTYFIKATOR MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="eacfd-150">Reseller MPN ID</span></span>

<span data-ttu-id="eacfd-151">Jeśli partner dostawcy usług kryptograficznych sprzedał subskrypcję bezpośrednio do klienta, jego **identyfikator MPN** zostanie wyświetlony dwukrotnie jako **identyfikator MPN** i **identyfikator MPN odsprzedawcy**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="eacfd-152">Jeśli partner CSP ma odsprzedawcę bez **identyfikatora MPN**, ta wartość jest ustawiana na **identyfikator MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="eacfd-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="eacfd-153">Jeśli partner CSP usunie **identyfikator MPN odsprzedawcy**, ta wartość zostanie ustawiona na *-1*.</span><span class="sxs-lookup"><span data-stu-id="eacfd-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="eacfd-154">Aby wyświetlić lub zaktualizować **identyfikator MPN odsprzedawcy**:</span><span class="sxs-lookup"><span data-stu-id="eacfd-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="eacfd-155">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="eacfd-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="eacfd-156">W menu Centrum partnerskiego wybierz pozycję **Customers**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="eacfd-157">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="eacfd-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="eacfd-158">W menu Klient wybierz pozycję **subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="eacfd-159">Wybierz subskrypcję z listy.</span><span class="sxs-lookup"><span data-stu-id="eacfd-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="eacfd-160">Wybierz pozycję **Aktualizuj** , aby zmienić **ODSPRZEDAWCA (identyfikator MPN)**.</span><span class="sxs-lookup"><span data-stu-id="eacfd-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eacfd-161">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eacfd-161">Next steps</span></span>

- [<span data-ttu-id="eacfd-162">Jak odczytać rozliczenie & pliku Rekonesans</span><span class="sxs-lookup"><span data-stu-id="eacfd-162">How to read your bill & recon file</span></span>](read-your-bill.md) 