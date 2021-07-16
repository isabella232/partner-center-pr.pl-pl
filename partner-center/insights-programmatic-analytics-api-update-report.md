---
title: Aktualizowanie interfejsu API raportów
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ten interfejs API umożliwia aktualizowanie parametrów raportu w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377179"
---
# <a name="update-report-api"></a><span data-ttu-id="af2d9-103">Aktualizowanie interfejsu API raportów</span><span class="sxs-lookup"><span data-stu-id="af2d9-103">Update report API</span></span>

<span data-ttu-id="af2d9-104">Ten interfejs API ułatwia modyfikowanie parametru raportu.</span><span class="sxs-lookup"><span data-stu-id="af2d9-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="af2d9-105">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="af2d9-105">**Request syntax**</span></span>

|    <span data-ttu-id="af2d9-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="af2d9-106">Method</span></span>    |    <span data-ttu-id="af2d9-107">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="af2d9-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="af2d9-108">PUT</span><span class="sxs-lookup"><span data-stu-id="af2d9-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="af2d9-109">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="af2d9-109">**Request header**</span></span>

|    <span data-ttu-id="af2d9-110">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="af2d9-110">Header</span></span>    |    <span data-ttu-id="af2d9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="af2d9-111">Type</span></span>    |    <span data-ttu-id="af2d9-112">Opis</span><span class="sxs-lookup"><span data-stu-id="af2d9-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="af2d9-113">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="af2d9-113">Authorization</span></span>    |    <span data-ttu-id="af2d9-114">ciąg</span><span class="sxs-lookup"><span data-stu-id="af2d9-114">string</span></span>    |    <span data-ttu-id="af2d9-115">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="af2d9-115">Required.</span></span> <span data-ttu-id="af2d9-116">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="af2d9-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="af2d9-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af2d9-117">Content-Type</span></span>    |    <span data-ttu-id="af2d9-118">ciąg</span><span class="sxs-lookup"><span data-stu-id="af2d9-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="af2d9-119">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="af2d9-119">**Path parameter**</span></span>

|    <span data-ttu-id="af2d9-120">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="af2d9-120">Parameter Name</span></span>    |    <span data-ttu-id="af2d9-121">Typ</span><span class="sxs-lookup"><span data-stu-id="af2d9-121">Type</span></span>    |    <span data-ttu-id="af2d9-122">Wymagane</span><span class="sxs-lookup"><span data-stu-id="af2d9-122">Required</span></span>    |    <span data-ttu-id="af2d9-123">Opis</span><span class="sxs-lookup"><span data-stu-id="af2d9-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="af2d9-124">reportId</span><span class="sxs-lookup"><span data-stu-id="af2d9-124">reportId</span></span>     |    <span data-ttu-id="af2d9-125">ciąg</span><span class="sxs-lookup"><span data-stu-id="af2d9-125">string</span></span>    |    <span data-ttu-id="af2d9-126">Nie</span><span class="sxs-lookup"><span data-stu-id="af2d9-126">No</span></span>    |    <span data-ttu-id="af2d9-127">Identyfikator modyfikowanego raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="af2d9-128">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="af2d9-128">**Query parameter**</span></span>

<span data-ttu-id="af2d9-129">Brak</span><span class="sxs-lookup"><span data-stu-id="af2d9-129">None</span></span>

<span data-ttu-id="af2d9-130">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="af2d9-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="af2d9-131">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="af2d9-131">**Glossary**</span></span>

<span data-ttu-id="af2d9-132">W tej tabeli wymieniono kluczowe definicje elementów w odpowiedzi.</span><span class="sxs-lookup"><span data-stu-id="af2d9-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="af2d9-133">Parametr</span><span class="sxs-lookup"><span data-stu-id="af2d9-133">Parameter</span></span>    |    <span data-ttu-id="af2d9-134">Wymagane</span><span class="sxs-lookup"><span data-stu-id="af2d9-134">Required</span></span>    |    <span data-ttu-id="af2d9-135">Opis</span><span class="sxs-lookup"><span data-stu-id="af2d9-135">Description</span></span>    |    <span data-ttu-id="af2d9-136">Dozwolone wartości</span><span class="sxs-lookup"><span data-stu-id="af2d9-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="af2d9-137">Reportname</span><span class="sxs-lookup"><span data-stu-id="af2d9-137">ReportName</span></span>     |    <span data-ttu-id="af2d9-138">Yes</span><span class="sxs-lookup"><span data-stu-id="af2d9-138">Yes</span></span>     |    <span data-ttu-id="af2d9-139">Nazwa, która ma zostać przypisana do raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="af2d9-140">Ciąg</span><span class="sxs-lookup"><span data-stu-id="af2d9-140">String</span></span>     |
|    <span data-ttu-id="af2d9-141">Opis</span><span class="sxs-lookup"><span data-stu-id="af2d9-141">Description</span></span>     |    <span data-ttu-id="af2d9-142">Nie</span><span class="sxs-lookup"><span data-stu-id="af2d9-142">No</span></span>     |    <span data-ttu-id="af2d9-143">Opis utworzonego raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-143">Description of the created report</span></span>     |    <span data-ttu-id="af2d9-144">Ciąg</span><span class="sxs-lookup"><span data-stu-id="af2d9-144">String</span></span>     |
|    <span data-ttu-id="af2d9-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="af2d9-145">StartTime</span></span>     |    <span data-ttu-id="af2d9-146">Yes</span><span class="sxs-lookup"><span data-stu-id="af2d9-146">Yes</span></span>    |    <span data-ttu-id="af2d9-147">Sygnatura czasowa, po której rozpocznie się generowanie raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="af2d9-148">Ciąg</span><span class="sxs-lookup"><span data-stu-id="af2d9-148">String</span></span>     |
|    <span data-ttu-id="af2d9-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="af2d9-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="af2d9-150">Nie</span><span class="sxs-lookup"><span data-stu-id="af2d9-150">No</span></span>     |    <span data-ttu-id="af2d9-151">Częstotliwość generowania raportu w godzinach.</span><span class="sxs-lookup"><span data-stu-id="af2d9-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="af2d9-152">Wartość minimalna to 4</span><span class="sxs-lookup"><span data-stu-id="af2d9-152">Minimum value is 4</span></span>     |    <span data-ttu-id="af2d9-153">Liczba całkowita</span><span class="sxs-lookup"><span data-stu-id="af2d9-153">Integer</span></span>     |
|    <span data-ttu-id="af2d9-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="af2d9-154">RecurrenceCount</span></span>     |    <span data-ttu-id="af2d9-155">Nie</span><span class="sxs-lookup"><span data-stu-id="af2d9-155">No</span></span>     |    <span data-ttu-id="af2d9-156">Liczba raportów do wygenerowania.</span><span class="sxs-lookup"><span data-stu-id="af2d9-156">Numbers of report to be generated.</span></span> <span data-ttu-id="af2d9-157">Wartość domyślna to nieokreślony.</span><span class="sxs-lookup"><span data-stu-id="af2d9-157">Default is indefinite.</span></span>     |    <span data-ttu-id="af2d9-158">Liczba całkowita</span><span class="sxs-lookup"><span data-stu-id="af2d9-158">Integer</span></span>     |
|    <span data-ttu-id="af2d9-159">Format</span><span class="sxs-lookup"><span data-stu-id="af2d9-159">Format</span></span>     |    <span data-ttu-id="af2d9-160">Nie</span><span class="sxs-lookup"><span data-stu-id="af2d9-160">No</span></span>    |    <span data-ttu-id="af2d9-161">Format wyeksportowanego pliku.</span><span class="sxs-lookup"><span data-stu-id="af2d9-161">File format of the exported file.</span></span> <span data-ttu-id="af2d9-162">Wartość domyślna to CSV</span><span class="sxs-lookup"><span data-stu-id="af2d9-162">Default is CSV</span></span>     |    <span data-ttu-id="af2d9-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="af2d9-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="af2d9-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="af2d9-164">CallbackURL</span></span>     |    <span data-ttu-id="af2d9-165">Nie</span><span class="sxs-lookup"><span data-stu-id="af2d9-165">No</span></span>     |    <span data-ttu-id="af2d9-166">Adres URL wywołania zwrotnego HTTPS, który ma być wywoływany podczas generowania raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="af2d9-167">Ciąg</span><span class="sxs-lookup"><span data-stu-id="af2d9-167">String</span></span>     |
|    <span data-ttu-id="af2d9-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="af2d9-168">CallbackMethod</span></span>    |    <span data-ttu-id="af2d9-169">Nie</span><span class="sxs-lookup"><span data-stu-id="af2d9-169">No</span></span>    |    <span data-ttu-id="af2d9-170">Metoda HTTP, która ma być używana do wywołania zwrotnego</span><span class="sxs-lookup"><span data-stu-id="af2d9-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="af2d9-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="af2d9-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="af2d9-172">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="af2d9-172">**Response**</span></span>

<span data-ttu-id="af2d9-173">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="af2d9-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="af2d9-174">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="af2d9-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="af2d9-175">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="af2d9-175">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="af2d9-176">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="af2d9-176">**Glossary**</span></span>

