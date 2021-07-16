---
title: Wznawianie interfejsu API wykonywania raportu — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ten interfejs API umożliwia wznowienie wykonywania dowolnego wstrzymanego raportu w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377194"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="b1aa7-103">Wznawianie interfejsu API wykonywania raportów</span><span class="sxs-lookup"><span data-stu-id="b1aa7-103">Resume report executions API</span></span>

<span data-ttu-id="b1aa7-104">Po wykonaniu ten interfejs API wznawia zaplanowane wykonywanie wstrzymanego raportu.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="b1aa7-105">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-105">**Request syntax**</span></span>

|    <span data-ttu-id="b1aa7-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="b1aa7-106">Method</span></span>    |    <span data-ttu-id="b1aa7-107">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="b1aa7-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b1aa7-108">PUT</span><span class="sxs-lookup"><span data-stu-id="b1aa7-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="b1aa7-109">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-109">**Request header**</span></span>

|    <span data-ttu-id="b1aa7-110">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="b1aa7-110">Header</span></span>    |    <span data-ttu-id="b1aa7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b1aa7-111">Type</span></span>    |    <span data-ttu-id="b1aa7-112">Opis</span><span class="sxs-lookup"><span data-stu-id="b1aa7-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="b1aa7-113">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="b1aa7-113">Authorization</span></span>    |    <span data-ttu-id="b1aa7-114">ciąg</span><span class="sxs-lookup"><span data-stu-id="b1aa7-114">string</span></span>    |    <span data-ttu-id="b1aa7-115">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-115">Required.</span></span> <span data-ttu-id="b1aa7-116">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="b1aa7-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="b1aa7-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1aa7-117">Content-Type</span></span>    |    <span data-ttu-id="b1aa7-118">ciąg</span><span class="sxs-lookup"><span data-stu-id="b1aa7-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="b1aa7-119">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-119">**Path parameter**</span></span>

|    <span data-ttu-id="b1aa7-120">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="b1aa7-120">Parameter Name</span></span>    |    <span data-ttu-id="b1aa7-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b1aa7-121">Type</span></span>    |    <span data-ttu-id="b1aa7-122">Wymagane</span><span class="sxs-lookup"><span data-stu-id="b1aa7-122">Required</span></span>    |    <span data-ttu-id="b1aa7-123">Opis</span><span class="sxs-lookup"><span data-stu-id="b1aa7-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="b1aa7-124">reportId</span><span class="sxs-lookup"><span data-stu-id="b1aa7-124">reportId</span></span>     |    <span data-ttu-id="b1aa7-125">ciąg</span><span class="sxs-lookup"><span data-stu-id="b1aa7-125">string</span></span>    |    <span data-ttu-id="b1aa7-126">Nie</span><span class="sxs-lookup"><span data-stu-id="b1aa7-126">No</span></span>    |    <span data-ttu-id="b1aa7-127">Identyfikator modyfikowanego raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="b1aa7-128">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-128">**Query parameter**</span></span>

<span data-ttu-id="b1aa7-129">Brak</span><span class="sxs-lookup"><span data-stu-id="b1aa7-129">None</span></span>

<span data-ttu-id="b1aa7-130">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-130">**Request payload**</span></span>

<span data-ttu-id="b1aa7-131">Brak</span><span class="sxs-lookup"><span data-stu-id="b1aa7-131">None</span></span>

<span data-ttu-id="b1aa7-132">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-132">**Glossary**</span></span>

<span data-ttu-id="b1aa7-133">Brak</span><span class="sxs-lookup"><span data-stu-id="b1aa7-133">None</span></span>

<span data-ttu-id="b1aa7-134">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-134">**Response**</span></span>

<span data-ttu-id="b1aa7-135">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="b1aa7-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="b1aa7-136">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="b1aa7-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="b1aa7-137">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="b1aa7-137">Response payload example:</span></span>

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

<span data-ttu-id="b1aa7-138">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="b1aa7-138">**Glossary**</span></span>

