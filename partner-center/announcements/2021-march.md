---
title: 2021 komunikatów o marcu
description: 2021. anonsów dla Centrum partnerskiego, w tym nowych możliwości, promocji, ofert, rynków lub zmian istniejących ofert.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 5b8c5f52207a7b9a49d07885a36b61486be45497
ms.sourcegitcommit: 60bbb8f4056120264b769f94431f84d86984c2e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/03/2021
ms.locfileid: "106280874"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="e0081-103">2021 komunikatów o marcu</span><span class="sxs-lookup"><span data-stu-id="e0081-103">March 2021 announcements</span></span>

<span data-ttu-id="e0081-104">Ta strona zawiera anonse dla programu Microsoft Partner Center dla marca 2021.</span><span class="sxs-lookup"><span data-stu-id="e0081-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="e0081-105">Zaktualizowany interfejs API weryfikacji adresu klienta dostawcy usług kryptograficznych jest teraz dostępny do testowania</span><span class="sxs-lookup"><span data-stu-id="e0081-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-106">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-106">Categories</span></span>

- <span data-ttu-id="e0081-107">Data: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="e0081-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="e0081-108">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-109">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-109">Summary</span></span>

<span data-ttu-id="e0081-110">W ramach naszego zobowiązania, aby pomóc partnerom i klientom w realizacji działalności w oparciu o relacje zaufania, będziemy zapraszać partnerów na całym świecie do testowania zmian w interfejsie API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="e0081-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-111">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-111">Impacted audience</span></span>

<span data-ttu-id="e0081-112">Wszyscy dostawcy usług kryptograficznych Direct Bill partner i dostawcy pośrednii, którzy tworzą nowe lub aktualizują szczegóły istniejącego adresu klienta</span><span class="sxs-lookup"><span data-stu-id="e0081-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="e0081-113">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-113">Details</span></span>

<span data-ttu-id="e0081-114">Firma Microsoft uruchamia się na zaufaniu.</span><span class="sxs-lookup"><span data-stu-id="e0081-114">Microsoft runs on trust.</span></span> <span data-ttu-id="e0081-115">Firma Microsoft dokłada starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę przesyłania walidacji adresów klienta w przypadku transakcyjnych subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="e0081-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="e0081-116">Obecnie w dniu 31 marca 2021 wprowadzono zmiany w interfejsie API ValidateAddress, które chcemy zaprosić Cię do przetestowania, przed rozpoczęciem wprowadzania zmian w dniu 2021 czerwca.</span><span class="sxs-lookup"><span data-stu-id="e0081-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="e0081-117">Należy zauważyć, że te zmiany mają wpływ tylko na interfejs API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="e0081-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="e0081-118">Nie ma to żadnego oddziaływania na interfejsy API xmlcustom i UpdateBillingProfile.</span><span class="sxs-lookup"><span data-stu-id="e0081-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="e0081-119">Odpowiedź zwróci jeden z następujących komunikatów o stanie:</span><span class="sxs-lookup"><span data-stu-id="e0081-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="e0081-120">Stan</span><span class="sxs-lookup"><span data-stu-id="e0081-120">Status</span></span> | <span data-ttu-id="e0081-121">Opis</span><span class="sxs-lookup"><span data-stu-id="e0081-121">Description</span></span> | <span data-ttu-id="e0081-122">Liczba zwróconych sugerowanych adresów</span><span class="sxs-lookup"><span data-stu-id="e0081-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="e0081-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="e0081-123">VerifiedShippable</span></span> | <span data-ttu-id="e0081-124">Adres jest zweryfikowany i może być wysyłany do.</span><span class="sxs-lookup"><span data-stu-id="e0081-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="e0081-125">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="e0081-125">Single</span></span> |
| <span data-ttu-id="e0081-126">Sprawdzić</span><span class="sxs-lookup"><span data-stu-id="e0081-126">Verified</span></span> | <span data-ttu-id="e0081-127">Adres został zweryfikowany.</span><span class="sxs-lookup"><span data-stu-id="e0081-127">Address is verified.</span></span> | <span data-ttu-id="e0081-128">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="e0081-128">Single</span></span> |
| <span data-ttu-id="e0081-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="e0081-129">InteractionRequired</span></span> | <span data-ttu-id="e0081-130">Sugerowane adresy zostały znacząco zmienione i wymagane jest potwierdzenie użytkownika.</span><span class="sxs-lookup"><span data-stu-id="e0081-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="e0081-131">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="e0081-131">Single</span></span> |
| <span data-ttu-id="e0081-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="e0081-132">StreetPartial</span></span> | <span data-ttu-id="e0081-133">Dana ulica w adresie jest częściowa i potrzebuje dodatkowych informacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="e0081-134">Wielokrotność — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="e0081-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="e0081-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="e0081-135">PremisesPartial</span></span> | <span data-ttu-id="e0081-136">Dane miejsce (numer budynku, numer zestawu itp.) jest częścią i wymaga więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="e0081-137">Wielokrotność — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="e0081-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="e0081-138">Wiele</span><span class="sxs-lookup"><span data-stu-id="e0081-138">Multiple</span></span> | <span data-ttu-id="e0081-139">Istnieje wiele pól, które są częścią adresu (potencjalnie również w tym StreetPartial i PremisesPartial).</span><span class="sxs-lookup"><span data-stu-id="e0081-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="e0081-140">Wielokrotność — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="e0081-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="e0081-141">Brak</span><span class="sxs-lookup"><span data-stu-id="e0081-141">None</span></span> | <span data-ttu-id="e0081-142">Adres jest nieprawidłowy.</span><span class="sxs-lookup"><span data-stu-id="e0081-142">Address is incorrect.</span></span> | <span data-ttu-id="e0081-143">Brak</span><span class="sxs-lookup"><span data-stu-id="e0081-143">None</span></span> |
| <span data-ttu-id="e0081-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="e0081-144">NotValidated</span></span> | <span data-ttu-id="e0081-145">Nie można wysłać adresu przy użyciu procesu weryfikacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="e0081-146">Brak</span><span class="sxs-lookup"><span data-stu-id="e0081-146">None</span></span> |

<span data-ttu-id="e0081-147">Po przesłaniu adresu do zweryfikowania za pośrednictwem interfejsu API ValidateAddress zostanie zwrócony następujący schemat odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="e0081-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="e0081-148">Zapoznaj się z tą przykładową odpowiedzią.</span><span class="sxs-lookup"><span data-stu-id="e0081-148">Take a look at this sample response.</span></span> <span data-ttu-id="e0081-149">Należy pamiętać, że dla Stanów Zjednoczonych odpowiedź zwróci dodatkowy, czterocyfrowy sufiks dla wiersza kodu pocztowego, jeśli w kodzie pocztowym wprowadzono tylko pięć cyfr.</span><span class="sxs-lookup"><span data-stu-id="e0081-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp
// IAggregatePartner partnerOperations;
// string customerId;
// s{
"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="e0081-150">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-150">Next steps</span></span>

- <span data-ttu-id="e0081-151">Udostępnij swój identyfikator dzierżawy piaskownicy naszym ekspertem (msp), khaki Ali, który ma zostać uwzględniony w teście testowym, aby rozpocząć przygotowywanie do aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="e0081-152">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), zapoznaj się z CPV.</span><span class="sxs-lookup"><span data-stu-id="e0081-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-153">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-153">Questions?</span></span>

<span data-ttu-id="e0081-154">Jeśli masz jakieś pytania lub potrzebujesz pomocy technicznej dotyczącej operacji w firmie Microsoft, skontaktuj się z działem pomocy technicznej Twojej partnera.</span><span class="sxs-lookup"><span data-stu-id="e0081-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="e0081-155">Nowe środowisko centrum administracyjnego programu Exchange (SKK)</span><span class="sxs-lookup"><span data-stu-id="e0081-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-156">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-156">Categories</span></span>

- <span data-ttu-id="e0081-157">Data: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="e0081-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="e0081-158">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-159">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-159">Summary</span></span>

<span data-ttu-id="e0081-160">Od 27 kwietnia 2021, centrum administracyjne programu Exchange (SKK) będzie przetworzyć nowe środowisko, które poprawi codzienne wydajność użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e0081-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-161">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-161">Impacted audience</span></span>

<span data-ttu-id="e0081-162">Administratorzy delegowani uzyskujący dostęp do programu Exchange za poorednictwem Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="e0081-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="e0081-163">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-163">Details</span></span>

<span data-ttu-id="e0081-164">Od 27 kwietnia 2021 partnerzy, którzy przejdą do programu Exchange za pomocą Centrum partnerskiego, zostaną przekierowani do nowego serwera SKK.</span><span class="sxs-lookup"><span data-stu-id="e0081-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="e0081-165">To nowe środowisko jest obecnie dostępne w wersji zapoznawczej, a administratorzy mogą aktywować to środowisko, wybierając przełącznik w prawym górnym rogu w ramach klasycznego elementu SKK.</span><span class="sxs-lookup"><span data-stu-id="e0081-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="e0081-166">Mogą również przechodzić do nowego elementu SKK, wybierając transparent "Wypróbuj teraz", który jest wyświetlany na wszystkich stronach.</span><span class="sxs-lookup"><span data-stu-id="e0081-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="e0081-167">Zalety nowej wartości SKK obejmują:</span><span class="sxs-lookup"><span data-stu-id="e0081-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="e0081-168">Dodano usługi Insights, raporty i mechanizmy alertów dotyczące problemów związanych z przepływem poczty.</span><span class="sxs-lookup"><span data-stu-id="e0081-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="e0081-169">Spersonalizowane pulpity nawigacyjne zwiększające produktywność.</span><span class="sxs-lookup"><span data-stu-id="e0081-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="e0081-170">Aby ułatwić przechodzenie przez nowe środowisko, klipy wideo są dostępne w sekcji **przewodnika & szkoleń** w nowym środowisku narzędzia SKK.</span><span class="sxs-lookup"><span data-stu-id="e0081-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="e0081-171">Dzięki temu można zapoznać się z omówieniem, jak najlepiej korzystać z nowego portalu.</span><span class="sxs-lookup"><span data-stu-id="e0081-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="e0081-172">W przypadku tej zmiany środowisko klasycznego programu SKK nie będzie przestarzałe.</span><span class="sxs-lookup"><span data-stu-id="e0081-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="e0081-173">Przed zaimplementowaniem jakiejkolwiek zmiany otrzymasz odpowiednie powiadomienie.</span><span class="sxs-lookup"><span data-stu-id="e0081-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-174">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-174">Next steps</span></span>

- <span data-ttu-id="e0081-175">Zapoznaj się z [zasobami dotyczącymi tego tematu](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), gdzie można wyświetlić zrzuty ekranu nowego środowiska.</span><span class="sxs-lookup"><span data-stu-id="e0081-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="e0081-176">Udostępnij te informacje właściwym udziałowcom w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="e0081-177">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-177">Questions?</span></span>

<span data-ttu-id="e0081-178">Aby dowiedzieć się więcej na temat tych zmian, należy zapoznać się z odpowiednimi społecznościami Yammer.</span><span class="sxs-lookup"><span data-stu-id="e0081-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="e0081-179">Operacje firmy Microsoft: wprowadzenie do kalendarza uruchamiania produktu</span><span class="sxs-lookup"><span data-stu-id="e0081-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-180">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-180">Categories</span></span>

- <span data-ttu-id="e0081-181">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="e0081-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="e0081-182">Oferty | Nowoczesne miejsce pracy</span><span class="sxs-lookup"><span data-stu-id="e0081-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-183">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-183">Summary</span></span>

<span data-ttu-id="e0081-184">W odpowiedzi na opinie partnerów działania firmy Microsoft będą usprawnić komunikację w przypadku uruchamiania produktu.</span><span class="sxs-lookup"><span data-stu-id="e0081-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-185">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-185">Impacted audience</span></span>

<span data-ttu-id="e0081-186">Partnerzy dostawcy rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="e0081-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="e0081-187">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-187">Details</span></span>

<span data-ttu-id="e0081-188">Firma Microsoft dokłada starań, aby stale ulepszać środowiska partnerskie.</span><span class="sxs-lookup"><span data-stu-id="e0081-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="e0081-189">Mamy opinię od Ciebie, że otrzymasz zbyt wiele komunikacji od firmy Microsoft, w tym zduplikowane powiadomienia dotyczące uruchamiania produktu.</span><span class="sxs-lookup"><span data-stu-id="e0081-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="e0081-190">W odpowiedzi na opinie firma Microsoft usprawnił środowisko gotowości dla uruchamiania produktu dla nowych i istniejących ofert.</span><span class="sxs-lookup"><span data-stu-id="e0081-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="e0081-191">Udostępniamy teraz jeden miesięczny widok uruchamiania produktu publikowany w galerii zasobów gotowości do działania.</span><span class="sxs-lookup"><span data-stu-id="e0081-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="e0081-192">Ten miesięczny [Widok kalendarza produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) spowoduje zamianę pojedynczej komunikacji z uruchamianiem produktu w galerii zasobów gotowości do obsługi operacji oraz w anonsach Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="e0081-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="e0081-193">Możesz również uzyskać dostęp do tego [kalendarza uruchamiania produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) z [kolekcji społeczności](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [widoków kalendarza](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)i [biuletynów CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="e0081-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="e0081-194">Powiadomimy Cię, gdy opublikujemy kalendarz uruchamiania produktu w każdym miesiącu przy użyciu anonsu w galerii zasobów gotowości do działania.</span><span class="sxs-lookup"><span data-stu-id="e0081-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="e0081-195">Nadal można znaleźć informacje dotyczące nowych i istniejących ofert w dziennikach zmian cennika i cennika, a także w blogach dotyczących produktów, przewodnikach licencjonowania i stronach marketingowych produktu.</span><span class="sxs-lookup"><span data-stu-id="e0081-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="e0081-196">Zmiana zostanie zastosowana do uruchomienia dla następujących produktów:</span><span class="sxs-lookup"><span data-stu-id="e0081-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="e0081-197">Lokalne dla systemu Dynamics</span><span class="sxs-lookup"><span data-stu-id="e0081-197">Dynamics on-premises</span></span>
- <span data-ttu-id="e0081-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e0081-198">Microsoft 365</span></span>
- <span data-ttu-id="e0081-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e0081-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="e0081-200">Windows</span><span class="sxs-lookup"><span data-stu-id="e0081-200">Windows</span></span>
- <span data-ttu-id="e0081-201">Serwer</span><span class="sxs-lookup"><span data-stu-id="e0081-201">Server</span></span>  
- <span data-ttu-id="e0081-202">Narzędzia</span><span class="sxs-lookup"><span data-stu-id="e0081-202">Tools</span></span>
- <span data-ttu-id="e0081-203">Zespoły i odpływ</span><span class="sxs-lookup"><span data-stu-id="e0081-203">Teams and Telco</span></span>

<span data-ttu-id="e0081-204">Będziemy dalej wysyłać określone anonse dla uruchamiania produktu, które wymagają szczegółowych informacji o gotowości operacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-205">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-205">Next steps</span></span>

<span data-ttu-id="e0081-206">Zapoznaj się z zasobami dotyczącymi tego tematu i Udostępnij te informacje odpowiednim udziałowcom w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-207">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-207">Questions?</span></span>

<span data-ttu-id="e0081-208">Aby dowiedzieć się więcej na temat tych ofert, należy zapoznać się z odpowiednimi społecznościami Yammer.</span><span class="sxs-lookup"><span data-stu-id="e0081-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="e0081-209">Zmiany wymagań dotyczących dołączania klienta dostawcy usług kryptograficznych</span><span class="sxs-lookup"><span data-stu-id="e0081-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-210">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-210">Categories</span></span>

- <span data-ttu-id="e0081-211">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="e0081-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="e0081-212">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-213">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-213">Summary</span></span>

<span data-ttu-id="e0081-214">W ramach naszych starań, aby pomóc partnerom i klientom w realizacji działalności w oparciu o relacje zaufania, będziemy żądać dodatkowych informacji o klientach, od 25 marca 2021.</span><span class="sxs-lookup"><span data-stu-id="e0081-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-215">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-215">Impacted audience</span></span>

<span data-ttu-id="e0081-216">Dostawcy rozwiązań w chmurze (CSP) — bezpośredni partnerzy rachunku i dostawcy pośrednim, którzy mają nowych lub istniejących klientów w krajach wymienionych w następnej sekcji</span><span class="sxs-lookup"><span data-stu-id="e0081-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="e0081-217">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-217">Details</span></span>

<span data-ttu-id="e0081-218">Firma Microsoft uruchamia się na zaufaniu.</span><span class="sxs-lookup"><span data-stu-id="e0081-218">Microsoft runs on trust.</span></span> <span data-ttu-id="e0081-219">Firma Microsoft dokłada starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji klienta w przypadku transakcyjnych subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="e0081-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="e0081-220">25 marca 2021. wprowadzimy udoskonalenia interfejsu API Centrum partnerskiego i interfejsu użytkownika, które będą miały wpływ na partnerów spełniających następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="e0081-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="e0081-221">Partner ma bezpośrednią relację rozliczeń z firmą Microsoft (co oznacza, że partner to bezpośredni partner Bill lub pośredni dostawca).</span><span class="sxs-lookup"><span data-stu-id="e0081-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="e0081-222">Partner wykonuje działalność z nowymi lub istniejącymi klientami w następujących krajach:</span><span class="sxs-lookup"><span data-stu-id="e0081-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="e0081-223">Tajlandia</span><span class="sxs-lookup"><span data-stu-id="e0081-223">Thailand</span></span>
    - <span data-ttu-id="e0081-224">Wietnam</span><span class="sxs-lookup"><span data-stu-id="e0081-224">Vietnam</span></span>
    - <span data-ttu-id="e0081-225">Turcja</span><span class="sxs-lookup"><span data-stu-id="e0081-225">Turkey</span></span>
    - <span data-ttu-id="e0081-226">Polska</span><span class="sxs-lookup"><span data-stu-id="e0081-226">Poland</span></span>
    - <span data-ttu-id="e0081-227">Republika Południowej Afryki</span><span class="sxs-lookup"><span data-stu-id="e0081-227">South Africa</span></span>
    - <span data-ttu-id="e0081-228">Indie</span><span class="sxs-lookup"><span data-stu-id="e0081-228">India</span></span>
    - <span data-ttu-id="e0081-229">Brazylia</span><span class="sxs-lookup"><span data-stu-id="e0081-229">Brazil</span></span>
    - <span data-ttu-id="e0081-230">Irak</span><span class="sxs-lookup"><span data-stu-id="e0081-230">Iraq</span></span>
    - <span data-ttu-id="e0081-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="e0081-231">Myanmar</span></span>
    - <span data-ttu-id="e0081-232">Sudan Południowy</span><span class="sxs-lookup"><span data-stu-id="e0081-232">South Sudan</span></span>
    - <span data-ttu-id="e0081-233">Arabia Saudyjska</span><span class="sxs-lookup"><span data-stu-id="e0081-233">Saudi Arabia</span></span>
    - <span data-ttu-id="e0081-234">Zjednoczone Emiraty Arabskie</span><span class="sxs-lookup"><span data-stu-id="e0081-234">United Arab Emirates</span></span>
    - <span data-ttu-id="e0081-235">Wenezuela</span><span class="sxs-lookup"><span data-stu-id="e0081-235">Venezuela</span></span>

<span data-ttu-id="e0081-236">Partnerzy, którzy spełniają kryteria, będą musieli przesłać **Identyfikator rejestracji firmy** klienta (znany także jako numer **Inn w organizacji** klienta) i **numer telefonu** , gdy dołączają nowych klientów lub modyfikują istniejące szczegóły klienta.</span><span class="sxs-lookup"><span data-stu-id="e0081-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="e0081-237">Ci partnerzy mogą również wprowadzić opcjonalne **drugie imię** klienta.</span><span class="sxs-lookup"><span data-stu-id="e0081-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="e0081-238">Należy pamiętać, że po dodaniu identyfikatora rejestracji firmy należy użyć identyfikatora podatkowego firmy, a nie identyfikatora osobistego klienta.</span><span class="sxs-lookup"><span data-stu-id="e0081-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="e0081-239">Partnerzy, którzy korzystają z nowych lub istniejących klientów w następujących krajach, zostali już dołączeni do wcześniejszej wersji w listopadzie 2020.</span><span class="sxs-lookup"><span data-stu-id="e0081-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="e0081-240">Armenia</span><span class="sxs-lookup"><span data-stu-id="e0081-240">Armenia</span></span>
- <span data-ttu-id="e0081-241">Azerbejdżan</span><span class="sxs-lookup"><span data-stu-id="e0081-241">Azerbaijan</span></span>
- <span data-ttu-id="e0081-242">Białoruś</span><span class="sxs-lookup"><span data-stu-id="e0081-242">Belarus</span></span>
- <span data-ttu-id="e0081-243">Węgry</span><span class="sxs-lookup"><span data-stu-id="e0081-243">Hungary</span></span>
- <span data-ttu-id="e0081-244">Kazachstan</span><span class="sxs-lookup"><span data-stu-id="e0081-244">Kazakhstan</span></span>
- <span data-ttu-id="e0081-245">Kirgistan</span><span class="sxs-lookup"><span data-stu-id="e0081-245">Kyrgyzstan</span></span>
- <span data-ttu-id="e0081-246">Mołdawia</span><span class="sxs-lookup"><span data-stu-id="e0081-246">Moldova</span></span>
- <span data-ttu-id="e0081-247">Rosja</span><span class="sxs-lookup"><span data-stu-id="e0081-247">Russia</span></span>
- <span data-ttu-id="e0081-248">Tadżykistan</span><span class="sxs-lookup"><span data-stu-id="e0081-248">Tajikistan</span></span>
- <span data-ttu-id="e0081-249">Ukraina</span><span class="sxs-lookup"><span data-stu-id="e0081-249">Ukraine</span></span>
- <span data-ttu-id="e0081-250">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="e0081-250">Uzbekistan</span></span>

<span data-ttu-id="e0081-251">Partnerzy z klientami na całym świecie będą mieli możliwość od 25 marca 2021 do wprowadzenia **identyfikatora rejestracji firmy**, **numeru telefonu** i **nazwy środkowej** klientom jako opcjonalne szczegóły.</span><span class="sxs-lookup"><span data-stu-id="e0081-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-252">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-252">Next steps</span></span>

- <span data-ttu-id="e0081-253">Zapoznaj się z dokumentacją techniczną i często zadawanymi pytaniami w [kolekcji dedykowanych partnerów](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) , aby uzyskać bardziej szczegółowe wskazówki.</span><span class="sxs-lookup"><span data-stu-id="e0081-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="e0081-254">Przygotuj się do uwzględnienia zmian za pomocą interfejsu API Centrum partnerskiego i środowiska użytkownika sieci Web.</span><span class="sxs-lookup"><span data-stu-id="e0081-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="e0081-255">Interfejsy API/zestawy SDK będą dostępne do testowania.</span><span class="sxs-lookup"><span data-stu-id="e0081-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="e0081-256">Pamiętaj o przesłaniu dodatkowych danych podczas dołączania nowych klientów lub modyfikowania istniejących szczegółów klienta.</span><span class="sxs-lookup"><span data-stu-id="e0081-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="e0081-257">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), zapoznaj się z CPV.</span><span class="sxs-lookup"><span data-stu-id="e0081-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-258">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-258">Questions?</span></span>

<span data-ttu-id="e0081-259">Jeśli masz jakieś pytania dotyczące identyfikatora prawnego (nazywanego również INN lub cyny), skontaktuj się z doradcą podatkowym lub lokalnym biurem podatkowym.</span><span class="sxs-lookup"><span data-stu-id="e0081-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="e0081-260">Firma Microsoft nie może zapewnić wskazówek dotyczących podatków.</span><span class="sxs-lookup"><span data-stu-id="e0081-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="e0081-261">Jeśli potrzebujesz pomocy technicznej w zakresie operacji w firmie Microsoft, [Otwórz żądanie obsługi](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="e0081-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="e0081-262">Poprawki wprowadzone do 1 marca, 2021 bezterminowych Cennik oprogramowania</span><span class="sxs-lookup"><span data-stu-id="e0081-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-263">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-263">Categories</span></span>

- <span data-ttu-id="e0081-264">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="e0081-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="e0081-265">Oferty/rynki</span><span class="sxs-lookup"><span data-stu-id="e0081-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-266">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-266">Impacted audience</span></span>

<span data-ttu-id="e0081-267">Dostawcy pośrednich i bezpośrednii partnerzy rozliczają w programie w programie dostawcy rozwiązań w chmurze</span><span class="sxs-lookup"><span data-stu-id="e0081-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="e0081-268">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-268">Details</span></span>

<span data-ttu-id="e0081-269">Cennik w przypadku oprogramowania bezterminowego ogłoszonego 1 marca, na 2021 uwzględnionych rynków, które nie powinny być tam dostępne.</span><span class="sxs-lookup"><span data-stu-id="e0081-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="e0081-270">Lista cenowych oprogramowania bez zmian została zaktualizowana o 17 marca 2021 z poprawkami.</span><span class="sxs-lookup"><span data-stu-id="e0081-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="e0081-271">Te poprawki dotyczyły tylko następujących:</span><span class="sxs-lookup"><span data-stu-id="e0081-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="e0081-272">Identyfikator produktu: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="e0081-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="e0081-273">Nazwa produktu: uaktualnienie systemu Windows 10 do wersji Home do wersji Pro dla Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e0081-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="e0081-274">Usunięte lub nieobsługiwane rynki: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, mld USD, BO, BR, BS, BW, przez, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP. OM, PA, PE, PH, PK, PR, PR, PYTAŃ I ODPOWIEDZI, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, UZ, UA, G, UY,, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="e0081-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="e0081-275">Te zmiany dotyczą tylko powyższego produktu.</span><span class="sxs-lookup"><span data-stu-id="e0081-275">These changes only apply to the above product.</span></span> <span data-ttu-id="e0081-276">Inne produkty nie miały żadnych poprawek.</span><span class="sxs-lookup"><span data-stu-id="e0081-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="e0081-277">Następne kroki i zasoby</span><span class="sxs-lookup"><span data-stu-id="e0081-277">Next steps and resources</span></span>

- <span data-ttu-id="e0081-278">Partnerzy, którzy korzystają z bezterminowego oprogramowania, powinni pobrać najnowszą listę cenową oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="e0081-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="e0081-279">Zapoznaj się z [kodami krajów regionów](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) , aby uzyskać przyjazne mapowanie dwuliterowego skrótu do krajów.</span><span class="sxs-lookup"><span data-stu-id="e0081-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="e0081-280">Wersja zestawu SDK na .NET Standard (v 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="e0081-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-281">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-281">Categories</span></span>

- <span data-ttu-id="e0081-282">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="e0081-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="e0081-283">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="e0081-284">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-284">Impacted audience</span></span>

<span data-ttu-id="e0081-285">Bezpośredni partnerzy rozliczeń i dostawcy pośredniemu uczestniczący w programie CSP, którzy korzystają z zestawu SDK platformy .NET dla usługi Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e0081-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="e0081-286">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-286">Details</span></span>

<span data-ttu-id="e0081-287">Od marca 23 2020 partnerzy mogą rozpocząć pobieranie wersji [MicrosoftPartnerCenter. NETSDK (Galeria NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), wraz z zaktualizowanymi [przykładami](https://github.com/Microsoft/Partner-Center-DotNet-Samples)z zestawu SDK usługi Public Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e0081-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="e0081-288">Ta wersja obejmuje aktualizacje następujących metod:</span><span class="sxs-lookup"><span data-stu-id="e0081-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="e0081-289">Zaktualizowano inspekcję: nowe typy operacji</span><span class="sxs-lookup"><span data-stu-id="e0081-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="e0081-290">Dodano nowe [typy operacji](https://docs.microsoft.com/partner-center/develop/auditing-resources) w celu znajomości sytuacji, w których klient zatwierdził i zakończył DAP.</span><span class="sxs-lookup"><span data-stu-id="e0081-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="e0081-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="e0081-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="e0081-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="e0081-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="e0081-293">Zaktualizowano inspekcję: nowe typy zasobów i operacji</span><span class="sxs-lookup"><span data-stu-id="e0081-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="e0081-294">Dodano nowe [typy zasobów i operacji](https://docs.microsoft.com/partner-center/develop/auditing-resources) na potrzeby obsługi scenariusza roli katalogu klienta.</span><span class="sxs-lookup"><span data-stu-id="e0081-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="e0081-295">Nowy typ zasobu "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="e0081-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="e0081-296">Typy operacji "AddUserMember" i "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="e0081-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="e0081-297">Aktualizacje zestawu SDK dla kont klientów</span><span class="sxs-lookup"><span data-stu-id="e0081-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="e0081-298">Obsługa GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="e0081-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="e0081-299">Pobierz/Customers/{Customer-tenant-ID}/Qualifications</span><span class="sxs-lookup"><span data-stu-id="e0081-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="e0081-300">Ogłoś/Customers/{customer_id}/Qualifications? Code = {validationCode}</span><span class="sxs-lookup"><span data-stu-id="e0081-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="e0081-301">Dodatkowe zmiany</span><span class="sxs-lookup"><span data-stu-id="e0081-301">Additional changes</span></span>

<span data-ttu-id="e0081-302">Następujące zmiany są wprowadzane w ramach nowych rodzajów handlu i są obecnie dostępne tylko dla partnerów, którzy są częścią M365/D365 New Commerce Experience Technical Preview.</span><span class="sxs-lookup"><span data-stu-id="e0081-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="e0081-303">Partnerzy, którzy nie są częścią nowego programu Commerce Technical Preview, nie powinni zauważyć i powinny być zgodni z poprzednimi wersjami.</span><span class="sxs-lookup"><span data-stu-id="e0081-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="e0081-304">Zmiany w katalogu:</span><span class="sxs-lookup"><span data-stu-id="e0081-304">Catalog Changes:</span></span>

  - <span data-ttu-id="e0081-305">Pobierz/Products/{Product-ID}/SKUs/{SKU-ID}</span><span class="sxs-lookup"><span data-stu-id="e0081-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="e0081-306">Kup i Zarządzaj:</span><span class="sxs-lookup"><span data-stu-id="e0081-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="e0081-307">Pobierz/customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="e0081-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="e0081-308">Pobierz/customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="e0081-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="e0081-309">/Customers/{customerId}/subscriptions/{subscriptionId} poprawek</span><span class="sxs-lookup"><span data-stu-id="e0081-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="e0081-310">Pobierz/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="e0081-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="e0081-311">Pobierz/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="e0081-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="e0081-312">Opublikuj/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="e0081-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-313">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-313">Next Steps</span></span>

- <span data-ttu-id="e0081-314">Pobierz najnowszą wersję [MicrosoftPartnerCenter. NETSDK (Galeria NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="e0081-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="e0081-315">Pobierz i przejrzyj przykłady w witrynie [GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="e0081-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="e0081-316">Oferta komercyjnego portalu CSP i zachęty dla FY21 dostawcy CSP dla kwalifikujących się ofert</span><span class="sxs-lookup"><span data-stu-id="e0081-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-317">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-317">Categories</span></span>

- <span data-ttu-id="e0081-318">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="e0081-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="e0081-319">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-320">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-320">Impacted audience</span></span>

<span data-ttu-id="e0081-321">Dostawcy pośrednich i bezpośrednii partnerzy rozliczeń w programie dostawcy rozwiązań w chmurze</span><span class="sxs-lookup"><span data-stu-id="e0081-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="e0081-322">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-322">Details</span></span>

<span data-ttu-id="e0081-323">Dostawcy usług pośrednich i bezpośrednich partnerów rozliczeniowych w programie dostawcy rozwiązań w chmurze mogą sprzedawać oferty innych firm i uzyskać zachętę rabatu dla każdej uprawniającej oferty innej firmy w centrum partnerskim lub w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="e0081-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="e0081-324">Zachęta będzie w formie rabatu dla kwalifikujących się sprzedaży ofert i będzie **dostępna do 30 czerwca 2021**.</span><span class="sxs-lookup"><span data-stu-id="e0081-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="e0081-325">Kontynuuj naukę na temat tego komercyjnej oferty dotyczącej portalu CSP i skontaktuj się z klientami w celu zidentyfikowania odpowiednich ofert, aby umożliwić ich ciągłe sukcesy i transformację cyfrową.</span><span class="sxs-lookup"><span data-stu-id="e0081-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="e0081-326">Firma Microsoft jest partnerem niezależnym dostawcom oprogramowania (ISV) w celu udostępnienia najnowszych rozwiązań IaaS i SaaS na rynku dla klientów korzystających z usługi.</span><span class="sxs-lookup"><span data-stu-id="e0081-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="e0081-327">Wydawcy niezależnego dostawcy oprogramowania mają możliwość włączenia sprzedaży ich ofert za pośrednictwem kanału partnerskiego firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e0081-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="e0081-328">Nasze oferty kwalifikujące się do zachęty dzielą się na dwie kategorie:</span><span class="sxs-lookup"><span data-stu-id="e0081-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="e0081-329">Wybierz pozycję SaaS i IaaS oferty innych firm, korzystając z usługi Azure IP współsprzedawana zachęcani status.</span><span class="sxs-lookup"><span data-stu-id="e0081-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="e0081-330">SaaS aplikacje zintegrowane z zespołami lub co najmniej dwiema Microsoft 365 aplikacjami produkcyjnymi, takimi jak PowerPoint, Word, Excel, Outlook lub SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e0081-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="e0081-331">Następne kroki i zasoby</span><span class="sxs-lookup"><span data-stu-id="e0081-331">Next steps and resources</span></span>

- <span data-ttu-id="e0081-332">Dowiedz się więcej na temat [zachęt partnerskich](https://partner.microsoft.com/membership/partner-incentives) do sprzedaży kwalifikujących się aplikacji z witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e0081-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="e0081-333">Nowe oferty są dodawane co miesiąc.</span><span class="sxs-lookup"><span data-stu-id="e0081-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="e0081-334">Zasoby zachęty dla partnerów rozwiązań w chmurze Direct Bill</span><span class="sxs-lookup"><span data-stu-id="e0081-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="e0081-335">Zasoby zachęty dla dostawcy rozwiązań w chmurze</span><span class="sxs-lookup"><span data-stu-id="e0081-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="e0081-336">Przejrzyj tę [prezentację](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) , aby dowiedzieć się więcej o sprzedawaniu komercyjnych aplikacji Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e0081-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="e0081-337">Zapoznaj się z dodatkowymi zasobami [tutaj](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="e0081-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="e0081-338">Poznaj komercyjny katalog portalu Marketplace w [centrum partnerskim](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) lub [Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="e0081-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="e0081-339">Używanie [interfejsów API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) do integrowania aplikacji z firmową firmą</span><span class="sxs-lookup"><span data-stu-id="e0081-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="e0081-340">Skontaktuj się z firmą ISV, z której interesują Cię interesy</span><span class="sxs-lookup"><span data-stu-id="e0081-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="e0081-341">Dostawcy niezależni muszą zintegrować się za pomocą interfejsów API i odsprzedawcy, w których są sprzedawane aplikacje</span><span class="sxs-lookup"><span data-stu-id="e0081-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-342">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-342">Questions?</span></span>  

<span data-ttu-id="e0081-343">Zapoznaj się z [tym artykułem](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) , aby zapoznać się z omówieniem komercyjnej witryny Marketplace w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="e0081-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="e0081-344">Jeśli potrzebujesz dodatkowej pomocy, możesz utworzyć żądanie pomocy technicznej w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="e0081-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="e0081-345">Dowiedz się więcej o [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="e0081-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="e0081-346">Power BI Premium nazw ofert i aktualizacji wymagań wstępnych</span><span class="sxs-lookup"><span data-stu-id="e0081-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-347">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-347">Categories</span></span>

- <span data-ttu-id="e0081-348">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="e0081-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="e0081-349">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-350">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-350">Summary</span></span>

<span data-ttu-id="e0081-351">Cennik końcowy 1 kwietnia 2021 zostanie zaktualizowany w celu dodania przejrzystości do nazw i/lub informacji o wymaganiach wstępnych dla ofert Power BI Premium na użytkownika.</span><span class="sxs-lookup"><span data-stu-id="e0081-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-352">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-352">Impacted audience</span></span>

<span data-ttu-id="e0081-353">Bezpośredni i pośredni partner dostawcy rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="e0081-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="e0081-354">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-354">Details</span></span>

<span data-ttu-id="e0081-355">Cennik końcowy 1 kwietnia 2021 zostanie zaktualizowany w celu dodania przejrzystości do nazw i/lub informacji o wymaganiach wstępnych dla ofert Power BI Premium na użytkownika.</span><span class="sxs-lookup"><span data-stu-id="e0081-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="e0081-356">Do momentu zaktualizowania cennika końcowego należy skorzystać z informacji w tej sekcji, aby upewnić się, że zamówiony produkt jest uporządkowany.</span><span class="sxs-lookup"><span data-stu-id="e0081-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="e0081-357">Poniższe szczegóły przedstawiają zależną jednostkę SKU i szczegółowe informacje o wymaganiach wstępnych.</span><span class="sxs-lookup"><span data-stu-id="e0081-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="e0081-358">Nazwa wyświetlana oferty na 1 marca — wersja zapoznawcza</span><span class="sxs-lookup"><span data-stu-id="e0081-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="e0081-359">Zaktualizowana nazwa wyświetlana oferty 1 kwietnia, końcowa lista cen</span><span class="sxs-lookup"><span data-stu-id="e0081-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="e0081-360">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="e0081-361">Power BI Premium na Add-On użytkownika (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="e0081-362">Power BI Premium na Add-On użytkownika **(Office)** (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="e0081-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="e0081-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="e0081-364">Aby kupić tę ofertę, klienci muszą dysponować jednym z następujących wymagań wstępnych:</span><span class="sxs-lookup"><span data-stu-id="e0081-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="e0081-365">Nazwa wyświetlana oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-365">Offer display name</span></span> | <span data-ttu-id="e0081-366">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="e0081-367">Microsoft 365 E5 (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="e0081-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="e0081-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="e0081-369">Microsoft 365 E5 bez wideokonferencji audio (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="e0081-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="e0081-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="e0081-371">Office 365 E5 (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="e0081-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="e0081-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="e0081-373">Office 365 E5 (cennik dla pracowników niedochodowych) okres próbny</span><span class="sxs-lookup"><span data-stu-id="e0081-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="e0081-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="e0081-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="e0081-375">Pakiet Office 365 E5 bez konferencji audio (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="e0081-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="e0081-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="e0081-377">Następująca oferta Power BI Premium ma wymaganie wstępne wymagane do zakupu:</span><span class="sxs-lookup"><span data-stu-id="e0081-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="e0081-378">Nazwa wyświetlana oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-378">Offer display name</span></span> | <span data-ttu-id="e0081-379">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="e0081-380">Power BI Premium na Add-On użytkownika (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="e0081-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="e0081-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="e0081-382">Do zakupu tej oferty wymagane są następujące wymagania wstępne:</span><span class="sxs-lookup"><span data-stu-id="e0081-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="e0081-383">Nazwa wyświetlana oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-383">Offer display name</span></span> | <span data-ttu-id="e0081-384">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="e0081-385">Power BI Pro (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="e0081-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="e0081-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="e0081-387">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-387">Next steps</span></span>

<span data-ttu-id="e0081-388">Zapoznaj się z zasobami dotyczącymi tego tematu i Udostępnij te informacje odpowiednim udziałowcom w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="e0081-389">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-389">Questions?</span></span>

<span data-ttu-id="e0081-390">Aby uzyskać odpowiedzi na pytania dotyczące tych ofert, należy zapoznać się z odpowiednimi społecznościami Yammer.</span><span class="sxs-lookup"><span data-stu-id="e0081-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="e0081-391">Aktualizacje cen w marcu dla Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="e0081-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-392">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-392">Categories</span></span>

- <span data-ttu-id="e0081-393">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="e0081-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="e0081-394">Oferty/rynki</span><span class="sxs-lookup"><span data-stu-id="e0081-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-395">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-395">Summary</span></span>

<span data-ttu-id="e0081-396">Skorygowano nieprawidłowe ceny 2021 marca dla Microsoft 365 F3 funta (GBP) i euro (EUR).</span><span class="sxs-lookup"><span data-stu-id="e0081-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-397">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-397">Impacted audience</span></span>

<span data-ttu-id="e0081-398">Partnerzy kupują Microsoft 365 F3 w programie GBP lub euro od 1 marca do 17 marca 2021 za pomocą programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="e0081-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="e0081-399">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-399">Details</span></span>

<span data-ttu-id="e0081-400">Firma Microsoft rozwiązała nieprawidłowe ceny dla Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="e0081-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="e0081-401">Niewłaściwe ceny dotyczyły GBP i EUR, a tylko w przypadku ofert zakupionych od 1 marca do 17 marca 2021.</span><span class="sxs-lookup"><span data-stu-id="e0081-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="e0081-402">Poniżej wymieniono uwzględnione oferty i waluty.</span><span class="sxs-lookup"><span data-stu-id="e0081-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="e0081-403">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-403">Offer name</span></span> | <span data-ttu-id="e0081-404">Waluta</span><span class="sxs-lookup"><span data-stu-id="e0081-404">Currency</span></span> | <span data-ttu-id="e0081-405">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-405">Offer ID</span></span> | <span data-ttu-id="e0081-406">Identyfikator materiału</span><span class="sxs-lookup"><span data-stu-id="e0081-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="e0081-407">Microsoft 365 F3 (Charity)</span><span class="sxs-lookup"><span data-stu-id="e0081-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="e0081-408">GBP</span><span class="sxs-lookup"><span data-stu-id="e0081-408">GBP</span></span> | <span data-ttu-id="e0081-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="e0081-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="e0081-410">AAD — 11626</span><span class="sxs-lookup"><span data-stu-id="e0081-410">AAD-11626</span></span> |
| <span data-ttu-id="e0081-411">Microsoft 365 F3 (komercyjne)</span><span class="sxs-lookup"><span data-stu-id="e0081-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="e0081-412">EUR</span><span class="sxs-lookup"><span data-stu-id="e0081-412">EUR</span></span>| <span data-ttu-id="e0081-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="e0081-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="e0081-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="e0081-414">AAA-89898</span></span> |
 
<span data-ttu-id="e0081-415">Licencja na wersję zapoznawczą marzec i kwiecień — Cennik podstawowy zostały zaktualizowane 16 marca, 17:00 Pacyfik (czas standardowy).</span><span class="sxs-lookup"><span data-stu-id="e0081-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-416">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-416">Next steps</span></span>

- <span data-ttu-id="e0081-417">Partnerzy powinni pobrać na bieżąco bieżące cenniki oparte na licencjach, w marcu i w kwietniu, z uwzględnieniem tych korekt cen.</span><span class="sxs-lookup"><span data-stu-id="e0081-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="e0081-418">Firma Microsoft będzie kontaktować się z partnerami, których to dotyczy, w najbliższych tygodniach za pośrednictwem poczty e-mail, aby poinformować ich o następnych krokach związanych z korygowaniem uwzględnionych transakcji.</span><span class="sxs-lookup"><span data-stu-id="e0081-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-419">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-419">Questions?</span></span>

<span data-ttu-id="e0081-420">Aby uzyskać więcej pytań, Sprawdź odpowiednie społeczności Yammera programu CSP.</span><span class="sxs-lookup"><span data-stu-id="e0081-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="e0081-421">Zaktualizuj nazwę firmy prawnej za pomocą Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="e0081-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-422">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-422">Categories</span></span>

- <span data-ttu-id="e0081-423">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="e0081-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="e0081-424">Skalowanie & wydajności dysku</span><span class="sxs-lookup"><span data-stu-id="e0081-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-425">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-425">Summary</span></span>

<span data-ttu-id="e0081-426">Począwszy od marca 2021, partnerzy Microsoft Partner Network (MPN) i dostawcy rozwiązań w chmurze (CSP) pośrednim Odsprzedawcy mogą zaktualizować swoją nazwę firmy w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="e0081-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-427">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-427">Impacted audience</span></span>

<span data-ttu-id="e0081-428">Partnerzy MPN i pośrednicy odsprzedawca dostawcy CSP (nie dotyczy bezpośrednich partnerów rozliczeniowych CSP)</span><span class="sxs-lookup"><span data-stu-id="e0081-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="e0081-429">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-429">Details</span></span>

<span data-ttu-id="e0081-430">Od marca 2021 partnerzy MPN i dostawcy usług kryptograficznych pośrednich odsprzedawca mogą zaktualizować swoją służbową nazwę firmy za pomocą Centrum partnerskiego w sposób zgodny z własnymi sposobami.</span><span class="sxs-lookup"><span data-stu-id="e0081-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="e0081-431">Dzięki tej nowej funkcji partnerzy nie będą już musieli przesyłać biletu pomocy technicznej Centrum partnerskiego w celu zaktualizowania nazwy firmy.</span><span class="sxs-lookup"><span data-stu-id="e0081-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="e0081-432">Pozwoli to zaoszczędzić znaczną ilość czasu partnerom podczas wykonywania tych działań.</span><span class="sxs-lookup"><span data-stu-id="e0081-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="e0081-433">Aby dowiedzieć się więcej, zobacz temat [Aktualizowanie służbowego profilu biznesowego](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="e0081-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="e0081-434">Upewnij się, że nazwa firmy w profilu biznesowym firmy nie zawiera błędów pisowni i skrótów, i dokładnie pasuje do formalnych firmowych rekordów rejestracyjnych firmy.</span><span class="sxs-lookup"><span data-stu-id="e0081-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="e0081-435">Aby uzyskać więcej informacji na temat aktualizowania profilu organizacji, zapoznaj się z tematem [Weryfikowanie profilu organizacji](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="e0081-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-436">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-436">Next steps</span></span>

<span data-ttu-id="e0081-437">Udostępnij te informacje w organizacji, tak aby odpowiedni zespół mógł przeglądać i aktualizować ich procesy.</span><span class="sxs-lookup"><span data-stu-id="e0081-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-438">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-438">Questions?</span></span>

<span data-ttu-id="e0081-439">Aby uzyskać więcej pytań, Sprawdź odpowiednie społeczności Yammera programu CSP.</span><span class="sxs-lookup"><span data-stu-id="e0081-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="e0081-440">Aktualizuj do ewolucji programu dla dostawcy rozwiązań w chmurze (CSP) i otwarte zmiany programu licencjonowania</span><span class="sxs-lookup"><span data-stu-id="e0081-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-441">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-441">Categories</span></span>

- <span data-ttu-id="e0081-442">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="e0081-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="e0081-443">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-444">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-444">Summary</span></span>

<span data-ttu-id="e0081-445">Nowe komercyjne i publiczne oferty bezterminowego oprogramowania są dostępne w programie Cloud Solution Provider (CSP) wraz ze zmianami w ramach programu licencjonowania Open.</span><span class="sxs-lookup"><span data-stu-id="e0081-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-446">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-446">Impacted audience</span></span>

<span data-ttu-id="e0081-447">Dystrybutorzy handlowi i zarządzani odsprzedawcy kupują w ramach programu licencjonowania Open, a także wszyscy partnerzy CSP w transakcyjnym oprogramowaniu</span><span class="sxs-lookup"><span data-stu-id="e0081-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="e0081-448">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-448">Details</span></span>

<span data-ttu-id="e0081-449">We wrześniu 2020 firma Microsoft [ogłosiła](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) szereg kroków w naszej podróży cyfrowej transformacji, aby zwiększyć szanse sprzedaży dla partnerów w programie CSP, w tym dostępność lokalnego oprogramowania dla partnerów.</span><span class="sxs-lookup"><span data-stu-id="e0081-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="e0081-450">Te zmiany pozwalają partnerom rozwijać swoją firmę i rozszerzać ich zasięg dzięki wykorzystaniu licencji na oprogramowanie w programie CSP, umieszczając je na sukcesie w świecie współczesnym w chmurze.</span><span class="sxs-lookup"><span data-stu-id="e0081-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="e0081-451">Umożliwiają one również przechodzenia klientów do chmury i zapewniają partnerom elastyczność potrzebną w środowiskach chmur hybrydowych klienta.</span><span class="sxs-lookup"><span data-stu-id="e0081-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="e0081-452">W dalszej części tej transformacji cyfrowej ogłaszamy następujące zmiany:</span><span class="sxs-lookup"><span data-stu-id="e0081-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="e0081-453">1 lipca 2021: żadne nowe jednostki SKU, produkty lub promocje nie zostaną dodane do listy cen programu licencjonowania Open.</span><span class="sxs-lookup"><span data-stu-id="e0081-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="e0081-454">7 lipca 2021: dwie oferty komercyjne, uzyskaj oryginalny system Windows i Visual Studio Professional i oferty sektorów publicznych (rządowych, edukacyjnych i niedochodowych — zobacz [anons](./2020-december.md#9)) zostaną dodane do cennika programu CSP.</span><span class="sxs-lookup"><span data-stu-id="e0081-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="e0081-455">Listę cen można znaleźć w sekcji oprogramowanie na stronie [sprzedaj > ceny & oferty](https://partnercenter.microsoft.com/pcv/sales) w centrum partnerskim i będzie ona ponownie publikowana w tym dniu.</span><span class="sxs-lookup"><span data-stu-id="e0081-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="e0081-456">Aby uzyskać szczegółowe informacje dotyczące ewolucji programu przez program CSP i otwartych zmian programu licencjonowania, zobacz **następne kroki** poniżej.</span><span class="sxs-lookup"><span data-stu-id="e0081-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-457">Następne kroki:</span><span class="sxs-lookup"><span data-stu-id="e0081-457">Next Steps:</span></span>

- <span data-ttu-id="e0081-458">Ewolucja programu CSP: Sprawdź bezterminowe oprogramowanie w materiałach gotowości [programu Cloud Solution Provider](https://partner.microsoft.com/resources/collection/software-in-csp#/) .</span><span class="sxs-lookup"><span data-stu-id="e0081-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="e0081-459">Użyj tej [mapy gotowości](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) , aby szybko zlokalizować odpowiednie informacje dla roli.</span><span class="sxs-lookup"><span data-stu-id="e0081-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="e0081-460">Otwarte zmiany programu licencjonowania: Przejrzyj [ewolucję programu CSP i Otwórz program licencjonowania](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) .</span><span class="sxs-lookup"><span data-stu-id="e0081-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="e0081-461">Użyj tej [mapy gotowości](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) , aby szybko zlokalizować odpowiednie informacje dla roli.</span><span class="sxs-lookup"><span data-stu-id="e0081-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-462">Pytania</span><span class="sxs-lookup"><span data-stu-id="e0081-462">Questions</span></span>

<span data-ttu-id="e0081-463">Aby uzyskać więcej pytań, Sprawdź odpowiednie społeczności Yammera programu CSP.</span><span class="sxs-lookup"><span data-stu-id="e0081-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="e0081-464">Aktualizacja do poprzedniego anonsu: oceny w wersji Premium, dodatek do Menedżera zgodności</span><span class="sxs-lookup"><span data-stu-id="e0081-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-465">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-465">Categories</span></span>

- <span data-ttu-id="e0081-466">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="e0081-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="e0081-467">Rozwijanie firmy</span><span class="sxs-lookup"><span data-stu-id="e0081-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-468">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-468">Summary</span></span>

<span data-ttu-id="e0081-469">Oferty wersji próbnej nie powinny znajdować się na liście cen i zostaną usunięte.</span><span class="sxs-lookup"><span data-stu-id="e0081-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-470">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-470">Impacted audience</span></span>

<span data-ttu-id="e0081-471">Partnerzy w transakcyjnym użyciu dostawcy rozwiązań w chmurze</span><span class="sxs-lookup"><span data-stu-id="e0081-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="e0081-472">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-472">Details</span></span>

<span data-ttu-id="e0081-473">Oferty wersji próbnej nie powinny znajdować się na liście cen.</span><span class="sxs-lookup"><span data-stu-id="e0081-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="e0081-474">Zostaną one usunięte z cennika 1 maja 2021.</span><span class="sxs-lookup"><span data-stu-id="e0081-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="e0081-475">Oryginalne ogłoszenie jest [tutaj](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="e0081-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="e0081-476">Dodatkowe zasoby</span><span class="sxs-lookup"><span data-stu-id="e0081-476">Additional resources</span></span>

- [<span data-ttu-id="e0081-477">Microsoft 365 E5 zabezpieczenia i zgodność</span><span class="sxs-lookup"><span data-stu-id="e0081-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="e0081-478">Kompiluj oceny i zarządzaj nimi w programie Microsoft zgodność Manager — zgodność Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e0081-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="e0081-479">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-479">Next steps</span></span>

<span data-ttu-id="e0081-480">Zapoznaj się z zasobami dotyczącymi tego tematu i Udostępnij te informacje odpowiednim udziałowcom w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-481">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-481">Questions?</span></span>

<span data-ttu-id="e0081-482">Pytania dotyczące tych ofert można znaleźć w odpowiednich społecznościach usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="e0081-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="e0081-483">Migrowanie rozwiązań z jednego partnera komercyjnego (OCP) do rynku (GTM) do komercyjnej witryny Microsoft Marketplace</span><span class="sxs-lookup"><span data-stu-id="e0081-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-484">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-484">Categories</span></span>

- <span data-ttu-id="e0081-485">Data: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="e0081-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="e0081-486">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-487">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-487">Summary</span></span>

<span data-ttu-id="e0081-488">Od 29 marca 2021 rozpocznie się korzystanie z ograniczonej liczby możliwości na rynku (GTM).</span><span class="sxs-lookup"><span data-stu-id="e0081-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="e0081-489">Zachęcamy do migrowania rozwiązań do komercyjnej witryny Marketplace w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="e0081-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-490">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-490">Impacted audience</span></span>

<span data-ttu-id="e0081-491">Organizacje współsprzedaży z rozwiązaniami w języku OCP GTM</span><span class="sxs-lookup"><span data-stu-id="e0081-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="e0081-492">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-492">Details</span></span>

<span data-ttu-id="e0081-493">W grudniu 2020 rozpoczęłamy naszą podróż od narzędzia Microsoft OCP GTM do portalu komercyjnego firmy Microsoft w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="e0081-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="e0081-494">To przejście rozszerza możliwości komercyjnej witryny Marketplace, w której można prezentować swoje rozwiązania do milionów klientów, wspólnie wspólnie dzielić się szansami sprzedaży z innymi sprzedawcami firmy Microsoft i partnerów, a jednocześnie sprzedawać innowacyjne rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="e0081-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="e0081-495">Następny punkt kontrolny w przejściu będzie miał miejsce 29 marca 2021.</span><span class="sxs-lookup"><span data-stu-id="e0081-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="e0081-496">Dzieje się tak, gdy rozpocznie się korzystanie z ograniczonych możliwości GTM, gdy niektóre pola stają się tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="e0081-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="e0081-497">Jeśli obecnie sprzedajesz produkty z rozwiązaniami w języku OCP GTM, zachęcamy do migracji rozwiązań do komercyjnej witryny Marketplace, aby korzystać z jej możliwości i uprościć proces publikowania.</span><span class="sxs-lookup"><span data-stu-id="e0081-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="e0081-498">Przejście do komercyjnej witryny Marketplace sprawia, że Centrum partnerskie jest głównym miejscem docelowym w przypadku publikowania współsprzedaży.</span><span class="sxs-lookup"><span data-stu-id="e0081-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="e0081-499">Można w dalszym ciągu rozwijać swoją firmę, łącząc swoje rozwiązania z naszymi udostępnionymi klientami za pomocą tych samych kanałów i środowisk produkcyjnych używanych przez nas dla produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e0081-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="e0081-500">[Dowiedz się więcej o komercyjnym rynku](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="e0081-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-501">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-501">Next steps</span></span>

- <span data-ttu-id="e0081-502">Jeśli nie przeniesiono jeszcze rozwiązań, postępuj zgodnie z instrukcjami szczegółowymi w [przewodniku](/azure/marketplace/co-sell-solution-migration) dotyczącym przejścia lub zapoznaj się z [samouczkiem wideo krok po kroku](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) , aby ukończyć wszystkie działania migracji i rozpocząć publikowanie rozwiązań w komercyjnej witrynie Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e0081-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="e0081-503">W przypadku pytań dotyczących ograniczonej funkcjonalności w OCP GTM zapoznaj się z [wymaganiami dotyczącymi współsprzedaży w celu opublikowania często zadawanych pytań dotyczących komercyjnego portalu Microsoft Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="e0081-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="e0081-504">(Zobacz sekcję "OCP GTM Limited Capabilities od 29 marca 2021.")</span><span class="sxs-lookup"><span data-stu-id="e0081-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-505">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-505">Questions?</span></span>

<span data-ttu-id="e0081-506">Skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/support/?stage=1) , jeśli masz jakieś pytania lub potrzebujesz dodatkowych informacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="e0081-507">Rozszerzanie nowego środowiska handlowego w programie Cloud Solution Provider (CSP) dla platformy Azure do Rosji</span><span class="sxs-lookup"><span data-stu-id="e0081-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-508">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-508">Categories</span></span>

- <span data-ttu-id="e0081-509">Data: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="e0081-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="e0081-510">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-511">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-511">Impacted audience</span></span>

<span data-ttu-id="e0081-512">Wszyscy partnerzy w Rosji transakcyjnej za pomocą programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="e0081-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="e0081-513">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-513">Details</span></span>

<span data-ttu-id="e0081-514">Od marca 10 2021 przyjemnością ogłaszamy dostępność **nowego środowiska handlowego w programie CSP dla platformy Azure w Rosji**.</span><span class="sxs-lookup"><span data-stu-id="e0081-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="e0081-515">To środowisko usprawnia i ulepsza sposób kupowania i korzystania z usług platformy Azure przez klientów.</span><span class="sxs-lookup"><span data-stu-id="e0081-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="e0081-516">Zapewni to również partnerom programu CSP spójny widok cen platformy Azure w ramach ruchu sprzedaży, cenniki USD dla globalnej spójności, wyrównania dat rozliczeń i dostęp do Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="e0081-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-517">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-517">Next steps</span></span>

<span data-ttu-id="e0081-518">Dostępnych jest kilka zasobów wprowadzających nowe środowisko Azure Commerce i dostarczających dodatkowe informacje.</span><span class="sxs-lookup"><span data-stu-id="e0081-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="e0081-519">Znajdź najnowsze często zadawane pytania, talie, wideo i nie tylko w [galerii zasobów aktualizacji programu CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="e0081-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="e0081-520">Klucz licencji oprogramowania Centrum partnerskiego i realizacja pobrania</span><span class="sxs-lookup"><span data-stu-id="e0081-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-521">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-521">Categories</span></span>

- <span data-ttu-id="e0081-522">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="e0081-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="e0081-523">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-524">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-524">Summary</span></span>

<span data-ttu-id="e0081-525">Funkcja pobierania oprogramowania Centrum partnerskiego i możliwość realizacji klucza licencji zostały przywrócone.</span><span class="sxs-lookup"><span data-stu-id="e0081-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-526">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-526">Impacted audience</span></span>

<span data-ttu-id="e0081-527">Wszyscy partnerzy dostawcy rozwiązań w chmurze (CSP) transakcji bezterminowych i subskrypcji serwera za poorednictwem Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="e0081-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="e0081-528">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-528">Details</span></span>

<span data-ttu-id="e0081-529">W odpowiedzi na opinie partnerów firma Microsoft przywraca funkcję realizacji Centrum partnerskiego, aby uzyskać klucze oprogramowania i licencji na potrzeby zamówień bezterminowych i subskrypcyjnych na serwerze.</span><span class="sxs-lookup"><span data-stu-id="e0081-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="e0081-530">Przed usunięciem z 19 stycznia 2021, zostanie przywrócony do poprzedniego stanu.</span><span class="sxs-lookup"><span data-stu-id="e0081-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="e0081-531">(Zobacz [ogłoszenie](2020-september.md#17)).</span><span class="sxs-lookup"><span data-stu-id="e0081-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="e0081-532">Należy pamiętać, że klucze licencji oprogramowania i linki do pobrania są cennymi i wysoce poszukiwane — po zasobach własności intelektualnej.</span><span class="sxs-lookup"><span data-stu-id="e0081-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="e0081-533">W przypadku przecieków można szybko przekroczyć limity aktywacji i spowodować negatywne środowisko klienta i partnera.</span><span class="sxs-lookup"><span data-stu-id="e0081-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-534">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-534">Next steps</span></span>

<span data-ttu-id="e0081-535">Zapoznaj się z poniższymi zasobami, aby uzyskać instrukcje dotyczące użycia i ważne wskazówki dotyczące dystrybucji kluczy oprogramowania:</span><span class="sxs-lookup"><span data-stu-id="e0081-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="e0081-536">Sprzedawanie oprogramowania lokalnego za pomocą programu CSP</span><span class="sxs-lookup"><span data-stu-id="e0081-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="e0081-537">[Centrum partnerskie — nowy Przewodnik operacji handlowych](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (zobacz **wskazówki dotyczące dystrybucji kluczy oprogramowania** ).</span><span class="sxs-lookup"><span data-stu-id="e0081-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-538">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-538">Questions?</span></span>

<span data-ttu-id="e0081-539">Jeśli masz jakieś pytania dotyczące tego powiadomienia, zapoznaj się z odpowiednimi społecznościami usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="e0081-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="e0081-540">Migrowanie Twoich transakcji z programu Partner Sales Connect (PSC) do Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="e0081-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-541">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-541">Categories</span></span>

- <span data-ttu-id="e0081-542">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="e0081-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="e0081-543">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-544">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-544">Summary</span></span>

<span data-ttu-id="e0081-545">Program Partner Sales Connect (PSC) zostanie przesunięty w dostęp tylko do odczytu od 31 marca 2021, więc zachęcamy do rozpoczęcia migracji Twoich transakcji z kontrolera PSC do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="e0081-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-546">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-546">Impacted audience</span></span>

<span data-ttu-id="e0081-547">Partnerzy z ofertami w systemie PSC</span><span class="sxs-lookup"><span data-stu-id="e0081-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="e0081-548">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-548">Details</span></span>

<span data-ttu-id="e0081-549">W ramach naszego wspólnego zobowiązania do wzrostu, **współsprzedaży z firmą Microsoft** jest ścieżką, która ma **zostać odnaleziona, dostarczasz wiedzę i rozszerzasz swój** wpływ na klientów w przypadku pozytywnych wyników klienta.</span><span class="sxs-lookup"><span data-stu-id="e0081-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="e0081-550">Dzięki średniej transakcji, która jest **3,5 razy szybsze** niż normalne, zarządzanie obsługą współsprzedaży w centrum partnerskim pozwala sprzedawać klientów, partnerów i kanałów sprzedającego firmy Microsoft oraz zarządzać całym potoku odwołań w jednej lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="e0081-551">**Kontroler PSC** przejdzie do **dostępu tylko do odczytu** od **31 marca 2021**, dlatego zachęcamy do rozpoczęcia przejścia do Centrum partnerskiego i uzyskania dostępu do tych ulepszeń funkcji:</span><span class="sxs-lookup"><span data-stu-id="e0081-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="e0081-552">Dokładniejsze **kierowanie tras** w przypadku współdzielenia się z firmą Microsoft z odpowiednim sprzedawcą na podstawie typu potrzebnej pomocy.</span><span class="sxs-lookup"><span data-stu-id="e0081-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="e0081-553">**Poprzednia transakcja sprawdza poprawność** dla rozwiązań kwalifikujących się do zachęty i spełnia kryteria programu niezależnych dostawców oprogramowania, upraszczając proces zatwierdzania i ostateczne potwierdzenie wykonania (PoE).</span><span class="sxs-lookup"><span data-stu-id="e0081-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="e0081-554">**Bezproblemowe środowisko użytkownika** umożliwiające zarządzanie wszystkimi szansami sprzedaży i potencjalnymi klientami w jednym miejscu.</span><span class="sxs-lookup"><span data-stu-id="e0081-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="e0081-555">Niedawno dodano również nowe funkcje w centrum partnerskim, które ułatwiają przechodzenie:</span><span class="sxs-lookup"><span data-stu-id="e0081-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="e0081-556">Operacje zbiorcze dla możliwości wspólnej sprzedaży</span><span class="sxs-lookup"><span data-stu-id="e0081-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="e0081-557">[Funkcja migracji transakcji](../psc-to-pc.md) (zobacz sekcję **migracja transakcji PSC** ).</span><span class="sxs-lookup"><span data-stu-id="e0081-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="e0081-558">Korzystając z funkcji współsprzedaży w centrum partnerskim, zespoły sprzedaży będą miały więcej czasu skupić się na Nurturing potencjalnych klientów i szansach sprzedaży, zamknięciu transakcji oraz tworzeniu trwałych relacji z klientami.</span><span class="sxs-lookup"><span data-stu-id="e0081-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="e0081-559">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-559">Next steps</span></span>

<span data-ttu-id="e0081-560">Skorzystaj z [przewodnika przejścia](../psc-to-pc.md) Centrum partnerskiego, aby przeprowadzić Cię przez procedurę migrowania Twoich transakcji z kontrolera PSC do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="e0081-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-561">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-561">Questions?</span></span>

<span data-ttu-id="e0081-562">Aby uzyskać więcej pytań, skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="e0081-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="e0081-563">Nowe produkty i oferty systemu Microsoft Dynamics 365 dostępne 1 kwietnia 2021</span><span class="sxs-lookup"><span data-stu-id="e0081-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-564">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-564">Categories</span></span>

- <span data-ttu-id="e0081-565">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="e0081-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="e0081-566">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-567">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-567">Summary</span></span>

<span data-ttu-id="e0081-568">1 kwietnia 2021 firma Microsoft będzie otrzymywać kilka nowych produktów i ofert dla programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="e0081-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-569">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-569">Impacted audience</span></span>

<span data-ttu-id="e0081-570">Wszyscy partnerzy przeprowadzają Operacje transakcyjne przez program Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="e0081-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="e0081-571">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-571">Details</span></span>

<span data-ttu-id="e0081-572">1 kwietnia 2021 firma Microsoft będzie otrzymywać następujące nowe produkty i oferty:</span><span class="sxs-lookup"><span data-stu-id="e0081-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="e0081-573">Power BI Premium na użytkownika</span><span class="sxs-lookup"><span data-stu-id="e0081-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="e0081-574">Obsługa głosu i marketingu NALICZENIA z klientami oraz rozszerzanie segmentów</span><span class="sxs-lookup"><span data-stu-id="e0081-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="e0081-575">**Power BI Premium na użytkownika**</span><span class="sxs-lookup"><span data-stu-id="e0081-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="e0081-576">Firma Microsoft wprowadzi pierwsze oferty Power BI Premium dla poszczególnych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e0081-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="e0081-577">Power BI Premium jest obecnie sprzedawany tylko w konstrukcji pojemności.</span><span class="sxs-lookup"><span data-stu-id="e0081-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="e0081-578">Power BI Premium na użytkownika zapewnia dostęp do funkcji analizy biznesowej (BI) przedsiębiorstwa i analizy.</span><span class="sxs-lookup"><span data-stu-id="e0081-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="e0081-579">Elastyczna Licencjonowanie indywidualnych miejsc jest przeznaczony dla małych i średnich firm.</span><span class="sxs-lookup"><span data-stu-id="e0081-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="e0081-580">Przejrzyj [szczegóły wydania Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) , aby dowiedzieć się więcej o tej ofercie.</span><span class="sxs-lookup"><span data-stu-id="e0081-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="e0081-581">**Szczegóły oferty**</span><span class="sxs-lookup"><span data-stu-id="e0081-581">**Offer details**</span></span>

<span data-ttu-id="e0081-582">Należy pamiętać, że nazwa oferty różni się nieco od wersji zapoznawczej cennika.</span><span class="sxs-lookup"><span data-stu-id="e0081-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="e0081-583">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-583">Offer name</span></span> | <span data-ttu-id="e0081-584">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="e0081-585">Power BI Premium na użytkownika</span><span class="sxs-lookup"><span data-stu-id="e0081-585">Power BI Premium Per User</span></span> | <span data-ttu-id="e0081-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="e0081-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="e0081-587">Power BI Premium na użytkownika w przypadku wykładowców</span><span class="sxs-lookup"><span data-stu-id="e0081-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="e0081-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="e0081-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="e0081-589">Power BI Premium na użytkownika dla studentów</span><span class="sxs-lookup"><span data-stu-id="e0081-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="e0081-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="e0081-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="e0081-591">Power BI Premium na użytkownika (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="e0081-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="e0081-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="e0081-593">Power BI Premium na użytkownika Add-On</span><span class="sxs-lookup"><span data-stu-id="e0081-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="e0081-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="e0081-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="e0081-595">Power BI Premium na Add-On użytkownika dla wykładowców</span><span class="sxs-lookup"><span data-stu-id="e0081-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="e0081-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="e0081-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="e0081-597">Power BI Premium na Add-On użytkownika dla studentów</span><span class="sxs-lookup"><span data-stu-id="e0081-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="e0081-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="e0081-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="e0081-599">Power BI Premium na Add-On użytkownika (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="e0081-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="e0081-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="e0081-601">**Obsługa głosu i marketingu NALICZENIA z klientami oraz rozszerzanie segmentów**</span><span class="sxs-lookup"><span data-stu-id="e0081-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="e0081-602">W ramach monitu o wprowadzenie do 2020 grudnia, oferta klienta Dynamics 365 i Marketing NALICZENIA zostały zmienione w celu dodania nowych krajów i większej liczby jednostek SKU i edukacyjnych.</span><span class="sxs-lookup"><span data-stu-id="e0081-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="e0081-603">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-603">Offer name</span></span> | <span data-ttu-id="e0081-604">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="e0081-605">Dynamics 365 Customer Voice NALICZENIA (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="e0081-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="e0081-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="e0081-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="e0081-607">Dynamics 365 Customer Voice NALICZENIA for wykładowcy</span><span class="sxs-lookup"><span data-stu-id="e0081-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="e0081-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="e0081-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="e0081-609">Odwiedź następujące strony, aby dowiedzieć się więcej na temat tych ofert:</span><span class="sxs-lookup"><span data-stu-id="e0081-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="e0081-610">Strona główna głosu usługi klienta Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e0081-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="e0081-611">Strona główna marketingowa Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e0081-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="e0081-612">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-612">Next steps</span></span>

<span data-ttu-id="e0081-613">Zapoznaj się z zasobami w tym temacie i Udostępnij te informacje odpowiednim udziałowcom w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="e0081-614">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-614">Questions?</span></span>

<span data-ttu-id="e0081-615">Aby uzyskać odpowiedzi na pytania dotyczące tych ofert, należy zapoznać się z odpowiednimi społecznościami Yammer.</span><span class="sxs-lookup"><span data-stu-id="e0081-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="e0081-616">Program Microsoft Universal Print jest teraz dostępny w niektórych pakietach</span><span class="sxs-lookup"><span data-stu-id="e0081-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="e0081-617">Kategorie</span><span class="sxs-lookup"><span data-stu-id="e0081-617">Categories</span></span>

- <span data-ttu-id="e0081-618">Data: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="e0081-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="e0081-619">Możliwości</span><span class="sxs-lookup"><span data-stu-id="e0081-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="e0081-620">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="e0081-620">Summary</span></span>

<span data-ttu-id="e0081-621">Program Microsoft Universal Print będzie dostępny w ramach usługi Transact in SELECT Microsoft 365 Suite i jako samodzielny dodatek od 1 marca 2021.</span><span class="sxs-lookup"><span data-stu-id="e0081-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="e0081-622">Odbiorcy, których dotyczy problem</span><span class="sxs-lookup"><span data-stu-id="e0081-622">Impacted audience</span></span>

<span data-ttu-id="e0081-623">Wszyscy partnerzy przeprowadzają Operacje transakcyjne przez program Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="e0081-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="e0081-624">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="e0081-624">Details</span></span>

<span data-ttu-id="e0081-625">[Drukowanie uniwersalne](https://aka.ms/universalprint) to usługa drukowania Microsoft 365, która eliminuje potrzebę stosowania lokalnych serwerów wydruku i umożliwia urządzeniom z systemem Windows drukowanie na drukarkach zarejestrowanych na platformie Azure.</span><span class="sxs-lookup"><span data-stu-id="e0081-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="e0081-626">Będzie on dostępny dla języka Transact od 1 marca 2021.</span><span class="sxs-lookup"><span data-stu-id="e0081-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="e0081-627">Pracownicy mogą korzystać z funkcji drukowania bez sterowników, usprawnionego odnajdowania drukarek opartych na lokalizacji oraz intuicyjnego środowiska drukowania, które nie ma krzywej szkoleniowej.</span><span class="sxs-lookup"><span data-stu-id="e0081-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="e0081-628">Urządzenia, które są przyłączone do Azure Active Directory (Azure AD), używają istniejących poświadczeń usługi Azure AD do bezpiecznego drukowania.</span><span class="sxs-lookup"><span data-stu-id="e0081-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="e0081-629">Administratorzy zarządzają drukowaniem przy użyciu Azure Portal i mogą łatwo łączyć się z drukarkami z natywną obsługą drukowania uniwersalnego.</span><span class="sxs-lookup"><span data-stu-id="e0081-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="e0081-630">Można wdrożyć uniwersalne drukowanie z niezgodnymi drukarkami przy użyciu oprogramowania uniwersalnego łącznika wydruku.</span><span class="sxs-lookup"><span data-stu-id="e0081-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="e0081-631">Drukowanie uniwersalne zostanie uzupełnione na początku do systemu Windows E3, A3, E5 i A5 oraz Microsoft 365 BP, F3, E3, A3, E5 i A5.</span><span class="sxs-lookup"><span data-stu-id="e0081-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="e0081-632">**Szczegóły oferty**</span><span class="sxs-lookup"><span data-stu-id="e0081-632">**Offer details**</span></span>

<span data-ttu-id="e0081-633">Należy pamiętać, że nazwa oferty różni się nieco od wersji zapoznawczej cennika.</span><span class="sxs-lookup"><span data-stu-id="e0081-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="e0081-634">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-634">Offer name</span></span> | <span data-ttu-id="e0081-635">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="e0081-635">Offer ID</span></span> | <span data-ttu-id="e0081-636">Identyfikator materiału</span><span class="sxs-lookup"><span data-stu-id="e0081-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="e0081-637">Dodatek dla woluminu uniwersalnego drukowania (500 zadań) — Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e0081-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="e0081-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="e0081-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="e0081-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="e0081-639">9BI-00004</span></span>   |
| <span data-ttu-id="e0081-640">Dodatek uniwersalnego drukowania woluminów (500 zadań) dla wykładowców — Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e0081-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="e0081-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="e0081-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="e0081-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="e0081-642">9BK-00004</span></span>   |
| <span data-ttu-id="e0081-643">Dodatek dla woluminu uniwersalnego drukowania (500 zadań) — Windows</span><span class="sxs-lookup"><span data-stu-id="e0081-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="e0081-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="e0081-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="e0081-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="e0081-645">9BI-00002</span></span>   |
| <span data-ttu-id="e0081-646">Dodatek do zbiorczej drukowania zbiorczego (500 zadań) dla wykładowców — Windows</span><span class="sxs-lookup"><span data-stu-id="e0081-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="e0081-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="e0081-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="e0081-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="e0081-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="e0081-649">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e0081-649">Next steps</span></span>

<span data-ttu-id="e0081-650">Zapoznaj się z cennikiem i [uniwersalnym omówieniem drukowania](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="e0081-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="e0081-651">Udostępnij te informacje wszystkim odpowiednim kontaktom w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e0081-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="e0081-652">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="e0081-652">Questions?</span></span>

<span data-ttu-id="e0081-653">Aby uzyskać odpowiedzi na pytania dotyczące tych ofert, należy zapoznać się z odpowiednimi społecznościami Yammer.</span><span class="sxs-lookup"><span data-stu-id="e0081-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
