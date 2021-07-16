---
title: Usuwanie interfejsu API raportu — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Użyj tego interfejsu API, aby usunąć dowolny raport w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377215"
---
# <a name="delete-report-api"></a><span data-ttu-id="ea89d-103">Usuwanie interfejsu API raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-103">Delete report API</span></span>

<span data-ttu-id="ea89d-104">Podczas wykonywania ten interfejs API usuwa wszystkie rekordy wykonywania raportu i raportu.</span><span class="sxs-lookup"><span data-stu-id="ea89d-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="ea89d-105">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="ea89d-105">**Request syntax**</span></span>

|    <span data-ttu-id="ea89d-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="ea89d-106">Method</span></span>    |    <span data-ttu-id="ea89d-107">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="ea89d-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ea89d-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="ea89d-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="ea89d-109">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="ea89d-109">**Request header**</span></span>

|    <span data-ttu-id="ea89d-110">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="ea89d-110">Header</span></span>    |    <span data-ttu-id="ea89d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ea89d-111">Type</span></span>    |    <span data-ttu-id="ea89d-112">Opis</span><span class="sxs-lookup"><span data-stu-id="ea89d-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="ea89d-113">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="ea89d-113">Authorization</span></span>    |    <span data-ttu-id="ea89d-114">ciąg</span><span class="sxs-lookup"><span data-stu-id="ea89d-114">string</span></span>    |    <span data-ttu-id="ea89d-115">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="ea89d-115">Required.</span></span> <span data-ttu-id="ea89d-116">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="ea89d-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="ea89d-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea89d-117">Content-Type</span></span>    |    <span data-ttu-id="ea89d-118">ciąg</span><span class="sxs-lookup"><span data-stu-id="ea89d-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="ea89d-119">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="ea89d-119">**Path parameter**</span></span>

|    <span data-ttu-id="ea89d-120">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="ea89d-120">Parameter Name</span></span>    |    <span data-ttu-id="ea89d-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ea89d-121">Type</span></span>    |    <span data-ttu-id="ea89d-122">Wymagane</span><span class="sxs-lookup"><span data-stu-id="ea89d-122">Required</span></span>    |    <span data-ttu-id="ea89d-123">Opis</span><span class="sxs-lookup"><span data-stu-id="ea89d-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ea89d-124">reportId</span><span class="sxs-lookup"><span data-stu-id="ea89d-124">reportId</span></span>     |    <span data-ttu-id="ea89d-125">ciąg</span><span class="sxs-lookup"><span data-stu-id="ea89d-125">string</span></span>    |    <span data-ttu-id="ea89d-126">Nie</span><span class="sxs-lookup"><span data-stu-id="ea89d-126">No</span></span>    |    <span data-ttu-id="ea89d-127">Identyfikator usuwanego raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="ea89d-128">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="ea89d-128">**Query parameter**</span></span>

<span data-ttu-id="ea89d-129">Brak</span><span class="sxs-lookup"><span data-stu-id="ea89d-129">None</span></span>

<span data-ttu-id="ea89d-130">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="ea89d-130">**Request payload**</span></span>

<span data-ttu-id="ea89d-131">Brak</span><span class="sxs-lookup"><span data-stu-id="ea89d-131">None</span></span>

<span data-ttu-id="ea89d-132">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="ea89d-132">**Glossary**</span></span>

<span data-ttu-id="ea89d-133">Brak</span><span class="sxs-lookup"><span data-stu-id="ea89d-133">None</span></span>

<span data-ttu-id="ea89d-134">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="ea89d-134">**Response**</span></span>

<span data-ttu-id="ea89d-135">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="ea89d-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="ea89d-136">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ea89d-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ea89d-137">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="ea89d-137">Response payload example:</span></span>

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

<span data-ttu-id="ea89d-138">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="ea89d-138">**Glossary**</span></span>

