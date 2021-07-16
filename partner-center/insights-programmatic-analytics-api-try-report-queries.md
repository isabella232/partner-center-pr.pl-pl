---
title: Wypróbuj interfejs API zapytań dotyczących raportów
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ten interfejs API umożliwia przetestowanie zapytania i zweryfikowanie wyników w Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377182"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="b0abc-103">Wypróbuj interfejs API zapytań dotyczących raportów</span><span class="sxs-lookup"><span data-stu-id="b0abc-103">Try report queries API</span></span>

<span data-ttu-id="b0abc-104">Ten interfejs API wykonuje instrukcje zapytania raportu.</span><span class="sxs-lookup"><span data-stu-id="b0abc-104">This API executes a Report query statement.</span></span> <span data-ttu-id="b0abc-105">Interfejs API zwraca tylko 100 rekordów, których partner może użyć do sprawdzenia, czy dane są zgodnie z oczekiwaniami.</span><span class="sxs-lookup"><span data-stu-id="b0abc-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b0abc-106">Ten interfejs API ma limit czasu wykonywania zapytania 100 sekund.</span><span class="sxs-lookup"><span data-stu-id="b0abc-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="b0abc-107">Jeśli zauważysz, że interfejs API trwa dłużej niż 100 sekund, istnieje duże prawdopodobieństwo, że zapytanie ma poprawną synaktywną odpowiedź. W innym przypadku zostałby odebrany kod błędu inny niż 200.</span><span class="sxs-lookup"><span data-stu-id="b0abc-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="b0abc-108">Rzeczywiste generowanie raportu zostanie przebiegło, jeśli składnia zapytania jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="b0abc-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="b0abc-109">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="b0abc-109">**Request syntax**</span></span>

|    <span data-ttu-id="b0abc-110">Metoda</span><span class="sxs-lookup"><span data-stu-id="b0abc-110">Method</span></span>    |    <span data-ttu-id="b0abc-111">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="b0abc-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b0abc-112">GET</span><span class="sxs-lookup"><span data-stu-id="b0abc-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="b0abc-113">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="b0abc-113">**Request header**</span></span>

|    <span data-ttu-id="b0abc-114">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="b0abc-114">Header</span></span>    |    <span data-ttu-id="b0abc-115">Typ</span><span class="sxs-lookup"><span data-stu-id="b0abc-115">Type</span></span>    |    <span data-ttu-id="b0abc-116">Opis</span><span class="sxs-lookup"><span data-stu-id="b0abc-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="b0abc-117">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="b0abc-117">Authorization</span></span>    |    <span data-ttu-id="b0abc-118">ciąg</span><span class="sxs-lookup"><span data-stu-id="b0abc-118">string</span></span>    |    <span data-ttu-id="b0abc-119">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="b0abc-119">Required.</span></span> <span data-ttu-id="b0abc-120">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="b0abc-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="b0abc-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0abc-121">Content-Type</span></span>    |    <span data-ttu-id="b0abc-122">ciąg</span><span class="sxs-lookup"><span data-stu-id="b0abc-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="b0abc-123">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="b0abc-123">**Path parameter**</span></span>

<span data-ttu-id="b0abc-124">Brak</span><span class="sxs-lookup"><span data-stu-id="b0abc-124">None</span></span>

<span data-ttu-id="b0abc-125">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="b0abc-125">**Query parameter**</span></span>

