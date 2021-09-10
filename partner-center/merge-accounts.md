---
title: Merge your partner account with another partner account (Scalanie konta partnera z kontem innego partnera)
description: Dowiedz się, jak scalić konto partnera z innym kontem partnera w Partner Center — dla firm, które są aktywnymi partnerami firmy Microsoft w Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-account
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: ace5ad2dc75600f9085af3d0d7fcfa1036c2da6d
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958893"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Merge your partner account with another partner account (Scalanie konta partnera z kontem innego partnera)

**Odpowiednie role:** Administrator konta

Co najmniej dwie firmy, które są aktywnymi partnerami firmy Microsoft i mają konta w Partner Center mogą zdecydować się na scalenie swoich kont.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>Co się stanie, gdy dwóch partnerów zdecyduje się scalić Partner Center kont

- Organizacja partnerska, która inicjuje scalanie, będzie kontem globalnym partnera (PGA).

- Pga organizacji zapraszana staje się lokalizacją inicjatora firmy.

- Wszystkie lokalizacje scalanych kont stają się lokalizacjami w ramach konta PGA.

- Po zakończeniu łączenia kont zobaczysz szczegóły konta, takie jak lokalizacje i użytkownicy w profilu PGA. Nie można cofnąć tego procesu.

- Wszystkie identyfikatory MPN lokalizacji są zachowywane podczas tej konsolidacji.

- Role użytkownika są przejmyne. Jeśli na przykład użytkownik był administratorem zachęt dla określonej lokalizacji, nadal będzie miał tę rolę po zakończeniu koncentracji i będzie mógł zobaczyć zachęty, które zobaczyli przed rozpoczęciem koncentracji.

- Dzierżawy usługi Azure AD i konta CSP nie są scalane i nie mają żadnego efektu.

- Opublikowane oferty i dane potoku co-sell skojarzone z obiema firmami są zachowywane

### <a name="view-of-merged-accounts"></a>Widok scalonych kont

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Łączenie kont.":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>Czego można oczekiwać, jeśli zaproszono Cię do scalenia konta Partner Center z innym Partner Center kontem

Jeśli zdecydujesz się zaakceptować zaproszenie do scalenia kont: · Twoje identyfikatory MPN i lokalizacje zostaną scalone z kontem PGA konta partnera, które Cię zaprosiło.

- Użytkownicy zostaną wywniosci do scalonego konta bez zmian z ich rolami.

- Istniejące korzyści i kompetencje zostaną zachowane dla obu firm po zakończeniu koncentracji do czasu odnowienia. Podczas odnawiania konta będą traktowane jak jedna firma i będą stosowane standardowe reguły odnawiania.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Zrozumienie wpływu na programy i korzyści w przypadku, gdy partnerzy wybiorą scalanie kont

- Wszystkie istniejące kompetencje (Gold/Silver), zakupy (takie jak microsoft Action Pack) i powiązane korzyści są zachowywane podczas konsolidacji. Jeśli obie firmy mają taką samą kompetencję, ale jedna jest złoty, a druga silver, kompetencja o najwyższym poziomie zaawansowania zostanie nadana, a partnerzy będą mieli jeden zestaw korzyści w kategorii Silver i jeden zestaw złotych korzyści dla tej kompetencji do czasu ich następnego odnowienia. 

- Data najwyższej rocznicy dla Action Pack Microsoft zostanie zachowana po zakończeniu koncentracji. Jeśli na przykład data rocznicy dla firmy 1 to czerwiec 202 Action Pack 0 r. w przypadku odnowienia, a data rocznicy odnowienia dla firmy Action Pack to październik 2020 r., firma Microsoft użyje daty października 2020 r. jako nowej daty rocznicy dla scalonej firmy.

- Podczas koncentracji konta i do następnego odnowienia każde konto zachowuje swoje Action Pack i/lub kompetencji. Podczas odnawiania obowiązują Action Pack odnawiania kompetencji.

- Po odnowieniu korzyści, które są objęte poziomem kompetencji i Action Pack są implementowane dla konta globalnego partnera firmy partnerskiej:

  - Microsoft Action Pack: firma partnerska będzie mogła zakupić jeden pakiet Action Pack na konto globalne partnera.

  - Kompetencja: firma partnerska otrzyma jeden pakiet podstawowych korzyści skojarzonych z najwyższym poziomem wiedzy oraz korzyści specyficzne dla kompetencji, do których partner kwalifikuje się na globalne konto partnera.

