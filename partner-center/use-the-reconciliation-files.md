---
title: Korzystanie z plików uzgodnień
ms.topic: article
ms.date: 03/26/2021
description: Dowiedz się więcej o plikach uzgodnień Partner Center i interpretowaniu szczegółowych widoków elementów wiersza opłat dla danego cyklu rozliczeniowego.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794959"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="3d6b6-103">Dowiedz się, jak odczytywać elementy wiersza w plikach Partner Center uzgodnień</span><span class="sxs-lookup"><span data-stu-id="3d6b6-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="3d6b6-104">**Odpowiednie role:** Administrator rozliczeń | Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="3d6b6-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="3d6b6-105">Pliki uzgodnień można pobrać ze strony Partner Center, aby uzyskać szczegółowy widok elementów wiersza każdej opłaty w cyklu rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="3d6b6-106">Szczegóły elementu wiersza obejmują opłaty za subskrypcje poszczególnych klientów i szczegółowe zdarzenia (takie jak krótkoterminowe dodawanie licencji do subskrypcji).</span><span class="sxs-lookup"><span data-stu-id="3d6b6-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="3d6b6-107">Aby uzyskać informacje na temat odczytywania **faktury,** zobacz [Odczytywanie rachunku.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="3d6b6-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="3d6b6-108">Opis pól pliku uzgodnień</span><span class="sxs-lookup"><span data-stu-id="3d6b6-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="3d6b6-109">Pola pliku uzgodnień w oparciu o licencję</span><span class="sxs-lookup"><span data-stu-id="3d6b6-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="3d6b6-110">Pola pliku uzgodnień w oparciu o użycie</span><span class="sxs-lookup"><span data-stu-id="3d6b6-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="3d6b6-111">Pola pliku uzgodnień dziennego użycia</span><span class="sxs-lookup"><span data-stu-id="3d6b6-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="3d6b6-112">Pola pliku uzgodnień programu CSP zakupu tylko raz</span><span class="sxs-lookup"><span data-stu-id="3d6b6-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="3d6b6-113">Opis typów opłat w plikach uzgodnień</span><span class="sxs-lookup"><span data-stu-id="3d6b6-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="3d6b6-114">Aby poznać typy opłat w plikach uzgodnień (kolumna **ChargeType),** zobacz Typy opłat [za pliki uzgodnień](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="3d6b6-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="3d6b6-115">Rozwiązywanie problemów z formatowaniem</span><span class="sxs-lookup"><span data-stu-id="3d6b6-115">Fix formatting issues</span></span>

<span data-ttu-id="3d6b6-116">Czasami plik uzgodnień może zawierać problemy z formatowaniem.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="3d6b6-117">Na przykład ten problem może wystąpić, jeśli nie są używane lokalne en-US.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="3d6b6-118">Wykonaj następujące kroki, aby rozwiązać wszelkie problemy z formatowaniem w plikach uzgodnień:</span><span class="sxs-lookup"><span data-stu-id="3d6b6-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="3d6b6-119">Otwórz plik uzgodnień (w formacie CSV) w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="3d6b6-120">Wybierz pierwszą kolumnę w pliku.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="3d6b6-121">Otwórz Kreatora **konwertowania tekstu na kolumny.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="3d6b6-122">Na wstążce wybierz pozycję **Dane,** a następnie wybierz pozycję **Tekst na kolumny.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="3d6b6-123">W kreatorze wybierz **typ pliku Rozdzielany.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="3d6b6-124">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="3d6b6-125">W polu **Ograniczniki** wybierz pozycję **Przecinek**.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="3d6b6-126">(Jeśli **karta** jest już zaznaczona, możesz pozostawić tę opcję zaznaczoną). Następnie wybierz pozycję **Dalej.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="3d6b6-127">W polu **Format danych kolumny** wybierz pozycję **Date:MDY**.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="3d6b6-128">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="3d6b6-129">W polu **Format danych kolumny** wybierz pozycję **Tekst** dla wszystkich kolumn ilości.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="3d6b6-130">Następnie wybierz pozycję **Finish** (Zakończ).</span><span class="sxs-lookup"><span data-stu-id="3d6b6-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="3d6b6-131">Programowe pobieranie plików uzgodnień</span><span class="sxs-lookup"><span data-stu-id="3d6b6-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="3d6b6-132">Pliki uzgodnień mogą być bardzo duże i czasami trudno je pobrać.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="3d6b6-133">Aby pobrać pliki uzgodnień programowo, zobacz [Pobieranie elementów wiersza faktury.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="3d6b6-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="3d6b6-134">Jeśli plik przekracza limit wierszy w programie Excel</span><span class="sxs-lookup"><span data-stu-id="3d6b6-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="3d6b6-135">Jeśli możesz pobrać plik uzgodnień, ale nie możesz go otworzyć w programie Microsoft Excel, prawdopodobnie oznacza to, że plik zawiera więcej wierszy niż zezwala program Excel.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="3d6b6-136">W takim przypadku możesz otworzyć plik za pomocą jednej z poniższych procedur.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="3d6b6-137">Otwórz plik rekonescji w Power BI</span><span class="sxs-lookup"><span data-stu-id="3d6b6-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="3d6b6-138">Pobierz plik uzgodnień w zwykły sposób.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="3d6b6-139">Pobierz, zainstaluj i otwórz wystąpienie Power BI.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-139">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="3d6b6-140">Na karcie Power BI **Narzędzia** główne wybierz pozycję **Pobierz dane.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="3d6b6-141">Na liście **wspólnych źródeł danych wybierz** pozycję **Tekst/CSV.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="3d6b6-142">Po wyświetleniu monitu otwórz plik rekonescji.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="3d6b6-143">Otwieranie pliku rekonescji w tabeli przestawnej programu Excel</span><span class="sxs-lookup"><span data-stu-id="3d6b6-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="3d6b6-144">Pobierz plik uzgodnień w zwykły sposób.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="3d6b6-145">Otwórz nowy plik w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="3d6b6-146">Na karcie **Dane** wybierz pozycję **Pobierz dane,** wybierz pozycję **Z pliku**, a następnie wybierz **pozycję Tekst/CSV.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="3d6b6-147">Po wyświetleniu monitu otwórz plik rekonescji.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-147">When prompted, open your recon file.</span></span> <span data-ttu-id="3d6b6-148">Zostaną wyświetlone dane.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-148">Your data will appear.</span></span>
5. <span data-ttu-id="3d6b6-149">Z menu **rozwijanego** Załaduj wybierz pozycję **Załaduj do**, a następnie kliknij **przycisk OK.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-149">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="3d6b6-150">W **oknie dialogowym Import danych** wybierz pozycję **Raport tabeli przestawnej,** aby otworzyć plik.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="3d6b6-151">Wyświetlana kwota ujemna</span><span class="sxs-lookup"><span data-stu-id="3d6b6-151">Negative amount displayed</span></span>

<span data-ttu-id="3d6b6-152">W pliku uzgodnień może zostać wyświetlony ujemny wynik.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="3d6b6-153">Jest to prawdopodobnie spowodowane przez jedną z następujących przyczyn:</span><span class="sxs-lookup"><span data-stu-id="3d6b6-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="3d6b6-154">Niedawno anulowano lub ograniczono liczbę licencji</span><span class="sxs-lookup"><span data-stu-id="3d6b6-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="3d6b6-155">Otrzymano kredyt na umowę licencyjną usługi (SLA) lub na korzystanie z platformy Azure</span><span class="sxs-lookup"><span data-stu-id="3d6b6-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="3d6b6-156">Aby uzyskać więcej informacji na temat tej transakcji, sprawdź jej atrybut typu opłaty w pliku uzgodnienia.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="3d6b6-157">Mapowanie podatków lub podatku VAT</span><span class="sxs-lookup"><span data-stu-id="3d6b6-157">Map taxes or VAT</span></span>

<span data-ttu-id="3d6b6-158">Aby zamapować podatki lub podatek od wartości dodanej (VAT) na fakturę:</span><span class="sxs-lookup"><span data-stu-id="3d6b6-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="3d6b6-159">**Zsuń kolumnę** Tax z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="3d6b6-160">**Zsuń kolumnę TaxAmount** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="3d6b6-161">Elementowanie plików uzgodnień według partnera</span><span class="sxs-lookup"><span data-stu-id="3d6b6-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="3d6b6-162">Partnerzy w modelu **pośrednim mogą** używać tych dodatkowych pól zarówno w plikach uzgodnień opartych na licencjach, jak i opartych na użyciu, aby elementować pliki według odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="3d6b6-163">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="3d6b6-163">MPN ID</span></span> | <span data-ttu-id="3d6b6-164">Opis</span><span class="sxs-lookup"><span data-stu-id="3d6b6-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="3d6b6-165">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="3d6b6-165">MPN ID</span></span> | <span data-ttu-id="3d6b6-166">Identyfikator Microsoft Partner Network (MPN) partnera Dostawca rozwiązań w chmurze (CSP) (bezpośredni lub pośredni).</span><span class="sxs-lookup"><span data-stu-id="3d6b6-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="3d6b6-167">Identyfikator MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="3d6b6-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="3d6b6-168">Identyfikator [MPN odsprzedawcy rekordu dla subskrypcji](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="3d6b6-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="3d6b6-169">To pole odpowiada identyfikatorowi odsprzedawcy wymienionemu dla określonej subskrypcji w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="3d6b6-170">Występuje tylko w plikach uzgodnień dla partnerów w modelu pośrednim.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="3d6b6-171">Identyfikator MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="3d6b6-171">Reseller MPN ID</span></span>

<span data-ttu-id="3d6b6-172">Jeśli partner CSP sprzedał subskrypcję bezpośrednio klientowi, jego identyfikator **MPN** jest dwukrotnie wymieniony jako identyfikator **MPN** i identyfikator **MPN odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="3d6b6-173">Jeśli partner programu CSP ma odsprzedawcę bez identyfikatora **MPN,** ta wartość jest ustawiana na identyfikator **MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="3d6b6-174">Jeśli partner CSP usunie identyfikator **MPN odsprzedawcy,** ta wartość zostanie ustawiona *na -1.*</span><span class="sxs-lookup"><span data-stu-id="3d6b6-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="3d6b6-175">Aby wyświetlić lub zaktualizować identyfikator **MPN odsprzedawcy:**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="3d6b6-176">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="3d6b6-177">W menu Partner Center wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="3d6b6-178">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="3d6b6-179">W menu klienta wybierz pozycję **Subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="3d6b6-180">Wybierz subskrypcję z listy.</span><span class="sxs-lookup"><span data-stu-id="3d6b6-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="3d6b6-181">Wybierz **pozycję aktualizuj,** aby zmienić **odsprzedawcę (identyfikator MPN).**</span><span class="sxs-lookup"><span data-stu-id="3d6b6-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3d6b6-182">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="3d6b6-182">Next steps</span></span>

- [<span data-ttu-id="3d6b6-183">Jak odczytać swój rachunek & pliku rekonescji</span><span class="sxs-lookup"><span data-stu-id="3d6b6-183">How to read your bill & recon file</span></span>](read-your-bill.md) 