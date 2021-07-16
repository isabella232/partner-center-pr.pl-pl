---
title: Interfejs API pobierz wszystkie zestawy danych — Szczegółowe informacje danych
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ten interfejs API umożliwia uzyskiwanie szczegółowych informacji o wszystkich dostępnych zestawach danych Partner Center szczegółowych informacji.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376958"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="c4a56-103">Interfejs API pobierz wszystkie zestawy danych</span><span class="sxs-lookup"><span data-stu-id="c4a56-103">Get all datasets API</span></span>

<span data-ttu-id="c4a56-104">Interfejs API Pobierz wszystkie zestawy danych pobiera wszystkie dostępne zestawy danych.</span><span class="sxs-lookup"><span data-stu-id="c4a56-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="c4a56-105">Zestawy danych zawierają listę tabel, kolumn, metryk i zakresów czasu.</span><span class="sxs-lookup"><span data-stu-id="c4a56-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="c4a56-106">**Składnia żądania**</span><span class="sxs-lookup"><span data-stu-id="c4a56-106">**Request syntax**</span></span>

|    <span data-ttu-id="c4a56-107">Metoda</span><span class="sxs-lookup"><span data-stu-id="c4a56-107">Method</span></span>    |    <span data-ttu-id="c4a56-108">Identyfikator URI żądania</span><span class="sxs-lookup"><span data-stu-id="c4a56-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c4a56-109">GET</span><span class="sxs-lookup"><span data-stu-id="c4a56-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="c4a56-110">**Nagłówek żądania**</span><span class="sxs-lookup"><span data-stu-id="c4a56-110">**Request header**</span></span>

|    <span data-ttu-id="c4a56-111">Nagłówek</span><span class="sxs-lookup"><span data-stu-id="c4a56-111">Header</span></span>    |    <span data-ttu-id="c4a56-112">Typ</span><span class="sxs-lookup"><span data-stu-id="c4a56-112">Type</span></span>    |    <span data-ttu-id="c4a56-113">Opis</span><span class="sxs-lookup"><span data-stu-id="c4a56-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="c4a56-114">Autoryzacja</span><span class="sxs-lookup"><span data-stu-id="c4a56-114">Authorization</span></span>    |    <span data-ttu-id="c4a56-115">ciąg</span><span class="sxs-lookup"><span data-stu-id="c4a56-115">string</span></span>    |    <span data-ttu-id="c4a56-116">Wymagane.</span><span class="sxs-lookup"><span data-stu-id="c4a56-116">Required.</span></span> <span data-ttu-id="c4a56-117">Token Azure Active Directory (AAD) w formularzu`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="c4a56-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="c4a56-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4a56-118">Content-Type</span></span>    |    <span data-ttu-id="c4a56-119">ciąg</span><span class="sxs-lookup"><span data-stu-id="c4a56-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="c4a56-120">**Parametr ścieżki**</span><span class="sxs-lookup"><span data-stu-id="c4a56-120">**Path parameter**</span></span>

<span data-ttu-id="c4a56-121">Brak</span><span class="sxs-lookup"><span data-stu-id="c4a56-121">None</span></span>

<span data-ttu-id="c4a56-122">**Parametr zapytania**</span><span class="sxs-lookup"><span data-stu-id="c4a56-122">**Query parameter**</span></span>

|    <span data-ttu-id="c4a56-123">Nazwa parametru</span><span class="sxs-lookup"><span data-stu-id="c4a56-123">Parameter Name</span></span>    |    <span data-ttu-id="c4a56-124">Typ</span><span class="sxs-lookup"><span data-stu-id="c4a56-124">Type</span></span>    |    <span data-ttu-id="c4a56-125">Wymagane</span><span class="sxs-lookup"><span data-stu-id="c4a56-125">Required</span></span>    |    <span data-ttu-id="c4a56-126">Opis</span><span class="sxs-lookup"><span data-stu-id="c4a56-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="c4a56-127">Datasetname</span><span class="sxs-lookup"><span data-stu-id="c4a56-127">datasetName</span></span>    |    <span data-ttu-id="c4a56-128">ciąg</span><span class="sxs-lookup"><span data-stu-id="c4a56-128">string</span></span>    |    <span data-ttu-id="c4a56-129">Nie</span><span class="sxs-lookup"><span data-stu-id="c4a56-129">No</span></span>    |    <span data-ttu-id="c4a56-130">Filtrowanie w celu uzyskania szczegółów tylko jednego zestawu danych</span><span class="sxs-lookup"><span data-stu-id="c4a56-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="c4a56-131">**Ładunek żądania**</span><span class="sxs-lookup"><span data-stu-id="c4a56-131">**Request payload**</span></span>

