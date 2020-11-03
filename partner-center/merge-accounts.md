---
title: Merge your partner account with another partner account (Scalanie konta partnera z kontem innego partnera)
description: Dowiedz się, jak scalić konto partnerskie z innym kontem partnera w centrum partnerskim — w przypadku firm, które są aktywnymi partnerami firmy Microsoft w centrum partnerskim.
ms.topic: article
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: d38c11e564d6776a5755f8df40ba6ad2dca27d12
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530520"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Merge your partner account with another partner account (Scalanie konta partnera z kontem innego partnera)

**Odpowiednie role**

- Administrator konta

Dwie lub więcej firm, które są aktywnymi partnerami firmy Microsoft i mają konta w centrum partnerskim, mogą scalić swoje konta.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>Co się stanie, gdy dwaj partnerzy zdecydują się na scalenie kont Centrum partnerskiego

- Organizacja partnera, która inicjuje scalanie, będzie kontem globalnym partnera (PGA).

- PGA organizacji zaproszonej jest lokalizacją firmy inicjującej.

- Wszystkie lokalizacje scalanego konta stają się lokalizacjami w ramach PGA.

- Po zakończeniu scalania kont zobaczysz szczegóły konta, takie jak lokalizacje i użytkownicy w ramach profilu PGA. Nie można wycofać tego procesu.

- Wszystkie identyfikatory MPN dla lokalizacji są zachowywane podczas konsolidacji.

- Role użytkownika są przenoszone. Na przykład jeśli użytkownik był administratorem zachęt dla określonej lokalizacji, nadal będzie miał tę rolę po fuzji i będzie mógł zobaczyć zachęty, które wystąpiły przed połączeniem.

- Dzierżawy usługi Azure AD i konta CSP nie są scalone i nie mają żadnego wpływu.

- Opublikowane oferty i wspólne dane potokowe skojarzone z obiema firmami są zachowywane

### <a name="view-of-merged-accounts"></a>Widok scalonych kont

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Łączenie kont":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>Czego można oczekiwać, jeśli zaproszono Cię do scalania Twojego konta Centrum partnerskiego z innym kontem Centrum partnerskiego

W przypadku podjęcia decyzji o zaakceptowaniu zaproszenia do kont scalania: · Twoje identyfikatory i lokalizacje MPN zostaną scalone z PGA konta partnera, które zaprosiło.

- Użytkownicy zostaną przeniesieni do scalonego konta z nienaruszonymi rolami.

- Istniejące korzyści i kompetencje zostaną zachowane dla obu firm po fuzji do momentu odnowienia. W przypadku odnowienia konta będą traktowane jak jedna firma i standardowe reguły odnawiania.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Poznaj wpływ na programy i korzyści, gdy partnerzy zdecydują się na scalanie kont

- Wszystkie istniejące kompetencje (Gold/Silver), zakupy (takie jak Microsoft Action Pack) i skojarzone z nimi korzyści są zachowywane podczas konsolidacji. Jeśli obie firmy mają takie same kompetencje, ale jedna z nich jest złota, a druga Silver, zostanie przyznana kompetencja o najwyższym poziomie umiejętności, a partnerzy będą mieli jeden zestaw korzyści Silver i jeden zestaw korzyści Gold dla tej kompetencji do momentu kolejnego odnowienia. 

- Najpóźniejsza data rocznicy dla programu Microsoft Action Pack zostanie zachowana po scaleniu. Jeśli na przykład Data rocznicy dla firmy 1 to Czerwiec 2020 dla Action Pack odnowienia, a rocznica Action Pack odnowienia dla firmy 2 to 2020 października, firma Microsoft będzie używać daty 2020 od października jako nowej daty rocznicy dla Scalonej firmy.

- Podczas fuzji kont i do momentu następnego odnowienia każde konto będzie zachować swoje Action Pack i/lub korzyści z kompetencji. W przypadku odnowienia obowiązują standardowe Action Pack i reguły odnawiania kompetencji.

- Po odnowieniu korzyści związane z osiągnięciem kompetencji i Action Pack są implementowane dla konta globalnego partnera firmy partnerskiej:

  - Microsoft Action Pack: Firma partnerska będzie mogła zakupić jeden Action Pack na konto globalne partnera.

  - Kompetencje: Firma partnerska otrzyma jeden pakiet głównych korzyści, które są powiązane z największą osiągnięciem, oraz uprawnienia specyficzne dla kompetencji partnera dla konta globalnego partnera.

- Wszystkie korzyści są uzależnione od [przewodnika użytkowania Microsoft Partner Network korzyści](https://aka.ms/partner-benefits-use-guide). Na przykład: aktywowany token E3 usługi O365 jest funkcjonalny przez dwanaście (12) miesięcy po aktywacji. Po aktywowaniu tokenu dla licencji w dzierżawie te licencje mogą nie zostać przeniesione do innej dzierżawy.

- Skojarzenia identyfikatorów MCP dla obu firm zostaną zachowane i skojarzone z IDENTYFIKATORem MPN PGA.

- Korzyści ze stosowania na rynku i techniczne są oferowane jako korzyść z tytułu kompetencji podstawowych. Po scaleniu zaleca się sprawdzenie banku i informacji podatkowych w celu zapewnienia dokładności.

- Jeśli firma znajduje się w programie MSP platformy Azure, korzyści są zachowywane do momentu odnowienia.

- Jeśli firma uzyskała zaawansowane specjalizacje, są one zachowywane na obu kontach.

- Wszystkie załączniki programu Software Assurance są zachowywane na obu kontach. 

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Zaproś firmę do scalenia swojego konta Centrum partnerskiego z kontem Centrum partnerskiego

>[!Note]
>Aby można było wykonać operację łączenia, musisz być **administratorem konta** dla Twojej firmy.

1. Wybierz pozycję **Ustawienia** z pulpitu nawigacyjnego Centrum partnerskiego. 

2. Wybierz pozycję **scalanie kont** .

3. Dodaj identyfikator MPN, który znajduje się w **profilu partnera** konta, które chcesz zaprosić do scalenia. Musisz użyć identyfikatora MPN globalnego partnera. Nie można użyć identyfikatora MPN lokalizacji.

4. Po wybraniu opcji **Scal** zaproszenie jest wysyłane do firmy partnerskiej. Po zaakceptowaniu żądania można zainicjować scalanie kont w centrum partnerskim. Jeśli firma odrzuci żądanie scalania kont, może wyjaśnić, Dlaczego odrzucono żądanie. Lista wszystkich scalanych kont jest dostępna dla Ciebie w obszarze **historia scalania** .

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md)

- [Weryfikowanie informacji o profilu partnera](update-your-partner-profile.md)

- [Dodaj udostępnione usługi partnerskie platformy Azure, aby partnerzy mogli kupować subskrypcje platformy Azure pod kątem własnych potrzeb](shared-services.md)
