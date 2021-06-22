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
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431575"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="8ef5b-103">Dowiedz się, jak odczytywać elementy wiersza w plikach Partner Center uzgodnień</span><span class="sxs-lookup"><span data-stu-id="8ef5b-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="8ef5b-104">**Odpowiednie role:** Administrator rozliczeń | Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="8ef5b-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="8ef5b-105">Pliki uzgodnień można pobrać ze strony Partner Center, aby uzyskać szczegółowy widok elementów wiersza każdej opłaty w cyklu rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="8ef5b-106">Szczegóły elementu wiersza obejmują opłaty za subskrypcje poszczególnych klientów i szczegółowe zdarzenia (takie jak krótkoterminowe dodawanie licencji do subskrypcji).</span><span class="sxs-lookup"><span data-stu-id="8ef5b-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="8ef5b-107">Aby uzyskać informacje na temat odczytywania **faktury,** zobacz [Odczytywanie rachunku.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="8ef5b-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="8ef5b-108">Opis pól pliku uzgodnień</span><span class="sxs-lookup"><span data-stu-id="8ef5b-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="8ef5b-109">Pola pliku uzgodnień w oparciu o licencję</span><span class="sxs-lookup"><span data-stu-id="8ef5b-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="8ef5b-110">Pola pliku uzgodnień w oparciu o użycie</span><span class="sxs-lookup"><span data-stu-id="8ef5b-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="8ef5b-111">Pola pliku uzgodnień dziennego użycia</span><span class="sxs-lookup"><span data-stu-id="8ef5b-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="8ef5b-112">Pola pliku uzgodnień programu CSP zakupu tylko raz</span><span class="sxs-lookup"><span data-stu-id="8ef5b-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="8ef5b-113">Opis typów opłat w plikach uzgodnień</span><span class="sxs-lookup"><span data-stu-id="8ef5b-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="8ef5b-114">Aby poznać typy opłat w plikach uzgodnień (kolumna **ChargeType),** zobacz Typy opłat [za pliki uzgodnień](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5b-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="8ef5b-115">Rozwiązywanie problemów z formatowaniem</span><span class="sxs-lookup"><span data-stu-id="8ef5b-115">Fix formatting issues</span></span>

<span data-ttu-id="8ef5b-116">Czasami plik uzgodnień może zawierać problemy z formatowaniem.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="8ef5b-117">Na przykład ten problem może wystąpić, jeśli nie są używane lokalne en-US.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="8ef5b-118">Wykonaj następujące kroki, aby rozwiązać wszelkie problemy z formatowaniem w plikach uzgodnień:</span><span class="sxs-lookup"><span data-stu-id="8ef5b-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="8ef5b-119">Otwórz plik uzgodnień (w formacie .csv) w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="8ef5b-120">Wybierz pierwszą kolumnę w pliku.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="8ef5b-121">Otwórz Kreatora **konwertowania tekstu na kolumny.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="8ef5b-122">Na wstążce wybierz pozycję **Dane,** a następnie wybierz pozycję **Tekst na kolumny.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="8ef5b-123">W kreatorze wybierz **typ pliku Rozdzielany.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="8ef5b-124">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="8ef5b-125">W polu **Ograniczniki** wybierz pozycję **Przecinek**.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="8ef5b-126">(Jeśli **karta** jest już zaznaczona, możesz pozostawić tę opcję zaznaczoną). Następnie wybierz pozycję **Dalej.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="8ef5b-127">W polu **Format danych kolumny** wybierz pozycję **Date:MDY.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="8ef5b-128">Następnie wybierz pozycję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="8ef5b-129">W polu **Format danych kolumny** wybierz pozycję **Tekst** dla wszystkich kolumn ilości.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="8ef5b-130">Następnie wybierz pozycję **Finish** (Zakończ).</span><span class="sxs-lookup"><span data-stu-id="8ef5b-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="8ef5b-131">Programowe pobieranie plików uzgodnień</span><span class="sxs-lookup"><span data-stu-id="8ef5b-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="8ef5b-132">Pliki uzgodnień mogą być bardzo duże i czasami trudno je pobrać.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="8ef5b-133">Aby pobrać pliki uzgodnień programowo, zobacz [Pobieranie elementów wiersza faktury.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="8ef5b-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="8ef5b-134">Jeśli plik przekracza limit wierszy w programie Excel</span><span class="sxs-lookup"><span data-stu-id="8ef5b-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="8ef5b-135">Jeśli możesz pobrać plik uzgodnień, ale nie możesz go otworzyć w programie Microsoft Excel, prawdopodobnie oznacza to, że plik zawiera więcej wierszy niż zezwala program Excel.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="8ef5b-136">W takim przypadku możesz otworzyć plik za pomocą jednej z poniższych procedur.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="8ef5b-137">Otwórz plik rekonescji w Power BI</span><span class="sxs-lookup"><span data-stu-id="8ef5b-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="8ef5b-138">Pobierz plik uzgodnień w zwykły sposób.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="8ef5b-139">Pobierz, zainstaluj i otwórz wystąpienie usługi Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="8ef5b-140">Na karcie Power BI **Narzędzia** główne wybierz pozycję **Pobierz dane.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="8ef5b-141">Na liście **wspólnych źródeł danych** wybierz pozycję **Tekst/CSV.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="8ef5b-142">Po wyświetleniu monitu otwórz plik rekonescji.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="8ef5b-143">Otwieranie pliku ponownego w tabeli przestawnej programu Excel</span><span class="sxs-lookup"><span data-stu-id="8ef5b-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="8ef5b-144">Pobierz plik uzgodnień w zwykły sposób.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="8ef5b-145">Otwórz nowy plik w programie Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="8ef5b-146">Na karcie **Dane** wybierz pozycję **Pobierz dane,** wybierz pozycję **Z pliku**, a następnie wybierz **pozycję Tekst/CSV.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="8ef5b-147">Po wyświetleniu monitu otwórz plik rekonescji.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-147">When prompted, open your recon file.</span></span> <span data-ttu-id="8ef5b-148">Zostaną wyświetlone dane.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-148">Your data will appear.</span></span>
5. <span data-ttu-id="8ef5b-149">Z menu **rozwijanego** Ładowanie wybierz pozycję **Załaduj do**, a następnie wybierz przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="8ef5b-150">W **oknie dialogowym Import danych** wybierz pozycję **Raport tabeli przestawnej,** aby otworzyć plik.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="8ef5b-151">Wyświetlana kwota ujemna</span><span class="sxs-lookup"><span data-stu-id="8ef5b-151">Negative amount displayed</span></span>

<span data-ttu-id="8ef5b-152">W pliku uzgodnień może zostać wyświetlony ujemny wynik.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="8ef5b-153">Jest to prawdopodobnie spowodowane przez jedną z następujących przyczyn:</span><span class="sxs-lookup"><span data-stu-id="8ef5b-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="8ef5b-154">Niedawno anulowano lub ograniczono liczbę licencji</span><span class="sxs-lookup"><span data-stu-id="8ef5b-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="8ef5b-155">Otrzymano kredyt na umowę licencyjną usługi (SLA) lub na korzystanie z platformy Azure</span><span class="sxs-lookup"><span data-stu-id="8ef5b-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="8ef5b-156">Aby uzyskać więcej informacji na temat tej transakcji, sprawdź jej atrybut typu opłaty w pliku uzgodnienia.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="8ef5b-157">Mapowanie podatków lub podatku VAT</span><span class="sxs-lookup"><span data-stu-id="8ef5b-157">Map taxes or VAT</span></span>

<span data-ttu-id="8ef5b-158">Aby zamapować podatki lub podatek od wartości dodanej (VAT) na fakturę:</span><span class="sxs-lookup"><span data-stu-id="8ef5b-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="8ef5b-159">**Zsuń kolumnę** Tax z pliku opartego na licencjach.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="8ef5b-160">**Zsuń kolumnę TaxAmount** z pliku opartego na użyciu.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="8ef5b-161">Elementowanie plików uzgodnień według partnera</span><span class="sxs-lookup"><span data-stu-id="8ef5b-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="8ef5b-162">Partnerzy w modelu **pośrednim mogą** używać tych dodatkowych pól zarówno w plikach uzgodnień opartych na licencjach, jak i opartych na użyciu, aby elementować pliki według odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="8ef5b-163">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="8ef5b-163">MPN ID</span></span> | <span data-ttu-id="8ef5b-164">Opis</span><span class="sxs-lookup"><span data-stu-id="8ef5b-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="8ef5b-165">Identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="8ef5b-165">MPN ID</span></span> | <span data-ttu-id="8ef5b-166">Identyfikator Microsoft Partner Network (MPN) partnera Dostawca rozwiązań w chmurze (CSP) (bezpośredni lub pośredni).</span><span class="sxs-lookup"><span data-stu-id="8ef5b-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="8ef5b-167">Identyfikator MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="8ef5b-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="8ef5b-168">Identyfikator [MPN odsprzedawcy rekordu dla subskrypcji](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="8ef5b-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="8ef5b-169">To pole odpowiada identyfikatorowi odsprzedawcy wymienionemu dla określonej subskrypcji w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="8ef5b-170">Występuje tylko w plikach uzgodnień dla partnerów w modelu pośrednim.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="8ef5b-171">Identyfikator MPN odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="8ef5b-171">Reseller MPN ID</span></span>

<span data-ttu-id="8ef5b-172">Jeśli partner CSP sprzedał subskrypcję bezpośrednio klientowi, jego identyfikator **MPN** jest dwukrotnie wymieniony jako zarówno identyfikator **MPN,** jak i identyfikator **MPN odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="8ef5b-173">Jeśli partner CSP ma odsprzedawcę bez identyfikatora **MPN,** ta wartość jest ustawiana na identyfikator **MPN** partnera.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="8ef5b-174">Jeśli partner CSP usunie identyfikator **MPN odsprzedawcy,** ta wartość zostanie ustawiona *na -1.*</span><span class="sxs-lookup"><span data-stu-id="8ef5b-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="8ef5b-175">Aby wyświetlić lub zaktualizować identyfikator **MPN odsprzedawcy:**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="8ef5b-176">Zaloguj się do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="8ef5b-177">W menu Partner Center wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="8ef5b-178">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="8ef5b-179">W menu klienta wybierz pozycję **Subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="8ef5b-180">Wybierz subskrypcję z listy.</span><span class="sxs-lookup"><span data-stu-id="8ef5b-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="8ef5b-181">Wybierz **pozycję aktualizuj,** aby zmienić **odsprzedawcę (identyfikator MPN).**</span><span class="sxs-lookup"><span data-stu-id="8ef5b-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8ef5b-182">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="8ef5b-182">Next steps</span></span>

- [<span data-ttu-id="8ef5b-183">Jak odczytać swój rachunek & pliku rekonescji</span><span class="sxs-lookup"><span data-stu-id="8ef5b-183">How to read your bill & recon file</span></span>](read-your-bill.md) 