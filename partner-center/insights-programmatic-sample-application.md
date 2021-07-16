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
# <a name="sample-application"></a><span data-ttu-id="eed2a-103">Przykładowa aplikacja</span><span class="sxs-lookup"><span data-stu-id="eed2a-103">Sample Application</span></span>

<span data-ttu-id="eed2a-104">Przykładowe aplikacje są tworzone w językach C# i JAVA i są dostępne w [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="eed2a-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="eed2a-105">Przykładowa aplikacja w języku C#</span><span class="sxs-lookup"><span data-stu-id="eed2a-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="eed2a-106">Przykładowa aplikacja JAVA</span><span class="sxs-lookup"><span data-stu-id="eed2a-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="eed2a-107">Możesz skorzystać z inspiracji z przykładowej aplikacji i utworzyć własną aplikację w dowolnym języku.</span><span class="sxs-lookup"><span data-stu-id="eed2a-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="eed2a-108">Przykładowa aplikacja osiąga następujące cele:</span><span class="sxs-lookup"><span data-stu-id="eed2a-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="eed2a-109">Generuje token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="eed2a-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="eed2a-110">Pobiera dostępne zestawy danych.</span><span class="sxs-lookup"><span data-stu-id="eed2a-110">Gets available datasets.</span></span>
- <span data-ttu-id="eed2a-111">Tworzy zapytania zdefiniowane przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eed2a-111">Creates user defined queries.</span></span>
- <span data-ttu-id="eed2a-112">Pobiera zapytania systemowe i zdefiniowane przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eed2a-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="eed2a-113">Planuje raport.</span><span class="sxs-lookup"><span data-stu-id="eed2a-113">Schedules a report.</span></span>

<span data-ttu-id="eed2a-114">Przykładowa aplikacja nie obejmuje metody wywoływania interfejsów API dla innych funkcji.</span><span class="sxs-lookup"><span data-stu-id="eed2a-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="eed2a-115">Jednak proces wywoływania innych interfejsów API pozostaje taki sam, jak opisano powyżej.</span><span class="sxs-lookup"><span data-stu-id="eed2a-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="eed2a-116">Jak uruchomić aplikację</span><span class="sxs-lookup"><span data-stu-id="eed2a-116">How to run the application</span></span>

- <span data-ttu-id="eed2a-117">Sklonuj repozytorium do systemu lokalnego przy użyciu tego polecenia:</span><span class="sxs-lookup"><span data-stu-id="eed2a-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="eed2a-118">Aby uzyskać więcej instrukcji, zapoznaj się z plikiem ProgrammaticExportSampleAppMPN/README.md w GitHub [repozytorium .](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)</span><span class="sxs-lookup"><span data-stu-id="eed2a-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="eed2a-119">Aby szybko uruchomić aplikację, zaktualizuj identyfikator klienta i klucz tajny klienta wappsettings.Development.js **na**</span><span class="sxs-lookup"><span data-stu-id="eed2a-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrowanie ciągu JSON tworzenia aplikacji":::

<span data-ttu-id="eed2a-121">Uruchomienie aplikacji spowoduje uruchomienie lokalnego serwera internetowego, a zostanie otwarta strona ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).</span><span class="sxs-lookup"><span data-stu-id="eed2a-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustrowanie interfejsu użytkownika przykładowej aplikacji":::

<span data-ttu-id="eed2a-123">Ta strona spowoduje wywołania interfejsu API do serwera internetowego uruchomionego na komputerze lokalnym, co z kolei spowoduje rzeczywiste programowe wywołania interfejsu API dostępu.</span><span class="sxs-lookup"><span data-stu-id="eed2a-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="eed2a-124">Wstawki kodu</span><span class="sxs-lookup"><span data-stu-id="eed2a-124">Code Snippets</span></span>

<span data-ttu-id="eed2a-125">Podstawowa struktura kodu języka C# do wykonywania programowych wywołań interfejsu API dostępu jest następująca:</span><span class="sxs-lookup"><span data-stu-id="eed2a-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrowanie fragmentu kodu":::

## <a name="next-steps"></a><span data-ttu-id="eed2a-127">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eed2a-127">Next steps</span></span>

[<span data-ttu-id="eed2a-128">Interfejsy API do uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów</span><span class="sxs-lookup"><span data-stu-id="eed2a-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