<span data-ttu-id="af2d9-177">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="af2d9-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="af2d9-178">Parametr</span><span class="sxs-lookup"><span data-stu-id="af2d9-178">Parameter</span></span>    |    <span data-ttu-id="af2d9-179">Opis</span><span class="sxs-lookup"><span data-stu-id="af2d9-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="af2d9-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="af2d9-180">ReportId</span></span>     |    <span data-ttu-id="af2d9-181">Uniwersalny unikatowy identyfikator (UUID) aktualizowanego raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="af2d9-182">Reportname</span><span class="sxs-lookup"><span data-stu-id="af2d9-182">ReportName</span></span>     |    <span data-ttu-id="af2d9-183">Nazwa nadana raportowi w ładunku żądania</span><span class="sxs-lookup"><span data-stu-id="af2d9-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="af2d9-184">Opis</span><span class="sxs-lookup"><span data-stu-id="af2d9-184">Description</span></span>     |    <span data-ttu-id="af2d9-185">Opis podany w raporcie w ładunku żądania</span><span class="sxs-lookup"><span data-stu-id="af2d9-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="af2d9-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="af2d9-186">QueryId</span></span>     |    <span data-ttu-id="af2d9-187">Identyfikator zapytania przekazany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="af2d9-188">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="af2d9-188">Query</span></span>     |    <span data-ttu-id="af2d9-189">Tekst zapytania, który zostanie wykonany dla tego raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="af2d9-190">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="af2d9-190">User</span></span>     |    <span data-ttu-id="af2d9-191">Identyfikator użytkownika użyty do utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="af2d9-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="af2d9-192">CreatedTime</span></span>     |    <span data-ttu-id="af2d9-193">Godzina utworzenia raportu.</span><span class="sxs-lookup"><span data-stu-id="af2d9-193">Time the report was created.</span></span> <span data-ttu-id="af2d9-194">Format czasu to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="af2d9-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="af2d9-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="af2d9-195">ModifiedTime</span></span>     |    <span data-ttu-id="af2d9-196">Godzina ostatniej modyfikacji raportu.</span><span class="sxs-lookup"><span data-stu-id="af2d9-196">Time the report was last modified.</span></span> <span data-ttu-id="af2d9-197">Format czasu to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="af2d9-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="af2d9-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="af2d9-198">ExecuteNow</span></span>     |    <span data-ttu-id="af2d9-199">Flaga ExecuteNow ustawiona w czasie tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="af2d9-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="af2d9-200">StartTime</span></span>     |    <span data-ttu-id="af2d9-201">Czas rozpoczęcia wykonywania raportu.</span><span class="sxs-lookup"><span data-stu-id="af2d9-201">Time the report execution will begin.</span></span> <span data-ttu-id="af2d9-202">Format godziny to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="af2d9-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="af2d9-203">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="af2d9-203">ReportStatus</span></span>     |    <span data-ttu-id="af2d9-204">Stan wykonania raportu.</span><span class="sxs-lookup"><span data-stu-id="af2d9-204">Status of the report execution.</span></span> <span data-ttu-id="af2d9-205">Możliwe wartości to Wstrzymane, Aktywne i Nieaktywne.</span><span class="sxs-lookup"><span data-stu-id="af2d9-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="af2d9-206">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="af2d9-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="af2d9-207">Interwał cyklu podany w ładunku żądania</span><span class="sxs-lookup"><span data-stu-id="af2d9-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="af2d9-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="af2d9-208">RecurrenceCount</span></span>     |    <span data-ttu-id="af2d9-209">Liczba cyklów podana w ładunku żądania</span><span class="sxs-lookup"><span data-stu-id="af2d9-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="af2d9-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="af2d9-210">CallbackUrl</span></span>     |    <span data-ttu-id="af2d9-211">Adres URL wywołania zwrotnego podany w żądaniu</span><span class="sxs-lookup"><span data-stu-id="af2d9-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="af2d9-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="af2d9-212">CallbackMethod</span></span>    |    <span data-ttu-id="af2d9-213">Metoda wywołania zwrotnego podana w żądaniu</span><span class="sxs-lookup"><span data-stu-id="af2d9-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="af2d9-214">Format</span><span class="sxs-lookup"><span data-stu-id="af2d9-214">Format</span></span>     |    <span data-ttu-id="af2d9-215">Format plików raportu</span><span class="sxs-lookup"><span data-stu-id="af2d9-215">Format of the report files</span></span>     |
|    <span data-ttu-id="af2d9-216">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="af2d9-216">TotalCount</span></span>     |    <span data-ttu-id="af2d9-217">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="af2d9-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="af2d9-218">Komunikat</span><span class="sxs-lookup"><span data-stu-id="af2d9-218">Message</span></span>     |    <span data-ttu-id="af2d9-219">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="af2d9-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="af2d9-220">Statuscode</span><span class="sxs-lookup"><span data-stu-id="af2d9-220">StatusCode</span></span>     |    <span data-ttu-id="af2d9-221">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="af2d9-221">Result Code.</span></span> <span data-ttu-id="af2d9-222">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="af2d9-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |