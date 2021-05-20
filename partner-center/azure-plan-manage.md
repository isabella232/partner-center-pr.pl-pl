---
title: Plan platformy Azure — zarządzanie subskrypcjami & zasobów
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak partnerzy mogą korzystać z różnych opcji kontroli dostępu opartej na rolach (RBAC) w celu uzyskania operacyjnej kontroli zasobów platformy Azure i zarządzania nimi.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 18cc5c62beaa76f6e3ade79f2f2069e0f2bd3c7e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149608"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure

**Odpowiednie role:** Agent administratora


W tym artykule wyjaśniono, jak partnerzy programu CSP mogą korzystać z różnych opcji kontroli dostępu opartej na rolach (RBAC) w celu uzyskania operacyjnej kontroli zasobów platformy Azure i zarządzania nimi. Po przejściu klienta do planu platformy Azure masz domyślnie przypisane uprzywilejowane prawa administratora na platformie Azure (prawa właściciela subskrypcji za pośrednictwem administratora w imieniu użytkownika).

 > [!NOTE]
 > Klient może usunąć prawa administratora do subskrypcji platformy Azure na poziomie subskrypcji, grupy zasobów lub obciążenia. 

 Partnerzy mogą uzyskać całodobową kontrolę operacyjną i zarządzanie zasobami platformy Azure klienta w programie CSP przy użyciu różnych opcji dostępnych za pośrednictwem funkcji kontroli dostępu opartej na rolach (RBAC). 

- **Admin on Behalf Of (AOBO)** — w przypadku funkcji [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)każdy użytkownik z rolą agenta administracyjnego w dzierżawie partnera będzie miał dostęp właściciela RBAC do subskrypcji platformy Azure tworzyć za pośrednictwem programu CSP.

- **Azure Lighthouse:** AOBO nie zezwala na elastyczność tworzenia odrębnych grup, które działają z różnymi klientami, ani włączania różnych ról dla grup lub użytkowników. Za Azure Lighthouse można przypisywać różne grupy do różnych klientów lub ról. Ponieważ użytkownicy będą mieć odpowiedni poziom dostępu za pośrednictwem zarządzania zasobami delegowanymi platformy Azure, można zmniejszyć liczbę użytkowników, którzy mają rolę agenta administracyjnego (i w związku z tym mają pełny dostęp do AOBO). Pomaga to zwiększyć bezpieczeństwo przez ograniczenie niepotrzebnego dostępu do zasobów klientów. Zapewnia ona również większą elastyczność zarządzania wieloma klientami na dużą skalę. Aby uzyskać więcej informacji, [przeczytaj Azure Lighthouse i Dostawca rozwiązań w chmurze programu](/azure/lighthouse/concepts/cloud-solution-provider).

- Użytkownicy katalogu lub użytkownicy-goście lub jednostki **[usługi:](/azure/active-directory/develop/app-objects-and-service-principals)** możesz delegować szczegółowy dostęp do subskrypcji CSP, dodając użytkowników w katalogu klienta lub dodając użytkowników-gości i przypisując określone role RBAC.

