---
title: Lista interfejsu API do uzyskiwania dostępu do danych szczegółowych informacji partnerów
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Lista interfejsów API do uzyskiwania dostępu do danych szczegółowych informacji partnerów.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 19c3094300e0d6c6f774117156cb6e26d80a0f22190c9736b12dd264178d6d7c
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115692419"
---
# <a name="available-apis-for-partner-insights-analytics"></a>Dostępne interfejsy API do analizy szczegółowych informacji partnerów

Poniżej znajduje się lista interfejsów API do analizy szczegółowych informacji partnerów i skojarzonych z nimi funkcji.

## <a name="dataset-pull-apis"></a>Interfejsy API ściągania zestawu danych

***Tabela 1. Interfejsy API ściągania zestawów danych***

| **Interfejs API** | **Funkcjonalność** |
| --- | --- |
| [Pobierz wszystkie zestawy danych](insights-programmatic-analytics-api-get-dataset.md) | Pobiera wszystkie dostępne zestawy danych. Zestawy danych zawierają listę tabel, kolumn, metryk i zakresów czasu. |
|||

## <a name="query-management-apis"></a>Interfejsy API zarządzania zapytaniami

***Tabela 2. Interfejsy API zarządzania zapytaniami***

| **Interfejs API** | **Funkcjonalność** |
| --- | --- |
| [Tworzenie zapytania raportu](insights-programmatic-access-paradigm.md#create-report-query-api) | Tworzy zapytania niestandardowe definiujące zestaw danych, z którego należy wyeksportować kolumny i metryki. |
| [GET Report Query](insights-programmatic-analytics-api-get-report-queries.md) | Pobiera wszystkie zapytania dostępne do użycia w raportach. Domyślnie pobiera wszystkie zapytania systemowe i zdefiniowane przez użytkownika. |
| [USUWANIE zapytania raportu](insights-programmatic-analytics-api-delete-report-queries.md) | Usuwa zapytania zdefiniowane przez użytkownika. |
|||

## <a name="report-management-apis"></a>Interfejsy API zarządzania raportami

***Tabela 3. Interfejsy API zarządzania raportami***

| **Interfejs API** | **Funkcjonalność** |
| --- | --- |
| [Tworzenie raportu](insights-programmatic-access-paradigm.md#create-report-api) | Planuje wykonywanie zapytania w regularnych odstępach czasu. |
| [TRY Report Query](insights-programmatic-analytics-api-try-report-queries.md) | Wykonuje instrukcje zapytania raportu. Zwraca tylko 10 rekordów, których partner może użyć do sprawdzenia, czy dane są zgodnie z oczekiwaniami. |
| [Pobierz raport](insights-programmatic-analytics-api-get-report.md) | Pobierz wszystkie raporty, które zostały zaplanowane. |
| [Aktualizowanie raportu](insights-programmatic-analytics-api-update-report.md) | Modyfikowanie parametru raportu. |
| [Usuwanie raportu](insights-programmatic-analytics-api-delete-report.md) | Usuwa wszystkie rekordy wykonywania raportu i raportu. |
| [Wstrzymywanie wykonań raportu](insights-programmatic-analytics-api-pause-report-executions.md) | Wstrzymuje zaplanowane wykonywanie raportów. |
| [Wznawianie wykonywania raportów](insights-programmatic-analytics-api-resume-report-executions.md) | Wznawia zaplanowane wykonywanie wstrzymanego raportu. |
|||

## <a name="report-execution-pull-apis"></a>Interfejsy API ściągania wykonywania raportu

***Tabela 4. Interfejsy API ściągania wykonywania raportu***

| **Interfejs API** | **Funkcjonalność** |
| --- | --- |
| [Uzyskiwanie wykonań raportu](insights-programmatic-access-paradigm.md#get-report-execution-api) | Pobierz wszystkie wykonania, które miały miejsce dla danego raportu. |
|||

## <a name="next-steps"></a>Następne kroki

- Interfejsy API można wypróbować za pomocą adresu URL interfejsu [API swagger.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)