---
title: Interfejs API get report queries — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ten interfejs API umożliwia uzyskiwanie wszystkich dostępnych zapytań do użycia w interfejsie API raportów.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377206"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="c5870-103">Interfejs API pobierz zapytania dotyczące raportów</span><span class="sxs-lookup"><span data-stu-id="c5870-103">Get report queries API</span></span>

<span data-ttu-id="c5870-104">Interfejs API get report queries pobiera wszystkie zapytania, które są dostępne do użycia w raportach.</span><span class="sxs-lookup"><span data-stu-id="c5870-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="c5870-105">Domyślnie pobiera wszystkie zapytania systemowe i zdefiniowane przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c5870-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="c5870-106">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="c5870-106">**Request syntax**</span></span>

|    <span data-ttu-id="c5870-107">Metoda</span><span class="sxs-lookup"><span data-stu-id="c5870-107">Method</span></span>    |    <span data-ttu-id="c5870-108">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="c5870-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c5870-109">GET</span><span class="sxs-lookup"><span data-stu-id="c5870-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="c5870-110">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="c5870-110">**Request header**</span></span>

|    <span data-ttu-id="c5870-111">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="c5870-111">Header</span></span>    |    <span data-ttu-id="c5870-112">Typ</span><span class="sxs-lookup"><span data-stu-id="c5870-112">Type</span></span>    |    <span data-ttu-id="c5870-113">Opis</span><span class="sxs-lookup"><span data-stu-id="c5870-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="c5870-114">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="c5870-114">Authorization</span></span>    |    <span data-ttu-id="c5870-115">ciąg</span><span class="sxs-lookup"><span data-stu-id="c5870-115">string</span></span>    |    <span data-ttu-id="c5870-116">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="c5870-116">Required.</span></span> <span data-ttu-id="c5870-117">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="c5870-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="c5870-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5870-118">Content-Type</span></span>    |    <span data-ttu-id="c5870-119">ciąg</span><span class="sxs-lookup"><span data-stu-id="c5870-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="c5870-120">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="c5870-120">**Path parameter**</span></span>

<span data-ttu-id="c5870-121">Brak</span><span class="sxs-lookup"><span data-stu-id="c5870-121">None</span></span>

<span data-ttu-id="c5870-122">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="c5870-122">**Query parameter**</span></span>

|    <span data-ttu-id="c5870-123">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="c5870-123">Parameter Name</span></span>    |    <span data-ttu-id="c5870-124">Typ</span><span class="sxs-lookup"><span data-stu-id="c5870-124">Type</span></span>    |    <span data-ttu-id="c5870-125">Wymagane</span><span class="sxs-lookup"><span data-stu-id="c5870-125">Required</span></span>    |    <span data-ttu-id="c5870-126">Opis</span><span class="sxs-lookup"><span data-stu-id="c5870-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="c5870-127">queryId</span><span class="sxs-lookup"><span data-stu-id="c5870-127">queryId</span></span>     |    <span data-ttu-id="c5870-128">ciąg</span><span class="sxs-lookup"><span data-stu-id="c5870-128">string</span></span>     |    <span data-ttu-id="c5870-129">Nie</span><span class="sxs-lookup"><span data-stu-id="c5870-129">No</span></span>    |    <span data-ttu-id="c5870-130">Filtrowanie w celu uzyskania szczegółów tylko zapytań o identyfikatorze podanym w argumentze</span><span class="sxs-lookup"><span data-stu-id="c5870-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="c5870-131">nazwa_zapytania</span><span class="sxs-lookup"><span data-stu-id="c5870-131">queryName</span></span>     |    <span data-ttu-id="c5870-132">ciąg</span><span class="sxs-lookup"><span data-stu-id="c5870-132">string</span></span>     |    <span data-ttu-id="c5870-133">Nie</span><span class="sxs-lookup"><span data-stu-id="c5870-133">No</span></span>    |    <span data-ttu-id="c5870-134">Filtrowanie w celu uzyskania szczegółów tylko zapytań o nazwie podanej w argumentze</span><span class="sxs-lookup"><span data-stu-id="c5870-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="c5870-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="c5870-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="c5870-136">boolean</span><span class="sxs-lookup"><span data-stu-id="c5870-136">boolean</span></span>     |    <span data-ttu-id="c5870-137">Nie</span><span class="sxs-lookup"><span data-stu-id="c5870-137">No</span></span>    |    <span data-ttu-id="c5870-138">Uwzględnianie wstępnie zdefiniowanych zapytań systemowych w odpowiedzi</span><span class="sxs-lookup"><span data-stu-id="c5870-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="c5870-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="c5870-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="c5870-140">boolean</span><span class="sxs-lookup"><span data-stu-id="c5870-140">boolean</span></span>     |    <span data-ttu-id="c5870-141">Nie</span><span class="sxs-lookup"><span data-stu-id="c5870-141">No</span></span>    |    <span data-ttu-id="c5870-142">Uwzględnianie w odpowiedzi tylko zapytań systemowych</span><span class="sxs-lookup"><span data-stu-id="c5870-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="c5870-143">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="c5870-143">**Request payload**</span></span>

<span data-ttu-id="c5870-144">Brak</span><span class="sxs-lookup"><span data-stu-id="c5870-144">None</span></span>

<span data-ttu-id="c5870-145">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="c5870-145">**Glossary**</span></span>

<span data-ttu-id="c5870-146">Brak</span><span class="sxs-lookup"><span data-stu-id="c5870-146">None</span></span>

<span data-ttu-id="c5870-147">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="c5870-147">**Response**</span></span>

<span data-ttu-id="c5870-148">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="c5870-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="c5870-149">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="c5870-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="c5870-150">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="c5870-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="c5870-151">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="c5870-151">**Glossary**</span></span>

<span data-ttu-id="c5870-152">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="c5870-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="c5870-153">Parametr</span><span class="sxs-lookup"><span data-stu-id="c5870-153">Parameter</span></span>    |    <span data-ttu-id="c5870-154">Opis</span><span class="sxs-lookup"><span data-stu-id="c5870-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c5870-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="c5870-155">QueryId</span></span>     |    <span data-ttu-id="c5870-156">Unikatowy identyfikator UUID zapytania</span><span class="sxs-lookup"><span data-stu-id="c5870-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="c5870-157">Nazwa</span><span class="sxs-lookup"><span data-stu-id="c5870-157">Name</span></span>     |    <span data-ttu-id="c5870-158">Nazwa nadana zapytaniu w czasie tworzenia zapytania</span><span class="sxs-lookup"><span data-stu-id="c5870-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="c5870-159">Opis</span><span class="sxs-lookup"><span data-stu-id="c5870-159">Description</span></span>     |    <span data-ttu-id="c5870-160">Opis podany podczas tworzenia zapytania</span><span class="sxs-lookup"><span data-stu-id="c5870-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="c5870-161">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="c5870-161">Query</span></span>     |    <span data-ttu-id="c5870-162">Ciąg zapytania raportu</span><span class="sxs-lookup"><span data-stu-id="c5870-162">Report query string</span></span>     |
|    <span data-ttu-id="c5870-163">Typ</span><span class="sxs-lookup"><span data-stu-id="c5870-163">Type</span></span>     |    <span data-ttu-id="c5870-164">Ustaw wartość userDefined dla zapytań utworzonych przez użytkownika i systemu dla wstępnie zdefiniowanych zapytań systemowych</span><span class="sxs-lookup"><span data-stu-id="c5870-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="c5870-165">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="c5870-165">User</span></span>     |    <span data-ttu-id="c5870-166">Identyfikator użytkownika, który utworzył zapytanie</span><span class="sxs-lookup"><span data-stu-id="c5870-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="c5870-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="c5870-167">CreatedTime</span></span>     |    <span data-ttu-id="c5870-168">Czas utworzenia zapytania</span><span class="sxs-lookup"><span data-stu-id="c5870-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="c5870-169">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="c5870-169">TotalCount</span></span>     |    <span data-ttu-id="c5870-170">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="c5870-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="c5870-171">Komunikat</span><span class="sxs-lookup"><span data-stu-id="c5870-171">Message</span></span>     |    <span data-ttu-id="c5870-172">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="c5870-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="c5870-173">Statuscode</span><span class="sxs-lookup"><span data-stu-id="c5870-173">StatusCode</span></span>     |    <span data-ttu-id="c5870-174">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="c5870-174">Result Code.</span></span> <span data-ttu-id="c5870-175">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="c5870-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
