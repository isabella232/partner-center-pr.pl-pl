---
title: Uprawnienia do przeniesienia — wskazówki dotyczące przenoszenia subskrypcji między kontami rozliczeniowymi i Azure Marketplace
description: Wytyczne dotyczące testów komercyjnych przed przeniesieniem subskrypcji między kontami rozliczeniowymi w Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247245"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Przenoszenie uprawnień do subskrypcji między kontami rozliczeniowymi

Subskrypcję [można przenieść z](/azure/cost-management-billing/understand/subscription-transfer) jednego konta rozliczeniowego na inne w sekcji rozliczeń Azure Portal. Przed przeniesieniem subskrypcja jest skanowana w celu skanowania produktów innych firm. Przeniesienie jest dozwolone tylko wtedy, *gdy wszystkie* produkty zostaną wyczyszone do przeniesienia (zobacz [poniższe](#criteria-for-transfer-approval-or-denial) kryteria). System wygeneruje odpowiednie komunikaty o błędach dla aplikacji, których wyczyszczenie nie powiodło się, aby ułatwić określenie następnych kroków.

> [!NOTE]
> Ten artykuł nie dotyczy ofert SaaS, ponieważ zasoby SaaS są dołączone do dzierżawy, a nie subskrypcji. Zasoby SaaS można przenosić z jednego konta rozliczeniowego na inne, ale odbywa się to dla każdego zasobu i przez pomoc techniczną platformy Azure jako żądanie pomocy technicznej.

## <a name="criteria-for-transfer-approval-or-denial"></a>Kryteria zatwierdzania lub odmowy transferu

Nie można przenieść subskrypcji, jeśli którakolwiek z jej aplikacji innych firm spełnia dowolne z następujących kryteriów:

- Konto docelowe jest komercyjne, a aplikacja zrezygnuje z jego sprzedaży za pośrednictwem partnerów.
- Aplikacja jest wybrańcem wybranych partnerów, a konto docelowe nie znajduje się na liście zezwalań.
- Ta oferta była ofertą w wersji zapoznawczej w przeszłości dla wybranych subskrypcji lub była ofertą prywatną, a subskrypcja nie znajduje się już na liście zezwalań.
- Nowe konto rozliczeniowe znajduje się w regionie innym niż sprzedaż oferty, a oferta nie ma być sprzedawana w tym regionie.

Zablokowany transfer pozostaje w mocy do momentu usunięcia zasobu z subskrypcji, po którym można spróbować ponownie wykonać przeniesienie.

## <a name="next-steps"></a>Następne kroki

[Uzyskaj pomoc techniczną Microsoft AppSource i Azure Marketplace](get-support.md)

