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
ms.openlocfilehash: 0f94b61e5228241e0314bca3443a8d5378d14916872e2bf3a4271aa7e6fae9f6
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693306"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych

**Odpowiednie role:** Administrator globalny | Administrator programu MPN

Aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji o partnerach, należy spełnić następujące wymagania.

## <a name="mpn-program-enrollment"></a>Rejestracja w programie MPN

Aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji o partnerach, musisz być zarejestrowany w programie MPN i mieć Partner Center konto. Aby dowiedzieć się, jak to zrobić, [zobacz Tworzenie konta MPN w u Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Tworzenie Azure Active Directory (AAD)

Zwykłych poświadczeń użytkownika nie można używać do programowego dostępu do danych Szczegółowe informacje Analytics. Aby Azure Active Directory programowych interfejsów API dostępu, należy utworzyć aplikację aplikacji Azure Active Directory (AAD) wraz z kluczem tajnym (aplikacja i dostęp użytkowników). Aby dowiedzieć się, jak utworzyć aplikację i wpis tajny w UAD, zobacz Szybki start: rejestrowanie aplikacji za pomocą [Platforma tożsamości Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Wymagane jest uprawnienie dostępu do usługi Microsoft interfejs API Partner. Aby dowiedzieć się, jak dodać uprawnienia, zobacz [interfejs API Partner — Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Przypisywanie użytkownikowi roli Executive Report Viewer (ERV)

Aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji o partnerach, musisz mieć programowy programowy wgląd w szczegółowe dane partnerów, czyli ERV (Executive Report Viewer). Aby dowiedzieć się, jak przypisać rolę ERV do użytkownika, zobacz [Partner Center Szczegółowe informacje dostępu opartego](insights-roles.md) na rolach — Partner Center

## <a name="generate-an-aad-token"></a>Generowanie tokenu usługi AAD

Token usługi AAD należy wygenerować przy użyciu identyfikatora aplikacji (klienta), hasła klienta, identyfikatora użytkownika i hasła.   [Sprawdź tutaj,](insights-programmatic-first-api-call.md#token-generation) aby uzyskać instrukcje generowania tokenu usługi AAD.

> [!Note]
> Token jest ważny przez jedną godzinę.

## <a name="next-steps"></a>Następne kroki
[Paradygmat dostępu programowego](insights-programmatic-access-paradigm.md)