- Wszystkie korzyści podlegają przewodnikowi [użycia Microsoft Partner Network korzyści.](https://aka.ms/partner-benefits-use-guide) Na przykład: aktywowany token usługi O365 E3 działa przez 12 miesięcy po aktywacji. Po aktywowaniu tokenu dla licencji w dzierżawie te licencje nie mogą zostać przeniesione do innej dzierżawy.

- Skojarzenia identyfikatorów MCP dla obu firm zostaną zachowane i skojarzone z identyfikatorem MPN PGA.

- Korzyści z wejścia na rynek i korzyści techniczne są oferowane jako podstawowa korzyść kompetencji. Po scaleniu zaleca się sprawdzenie informacji bankowych i podatkowych w celu zapewnienia dokładności.

- Jeśli Twoja firma jest w programie Azure Expert MSP, korzyści są zachowywane do czasu odnowienia.

- Jeśli Firma uzyskała zaawansowane specjalizacje, są one zachowywane na obu kontach.

- Wszystkie gwarancje programu Software Assurance są zachowywane na obu kontach. 

- Nie ma to wpływu na skojarzenie DPOR ani PAL. Wszelkie powiązane udziały w przychodach zaczną przepływać do nowego konta globalnego partnera

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Zaproś firmę do scalenia konta Partner Center z Twoim kontem Partner Center

>[!Note]
>Aby przeprowadzić połączenie konta, musisz być **administratorem konta** w swojej firmie.

1. Wybierz **Ustawienia** na pulpicie nawigacyjnym Partner Center nawigacyjnym. 

2. Wybierz **pozycję Scalanie konta.**

3. Dodaj identyfikator MPN znajdujący się w **profilu partnera** konta, które chcesz zaprosić do scalenia z Toem. Musisz użyć globalnego identyfikatora MPN partnera. Nie można użyć identyfikatora MPN lokalizacji.

4. Po wybraniu opcji **Scal** zaproszenie zostanie wysłane do firmy partnerskiej. Po zaakceptowaniu żądania możesz zainicjować scalanie konta w ramach Partner Center. Jeśli firma odrzuci Żądanie scalenia kont, może wyjaśnić, dlaczego żądanie zostało odrzucone. Lista wszystkich scaleń Twojego konta jest dostępna w obszarze **Historia scalania.**
 
### <a name="example-of-two-companies-merging-accounts"></a>Przykład scalania kont dwóch firm

1. Firma Contoso, Ltd. ma 

    a. globalny [identyfikator MPN 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) i jeden identyfikator [MPN](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)lokalizacji podrzędnej 2222222 .
  
    b. dzierżawa usługi Azure AD = @contoso.com
 
    c. gold competency, która wygasa 1 października 2020 r.
2. Firma Fabrikam, Inc. ma
 
    a.  globalny identyfikator MPN 3333333 dwa identyfikatory MPN lokalizacji podrzędnej 4444444 i 5555555

    b.  dzierżawa usługi Azure AD = @fabrikam.com

    c.  dwie złote kompetencje, które wygasną 1 grudnia 2020 r.
3.  Firma Contoso kupuje firmę Fabrikam i przechodzi [tutaj,](https://partner.microsoft.com/dashboard/account/merger) aby zainicjować żądanie scalenia.
4.  Firma Fabrikam Partner Center do tej samej strony, co firma Contoso w kroku #3, w celu zatwierdzenia żądania firmy Contoso.
5.  Firma Contoso przegląda szczegóły scalania na tej samej stronie i zapewnia potwierdzenie kontynuowania scalania kont.
6.  Po zakończeniu koncentracji konto firmowe będzie wyświetlane jako:

    a.  Firma o nazwie Contoso z globalnym identyfikatorem MPN 1111111 i 4 identyfikatorami MPN lokalizacji podrzędnej 2222222, 3333333, 4444444 i 5555555
    
    b.  Będzie ona mieć dwie dzierżawy usługi Azure AD ( + ), które mają dostęp do tego samego @contoso.com @fabrikam.com Partner Center konta
    
    c.  Będzie ona mieć dwa pakiety korzyści kompetencji: jeden, który wygasa 1 października 2020 r., i drugi, który wygasa 1 grudnia 2020 r. 1 grudnia 2020 r. będą mogli odnowić ten pakiet jako pojedynczy pakiet korzyści z kompetencji. Po odnowieniu firma Contoso zachowa wszystkie trzy kompetencje, mimo że może zachować tylko jeden pakiet korzyści.
    
7.  Administratorzy firmy Contoso będą nadal zarządzać rolami Partner Center dla @contoso.com użytkowników firmy. Administratorzy firmy Fabrikam będą nadal zarządzać rolami Partner Center @fabrikam.com użytkownikami firmy Fabrikam. Administratorzy firmy Contoso mogą administrować użytkownikami firmy Fabrikam tylko wtedy, gdy zostaną zaproszeni jako goście do dzierżawy firmy Fabrikam.
8.  Firma Contoso może zignorować dzierżawę i ponownie wyedytować pracownikom firmy Fabrikam nowe poświadczenia z nowymi rolami @fabrikam.com @contoso.com i uprawnieniami.

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md)

- [Weryfikowanie informacji o profilu partnera](update-your-partner-profile.md)

- [Dodaj Azure Partner Shared Services, aby partnerzy mogą kupować subskrypcje platformy Azure na własny użytek](shared-services.md)
