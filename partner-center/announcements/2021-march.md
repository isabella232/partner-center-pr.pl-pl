---
title: Ogłoszenia z marca 2021 r.
description: Ogłoszenia dotyczące platformy Microsoft Partner Center z marca 2021 r., w tym nowe możliwości, promocje, oferty, rynki lub zmiany istniejących ofert.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328070"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="6bd05-103">Ogłoszenia z marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-103">March 2021 announcements</span></span>

<span data-ttu-id="6bd05-104">Ta strona zawiera ogłoszenia dotyczące platformy Microsoft Partner Center na marzec 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a><span data-ttu-id="6bd05-105">Gotowość: zmiany interfejsu API weryfikacji adresu Dostawca rozwiązań w chmurze (CSP) zostaną wprowadzone w czerwcu; Funkcja testowania jest teraz dostępna</span><span class="sxs-lookup"><span data-stu-id="6bd05-105">Readiness: Changes to the Cloud Solution Provider (CSP) customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-106">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-106">Categories</span></span>

- <span data-ttu-id="6bd05-107">Data: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="6bd05-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="6bd05-108">Gotowość</span><span class="sxs-lookup"><span data-stu-id="6bd05-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-109">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-109">Summary</span></span>

<span data-ttu-id="6bd05-110">Aby pomóc partnerom i klientom w prowadzenia działalności w oparciu o zaufanie, będziemy zapraszać partnerów do testowania zmian w interfejsie API weryfikowania adresów dla wszystkich krajów na całym świecie.</span><span class="sxs-lookup"><span data-stu-id="6bd05-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-111">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-111">Impacted audience</span></span>

<span data-ttu-id="6bd05-112">Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy tworzą nowych lub aktualizują istniejących klientów, rozsyłają szczegółowe informacje.</span><span class="sxs-lookup"><span data-stu-id="6bd05-112">CSP direct bill partners and indirect providers who create new or update existing customers address details.</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-113">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-113">Details</span></span>

<span data-ttu-id="6bd05-114">Firma Microsoft działa w oparciu o zaufanie.</span><span class="sxs-lookup"><span data-stu-id="6bd05-114">Microsoft runs on trust.</span></span> <span data-ttu-id="6bd05-115">Dokładamy starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji adresu klienta na potrzeby transakcji subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="6bd05-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="6bd05-116">Od 31 marca 2021 r. wprowadziliśmy zmiany w interfejsie API weryfikowania adresu, które zaprosiliśmy partnerów do testowania przed wprowadzeniem zmian w czerwcu 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-116">As of March 31, 2021, we’ve introduced changes to the Validate Address API that we invited partners to test, prior to going live with the changes in June 2021.</span></span>

<span data-ttu-id="6bd05-117">Zmiany mają wpływ tylko na interfejs API weryfikacji adresu.</span><span class="sxs-lookup"><span data-stu-id="6bd05-117">Changes affect the Validate Address API only.</span></span> <span data-ttu-id="6bd05-118">Nie ma to wpływu na interfejsy API tworzenia klienta i aktualizowania profilu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="6bd05-118">Create Customer and Update Billing Profile APIs aren’t impacted.</span></span>

<span data-ttu-id="6bd05-119">Odpowiedź zwróci jeden z następujących komunikatów o stanie:</span><span class="sxs-lookup"><span data-stu-id="6bd05-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="6bd05-120">Stan</span><span class="sxs-lookup"><span data-stu-id="6bd05-120">Status</span></span>     | <span data-ttu-id="6bd05-121">Opis</span><span class="sxs-lookup"><span data-stu-id="6bd05-121">Description</span></span> |    <span data-ttu-id="6bd05-122">Liczba zwróconych sugerowanych adresów</span><span class="sxs-lookup"><span data-stu-id="6bd05-122">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="6bd05-123">Zweryfikowana wysyłka</span><span class="sxs-lookup"><span data-stu-id="6bd05-123">Verified shippable</span></span> | <span data-ttu-id="6bd05-124">Adres jest weryfikowany i można go wysłać.</span><span class="sxs-lookup"><span data-stu-id="6bd05-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="6bd05-125">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="6bd05-125">Single</span></span> |
|<span data-ttu-id="6bd05-126">Sprawdzonych</span><span class="sxs-lookup"><span data-stu-id="6bd05-126">Verified</span></span> | <span data-ttu-id="6bd05-127">Adres jest weryfikowany.</span><span class="sxs-lookup"><span data-stu-id="6bd05-127">Address is verified.</span></span> | <span data-ttu-id="6bd05-128">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="6bd05-128">Single</span></span> |
|<span data-ttu-id="6bd05-129">Wymagana interakcja</span><span class="sxs-lookup"><span data-stu-id="6bd05-129">Interaction required</span></span> | <span data-ttu-id="6bd05-130">Sugerowany adres został znacząco zmieniony i wymaga potwierdzenia przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6bd05-130">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="6bd05-131">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="6bd05-131">Single</span></span> |
|<span data-ttu-id="6bd05-132">Część częściowa ulicy</span><span class="sxs-lookup"><span data-stu-id="6bd05-132">Street partial</span></span> | <span data-ttu-id="6bd05-133">Podana ulica w adresie jest częściowa i wymaga więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="6bd05-134">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="6bd05-134">Multiple—maximum of three</span></span> |
|<span data-ttu-id="6bd05-135">Część lokalna</span><span class="sxs-lookup"><span data-stu-id="6bd05-135">Premises partial</span></span> | <span data-ttu-id="6bd05-136">Dane lokalne (numer budynku, numer pakietu i inne) są częściowe i wymagają więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-136">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="6bd05-137">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="6bd05-137">Multiple—maximum of three</span></span> |
|<span data-ttu-id="6bd05-138">Wiele</span><span class="sxs-lookup"><span data-stu-id="6bd05-138">Multiple</span></span> | <span data-ttu-id="6bd05-139">Istnieje wiele pól, które są częściowo w adresie (potencjalnie również częściowe ulice i część lokalna).</span><span class="sxs-lookup"><span data-stu-id="6bd05-139">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="6bd05-140">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="6bd05-140">Multiple—maximum of three</span></span> |
|<span data-ttu-id="6bd05-141">Brak</span><span class="sxs-lookup"><span data-stu-id="6bd05-141">None</span></span> | <span data-ttu-id="6bd05-142">Adres jest niepoprawny.</span><span class="sxs-lookup"><span data-stu-id="6bd05-142">Address is incorrect.</span></span> | <span data-ttu-id="6bd05-143">Brak</span><span class="sxs-lookup"><span data-stu-id="6bd05-143">None</span></span> |
|<span data-ttu-id="6bd05-144">Nie sprawdzono</span><span class="sxs-lookup"><span data-stu-id="6bd05-144">Not validated</span></span> | <span data-ttu-id="6bd05-145">Nie można wysłać adresu w procesie walidacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-145">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="6bd05-146">Brak</span><span class="sxs-lookup"><span data-stu-id="6bd05-146">None</span></span> |

<span data-ttu-id="6bd05-147">Kody pocztowe w USA zwracają dodatkowe 4 cyfry i łącznik — na przykład 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="6bd05-147">US post codes will return an additional 4 digits + hyphen - for example, 12345-6789.</span></span>

<span data-ttu-id="6bd05-148">Po przesłaniu adresu do weryfikacji za pośrednictwem interfejsu API weryfikacji adresu zostanie zwrócony następujący schemat odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="6bd05-148">Once an address is submitted for validation via the Validate Address API, the following response schema will be returned:</span></span>

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

<span data-ttu-id="6bd05-149">Przyjrzyj się tej przykładowej odpowiedzi.</span><span class="sxs-lookup"><span data-stu-id="6bd05-149">Take a look at this sample response.</span></span> <span data-ttu-id="6bd05-150">Pamiętaj, że w przypadku Stanów Zjednoczonych odpowiedź zwróci dodatkowy czterocyfrowy sufiks dla wiersza kodu pocztowego, jeśli wprowadzasz tylko pięć cyfr dla kodu pocztowego.</span><span class="sxs-lookup"><span data-stu-id="6bd05-150">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

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

### <a name="next-steps"></a><span data-ttu-id="6bd05-151">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-151">Next steps</span></span>

- <span data-ttu-id="6bd05-152">Udostępnij swój identyfikator dzierżawy piaskownicy ekspertowi w tej dziedzinie (Ali Ichki), który zostanie uwzględniony w teście testowym, aby rozpocząć przygotowywanie do aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-152">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="6bd05-153">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.</span><span class="sxs-lookup"><span data-stu-id="6bd05-153">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-154">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-154">Questions?</span></span>

<span data-ttu-id="6bd05-155">Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych przez firmę Microsoft, swiązyj się z grupą usługi Yammer pomocy technicznej partnera.</span><span class="sxs-lookup"><span data-stu-id="6bd05-155">If you need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

### <a name="change-log"></a><span data-ttu-id="6bd05-156">Dziennik zmian:</span><span class="sxs-lookup"><span data-stu-id="6bd05-156">Change log:</span></span>

- <span data-ttu-id="6bd05-157">31 marca 2020 r.: oryginalna publikacja</span><span class="sxs-lookup"><span data-stu-id="6bd05-157">March 31, 2020: Original publication</span></span>

- <span data-ttu-id="6bd05-158">30 kwietnia 2021 r.: aktualizacje przykładowej odpowiedzi i szczegółów kodu pocztowego</span><span class="sxs-lookup"><span data-stu-id="6bd05-158">April 30, 2021: Updates for sample response and Zip code details</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="6bd05-159">Nowe środowisko centrum administracyjnego programu Exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="6bd05-159">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-160">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-160">Categories</span></span>

- <span data-ttu-id="6bd05-161">Data: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="6bd05-161">Date: 2021-03-29</span></span>
- <span data-ttu-id="6bd05-162">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-162">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-163">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-163">Summary</span></span>

<span data-ttu-id="6bd05-164">Od 27 kwietnia 2021 r. w centrum administracyjnym programu Exchange (EAC) zostanie wdane nowe środowisko, które poprawi wydajność pracy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6bd05-164">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-165">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-165">Impacted audience</span></span>

<span data-ttu-id="6bd05-166">Administratorzy delegowani uzyskiwania dostępu do programu Exchange za pośrednictwem Partner Center</span><span class="sxs-lookup"><span data-stu-id="6bd05-166">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-167">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-167">Details</span></span>

