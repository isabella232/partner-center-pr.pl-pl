---
title: Przykładowa aplikacja
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Użyj przykładowej aplikacji, aby skompilować własną aplikację, aby programowo uzyskać dostęp do danych szczegółowych informacji o partnerach.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376661"
---
# <a name="sample-application"></a>Przykładowa aplikacja

Przykładowe aplikacje są tworzone w językach C# i JAVA i są dostępne w [GitHub](https://github.com/partneranalytics)

- [Przykładowa aplikacja w języku C#](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Przykładowa aplikacja JAVA](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Możesz skorzystać z inspiracji z przykładowej aplikacji i utworzyć własną aplikację w dowolnym języku.

Przykładowa aplikacja osiąga następujące cele:

- Generuje token Azure Active Directory (Azure AD).
- Pobiera dostępne zestawy danych.
- Tworzy zapytania zdefiniowane przez użytkownika.
- Pobiera zapytania systemowe i zdefiniowane przez użytkownika.
- Planuje raport.

Przykładowa aplikacja nie obejmuje metody wywoływania interfejsów API dla innych funkcji. Jednak proces wywoływania innych interfejsów API pozostaje taki sam, jak opisano powyżej.

## <a name="how-to-run-the-application"></a>Jak uruchomić aplikację

- Sklonuj repozytorium do systemu lokalnego przy użyciu tego polecenia:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Aby uzyskać więcej instrukcji, zapoznaj się z plikiem ProgrammaticExportSampleAppMPN/README.md w GitHub [repozytorium .](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

- Aby szybko uruchomić aplikację, zaktualizuj identyfikator klienta i klucz tajny klienta wappsettings.Development.js **na**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrowanie ciągu JSON tworzenia aplikacji":::

Uruchomienie aplikacji spowoduje uruchomienie lokalnego serwera internetowego, a zostanie otwarta strona ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustrowanie interfejsu użytkownika przykładowej aplikacji":::

Ta strona spowoduje wywołania interfejsu API do serwera internetowego uruchomionego na komputerze lokalnym, co z kolei spowoduje rzeczywiste programowe wywołania interfejsu API dostępu.

## <a name="code-snippets"></a>Wstawki kodu

Podstawowa struktura kodu języka C# do wykonywania programowych wywołań interfejsu API dostępu jest następująca:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrowanie fragmentu kodu":::

## <a name="next-steps"></a>Następne kroki

[Interfejsy API do uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów](insights-programmatic-analytics-available-api.md)