<span data-ttu-id="c4a56-132">Brak</span><span class="sxs-lookup"><span data-stu-id="c4a56-132">None</span></span>

<span data-ttu-id="c4a56-133">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="c4a56-133">**Glossary**</span></span>

<span data-ttu-id="c4a56-134">Brak</span><span class="sxs-lookup"><span data-stu-id="c4a56-134">None</span></span>

<span data-ttu-id="c4a56-135">**Odpowiedź**</span><span class="sxs-lookup"><span data-stu-id="c4a56-135">**Response**</span></span>

<span data-ttu-id="c4a56-136">Ładunek odpowiedzi ma następującą strukturę:</span><span class="sxs-lookup"><span data-stu-id="c4a56-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="c4a56-137">Kod odpowiedzi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="c4a56-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="c4a56-138">Przykład ładunku odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="c4a56-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="c4a56-139">**Słownik**</span><span class="sxs-lookup"><span data-stu-id="c4a56-139">**Glossary**</span></span>

<span data-ttu-id="c4a56-140">W tej tabeli zdefiniowano kluczowe elementy odpowiedzi:</span><span class="sxs-lookup"><span data-stu-id="c4a56-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="c4a56-141">Parametr</span><span class="sxs-lookup"><span data-stu-id="c4a56-141">Parameter</span></span>    |    <span data-ttu-id="c4a56-142">Opis</span><span class="sxs-lookup"><span data-stu-id="c4a56-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c4a56-143">Datasetname</span><span class="sxs-lookup"><span data-stu-id="c4a56-143">DatasetName</span></span>     |    <span data-ttu-id="c4a56-144">Nazwa zestawu danych, który definiuje ten obiekt tablicy</span><span class="sxs-lookup"><span data-stu-id="c4a56-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="c4a56-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="c4a56-145">SelectableColumns</span></span>     |    <span data-ttu-id="c4a56-146">Nieprzetworzone kolumny, które można określić w wybranych kolumnach</span><span class="sxs-lookup"><span data-stu-id="c4a56-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="c4a56-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="c4a56-147">AvailableMetrics</span></span>     |    <span data-ttu-id="c4a56-148">Nazwy kolumn agregacji/metryk, które można określić w wybranych kolumnach</span><span class="sxs-lookup"><span data-stu-id="c4a56-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="c4a56-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="c4a56-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="c4a56-150">Zakres dat, który może być używany w zapytaniach dotyczących raportu dla zestawu danych</span><span class="sxs-lookup"><span data-stu-id="c4a56-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="c4a56-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="c4a56-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="c4a56-152">Minimalna wartość interwału cyklu</span><span class="sxs-lookup"><span data-stu-id="c4a56-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="c4a56-153">Łączna liczba</span><span class="sxs-lookup"><span data-stu-id="c4a56-153">TotalCount</span></span>     |    <span data-ttu-id="c4a56-154">Liczba zestawów danych w tablicy Value</span><span class="sxs-lookup"><span data-stu-id="c4a56-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="c4a56-155">Komunikat</span><span class="sxs-lookup"><span data-stu-id="c4a56-155">Message</span></span>     |    <span data-ttu-id="c4a56-156">Komunikat o stanie z wykonania interfejsu API</span><span class="sxs-lookup"><span data-stu-id="c4a56-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="c4a56-157">Statuscode</span><span class="sxs-lookup"><span data-stu-id="c4a56-157">StatusCode</span></span>     |    <span data-ttu-id="c4a56-158">Kod wyniku.</span><span class="sxs-lookup"><span data-stu-id="c4a56-158">Result Code.</span></span> <span data-ttu-id="c4a56-159">Możliwe wartości to 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="c4a56-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