|    <span data-ttu-id="b0abc-126">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="b0abc-126">Parameter Name</span></span>    |    <span data-ttu-id="b0abc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b0abc-127">Type</span></span>    |    <span data-ttu-id="b0abc-128">Wymagane</span><span class="sxs-lookup"><span data-stu-id="b0abc-128">Required</span></span>    |    <span data-ttu-id="b0abc-129">Opis</span><span class="sxs-lookup"><span data-stu-id="b0abc-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="b0abc-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="b0abc-130">exportQuery</span></span>     |    <span data-ttu-id="b0abc-131">ciąg</span><span class="sxs-lookup"><span data-stu-id="b0abc-131">string</span></span>    |    <span data-ttu-id="b0abc-132">Nie</span><span class="sxs-lookup"><span data-stu-id="b0abc-132">No</span></span>    |    <span data-ttu-id="b0abc-133">Ciąg zapytania raportu, który musi zostać wykonany</span><span class="sxs-lookup"><span data-stu-id="b0abc-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="b0abc-134">queryId</span><span class="sxs-lookup"><span data-stu-id="b0abc-134">queryId</span></span>     |    <span data-ttu-id="b0abc-135">ciąg</span><span class="sxs-lookup"><span data-stu-id="b0abc-135">string</span></span>    |    <span data-ttu-id="b0abc-136">Nie</span><span class="sxs-lookup"><span data-stu-id="b0abc-136">No</span></span>    |    <span data-ttu-id="b0abc-137">Prawidłowy istniejący identyfikator zapytania.</span><span class="sxs-lookup"><span data-stu-id="b0abc-137">A valid existing query ID.</span></span> <span data-ttu-id="b0abc-138">Wzajemnie wykluczają się z ciągiem zapytania określonym w parametrze exportQuery</span><span class="sxs-lookup"><span data-stu-id="b0abc-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="b0abc-139">startTime</span><span class="sxs-lookup"><span data-stu-id="b0abc-139">startTime</span></span>     |    <span data-ttu-id="b0abc-140">ciąg</span><span class="sxs-lookup"><span data-stu-id="b0abc-140">string</span></span>    |    <span data-ttu-id="b0abc-141">Nie</span><span class="sxs-lookup"><span data-stu-id="b0abc-141">No</span></span>    |    <span data-ttu-id="b0abc-142">Godzina rozpoczęcia, z której chcemy uzyskać dane.</span><span class="sxs-lookup"><span data-stu-id="b0abc-142">Start time from which we want the data.</span></span> <span data-ttu-id="b0abc-143">Zastępuje on przedziale czasu określonym w zapytaniu</span><span class="sxs-lookup"><span data-stu-id="b0abc-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="b0abc-144">endTime</span><span class="sxs-lookup"><span data-stu-id="b0abc-144">endTime</span></span>     |    <span data-ttu-id="b0abc-145">ciąg</span><span class="sxs-lookup"><span data-stu-id="b0abc-145">string</span></span>    |    <span data-ttu-id="b0abc-146">Nie</span><span class="sxs-lookup"><span data-stu-id="b0abc-146">No</span></span>    |    <span data-ttu-id="b0abc-147">Czas zakończenia, do którego chcemy uzyskać dane.</span><span class="sxs-lookup"><span data-stu-id="b0abc-147">End time till which we want the data.</span></span> <span data-ttu-id="b0abc-148">Zastępuje on przedziale czasu określonym w zapytaniu</span><span class="sxs-lookup"><span data-stu-id="b0abc-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="b0abc-149">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="b0abc-149">**Request payload**</span></span>

<span data-ttu-id="b0abc-150">Brak</span><span class="sxs-lookup"><span data-stu-id="b0abc-150">None</span></span>

<span data-ttu-id="b0abc-151">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="b0abc-151">**Glossary**</span></span>

<span data-ttu-id="b0abc-152">Brak</span><span class="sxs-lookup"><span data-stu-id="b0abc-152">None</span></span>

<span data-ttu-id="b0abc-153">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="b0abc-153">**Response**</span></span>

<span data-ttu-id="b0abc-154">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="b0abc-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="b0abc-155">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="b0abc-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="b0abc-156">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="b0abc-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="b0abc-157">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="b0abc-157">**Glossary**</span></span>

<span data-ttu-id="b0abc-158">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="b0abc-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="b0abc-159">Parametr</span><span class="sxs-lookup"><span data-stu-id="b0abc-159">Parameter</span></span>    |    <span data-ttu-id="b0abc-160">Opis</span><span class="sxs-lookup"><span data-stu-id="b0abc-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b0abc-161">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="b0abc-161">TotalCount</span></span>     |    <span data-ttu-id="b0abc-162">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="b0abc-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="b0abc-163">Komunikat</span><span class="sxs-lookup"><span data-stu-id="b0abc-163">Message</span></span>     |    <span data-ttu-id="b0abc-164">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="b0abc-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="b0abc-165">Statuscode</span><span class="sxs-lookup"><span data-stu-id="b0abc-165">StatusCode</span></span>     |    <span data-ttu-id="b0abc-166">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="b0abc-166">Result Code.</span></span> <span data-ttu-id="b0abc-167">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="b0abc-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
