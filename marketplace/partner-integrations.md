---
title: Integracja z partnerem portalu Azure Marketplace
description: Dowiedz się więcej o rozwiązaniach portalu Azure Marketplace, które integrują się ze środowiskiem platformy Azure, i uzyskaj link do przewodników wdrażania od partnerów firmy Microsoft.
ms.service: partner-services
ms.topic: conceptual
author: dsindona
ms.author: dsindona
ms.date: 11/16/2020
ms.openlocfilehash: 7c97936e7764361c21503eca174433029707cf69
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691688"
---
# <a name="azure-marketplace-partner-integrations"></a>Integracja z partnerem portalu Azure Marketplace

Dowiedz się, jak zintegrować rozwiązania partnerskie ze środowiskiem platformy Azure. Ten artykuł zawiera omówienie poszczególnych rozwiązań i linki do szczegółowych wskazówek dotyczących wdrażania. Rozwiązania są wyświetlane w kolejności alfabetycznej. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka w chmurze z systemem

![Chmura w chmurze](./media/partners/confluent-cloud.png)

Platforma Azure umożliwia integrację z chmurą w chmurze oprócz aplikacji w chmurze. Klienci korzystający z tej usługi często przechodźą między Azure Portal i chmurą. Na przykład, gdy użytkownik kupuje ofertę w chmurze w portalu Azure Marketplace, oczekujemy na skonfigurowanie konta z chmurą. Ten proces zwiększa złożoność i czas oraz wymaga od użytkowników zarządzania konfiguracją i zasobami między tymi dwoma portalami. Aby zmniejszyć obciążenie związane z zarządzaniem między platformami, firma Microsoft, w ramach partnerstwa z usługą współpracy w chmurze, utworzyła zintegrowaną warstwę aprowizacji z platformy Azure do współpracy w chmurze. Rozwiązanie jest dostępne w witrynie Azure Marketplace i zapewnia bezproblemowe środowisko do korzystania z oferty usługi Cloud-The-Fluent na platformie Azure

Rozwiązanie korzysta z dostawcy zasobów włączonego na platformie Azure, aby zapewnić obsługę zasobów w chmurze. Dzięki temu użytkownicy mogą uzyskiwać dostęp do przesyłania strumieniowego w czasie rzeczywistym za pośrednictwem Azure Portal, interfejsu wiersza polecenia platformy Azure i zestawów SDK platformy Azure. Usługa w chmurze jest własnością i uruchamia aplikację SaaS, która obejmuje środowiska, klastry, tematy, klucze interfejsu API i łączniki zarządzane.

Ścisła integracja z usługą zapewniającą integrację z chmurą zapewnia następujące możliwości:

- Zainicjuj obsługę nowego zasobu organizacji z obsługą chmury, korzystając z Azure Portal z w pełni zarządzaną infrastrukturą.
- Usprawnij Logowanie jednokrotne z platformy Azure, aby uzyskać chmurę z usługą Azure Active Directory. w portalu z chmurą w chmurze nie trzeba wykonywać oddzielnego uwierzytelniania.
- Uzyskaj ujednolicone rozliczanie opłat za użycie w chmurze za pomocą fakturowania subskrypcji platformy Azure.
- Zarządzaj zasobami w chmurze z poziomu Azure Portal i śledź je na stronie **wszystkie zasoby** , obok zasobów platformy Azure.

[Przewodniki wdrażania w chmurze](https://docs.confluent.io/current/cloud/marketplace/index.html)

W przypadku problemów związanych z działaniem na platformie Azure przejdź do [https://support.confluent.io](https://support.confluent.io) . Jeśli jesteś użytkownikiem po raz pierwszy, zresetuj hasło przed zalogowaniem się do portalu pomocy technicznej. Jeśli nie masz konta z usługą, Wyślij wiadomość e-mail na adres [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Logo usługi Datadog](./media/partners/datadog.png)

Usługi Datadog udostępnia narzędzia do obsługi i zabezpieczeń dla użytkowników platformy Azure, aby poznać kondycję i wydajność swoich aplikacji w środowiskach hybrydowych i wielochmurowych. Jednak skonfigurowanie niezbędnych integracji często wymaga przechodzenia między Azure Portal i usługi Datadog. Aby uprościć zarządzanie konfiguracjami i zasobami w wielu portalach, firma Microsoft pracowała z usługą usługi Datadog w celu utworzenia zintegrowanego rozwiązania usługi Datadog na platformie Azure. To rozwiązanie jest dostępne za pośrednictwem portalu Azure Marketplace, ponieważ umożliwia klientom platformy Azure bezproblemowe korzystanie z rozwiązania do monitorowania w chmurze usługi Datadog.

Zapoznaj się z [dokumentacją Azure monitor](/azure/azure-monitor/platform/partners#datadog) , aby dowiedzieć się więcej o tym rozwiązaniu i utworzyć konto w publicznej wersji zapoznawczej.

## <a name="next-steps"></a>Następne kroki

- [Sklep online w portalu Azure Marketplace](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Tworzenie konta platformy Azure](/learn/modules/create-an-azure-account/)
