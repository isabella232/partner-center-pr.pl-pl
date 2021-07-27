---
title: Często zadawane pytania dotyczące środków uzyskane przez partnerów
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Znajdź odpowiedzi na często zadawane pytania dotyczące środków uzyskane przez partnerów.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e5d6aa77a02a24648828f06fb2c56640abdbfc56
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434217"
---
# <a name="frequently-asked-questions-for-partner-earned-credit"></a>Często zadawane pytania dotyczące środków uzyskane przez partnerów

Odpowiednie role: Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Administrator rozliczeń | Agent sprzedaży

Poniżej znajduje się lista często zadawanych pytań dotyczących środków uzyskane przez partnerów.

## <a name="how-much-is-pec"></a>Ile wynosi PEC?

Kwota zarobków partnerów dla PEC będzie się różnić (zobacz [Obliczanie](partner-earned-credit-explanation.md#calculation)). Stawka znajduje się na stronie cennika w Partner Center.

## <a name="what-azure-services-are-eligible-for-pec"></a>Jakie usługi platformy Azure kwalifikują się do PEC?

PEC kwalifikuje się do wszystkich usług związanych z nową ofertą platformy Azure w programie CSP (plan platformy Azure), z wyjątkiem następujących: 
- Rezerwacje nowej oferty platformy Azure (plan platformy Azure)
- Produkty innych firm zidentyfikowane jako produkty innych firm w kolumnie Tagi cennika użycia planu platformy Azure
- Produkty w cenniku witryny Marketplace
- [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

## <a name="where-can-i-see-pec"></a>Gdzie mogę zobaczyć PEC?

Zobacz [Obliczanie](partner-earned-credit-explanation.md#calculation).

## <a name="where-can-i-find-pec-details"></a>Gdzie można znaleźć szczegóły PEC?

Szczegóły dotyczące PEC mogą być wyszukiwane bezpośrednio przez interfejs [API,](partner-earned-credit-explanation.md#calculation) codzienny plik rekonescji i [narzędzie ACM (Azure Cost Mgmt)](partner-earned-credit-explanation.md#azure-cost-management-and-pec) przez partnerów.

## <a name="how-can-i-reconcile-my-pec-information-across-the-two-recon-files"></a>Jak mogę uzgodnić informacje dotyczące PEC między dwoma plikami rekonescji?

W obszarze Rozliczenia znajdują się dwa pliki uzgodnień Partner Center, których można użyć.

- Ostatnie działania uzgadniania użycia ocenianego codziennie (.csv)
- Działanie uzgadniania ostatnich (.csv)

Aby uzgodnić, partner może porównać pola ProductID, SKUID i AvailabilityID z tych dwóch plików dla każdego pola SubscriptionID.

## <a name="for-an-indirect-reseller-working-with-an-indirect-provider-does-an-indirect-provider-need-to-add-the-indirect-resellers-account-as-an-rbac-identity-and-access-management-iam-role-to-the-end-customers-subscription-in-order-to-utilize-acm"></a>Czy w przypadku odsprzedawcy pośredniego, który współpracuje z dostawcą pośrednim, czy dostawca pośredni musi dodać konto odsprzedawcy pośredniego jako rolę zarządzania tożsamościami i dostępem RBAC (IAM) do subskrypcji klienta końcowego, aby móc korzystać z usługi ACM?

Tak, użytkownik CSP Indirect Provider dostęp [RBAC](/azure/role-based-access-control/overview) do odsprzedawcy pośredniego w subskrypcji platformy Azure.

## <a name="what-happens-if-a-customer-removes-a-partners-rbac-admin-access"></a>Co się stanie, jeśli klient usunie dostęp administratora RBAC partnera?

Partner bez odpowiedniego dostępu RBAC w programie CSP zachowuje w firmie Microsoft relację rozliczeń i odpowiedzialność klienta z platformą Azure. Chociaż nie ma to wpływu na partnera sprzedaży poprzedniej oferty platformy Azure w programie CSP, w przypadku nowej oferty platformy Azure w programie CSP, zafakturowany partner nie będzie kwalifikować się do PEC na fakturze za platformę Azure. Partnerzy mogą uzyskać częściowy dostęp administratora w programie CSP, uzyskanie dostępu za pośrednictwem konta użytkownika za pośrednictwem dostępu do katalogu/gościa przy użyciu kontroli dostępu na Azure Lighthouse. Aby uzyskać więcej informacji, zobacz [Przywróć](revoke-reinstate-csp.md)uprawnienia administratora dla subskrypcji Azure CSP klienta.

## <a name="how-do-i-know-if-im-earning-pec"></a>Jak mogę, czy zarobkuję PEC?

Istnieje kilka sposobów, w jakie partner może potwierdzić, że ma odpowiedni dostęp do zasobów platformy Azure klienta.

- Przejrzyj plik dziennego użycia: Jeśli partner otrzymuje kredyt uzyskane przez partnera dla usług zarządzanych, ma dostęp administratora. Można to ustalić, przeglądając cenę jednostkową i efektywną cenę jednostkową w pliku dziennego użycia i potwierdzając, czy rabat jest stosowany.
- Tworzenie alertu Azure Monitor: alerty [](/azure/azure-monitor/platform/alerts-activity-log) dziennika aktywności można tworzyć przy użyciu usługi Azure Monitor w celu otrzymywania powiadomień o usunięciu dostępu RBAC z subskrypcji CSP. Zapoznaj się z przewodnikiem Opis środków uzyskane przez partnerów i dokumentacją techniczną.

## <a name="why-dont-i-see-pec-on-the-invoice"></a>Dlaczego na fakturze nie widzę PEC?

PEC nie jest jawnie wywoływana na fakturze i nie ma oddzielnej pozycji do wyświetlania PEC, jednak zarobki PEC są uwzględniane w skorygowanej kwoty opłat netto na fakturze. Aby dowiedzieć się więcej o tym, gdzie można wyświetlić szczegóły PEC, zobacz sekcje How is PEC paid (Jak są płatne PEC).

## <a name="next-steps"></a>Następne kroki

- [Cennik nowego środowisko handlowego dla Platforma Azure w programie CSP](azure-plan-price-list.md)
- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure](azure-plan-billing.md)
- [Przywracanie uprawnień administratora dla subskrypcji w ramach programu Azure CSP](revoke-reinstate-csp.md)
- [Punkty uzyskane przez partnerów — omówienie](partner-earned-credit.md)
- [Role, uprawnienia do środków uzyskane przez partnerów](azure-roles-perms-pec.md)
- [Informacje o środków uzyskane przez partnerów (przewodnik)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (wymagane logowanie)
