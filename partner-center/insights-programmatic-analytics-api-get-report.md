---
title: Uzyskiwanie interfejsu API raportów — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ten interfejs API umożliwia uzyskiwanie wszystkich dostępnych identyfikatorów raportów w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377203"
---
# <a name="get-report-api"></a><span data-ttu-id="f44cf-103">Uzyskiwanie interfejsu API raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-103">Get report API</span></span>

<span data-ttu-id="f44cf-104">Ten interfejs API pobiera wszystkie raporty, które zostały zaplanowane.</span><span class="sxs-lookup"><span data-stu-id="f44cf-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="f44cf-105">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="f44cf-105">**Request syntax**</span></span>

|    <span data-ttu-id="f44cf-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="f44cf-106">Method</span></span>    |    <span data-ttu-id="f44cf-107">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="f44cf-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="f44cf-108">GET</span><span class="sxs-lookup"><span data-stu-id="f44cf-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="f44cf-109">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="f44cf-109">**Request header**</span></span>

|    <span data-ttu-id="f44cf-110">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="f44cf-110">Header</span></span>    |    <span data-ttu-id="f44cf-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f44cf-111">Type</span></span>    |    <span data-ttu-id="f44cf-112">Opis</span><span class="sxs-lookup"><span data-stu-id="f44cf-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="f44cf-113">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="f44cf-113">Authorization</span></span>    |    <span data-ttu-id="f44cf-114">ciąg</span><span class="sxs-lookup"><span data-stu-id="f44cf-114">string</span></span>    |    <span data-ttu-id="f44cf-115">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="f44cf-115">Required.</span></span> <span data-ttu-id="f44cf-116">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="f44cf-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="f44cf-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f44cf-117">Content-Type</span></span>    |    <span data-ttu-id="f44cf-118">ciąg</span><span class="sxs-lookup"><span data-stu-id="f44cf-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="f44cf-119">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="f44cf-119">**Path parameter**</span></span>

<span data-ttu-id="f44cf-120">Brak</span><span class="sxs-lookup"><span data-stu-id="f44cf-120">None</span></span>

<span data-ttu-id="f44cf-121">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="f44cf-121">**Query parameter**</span></span>

|    <span data-ttu-id="f44cf-122">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="f44cf-122">Parameter Name</span></span>    |    <span data-ttu-id="f44cf-123">Typ</span><span class="sxs-lookup"><span data-stu-id="f44cf-123">Type</span></span>    |    <span data-ttu-id="f44cf-124">Wymagane</span><span class="sxs-lookup"><span data-stu-id="f44cf-124">Required</span></span>    |    <span data-ttu-id="f44cf-125">Opis</span><span class="sxs-lookup"><span data-stu-id="f44cf-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="f44cf-126">reportId</span><span class="sxs-lookup"><span data-stu-id="f44cf-126">reportId</span></span>     |    <span data-ttu-id="f44cf-127">ciąg</span><span class="sxs-lookup"><span data-stu-id="f44cf-127">string</span></span>    |    <span data-ttu-id="f44cf-128">Nie</span><span class="sxs-lookup"><span data-stu-id="f44cf-128">No</span></span>    |    <span data-ttu-id="f44cf-129">Filtrowanie w celu uzyskania szczegółów tylko raportów z argumentem reportId podanym w tym argumentie</span><span class="sxs-lookup"><span data-stu-id="f44cf-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="f44cf-130">Reportname</span><span class="sxs-lookup"><span data-stu-id="f44cf-130">reportName</span></span>     |    <span data-ttu-id="f44cf-131">ciąg</span><span class="sxs-lookup"><span data-stu-id="f44cf-131">string</span></span>    |    <span data-ttu-id="f44cf-132">Nie</span><span class="sxs-lookup"><span data-stu-id="f44cf-132">No</span></span>    |    <span data-ttu-id="f44cf-133">Filtrowanie w celu uzyskania szczegółów tylko raportów o nazwie reportName podanej w tym argumentie</span><span class="sxs-lookup"><span data-stu-id="f44cf-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="f44cf-134">queryId</span><span class="sxs-lookup"><span data-stu-id="f44cf-134">queryId</span></span>     |    <span data-ttu-id="f44cf-135">ciąg</span><span class="sxs-lookup"><span data-stu-id="f44cf-135">string</span></span>    |    <span data-ttu-id="f44cf-136">Nie</span><span class="sxs-lookup"><span data-stu-id="f44cf-136">No</span></span>    |    <span data-ttu-id="f44cf-137">Filtrowanie w celu uzyskania szczegółów tylko raportów z argumentem queryId podanym w tym argumentie</span><span class="sxs-lookup"><span data-stu-id="f44cf-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="f44cf-138">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="f44cf-138">**Request payload**</span></span>

<span data-ttu-id="f44cf-139">Brak</span><span class="sxs-lookup"><span data-stu-id="f44cf-139">None</span></span>

<span data-ttu-id="f44cf-140">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="f44cf-140">**Glossary**</span></span>

<span data-ttu-id="f44cf-141">Brak</span><span class="sxs-lookup"><span data-stu-id="f44cf-141">None</span></span>

