---
title: Migrowanie firm z pmc do Partner Center
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Co należy wiedzieć w przypadku migracji wielu firm z Partner Membership Center (PMC) do Partner Center i skonsolidowania ich na globalnym koncie partnera.
author: parthpandyaMSFT
ms.author: ParthP
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2c9973bf82957cd017abfc59c25b0c17173cb3f8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151597"
---
# <a name="moving-multiple-companies-to-partner-center-from-partner-membership-center-pmc"></a>Przenoszenie wielu firm do Partner Center z Partner Membership Center (PMC)

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży

Podczas przenoszenia konta firmy z witryny PMC do Centrum partnerskiego może być konieczne przeniesienie kilku kont. W Partner Center te konta zostaną skonsolidowane na jednym koncie globalnym (PGA). Pierwsze konto, które przeniesiesz, będzie traktowane jako konto globalne partnera, a wszystkie kolejne konta zostaną skonsolidowane na pierwszym koncie jako lokalizacje. Rozpocznij przenoszenie przy użyciu konta PMC dla siedzibie firmy. Aby uzyskać więcej informacji, zobacz Przewodnik migracji z [usługi PMC](guide-to-migration.md) do usługi Partner Center lub obejrzyj ten krótki klip wideo, w którym konta z [wieloma lokalizacjami zostały łatwe.](https://vimeo.com/290335248)

## <a name="move-your-additional-accounts-into-partner-center"></a>Przenoszenie dodatkowych kont do Partner Center

Ponieważ jedno konto firmowe zostało już przeniesione do Partner Center, gdy się zalogujesz, powiesz, które konto znajduje się już w Partner Center.

Po migracji, jeśli odkryjesz, że niewłaściwe konto firmowe zostało wyznaczone jako firma prawna, możesz zmienić to oznaczenie.

1. Przejdź do profilu **partnera.**

2. Upewnij się, że lokalizacja, którą chcesz wyznaczyć jako Legal business, znajduje się na liście lokalizacji. Jeśli tak nie jest, dodaj go.

3. Wybierz **pozycję Aktualizuj legalny profil biznesowy.**

4. Wybierz firmę i region i zapisz je.

:::image type="content" source="images/migration/accountwithus.png" alt-text="Istniejące konto":::

## <a name="your-company-has-an-account-in-partner-center"></a>Twoja firma ma konto w Partner Center

Zobaczysz istniejące konto i notatkę z informacją, że szczegóły Twojej firmy (konto, za pomocą których aktualnie się logujesz) zostaną skonsolidowane na tym koncie.

:::image type="content" source="images/migration/existingaccount2.png" alt-text="Konto w Partner Center":::

Na tym ekranie przedstawiono szczegóły istniejącego konta (nazwę i adres), które zostało już utworzone w u Partner Center wraz ze szczegółami kontaktu podstawowego.

Wybierz opcję **Kontynuuj**.

## <a name="what-happens-during-consolidation-of-accounts"></a>Co się dzieje podczas konsolidacji kont

- Na tym ekranie nie można zmienić żadnych szczegółów.

- Konto w chmurze PMC (obecnie przenoszące się) zostanie skonsolidowane z istniejącym kontem

- Twoja HQ i wszystkie lokalizacje w centrum pmc zostaną przeniesione na to istniejące konto Partner Center jako lokalizacje

- Po zakończeniu konsolidacji wszystkie szczegóły konta będą widzieć jako lokalizacje w ramach istniejącego Partner Center konta

- Wszystkie identyfikatory MPN są zachowywane podczas tej konsolidacji

- Wszystkie istniejące kompetencje (Gold/Silver), zakupy (MAPS/Gold/Silver) i powiązane korzyści są zachowywane podczas konsolidacji

- Ty (użytkownik, który zalogował się przy użyciu służbowego identyfikatora poczty e-mail) zostanie automatycznie dodany jako administrator MPN i administrator konta do istniejącego konta usługi Partner Center, aby można było administrować kontem zgodnie z potrzebami

## <a name="review-your-company-information"></a>Przeglądanie informacji o firmie

Sprawdź informacje o firmie i w razie potrzeby edytuj je.  Te szczegóły będą używane do migrowania konta do Partner Center, dlatego upewnij się, że szczegóły są poprawne.

Szczegółowe informacje są oparte na informacjach w chmurze pmc i zostaną zweryfikowane w celu zapewnienia, że firma jest uzasadniona.


:::image type="content" source="images/migration/review.png" alt-text="Przeglądanie szczegółów":::

Jeśli konto, które przenosisz, znajduje się w tym samym kraju lub regionie co istniejące konto, możesz zdecydować, czy chcesz użyć tego adresu, czy dodać inny. Jeśli zdecydujesz się użyć innego adresu, ten adres zostanie zweryfikowany. Jeśli chcesz użyć tego samego adresu, zostanie użyty istniejący adres i kontakt podstawowy.

Po zweryfikowaniu/edytowaniu informacji na tym ekranie wybierz pozycję **Prześlij.** Twoje konta zostaną skonsolidowane.

## <a name="partner-profile"></a>Profil partnera

Podczas wyświetlania profilu zobaczysz informacje dotyczące twojej firmy prawnej (w chmurze PMC, w tej siedzibie) oraz informacje dotyczące wszystkich dodatkowych lokalizacji.

## <a name="next-steps"></a>Następne kroki

- [Przenoszenie z witryny PMC do Centrum partnerskiego](move-pmc-pc-map.md)
- [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md)
- [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md)
- [Zarządzanie programami członkostwa](renew-mpn-offers.md)
- [Tworzenie profilu biznesowego firmy](create-a-marketing-profile.md)
- [Nawiązywanie połączenia z klientami za pośrednictwem poleceń](manage-leads.md)
