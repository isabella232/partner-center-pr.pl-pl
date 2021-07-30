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
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845095"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych

**Odpowiednie role:** Administrator globalny | Administrator programu MPN

Aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji o partnerach, należy spełnić następujące wymagania.

## <a name="mpn-program-enrollment"></a>Rejestracja w programie MPN

Aby programowo uzyskać dostęp do danych analizy analizy partnerów, musisz być zarejestrowany w programie MPN i mieć Partner Center konto. Aby dowiedzieć się, jak to zrobić, [zobacz Tworzenie konta MPN w u Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Tworzenie Azure Active Directory (AAD)

Zwykłych poświadczeń użytkownika nie można używać do programowego dostępu do danych Szczegółowe informacje Analytics. Aby Azure Active Directory programowych interfejsów API dostępu, należy utworzyć aplikację aplikacji Azure Active Directory (AAD) wraz z kluczem tajnym (aplikacja i dostęp użytkowników). Aby dowiedzieć się, jak utworzyć aplikację i wpis tajny w UAD, zobacz Szybki start: rejestrowanie aplikacji za pomocą [Platforma tożsamości Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Wymagane jest uprawnienie dostępu do usługi Microsoft interfejs API Partner. Aby dowiedzieć się, jak dodać uprawnienia, zobacz [interfejs API Partner — Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Przypisywanie użytkownikowi roli Executive Report Viewer (ERV)

Aby programowo uzyskać dostęp do danych analizy szczegółowych informacji o partnerach, musisz mieć programowy programowy wgląd w szczegółowe dane partnerów, czyli E Aby dowiedzieć się, jak przypisać rolę ERV do użytkownika, zobacz [Partner Center Szczegółowe informacje dostępu opartego](insights-roles.md) na rolach — Partner Center

## <a name="generate-an-aad-token"></a>Generowanie tokenu usługi AAD

Token usługi AAD należy wygenerować przy użyciu identyfikatora aplikacji (klienta), hasła klienta, identyfikatora użytkownika i hasła.   [Sprawdź tutaj,](insights-programmatic-first-api-call.md#token-generation) aby uzyskać instrukcje generowania tokenu usługi AAD.

> [!Note]
> Token jest ważny przez jedną godzinę.

## <a name="next-steps"></a>Następne kroki
[Paradygmat dostępu programowego](insights-programmatic-access-paradigm.md)