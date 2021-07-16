---
title: Lista interfejsu API do uzyskiwania dostępu do danych szczegółowych informacji partnerów
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lista interfejsów API do uzyskiwania dostępu do danych szczegółowych informacji partnerów.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377170"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="a7ab7-103">Dostępne interfejsy API do analizy szczegółowych informacji partnerów</span><span class="sxs-lookup"><span data-stu-id="a7ab7-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="a7ab7-104">Poniżej znajduje się lista interfejsów API do analizy szczegółowych informacji partnerów i skojarzonych z nimi funkcji.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="a7ab7-105">Interfejsy API ściągania zestawu danych</span><span class="sxs-lookup"><span data-stu-id="a7ab7-105">Dataset pull APIs</span></span>

<span data-ttu-id="a7ab7-106">***Tabela 1. Interfejsy API ściągania zestawów danych***</span><span class="sxs-lookup"><span data-stu-id="a7ab7-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="a7ab7-107">**Interfejs API**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-107">**API**</span></span> | <span data-ttu-id="a7ab7-108">**Funkcjonalność**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="a7ab7-109">Pobierz wszystkie zestawy danych</span><span class="sxs-lookup"><span data-stu-id="a7ab7-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="a7ab7-110">Pobiera wszystkie dostępne zestawy danych.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-110">Gets all the available datasets.</span></span> <span data-ttu-id="a7ab7-111">Zestawy danych zawierają listę tabel, kolumn, metryk i zakresów czasu.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="a7ab7-112">Interfejsy API zarządzania zapytaniami</span><span class="sxs-lookup"><span data-stu-id="a7ab7-112">Query management APIs</span></span>

<span data-ttu-id="a7ab7-113">***Tabela 2. Interfejsy API zarządzania zapytaniami***</span><span class="sxs-lookup"><span data-stu-id="a7ab7-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="a7ab7-114">**Interfejs API**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-114">**API**</span></span> | <span data-ttu-id="a7ab7-115">**Funkcjonalność**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="a7ab7-116">Tworzenie zapytania raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="a7ab7-117">Tworzy zapytania niestandardowe definiujące zestaw danych, z którego należy wyeksportować kolumny i metryki.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="a7ab7-118">ZAPYTANIE GET raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="a7ab7-119">Pobiera wszystkie zapytania dostępne do użycia w raportach.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="a7ab7-120">Domyślnie pobiera wszystkie zapytania systemowe i zdefiniowane przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="a7ab7-121">USUWANIE zapytania raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="a7ab7-122">Usuwa zapytania zdefiniowane przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="a7ab7-123">Interfejsy API zarządzania raportami</span><span class="sxs-lookup"><span data-stu-id="a7ab7-123">Report management APIs</span></span>

<span data-ttu-id="a7ab7-124">***Tabela 3. Interfejsy API zarządzania raportami***</span><span class="sxs-lookup"><span data-stu-id="a7ab7-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="a7ab7-125">**Interfejs API**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-125">**API**</span></span> | <span data-ttu-id="a7ab7-126">**Funkcjonalność**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="a7ab7-127">Tworzenie raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="a7ab7-128">Planuje wykonywanie zapytania w regularnych odstępach czasu.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="a7ab7-129">TRY Report Query</span><span class="sxs-lookup"><span data-stu-id="a7ab7-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="a7ab7-130">Wykonuje instrukcje zapytania raportu.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-130">Executes a Report query statement.</span></span> <span data-ttu-id="a7ab7-131">Zwraca tylko 10 rekordów, których partner może użyć do sprawdzenia, czy dane są zgodnie z oczekiwaniami.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="a7ab7-132">Pobierz raport</span><span class="sxs-lookup"><span data-stu-id="a7ab7-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="a7ab7-133">Pobierz wszystkie raporty, które zostały zaplanowane.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="a7ab7-134">Aktualizowanie raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="a7ab7-135">Modyfikowanie parametru raportu.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="a7ab7-136">Usuwanie raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="a7ab7-137">Usuwa wszystkie rekordy wykonywania raportu i raportu.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="a7ab7-138">Wstrzymywanie wykonań raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="a7ab7-139">Wstrzymuje zaplanowane wykonywanie raportów.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="a7ab7-140">Wznawianie wykonywania raportów</span><span class="sxs-lookup"><span data-stu-id="a7ab7-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="a7ab7-141">Wznawia zaplanowane wykonywanie wstrzymanego raportu.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="a7ab7-142">Interfejsy API ściągania wykonywania raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-142">Report execution pull APIs</span></span>

<span data-ttu-id="a7ab7-143">***Tabela 4. Interfejsy API ściągania wykonywania raportu***</span><span class="sxs-lookup"><span data-stu-id="a7ab7-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="a7ab7-144">**Interfejs API**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-144">**API**</span></span> | <span data-ttu-id="a7ab7-145">**Funkcjonalność**</span><span class="sxs-lookup"><span data-stu-id="a7ab7-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="a7ab7-146">Uzyskiwanie wykonań raportu</span><span class="sxs-lookup"><span data-stu-id="a7ab7-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="a7ab7-147">Pobierz wszystkie wykonania, które miały miejsce dla danego raportu.</span><span class="sxs-lookup"><span data-stu-id="a7ab7-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="a7ab7-148">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="a7ab7-148">Next steps</span></span>

- <span data-ttu-id="a7ab7-149">Interfejsy API można wypróbować za pomocą adresu URL interfejsu [API swagger.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="a7ab7-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>