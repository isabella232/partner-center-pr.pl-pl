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
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702828"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="cac9d-103">Ogłoszenia z kwietnia 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-103">April 2021 announcements</span></span>

<span data-ttu-id="cac9d-104">Ta strona zawiera ogłoszenia dotyczące usługi Microsoft Partner Center na kwiecień 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="cac9d-105">Gotowość: zaktualizowany interfejs API weryfikacji adresu klienta dostawcy usług w chmurze zostanie zaktualizowany w czerwcu; Możliwość testowania jest teraz dostępna</span><span class="sxs-lookup"><span data-stu-id="cac9d-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-106">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-106">Categories</span></span>

- <span data-ttu-id="cac9d-107">Data: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="cac9d-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="cac9d-108">Gotowość</span><span class="sxs-lookup"><span data-stu-id="cac9d-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-109">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-109">Summary</span></span>

<span data-ttu-id="cac9d-110">Aby ułatwić partnerom i klientom prowadzenia działalności w oparciu o zaufanie, będziemy zapraszać partnerów do testowania zmian interfejsu API weryfikowania adresów dla wszystkich krajów na całym świecie.</span><span class="sxs-lookup"><span data-stu-id="cac9d-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-111">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-111">Impacted audience</span></span>

<span data-ttu-id="cac9d-112">Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy tworzą nowe lub aktualizują szczegóły adresów istniejących klientów</span><span class="sxs-lookup"><span data-stu-id="cac9d-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-113">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-113">Details</span></span>

<span data-ttu-id="cac9d-114">Firma Microsoft działa w oparciu o zaufanie.</span><span class="sxs-lookup"><span data-stu-id="cac9d-114">Microsoft runs on trust.</span></span> <span data-ttu-id="cac9d-115">Dążymy do zapewnienia zgodnej, bezpiecznej i bezpiecznej metody weryfikacji adresu klienta na potrzeby transakcji subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="cac9d-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="cac9d-116">Od 31 marca 2021 r. wprowadziliśmy zmiany w interfejsie API weryfikacji adresu.</span><span class="sxs-lookup"><span data-stu-id="cac9d-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="cac9d-117">Zachęcamy partnerów do przetestowania interfejsu API przed rozpoczęciem jego pracy pod koniec czerwca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="cac9d-118">Należy pamiętać, że te zmiany mają wpływ tylko na interfejs API weryfikacji adresu.</span><span class="sxs-lookup"><span data-stu-id="cac9d-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="cac9d-119">Nie ma to wpływu na interfejsy API tworzenia klienta i aktualizowania profilu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="cac9d-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="cac9d-120">Chociaż sugerowany adres nie musi być obecnie używany z interfejsem API tworzenia klienta, jest to zdecydowanie zalecane.</span><span class="sxs-lookup"><span data-stu-id="cac9d-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="cac9d-121">Odpowiedź zwróci jeden z następujących komunikatów o stanie:</span><span class="sxs-lookup"><span data-stu-id="cac9d-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="cac9d-122">Stan</span><span class="sxs-lookup"><span data-stu-id="cac9d-122">Status</span></span>     | <span data-ttu-id="cac9d-123">Opis</span><span class="sxs-lookup"><span data-stu-id="cac9d-123">Description</span></span> |    <span data-ttu-id="cac9d-124">Liczba zwracanych sugerowanych adresów</span><span class="sxs-lookup"><span data-stu-id="cac9d-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="cac9d-125">Zweryfikowana wysyłka</span><span class="sxs-lookup"><span data-stu-id="cac9d-125">Verified shippable</span></span> | <span data-ttu-id="cac9d-126">Adres jest weryfikowany i można go wysłać.</span><span class="sxs-lookup"><span data-stu-id="cac9d-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="cac9d-127">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="cac9d-127">Single</span></span> |
|<span data-ttu-id="cac9d-128">Sprawdzonych</span><span class="sxs-lookup"><span data-stu-id="cac9d-128">Verified</span></span> | <span data-ttu-id="cac9d-129">Adres jest weryfikowany.</span><span class="sxs-lookup"><span data-stu-id="cac9d-129">Address is verified.</span></span> | <span data-ttu-id="cac9d-130">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="cac9d-130">Single</span></span> |
|<span data-ttu-id="cac9d-131">Wymagana interakcja</span><span class="sxs-lookup"><span data-stu-id="cac9d-131">Interaction required</span></span> | <span data-ttu-id="cac9d-132">Sugerowany adres został znacząco zmieniony i wymaga potwierdzenia przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="cac9d-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="cac9d-133">Pojedynczy</span><span class="sxs-lookup"><span data-stu-id="cac9d-133">Single</span></span> |
|<span data-ttu-id="cac9d-134">Część częściowa ulicy</span><span class="sxs-lookup"><span data-stu-id="cac9d-134">Street partial</span></span> | <span data-ttu-id="cac9d-135">Podana ulica w adresie jest częściowa i wymaga więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="cac9d-136">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="cac9d-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="cac9d-137">Część lokalna</span><span class="sxs-lookup"><span data-stu-id="cac9d-137">Premises partial</span></span> | <span data-ttu-id="cac9d-138">Dane lokalne (numer budynku, numer pakietu i inne) są częściowe i wymagają więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="cac9d-139">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="cac9d-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="cac9d-140">Wiele</span><span class="sxs-lookup"><span data-stu-id="cac9d-140">Multiple</span></span> | <span data-ttu-id="cac9d-141">Adres zawiera wiele pól, które są częściowe (potencjalnie również częściowe ulice i część lokalna).</span><span class="sxs-lookup"><span data-stu-id="cac9d-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="cac9d-142">Wiele — maksymalnie trzy</span><span class="sxs-lookup"><span data-stu-id="cac9d-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="cac9d-143">Brak</span><span class="sxs-lookup"><span data-stu-id="cac9d-143">None</span></span> | <span data-ttu-id="cac9d-144">Adres jest nieprawidłowy.</span><span class="sxs-lookup"><span data-stu-id="cac9d-144">Address is incorrect.</span></span> | <span data-ttu-id="cac9d-145">Brak</span><span class="sxs-lookup"><span data-stu-id="cac9d-145">None</span></span> |
|<span data-ttu-id="cac9d-146">Nie sprawdzono</span><span class="sxs-lookup"><span data-stu-id="cac9d-146">Not validated</span></span> | <span data-ttu-id="cac9d-147">Nie można wysłać adresu w procesie weryfikacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="cac9d-148">Brak</span><span class="sxs-lookup"><span data-stu-id="cac9d-148">None</span></span> |

