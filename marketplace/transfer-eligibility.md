---
title: Uprawnienie do transferu — wskazówki dotyczące przenoszenia subskrypcji między kontami rozliczeniowymi, Azure Marketplace
description: Wskazówki dotyczące kontroli komercyjnej przed przeniesieniem subskrypcji między kontami rozliczeń w Azure Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007533"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Przenoszenie uprawnień do subskrypcji między kontami rozliczeniowymi

[Subskrypcję można przenieść](/azure/cost-management-billing/understand/subscription-transfer) z jednego konta rozliczeniowego do innego w sekcji Rozliczenia w Azure Portal. Przed przeniesieniem subskrypcja jest skanowana pod kątem produktów innych firm. Transfer jest dozwolony tylko wtedy, gdy *wszystkie* produkty są wyczyszczone do przeniesienia (patrz poniższe [kryteria](#criteria-for-transfer-approval-or-denial) ). System wygeneruje odpowiednie komunikaty o błędach dla aplikacji, które nie zostały wyczyszczone, aby pomóc w ustaleniu następnych kroków.

> [!NOTE]
> Ten artykuł nie dotyczy ofert SaaS, ponieważ zasoby SaaS są dołączone do dzierżawy, a nie do subskrypcji. Zasoby SaaS są przenoszone z jednego konta rozliczeniowego do innego, ale jest to wykonywane dla każdego zasobu i pomocy technicznej platformy Azure jako żądania pomocy technicznej.

## <a name="criteria-for-transfer-approval-or-denial"></a>Kryteria zatwierdzania transferu lub odmowy

Nie można przenieść subskrypcji, Jeśli którakolwiek z jej aplikacji innych firm spełnia następujące kryteria:

- Konto docelowe jest komercyjne, a aplikacja jest niedostępna do sprzedaży przez partnerów.
- Aplikacja jest opcjonalna dla wybranych partnerów, a konto docelowe nie znajduje się na liście dozwolonych.
- Oferta była ofertą wersji zapoznawczej w przeszłości dla wybranych subskrypcji lub była ofertą prywatną, a subskrypcja nie znajduje się już na liście dozwolonych.
- Nowe konto rozliczeniowe znajduje się w regionie innym niż miejsce sprzedaży oferty i oferta nie jest sprzedawana w tym regionie.

Zablokowany transfer nadal obowiązuje do momentu usunięcia zasobu z subskrypcji, po upływie którego można ponowić próbę przeniesienia.

## <a name="next-steps"></a>Następne kroki

[Uzyskaj pomoc techniczną dla Microsoft AppSource i witryny Azure Marketplace](get-support.md)

