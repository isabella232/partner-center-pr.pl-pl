---
title: Azure plan — zarządzanie subskrypcjami & zasoby
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób partnerzy mogą korzystać z różnych opcji kontroli dostępu opartej na rolach (RBAC), aby uzyskiwać kontrolę operacyjną i zarządzać zasobami platformy Azure klienta.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534934"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure

**Odpowiednie role**

- Agent administracyjny


W tym artykule wyjaśniono, w jaki sposób partnerzy CSP mogą korzystać z różnych opcji kontroli dostępu opartej na rolach (RBAC), aby uzyskiwać kontrolę operacyjną i zarządzać zasobami platformy Azure klienta. Gdy przeniesiesz klienta do planu platformy Azure, domyślnie przypiszesz uprawnienia administratora na platformie Azure (prawa właściciela subskrypcji za pomocą administratora w imieniu).

 > [!NOTE]
 > Prawa administratora do subskrypcji platformy Azure mogą zostać usunięte przez klienta w ramach subskrypcji, grupy zasobów lub poziomu obciążenia. 

 Partnerzy mogą uzyskać 24x7ą kontrolę operacyjną i zarządzanie zasobami platformy Azure klienta w programie CSP przy użyciu różnych opcji dostępnych za pośrednictwem funkcji kontroli dostępu opartej na rolach (RBAC). 

- **Administrator w imieniu (AOBO)** — z [AOBOem](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)każdy użytkownik mający rolę Agent administracyjny w dzierżawie partnerskiej będzie miał dostęp do subskrypcji platformy Azure utworzonych za pomocą programu CSP.

- **Azure Lighthouse**: AOBO nie pozwala na elastyczność tworzenia odrębnych grup, które współpracują z różnymi klientami, lub aby włączyć różne role dla grup lub użytkowników. Za pomocą usługi Azure Lighthouse można przypisywać różne grupy do różnych klientów lub ról. Ze względu na to, że użytkownicy będą mieć odpowiedni poziom dostępu za pomocą zarządzania zasobami delegowanymi przez platformę Azure, można zmniejszyć liczbę użytkowników, którzy mają rolę agenta administratora (i w związku z tym mieć pełny dostęp AOBO). Pozwala to zwiększyć bezpieczeństwo przez ograniczenie niepotrzebnego dostępu do zasobów klientów. Zapewnia również większą elastyczność zarządzania wieloma klientami w odpowiedniej skali. Aby uzyskać więcej informacji, przeczytaj artykuł [Azure Lighthouse i program Cloud Solution Provider](/azure/lighthouse/concepts/cloud-solution-provider).

- **Użytkownicy katalogu lub Gości lub jednostki [usługi](/azure/active-directory/develop/app-objects-and-service-principals)**: można delegować szczegółowy dostęp do subskrypcji CSP przez dodanie użytkowników w katalogu klienta lub dodanie użytkowników-Gości i przypisanie określonych ról RBAC.