<span data-ttu-id="f44cf-142">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="f44cf-142">**Response**</span></span>

<span data-ttu-id="f44cf-143">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="f44cf-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="f44cf-144">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="f44cf-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="f44cf-145">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="f44cf-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="f44cf-146">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="f44cf-146">**Glossary**</span></span>

<span data-ttu-id="f44cf-147">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="f44cf-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="f44cf-148">Parametr</span><span class="sxs-lookup"><span data-stu-id="f44cf-148">Parameter</span></span>    |    <span data-ttu-id="f44cf-149">Opis</span><span class="sxs-lookup"><span data-stu-id="f44cf-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="f44cf-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="f44cf-150">ReportId</span></span>     |    <span data-ttu-id="f44cf-151">Unikatowy identyfikator UUID utworzonego raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="f44cf-152">Reportname</span><span class="sxs-lookup"><span data-stu-id="f44cf-152">ReportName</span></span>     |    <span data-ttu-id="f44cf-153">Nazwa nadana raportowi w ładunku żądania</span><span class="sxs-lookup"><span data-stu-id="f44cf-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="f44cf-154">Opis</span><span class="sxs-lookup"><span data-stu-id="f44cf-154">Description</span></span>     |    <span data-ttu-id="f44cf-155">Opis podany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="f44cf-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="f44cf-156">QueryId</span></span>     |    <span data-ttu-id="f44cf-157">Identyfikator zapytania przekazany w momencie utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="f44cf-158">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="f44cf-158">Query</span></span>     |    <span data-ttu-id="f44cf-159">Tekst zapytania, który zostanie wykonany dla tego raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="f44cf-160">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="f44cf-160">User</span></span>     |    <span data-ttu-id="f44cf-161">Identyfikator użytkownika użyty do utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="f44cf-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="f44cf-162">CreatedTime</span></span>     |    <span data-ttu-id="f44cf-163">Godzina utworzenia raportu.</span><span class="sxs-lookup"><span data-stu-id="f44cf-163">Time the report was created.</span></span> <span data-ttu-id="f44cf-164">Format godziny to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="f44cf-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="f44cf-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="f44cf-165">ModifiedTime</span></span>     |    <span data-ttu-id="f44cf-166">Godzina ostatniej modyfikacji raportu.</span><span class="sxs-lookup"><span data-stu-id="f44cf-166">Time the report was last modified.</span></span> <span data-ttu-id="f44cf-167">Format godziny to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="f44cf-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="f44cf-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="f44cf-168">executeNow</span></span>     |    <span data-ttu-id="f44cf-169">Flaga ExecuteNow ustawiona w czasie tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="f44cf-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="f44cf-170">StartTime</span></span>     |    <span data-ttu-id="f44cf-171">Rozpocznie się wykonywanie czasu.</span><span class="sxs-lookup"><span data-stu-id="f44cf-171">Time execution will begin.</span></span> <span data-ttu-id="f44cf-172">Format godziny to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="f44cf-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="f44cf-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="f44cf-173">ReportStatus</span></span>     |    <span data-ttu-id="f44cf-174">Stan wykonania raportu.</span><span class="sxs-lookup"><span data-stu-id="f44cf-174">Status of the report execution.</span></span> <span data-ttu-id="f44cf-175">Możliwe wartości to Wstrzymane, Aktywne i Nieaktywne.</span><span class="sxs-lookup"><span data-stu-id="f44cf-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="f44cf-176">CyklInterval</span><span class="sxs-lookup"><span data-stu-id="f44cf-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="f44cf-177">Interwał cyklu zapewniany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="f44cf-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="f44cf-178">RecurrenceCount</span></span>     |    <span data-ttu-id="f44cf-179">Liczba cyklów zapewniana podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="f44cf-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="f44cf-180">CallbackUrl</span></span>     |    <span data-ttu-id="f44cf-181">Adres URL wywołania zwrotnego podany w żądaniu</span><span class="sxs-lookup"><span data-stu-id="f44cf-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="f44cf-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="f44cf-182">CallbackMethod</span></span>    |    <span data-ttu-id="f44cf-183">Metoda wywołania zwrotnego podana w żądaniu</span><span class="sxs-lookup"><span data-stu-id="f44cf-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="f44cf-184">Format</span><span class="sxs-lookup"><span data-stu-id="f44cf-184">Format</span></span>     |    <span data-ttu-id="f44cf-185">Format plików raportu</span><span class="sxs-lookup"><span data-stu-id="f44cf-185">Format of the report files</span></span>     |
|    <span data-ttu-id="f44cf-186">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="f44cf-186">TotalCount</span></span>     |    <span data-ttu-id="f44cf-187">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="f44cf-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="f44cf-188">Komunikat</span><span class="sxs-lookup"><span data-stu-id="f44cf-188">Message</span></span>     |    <span data-ttu-id="f44cf-189">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="f44cf-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="f44cf-190">Statuscode</span><span class="sxs-lookup"><span data-stu-id="f44cf-190">StatusCode</span></span>     |    <span data-ttu-id="f44cf-191">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="f44cf-191">Result Code.</span></span> <span data-ttu-id="f44cf-192">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="f44cf-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |