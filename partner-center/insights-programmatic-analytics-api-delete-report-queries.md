---
title: Interfejs API usuwania zapytań dotyczących raportów — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Użyj tego interfejsu API, aby usunąć zapytanie zdefiniowane przez użytkownika w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376979"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="20570-103">Interfejs API usuwania zapytań dotyczących raportów</span><span class="sxs-lookup"><span data-stu-id="20570-103">Delete report queries API</span></span>

<span data-ttu-id="20570-104">Ten interfejs API usuwa zapytania zdefiniowane przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="20570-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="20570-105">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="20570-105">**Request syntax**</span></span>

|    <span data-ttu-id="20570-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="20570-106">Method</span></span>    |    <span data-ttu-id="20570-107">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="20570-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="20570-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="20570-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="20570-109">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="20570-109">**Request header**</span></span>

|    <span data-ttu-id="20570-110">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="20570-110">Header</span></span>    |    <span data-ttu-id="20570-111">Typ</span><span class="sxs-lookup"><span data-stu-id="20570-111">Type</span></span>    |    <span data-ttu-id="20570-112">Opis</span><span class="sxs-lookup"><span data-stu-id="20570-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="20570-113">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="20570-113">Authorization</span></span>    |    <span data-ttu-id="20570-114">ciąg</span><span class="sxs-lookup"><span data-stu-id="20570-114">string</span></span>    |    <span data-ttu-id="20570-115">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="20570-115">Required.</span></span> <span data-ttu-id="20570-116">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="20570-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="20570-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20570-117">Content-Type</span></span>    |    <span data-ttu-id="20570-118">ciąg</span><span class="sxs-lookup"><span data-stu-id="20570-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="20570-119">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="20570-119">**Path parameter**</span></span>

|    <span data-ttu-id="20570-120">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="20570-120">Parameter Name</span></span>    |    <span data-ttu-id="20570-121">Typ</span><span class="sxs-lookup"><span data-stu-id="20570-121">Type</span></span>    |    <span data-ttu-id="20570-122">Wymagane</span><span class="sxs-lookup"><span data-stu-id="20570-122">Required</span></span>    |    <span data-ttu-id="20570-123">Opis</span><span class="sxs-lookup"><span data-stu-id="20570-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="20570-124">queryId</span><span class="sxs-lookup"><span data-stu-id="20570-124">queryId</span></span>     |    <span data-ttu-id="20570-125">ciąg</span><span class="sxs-lookup"><span data-stu-id="20570-125">string</span></span>     |    <span data-ttu-id="20570-126">Nie</span><span class="sxs-lookup"><span data-stu-id="20570-126">No</span></span>    |    <span data-ttu-id="20570-127">Filtruj, aby uzyskać szczegółowe informacje tylko o zapytaniach o identyfikatorze podanym w argumentze</span><span class="sxs-lookup"><span data-stu-id="20570-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="20570-128">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="20570-128">**Query parameter**</span></span>

<span data-ttu-id="20570-129">Brak</span><span class="sxs-lookup"><span data-stu-id="20570-129">None</span></span>

<span data-ttu-id="20570-130">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="20570-130">**Request payload**</span></span>

<span data-ttu-id="20570-131">Brak</span><span class="sxs-lookup"><span data-stu-id="20570-131">None</span></span>

<span data-ttu-id="20570-132">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="20570-132">**Glossary**</span></span>

<span data-ttu-id="20570-133">Brak</span><span class="sxs-lookup"><span data-stu-id="20570-133">None</span></span>

<span data-ttu-id="20570-134">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="20570-134">**Response**</span></span>

<span data-ttu-id="20570-135">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="20570-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="20570-136">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="20570-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="20570-137">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="20570-137">Response payload example:</span></span>

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

<span data-ttu-id="20570-138">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="20570-138">**Glossary**</span></span>

<span data-ttu-id="20570-139">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="20570-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="20570-140">Parametr</span><span class="sxs-lookup"><span data-stu-id="20570-140">Parameter</span></span>    |    <span data-ttu-id="20570-141">Opis</span><span class="sxs-lookup"><span data-stu-id="20570-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="20570-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="20570-142">QueryId</span></span>     |    <span data-ttu-id="20570-143">Unikatowy identyfikator UUID zapytania, które zostało usunięte</span><span class="sxs-lookup"><span data-stu-id="20570-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="20570-144">Nazwa</span><span class="sxs-lookup"><span data-stu-id="20570-144">Name</span></span>     |    <span data-ttu-id="20570-145">Nazwa zapytania, które zostało usunięte</span><span class="sxs-lookup"><span data-stu-id="20570-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="20570-146">Opis</span><span class="sxs-lookup"><span data-stu-id="20570-146">Description</span></span>     |    <span data-ttu-id="20570-147">Opis usuniętego zapytania</span><span class="sxs-lookup"><span data-stu-id="20570-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="20570-148">Zapytanie</span><span class="sxs-lookup"><span data-stu-id="20570-148">Query</span></span>     |    <span data-ttu-id="20570-149">Ciąg zapytania raportu usuniętego zapytania</span><span class="sxs-lookup"><span data-stu-id="20570-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="20570-150">Typ</span><span class="sxs-lookup"><span data-stu-id="20570-150">Type</span></span>     |    <span data-ttu-id="20570-151">Ustaw wartość userDefined dla zapytań utworzonych przez użytkownika</span><span class="sxs-lookup"><span data-stu-id="20570-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="20570-152">Użytkownik</span><span class="sxs-lookup"><span data-stu-id="20570-152">User</span></span>     |    <span data-ttu-id="20570-153">Identyfikator użytkownika, który utworzył zapytanie</span><span class="sxs-lookup"><span data-stu-id="20570-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="20570-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="20570-154">CreatedTime</span></span>     |    <span data-ttu-id="20570-155">Czas utworzenia zapytania</span><span class="sxs-lookup"><span data-stu-id="20570-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="20570-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="20570-156">TotalCount</span></span>     |    <span data-ttu-id="20570-157">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="20570-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="20570-158">Komunikat</span><span class="sxs-lookup"><span data-stu-id="20570-158">Message</span></span>     |    <span data-ttu-id="20570-159">Komunikat o stanie z wykonywania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="20570-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="20570-160">Statuscode</span><span class="sxs-lookup"><span data-stu-id="20570-160">StatusCode</span></span>     |    <span data-ttu-id="20570-161">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="20570-161">Result Code.</span></span> <span data-ttu-id="20570-162">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="20570-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