<span data-ttu-id="b1aa7-139">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="b1aa7-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="b1aa7-140">Parametr</span><span class="sxs-lookup"><span data-stu-id="b1aa7-140">Parameter</span></span>    |    <span data-ttu-id="b1aa7-141">Opis</span><span class="sxs-lookup"><span data-stu-id="b1aa7-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b1aa7-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="b1aa7-142">ReportId</span></span>     |    <span data-ttu-id="b1aa7-143">Uniwersalny unikatowy identyfikator (UUID) wznowienia raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="b1aa7-144">Reportname</span><span class="sxs-lookup"><span data-stu-id="b1aa7-144">ReportName</span></span>     |    <span data-ttu-id="b1aa7-145">Nazwa nadana raportowi podczas tworzenia</span><span class="sxs-lookup"><span data-stu-id="b1aa7-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="b1aa7-146">Opis</span><span class="sxs-lookup"><span data-stu-id="b1aa7-146">Description</span></span>     |    <span data-ttu-id="b1aa7-147">Opis podany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="b1aa7-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="b1aa7-148">QueryId</span></span>     |    <span data-ttu-id="b1aa7-149">Identyfikator zapytania przekazany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="b1aa7-150">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="b1aa7-150">Query</span></span>     |    <span data-ttu-id="b1aa7-151">Tekst zapytania, który zostanie wykonany dla tego raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="b1aa7-152">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="b1aa7-152">User</span></span>     |    <span data-ttu-id="b1aa7-153">Identyfikator użytkownika użyty do utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="b1aa7-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="b1aa7-154">CreatedTime</span></span>     |    <span data-ttu-id="b1aa7-155">Godzina utworzenia raportu.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-155">Time the report was created.</span></span> <span data-ttu-id="b1aa7-156">Format czasu to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="b1aa7-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="b1aa7-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="b1aa7-157">ModifiedTime</span></span>     |    <span data-ttu-id="b1aa7-158">Godzina ostatniej modyfikacji raportu.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-158">Time the report was last modified.</span></span> <span data-ttu-id="b1aa7-159">Format czasu to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="b1aa7-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="b1aa7-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="b1aa7-160">ExecuteNow</span></span>     |    <span data-ttu-id="b1aa7-161">Flaga ExecuteNow ustawiona w czasie tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="b1aa7-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="b1aa7-162">StartTime</span></span>     |    <span data-ttu-id="b1aa7-163">Godzina rozpoczęcia wykonywania raportu.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-163">Time the report execution will begin.</span></span> <span data-ttu-id="b1aa7-164">Format czasu to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="b1aa7-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="b1aa7-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="b1aa7-165">ReportStatus</span></span>     |    <span data-ttu-id="b1aa7-166">Stan wykonania raportu.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-166">Status of the report execution.</span></span> <span data-ttu-id="b1aa7-167">Możliwe wartości to Wstrzymane, Aktywne i Nieaktywne.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="b1aa7-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="b1aa7-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="b1aa7-169">Interwał cyklu zapewniany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="b1aa7-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="b1aa7-170">RecurrenceCount</span></span>     |    <span data-ttu-id="b1aa7-171">Liczba cyklów zapewniana podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="b1aa7-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="b1aa7-172">CallbackUrl</span></span>     |    <span data-ttu-id="b1aa7-173">Adres URL wywołania zwrotnego podany w żądaniu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="b1aa7-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="b1aa7-174">CallbackMethod</span></span>    |    <span data-ttu-id="b1aa7-175">Metoda wywołania zwrotnego dostarczana w żądaniu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="b1aa7-176">Format</span><span class="sxs-lookup"><span data-stu-id="b1aa7-176">Format</span></span>     |    <span data-ttu-id="b1aa7-177">Format plików raportu</span><span class="sxs-lookup"><span data-stu-id="b1aa7-177">Format of the report files</span></span>     |
|    <span data-ttu-id="b1aa7-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="b1aa7-178">TotalCount</span></span>     |    <span data-ttu-id="b1aa7-179">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="b1aa7-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="b1aa7-180">Komunikat</span><span class="sxs-lookup"><span data-stu-id="b1aa7-180">Message</span></span>     |    <span data-ttu-id="b1aa7-181">Komunikat o stanie z wykonywania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="b1aa7-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="b1aa7-182">Statuscode</span><span class="sxs-lookup"><span data-stu-id="b1aa7-182">StatusCode</span></span>     |    <span data-ttu-id="b1aa7-183">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="b1aa7-183">Result Code.</span></span> <span data-ttu-id="b1aa7-184">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="b1aa7-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