<span data-ttu-id="6bd05-168">Od 27 kwietnia 2021 r. partnerzy, którzy przejdą do programu Exchange za pośrednictwem programu Partner Center, zostaną przekierowani do nowego konta EAC.</span><span class="sxs-lookup"><span data-stu-id="6bd05-168">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="6bd05-169">To nowe środowisko jest obecnie dostępne w wersji zapoznawczej, a administratorzy mogą aktywować to środowisko, wybierając przełącznik w prawym górnym rogu klasycznej funkcji EAC.</span><span class="sxs-lookup"><span data-stu-id="6bd05-169">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="6bd05-170">Mogą również przejść do nowej EAC, wybierając baner "Wypróbuj teraz", który jest wyświetlany na wszystkich stronach.</span><span class="sxs-lookup"><span data-stu-id="6bd05-170">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="6bd05-171">Nowe funkcje EAC mają następujące zalety:</span><span class="sxs-lookup"><span data-stu-id="6bd05-171">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="6bd05-172">Dodano szczegółowe informacje, raporty i mechanizmy alertów dotyczące problemów związanych z przepływem poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="6bd05-172">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="6bd05-173">Spersonalizowane pulpity nawigacyjne zwiększające produktywność.</span><span class="sxs-lookup"><span data-stu-id="6bd05-173">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="6bd05-174">Aby ułatwić nawigowanie po nowym środowisko, filmy wideo są dostępne w sekcji **Training & Guide** (Przewodnik szkoleniowy) dotyczącej nowego doświadczenia EAC.</span><span class="sxs-lookup"><span data-stu-id="6bd05-174">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="6bd05-175">Te informacje zapewniają przegląd sposobu najlepszego korzystania z nowego portalu.</span><span class="sxs-lookup"><span data-stu-id="6bd05-175">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="6bd05-176">Dzięki tej zmianie klasyczne środowisko funkcji EAC nie będzie przestarzałe.</span><span class="sxs-lookup"><span data-stu-id="6bd05-176">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="6bd05-177">Przed zaimplementowaniem każdej zmiany użytkownik zostanie o tym powiadomiony z dużym wyprzedzeniem.</span><span class="sxs-lookup"><span data-stu-id="6bd05-177">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-178">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-178">Next steps</span></span>

- <span data-ttu-id="6bd05-179">Zapoznaj się z [zasobami na ten temat,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)gdzie możesz wyświetlać zrzuty ekranu nowego doświadczenia.</span><span class="sxs-lookup"><span data-stu-id="6bd05-179">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="6bd05-180">Udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-180">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="6bd05-181">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-181">Questions?</span></span>

<span data-ttu-id="6bd05-182">Jeśli masz pytania dotyczące tych zmian, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-182">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="6bd05-183">Microsoft Operations: Introducing the product launch calendar (Operacje firmy Microsoft: wprowadzenie do kalendarza uruchamiania produktu)</span><span class="sxs-lookup"><span data-stu-id="6bd05-183">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-184">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-184">Categories</span></span>

- <span data-ttu-id="6bd05-185">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="6bd05-185">Date: 2021-03-25</span></span>
- <span data-ttu-id="6bd05-186">Oferty | Nowoczesne miejsce pracy</span><span class="sxs-lookup"><span data-stu-id="6bd05-186">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-187">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-187">Summary</span></span>

<span data-ttu-id="6bd05-188">W odpowiedzi na opinie partnerów operacje firmy Microsoft usprawniają komunikację podczas uruchamiania produktów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-188">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-189">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-189">Impacted audience</span></span>

<span data-ttu-id="6bd05-190">Dostawca rozwiązań w chmurze partnerów (CSP)</span><span class="sxs-lookup"><span data-stu-id="6bd05-190">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-191">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-191">Details</span></span>

<span data-ttu-id="6bd05-192">Firma Microsoft dokłada starań, aby stale ulepszać środowisko partnerów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-192">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="6bd05-193">Otrzymaliśmy opinię, że otrzymujesz zbyt wiele komunikatów od firmy Microsoft, w tym zduplikowane ogłoszenia dotyczące startów produktów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-193">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="6bd05-194">W odpowiedzi na Twoją opinię firma Microsoft usprawniła środowisko gotowości do wprowadzenia nowych i istniejących ofert produktów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-194">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="6bd05-195">Teraz zapewniamy pojedynczy miesięczny widok uruchomień produktów opublikowany w galerii zasobów gotowości operacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-195">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="6bd05-196">Ten [comiesięczny widok](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) kalendarza uruchamiania produktu zastąpi komunikację o uruchomieniu poszczególnych produktów w galerii zasobów Gotowości na operacje i w Partner Center o ogłoszeniach.</span><span class="sxs-lookup"><span data-stu-id="6bd05-196">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="6bd05-197">Możesz również uzyskać dostęp do kalendarza [uruchamiania tego produktu z](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) kolekcji [społeczności,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)widoków [kalendarza](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)i [biuletynów CSP.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)</span><span class="sxs-lookup"><span data-stu-id="6bd05-197">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="6bd05-198">Powiadomimy Cię, gdy opublikujemy kalendarz uruchamiania produktów z każdego miesiąca z ogłoszeniem w galerii zasobów Gotowości na operacje.</span><span class="sxs-lookup"><span data-stu-id="6bd05-198">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="6bd05-199">Informacje dotyczące nowych i istniejących ofert można nadal znaleźć w dziennikach podglądu cennika i zmian cennika, a także w blogach dotyczących produktów, przewodnikach licencjonowania i stronach marketingowych produktów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-199">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="6bd05-200">Zmiana będzie dotyczyć startów następujących produktów:</span><span class="sxs-lookup"><span data-stu-id="6bd05-200">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="6bd05-201">Lokalna usługa Dynamics</span><span class="sxs-lookup"><span data-stu-id="6bd05-201">Dynamics on-premises</span></span>
- <span data-ttu-id="6bd05-202">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6bd05-202">Microsoft 365</span></span>
- <span data-ttu-id="6bd05-203">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="6bd05-203">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="6bd05-204">Windows</span><span class="sxs-lookup"><span data-stu-id="6bd05-204">Windows</span></span>
- <span data-ttu-id="6bd05-205">Serwer</span><span class="sxs-lookup"><span data-stu-id="6bd05-205">Server</span></span>  
- <span data-ttu-id="6bd05-206">Narzędzia</span><span class="sxs-lookup"><span data-stu-id="6bd05-206">Tools</span></span>
- <span data-ttu-id="6bd05-207">Teams i Telco</span><span class="sxs-lookup"><span data-stu-id="6bd05-207">Teams and Telco</span></span>

<span data-ttu-id="6bd05-208">Będziemy nadal wysyłać konkretne ogłoszenia dotyczące startów produktów, które wymagają szczegółów gotowości operacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-208">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-209">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-209">Next steps</span></span>

<span data-ttu-id="6bd05-210">Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-210">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-211">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-211">Questions?</span></span>

<span data-ttu-id="6bd05-212">Jeśli masz dodatkowe pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-212">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="6bd05-213">Zmiany wymagań dotyczących dołączania klientów do CSP</span><span class="sxs-lookup"><span data-stu-id="6bd05-213">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-214">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-214">Categories</span></span>

- <span data-ttu-id="6bd05-215">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="6bd05-215">Date: 2021-03-25</span></span>
- <span data-ttu-id="6bd05-216">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-216">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-217">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-217">Summary</span></span>

<span data-ttu-id="6bd05-218">W ramach naszego zobowiązania do pomocy partnerom i klientom w zakresie prowadzenia działalności w oparciu o zaufanie poprosimy o dodatkowe informacje o klientach od 25 marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-218">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-219">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-219">Impacted audience</span></span>

<span data-ttu-id="6bd05-220">Dostawca rozwiązań w chmurze (CSP) i dostawcy pośredni, którzy mają nowych lub istniejących klientów w krajach wymienionych w następnej sekcji</span><span class="sxs-lookup"><span data-stu-id="6bd05-220">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-221">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-221">Details</span></span>

<span data-ttu-id="6bd05-222">Firma Microsoft działa w oparciu o zaufanie.</span><span class="sxs-lookup"><span data-stu-id="6bd05-222">Microsoft runs on trust.</span></span> <span data-ttu-id="6bd05-223">Dokładamy starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji klientów na potrzeby transakcji subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="6bd05-223">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="6bd05-224">25 marca 2021 r. wprowadzimy ulepszenia interfejsu API i interfejsu użytkownika usługi Partner Center, które będą mieć wpływ na partnerów spełniających oba następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="6bd05-224">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="6bd05-225">Partner ma bezpośrednią relację rozliczeń z firmą Microsoft (co oznacza, że partner jest partnerem z rozliczaniem bezpośrednim lub dostawcą pośrednim).</span><span class="sxs-lookup"><span data-stu-id="6bd05-225">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="6bd05-226">Partner współpracuje z nowymi lub istniejącymi klientami w następujących krajach:</span><span class="sxs-lookup"><span data-stu-id="6bd05-226">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="6bd05-227">Tajlandia</span><span class="sxs-lookup"><span data-stu-id="6bd05-227">Thailand</span></span>
    - <span data-ttu-id="6bd05-228">Wietnam</span><span class="sxs-lookup"><span data-stu-id="6bd05-228">Vietnam</span></span>
    - <span data-ttu-id="6bd05-229">Turcja</span><span class="sxs-lookup"><span data-stu-id="6bd05-229">Turkey</span></span>
    - <span data-ttu-id="6bd05-230">Polska</span><span class="sxs-lookup"><span data-stu-id="6bd05-230">Poland</span></span>
    - <span data-ttu-id="6bd05-231">Republika Południowej Afryki</span><span class="sxs-lookup"><span data-stu-id="6bd05-231">South Africa</span></span>
    - <span data-ttu-id="6bd05-232">Indie</span><span class="sxs-lookup"><span data-stu-id="6bd05-232">India</span></span>
    - <span data-ttu-id="6bd05-233">Brazylia</span><span class="sxs-lookup"><span data-stu-id="6bd05-233">Brazil</span></span>
    - <span data-ttu-id="6bd05-234">Irak</span><span class="sxs-lookup"><span data-stu-id="6bd05-234">Iraq</span></span>
    - <span data-ttu-id="6bd05-235">Myanmar</span><span class="sxs-lookup"><span data-stu-id="6bd05-235">Myanmar</span></span>
    - <span data-ttu-id="6bd05-236">Sudan Południowy</span><span class="sxs-lookup"><span data-stu-id="6bd05-236">South Sudan</span></span>
    - <span data-ttu-id="6bd05-237">Arabia Saudyjska</span><span class="sxs-lookup"><span data-stu-id="6bd05-237">Saudi Arabia</span></span>
    - <span data-ttu-id="6bd05-238">Zjednoczone Emiraty Arabskie</span><span class="sxs-lookup"><span data-stu-id="6bd05-238">United Arab Emirates</span></span>
    - <span data-ttu-id="6bd05-239">Wenezuela</span><span class="sxs-lookup"><span data-stu-id="6bd05-239">Venezuela</span></span>

<span data-ttu-id="6bd05-240">Partnerzy spełniający kryteria będą mieli możliwość przesyłania identyfikatora rejestracji firmy **klienta** (znanego także  jako organizacja klienta **), oraz** numeru telefonu podczas dołączania nowych klientów lub modyfikowania istniejących danych klienta.</span><span class="sxs-lookup"><span data-stu-id="6bd05-240">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="6bd05-241">Ci partnerzy mogą również wprowadzić opcjonalne **drugie imię** klienta.</span><span class="sxs-lookup"><span data-stu-id="6bd05-241">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="6bd05-242">Pamiętaj, że podczas dodawania identyfikatora rejestracji firmy należy użyć identyfikatora podatku od działalności biznesowej, a nie identyfikatora osobistego klienta.</span><span class="sxs-lookup"><span data-stu-id="6bd05-242">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="6bd05-243">Partnerzy, którzy firma współpracuje z nowymi lub istniejącymi klientami w następujących krajach, są już do dołączani w poprzedniej wersji w listopadzie 2020 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-243">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="6bd05-244">Armenia</span><span class="sxs-lookup"><span data-stu-id="6bd05-244">Armenia</span></span>
- <span data-ttu-id="6bd05-245">Azerbejdżan</span><span class="sxs-lookup"><span data-stu-id="6bd05-245">Azerbaijan</span></span>
- <span data-ttu-id="6bd05-246">Białoruś</span><span class="sxs-lookup"><span data-stu-id="6bd05-246">Belarus</span></span>
- <span data-ttu-id="6bd05-247">Węgry</span><span class="sxs-lookup"><span data-stu-id="6bd05-247">Hungary</span></span>
- <span data-ttu-id="6bd05-248">Kazachstan</span><span class="sxs-lookup"><span data-stu-id="6bd05-248">Kazakhstan</span></span>
- <span data-ttu-id="6bd05-249">Kirgistan</span><span class="sxs-lookup"><span data-stu-id="6bd05-249">Kyrgyzstan</span></span>
- <span data-ttu-id="6bd05-250">Mołdawia</span><span class="sxs-lookup"><span data-stu-id="6bd05-250">Moldova</span></span>
- <span data-ttu-id="6bd05-251">Rosja</span><span class="sxs-lookup"><span data-stu-id="6bd05-251">Russia</span></span>
- <span data-ttu-id="6bd05-252">Tadżykistan</span><span class="sxs-lookup"><span data-stu-id="6bd05-252">Tajikistan</span></span>
- <span data-ttu-id="6bd05-253">Ukraina</span><span class="sxs-lookup"><span data-stu-id="6bd05-253">Ukraine</span></span>
- <span data-ttu-id="6bd05-254">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="6bd05-254">Uzbekistan</span></span>

<span data-ttu-id="6bd05-255">Partnerzy z klientami na całym świecie będą mieć możliwość wprowadzania identyfikatora rejestracji **firmy,** numeru telefonu i środkowego  imienia i nazwiska klientów w dniu 25 marca 2021 r. jako opcjonalnych szczegółów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-255">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-256">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-256">Next steps</span></span>

- <span data-ttu-id="6bd05-257">Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.</span><span class="sxs-lookup"><span data-stu-id="6bd05-257">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="6bd05-258">Przygotuj się do uwzględnienia zmian przy użyciu Partner Center API i internetowego interfejsu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6bd05-258">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="6bd05-259">Zestawy API/zestawy SDK będą dostępne do testowania.</span><span class="sxs-lookup"><span data-stu-id="6bd05-259">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="6bd05-260">Pamiętaj, aby przesłać dodatkowe dane podczas dołączania nowych klientów lub modyfikowania istniejących danych klienta.</span><span class="sxs-lookup"><span data-stu-id="6bd05-260">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="6bd05-261">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.</span><span class="sxs-lookup"><span data-stu-id="6bd05-261">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-262">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-262">Questions?</span></span>

<span data-ttu-id="6bd05-263">Skontaktuj się z doradcą podatkowym lub lokalnym urzędem podatkowym, jeśli masz pytania związane z identyfikatorem prawna (nazywanym również URZĘDEM podatkowym lub NIP).</span><span class="sxs-lookup"><span data-stu-id="6bd05-263">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="6bd05-264">Firma Microsoft nie może zapewnić wskazówek dotyczących kwestii podatkowych.</span><span class="sxs-lookup"><span data-stu-id="6bd05-264">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="6bd05-265">Jeśli potrzebujesz pomocy technicznej w operacjach wykonywanych w firmie Microsoft, [otwórz żądanie obsługi](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="6bd05-265">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="6bd05-266">Korekty wprowadzone do 1 marca 2021 r. bezterminowy cennik oprogramowania</span><span class="sxs-lookup"><span data-stu-id="6bd05-266">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-267">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-267">Categories</span></span>

- <span data-ttu-id="6bd05-268">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="6bd05-268">Date: 2021-03-23</span></span>
- <span data-ttu-id="6bd05-269">Oferty/rynki</span><span class="sxs-lookup"><span data-stu-id="6bd05-269">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-270">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-270">Impacted audience</span></span>

<span data-ttu-id="6bd05-271">Dostawcy pośredni i bezpośredni partnerzy rozliczający się bezterminowo w ramach programu Dostawca rozwiązań w chmurze oprogramowania</span><span class="sxs-lookup"><span data-stu-id="6bd05-271">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="6bd05-272">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-272">Details</span></span>

<span data-ttu-id="6bd05-273">Cennik oprogramowania bezterminowego opublikowany 1 marca 2021 r. obejmował rynki, które nie powinny tam być.</span><span class="sxs-lookup"><span data-stu-id="6bd05-273">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="6bd05-274">Cennik oprogramowania bezterminowego został zaktualizowany 17 marca 2021 r. o korekty.</span><span class="sxs-lookup"><span data-stu-id="6bd05-274">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="6bd05-275">Te poprawki miały zastosowanie tylko do:</span><span class="sxs-lookup"><span data-stu-id="6bd05-275">These corrections were only applicable to:</span></span>

- <span data-ttu-id="6bd05-276">Identyfikator produktu: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="6bd05-276">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="6bd05-277">Nazwa produktu: Windows 10 Home do wersji Pro Upgrade for Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6bd05-277">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="6bd05-278">Usunięte lub nieobsługiwane rynki: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, LM, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="6bd05-278">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="6bd05-279">Te zmiany dotyczą tylko powyższego produktu.</span><span class="sxs-lookup"><span data-stu-id="6bd05-279">These changes only apply to the above product.</span></span> <span data-ttu-id="6bd05-280">Inne produkty nie miały poprawek.</span><span class="sxs-lookup"><span data-stu-id="6bd05-280">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="6bd05-281">Następne kroki i zasoby</span><span class="sxs-lookup"><span data-stu-id="6bd05-281">Next steps and resources</span></span>

- <span data-ttu-id="6bd05-282">Partnerzy, którzy transakcjiują oprogramowanie bezterminowe, powinni pobrać najnowszy cennik oprogramowania bezterminowego.</span><span class="sxs-lookup"><span data-stu-id="6bd05-282">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="6bd05-283">Zapoznaj się z [kodami krajów regionów,](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) aby uzyskać przyjazne mapowanie dwuliterowego skrótu na kraje.</span><span class="sxs-lookup"><span data-stu-id="6bd05-283">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="6bd05-284">Wersja zestawu SDK w .NET Standard (wersja 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="6bd05-284">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-285">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-285">Categories</span></span>

- <span data-ttu-id="6bd05-286">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="6bd05-286">Date: 2021-03-23</span></span>

- <span data-ttu-id="6bd05-287">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-287">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="6bd05-288">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-288">Impacted audience</span></span>

<span data-ttu-id="6bd05-289">Partnerzy z rozliczeniami bezpośrednimi i dostawcy pośredni uczestniczący w programie CSP, którzy Partner Center zestawu SDK platformy .NET.</span><span class="sxs-lookup"><span data-stu-id="6bd05-289">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-290">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-290">Details</span></span>

<span data-ttu-id="6bd05-291">Od 23 marca 2020 r. partnerzy mogą rozpocząć pobieranie wersji pakietu [MicrosoftPartnerCenter.NETSDK (galerii NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)wraz ze zaktualizowanymi publicznymi zestaw SDK Centrum partnerskiego [przykładami usługi GitHub.](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="6bd05-291">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="6bd05-292">Ta wersja zawiera aktualizacje następujących metod:</span><span class="sxs-lookup"><span data-stu-id="6bd05-292">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="6bd05-293">Aktualizacja inspekcji: nowe typy operacji</span><span class="sxs-lookup"><span data-stu-id="6bd05-293">Audit Updated: New operation types</span></span>

<span data-ttu-id="6bd05-294">Dodano [nowe typy operacji,](https://docs.microsoft.com/partner-center/develop/auditing-resources) aby wiedzieć, kiedy klient zatwierdził i zakończył działanie daP.</span><span class="sxs-lookup"><span data-stu-id="6bd05-294">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="6bd05-295">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="6bd05-295">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="6bd05-296">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="6bd05-296">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="6bd05-297">Aktualizacja inspekcji: nowe typy zasobów i operacji</span><span class="sxs-lookup"><span data-stu-id="6bd05-297">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="6bd05-298">Dodano [nowe typy zasobów i operacji](https://docs.microsoft.com/partner-center/develop/auditing-resources) na potrzeby obsługi scenariusza roli katalogu klienta.</span><span class="sxs-lookup"><span data-stu-id="6bd05-298">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="6bd05-299">Nowy typ zasobu "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="6bd05-299">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="6bd05-300">Typy operacji "AddUserMember" i "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="6bd05-300">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="6bd05-301">Aktualizacje zestawu SDK dla kont klientów</span><span class="sxs-lookup"><span data-stu-id="6bd05-301">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="6bd05-302">Obsługa get /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="6bd05-302">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="6bd05-303">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="6bd05-303">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="6bd05-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="6bd05-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="6bd05-305">Dodatkowe zmiany</span><span class="sxs-lookup"><span data-stu-id="6bd05-305">Additional changes</span></span>

<span data-ttu-id="6bd05-306">Następujące zmiany są wprowadzane w ramach nowego handlu i są obecnie dostępne na zaproszenie tylko dla partnerów, którzy są częścią nowego doświadczenia handlowego M365/D365 w wersji Technical Preview.</span><span class="sxs-lookup"><span data-stu-id="6bd05-306">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="6bd05-307">Partnerzy, którzy nie są częścią wersji New Commerce Technical Preview, nie powinni zauważyć wpływu i powinni być zgodni z poprzednimi wersjami.</span><span class="sxs-lookup"><span data-stu-id="6bd05-307">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="6bd05-308">Zmiany katalogu:</span><span class="sxs-lookup"><span data-stu-id="6bd05-308">Catalog Changes:</span></span>

  - <span data-ttu-id="6bd05-309">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="6bd05-309">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="6bd05-310">Zakup i zarządzanie:</span><span class="sxs-lookup"><span data-stu-id="6bd05-310">Purchase and Manage:</span></span>
  - <span data-ttu-id="6bd05-311">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="6bd05-311">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="6bd05-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="6bd05-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="6bd05-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="6bd05-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="6bd05-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="6bd05-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="6bd05-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="6bd05-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="6bd05-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="6bd05-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-317">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-317">Next Steps</span></span>

- <span data-ttu-id="6bd05-318">Pobierz najnowszą wersję [microsoftPartnerCenter.NETSDK (Galeria NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="6bd05-318">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="6bd05-319">Pobieranie i przeglądanie [przykładów usługi GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="6bd05-319">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="6bd05-320">Oferta komercyjnej platformy handlowej programu CSP i zachęty FY21 CSP dla kwalifikujących się ofert</span><span class="sxs-lookup"><span data-stu-id="6bd05-320">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-321">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-321">Categories</span></span>

- <span data-ttu-id="6bd05-322">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="6bd05-322">Date: 2021-03-18</span></span>
- <span data-ttu-id="6bd05-323">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-323">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-324">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-324">Impacted audience</span></span>

<span data-ttu-id="6bd05-325">Dostawcy pośredni i bezpośredni partnerzy rozliczani w Dostawca rozwiązań w chmurze programie</span><span class="sxs-lookup"><span data-stu-id="6bd05-325">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="6bd05-326">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-326">Details</span></span>

<span data-ttu-id="6bd05-327">Dostawcy pośredni i bezpośredni partnerzy rozliczający w programie Dostawca rozwiązań w chmurze mogą sprzedawać oferty innych firm i uzyskać zachętę motywacyjną dla każdej kwalifikującej się oferty innej firmy Partner Center lub Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="6bd05-327">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="6bd05-328">Zachęta będzie mieć formę rachunku za rozliczaną sprzedaż dla kwalifikujących się ofert i będzie dostępna do 30 czerwca **2021 r.**.</span><span class="sxs-lookup"><span data-stu-id="6bd05-328">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="6bd05-329">Kontynuuj dalsze informacje na temat tej zachęty oferty komercyjnej platformy handlowej CSP poniżej i skontaktuj się z klientami już dzisiaj, aby zidentyfikować odpowiednie oferty, aby umożliwić ich dalszy sukces i transformację cyfrową.</span><span class="sxs-lookup"><span data-stu-id="6bd05-329">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="6bd05-330">Współpracujemy z niezależnymi dostawcami oprogramowania (ISV), aby wprowadzić na rynek najnowsze rozwiązania IaaS i SaaS dla klientów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6bd05-330">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="6bd05-331">Wydawcy isV mają możliwość włączenia sprzedaży swoich ofert za pośrednictwem kanału partnerskiego firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6bd05-331">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="6bd05-332">Nasze oferty kwalifikujące się do zachęt można podzielone na dwie kategorie:</span><span class="sxs-lookup"><span data-stu-id="6bd05-332">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="6bd05-333">Wybierz oferty SaaS i IaaS innych firm ze stanem zniechęceń do współscenizacji adresu IP platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="6bd05-333">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="6bd05-334">Aplikacje SaaS zintegrowane z usługą Teams lub co najmniej dwie Microsoft 365 aplikacji zwiększających produktywność, takich jak PowerPoint, Word, Excel, Outlook lub SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6bd05-334">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="6bd05-335">Następne kroki i zasoby</span><span class="sxs-lookup"><span data-stu-id="6bd05-335">Next steps and resources</span></span>

- <span data-ttu-id="6bd05-336">Dowiedz się więcej o zarobkach [w programie Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps (Zachęty dla partnerów do sprzedaży kwalifikujących się aplikacji na platformie handlowej).</span><span class="sxs-lookup"><span data-stu-id="6bd05-336">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="6bd05-337">Nowe oferty są dodawane co miesiąc.</span><span class="sxs-lookup"><span data-stu-id="6bd05-337">New offers are added monthly.</span></span>  
- [<span data-ttu-id="6bd05-338">Dostawca rozwiązań w chmurze zasobów zachęt dla partnerów rozliczanych bezpośrednio</span><span class="sxs-lookup"><span data-stu-id="6bd05-338">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="6bd05-339">Dostawca rozwiązań w chmurze zasobów zachęt dostawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="6bd05-339">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="6bd05-340">Przejrzyj tę [prezentację,](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) aby dowiedzieć się więcej o sprzedaży aplikacji platformy handlowej.</span><span class="sxs-lookup"><span data-stu-id="6bd05-340">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="6bd05-341">Zapoznaj się z dodatkowymi zasobami [tutaj.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)</span><span class="sxs-lookup"><span data-stu-id="6bd05-341">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="6bd05-342">Eksplorowanie katalogu komercyjnej platformy [handlowej w Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) lub [Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="6bd05-342">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="6bd05-343">Integrowanie [aplikacji z](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) firmową platformą handlowa przy użyciu interfejsów API</span><span class="sxs-lookup"><span data-stu-id="6bd05-343">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="6bd05-344">Docieranie do isvs you interested in doing business with</span><span class="sxs-lookup"><span data-stu-id="6bd05-344">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="6bd05-345">Dostawcy pośredni muszą integrować się przy użyciu interfejsów API i kierować odsprzedawcami aplikacji do sprzedaży</span><span class="sxs-lookup"><span data-stu-id="6bd05-345">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-346">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-346">Questions?</span></span>  

<span data-ttu-id="6bd05-347">Zapoznaj się [z tym artykułem,](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) aby zapoznać się z omówieniem platformy handlowej w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6bd05-347">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="6bd05-348">Jeśli potrzebujesz dodatkowej pomocy, możesz utworzyć wniosek o pomoc techniczną w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6bd05-348">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="6bd05-349">Dowiedz się więcej na stronie [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="6bd05-349">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="6bd05-350">Power BI Premium oferty nazewnictwa i aktualizacji wymagań wstępnych</span><span class="sxs-lookup"><span data-stu-id="6bd05-350">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-351">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-351">Categories</span></span>

- <span data-ttu-id="6bd05-352">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="6bd05-352">Date: 2021-03-18</span></span>
- <span data-ttu-id="6bd05-353">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-353">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-354">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-354">Summary</span></span>

<span data-ttu-id="6bd05-355">Ostateczny cennik z 1 kwietnia 2021 r. zostanie zaktualizowany w celu zwiększenia przejrzystości nazw i/lub informacji o wymaganiach wstępnych dotyczących Power BI Premium ofert dla 1 użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6bd05-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-356">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-356">Impacted audience</span></span>

<span data-ttu-id="6bd05-357">Dostawca rozwiązań w chmurze (CSP) partnerów bezpośrednich i pośrednich</span><span class="sxs-lookup"><span data-stu-id="6bd05-357">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-358">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-358">Details</span></span>

<span data-ttu-id="6bd05-359">Ostateczny cennik z 1 kwietnia 2021 r. zostanie zaktualizowany, aby dodać przejrzystość do nazewnictwa i/lub informacji o wymaganiach wstępnych dotyczących Power BI Premium ofert na użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6bd05-359">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="6bd05-360">Do momentu zaktualizowania ostatecznego cennika skorzystaj z informacji w tej sekcji, aby upewnić się, że zamówiony jest prawidłowy produkt.</span><span class="sxs-lookup"><span data-stu-id="6bd05-360">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="6bd05-361">Poniżej przedstawiono szczegóły dotyczące objętej sku i wymagań wstępnych.</span><span class="sxs-lookup"><span data-stu-id="6bd05-361">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="6bd05-362">Nazwa wyświetlana oferty w wersji zapoznawczej cennika z 1 marca</span><span class="sxs-lookup"><span data-stu-id="6bd05-362">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="6bd05-363">Zaktualizowano nazwę wyświetlaną oferty w ostatecznym cenniku z 1 kwietnia</span><span class="sxs-lookup"><span data-stu-id="6bd05-363">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="6bd05-364">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-364">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="6bd05-365">Power BI Premium na użytkownika Add-On (cennik dla pracowników organizacji non profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-365">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="6bd05-366">Power BI Premium na użytkownika Add-On **(Office)** (cennik dla pracowników organizacji non-profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-366">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="6bd05-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="6bd05-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="6bd05-368">Klienci muszą mieć jedno z następujących wymagań wstępnych, aby kupić tę ofertę:</span><span class="sxs-lookup"><span data-stu-id="6bd05-368">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="6bd05-369">Nazwa wyświetlana oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-369">Offer display name</span></span> | <span data-ttu-id="6bd05-370">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-370">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6bd05-371">Microsoft 365 E5 (cennik dla pracowników organizacji non profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-371">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="6bd05-372">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="6bd05-372">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="6bd05-373">Microsoft 365 E5 bez konferencji audio (cennik dla personelu organizacji non profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-373">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6bd05-374">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="6bd05-374">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="6bd05-375">Office 365 E5 (cennik dla pracowników organizacji non profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-375">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="6bd05-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="6bd05-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="6bd05-377">Wersja próbna usługi Office 365 E5 (cennik dla pracowników organizacji non profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-377">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="6bd05-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="6bd05-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="6bd05-379">Office 365 E5 bez konferencji audio (cennik dla pracowników organizacji non-profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-379">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6bd05-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="6bd05-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="6bd05-381">Do zakupu Power BI Premium wymagana jest następująca oferta usługi:</span><span class="sxs-lookup"><span data-stu-id="6bd05-381">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="6bd05-382">Nazwa wyświetlana oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-382">Offer display name</span></span> | <span data-ttu-id="6bd05-383">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-383">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="6bd05-384">Power BI Premium na użytkownika Add-On (cennik dla pracowników non profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-384">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6bd05-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="6bd05-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="6bd05-386">Klienci muszą mieć następujące wymagania wstępne, aby kupić tę ofertę:</span><span class="sxs-lookup"><span data-stu-id="6bd05-386">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="6bd05-387">Nazwa wyświetlana oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-387">Offer display name</span></span> | <span data-ttu-id="6bd05-388">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-388">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="6bd05-389">Power BI Pro (Nonprofit Staff Pricing)</span><span class="sxs-lookup"><span data-stu-id="6bd05-389">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="6bd05-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="6bd05-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="6bd05-391">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-391">Next steps</span></span>

<span data-ttu-id="6bd05-392">Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-392">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="6bd05-393">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-393">Questions?</span></span>

<span data-ttu-id="6bd05-394">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-394">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="6bd05-395">Aktualizacje marcowych cen dla Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="6bd05-395">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-396">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-396">Categories</span></span>

- <span data-ttu-id="6bd05-397">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="6bd05-397">Date: 2021-03-16</span></span>
- <span data-ttu-id="6bd05-398">Oferty/rynki</span><span class="sxs-lookup"><span data-stu-id="6bd05-398">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-399">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-399">Summary</span></span>

<span data-ttu-id="6bd05-400">Poprawiono niepoprawne ceny z marca 2021 r. dla waluty Microsoft 365 F3 Funt brytyjskie (GB) i Euro (EUR).</span><span class="sxs-lookup"><span data-stu-id="6bd05-400">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-401">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-401">Impacted audience</span></span>

<span data-ttu-id="6bd05-402">Partnerzy kupują Microsoft 365 F3 w GB lub EUR między 1 marca a 17 marca 2021 r. w ramach programu Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="6bd05-402">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-403">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-403">Details</span></span>

<span data-ttu-id="6bd05-404">Firma Microsoft rozwiązała problem z nieprawidłowymi cenami Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="6bd05-404">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="6bd05-405">Nieprawidłowe ceny dotyczyły gb/usd i tylko ofert zakupionych w okresie od 1 marca do 17 marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-405">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="6bd05-406">Poniżej przedstawiono oferty i waluty, których to ma wpływ.</span><span class="sxs-lookup"><span data-stu-id="6bd05-406">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="6bd05-407">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-407">Offer name</span></span> | <span data-ttu-id="6bd05-408">Waluta</span><span class="sxs-lookup"><span data-stu-id="6bd05-408">Currency</span></span> | <span data-ttu-id="6bd05-409">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-409">Offer ID</span></span> | <span data-ttu-id="6bd05-410">Identyfikator materiału</span><span class="sxs-lookup"><span data-stu-id="6bd05-410">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="6bd05-411">Microsoft 365 F3 (Wc)</span><span class="sxs-lookup"><span data-stu-id="6bd05-411">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="6bd05-412">GBP</span><span class="sxs-lookup"><span data-stu-id="6bd05-412">GBP</span></span> | <span data-ttu-id="6bd05-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="6bd05-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="6bd05-414">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="6bd05-414">AAD-11626</span></span> |
| <span data-ttu-id="6bd05-415">Microsoft 365 F3 (komercyjne)</span><span class="sxs-lookup"><span data-stu-id="6bd05-415">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="6bd05-416">EUR</span><span class="sxs-lookup"><span data-stu-id="6bd05-416">EUR</span></span>| <span data-ttu-id="6bd05-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="6bd05-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="6bd05-418">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="6bd05-418">AAA-89898</span></span> |
 
<span data-ttu-id="6bd05-419">Cenniki bazowe licencji w wersji zapoznawczej z marca i kwietnia zostały zaktualizowane 16 marca o godzinie 17:00 czasu pacyficznego.</span><span class="sxs-lookup"><span data-stu-id="6bd05-419">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-420">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-420">Next steps</span></span>

- <span data-ttu-id="6bd05-421">Partnerzy powinni ponownie pobrać bieżące cenniki oparte na licencjach, zarówno w wersji zapoznawczej z marca, jak i kwietnia, z tymi korektami cen, jeśli ma to zastosowanie.</span><span class="sxs-lookup"><span data-stu-id="6bd05-421">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="6bd05-422">Firma Microsoft skontaktuje się z partnerami, których dotyczy problem, w najbliższych tygodniach za pośrednictwem poczty e-mail, aby poinformować ich o następnych krokach związanych z korygowania transakcji, których dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="6bd05-422">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-423">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-423">Questions?</span></span>

<span data-ttu-id="6bd05-424">Aby uzyskać więcej pytań, zapoznaj się z odpowiednimi społecznościami usługi Yammer dla CSP.</span><span class="sxs-lookup"><span data-stu-id="6bd05-424">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="6bd05-425">Aktualizowanie nazwy firmy prawnej za pomocą Partner Center</span><span class="sxs-lookup"><span data-stu-id="6bd05-425">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-426">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-426">Categories</span></span>

- <span data-ttu-id="6bd05-427">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="6bd05-427">Date: 2021-03-16</span></span>
- <span data-ttu-id="6bd05-428">Wydajność dysków & skalowania</span><span class="sxs-lookup"><span data-stu-id="6bd05-428">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-429">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-429">Summary</span></span>

<span data-ttu-id="6bd05-430">Od marca 2021 r. partnerzy Microsoft Partner Network (MPN) i odsprzedawcy pośredni Dostawca rozwiązań w chmurze (CSP) mogą aktualizować swoją nazwę firmy prawnej za pośrednictwem Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6bd05-430">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-431">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-431">Impacted audience</span></span>

<span data-ttu-id="6bd05-432">Partnerzy MPN i odsprzedawcy pośredni w programie CSP (nie dotyczy partnerów rozliczanych bezpośrednio w programie CSP)</span><span class="sxs-lookup"><span data-stu-id="6bd05-432">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-433">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-433">Details</span></span>

<span data-ttu-id="6bd05-434">Od marca 2021 r. partnerzy MPN i odsprzedawcy pośredni w programie CSP mogą aktualizować swoje prawne nazwy firmy za pośrednictwem Partner Center w sposób zgodny i samoobsługowy.</span><span class="sxs-lookup"><span data-stu-id="6bd05-434">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="6bd05-435">Dzięki tej nowej funkcji partnerzy nie będą już musieli przesyłać biletu Partner Center pomocy technicznej, aby zaktualizować nazwę firmy.</span><span class="sxs-lookup"><span data-stu-id="6bd05-435">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="6bd05-436">Pozwoli to zaoszczędzić znaczną ilość czasu dla partnerów podczas wykonywania tych działań.</span><span class="sxs-lookup"><span data-stu-id="6bd05-436">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="6bd05-437">Aby dowiedzieć się więcej, zobacz [Aktualizowanie legalnych profilów biznesowych.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="6bd05-437">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="6bd05-438">Upewnij się, że nazwa firmy w Twoim profilu biznesowym jest bezpłatna od błędów pisowni i skrótów, i dokładnie pasuje do formalnych rekordów rejestracji firmy w firmie.</span><span class="sxs-lookup"><span data-stu-id="6bd05-438">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="6bd05-439">Aby uzyskać więcej informacji na temat aktualizowania profilu organizacji, zobacz [Weryfikowanie profilu organizacji.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="6bd05-439">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-440">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-440">Next steps</span></span>

<span data-ttu-id="6bd05-441">Udostępnij te informacje w organizacji, aby odpowiedni zespół może przeglądać i aktualizować swoje procesy.</span><span class="sxs-lookup"><span data-stu-id="6bd05-441">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-442">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-442">Questions?</span></span>

<span data-ttu-id="6bd05-443">Jeśli masz dodatkowe pytania, sprawdź odpowiednie społeczności CSP w usłudze Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-443">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="6bd05-444">Aktualizacja ewolucji programu Dostawca rozwiązań w chmurze (CSP) i zmiany programu licencjonowania Open License</span><span class="sxs-lookup"><span data-stu-id="6bd05-444">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-445">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-445">Categories</span></span>

- <span data-ttu-id="6bd05-446">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="6bd05-446">Date: 2021-03-15</span></span>
- <span data-ttu-id="6bd05-447">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-447">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-448">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-448">Summary</span></span>

<span data-ttu-id="6bd05-449">Nowe bezterminowe oferty oprogramowania w sektorze komercyjnym i publicznym będą dostępne w programie licencjonowania Dostawca rozwiązań w chmurze (CSP) wraz ze zmianami w programie licencjonowania Open.</span><span class="sxs-lookup"><span data-stu-id="6bd05-449">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-450">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-450">Impacted audience</span></span>

<span data-ttu-id="6bd05-451">Dystrybutorzy handlowi i odsprzedawcy zarządzani sprzedawani za pośrednictwem programu Licencjonowanie Open, a także wszyscy partnerzy programu CSP, którzy odsprzedają oprogramowanie bezterminowe</span><span class="sxs-lookup"><span data-stu-id="6bd05-451">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-452">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-452">Details</span></span>

<span data-ttu-id="6bd05-453">We wrześniu 2020 r. firma [Microsoft](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) ogłosiła szereg kroków w ramach naszej cyfrowej transformacji w celu rozszerzenia możliwości partnerów w programie CSP, w tym dostępności oprogramowania lokalnego dla partnerów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-453">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="6bd05-454">Te zmiany umożliwiają partnerom rozwój firmy i rozszerzenie zasięgu dzięki wykorzystaniu licencji na oprogramowanie w programie CSP, pozycjonowając ich w celu osiągnięcia sukcesu we współczesnym świecie chmury.</span><span class="sxs-lookup"><span data-stu-id="6bd05-454">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="6bd05-455">Zapewniają one również klientom przejście do chmury i zapewniają partnerom elastyczność potrzebną dla środowisk chmury hybrydowej klienta.</span><span class="sxs-lookup"><span data-stu-id="6bd05-455">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="6bd05-456">W kontynuacji tej transformacji cyfrowej ogłaszamy następujące zmiany:</span><span class="sxs-lookup"><span data-stu-id="6bd05-456">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="6bd05-457">1 lipca 2021 r.: do cennika programu Licencjonowanie open nie zostaną dodane żadne nowe jednostki SKU, produkty ani promocje.</span><span class="sxs-lookup"><span data-stu-id="6bd05-457">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="6bd05-458">7 lipca 2021 r.: do cennika oprogramowania CSP zostaną dodane dwie oferty komercyjne: Uzyskaj [](./2020-december.md#9)oryginalne systemy Windows i Visual Studio Professional oraz oferty sektora publicznego (dla instytucji rządowych, edukacji i organizacji non profit — zobacz ogłoszenie).</span><span class="sxs-lookup"><span data-stu-id="6bd05-458">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="6bd05-459">Cennik można znaleźć w sekcji Oprogramowanie na stronie Sell > Pricing & Offers (Ceny & [sprzedaży)](https://partnercenter.microsoft.com/pcv/sales) w Partner Center i zostanie ponownie opublikowany w tym dniu.</span><span class="sxs-lookup"><span data-stu-id="6bd05-459">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="6bd05-460">Aby uzyskać szczegółowe informacje dotyczące ewolucji programu CSP i zmian programu licencjonowania Open License, zobacz **Następne kroki** poniżej.</span><span class="sxs-lookup"><span data-stu-id="6bd05-460">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-461">Następne kroki:</span><span class="sxs-lookup"><span data-stu-id="6bd05-461">Next Steps:</span></span>

- <span data-ttu-id="6bd05-462">Ewolucja programu CSP: Przejrzyj oprogramowanie [bezterminowe w Dostawca rozwiązań w chmurze gotowość](https://partner.microsoft.com/resources/collection/software-in-csp#/) programu.</span><span class="sxs-lookup"><span data-stu-id="6bd05-462">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="6bd05-463">Użyj tej [mapy gotowości,](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) aby szybko znaleźć odpowiednie informacje dla swojej roli.</span><span class="sxs-lookup"><span data-stu-id="6bd05-463">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="6bd05-464">Zmiany programu licencjonowania Open: Przejrzyj materiały dotyczące zmian gotowości programu CSP i [Open License Program.](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)</span><span class="sxs-lookup"><span data-stu-id="6bd05-464">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="6bd05-465">Użyj tej [mapy gotowości,](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) aby szybko znaleźć odpowiednie informacje dla swojej roli.</span><span class="sxs-lookup"><span data-stu-id="6bd05-465">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-466">Pytania</span><span class="sxs-lookup"><span data-stu-id="6bd05-466">Questions</span></span>

<span data-ttu-id="6bd05-467">Aby uzyskać więcej pytań, zapoznaj się z odpowiednimi społecznościami usługi Yammer dla CSP.</span><span class="sxs-lookup"><span data-stu-id="6bd05-467">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="6bd05-468">Aktualizacja do poprzedniego anonsu: Premium Assessments , dodatek do Menedżera zgodności</span><span class="sxs-lookup"><span data-stu-id="6bd05-468">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-469">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-469">Categories</span></span>

- <span data-ttu-id="6bd05-470">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="6bd05-470">Date: 2021-03-15</span></span>
- <span data-ttu-id="6bd05-471">Rozwijanie firmy</span><span class="sxs-lookup"><span data-stu-id="6bd05-471">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-472">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-472">Summary</span></span>

<span data-ttu-id="6bd05-473">Oferty wersji próbnej nie powinny być wymienione w cenniku i zostaną usunięte.</span><span class="sxs-lookup"><span data-stu-id="6bd05-473">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-474">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-474">Impacted audience</span></span>

<span data-ttu-id="6bd05-475">Partnerzy inicjujące transakcje za pośrednictwem Dostawca rozwiązań w chmurze</span><span class="sxs-lookup"><span data-stu-id="6bd05-475">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-476">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-476">Details</span></span>

<span data-ttu-id="6bd05-477">Oferty wersji próbnej nie powinny zostać uwzględnione w cenniku.</span><span class="sxs-lookup"><span data-stu-id="6bd05-477">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="6bd05-478">Zostaną one usunięte z cennika z 1 maja 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-478">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="6bd05-479">Oryginalne zawiadomienie znajduje się [tutaj.](./2021-february.md#4)</span><span class="sxs-lookup"><span data-stu-id="6bd05-479">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="6bd05-480">Dodatkowe zasoby</span><span class="sxs-lookup"><span data-stu-id="6bd05-480">Additional resources</span></span>

- [<span data-ttu-id="6bd05-481">Microsoft 365 zabezpieczeń i zgodności E5</span><span class="sxs-lookup"><span data-stu-id="6bd05-481">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="6bd05-482">Tworzenie ocen i zarządzanie nimi w Menedżerze zgodności firmy Microsoft — Microsoft 365 Zgodności</span><span class="sxs-lookup"><span data-stu-id="6bd05-482">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="6bd05-483">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-483">Next steps</span></span>

<span data-ttu-id="6bd05-484">Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-484">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-485">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-485">Questions?</span></span>

<span data-ttu-id="6bd05-486">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-486">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="6bd05-487">Migrowanie rozwiązań z usługi One Commercial Partner (OCP) do platformy handlowej firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="6bd05-487">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-488">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-488">Categories</span></span>

- <span data-ttu-id="6bd05-489">Data: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="6bd05-489">Date: 2021-03-12</span></span>
- <span data-ttu-id="6bd05-490">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-490">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-491">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-491">Summary</span></span>

<span data-ttu-id="6bd05-492">Od 29 marca 2021 r. zaczniesz mieć ograniczone możliwości jednego partnera komercyjnego (OCP, One Commercial Partner) go-to-market (GTM).</span><span class="sxs-lookup"><span data-stu-id="6bd05-492">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="6bd05-493">Zachęcamy do migrowania rozwiązań na platformę handlową w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6bd05-493">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-494">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-494">Impacted audience</span></span>

<span data-ttu-id="6bd05-495">Organizacje sprzedają się razem z rozwiązaniami w OCP GTM</span><span class="sxs-lookup"><span data-stu-id="6bd05-495">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-496">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-496">Details</span></span>

<span data-ttu-id="6bd05-497">W grudniu 2020 r. rozpoczęliśmy podróż od narzędzia Microsoft OCP GTM do platformy handlowej firmy Microsoft w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6bd05-497">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="6bd05-498">To przejście rozszerza możliwości platformy handlowej, na której można prezentować swoje rozwiązania milionom klientów, dwukierunkowo udostępniać możliwości innym sprzedawcom firmy Microsoft i partnerów oraz wspólnie sprzedawać innowacyjne rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="6bd05-498">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="6bd05-499">Kolejny kamień milowy w przejściu zostanie miał miejsce 29 marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-499">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="6bd05-500">Właśnie wtedy zaczniesz mieć ograniczone możliwości OCP GTM, a niektóre pola stają się tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="6bd05-500">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="6bd05-501">Jeśli obecnie sprzedajesz rozwiązania w OCP GTM, zachęcamy do migrowania rozwiązań na platformę handlową, aby wykorzystać jej możliwości i uprościć środowisko publikowania.</span><span class="sxs-lookup"><span data-stu-id="6bd05-501">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="6bd05-502">Przejście na platformę handlową sprawia, Partner Center głównym miejscem docelowym dla publikowania we współpracy sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="6bd05-502">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="6bd05-503">Jest to miejsce, w którym można kontynuować rozwój firmy, łącząc swoje rozwiązania z naszymi wspólnymi klientami za pośrednictwem tych samych kanałów i funkcji w produktach, których używamy dla produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6bd05-503">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="6bd05-504">[Dowiedz się więcej o platformie handlowej](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="6bd05-504">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-505">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-505">Next steps</span></span>

- <span data-ttu-id="6bd05-506">Jeśli rozwiązania nie zostały jeszcze przeniesione, postępuj [](/azure/marketplace/co-sell-solution-migration) zgodnie z instrukcjami podanymi w przewodniku przejścia lub wyświetl samouczek wideo krok po kroku, aby ukończyć wszystkie działania migracji i rozpocząć publikowanie swoich rozwiązań na platformie handlowej. [](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)</span><span class="sxs-lookup"><span data-stu-id="6bd05-506">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="6bd05-507">W przypadku pytań dotyczących ograniczonego środowiska możliwości w UCP GTM zobacz wymagania dotyczące współpracy sprzedaży, aby opublikować w artykule Często zadawane pytania dotyczące platformy handlowej [firmy Microsoft.](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)</span><span class="sxs-lookup"><span data-stu-id="6bd05-507">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="6bd05-508">(Zobacz sekcję "Ograniczone możliwości OCP GTM od 29 marca 2021 r.").</span><span class="sxs-lookup"><span data-stu-id="6bd05-508">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-509">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-509">Questions?</span></span>

<span data-ttu-id="6bd05-510">Jeśli [masz pytania](https://partner.microsoft.com/support/?stage=1) lub potrzebujesz więcej informacji, skontaktuj się z pomocą techniczną.</span><span class="sxs-lookup"><span data-stu-id="6bd05-510">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="6bd05-511">Rozszerzanie nowego doświadczenia handlowego w programie Dostawca rozwiązań w chmurze (CSP) dla platformy Azure na Rosję</span><span class="sxs-lookup"><span data-stu-id="6bd05-511">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-512">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-512">Categories</span></span>

- <span data-ttu-id="6bd05-513">Data: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="6bd05-513">Date: 2021-03-10</span></span>
- <span data-ttu-id="6bd05-514">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-514">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-515">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-515">Impacted audience</span></span>

<span data-ttu-id="6bd05-516">Wszyscy partnerzy w Rosyjskim inicjuje transakcję za pośrednictwem Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="6bd05-516">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-517">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-517">Details</span></span>

<span data-ttu-id="6bd05-518">Od 10 marca 2021 r. z przyjemnością ogłaszamy dostępność nowego rozwiązania handlowego w programie CSP dla platformy **Azure w Rosyjskim**.</span><span class="sxs-lookup"><span data-stu-id="6bd05-518">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="6bd05-519">To środowisko usprawni i poprawi sposób, w jaki klienci kupują i zużywają usługi platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="6bd05-519">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="6bd05-520">Zapewni ona również partnerom w programie CSP spójny widok cen platformy Azure w różnych ruchach sprzedaży, cen USD dla globalnej spójności, wyrównania dat rozliczeń i dostępu do Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="6bd05-520">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-521">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-521">Next steps</span></span>

<span data-ttu-id="6bd05-522">Dostępnych jest kilka zasobów wprowadzających nowe środowisko handlowe platformy Azure i udostępniających dodatkowe informacje.</span><span class="sxs-lookup"><span data-stu-id="6bd05-522">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="6bd05-523">Najnowsze często zadawane pytania, talii, wideo i inne informacje można znaleźć w galerii zasobów aktualizacji [programu CSP.](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)</span><span class="sxs-lookup"><span data-stu-id="6bd05-523">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="6bd05-524">Partner Center klucza licencji oprogramowania i realizacji pobierania</span><span class="sxs-lookup"><span data-stu-id="6bd05-524">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-525">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-525">Categories</span></span>

- <span data-ttu-id="6bd05-526">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="6bd05-526">Date: 2021-03-04</span></span>
- <span data-ttu-id="6bd05-527">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-527">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-528">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-528">Summary</span></span>

<span data-ttu-id="6bd05-529">Funkcja Partner Center pobierania oprogramowania i realizacji klucza licencji została przywrócona.</span><span class="sxs-lookup"><span data-stu-id="6bd05-529">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-530">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-530">Impacted audience</span></span>

<span data-ttu-id="6bd05-531">Wszyscy Dostawca rozwiązań w chmurze (CSP) w ramach zamówień oprogramowania bezterminowych subskrypcji serwerów za pośrednictwem Partner Center</span><span class="sxs-lookup"><span data-stu-id="6bd05-531">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-532">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-532">Details</span></span>

<span data-ttu-id="6bd05-533">W odpowiedzi na opinie partnerów przywracamy możliwość realizacji Partner Center uzyskiwania kluczy oprogramowania i licencji w przypadku bezterminowych zamówień oprogramowania i zamówień na oprogramowanie subskrypcji serwera.</span><span class="sxs-lookup"><span data-stu-id="6bd05-533">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="6bd05-534">Zostanie on przywrócony do poprzedniego stanu przed usunięciem 19 stycznia 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-534">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="6bd05-535">(Zobacz [anons).](2020-september.md#17)</span><span class="sxs-lookup"><span data-stu-id="6bd05-535">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="6bd05-536">Należy pamiętać, że klucze licencji na oprogramowanie i linki pobierania są cennymi i wysoce pożądanymi zasobami własności intelektualnej.</span><span class="sxs-lookup"><span data-stu-id="6bd05-536">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="6bd05-537">W przypadku wycieku mogą one szybko zostać wyczerpane limity aktywacji i spowodować negatywne doświadczenia klientów i partnerów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-537">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-538">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-538">Next steps</span></span>

<span data-ttu-id="6bd05-539">Zapoznaj się z następującymi zasobami, aby uzyskać instrukcje dotyczące użycia i ważne wskazówki dotyczące dystrybucji kluczy oprogramowania:</span><span class="sxs-lookup"><span data-stu-id="6bd05-539">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="6bd05-540">Sprzedaż oprogramowania lokalnego za pośrednictwem programu CSP</span><span class="sxs-lookup"><span data-stu-id="6bd05-540">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="6bd05-541">[Partner Center nowego przewodnika operacji handlowych](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (zobacz **sekcję Guidance on Software Key Distribution** (Wskazówki dotyczące dystrybucji kluczy oprogramowania).</span><span class="sxs-lookup"><span data-stu-id="6bd05-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-542">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-542">Questions?</span></span>

<span data-ttu-id="6bd05-543">Jeśli masz dodatkowe pytania dotyczące tego powiadomienia, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-543">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="6bd05-544">Migrowanie transakcji z programu Partner Sales Connect (PSC) do Partner Center</span><span class="sxs-lookup"><span data-stu-id="6bd05-544">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-545">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-545">Categories</span></span>

- <span data-ttu-id="6bd05-546">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="6bd05-546">Date: 2021-03-04</span></span>
- <span data-ttu-id="6bd05-547">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-547">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-548">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-548">Summary</span></span>

<span data-ttu-id="6bd05-549">Partner Sales Connect (PSC) będzie miał dostęp tylko do odczytu od 31 marca 2021 r., dlatego zachęcamy do rozpoczęcia migracji twoich transakcji z programu PSC do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6bd05-549">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-550">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-550">Impacted audience</span></span>

<span data-ttu-id="6bd05-551">Partnerzy z transakcjami w chmurze</span><span class="sxs-lookup"><span data-stu-id="6bd05-551">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-552">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-552">Details</span></span>

<span data-ttu-id="6bd05-553">W ramach naszego wspólnego zobowiązania do rozwoju wspólna sprzedaż z firmą **Microsoft** to ścieżka, którą możesz **odkryć,** dostarczyć swoją wiedzę i rozszerzyć zasięg klientów, aby uzyskać pozytywne wyniki dla klientów.</span><span class="sxs-lookup"><span data-stu-id="6bd05-553">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="6bd05-554">Przy średniej transakcji, która jest **3,5** raza szybsza niż zwykle, zarządzanie doświadczeniem w zakresie współpracy sprzedaży w programie Partner Center umożliwia sprzedaż w kanałach bezpośrednich klientów, partnerów i sprzedawców firmy Microsoft oraz zarządzanie całym potokiem poleceń w jednej lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-554">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="6bd05-555">Od 31  marca **2021** r. program **PSC** będzie miał dostęp tylko do odczytu, dlatego zachęcamy do rozpoczęcia przechodzenia do programu Partner Center i uzyskiwania dostępu do tych ulepszeń możliwości:</span><span class="sxs-lookup"><span data-stu-id="6bd05-555">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="6bd05-556">**Dokładniejszy routing** transakcji, które udostępniasz firmie Microsoft właściwemu sprzedawcy, w zależności od rodzaju potrzebnej pomocy.</span><span class="sxs-lookup"><span data-stu-id="6bd05-556">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="6bd05-557">**Weryfikacja uprawnień do** transakcji z góry dla rozwiązań kwalifikujących się do zachęt oraz spełnianie kryteriów programu ISV Connect, upraszczając proces zatwierdzania i ostateczne potwierdzenie wykonania (POE).</span><span class="sxs-lookup"><span data-stu-id="6bd05-557">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="6bd05-558">**Bezproblemowe środowisko użytkownika** do zarządzania wszystkimi możliwościami sprzedaży i potencjalnymi klientami zakwalifikowanym do sprzedaży w jednym miejscu.</span><span class="sxs-lookup"><span data-stu-id="6bd05-558">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="6bd05-559">Niedawno dodaliśmy również nowe funkcje w programie Partner Center, które mogą pomóc w przenoszeniu:</span><span class="sxs-lookup"><span data-stu-id="6bd05-559">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="6bd05-560">Operacje zbiorcze dotyczące możliwości współpracy sprzedaży</span><span class="sxs-lookup"><span data-stu-id="6bd05-560">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="6bd05-561">[Funkcja migracji transakcji](../psc-to-pc.md) (zobacz **sekcję Migracja transakcji psc).**</span><span class="sxs-lookup"><span data-stu-id="6bd05-561">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="6bd05-562">Dzięki środowisku współpracy w Partner Center zespoły sprzedaży będą miały więcej czasu na skoncentrowanie się na tworzeniu potencjalnych klientów i szans sprzedaży, zamykaniu transakcji i tworzeniu długotrwałych relacji z klientami.</span><span class="sxs-lookup"><span data-stu-id="6bd05-562">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6bd05-563">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-563">Next steps</span></span>

<span data-ttu-id="6bd05-564">Skorzystaj z Partner Center [przejścia,](../psc-to-pc.md) aby przejść przez kroki migracji transakcji z usługi PSC do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6bd05-564">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-565">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-565">Questions?</span></span>

<span data-ttu-id="6bd05-566">W przypadku jakichkolwiek dodatkowych pytań skontaktuj się z pomocą [techniczną.](https://partner.microsoft.com/support/?stage=1)</span><span class="sxs-lookup"><span data-stu-id="6bd05-566">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="6bd05-567">Nowe produkty i oferty usługi Microsoft Dynamics 365 dostępne od 1 kwietnia 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-567">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-568">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-568">Categories</span></span>

- <span data-ttu-id="6bd05-569">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="6bd05-569">Date: 2021-03-04</span></span>
- <span data-ttu-id="6bd05-570">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-570">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-571">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-571">Summary</span></span>

<span data-ttu-id="6bd05-572">1 kwietnia 2021 r. firma Microsoft uruchomi kilka nowych produktów i ofert dla programu Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="6bd05-572">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-573">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-573">Impacted audience</span></span>

<span data-ttu-id="6bd05-574">Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="6bd05-574">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-575">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-575">Details</span></span>

<span data-ttu-id="6bd05-576">1 kwietnia 2021 r. firma Microsoft będzie wprowadzać następujące nowe produkty i oferty:</span><span class="sxs-lookup"><span data-stu-id="6bd05-576">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="6bd05-577">Power BI Premium na użytkownika</span><span class="sxs-lookup"><span data-stu-id="6bd05-577">Power BI Premium Per User</span></span>
- <span data-ttu-id="6bd05-578">Rozszerzenie segmentów i obszarów geograficznych customer voice and marketing USL</span><span class="sxs-lookup"><span data-stu-id="6bd05-578">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="6bd05-579">**Power BI Premium na użytkownika**</span><span class="sxs-lookup"><span data-stu-id="6bd05-579">**Power BI Premium Per User**</span></span>

<span data-ttu-id="6bd05-580">Firma Microsoft wprowadzi pierwszą ofertę dla użytkowników Power BI Premium użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6bd05-580">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="6bd05-581">Power BI Premium jest obecnie sprzedawane tylko w konstrukcji pojemności.</span><span class="sxs-lookup"><span data-stu-id="6bd05-581">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="6bd05-582">Power BI Premium na użytkownika zapewnia dostęp do funkcji analizy biznesowej (BI) i analizy przedsiębiorstwa.</span><span class="sxs-lookup"><span data-stu-id="6bd05-582">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="6bd05-583">Elastyczne licencjonowanie poszczególnych miejsc jest przeznaczone dla małych i średnich firm.</span><span class="sxs-lookup"><span data-stu-id="6bd05-583">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="6bd05-584">Przejrzyj szczegóły [Power BI wersji,](/power-platform-release-plan/2020wave2/power-bi/planned-features) aby dowiedzieć się więcej o tej ofercie.</span><span class="sxs-lookup"><span data-stu-id="6bd05-584">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="6bd05-585">**Szczegóły oferty**</span><span class="sxs-lookup"><span data-stu-id="6bd05-585">**Offer details**</span></span>

<span data-ttu-id="6bd05-586">Pamiętaj, że nazwa oferty różni się nieco od wersji zapoznawczej cennika.</span><span class="sxs-lookup"><span data-stu-id="6bd05-586">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="6bd05-587">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-587">Offer name</span></span> | <span data-ttu-id="6bd05-588">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-588">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="6bd05-589">Power BI Premium na użytkownika</span><span class="sxs-lookup"><span data-stu-id="6bd05-589">Power BI Premium Per User</span></span> | <span data-ttu-id="6bd05-590">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="6bd05-590">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="6bd05-591">Power BI Premium na użytkownika dla nauczycieli lub wykładowców</span><span class="sxs-lookup"><span data-stu-id="6bd05-591">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="6bd05-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="6bd05-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="6bd05-593">Power BI Premium na użytkownika dla uczniów</span><span class="sxs-lookup"><span data-stu-id="6bd05-593">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="6bd05-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="6bd05-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="6bd05-595">Power BI Premium na użytkownika (cennik dla pracowników niedochodowych)</span><span class="sxs-lookup"><span data-stu-id="6bd05-595">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6bd05-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="6bd05-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="6bd05-597">Power BI Premium na użytkownika Add-On</span><span class="sxs-lookup"><span data-stu-id="6bd05-597">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="6bd05-598">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="6bd05-598">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="6bd05-599">Power BI Premium na użytkownika Add-On dla nauczycieli lub wykładowców</span><span class="sxs-lookup"><span data-stu-id="6bd05-599">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="6bd05-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="6bd05-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="6bd05-601">Power BI Premium na użytkownika Add-On dla uczniów</span><span class="sxs-lookup"><span data-stu-id="6bd05-601">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="6bd05-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="6bd05-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="6bd05-603">Power BI Premium na użytkownika Add-On (cennik dla pracowników non profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-603">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6bd05-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="6bd05-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="6bd05-605">**Rozszerzenie segmentów i obszarów geograficznych CUSTOMER Voice and Marketing USL**</span><span class="sxs-lookup"><span data-stu-id="6bd05-605">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="6bd05-606">W związku z wprowadzeniem w grudniu 2020 r. oferty Dynamics 365 Customer Voice and Marketing USL zostały zmienione w celu dodania nowych krajów oraz bardziej niedochodowych i edukacyjnych jednostki SKU.</span><span class="sxs-lookup"><span data-stu-id="6bd05-606">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="6bd05-607">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-607">Offer name</span></span> | <span data-ttu-id="6bd05-608">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-608">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="6bd05-609">Dynamics 365 Customer Voice USL (cennik dla pracowników non-profit)</span><span class="sxs-lookup"><span data-stu-id="6bd05-609">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6bd05-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="6bd05-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="6bd05-611">Dynamics 365 Customer Voice USL dla nauczycieli lub wykładowców</span><span class="sxs-lookup"><span data-stu-id="6bd05-611">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="6bd05-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="6bd05-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="6bd05-613">Odwiedź następujące strony, aby dowiedzieć się więcej o tych ofertach:</span><span class="sxs-lookup"><span data-stu-id="6bd05-613">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="6bd05-614">Strona główna usługi Dynamics 365 Customer Service Voice</span><span class="sxs-lookup"><span data-stu-id="6bd05-614">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="6bd05-615">Strona główna usługi Dynamics 365 Marketing</span><span class="sxs-lookup"><span data-stu-id="6bd05-615">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="6bd05-616">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-616">Next steps</span></span>

<span data-ttu-id="6bd05-617">Przejrzyj zasoby dotyczące tego tematu i udostępnij te informacje odpowiednim uczestnikom projektu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-617">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="6bd05-618">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-618">Questions?</span></span>

<span data-ttu-id="6bd05-619">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-619">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="6bd05-620">Usługa Microsoft Drukowanie uniwersalne jest teraz dostępna w niektórych pakietach</span><span class="sxs-lookup"><span data-stu-id="6bd05-620">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="6bd05-621">Kategorie</span><span class="sxs-lookup"><span data-stu-id="6bd05-621">Categories</span></span>

- <span data-ttu-id="6bd05-622">Data: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="6bd05-622">Date: 2021-03-33</span></span>
- <span data-ttu-id="6bd05-623">Możliwości</span><span class="sxs-lookup"><span data-stu-id="6bd05-623">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6bd05-624">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="6bd05-624">Summary</span></span>

<span data-ttu-id="6bd05-625">Usługa Microsoft Drukowanie uniwersalne będzie dostępna do transakcji w ramach wybranych pakietów Microsoft 365 i jako dodatek autonomiczny od 1 marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-625">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6bd05-626">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="6bd05-626">Impacted audience</span></span>

<span data-ttu-id="6bd05-627">Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="6bd05-627">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="6bd05-628">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="6bd05-628">Details</span></span>

<span data-ttu-id="6bd05-629">[Drukowanie uniwersalne](https://aka.ms/universalprint) to Microsoft 365 drukowania, która nie wymaga lokalnych serwerów wydruku i umożliwia drukowanie na urządzeniach z systemem Windows na drukarkach zarejestrowanych na platformie Azure.</span><span class="sxs-lookup"><span data-stu-id="6bd05-629">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="6bd05-630">Będzie ona dostępna do transakcji od 1 marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="6bd05-630">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="6bd05-631">Pracownicy korzystają z drukowania bez sterowników, usprawnionego odnajdywania drukarek opartego na lokalizacji i intuicyjnego drukowania bez uczenia się.</span><span class="sxs-lookup"><span data-stu-id="6bd05-631">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="6bd05-632">Urządzenia przyłączone do usługi Azure Active Directory (Azure AD) używają istniejących poświadczeń usługi Azure AD w celu bezpiecznego drukowania.</span><span class="sxs-lookup"><span data-stu-id="6bd05-632">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="6bd05-633">Administratorzy zarządzają drukowaniem przy użyciu Azure Portal i mogą łatwo łączyć drukarki z natywną obsługą Drukowanie uniwersalne.</span><span class="sxs-lookup"><span data-stu-id="6bd05-633">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="6bd05-634">Drukowanie uniwersalne można wdrożyć za pomocą niezgodnych drukarek przy użyciu łącznik Drukowanie uniwersalne oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="6bd05-634">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="6bd05-635">Drukowanie uniwersalne zostaną wypełnione podczas startu w systemach Windows E3, A3, E5 i A5 oraz Microsoft 365 BP, F3, E3, A3, E5 i A5.</span><span class="sxs-lookup"><span data-stu-id="6bd05-635">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="6bd05-636">**Szczegóły oferty**</span><span class="sxs-lookup"><span data-stu-id="6bd05-636">**Offer details**</span></span>

<span data-ttu-id="6bd05-637">Pamiętaj, że nazwa oferty różni się nieco od wersji zapoznawczej cennika.</span><span class="sxs-lookup"><span data-stu-id="6bd05-637">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="6bd05-638">Nazwa oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-638">Offer name</span></span> | <span data-ttu-id="6bd05-639">Identyfikator oferty</span><span class="sxs-lookup"><span data-stu-id="6bd05-639">Offer ID</span></span> | <span data-ttu-id="6bd05-640">Identyfikator materiału</span><span class="sxs-lookup"><span data-stu-id="6bd05-640">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="6bd05-641">Drukowanie uniwersalne woluminu (500 zadań) — Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6bd05-641">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="6bd05-642">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="6bd05-642">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="6bd05-643">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="6bd05-643">9BI-00004</span></span>   |
| <span data-ttu-id="6bd05-644">Drukowanie uniwersalne (500 zadań) dla nauczycieli lub wykładowców — Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6bd05-644">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="6bd05-645">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="6bd05-645">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="6bd05-646">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="6bd05-646">9BK-00004</span></span>   |
| <span data-ttu-id="6bd05-647">Drukowanie uniwersalne woluminu (500 zadań) — System Windows</span><span class="sxs-lookup"><span data-stu-id="6bd05-647">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="6bd05-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="6bd05-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="6bd05-649">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="6bd05-649">9BI-00002</span></span>   |
| <span data-ttu-id="6bd05-650">Drukowanie uniwersalne woluminu (500 zadań) dla nauczycieli lub wykładowców — Windows</span><span class="sxs-lookup"><span data-stu-id="6bd05-650">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="6bd05-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="6bd05-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="6bd05-652">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="6bd05-652">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="6bd05-653">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="6bd05-653">Next steps</span></span>

<span data-ttu-id="6bd05-654">Zapoznaj się z cennikiem i omówieniem [Drukowanie uniwersalne .](/universal-print/fundamentals/universal-print-whatis)</span><span class="sxs-lookup"><span data-stu-id="6bd05-654">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="6bd05-655">Udostępnij te informacje wszystkim odpowiednim kontaktom w twojej organizacji.</span><span class="sxs-lookup"><span data-stu-id="6bd05-655">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6bd05-656">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="6bd05-656">Questions?</span></span>

<span data-ttu-id="6bd05-657">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bd05-657">For any questions about these offers, check your relevant Yammer communities.</span></span>
