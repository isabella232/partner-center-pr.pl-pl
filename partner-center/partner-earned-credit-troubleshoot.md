---
title: Rozwiązywanie problemów ze środków uzyskane przez partnerów
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak rozwiązać problemy z fakturami i inne problemy dotyczące środków uzyskane przez partnerów.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: a8bb370c7154c8033990cac798c28e01eec7e17f
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593229"
---
# <a name="troubleshooting-partner-earned-credit"></a>Rozwiązywanie problemów ze środków uzyskane przez partnerów

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny | Administrator rozliczeń | Agent sprzedaży

## <a name="troubleshooting-guide"></a>Przewodnik rozwiązywania problemów

Jeśli masz problemy z PEC, takie jak dostęp lub brakujące informacje, sprawdź poniższe elementy w podanej kolejności.

1. Upewnij się, że patrzysz na fakturę G (Modern) i ponownie plik. Plan platformy Azure i PEC nie są wyświetlane na fakturze D (starsza wersja) ani w pliku rekonesfiguru.

2. Zidentyfikuj typ partnera. (Odsprzedawcy pośredni nie są uprawnieni).

3. Upewnij się, że umowa MPN jest aktywna.

4. W przypadku dostawców pośrednich upewnij się, że identyfikator MPN odsprzedawcy wprowadzony w Partner Center (lub za pośrednictwem interfejsu API) odpowiada identyfikatorowi MPN odsprzedawcy wprowadzonego w Azure Portal.

5. Potwierdź, że Twoja oferta kwalifikuje się. (Stare oferty platformy Azure, wystąpienia zarezerwowane platformy Azure i produkty innych firm nie kwalifikują się).

6. Upewnij się, że masz prawidłową rolę Administrowanie w imieniu (AOBO) lub Role-Based Access Control (RBAC) dla subskrypcji/grupy zasobów/zasobu.

7. Ustal, czy klient usunął Twoją rolę RBAC. Jeśli tak, zobacz Przywróć uprawnienia administratora dla subskrypcji Azure CSP klienta

8. Upewnij się, że masz dostęp administratora przez cały dzień.

9. Upewnij się, że przeglądasz poprawne kolumny w pliku dziennego użycia.

## <a name="next-steps"></a>Następne kroki

- [Cennik nowego środowisko handlowego dla Platforma Azure w programie CSP](azure-plan-price-list.md)
- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
- [Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure](azure-plan-billing.md)
- [Przywracanie uprawnień administratora dla subskrypcji w ramach programu Azure CSP](reinstate-csp.md)
- [Środków uzyskane przez partnerów — omówienie](partner-earned-credit.md)
- [Role, uprawnienia do środków uzyskane przez partnerów](azure-roles-perms-pec.md)
- [Informacje o środków uzyskane przez partnerów (przewodnik)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (wymagane logowanie)
