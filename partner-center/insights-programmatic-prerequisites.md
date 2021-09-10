---
title: Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych
description: Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 12c466cce37ac252fedf5f72ef90e390bb1af256
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958965"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych

**Odpowiednie role:** Administrator globalny | Administrator programu MPN

Aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji dla partnerów, należy spełnić następujące wymagania.

## <a name="mpn-program-enrollment"></a>Rejestracja w programie MPN

Aby programowo uzyskać dostęp do danych analizy szczegółowych informacji partnera, musisz być zarejestrowany w programie MPN i mieć Partner Center konto. Aby dowiedzieć się, jak to zrobić, [zobacz Tworzenie konta MPN w Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Tworzenie Azure Active Directory (AAD)

Zwykłych poświadczeń użytkownika nie można używać do programowego dostępu do danych usługi Partner Szczegółowe informacje Analytics. Aby Azure Active Directory programowych interfejsów API dostępu, należy utworzyć aplikację Azure Active Directory (AAD) wraz z kluczem tajnym (aplikacja i dostęp użytkowników). Aby dowiedzieć się, jak utworzyć aplikację i klucz tajny WAD, zobacz Szybki start: rejestrowanie aplikacji za pomocą [Platforma tożsamości Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Aby uzyskać dostęp do usługi Microsoft interfejs API Partner, wymagane jest interfejs API Partner. Aby dowiedzieć się, jak dodać uprawnienie, [zobacz interfejs API Partner — Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Przypisywanie użytkownikowi roli Executive Report Viewer (ERV)

Aby programowo uzyskać dostęp do danych analizy szczegółowych informacji partnerów, musisz mieć programowego podglądu raportów kadry kierowniczej (ERV). Aby dowiedzieć się, jak przypisać użytkownikowi rolę ERV, zobacz [Partner Center Szczegółowe informacje dostęp oparty](insights-roles.md) na rolach — Partner Center

## <a name="generate-an-aad-token"></a>Generowanie tokenu usługi AAD

Token usługi AAD należy wygenerować przy użyciu identyfikatora aplikacji (klienta), hasła klienta, identyfikatora użytkownika i hasła.   [Sprawdź tutaj,](insights-programmatic-first-api-call.md#token-generation) aby uzyskać instrukcje generowania tokenu usługi AAD.

> [!Note]
> Token jest ważny przez jedną godzinę.

## <a name="next-steps"></a>Następne kroki
[Paradygmat dostępu programowego](insights-programmatic-access-paradigm.md)