Firma Microsoft zaleca, aby użytkownicy mieli minimalne uprawnienia, których potrzebują, aby wykonać swoją pracę jako rozwiązanie w zakresie zabezpieczeń. Zobacz [Azure Active Directory Privileged Identity Management zasobów.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>Łączenie identyfikatora partnera (identyfikatora MPN) z poświadczeniami na potrzeby zarządzania zasobami platformy Azure klienta

W poniższej tabeli przedstawiono metody używane do skojarzenia identyfikatora partnera z różnymi opcjami dostępu RBAC.

|**Kategoria**   |**Scenariusz**   |**Skojarzenie identyfikatora MPN**|
|-----------------|:------------------------|:------------------|
|Aobo   |Partner bezpośredni lub dostawca pośredni dostawcy CSP tworzy subskrypcję dla klienta, dzięki czemu partner bezpośredni lub dostawca pośredni jest domyślnym właścicielem subskrypcji przy użyciu usługi AOBO. Bezpośredni partner programu CSP lub dostawca pośredni zapewniają odsprzedawcy pośredniego dostęp do subskrypcji przy użyciu usługi AOBO.|Automatyczne (nie jest wymagana żadna praca partnerska)|
|Azure Lighthouse|Partner tworzy nową [ofertę usług zarządzanych w witrynie Marketplace.](/azure/lighthouse/concepts/managed-services-offers) Ta oferta jest akceptowana w ramach subskrypcji programu CSP, a partner uzyskuje dostęp do subskrypcji CSP.|Automatyczne (nie jest wymagana żadna praca partnerska)|
|Azure Lighthouse|Partner wdraża szablon [usługi ARM w](/azure/lighthouse/how-to/onboard-customer) subskrypcji platformy Azure|Partner musi skojarzyć identyfikator MPN z użytkownikiem lub jednostką usługi w dzierżawie partnera. Aby uzyskać więcej informacji, [kliknij identyfikator partnera](/azure/billing/billing-partner-admin-link-started).|
|Katalog lub użytkownik-gość|Partner tworzy nowego użytkownika lub jednostkę usługi w katalogu klienta i zapewnia użytkownikowi dostęp do subskrypcji dostawcy usług w chmurze. Partner tworzy nowego użytkownika lub jednostkę usługi w katalogu klienta. Partner dodaje użytkownika do grupy i zapewnia dostęp do subskrypcji programu CSP do grupy.|Partner musi skojarzyć identyfikator MPN z użytkownikiem lub jednostką usługi w dzierżawie klienta. Aby uzyskać więcej informacji, [kliknij link identyfikator partnera](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Potwierdź, że masz dostęp administratora

Aby zarządzać usługami klienta i uzyskać uzyskane środki, wymagany jest dostęp administratora. Przeczytaj [informacje o środki uzyskane przez partnerów,](partner-earned-credit.md) aby uzyskać szczegółowe informacje na temat uzyskanego środków. Masz dwa sposoby, aby upewnić się, że masz dostęp administratora.

- Przejrzyj plik dziennego użycia — można to ustalić, przeglądając cenę jednostkową i efektywną cenę jednostkową w pliku dziennego użycia i potwierdzając, czy rabat jest stosowany. Jeśli otrzymujesz rabat, jesteś administratorem.

- Tworzenie alertu usługi Azure Monitor — możesz utworzyć [](/azure/azure-monitor/platform/alerts-activity-log) alert dziennika aktywności usługi Azure Monitor, który będzie powiadamiany o usunięciu dostępu RBAC z subskrypcji CSP.

### <a name="create-an-azure-monitor-alert"></a>Tworzenie alertu usługi Azure Monitor

1. Utwórz alert.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="alert platformy azure":::

2. Wybierz typ akcji, którą ma podjąć alert. Jeśli na przykład określisz, że chcesz otrzymywać wiadomości e-mail, otrzymasz wiadomość e-mail z powiadomieniem o usunięciu przypisania roli.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="konfigurowanie alertu":::

### <a name="aobo-removal"></a>Usuwanie AOBO

Klienci mogą zarządzać dostępem do swoich subskrypcji, przechodząc **do Access Control** na Azure Portal. Na karcie **Przypisania ról zaznacz** opcję Usuń **dostęp.** W takim przypadku można:

- Porozmawiaj z klientem, aby sprawdzić, czy można przywrócić dostęp administratora.

- Użyj dostępu zapewnianych za [pośrednictwem kontroli dostępu opartej na rolach (RBAC).](/azure/role-based-access-control/overview)

- Użyj dostępu udostępnianego za [pośrednictwem Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Dostęp oparty na rolach różni się od dostępu administratora. Role dokładnie oddzielają to, co można, a czego nie można robić. Dostęp administratora jest szerszy.

Aby wyświetlić role kwalifikujące się do uzyskania punktów PEC, przeczytaj [role i uprawnienia dla środków uzyskane przez partnera.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)

## <a name="next-steps"></a>Następne kroki

- [Odwoływanie i ponowne odwoływanie uprawnień administratora dla Azure CSP subskrypcji](revoke-reinstate-csp.md)

- [Środków uzyskane przez partnerów — omówienie](partner-earned-credit.md)

- [Środków uzyskane przez partnerów dla usług zarządzanych](partner-earned-credit-explanation.md)