<span data-ttu-id="cac9d-149">Kody pocztowe w USA zwracają dodatkowe cztery cyfry + łącznik, na przykład 12345–6789.</span><span class="sxs-lookup"><span data-stu-id="cac9d-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-150">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-150">Next steps</span></span>

- <span data-ttu-id="cac9d-151">Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.</span><span class="sxs-lookup"><span data-stu-id="cac9d-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="cac9d-152">Przygotuj się do uwzględnienia zmian przy użyciu Partner Center API i internetowego interfejsu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="cac9d-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="cac9d-153">Udostępnij swój identyfikator dzierżawy piaskownicy ekspertowi w swoich tematach (AliKieki), który zostanie uwzględniony w teście testowym, aby można było rozpocząć przygotowanie do aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="cac9d-154">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.</span><span class="sxs-lookup"><span data-stu-id="cac9d-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="cac9d-155">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-155">Questions?</span></span>

<span data-ttu-id="cac9d-156">Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych przez firmę Microsoft, uzyskaj pomoc techniczną dla swojego partnera w grupie usługi Yammer lub otwórz [żądanie obsługi](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="cac9d-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="cac9d-157">Nowa lokalizacja dokumentacji programu Swagger Partner Center API</span><span class="sxs-lookup"><span data-stu-id="cac9d-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-158">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-158">Categories</span></span>

- <span data-ttu-id="cac9d-159">Data: 2021-04-26</span><span class="sxs-lookup"><span data-stu-id="cac9d-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="cac9d-160">Możliwości</span><span class="sxs-lookup"><span data-stu-id="cac9d-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-161">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-161">Summary</span></span>

<span data-ttu-id="cac9d-162">Partner Center api Swagger zostały zmigrowane z poprzedniej witryny dokumentacji programu [Swagger](https://apidocs.microsoft.com/services/partnercenter) do nowej [witryny dokumentacji programu Swagger.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="cac9d-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-163">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-163">Impacted audience</span></span>

<span data-ttu-id="cac9d-164">Partnerzy rozliczający się bezpośrednio i dostawcy pośredni uczestniczący w programie Dostawca rozwiązań w chmurze (CSP), którzy korzystali z interfejsów API Partner Center internetowych</span><span class="sxs-lookup"><span data-stu-id="cac9d-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-165">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-165">Details</span></span>

<span data-ttu-id="cac9d-166">Od 26 kwietnia 2021 r. dokumentacja programu Swagger interfejsu API Partner Center, w tym zawartość interfejsu API REST, znajduje się w [nowej witrynie.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="cac9d-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="cac9d-167">Stara witryna będzie niedostępna po kilku tygodniach.</span><span class="sxs-lookup"><span data-stu-id="cac9d-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="cac9d-168">Korzyści</span><span class="sxs-lookup"><span data-stu-id="cac9d-168">Benefits</span></span>

<span data-ttu-id="cac9d-169">Dokumentacja Partner Center API Swagger będzie zawierała funkcję **Wypróbuj.**</span><span class="sxs-lookup"><span data-stu-id="cac9d-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="cac9d-170">Aby użyć tej funkcji, musisz mieć token bearer, który można wygenerować, korzystając z kroków wymienionych w te [Partner Center Authentication (Uwierzytelnianie).](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)</span><span class="sxs-lookup"><span data-stu-id="cac9d-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-171">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-171">Next steps</span></span>

<span data-ttu-id="cac9d-172">Udostępnij te informacje w organizacji, aby odpowiedni zespół może przeglądać i aktualizować swoje procesy.</span><span class="sxs-lookup"><span data-stu-id="cac9d-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="cac9d-173">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-173">Questions?</span></span>

<span data-ttu-id="cac9d-174">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="cac9d-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="cac9d-175">Dostawca rozwiązań w chmurze (CSP) okresu zwrotu oprogramowania i powiadomienia o wygaśnięciu linku pobierania</span><span class="sxs-lookup"><span data-stu-id="cac9d-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-176">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-176">Categories</span></span>

- <span data-ttu-id="cac9d-177">Data: 2021-04-21</span><span class="sxs-lookup"><span data-stu-id="cac9d-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="cac9d-178">Możliwości</span><span class="sxs-lookup"><span data-stu-id="cac9d-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-179">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-179">Summary</span></span>

<span data-ttu-id="cac9d-180">W zasadach okresów powrotu oprogramowania CSP i wygaśnięcia linku pobierania w programie CSP wejdą zmiany.</span><span class="sxs-lookup"><span data-stu-id="cac9d-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-181">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-181">Impacted audience</span></span>

<span data-ttu-id="cac9d-182">Partnerzy w ramach transakcji bezterminowych ofert subskrypcji oprogramowania lub oprogramowania w programie CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-183">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-183">Details</span></span>

<span data-ttu-id="cac9d-184">Należy pamiętać o następujących ważnych powiadomieniach dotyczących bezterminowych zakupów oprogramowania i subskrypcji oprogramowania za pośrednictwem Partner Center:</span><span class="sxs-lookup"><span data-stu-id="cac9d-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="cac9d-185">Zasady okresu zwrotu oprogramowania</span><span class="sxs-lookup"><span data-stu-id="cac9d-185">Software return period policy</span></span>

<span data-ttu-id="cac9d-186">Od 1 czerwca 2021 r. okres zwrotu dla ofert oprogramowania w programie CSP, zgodnie z Microsoft Partner Agreement (MPA), zmieni się z 60 dni od daty zamówienia do 30 dni od daty zamówienia.</span><span class="sxs-lookup"><span data-stu-id="cac9d-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="cac9d-187">Po przesłaniu zamówienia na ofertę oprogramowania partnerzy będą mieć 30 dni od daty zamówienia, aby przesłać poprawki do takiego zamówienia:</span><span class="sxs-lookup"><span data-stu-id="cac9d-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="cac9d-188">Każda bezterminowa licencja na oprogramowanie zwrócona w ciągu 30-dniowego okresu zwrotu otrzyma pełne środków z płatnej ceny zakupu.</span><span class="sxs-lookup"><span data-stu-id="cac9d-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="cac9d-189">Każdy produkt subskrypcji oprogramowania zwrócony w 30-dniowym okresie zwrotu otrzyma proporcjonalną kredyt z płatnej ceny zakupu.</span><span class="sxs-lookup"><span data-stu-id="cac9d-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="cac9d-190">Ta wiadomość jest kontynuacją wiadomości e-mail wysłanych w grudniu 2020 r. i kwietniu 2021 r. do wszystkich partnerów programu CSP w związku z okresem zwrotu i innymi aktualizacjami do mpA.</span><span class="sxs-lookup"><span data-stu-id="cac9d-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="cac9d-191">Zapoznaj się z tymi uwagami, aby uzyskać szczegółowe informacje dotyczące zmian wpływających na owa owa zmianami.</span><span class="sxs-lookup"><span data-stu-id="cac9d-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="cac9d-192">Wygaśnięcie linku pobierania oprogramowania</span><span class="sxs-lookup"><span data-stu-id="cac9d-192">Software download link expiry</span></span>

<span data-ttu-id="cac9d-193">Od 3 czerwca 2021 r. linki do pobierania oprogramowania w przypadku bezterminowego zakupu oprogramowania i subskrypcji oprogramowania za pośrednictwem usługi Partner Center będą mieć datę wygaśnięcia 5 dni od początkowego pobrania.</span><span class="sxs-lookup"><span data-stu-id="cac9d-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="cac9d-194">Okres wygaśnięcia będzie miał zastosowanie do wszystkich zakupów przed 3 czerwca 2021 r. oraz od 3 czerwca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-195">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-195">Next steps</span></span>

<span data-ttu-id="cac9d-196">Przejrzyj okres [zwrotny CSP i pobierz często](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)zadawane pytania dotyczące wygaśnięcia linku i poinformuj wszystkie odpowiednie zespoły w organizacji o tych zmianach:</span><span class="sxs-lookup"><span data-stu-id="cac9d-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="cac9d-197">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-197">Questions?</span></span>

<span data-ttu-id="cac9d-198">Jeśli masz pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="cac9d-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="cac9d-199">Program licencjonowania Open: Przechodzenie odsprzedawców do programu Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="cac9d-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-200">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-200">Categories</span></span>

- <span data-ttu-id="cac9d-201">Data: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="cac9d-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="cac9d-202">Rozwój firmy</span><span class="sxs-lookup"><span data-stu-id="cac9d-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-203">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-203">Summary</span></span>

<span data-ttu-id="cac9d-204">W tym komunikacie szczegółowo opisano, jak przygotować się do zmian, które zostaną wkrótce wprowadzone w programie licencjonowania Open.</span><span class="sxs-lookup"><span data-stu-id="cac9d-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-205">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-205">Impacted audience</span></span>

<span data-ttu-id="cac9d-206">Partnerzy CSP i Open License</span><span class="sxs-lookup"><span data-stu-id="cac9d-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-207">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-207">Details</span></span>

<span data-ttu-id="cac9d-208">W 2020 r. firma [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) ogłosiła, że bezterminowe licencje na oprogramowanie będą szeroko dostępne dla partnerów i klientów za pośrednictwem programu Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="cac9d-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="cac9d-209">Pierwszy kamień milowy został osiągnięty w styczniu 2021 r., gdy stały się dostępne bezterminowe oferty oprogramowania komercyjnego.</span><span class="sxs-lookup"><span data-stu-id="cac9d-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="cac9d-210">Następny kluczowy kamień milowy nastąpi w lipcu 2021 r., gdy [staną](https://aka.ms/openlicensepublicsector) się dostępne oferty sektora publicznego.</span><span class="sxs-lookup"><span data-stu-id="cac9d-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="cac9d-211">Informujemy [](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) również, że od 1 stycznia 2022 r. za pośrednictwem programu licencjonowania Open nie będzie można kupować ani odnowić licencji na nowe oprogramowanie ani odnowić licencji usługi pakiet Software Assurance ani Usługi online.</span><span class="sxs-lookup"><span data-stu-id="cac9d-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="cac9d-212">Przejście bezterminowego oprogramowania do programu CSP w nowym środowisku handlowym pomoże partnerom rozszerzyć możliwości zaoferowania zróżnicowanych rozwiązań i usług zarządzanych.</span><span class="sxs-lookup"><span data-stu-id="cac9d-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="cac9d-213">Przyspieszy to również przejście klientów do chmury.</span><span class="sxs-lookup"><span data-stu-id="cac9d-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="cac9d-214">Aby pomóc zapewnić bezproblemowe przejście dla naszych partnerów i klientów, dostosowaliśmy te korekty i materiały, aby przyspieszyć tę transformację cyfrową:</span><span class="sxs-lookup"><span data-stu-id="cac9d-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="cac9d-215">Kwiecień 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-215">April 2021</span></span>

<span data-ttu-id="cac9d-216">[Teraz dostępne:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Open License-to-CSP transition materials for resellers (Otwórz materiały przejściowe z licencji na program CSP dla odsprzedawców)</span><span class="sxs-lookup"><span data-stu-id="cac9d-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="cac9d-217">Lipiec 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="cac9d-218">CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-218">CSP</span></span>

- <span data-ttu-id="cac9d-219">1 lipca: bezterminowe licencje na oprogramowanie dostępne dla klientów z sektora publicznego</span><span class="sxs-lookup"><span data-stu-id="cac9d-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="cac9d-220">7 lipca: Visual Studio Pro i Get Genuine Windows Agreement bezterminowe licencje na oprogramowanie dostępne dla wszystkich segmentów</span><span class="sxs-lookup"><span data-stu-id="cac9d-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="cac9d-221">Otwórz wartość</span><span class="sxs-lookup"><span data-stu-id="cac9d-221">Open Value</span></span>

- <span data-ttu-id="cac9d-222">1 lipca: dodatkowe jednostki SKU dostępne w programie Open Value dla organizacji edukacyjnych i non profit, oferując podobne oferty do programu licencjonowania Open</span><span class="sxs-lookup"><span data-stu-id="cac9d-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="cac9d-223">Licencja Open</span><span class="sxs-lookup"><span data-stu-id="cac9d-223">Open License</span></span>

- <span data-ttu-id="cac9d-224">1 lipca: firma Microsoft nie będzie już uruchamiać nowych ofert w programie licencjonowania Open.</span><span class="sxs-lookup"><span data-stu-id="cac9d-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="cac9d-225">Styczeń 2022 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-225">January 2022</span></span>

- <span data-ttu-id="cac9d-226">1 stycznia: w ramach programu licencjonowania Open License nie można dokonać żadnych nowych zakupów ani odnowień</span><span class="sxs-lookup"><span data-stu-id="cac9d-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-227">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="cac9d-228">Dostawcy pośredni dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-228">CSP indirect providers</span></span>

<span data-ttu-id="cac9d-229">Skorzystaj z najbliższych miesięcy, aby pomóc odsprzedawcy licencji Open w zorientowaniu się na program CSP, uczestnicząc w wydarzeniach społeczności partnerów i korzystając z materiałów przejściowych Open License-to-CSP dla odsprzedawców:</span><span class="sxs-lookup"><span data-stu-id="cac9d-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="cac9d-230">Otwórz materiały przejściowe z licencji na CSP dla odsprzedawców — dostosowywalna prezentacja z omówieniem, szablon wiadomości [e-mail,](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)przewodnik dołączania odsprzedawcy pośredniego programu CSP i inne materiały, które ułatwiają wdrożenie dla odsprzedawców na dużą skalę.</span><span class="sxs-lookup"><span data-stu-id="cac9d-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="cac9d-231">[Wydarzenia społeczności partnerów programu CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) hostowane przez firmę Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="cac9d-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="cac9d-232">Dołącz do różnych sesji, aby poznać podstawy programu CSP (CSP Fundamentals) lub być na bieżąco i zadawać pytania dotyczące oprogramowania w programie CSP (Q&A Sessions).</span><span class="sxs-lookup"><span data-stu-id="cac9d-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="cac9d-233">(Już wkrótce) Sesja szkoleniowa ukierunkowana na odsprzedawcę pośredniego w programie CSP hostowana przez firmę Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="cac9d-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="cac9d-234">Odsprzedawcy licencji open</span><span class="sxs-lookup"><span data-stu-id="cac9d-234">Open License resellers</span></span>

- <span data-ttu-id="cac9d-235">Jeśli Twoja organizacja nie jest obecnie zarejestrowane w programie CSP, skontaktuj się z dystrybutorem, aby uzyskać informacje na temat rozpoczynania pracy.</span><span class="sxs-lookup"><span data-stu-id="cac9d-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="cac9d-236">W tym miejscu połącz się z [dostawcą pośrednim.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="cac9d-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="cac9d-237">Jeśli Twoja organizacja jest już zarejestrowane w programie CSP, dowiedz się więcej o oprogramowaniu bezterminowym w programie CSP [tutaj.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="cac9d-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="cac9d-238">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-238">Questions?</span></span>

<span data-ttu-id="cac9d-239">Aby uzyskać więcej pytań na temat tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="cac9d-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="cac9d-240">Teraz na żywo: Przewodnik dotyczący gotowości na promocję globalną</span><span class="sxs-lookup"><span data-stu-id="cac9d-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-241">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-241">Categories</span></span>

- <span data-ttu-id="cac9d-242">Data: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="cac9d-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="cac9d-243">Możliwości</span><span class="sxs-lookup"><span data-stu-id="cac9d-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-244">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-244">Summary</span></span>

<span data-ttu-id="cac9d-245">Gotowość do uruchomienia opublikowała nowy [przewodnik dotyczący gotowości na promocję](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) globalną w galerii zasobów Operations Readiness.</span><span class="sxs-lookup"><span data-stu-id="cac9d-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="cac9d-246">Ten przewodnik zawiera skonsolidowany widok wszystkich aktywnych promocji [globalnych.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="cac9d-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-247">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-247">Impacted audience</span></span>

<span data-ttu-id="cac9d-248">Wszyscy partnerzy licencjonowania zbiorowego (VL), Dynamics Price List (DPL) i Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="cac9d-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-249">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-249">Details</span></span>

<span data-ttu-id="cac9d-250">Partnerzy firmy Microsoft podzielili się z nami potrzebą zapewnienia skonsolidowanego widoku wszystkich globalnych promocji ze szczegółami obsługi.</span><span class="sxs-lookup"><span data-stu-id="cac9d-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="cac9d-251">Chcesz, aby ten skonsolidowany przewodnik ułatwiał korzystanie z promocji z przekonaniem, że wszystkie dostępne informacje będą łatwo dostępne w centralnej i wygodnej lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="cac9d-252">Począwszy od kwietnia 2021 r., firma Microsoft będzie aktualizować ten przewodnik co miesiąc i będzie dostępny w dedykowanej kolekcji przewodników po gotowości na promocję globalną w galerii zasobów Gotowość do operacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="cac9d-253">Linki do tego przewodnika będą również zawarte w następujących kolekcjach:</span><span class="sxs-lookup"><span data-stu-id="cac9d-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="cac9d-254">[Uruchom kolekcję kalendarza](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), która zapewnia scentralizowany widok nadchodzących zmian i startów.</span><span class="sxs-lookup"><span data-stu-id="cac9d-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="cac9d-255">[Kolekcje społeczności](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), które zawierają materiały pomocy technicznej dla naszych comiesięcznych rozmów z partnerami, z wyróżnieniem nadchodzących zmian i terminowych tematów związanych z działaniami operacyjnymi.</span><span class="sxs-lookup"><span data-stu-id="cac9d-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="cac9d-256">[Biuletyny dla partnerów,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)takie jak miesięczna aktualizacja programu CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="cac9d-257">Jako comiesięczne przypomnienie opublikujemy również Partner Center z każdym nowym wydaniem przewodnika po globalnej gotowości na promocję.</span><span class="sxs-lookup"><span data-stu-id="cac9d-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-258">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-258">Next steps</span></span>

<span data-ttu-id="cac9d-259">Na początku każdego miesiąca w galerii [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) zasobów Operations Readiness znajdziesz najnowszy globalny przewodnik gotowości [na promocję.](https://partner.microsoft.com/resources)</span><span class="sxs-lookup"><span data-stu-id="cac9d-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="cac9d-260">Udostępnij te informacje odpowiednim kontaktom w organizacjach i daj nam znać, jak pomocny jest przewodnik, za pośrednictwem strony "Czy ta strona była pomocna?".</span><span class="sxs-lookup"><span data-stu-id="cac9d-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="cac9d-261">na końcu każdej strony.</span><span class="sxs-lookup"><span data-stu-id="cac9d-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="cac9d-262">Aktualizacja społeczności Dostawca rozwiązań w chmurze (CSP) z kwietnia</span><span class="sxs-lookup"><span data-stu-id="cac9d-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-263">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-263">Categories</span></span>

- <span data-ttu-id="cac9d-264">Data: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="cac9d-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="cac9d-265">Społeczność | Zaproszenia i przypomnienia</span><span class="sxs-lookup"><span data-stu-id="cac9d-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-266">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-266">Summary</span></span>

<span data-ttu-id="cac9d-267">Zasoby społeczności CSP są dostępne na żądanie i aktualizowane co miesiąc, aby być na bieżąco z aktualnymi i przygotowanymi do zmian w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="cac9d-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-268">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-268">Impacted audience</span></span>

<span data-ttu-id="cac9d-269">Partnerzy rozliczani bezpośrednio i dostawcy pośredni dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-270">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-270">Details</span></span>

<span data-ttu-id="cac9d-271">W tym miesiącu zasoby obejmują następujące kluczowe tematy:</span><span class="sxs-lookup"><span data-stu-id="cac9d-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="cac9d-272">Aktualizacja do ewolucji programu CSP i zmiany programu licencjonowania Open License</span><span class="sxs-lookup"><span data-stu-id="cac9d-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="cac9d-273">Zmiany wymagań dotyczących dołączania klientów w programie CSP w niektórych regionach</span><span class="sxs-lookup"><span data-stu-id="cac9d-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="cac9d-274">Nowy format nowej faktury w formacie PDF dla handlu w programie CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="cac9d-275">W [kolekcji społeczności CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)znajdziesz:</span><span class="sxs-lookup"><span data-stu-id="cac9d-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="cac9d-276">Biuletyn comiesięcznej aktualizacji programu CSP do pobrania, który agreguje najnowsze ogłoszenia, aktualizacje, zdarzenia i przypomnienia dotyczące programu [CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)w czytelnym dokumencie.</span><span class="sxs-lookup"><span data-stu-id="cac9d-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="cac9d-277">Kalendarz [anonsów dla programu CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)który zapewnia widok osi czasu przyszłych zmian wpływających na program.</span><span class="sxs-lookup"><span data-stu-id="cac9d-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="cac9d-278">Nowy kalendarz [uruchamiania produktu](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), w którym można wyświetlić nadchodzące premiery i oferty produktów.</span><span class="sxs-lookup"><span data-stu-id="cac9d-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="cac9d-279">[Program CSP uruchamia zasoby aktualizacji z](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) łatwą w użyciu zawartością dla kluczowych zmian operacyjnych.</span><span class="sxs-lookup"><span data-stu-id="cac9d-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="cac9d-280">[Odświeżenia i przypomnienia dotyczące kluczowych](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) tematów dotyczących CSP, które otrzymują zainteresowanie i zapytania.</span><span class="sxs-lookup"><span data-stu-id="cac9d-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="cac9d-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="cac9d-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="cac9d-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span><span class="sxs-lookup"><span data-stu-id="cac9d-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="cac9d-283">Zarejestruj się teraz, aby rejestrować się w csp community call Q <1> <3> As that are place in April, May, and June (Zarejestruj się teraz w CSP Community Call Q&amp;Ponieważ odbywa się to w kwietniu, maju i czerwcu.</span><span class="sxs-lookup"><span data-stu-id="cac9d-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="cac9d-284">Skupią się one na najnowszych startach, ważnych odświeżeniach i przypomnieniach.</span><span class="sxs-lookup"><span data-stu-id="cac9d-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="cac9d-285">[Zarejestruj się tutaj.](https://globalpbocomm.eventbuilder.com/GlobalCSP)</span><span class="sxs-lookup"><span data-stu-id="cac9d-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-286">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-286">Next steps</span></span>

<span data-ttu-id="cac9d-287">Zapoznaj się z zasobami społeczności i zarejestruj się w rozmowę społeczności z&A.</span><span class="sxs-lookup"><span data-stu-id="cac9d-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="cac9d-288">Aby upewnić się, że otrzymasz jak najwięcej informacji z forum community Call Q&A, przejrzyj zawartość społeczności na żądanie i prześlij swoje pytania do 48 godzin przed wywołaniem.</span><span class="sxs-lookup"><span data-stu-id="cac9d-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="cac9d-289">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-289">Questions?</span></span>

<span data-ttu-id="cac9d-290">Comiesięczne zaproszenie społeczności CSP&A to najlepsze miejsce na pytania związane ze zmianami w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="cac9d-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="cac9d-291">W każdym miesiącu zapoznaj się z materiałami i prześlij pytania z wyprzedzeniem, abyśmy spędzali sesję na najważniejszych tematach.</span><span class="sxs-lookup"><span data-stu-id="cac9d-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="cac9d-292">Aby uzyskać więcej informacji, skontaktuj się z [pomocą techniczną.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)</span><span class="sxs-lookup"><span data-stu-id="cac9d-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="cac9d-293">Ostatnie przypomnienie: 6 maja 2021 r. oznaczało to, że kwalifikacja GET jest już wyefiniowana</span><span class="sxs-lookup"><span data-stu-id="cac9d-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-294">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-294">Categories</span></span>

- <span data-ttu-id="cac9d-295">Data: 2021-05-04</span><span class="sxs-lookup"><span data-stu-id="cac9d-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="cac9d-296">Możliwości</span><span class="sxs-lookup"><span data-stu-id="cac9d-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-297">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-297">Impacted audience</span></span>

<span data-ttu-id="cac9d-298">Partnerzy sprzedają oferty Academic, Nonprofit i Government Community Cloud (GCC) za pośrednictwem programu Dostawca rozwiązań w chmurze przy użyciu interfejsu API Partner Center api</span><span class="sxs-lookup"><span data-stu-id="cac9d-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-299">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-299">Details</span></span>

<span data-ttu-id="cac9d-300">To zawiadomienie jest kontynuacją rozszerzenia usługi Partner Center [wydanych w grudniu.](https://docs.microsoft.com/partner-center/announcements/2020-december#1)</span><span class="sxs-lookup"><span data-stu-id="cac9d-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="cac9d-301">W ramach tej wersji zostały wdrożone nowe interfejsy API kwalifikacji GET i POST, w związku z tym istniejąca kwalifikacja GET zostanie wycofana 6 maja **2021 r.**</span><span class="sxs-lookup"><span data-stu-id="cac9d-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="cac9d-302">W tym czasie konieczne będzie przejście do korzystania z nowych interfejsów API Partner Center POST.</span><span class="sxs-lookup"><span data-stu-id="cac9d-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="cac9d-303">Nowe interfejsy API POST umożliwią zakup ofert edukacyjnych, a nowe interfejsy API GET umożliwią zakup wstępnie kwalifikowanych ofert organizacji nonprofit i GCC.</span><span class="sxs-lookup"><span data-stu-id="cac9d-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-304">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-304">Next steps</span></span>

- <span data-ttu-id="cac9d-305">**Zaktualizuj do nowych interfejsów API w** celu pomyślnego i terminowego przejścia.</span><span class="sxs-lookup"><span data-stu-id="cac9d-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="cac9d-306">**Zapoznaj się z nowymi zmianami Partner Center API** i przewodnikiem w zasobach gotowość do operacji: [rozszerzenia procesu weryfikacji](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)klienta Partner Center Education.</span><span class="sxs-lookup"><span data-stu-id="cac9d-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="cac9d-307">Udostępnij te informacje odpowiednim zespołom w organizacji oraz odsprzedawcom, aby pomóc im przygotować się do tych zmian.</span><span class="sxs-lookup"><span data-stu-id="cac9d-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="cac9d-308">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-308">Questions?</span></span>

<span data-ttu-id="cac9d-309">W przypadku jakichkolwiek pytań związanych z tym powiadomieniem skontaktuj się z [Partner Center pomocą techniczną.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)</span><span class="sxs-lookup"><span data-stu-id="cac9d-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="cac9d-310">Dziennik zmian</span><span class="sxs-lookup"><span data-stu-id="cac9d-310">Change log</span></span>

- <span data-ttu-id="cac9d-311">4 maja 2021 r.: Ostateczne przypomnienie o zbliżającym się cofaniu kwalifikowania get</span><span class="sxs-lookup"><span data-stu-id="cac9d-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="cac9d-312">9 kwietnia 2021 r.: Przypomnienie o zbliżającym się cofaniu kwalifikowania get</span><span class="sxs-lookup"><span data-stu-id="cac9d-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="cac9d-313">Luty: zaktualizowane osie czasu dotyczące cofania pracy z kwalifikacjami GET & PUT</span><span class="sxs-lookup"><span data-stu-id="cac9d-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="cac9d-314">Styczeń: Przypomnienie o zbliżających się cofaniach pracy z kwalifikacjami GET & PUT</span><span class="sxs-lookup"><span data-stu-id="cac9d-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="cac9d-315">Nowy format nowej faktury w formacie PDF dla handlu w programie CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-316">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-316">Categories</span></span>

- <span data-ttu-id="cac9d-317">Data: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="cac9d-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="cac9d-318">Możliwości</span><span class="sxs-lookup"><span data-stu-id="cac9d-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-319">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-319">Summary</span></span>

<span data-ttu-id="cac9d-320">Firma Microsoft wprowadza nowy format nowej faktury w formacie PDF dla handlu w programie Dostawca rozwiązań w chmurze (CSP) w celu wyświetlania szczegółów rozliczeń według szczegółów produktu zamiast opisu sku.</span><span class="sxs-lookup"><span data-stu-id="cac9d-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-321">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-321">Impacted audience</span></span>

<span data-ttu-id="cac9d-322">Partnerzy inicjujące transakcje za pośrednictwem programu CSP</span><span class="sxs-lookup"><span data-stu-id="cac9d-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-323">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-323">Details</span></span>

<span data-ttu-id="cac9d-324">Od maja 2021 r. firma Microsoft wprowadza nowy format nowej faktury w formacie PDF dla handlu w programie CSP w celu wyświetlania szczegółów rozliczeń według szczegółów produktu zamiast opisu sku.</span><span class="sxs-lookup"><span data-stu-id="cac9d-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="cac9d-325">Dzięki tej nowej aktualizacji będziemy agregować pozycje według typu produktu, jednocześnie wyświetlając każdy produkt w poszczególnych wierszach.</span><span class="sxs-lookup"><span data-stu-id="cac9d-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="cac9d-326">Partnerzy zauważą, że ta zmiana wchodzi w życie na fakturze za maj dla okresu rozliczeniowego od 1 kwietnia 2021 r. do 30 kwietnia 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="cac9d-327">Oferty, których dotyczy problem, Microsoft Azure wystąpienie zarezerwowane, subskrypcje platformy Azure (plan platformy Azure) i marketplace.</span><span class="sxs-lookup"><span data-stu-id="cac9d-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="cac9d-328">Wszystkie żądania dotyczące środków po zaktualizowaniu formatu faktury zostaną wygenerowane w nowym formacie.</span><span class="sxs-lookup"><span data-stu-id="cac9d-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="cac9d-329">Korzyści dla partnerów</span><span class="sxs-lookup"><span data-stu-id="cac9d-329">Partner benefits</span></span>

<span data-ttu-id="cac9d-330">Ta aktualizacja oferuje następujące ulepszenia w zakresie fakturowania dla partnerów:</span><span class="sxs-lookup"><span data-stu-id="cac9d-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="cac9d-331">Zmniejszenie rozmiaru faktury przy zachowaniu danych krytycznych</span><span class="sxs-lookup"><span data-stu-id="cac9d-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="cac9d-332">Dopasowanie formatu do standardów branżowych w przypadku faktur kompaktowych i przyjaznych dla użytkownika</span><span class="sxs-lookup"><span data-stu-id="cac9d-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="cac9d-333">Nie będzie to mieć wpływu na następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="cac9d-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="cac9d-334">Strona podsumowania rozliczeń w pliku PDF faktury</span><span class="sxs-lookup"><span data-stu-id="cac9d-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="cac9d-335">Istniejące interfejsy API fakturowania</span><span class="sxs-lookup"><span data-stu-id="cac9d-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="cac9d-336">Pliki uzgodnień (pliki rekonescji mogą służyć do pobierania szczegółowych danych).</span><span class="sxs-lookup"><span data-stu-id="cac9d-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="cac9d-337">Faktury za użycie i opłaty na podstawie licencji</span><span class="sxs-lookup"><span data-stu-id="cac9d-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-338">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-338">Next steps</span></span>

<span data-ttu-id="cac9d-339">Przejrzyj informacje dotyczące tego tematu w [galerii zasobów Operations Readiness](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) w witrynie internetowej partnerów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cac9d-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="cac9d-340">Aby uzyskać więcej informacji na temat rozliczeń i podatków, w tym zasobów rozliczeniowych, faktur, rozliczeń CSP i podatków, odwiedź sekcję Rozliczenia [w](https://docs.microsoft.com/partner-center/billing) Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cac9d-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="cac9d-341">Zmiany wymagań Dostawca rozwiązań w chmurze (CSP) dotyczące dołączania klientów</span><span class="sxs-lookup"><span data-stu-id="cac9d-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-342">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-342">Categories</span></span>

- <span data-ttu-id="cac9d-343">Data: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="cac9d-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="cac9d-344">Oferty/rynki</span><span class="sxs-lookup"><span data-stu-id="cac9d-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="cac9d-345">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-345">Summary</span></span>

<span data-ttu-id="cac9d-346">W ramach naszego zobowiązania do pomocy partnerom i klientom w perspektywie zaufania poprosimy o dodatkowe informacje o klientach od 25 marca 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-347">Odbiorcy, których to miało wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-347">Impacted audience</span></span>

<span data-ttu-id="cac9d-348">Partnerzy rozliczani bezpośrednio w programie CSP i dostawcy pośredni, którzy mają nowych lub istniejących klientów w krajach wymienionych w następnej sekcji</span><span class="sxs-lookup"><span data-stu-id="cac9d-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-349">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-349">Details</span></span>

<span data-ttu-id="cac9d-350">Firma Microsoft działa w oparciu o zaufanie.</span><span class="sxs-lookup"><span data-stu-id="cac9d-350">Microsoft runs on trust.</span></span> <span data-ttu-id="cac9d-351">Dążymy do zapewnienia zgodnej, bezpiecznej i bezpiecznej metody weryfikacji klienta na potrzeby transakcji subskrypcji klientów w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="cac9d-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="cac9d-352">25 marca 2021 r. wprowadzimy ulepszenia interfejsu API i interfejsu użytkownika usługi Partner Center, które będą mieć wpływ na partnerów spełniających oba następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="cac9d-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="cac9d-353">Partner ma bezpośrednią relację rozliczeń z firmą Microsoft (co oznacza, że partner jest partnerem z rozliczaniem bezpośrednim lub dostawcą pośrednim).</span><span class="sxs-lookup"><span data-stu-id="cac9d-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="cac9d-354">Partner współpracuje z nowymi lub istniejącymi klientami w następujących krajach:</span><span class="sxs-lookup"><span data-stu-id="cac9d-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="cac9d-355">Tajlandia</span><span class="sxs-lookup"><span data-stu-id="cac9d-355">Thailand</span></span>
    - <span data-ttu-id="cac9d-356">Wietnam</span><span class="sxs-lookup"><span data-stu-id="cac9d-356">Vietnam</span></span>
    - <span data-ttu-id="cac9d-357">Turcja</span><span class="sxs-lookup"><span data-stu-id="cac9d-357">Turkey</span></span>
    - <span data-ttu-id="cac9d-358">Polska</span><span class="sxs-lookup"><span data-stu-id="cac9d-358">Poland</span></span>
    - <span data-ttu-id="cac9d-359">Republika Południowej Afryki</span><span class="sxs-lookup"><span data-stu-id="cac9d-359">South Africa</span></span>
    - <span data-ttu-id="cac9d-360">Indie</span><span class="sxs-lookup"><span data-stu-id="cac9d-360">India</span></span>
    - <span data-ttu-id="cac9d-361">Brazylia</span><span class="sxs-lookup"><span data-stu-id="cac9d-361">Brazil</span></span>
    - <span data-ttu-id="cac9d-362">Irak</span><span class="sxs-lookup"><span data-stu-id="cac9d-362">Iraq</span></span>
    - <span data-ttu-id="cac9d-363">Myanmar</span><span class="sxs-lookup"><span data-stu-id="cac9d-363">Myanmar</span></span>
    - <span data-ttu-id="cac9d-364">Sudan Południowy</span><span class="sxs-lookup"><span data-stu-id="cac9d-364">South Sudan</span></span>
    - <span data-ttu-id="cac9d-365">Arabia Saudyjska</span><span class="sxs-lookup"><span data-stu-id="cac9d-365">Saudi Arabia</span></span>
    - <span data-ttu-id="cac9d-366">Zjednoczone Emiraty Arabskie</span><span class="sxs-lookup"><span data-stu-id="cac9d-366">United Arab Emirates</span></span>
    - <span data-ttu-id="cac9d-367">Wenezuela</span><span class="sxs-lookup"><span data-stu-id="cac9d-367">Venezuela</span></span>

<span data-ttu-id="cac9d-368">Partnerzy spełniający te kryteria muszą przesłać identyfikator rejestracji firmy klienta (znany także jako organizacja klienta ), oraz numer telefonu podczas następnej aktualizacji lub utworzenia subskrypcji dla tego klienta.</span><span class="sxs-lookup"><span data-stu-id="cac9d-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="cac9d-369">Ci partnerzy mogą również wprowadzić opcjonalne drugie imię klienta.</span><span class="sxs-lookup"><span data-stu-id="cac9d-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="cac9d-370">Pamiętaj, że podczas dodawania identyfikatora rejestracji firmy należy użyć identyfikatora podatku od działalności biznesowej, a nie identyfikatora osobistego klienta.</span><span class="sxs-lookup"><span data-stu-id="cac9d-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="cac9d-371">Partnerzy, którzy współpracuje z nowymi lub istniejącymi klientami w następujących krajach, są już dołączani do poprzedniej wersji w listopadzie 2020 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="cac9d-372">Armenia</span><span class="sxs-lookup"><span data-stu-id="cac9d-372">Armenia</span></span>
- <span data-ttu-id="cac9d-373">Azerbejdżan</span><span class="sxs-lookup"><span data-stu-id="cac9d-373">Azerbaijan</span></span>
- <span data-ttu-id="cac9d-374">Białoruś</span><span class="sxs-lookup"><span data-stu-id="cac9d-374">Belarus</span></span>
- <span data-ttu-id="cac9d-375">Węgry</span><span class="sxs-lookup"><span data-stu-id="cac9d-375">Hungary</span></span>
- <span data-ttu-id="cac9d-376">Kazachstan</span><span class="sxs-lookup"><span data-stu-id="cac9d-376">Kazakhstan</span></span>
- <span data-ttu-id="cac9d-377">Kirgistan</span><span class="sxs-lookup"><span data-stu-id="cac9d-377">Kyrgyzstan</span></span>
- <span data-ttu-id="cac9d-378">Mołdawia</span><span class="sxs-lookup"><span data-stu-id="cac9d-378">Moldova</span></span>
- <span data-ttu-id="cac9d-379">Rosja</span><span class="sxs-lookup"><span data-stu-id="cac9d-379">Russia</span></span>
- <span data-ttu-id="cac9d-380">Tadżykistan</span><span class="sxs-lookup"><span data-stu-id="cac9d-380">Tajikistan</span></span>
- <span data-ttu-id="cac9d-381">Ukraina</span><span class="sxs-lookup"><span data-stu-id="cac9d-381">Ukraine</span></span>
- <span data-ttu-id="cac9d-382">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="cac9d-382">Uzbekistan</span></span>

<span data-ttu-id="cac9d-383">Pod koniec marca 2021 r. partnerzy z klientami na całym świecie będą mieć możliwość wprowadzania identyfikatora rejestracji firmy, numeru telefonu i średniego imienia dla klientów jako opcjonalnych szczegółów.</span><span class="sxs-lookup"><span data-stu-id="cac9d-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-384">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-384">Next steps</span></span>

- <span data-ttu-id="cac9d-385">Przejrzyj dokumentację techniczną i często zadawane pytania w dedykowanej [kolekcji partnerów,](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) aby uzyskać bardziej szczegółowe wskazówki.</span><span class="sxs-lookup"><span data-stu-id="cac9d-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="cac9d-386">Przygotuj się do uwzględnienia zmian przy użyciu Partner Center API i internetowego interfejsu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="cac9d-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="cac9d-387">Zestawy API/zestawy SDK będą dostępne do testowania.</span><span class="sxs-lookup"><span data-stu-id="cac9d-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="cac9d-388">Pamiętaj, aby przesłać dodatkowe dane podczas dołączania nowych klientów lub modyfikowania istniejących danych klienta.</span><span class="sxs-lookup"><span data-stu-id="cac9d-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="cac9d-389">Jeśli używasz rozwiązania dostawcy panelu sterowania (CPV), skonsultuj się z dostawcą CPV.</span><span class="sxs-lookup"><span data-stu-id="cac9d-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="cac9d-390">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-390">Questions?</span></span>

<span data-ttu-id="cac9d-391">Skontaktuj się z doradcą podatkowym lub lokalnym urzędem podatkowym, jeśli masz pytania związane z identyfikatorem rejestracji firmy (nazywanym również INFORMACJAMI lub NIP).</span><span class="sxs-lookup"><span data-stu-id="cac9d-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="cac9d-392">Firma Microsoft nie może zapewnić wskazówek dotyczących kwestii podatkowych.</span><span class="sxs-lookup"><span data-stu-id="cac9d-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="cac9d-393">Jeśli potrzebujesz pomocy technicznej dotyczącej operacji wykonywanych w firmie Microsoft, otwórz [żądanie obsługi](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="cac9d-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="cac9d-394">Wyświetlanie ofert i uruchomień produktów w tym miesiącu</span><span class="sxs-lookup"><span data-stu-id="cac9d-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="cac9d-395">Kategorie</span><span class="sxs-lookup"><span data-stu-id="cac9d-395">Categories</span></span>

- <span data-ttu-id="cac9d-396">Data: 2021-04-01</span><span class="sxs-lookup"><span data-stu-id="cac9d-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="cac9d-397">Możliwości</span><span class="sxs-lookup"><span data-stu-id="cac9d-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="cac9d-398">Podsumowanie</span><span class="sxs-lookup"><span data-stu-id="cac9d-398">Summary</span></span>

<span data-ttu-id="cac9d-399">Opublikowano kalendarz uruchamiania produktów z kwietnia 2021 r.</span><span class="sxs-lookup"><span data-stu-id="cac9d-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="cac9d-400">Odbiorcy, na które ma to wpływ</span><span class="sxs-lookup"><span data-stu-id="cac9d-400">Impacted audience</span></span>

<span data-ttu-id="cac9d-401">Wszyscy partnerzy w ramach programu Dostawca rozwiązań w chmurze (CSP)</span><span class="sxs-lookup"><span data-stu-id="cac9d-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="cac9d-402">Szczegóły</span><span class="sxs-lookup"><span data-stu-id="cac9d-402">Details</span></span>

<span data-ttu-id="cac9d-403">Kalendarz uruchamiania produktów z [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) kwietnia 2021 r. jest teraz dostępny w galerii zasobów gotowość do operacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="cac9d-404">Zobacz nadchodzące wprowadzenie produktu i oferty tutaj.</span><span class="sxs-lookup"><span data-stu-id="cac9d-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="cac9d-405">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cac9d-405">Next steps</span></span>

<span data-ttu-id="cac9d-406">Przejrzyj kalendarz [uruchamiania produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)i udostępnij informacje odpowiednim uczestnikom projektu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="cac9d-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="cac9d-407">Masz pytania?</span><span class="sxs-lookup"><span data-stu-id="cac9d-407">Questions?</span></span>

<span data-ttu-id="cac9d-408">Jeśli masz dodatkowe pytania dotyczące tych ofert, sprawdź odpowiednie społeczności usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="cac9d-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>
