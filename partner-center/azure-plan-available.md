---
title: Dostępne usługi platformy Azure w programie Azure CSP
description: W tym artykule omówiono usługi platformy Azure, które są i nie są dostępne w programie Azure Dostawca rozwiązań w chmurze (CSP).
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 6037044a72bd9bd71131ddbc66fec0555bbd5f86
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246393"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Usługi platformy Azure dostępne w programie Azure Dostawca rozwiązań w chmurze (CSP)

**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny | Agent pomocy technicznej | Agent sprzedaży | Administrator zarządzania użytkownikami

## <a name="available-azure-services-in-azure-csp"></a>Dostępne usługi platformy Azure w programie Azure CSP

W tym artykule wymieniono usługi platformy Azure, które są i nie są dostępne w programie Azure Dostawca rozwiązań w chmurze (CSP). Omówiono w nim również dostępność usług w chmurach krajowych Microsoft Azure [Niemcy i](https://azure.microsoft.com/overview/clouds/germany/) [Microsoft Azure Government.](https://azure.microsoft.com/overview/clouds/government/)

>[!Note]
> [Platforma Azure (Chiny)](https://www.azure.cn/) nie jest dostępna w Azure CSP chmurze.

## <a name="global-cloud"></a>Chmura globalna

Wszystkie usługi oparte na Azure Resource Manager są dostępne w programie CSP.  Usługi inne Azure Resource Manager, takie jak usługi klasycznego modelu wdrażania, nie są dostępne w programie CSP.  

## <a name="csp-specific-service-configurations"></a>CSP-Specific konfiguracji usługi

Następujące usługi wymagają specjalnych konfiguracji w programie CSP:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Usługa Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Szczegółowe informacje](https://azure.microsoft.com/services/time-series-insights/) Tylko użytkownicy z dzierżawy klienta mogą uzyskać dostęp do danych w ich środowisku Szczegółowe informacje Time Series. Partnerzy mogą domyślnie zarządzać środowiskiem usługi Time Series Szczegółowe informacje klienta, ale jeśli potrzebują dostępu do danych w nim, muszą zostać dodani do dzierżawy klienta.

- Certyfikaty zarządzania do uwierzytelniania bibliotek zestawu Azure SDK za pośrednictwem certyfikatu nie są obsługiwane w modelu CSP.  Zamiast tego skorzystaj z uwierzytelniania jednostki usługi Azure AD i biblioteki Azure.Identity.  Odwołanie [do uwierzytelniania za pomocą zestawu Azure SDK dla platformy .NET](/dotnet/azure/sdk/authentication)

## <a name="visual-studio-marketplace"></a>Witryna Visual Studio Marketplace

Teraz możesz kupić elementy wymienione poniżej w witrynie Visual Studio Marketplace, z wyjątkiem rozszerzeń innych firm.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Subskrypcje programu Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Xamarin University szkoleniowe](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Aby ułatwić ci pracę, utworzono filmy wideo i dokumentację dotyczące sposobu konfigurowanie i kupowanie aplikacji oraz zarządzania nimi [Azure DevOps](/vsts/billing/csp/set-up-csp-customer) CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Elementy witryny Azure Marketplace w programie Azure CSP

Nie wszystkie Azure Marketplace są obecnie dostępne w Azure CSP subskrypcji.

- Usługi platformy Azure oparte na firmie Microsoft: te usługi są dostępne. Przejrzyj poprzednią tabelę i komentarze.

- Bring your own license (BYOL): te elementy są dostępne. Pełna lista elementów aplikacji z włączoną obsługą Azure Marketplace BYOL jest dostępna na stronie [Azure Marketplace BYOL.](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)

- Elementy aplikacji innych firm z płatnością zgodnie z Azure Marketplace: te elementy są dostępne, jeśli dostawca został opublikowany w kanale dostawcy usług w chmurze. Aby uzyskać więcej informacji, zobacz [Sell subscriptions to Azure Marketplace products](csp-commercial-marketplace-overview.md)(Sprzedaż subskrypcji Azure Marketplace produktów).

- Citrix XenApp Essentials: Partnerzy mogą zakupić XenApp Essentials dla klientów w programie CSP. Aby uzyskać więcej informacji, zobacz następujący blog Citrix — Dystrybucja XenApp Essentials [jest teraz dostępna za pośrednictwem Microsoft Cloud Solution Provider Channel.](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/)

## <a name="national-clouds"></a>Chmury narodowe

W poniższej tabeli przedstawiono regularnie aktualizowaną listę dostępnych produktów, usług i funkcji platformy Azure oferowanych przez dostawców rozwiązań w chmurze krajowej.

| Produkt, usługa lub funkcja platformy Azure | US Government | Niemcy |
| ------ | :-----------: | :-----------: |
|  **Środowisko obliczeniowe**  |    |    |
|  Virtual Machines  |  X  |  X  |
|  Cloud Services  |    |    |
|  Zestawy skalowania maszyn wirtualnych  |  X  |  X  |
|  Funkcje  |    |    |
|  Azure Container Service  |    |    |
|  **Sieć**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Virtual Network  |  X  |  X  |
|  Load Balancer  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **Storage**  |    |    |
|  Storage  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Dyski zarządzane  |  X  |  X  |
|  **Sieć Web + aplikacje mobilne**  |    |    |
|  App Service  |  X  |  X  |
|  Usługa App Service w systemie Linux  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Logic Apps funkcji Azure App Service  |    |    |
|  **Containers**  |    |    |
|  App Service  |  X  |  X  |
|  Usługa App Service w systemie Linux  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **Bazy danych**  |    |    |
|  SQL Database  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Pamięć podręczna Redis  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **Dane + analiza**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI + Cognitive Services**  |    |    |
|  Usługa Machine Learning  |    |  X  |
|  Usługa Azure Bot  |    |    |
|  Cognitive Services  |    |    |
|  Sztuczna inteligencja w usłudze Azure Batch  |    |    |
|  **Internet rzeczy**  |    |    |
|  Usługa IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Usługa Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location-Based Services  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Enterprise Integracji**  |    |    |
|  StorSimple  |  X  |    |
|  API Management  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Logic Apps funkcji Azure App Service  |    |    |
|  **Zabezpieczenia + tożsamość**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Uwierzytelnianie wieloskładnikowe  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Security Center  |  X  |  X  |
|  **Narzędzia deweloperskie**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Monitorowanie + zarządzanie**  |    |    |
|  Advisor  |    |    |
|  Backup  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Scheduler  |  X  |  X  |
|  Automation  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Azure-Managed aplikacji  |    |    |
|  Azure Migrate  |    |    |
|  Grupy zarządzania  |    |  

## <a name="next-steps"></a>Następne kroki

- [Dowiedz się](/azure/cloud-solution-provider/overview/partner-center-overview) więcej o dostępnych możliwościach platformy Azure w Partner Center.

- [Tworzenie](/azure/cloud-solution-provider/customer-management/create-new-customer) pierwszego klienta w Azure CSP i wdrażanie usług platformy Azure.
