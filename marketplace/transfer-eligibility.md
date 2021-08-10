---
title: Uprawnienia do przeniesienia — wskazówki dotyczące przenoszenia subskrypcji między kontami rozliczeniowymi, Azure Marketplace
description: Wytyczne dotyczące testów komercyjnych przed przeniesieniem subskrypcji między kontami rozliczeniowymi w Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 22c53238fd74501f32a56d66f15133cbbe8765cffe67a04c4f66779c15b16c37
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688321"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Przenoszenie uprawnień do subskrypcji między kontami rozliczeniowymi

Subskrypcję [można przenieść z](/azure/cost-management-billing/understand/subscription-transfer) jednego konta rozliczeniowego na inne w sekcji rozliczeń Azure Portal. Przed przeniesieniem subskrypcja jest skanowana w celu skanowania produktów innych firm. Przeniesienie jest dozwolone tylko wtedy, *gdy wszystkie* produkty zostaną wyczyszone do przeniesienia (zobacz [poniższe](#criteria-for-transfer-approval-or-denial) kryteria). System wygeneruje odpowiednie komunikaty o błędach dla aplikacji, których wyczyszczenie nie powiodło się, aby ułatwić określenie następnych kroków.

> [!NOTE]
> Ten artykuł nie dotyczy ofert SaaS, ponieważ zasoby SaaS są dołączone do dzierżawy, a nie subskrypcji. Zasoby SaaS można przenosić z jednego konta rozliczeniowego na inne, ale odbywa się to dla każdego zasobu i pomocy technicznej platformy Azure jako wniosek o pomoc techniczną.

## <a name="criteria-for-transfer-approval-or-denial"></a>Kryteria zatwierdzania lub odmowy przeniesienia

Nie można przenieść subskrypcji, jeśli którakolwiek z jej aplikacji innych firm spełnia dowolne z następujących kryteriów:

- Konto docelowe jest komercyjne, a aplikacja nie może być sprzedawana za pośrednictwem partnerów.
- Aplikacja ma zgodę dla wybranych partnerów, a konto docelowe nie znajduje się na liście zezwalań.
- Ta oferta była ofertą w wersji zapoznawczej w przeszłości dla wybranych subskrypcji lub była ofertą prywatną, a subskrypcja nie znajduje się już na liście zezwalań.
- Nowe konto rozliczeniowe znajduje się w regionie innym niż sprzedaż oferty, a oferta nie ma być sprzedawana w tym regionie.

Zablokowany transfer pozostaje w mocy, dopóki nie usuniesz zasobu z subskrypcji, po czym możesz spróbować ponownie wykonać przeniesienie.

## <a name="next-steps"></a>Następne kroki

[Uzyskaj pomoc techniczną Microsoft AppSource i Azure Marketplace](get-support.md)