<span data-ttu-id="ea89d-139">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="ea89d-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="ea89d-140">Parametr</span><span class="sxs-lookup"><span data-stu-id="ea89d-140">Parameter</span></span>    |    <span data-ttu-id="ea89d-141">Opis</span><span class="sxs-lookup"><span data-stu-id="ea89d-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ea89d-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="ea89d-142">ReportId</span></span>     |    <span data-ttu-id="ea89d-143">Uniwersalnie unikatowy identyfikator (UUID) usuniętego raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="ea89d-144">Reportname</span><span class="sxs-lookup"><span data-stu-id="ea89d-144">ReportName</span></span>     |    <span data-ttu-id="ea89d-145">Nazwa nadana raportowi podczas tworzenia</span><span class="sxs-lookup"><span data-stu-id="ea89d-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="ea89d-146">Opis</span><span class="sxs-lookup"><span data-stu-id="ea89d-146">Description</span></span>     |    <span data-ttu-id="ea89d-147">Opis podany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="ea89d-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="ea89d-148">QueryId</span></span>     |    <span data-ttu-id="ea89d-149">Identyfikator zapytania przekazany w momencie utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="ea89d-150">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="ea89d-150">Query</span></span>     |    <span data-ttu-id="ea89d-151">Tekst zapytania, który zostanie wykonany dla tego raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="ea89d-152">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="ea89d-152">User</span></span>     |    <span data-ttu-id="ea89d-153">Identyfikator użytkownika użyty do utworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="ea89d-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ea89d-154">CreatedTime</span></span>     |    <span data-ttu-id="ea89d-155">Godzina utworzenia raportu.</span><span class="sxs-lookup"><span data-stu-id="ea89d-155">Time the report was created.</span></span> <span data-ttu-id="ea89d-156">Format godziny to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ea89d-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ea89d-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ea89d-157">ModifiedTime</span></span>     |    <span data-ttu-id="ea89d-158">Godzina ostatniej modyfikacji raportu.</span><span class="sxs-lookup"><span data-stu-id="ea89d-158">Time the report was last modified.</span></span> <span data-ttu-id="ea89d-159">Format godziny to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ea89d-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ea89d-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="ea89d-160">ExecuteNow</span></span>     |    <span data-ttu-id="ea89d-161">Flaga ExecuteNow ustawiona w czasie tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="ea89d-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="ea89d-162">StartTime</span></span>     |    <span data-ttu-id="ea89d-163">Czas rozpoczęcia wykonywania raportu.</span><span class="sxs-lookup"><span data-stu-id="ea89d-163">Time the report execution will begin.</span></span> <span data-ttu-id="ea89d-164">Format godziny to yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ea89d-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ea89d-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="ea89d-165">ReportStatus</span></span>     |    <span data-ttu-id="ea89d-166">Stan wykonania raportu.</span><span class="sxs-lookup"><span data-stu-id="ea89d-166">Status of the report execution.</span></span> <span data-ttu-id="ea89d-167">Możliwe wartości to Wstrzymane, Aktywne i Nieaktywne.</span><span class="sxs-lookup"><span data-stu-id="ea89d-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="ea89d-168">CyklInterval</span><span class="sxs-lookup"><span data-stu-id="ea89d-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="ea89d-169">Interwał cyklu zapewniany podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="ea89d-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="ea89d-170">RecurrenceCount</span></span>     |    <span data-ttu-id="ea89d-171">Liczba cyklów zapewniana podczas tworzenia raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="ea89d-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="ea89d-172">CallbackUrl</span></span>     |    <span data-ttu-id="ea89d-173">Adres URL wywołania zwrotnego podany w żądaniu</span><span class="sxs-lookup"><span data-stu-id="ea89d-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="ea89d-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="ea89d-174">CallbackMethod</span></span>    |    <span data-ttu-id="ea89d-175">Metoda wywołania zwrotnego podana w żądaniu</span><span class="sxs-lookup"><span data-stu-id="ea89d-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="ea89d-176">Format</span><span class="sxs-lookup"><span data-stu-id="ea89d-176">Format</span></span>     |    <span data-ttu-id="ea89d-177">Format plików raportu</span><span class="sxs-lookup"><span data-stu-id="ea89d-177">Format of the report files</span></span>     |
|    <span data-ttu-id="ea89d-178">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="ea89d-178">TotalCount</span></span>     |    <span data-ttu-id="ea89d-179">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="ea89d-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ea89d-180">Komunikat</span><span class="sxs-lookup"><span data-stu-id="ea89d-180">Message</span></span>     |    <span data-ttu-id="ea89d-181">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="ea89d-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="ea89d-182">Statuscode</span><span class="sxs-lookup"><span data-stu-id="ea89d-182">StatusCode</span></span>     |    <span data-ttu-id="ea89d-183">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="ea89d-183">Result Code.</span></span> <span data-ttu-id="ea89d-184">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ea89d-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
