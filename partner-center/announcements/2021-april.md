---
title: Ogłoszenia z kwietnia 2021 r.
description: Ogłoszenia dotyczące platformy Microsoft Partner Center z kwietnia 2021 r., w tym nowe możliwości, promocje, oferty, rynki lub zmiany istniejących ofert.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150135"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="eb4b9-103">Ogłoszenia z kwietnia 2021 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-103">April 2021 announcements</span></span>

<span data-ttu-id="eb4b9-104">Ta strona zawiera ogłoszenia dotyczące usługi Microsoft Partner Center na kwiecień 2021 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="eb4b9-105">Gotowość: zaktualizowany interfejs API weryfikacji adresu klienta dostawcy usług w chmurze zostanie zaktualizowany w czerwcu; Możliwość testowania jest teraz dostępna</span><span class="sxs-lookup"><span data-stu-id="eb4b9-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-106">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-106">Categories</span></span>

- <span data-ttu-id="eb4b9-107">Data: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="eb4b9-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="eb4b9-108">Gotowość</span><span class="sxs-lookup"><span data-stu-id="eb4b9-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-109">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-109">Summary</span></span>

<span data-ttu-id="eb4b9-110">Aby ułatwić partnerom i klientom prowadzenia działalności w oparciu o zaufanie, będziemy zapraszać partnerów do testowania zmian interfejsu API weryfikowania adresów dla wszystkich krajów na całym świecie.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-111">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-111">Impacted audience</span></span>

<span data-ttu-id="eb4b9-112">Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy tworzą nowe lub aktualizują szczegóły adresów istniejących klientów</span><span class="sxs-lookup"><span data-stu-id="eb4b9-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-113">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-113">Details</span></span>

<span data-ttu-id="eb4b9-114">Firma Microsoft działa w oparciu o zaufanie.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-114">Microsoft runs on trust.</span></span> <span data-ttu-id="eb4b9-115">Dążymy do zapewnienia zgodnej, bezpiecznej i bezpiecznej metody weryfikacji adresu klienta na potrzeby transakcji subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="eb4b9-116">Od 31 marca 2021 r. wprowadziliśmy zmiany w interfejsie API weryfikacji adresu.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="eb4b9-117">Zachęcamy partnerów do przetestowania interfejsu API przed rozpoczęciem jego pracy pod koniec czerwca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="eb4b9-118">Należy pamiętać, że te zmiany mają wpływ tylko na interfejs API weryfikacji adresu.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="eb4b9-119">Nie ma to wpływu na interfejsy API tworzenia klienta i aktualizowania profilu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="eb4b9-120">Chociaż sugerowany adres nie musi być obecnie używany z interfejsem API tworzenia klienta, jest to zdecydowanie zalecane.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="eb4b9-121">Odpowiedź zwróci jeden z następujących komunikatów o stanie:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="eb4b9-122">Stan</span><span class="sxs-lookup"><span data-stu-id="eb4b9-122">Status</span></span>     | <span data-ttu-id="eb4b9-123">Opis</span><span class="sxs-lookup"><span data-stu-id="eb4b9-123">Description</span></span> |    <span data-ttu-id="eb4b9-124">Liczba zwracanych sugerowanych adresów</span><span class="sxs-lookup"><span data-stu-id="eb4b9-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="eb4b9-125">Zweryfikowana wysyłka</span><span class="sxs-lookup"><span data-stu-id="eb4b9-125">Verified shippable</span></span> | <span data-ttu-id="eb4b9-126">Adres jest weryfikowany i można go wysłać.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="eb4b9-127">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-127">Single</span></span> |
|<span data-ttu-id="eb4b9-128">Sprawdzonych</span><span class="sxs-lookup"><span data-stu-id="eb4b9-128">Verified</span></span> | <span data-ttu-id="eb4b9-129">Adres jest weryfikowany.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-129">Address is verified.</span></span> | <span data-ttu-id="eb4b9-130">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-130">Single</span></span> |
|<span data-ttu-id="eb4b9-131">Wymagana interakcja</span><span class="sxs-lookup"><span data-stu-id="eb4b9-131">Interaction required</span></span> | <span data-ttu-id="eb4b9-132">Sugerowany adres został znacząco zmieniony i wymaga potwierdzenia przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="eb4b9-133">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-133">Single</span></span> |
|<span data-ttu-id="eb4b9-134">Część częściowa ulicy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-134">Street partial</span></span> | <span data-ttu-id="eb4b9-135">Podana ulica w adresie jest częściowa i wymaga więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="eb4b9-136">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="eb4b9-137">Część lokalna</span><span class="sxs-lookup"><span data-stu-id="eb4b9-137">Premises partial</span></span> | <span data-ttu-id="eb4b9-138">Dane lokalne (numer budynku, numer pakietu i inne) są częściowe i wymagają więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="eb4b9-139">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="eb4b9-140">Wiele</span><span class="sxs-lookup"><span data-stu-id="eb4b9-140">Multiple</span></span> | <span data-ttu-id="eb4b9-141">Adres zawiera wiele pól, które są częściowe (potencjalnie również częściowe ulice i część lokalna).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="eb4b9-142">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="eb4b9-143">Brak</span><span class="sxs-lookup"><span data-stu-id="eb4b9-143">None</span></span> | <span data-ttu-id="eb4b9-144">Adres jest nieprawidłowy.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-144">Address is incorrect.</span></span> | <span data-ttu-id="eb4b9-145">Brak</span><span class="sxs-lookup"><span data-stu-id="eb4b9-145">None</span></span> |
|<span data-ttu-id="eb4b9-146">Nie sprawdzono</span><span class="sxs-lookup"><span data-stu-id="eb4b9-146">Not validated</span></span> | <span data-ttu-id="eb4b9-147">Nie można wysłać adresu w procesie weryfikacji.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="eb4b9-148">Brak</span><span class="sxs-lookup"><span data-stu-id="eb4b9-148">None</span></span> |

