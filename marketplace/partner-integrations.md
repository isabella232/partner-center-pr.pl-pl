---
title: Integracje partnerów witryny Azure Marketplace
description: Dowiedz się więcej Azure Marketplace, które integrują się ze środowiskiem platformy Azure, oraz uzyskaj link do przewodników wdrażania od partnerów firmy Microsoft.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276488"
---
# <a name="azure-marketplace-partner-integrations"></a>Integracje partnerów witryny Azure Marketplace

Dowiedz się, jak zintegrować rozwiązania partnerskie ze środowiskiem platformy Azure. Ten artykuł zawiera omówienie poszczególnych rozwiązań i linki do szczegółowych przewodników wdrażania. Rozwiązania są wyświetlane w kolejności alfabetycznej. 

## <a name="apache-kafka-on-confluent-cloud"></a>Platforma Apache Kafka na platformie Confluent Cloud

![Confluent Cloud.](./media/partners/confluent-cloud.png)

Platforma Azure umożliwia integrację z aplikacją Confluent Cloud oraz aplikacjami w chmurze. Klienci confluent często nawigują między Azure Portal i confluent Cloud. Na przykład gdy użytkownik kupi ofertę Confluent Cloud w usłudze Azure Marketplace, powinien skonfigurować konto w aplikacji Confluent Cloud. Ten proces zwiększa złożoność i czas oraz wymaga od użytkowników zarządzania konfiguracją i zasobami między dwoma portalami. Aby zmniejszyć obciążenie związane z zarządzaniem na różnych platformach, firma Microsoft, we współpracy z firmą Confluent Cloud, zbudowała zintegrowaną warstwę aprowizowania od platformy Azure do aplikacji Confluent Cloud. Rozwiązanie jest dostępne w witrynie Azure Marketplace i zapewnia bezproblemowe środowisko do korzystania z oferty Confluent Cloud na platformie Azure

Rozwiązanie używa dostawcy zasobów włączonego na platformie Azure, aby aprowizować zasoby aplikacji Confluent Cloud. Dzięki temu użytkownicy mogą uzyskać dostęp do przesyłania strumieniowego zdarzeń w czasie rzeczywistym za pośrednictwem interfejsu Azure Portal, interfejsu wiersza polecenia platformy Azure i zestawów Azure SDK. Confluent Cloud jest właścicielem i uruchamia aplikację SaaS, która obejmuje środowiska, klastry, tematy, klucze interfejsu API i zarządzane łączniki.

Głęboka integracja z usługą Confluent Cloud zapewnia następujące możliwości:

- Aprowizuj nowy zasób organizacji Confluent Cloud z Azure Portal w pełni zarządzaną infrastrukturą.
- Usprawnij logowanie single sign-on from Azure to Confluent Cloud with Azure Active Directory; nie jest wymagane oddzielne uwierzytelnianie od portalu Confluent Cloud.
- Uzyskaj ujednolicone rozliczenia opłat za korzystanie z usługi Confluent Cloud za pośrednictwem fakturowania subskrypcji platformy Azure.
- Zarządzaj zasobami aplikacji Confluent Cloud z Azure Portal i śledź je na stronie **Wszystkie** zasoby obok zasobów platformy Azure.

[Przewodniki wdrażania aplikacji Confluent Cloud](https://docs.confluent.io/current/cloud/marketplace/index.html)

W przypadku problemów związanych z usługą Confluent on Azure przejdź do witryny [https://support.confluent.io](https://support.confluent.io) . Jeśli jesteś użytkownikiem po raz pierwszy, zresetuj hasło przed zalogowaniem się do portalu pomocy technicznej aplikacji Confluent. Jeśli nie masz konta w aplikacji Confluent, wyślij wiadomość e-mail na adres [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Logo DataDog.](./media/partners/datadog.png)

Usługa Datadog udostępnia użytkownikom platformy Azure narzędzia do monitorowania i zabezpieczeń, które pozwalają zrozumieć kondycję i wydajność aplikacji w środowiskach hybrydowych i wielochmurowych. Jednak skonfigurowanie niezbędnych integracji często wymaga nawigowania między Azure Portal i usługą Datadog. Aby uprościć konfigurację i zarządzanie zasobami w różnych portalach, firma Microsoft współpracowała z usługą Datadog w celu utworzenia zintegrowanego rozwiązania Usługi Datadog na platformie Azure. Dostępne za pośrednictwem Azure Marketplace to rozwiązanie zapewnia bezproblemowe środowisko dla klientów platformy Azure do korzystania z rozwiązania do monitorowania chmury usługi Datadog.

Zobacz [dokumentację Azure Monitor,](/azure/azure-monitor/platform/partners#datadog) aby dowiedzieć się więcej o tym rozwiązaniu i zarejestrować się w publicznej wersji zapoznawczej.

## <a name="next-steps"></a>Następne kroki

- [Azure Marketplace sklepu online](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Tworzenie konta platformy Azure](/learn/modules/create-an-azure-account/)