Firma Microsoft zaleca, aby użytkownicy mieli minimalne uprawnienia, których potrzebują do wykonywania swojej pracy jako rozwiązania zabezpieczeń. Zobacz [zasoby Azure Active Directory Privileged Identity Management](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Połącz swój identyfikator partnera (identyfikator MPN) z poświadczeniami, aby zarządzać zasobami platformy Azure klienta

W poniższej tabeli przedstawiono metody służące do kojarzenia identyfikatora partnera z różnymi opcjami dostępu RBAC.

|**Kategoria**   |**Scenariusz**   |**Skojarzenie identyfikatora MPN**|
|-----------------|:------------------------|:------------------|
|AOBO   |Bezpośredni partner lub dostawca usług kryptograficznych tworzy subskrypcję dla klienta, który domyślnie jest partnerem dostawcy usług kryptograficznych lub dostawcy pośrednim, przy użyciu AOBO.; Bezpośredni partner CSP lub Dostawca pośredni zapewniają pośredni dostęp do subskrypcji przy użyciu usługi AOBO.|Automatyczna (brak wymaganej pracy z partnerem)|
|Azure Lighthouse|Partner tworzy nową [ofertę usług zarządzanych w portalu Marketplace](/azure/lighthouse/concepts/managed-services-offers). Ta oferta zostanie zaakceptowana w ramach subskrypcji dostawcy usług kryptograficznych, a partner uzyskuje dostęp do subskrypcji dostawcy usług kryptograficznych.|Automatyczna (brak wymaganej pracy z partnerem)|
|Azure Lighthouse|Partner wdraża [szablon ARM](/azure/lighthouse/how-to/onboard-customer) w subskrypcji platformy Azure|Partner musi skojarzyć identyfikator MPN z użytkownikiem lub jednostką usługi w dzierżawie partnera. Aby uzyskać więcej informacji — [Identyfikator partnera linku](/azure/billing/billing-partner-admin-link-started).|
|Użytkownik katalogu lub gościa|Partner tworzy nowego użytkownika lub nazwę główną usługi w katalogu klienta i udziela użytkownikowi dostępu do subskrypcji dostawcy usług kryptograficznych. Partner tworzy nowego użytkownika lub nazwę główną usługi w katalogu klienta. Partner dodaje użytkownika do grupy i zapewnia dostęp do subskrypcji dostawcy usług kryptograficznych do grupy.|Partner musi skojarzyć identyfikator MPN z użytkownikiem lub jednostką usługi w dzierżawie klienta. Aby uzyskać więcej informacji — [Identyfikator partnera linku](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Upewnij się, że masz uprawnienia dostępu administratora

Musisz mieć dostęp administratora, aby zarządzać usługami klienta i otrzymać kredyty. W celu uzyskania szczegółowych informacji na temat dochodów uzyskanych przez [partnerów](partner-earned-credit.md) . Masz dwa sposoby, aby upewnić się, że masz pewność, że masz dostęp administratora.

- Przejrzyj plik dziennego użycia — można to ustalić, przeglądając cenę jednostkową i obowiązującą cenę jednostkową w pliku dziennego użycia i sprawdzając, czy jest stosowany rabat. Jeśli otrzymujesz rabat, który jesteś administratorem.

- Tworzenie alertu usługi Azure monitor — możesz utworzyć [alert](/azure/azure-monitor/platform/alerts-activity-log) dziennika aktywności Azure monitor, aby otrzymywać powiadomienia o tym, kiedy dostęp do usługi RBAC zostanie usunięty z subskrypcji dostawcy usług kryptograficznych.

### <a name="create-an-azure-monitor-alert"></a>Tworzenie alertu usługi Azure monitor

1. Utwórz alert.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Alert platformy Azure":::

2. Wybierz typ akcji, która ma zostać podjęta przez alert. Na przykład jeśli określisz, że chcesz wysłać wiadomość e-mail, otrzymasz wiadomość e-mail z powiadomieniem, jeśli wystąpi jakiekolwiek usunięcie przypisania roli.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="Konfigurowanie alertu":::

### <a name="aobo-removal"></a>Usuwanie AOBO

Klienci mogą zarządzać dostępem do swoich subskrypcji, przechodząc do **Access Control** na Azure Portal. Na karcie **przypisania ról** wybierają pozycję **Usuń dostęp**. W takim przypadku można:

- Skontaktuj się z klientem, aby sprawdzić, czy można przywrócić dostęp administratora.

- Użyj dostępu dostępnego za pośrednictwem [kontroli dostępu opartej na rolach (RBAC)](/azure/role-based-access-control/overview).

- Użyj dostępu dostępnego za pomocą [usługi Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Dostęp oparty na rolach różni się od dostępu administratora. Role ograniczają precyzyjne działania i nie mogą być wykonywane. Dostęp administratora jest szerszy.

Aby zobaczyć role kwalifikujące się do zdobycia PEC, Przeczytaj [role i uprawnienia dla partnera](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).

## <a name="next-steps"></a>Następne kroki

- [Odwoływanie i przywraca uprawnień administratora dla subskrypcji CSP platformy Azure](revoke-reinstate-csp.md)

- [Kredyt wypracowany przez partnera — przegląd](partner-earned-credit.md)

- [Kwota uzyskana przez partnera w przypadku usług zarządzanych](partner-earned-credit-explanation.md)