<span data-ttu-id="eb4b9-149">Kody pocztowe w USA zwracają dodatkowe cztery cyfry + łącznik, na przykład 12345–6789.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-150">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-150">Next steps</span></span>

- <span data-ttu-id="eb4b9-151">Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="eb4b9-152">Przygotuj się do uwzględnienia zmian przy użyciu Partner Center API i internetowego interfejsu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="eb4b9-153">Udostępnij swój identyfikator dzierżawy piaskownicy ekspertowi w swoich tematach (AliKieki), który ma zostać uwzględniony w teście testowym, aby rozpocząć przygotowanie do aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="eb4b9-154">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="eb4b9-155">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-155">Questions?</span></span>

<span data-ttu-id="eb4b9-156">Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych przez firmę Microsoft, poproś o pomoc techniczną partnera w grupie usługi Yammer lub otwórz [żądanie obsługi.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="eb4b9-157">Nowa lokalizacja dokumentacji programu Swagger Partner Center API</span><span class="sxs-lookup"><span data-stu-id="eb4b9-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-158">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-158">Categories</span></span>

- <span data-ttu-id="eb4b9-159">Data: 2021-04-26</span><span class="sxs-lookup"><span data-stu-id="eb4b9-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="eb4b9-160">Możliwości</span><span class="sxs-lookup"><span data-stu-id="eb4b9-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-161">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-161">Summary</span></span>

<span data-ttu-id="eb4b9-162">Partner Center dokumentów programu Swagger interfejsu API zostały zmigrowane z poprzedniej witryny dokumentacji programu [Swagger](https://apidocs.microsoft.com/services/partnercenter) do nowej [witryny dokumentacji programu Swagger.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-163">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-163">Impacted audience</span></span>

<span data-ttu-id="eb4b9-164">Partnerzy rozliczający się bezpośrednio i dostawcy pośredni uczestniczący w programie Dostawca rozwiązań w chmurze (CSP), którzy korzystali z interfejsów API Partner Center internetowych</span><span class="sxs-lookup"><span data-stu-id="eb4b9-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-165">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-165">Details</span></span>

<span data-ttu-id="eb4b9-166">Od 26 kwietnia 2021 r. dokumentacja programu Swagger interfejsu PARTNER CENTER API, w tym zawartość interfejsu API REST, znajduje się w [nowej witrynie](/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="eb4b9-167">Stara lokacja będzie niedostępna po kilku tygodniach.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="eb4b9-168">Korzyści</span><span class="sxs-lookup"><span data-stu-id="eb4b9-168">Benefits</span></span>

<span data-ttu-id="eb4b9-169">Dokumentacja Partner Center API programu Swagger będzie zawierała funkcję **Wypróbuj.**</span><span class="sxs-lookup"><span data-stu-id="eb4b9-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="eb4b9-170">Aby użyć tej funkcji, musisz mieć token bearer, który można wygenerować, korzystając z procedury opisanej w te Partner Center [Authentication (Uwierzytelnianie).](/partner-center/develop/partner-center-authentication#app--user-authentication)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-171">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-171">Next steps</span></span>

<span data-ttu-id="eb4b9-172">Udostępnij te informacje w organizacji, aby odpowiedni zespół może przeglądać i aktualizować swoje procesy.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="eb4b9-173">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-173">Questions?</span></span>

<span data-ttu-id="eb4b9-174">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="eb4b9-175">Dostawca rozwiązań w chmurze zasady dotyczące okresu zwracania oprogramowania (CSP) i powiadomienia o wygaśnięciu linku pobierania</span><span class="sxs-lookup"><span data-stu-id="eb4b9-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-176">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-176">Categories</span></span>

- <span data-ttu-id="eb4b9-177">Data: 2021-04-21</span><span class="sxs-lookup"><span data-stu-id="eb4b9-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="eb4b9-178">Możliwości</span><span class="sxs-lookup"><span data-stu-id="eb4b9-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-179">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-179">Summary</span></span>

<span data-ttu-id="eb4b9-180">Istnieją zmiany zasad okresów zwrotu oprogramowania CSP i wygaśnięcia linku pobierania.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-181">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-181">Impacted audience</span></span>

<span data-ttu-id="eb4b9-182">Partnerzy w ramach transakcji bezterminowych ofert subskrypcji oprogramowania lub oprogramowania w programie CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-183">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-183">Details</span></span>

<span data-ttu-id="eb4b9-184">Należy pamiętać o następujących ważnych powiadomieniach dotyczących bezterminowego zakupu oprogramowania i subskrypcji oprogramowania za pośrednictwem Partner Center:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="eb4b9-185">Zasady dotyczące okresu zwrotu oprogramowania</span><span class="sxs-lookup"><span data-stu-id="eb4b9-185">Software return period policy</span></span>

<span data-ttu-id="eb4b9-186">Od 1 czerwca 2021 r. okres zwrotu dla ofert oprogramowania w programie CSP, zgodnie z Microsoft Partner Agreement (MPA), zmieni się z 60 dni od daty zamówienia do 30 dni od daty zamówienia.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="eb4b9-187">Po przesłaniu zamówienia na ofertę oprogramowania partnerzy będą mieć 30 dni od daty zamówienia, aby przesłać poprawki do takiego zamówienia:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="eb4b9-188">Każda bezterminowa licencja na oprogramowanie zwrócona w ciągu 30-dniowego okresu zwrotu otrzyma pełne środków z płatnej ceny zakupu.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="eb4b9-189">Każdy produkt subskrypcji oprogramowania zwrócony w ciągu 30-dniowego okresu zwrotu otrzyma proporcjonalną kredyt z płatnej ceny zakupu.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="eb4b9-190">Ta wiadomość jest kontynuacją naszej wiadomości e-mail wysłanej w grudniu 2020 r. i kwietniu 2021 r. do wszystkich partnerów CSP w związku z okresem zwrotu i innymi aktualizacjami mpA.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="eb4b9-191">Zapoznaj się z tymi uwagami, aby uzyskać szczegółowe informacje dotyczące zmian wpływających na owe mpA.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="eb4b9-192">Wygaśnięcie linku pobierania oprogramowania</span><span class="sxs-lookup"><span data-stu-id="eb4b9-192">Software download link expiry</span></span>

<span data-ttu-id="eb4b9-193">Od 3 czerwca 2021 r. linki do pobierania oprogramowania w przypadku bezterminowego zakupu oprogramowania i subskrypcji oprogramowania za pośrednictwem usługi Partner Center będą mieć datę wygaśnięcia 5 dni od początkowego pobrania.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="eb4b9-194">Okres wygaśnięcia będzie miał zastosowanie do wszystkich zakupów przed 3 czerwca 2021 r., a także w dniu 3 czerwca 2021 r. lub później.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-195">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-195">Next steps</span></span>

<span data-ttu-id="eb4b9-196">Przejrzyj okres [zwrotny CSP i pobierz często](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)zadawane pytania dotyczące wygaśnięcia linku i poinformuj wszystkie odpowiednie zespoły w organizacji o tych zmianach:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="eb4b9-197">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-197">Questions?</span></span>

<span data-ttu-id="eb4b9-198">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="eb4b9-199">Otwórz program licencjonowania: Przechodzenie odsprzedawców do programu Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-200">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-200">Categories</span></span>

- <span data-ttu-id="eb4b9-201">Data: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="eb4b9-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="eb4b9-202">Rozwój firmy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-203">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-203">Summary</span></span>

<span data-ttu-id="eb4b9-204">W tej komunikacji szczegółowo opisano, jak przygotować się na zmiany, które zostaną wprowadzone wkrótce w programie licencjonowania Open.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-205">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-205">Impacted audience</span></span>

<span data-ttu-id="eb4b9-206">Program CSP i partnerzy licencji Open License</span><span class="sxs-lookup"><span data-stu-id="eb4b9-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-207">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-207">Details</span></span>

<span data-ttu-id="eb4b9-208">W 2020 r. firma [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) ogłosiła, że bezterminowe licencje na oprogramowanie będą szeroko dostępne dla partnerów i klientów za pośrednictwem programu Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="eb4b9-209">Pierwszy kamień milowy został osiągnięty w styczniu 2021 r., gdy stały się dostępne komercyjne bezterminowe oferty oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="eb4b9-210">Kolejny kluczowy punkt kontrolny nastąpi w lipcu [](https://aka.ms/openlicensepublicsector) 2021 r., gdy staną się dostępne oferty sektora publicznego.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="eb4b9-211">Informujemy [](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) również pakiet Software Assurance, że od 1 stycznia 2022 r. nie będzie można kupować nowych licencji na oprogramowanie ani ich odnawianie ani Usługi online w ramach programu Licencjonowanie otwarte.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="eb4b9-212">Przejście oprogramowania bezterminowego do programu CSP w nowym środowisku handlowym pomoże partnerom rozszerzyć możliwości zaoferowania różnorodnych rozwiązań i usług zarządzanych.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="eb4b9-213">Przyspieszy to również przejście klientów do chmury.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="eb4b9-214">Aby ułatwić bezproblemowe przejście zarówno naszym partnerom, jak i klientom, dostosowaliśmy te korekty i materiały, aby przyspieszyć tę transformację cyfrową:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="eb4b9-215">Kwiecień 2021 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-215">April 2021</span></span>

<span data-ttu-id="eb4b9-216">[Teraz dostępne:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Otwórz materiały przejściowe z licencji na program CSP dla odsprzedawców</span><span class="sxs-lookup"><span data-stu-id="eb4b9-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="eb4b9-217">Lipiec 2021 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="eb4b9-218">CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-218">CSP</span></span>

- <span data-ttu-id="eb4b9-219">1 lipca: bezterminowe licencje na oprogramowanie dostępne dla klientów z sektora publicznego</span><span class="sxs-lookup"><span data-stu-id="eb4b9-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="eb4b9-220">7 lipca: Visual Studio oprogramowania Pro i Get Genuine Windows Agreement bezterminowych licencji na oprogramowanie dostępne dla wszystkich segmentów</span><span class="sxs-lookup"><span data-stu-id="eb4b9-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="eb4b9-221">Otwórz wartość</span><span class="sxs-lookup"><span data-stu-id="eb4b9-221">Open Value</span></span>

- <span data-ttu-id="eb4b9-222">1 lipca: Dodatkowe jednostki SKU dostępne w programie Open Value dla organizacji edukacyjnych i non-profit, oferując podobne oferty do programu Licencjonowanie open</span><span class="sxs-lookup"><span data-stu-id="eb4b9-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="eb4b9-223">Licencja open</span><span class="sxs-lookup"><span data-stu-id="eb4b9-223">Open License</span></span>

- <span data-ttu-id="eb4b9-224">1 lipca: Firma Microsoft nie będzie już uruchamiać nowych ofert w programie Licencjonowanie open.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="eb4b9-225">Styczeń 2022 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-225">January 2022</span></span>

- <span data-ttu-id="eb4b9-226">1 stycznia: w ramach programu licencjonowania Open License nie można dokonać żadnych nowych zakupów ani odnowień</span><span class="sxs-lookup"><span data-stu-id="eb4b9-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-227">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="eb4b9-228">Dostawcy pośredni dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-228">CSP indirect providers</span></span>

<span data-ttu-id="eb4b9-229">Skorzystaj z najbliższych miesięcy, aby pomóc odsprzedawcy licencji Open w zorientowaniu się na program CSP, udział w wydarzeniach społeczności partnerów i korzystanie z materiałów przejściowych Open License-to-CSP dla odsprzedawców:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="eb4b9-230">Otwórz materiały przejściowe [license-to-CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)dla odsprzedawców — dostosowywalna prezentacja z omówieniem, szablon wiadomości e-mail, przewodnik dołączania odsprzedawcy pośredniego w programie CSP i inne materiały, które ułatwiają wdrożenie odsprzedawców na dużą skalę.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="eb4b9-231">[Wydarzenia społeczności partnerów programu CSP hostowane](https://globalpbocomm.eventbuilder.com/GlobalCSP) przez firmę Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="eb4b9-232">Dołącz do różnych sesji, aby poznać podstawy programu CSP (CSP Fundamentals) lub być na bieżąco i zadawać pytania dotyczące oprogramowania w programie CSP (Q&A Sessions).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="eb4b9-233">(Już wkrótce) Sesja szkoleniowa ukierunkowana na odsprzedawcę pośredniego w programie CSP hostowana przez firmę Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="eb4b9-234">Odsprzedawcy licencji open</span><span class="sxs-lookup"><span data-stu-id="eb4b9-234">Open License resellers</span></span>

- <span data-ttu-id="eb4b9-235">Jeśli Twoja organizacja nie jest obecnie zarejestrowane w programie CSP, skontaktuj się z dystrybutorem, aby uzyskać informacje na temat rozpoczynania pracy.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="eb4b9-236">W tym miejscu połącz się z dostawcą [pośrednim.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="eb4b9-237">Jeśli Twoja organizacja jest już zarejestrowane w programie CSP, dowiedz się więcej na temat oprogramowania bezterminowego w programie CSP [tutaj.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="eb4b9-238">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-238">Questions?</span></span>

<span data-ttu-id="eb4b9-239">Aby uzyskać więcej pytań dotyczących tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="eb4b9-240">Teraz na żywo: Przewodnik dotyczący gotowości na globalną promocję</span><span class="sxs-lookup"><span data-stu-id="eb4b9-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-241">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-241">Categories</span></span>

- <span data-ttu-id="eb4b9-242">Data: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="eb4b9-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="eb4b9-243">Możliwości</span><span class="sxs-lookup"><span data-stu-id="eb4b9-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-244">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-244">Summary</span></span>

<span data-ttu-id="eb4b9-245">Launch Readiness has published a [new global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) (Gotowość do uruchomienia) opublikowano nowy przewodnik dotyczący gotowości na poziomie globalnym w galerii zasobów Operations Readiness.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="eb4b9-246">Ten przewodnik zawiera skonsolidowany widok wszystkich aktywnych promocji [globalnych.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-247">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-247">Impacted audience</span></span>

<span data-ttu-id="eb4b9-248">Wszyscy partnerzy licencjonowania zbiorowego (VL), dynamics price list (DPL) i Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-249">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-249">Details</span></span>

<span data-ttu-id="eb4b9-250">Partnerzy firmy Microsoft udostępnili nam potrzebę zapewnienia skonsolidowanego widoku wszystkich globalnych promocji ze szczegółami obsługi.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="eb4b9-251">Chcesz, aby ten skonsolidowany przewodnik ułatwiał korzystanie z promocji z przekonaniem, że wszystkie dostępne informacje będą łatwo dostępne w centralnej i wygodnej lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="eb4b9-252">Począwszy od kwietnia 2021 r., firma Microsoft będzie aktualizować ten przewodnik co miesiąc i będzie on dostępny w dedykowanej kolekcji Przewodnika po globalnej gotowości dotyczącej promocji w galerii zasobów Gotowość na operacje.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="eb4b9-253">Linki do tego przewodnika będą również zawarte w następujących kolekcjach:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="eb4b9-254">[Uruchom kolekcję kalendarza](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), która zapewnia scentralizowany widok przyszłych zmian i uruchomień.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="eb4b9-255">[Kolekcje społeczności](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), które zawierają materiały szkoleniowe dla naszych comiesięcznych rozmów z partnerami, z wyróżnieniem nadchodzących zmian i terminowych tematów zainteresowań operacyjnych.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="eb4b9-256">[Biuletyny partnerów,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)takie jak comiesięczne aktualizacje programu CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="eb4b9-257">Jako comiesięczne przypomnienie opublikujemy również Partner Center z każdym nowym problemem przewodnika po globalnej gotowości na promocję.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-258">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-258">Next steps</span></span>

<span data-ttu-id="eb4b9-259">Na początku każdego miesiąca w galerii [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) zasobów Operations Readiness znajdziesz najnowszy globalny przewodnik dotyczący gotowości [na promocję.](https://partner.microsoft.com/resources)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="eb4b9-260">Udostępnij te informacje odpowiednim kontaktom w organizacjach i daj nam znać, jak pomocny jest przewodnik za pośrednictwem strony "Czy ta strona była pomocna?".</span><span class="sxs-lookup"><span data-stu-id="eb4b9-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="eb4b9-261">na końcu każdej strony.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="eb4b9-262">Aktualizacja społeczności Dostawca rozwiązań w chmurze (CSP) z kwietnia</span><span class="sxs-lookup"><span data-stu-id="eb4b9-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-263">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-263">Categories</span></span>

- <span data-ttu-id="eb4b9-264">Data: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="eb4b9-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="eb4b9-265">Społeczność | Zaproszenia i przypomnienia</span><span class="sxs-lookup"><span data-stu-id="eb4b9-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-266">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-266">Summary</span></span>

<span data-ttu-id="eb4b9-267">Zasoby społeczności programu CSP są dostępne na żądanie i aktualizowane co miesiąc, aby być na bieżąco z aktualnymi i przygotowanymi do zmian w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-268">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-268">Impacted audience</span></span>

<span data-ttu-id="eb4b9-269">Partnerzy rozliczani bezpośrednio i dostawcy pośredni dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-270">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-270">Details</span></span>

<span data-ttu-id="eb4b9-271">W tym miesiącu zasoby obejmują następujące kluczowe tematy:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="eb4b9-272">Aktualizacja ewolucji programu CSP i zmiany programu licencjonowania Open License</span><span class="sxs-lookup"><span data-stu-id="eb4b9-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="eb4b9-273">Zmiany wymagań dotyczących dołączania klientów w programie CSP w niektórych regionach</span><span class="sxs-lookup"><span data-stu-id="eb4b9-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="eb4b9-274">Nowy format nowej faktury w formacie PDF dla handlu w programie CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="eb4b9-275">W [kolekcji społeczności CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)znajdziesz:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="eb4b9-276">Biuletyn comiesięcznej aktualizacji programu [CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)do pobrania, który agreguje najnowsze ogłoszenia, aktualizacje, zdarzenia i przypomnienia dotyczące programu CSP w czytelnym dokumencie.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="eb4b9-277">Kalendarz [anonsów programu CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)który zapewnia widok osi czasu przyszłych zmian wpływających na program.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="eb4b9-278">Nowy kalendarz [uruchamiania produktu](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), w którym można wyświetlić nadchodzące premiery i oferty produktów.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="eb4b9-279">[Program CSP uruchamia zasoby aktualizacji z](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) łatwą w użyciu zawartością dla kluczowych zmian operacyjnych.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="eb4b9-280">[Odświeżenia i przypomnienia dotyczące kluczowych](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) tematów dotyczących CSP, które otrzymują zainteresowanie i zapytania.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="eb4b9-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="eb4b9-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="eb4b9-282">Community Call Q&As are available to help you with questions related to upcoming changes .</span><span class="sxs-lookup"><span data-stu-id="eb4b9-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="eb4b9-283">Zarejestruj się teraz, aby rejestrować się w csp community call Q <1> <3> As that are place in April, May, and June (Zarejestruj się teraz w CSP Community Call Q&amp;Ponieważ odbywa się to w kwietniu, maju i czerwcu.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="eb4b9-284">Skupią się one na najnowszych startach, ważnych odświeżeniach i przypomnieniach.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="eb4b9-285">[Zarejestruj się tutaj.](https://globalpbocomm.eventbuilder.com/GlobalCSP)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-286">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-286">Next steps</span></span>

<span data-ttu-id="eb4b9-287">Zapoznaj się z zasobami społeczności i zarejestruj się w rozmowę społeczności z&A.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="eb4b9-288">Aby upewnić się, że otrzymasz jak najwięcej informacji z forum community Call Q&A, przejrzyj zawartość społeczności na żądanie i prześlij swoje pytania do 48 godzin przed wywołaniem.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="eb4b9-289">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-289">Questions?</span></span>

<span data-ttu-id="eb4b9-290">Comiesięczne zaproszenie społeczności CSP&A to najlepsze miejsce na pytania związane ze zmianami w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="eb4b9-291">W każdym miesiącu zapoznaj się z materiałami i prześlij pytania z wyprzedzeniem, abyśmy spędzali sesję na najważniejszych tematach.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="eb4b9-292">Aby uzyskać więcej informacji, skontaktuj się z [pomocą techniczną.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="eb4b9-293">Ostatnie przypomnienie: 6 maja 2021 r. oznaczało to, że kwalifikacja GET jest już wyefiniowana</span><span class="sxs-lookup"><span data-stu-id="eb4b9-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-294">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-294">Categories</span></span>

- <span data-ttu-id="eb4b9-295">Data: 2021-05-04</span><span class="sxs-lookup"><span data-stu-id="eb4b9-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="eb4b9-296">Możliwości</span><span class="sxs-lookup"><span data-stu-id="eb4b9-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-297">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-297">Impacted audience</span></span>

<span data-ttu-id="eb4b9-298">Partnerzy sprzedają oferty Academic, Nonprofit i Government Community Cloud (GCC) za pośrednictwem programu Dostawca rozwiązań w chmurze przy użyciu interfejsu API Partner Center api</span><span class="sxs-lookup"><span data-stu-id="eb4b9-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-299">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-299">Details</span></span>

<span data-ttu-id="eb4b9-300">To zawiadomienie jest kontynuacją rozszerzenia usługi Partner Center [wydanego w grudniu.](./2020-december.md#1)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-300">This announcement is a follow-up to the Partner Center [enhancements released in December](./2020-december.md#1).</span></span> <span data-ttu-id="eb4b9-301">W ramach tej wersji zostały wdrożone nowe interfejsy API kwalifikacji GET i POST, w związku z tym istniejąca kwalifikacja GET zostanie wycofana 6 maja **2021 r.**</span><span class="sxs-lookup"><span data-stu-id="eb4b9-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="eb4b9-302">W tym czasie konieczne będzie przejście do korzystania z nowych interfejsów API Partner Center POST.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="eb4b9-303">Nowe interfejsy API POST umożliwią zakup ofert edukacyjnych, a nowe interfejsy API GET umożliwią zakup wstępnie kwalifikowanych ofert organizacji nonprofit i GCC.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-304">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-304">Next steps</span></span>

- <span data-ttu-id="eb4b9-305">**Zaktualizuj do nowych interfejsów API w** celu pomyślnego i terminowego przejścia.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="eb4b9-306">**Zapoznaj się z nowymi zmianami Partner Center API** i przewodnikiem w zasobach gotowość do operacji: [rozszerzenia procesu weryfikacji](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)klienta Partner Center Education.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="eb4b9-307">Udostępnij te informacje odpowiednim zespołom w organizacji oraz odsprzedawcom, aby pomóc im przygotować się do tych zmian.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="eb4b9-308">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-308">Questions?</span></span>

<span data-ttu-id="eb4b9-309">W przypadku jakichkolwiek pytań związanych z tym powiadomieniem skontaktuj się z [Partner Center pomocą techniczną.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="eb4b9-310">Dziennik zmian</span><span class="sxs-lookup"><span data-stu-id="eb4b9-310">Change log</span></span>

- <span data-ttu-id="eb4b9-311">4 maja 2021 r.: Ostateczne przypomnienie o zbliżającym się cofaniu kwalifikacji GET</span><span class="sxs-lookup"><span data-stu-id="eb4b9-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="eb4b9-312">9 kwietnia 2021 r.: Przypomnienie o zbliżającym się cofaniu kwalifikacji GET</span><span class="sxs-lookup"><span data-stu-id="eb4b9-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="eb4b9-313">Luty: zaktualizowane osie czasu dotyczące cofania pracy z kwalifikacjami GET & PUT</span><span class="sxs-lookup"><span data-stu-id="eb4b9-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="eb4b9-314">Styczeń: Przypomnienie o zbliżających się cofaniach pracy z kwalifikacjami GET & PUT</span><span class="sxs-lookup"><span data-stu-id="eb4b9-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="eb4b9-315">Nowy format nowej faktury w formacie PDF dla handlu w programie CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-316">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-316">Categories</span></span>

- <span data-ttu-id="eb4b9-317">Data: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="eb4b9-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="eb4b9-318">Możliwości</span><span class="sxs-lookup"><span data-stu-id="eb4b9-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-319">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-319">Summary</span></span>

<span data-ttu-id="eb4b9-320">Firma Microsoft wprowadza nowy format nowej faktury w formacie PDF dla handlu w programie Dostawca rozwiązań w chmurze (CSP) w celu wyświetlania szczegółów rozliczeń według szczegółów produktu zamiast opisu sku.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-321">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-321">Impacted audience</span></span>

<span data-ttu-id="eb4b9-322">Partnerzy inicjujące transakcje za pośrednictwem programu CSP</span><span class="sxs-lookup"><span data-stu-id="eb4b9-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-323">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-323">Details</span></span>

<span data-ttu-id="eb4b9-324">Od maja 2021 r. firma Microsoft wprowadza nowy format nowej faktury w formacie PDF dla handlu w programie CSP w celu wyświetlania szczegółów rozliczeń według szczegółów produktu zamiast opisu sku.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="eb4b9-325">Dzięki tej nowej aktualizacji będziemy agregować elementy wiersza według typu produktu, jednocześnie wyświetlając każdy produkt w poszczególnych wierszach.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="eb4b9-326">Partnerzy zauważą, że ta zmiana wchodzi w życie na fakturze za maj dla okresu rozliczeniowego od 1 kwietnia 2021 r. do 30 kwietnia 2021 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="eb4b9-327">Oferty, których dotyczy problem, Microsoft Azure wystąpienie zarezerwowane, subskrypcje platformy Azure (plan platformy Azure) i Marketplace.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="eb4b9-328">Wszystkie żądania środków po zaktualizowaniu formatu faktury zostaną wygenerowane w nowym formacie.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="eb4b9-329">Korzyści dla partnerów</span><span class="sxs-lookup"><span data-stu-id="eb4b9-329">Partner benefits</span></span>

<span data-ttu-id="eb4b9-330">Ta aktualizacja oferuje następujące ulepszenia w zakresie fakturowania dla partnerów:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="eb4b9-331">Zmniejszenie rozmiaru faktury przy zachowaniu danych krytycznych</span><span class="sxs-lookup"><span data-stu-id="eb4b9-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="eb4b9-332">Dopasowanie formatu do standardów branżowych w przypadku faktur kompaktowych i przyjaznych dla użytkownika</span><span class="sxs-lookup"><span data-stu-id="eb4b9-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="eb4b9-333">Nie będzie to mieć wpływu na następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="eb4b9-334">Strona podsumowania rozliczeń w pliku PDF faktury</span><span class="sxs-lookup"><span data-stu-id="eb4b9-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="eb4b9-335">Istniejące interfejsy API fakturowania</span><span class="sxs-lookup"><span data-stu-id="eb4b9-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="eb4b9-336">Pliki uzgodnień (pliki rekonescji mogą służyć do pobierania szczegółowych danych).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="eb4b9-337">Faktury za użycie i opłaty na podstawie licencji</span><span class="sxs-lookup"><span data-stu-id="eb4b9-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-338">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-338">Next steps</span></span>

<span data-ttu-id="eb4b9-339">Zapoznaj się z informacjami na ten temat w [galerii zasobów Operations Readiness](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) w witrynie internetowej partnerów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="eb4b9-340">Aby uzyskać więcej informacji na temat rozliczeń i podatków, w tym zasobów rozliczeniowych, faktur, rozliczeń CSP i podatków, odwiedź sekcję Rozliczenia [w](../billing.md) Partner Center.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](../billing.md) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="eb4b9-341">Zmiany wymagań Dostawca rozwiązań w chmurze (CSP) dotyczące dołączania klientów</span><span class="sxs-lookup"><span data-stu-id="eb4b9-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-342">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-342">Categories</span></span>

- <span data-ttu-id="eb4b9-343">Data: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="eb4b9-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="eb4b9-344">Oferty/rynki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="eb4b9-345">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-345">Summary</span></span>

<span data-ttu-id="eb4b9-346">W ramach naszego zobowiązania do pomocy partnerom i klientom w perspektywie zaufania poprosimy o dodatkowe informacje o klientach od 25 marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-347">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-347">Impacted audience</span></span>

<span data-ttu-id="eb4b9-348">Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy mają nowych lub istniejących klientów w krajach wymienionych w następnej sekcji</span><span class="sxs-lookup"><span data-stu-id="eb4b9-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-349">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-349">Details</span></span>

<span data-ttu-id="eb4b9-350">Firma Microsoft działa w oparciu o zaufanie.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-350">Microsoft runs on trust.</span></span> <span data-ttu-id="eb4b9-351">Dokładamy starań, aby zapewnić zgodną, bezpieczną i bezpieczną metodę weryfikacji klienta na potrzeby transakcji subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="eb4b9-352">25 marca 2021 r. wprowadzimy ulepszenia interfejsu API i interfejsu użytkownika usługi Partner Center, które będą mieć wpływ na partnerów spełniających oba następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="eb4b9-353">Partner ma bezpośrednią relację rozliczeń z firmą Microsoft (co oznacza, że partner jest partnerem z rozliczaniem bezpośrednim lub dostawcą pośrednim).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="eb4b9-354">Partner współpracuje z nowymi lub istniejącymi klientami w następujących krajach:</span><span class="sxs-lookup"><span data-stu-id="eb4b9-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="eb4b9-355">Tajlandia</span><span class="sxs-lookup"><span data-stu-id="eb4b9-355">Thailand</span></span>
    - <span data-ttu-id="eb4b9-356">Wietnam</span><span class="sxs-lookup"><span data-stu-id="eb4b9-356">Vietnam</span></span>
    - <span data-ttu-id="eb4b9-357">Turcja</span><span class="sxs-lookup"><span data-stu-id="eb4b9-357">Turkey</span></span>
    - <span data-ttu-id="eb4b9-358">Polska</span><span class="sxs-lookup"><span data-stu-id="eb4b9-358">Poland</span></span>
    - <span data-ttu-id="eb4b9-359">Republika Południowej Afryki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-359">South Africa</span></span>
    - <span data-ttu-id="eb4b9-360">Indie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-360">India</span></span>
    - <span data-ttu-id="eb4b9-361">Brazylia</span><span class="sxs-lookup"><span data-stu-id="eb4b9-361">Brazil</span></span>
    - <span data-ttu-id="eb4b9-362">Irak</span><span class="sxs-lookup"><span data-stu-id="eb4b9-362">Iraq</span></span>
    - <span data-ttu-id="eb4b9-363">Myanmar</span><span class="sxs-lookup"><span data-stu-id="eb4b9-363">Myanmar</span></span>
    - <span data-ttu-id="eb4b9-364">Sudan Południowy</span><span class="sxs-lookup"><span data-stu-id="eb4b9-364">South Sudan</span></span>
    - <span data-ttu-id="eb4b9-365">Arabia Saudyjska</span><span class="sxs-lookup"><span data-stu-id="eb4b9-365">Saudi Arabia</span></span>
    - <span data-ttu-id="eb4b9-366">Zjednoczone Emiraty Arabskie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-366">United Arab Emirates</span></span>
    - <span data-ttu-id="eb4b9-367">Wenezuela</span><span class="sxs-lookup"><span data-stu-id="eb4b9-367">Venezuela</span></span>

<span data-ttu-id="eb4b9-368">Partnerzy spełniający te kryteria muszą przesłać identyfikator rejestracji firmy klienta (znany również jako organizacja klienta ), oraz numer telefonu podczas następnej aktualizacji lub utworzenia subskrypcji dla tego klienta.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="eb4b9-369">Ci partnerzy mogą również wprowadzić opcjonalne drugie imię klienta.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="eb4b9-370">Pamiętaj, że podczas dodawania identyfikatora rejestracji firmy należy użyć identyfikatora podatku od działalności biznesowej, a nie identyfikatora osobistego klienta.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="eb4b9-371">Partnerzy, którzy współpracuje z nowymi lub istniejącymi klientami w następujących krajach, są już dołączani do poprzedniej wersji w listopadzie 2020 r.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="eb4b9-372">Armenia</span><span class="sxs-lookup"><span data-stu-id="eb4b9-372">Armenia</span></span>
- <span data-ttu-id="eb4b9-373">Azerbejdżan</span><span class="sxs-lookup"><span data-stu-id="eb4b9-373">Azerbaijan</span></span>
- <span data-ttu-id="eb4b9-374">Białoruś</span><span class="sxs-lookup"><span data-stu-id="eb4b9-374">Belarus</span></span>
- <span data-ttu-id="eb4b9-375">Węgry</span><span class="sxs-lookup"><span data-stu-id="eb4b9-375">Hungary</span></span>
- <span data-ttu-id="eb4b9-376">Kazachstan</span><span class="sxs-lookup"><span data-stu-id="eb4b9-376">Kazakhstan</span></span>
- <span data-ttu-id="eb4b9-377">Kirgistan</span><span class="sxs-lookup"><span data-stu-id="eb4b9-377">Kyrgyzstan</span></span>
- <span data-ttu-id="eb4b9-378">Mołdawia</span><span class="sxs-lookup"><span data-stu-id="eb4b9-378">Moldova</span></span>
- <span data-ttu-id="eb4b9-379">Rosja</span><span class="sxs-lookup"><span data-stu-id="eb4b9-379">Russia</span></span>
- <span data-ttu-id="eb4b9-380">Tadżykistan</span><span class="sxs-lookup"><span data-stu-id="eb4b9-380">Tajikistan</span></span>
- <span data-ttu-id="eb4b9-381">Ukraina</span><span class="sxs-lookup"><span data-stu-id="eb4b9-381">Ukraine</span></span>
- <span data-ttu-id="eb4b9-382">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="eb4b9-382">Uzbekistan</span></span>

<span data-ttu-id="eb4b9-383">Pod koniec marca 2021 r. partnerzy z klientami na całym świecie będą mieć możliwość wprowadzenia identyfikatora rejestracji firmy, numeru telefonu i środkowej nazwy klienta jako opcjonalnych szczegółów.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-384">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-384">Next steps</span></span>

- <span data-ttu-id="eb4b9-385">Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="eb4b9-386">Przygotuj się do uwzględnienia zmian przy użyciu Partner Center API i internetowego interfejsu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="eb4b9-387">Zestawy API/zestawy SDK będą dostępne do testowania.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="eb4b9-388">Pamiętaj, aby przesłać dodatkowe dane podczas dołączania nowych klientów lub modyfikowania istniejących danych klienta.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="eb4b9-389">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="eb4b9-390">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-390">Questions?</span></span>

<span data-ttu-id="eb4b9-391">Skontaktuj się z doradcą podatkowym lub lokalnym urzędem podatkowym, jeśli masz pytania związane z identyfikatorem rejestracji firmy (nazywanym również URZĘDEM PODATKOWYM lub NIP).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="eb4b9-392">Firma Microsoft nie może zapewnić wskazówek dotyczących kwestii podatkowych.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="eb4b9-393">Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych w firmie Microsoft, otwórz [żądanie obsługi](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="eb4b9-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="eb4b9-394">Wyświetlanie ofert i uruchomień produktów w tym miesiącu</span><span class="sxs-lookup"><span data-stu-id="eb4b9-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="eb4b9-395">Kategorie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-395">Categories</span></span>

- <span data-ttu-id="eb4b9-396">Data: 2021-04-01</span><span class="sxs-lookup"><span data-stu-id="eb4b9-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="eb4b9-397">Możliwości</span><span class="sxs-lookup"><span data-stu-id="eb4b9-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="eb4b9-398">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="eb4b9-398">Summary</span></span>

<span data-ttu-id="eb4b9-399">Kalendarz produktów z kwietnia 2021 r. został opublikowany.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="eb4b9-400">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="eb4b9-400">Impacted audience</span></span>

<span data-ttu-id="eb4b9-401">Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="eb4b9-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="eb4b9-402">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="eb4b9-402">Details</span></span>

<span data-ttu-id="eb4b9-403">Kalendarz uruchamiania produktów z [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) kwietnia 2021 r. jest teraz dostępny w galerii zasobów Gotowość na operacje.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="eb4b9-404">Zobacz nadchodzące premiery i oferty produktów tutaj.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="eb4b9-405">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eb4b9-405">Next steps</span></span>

<span data-ttu-id="eb4b9-406">Przejrzyj kalendarz [uruchamiania produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)i udostępnij informacje odpowiednim uczestnikom projektu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="eb4b9-407">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="eb4b9-407">Questions?</span></span>

<span data-ttu-id="eb4b9-408">Jeśli masz dodatkowe pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="eb4b9-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>