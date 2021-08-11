---
title: Przenoszenie subskrypcji platformy Azure w ramach planu platformy Azure do innego partnera CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się, jak Dostawca rozwiązań w chmurze partner programu skojarzonego z subskrypcjami platformy Azure klienta w ramach planu platformy Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 3b1f2213537a0a62b60d14b8209ba5c8a71a2a5f702476cefdb7845c7c6e5438
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115695519"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-csp-under-an-azure-plan"></a>Przenoszenie subskrypcji platformy Azure klienta do innego programu CSP (w ramach planu platformy Azure)

**Odpowiednie role:** Administrator konta | Agent sprzedaży | Agent rozliczeń

W tym artykule opisano, jak klienci mogą zmieniać swoje subskrypcje platformy Azure z jednego partnera w programie Dostawca rozwiązań w chmurze (CSP) na inny w ramach planu platformy Azure.

Aby przełączyć subskrypcje platformy Azure klienta od innego partnera, wykonaj następujące kroki. Bieżący partner, przyszły partner i klient mają kroki do wykonania.

> [!Note]  
> Tylko partnerzy, którzy mają bezpośrednią relację rozliczeń z firmą Microsoft, mogą uzyskać dostęp do narzędzia przejściowego. Odsprzedawcy pośredni muszą współpracować ze swoimi dostawcami pośrednimi, aby korzystać z tego narzędzia przejściowego.

Zanim będzie można użyć narzędzia przejścia, klient musi komunikować się zarówno z bieżącym, jak i przyszłym partnerem. Aby uniknąć nieporozumień i rezygnacji, musi nastąpić konwersacja w trybie offline. Partnerzy i klienci powinni zrozumieć następujące zagadnienia i wymagania wstępne przed rozpoczęciem przejścia.

## <a name="considerations"></a>Zagadnienia do rozważenia

- Rezerwacje platformy Azure nie będą przenosine z subskrypcją do przyszłego partnera.
- Cennik programu CSP dla usług platformy Azure w ramach bieżącego partnera nie będzie się przesłonił.
- W przypadku przeniesienia poprzednich subskrypcji ofert platformy [Azure (MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) te subskrypcje platformy Azure zostaną jednocześnie przekonwertowane na nowe subskrypcje ofert platformy Azure w ramach planu platformy Azure.
- Obowiązki pomocy technicznej klienta zostaną przeniesieni do przyszłego partnera.
- Rozliczenia i fakturowanie zostaną przeniesione do przyszłego partnera po przeniesieniu subskrypcji.
- Transfery nie mają wpływu na kontrolę dostępu opartą na rolach (RBAC) platformy Azure.
- Administrator w imieniu (AOBO) nie zostanie przyznany domyślnie przyszłego partnera.
- Produkty innych Azure Marketplace będą transferowe, o ile produkty przejdą weryfikację Azure Marketplace uprawnień.
    - Nie ma żadnych specjalnych rabatów ani ograniczeń regionalnych.
    - Produkty nie są oparte na subskrypcji.
    - Przyszły partner powinien współpracować z wydawcą, aby upewnić się, że znajduje się on na liście zezwalania na wdrożenie produktu.
    - Jeśli którykolwiek z tych warunków nie zostanie spełniony, Azure Marketplace produkty powinny zostać anulowane. Następnie subskrypcje platformy Azure powinny zostać przeniesione, a Azure Marketplace powinny zostać zakupione u nowego partnera.

## <a name="prerequisites"></a>Wymagania wstępne

- Klient powiadamia bieżącego partnera CSP o zamiarze przejścia.
- Przyszły partner CSP współpracuje z klientem w celu zapewnienia, że można spełnić potrzeby klientów.
- Przyszły partner CSP ustanawia relację z klientem i kupuje plan platformy Azure przed rozpoczęciem przejścia.
- Klient podpisuje Umowa z Klientem Microsoft z przyszłym partnerem CSP.
- Przyszły partner CSP podpisuje Microsoft Partner Agreement przed użyciem narzędzia przejścia.

> [!NOTE]
> Samoobsługowego narzędzia przejściowego można używać, gdy bieżący partner klienta ma poprzednią ofertę platformy Azure (MS-AZR-0145p) lub nową ofertę platformy Azure (plan platformy Azure). W obu przypadkach po zakończeniu przenoszenia subskrypcje platformy Azure będą podlegać planowi platformy Azure z przyszłym partnerem.

## <a name="customer-tasks"></a>Zadania klientów

Aby przenieść subskrypcje platformy Azure, klient musi rozpocząć proces, kontaktując się z bieżącym partnerem. Klient powinien zebrać nazwę firmy bieżącego partnera i identyfikator Microsoft, aby przyszła partnerka może wypełnić formularz żądania przeniesienia w imieniu klienta.

Klienci muszą również zidentyfikować subskrypcje, które chcą przenieść od bieżącego partnera. Nie można zmieniać partnerów dla Office 365, Enterprise Mobility Suite ani Microsoft Dynamics CRM subskrypcji.

> [!NOTE]  
> Przyszła odpowiedzialność partnera za ukończenie formularza żądania przeniesienia, który inicjuje proces transferu. Firma Microsoft nie może interweniować w imieniu klienta ani bieżącego partnera. Klient powinien zaplanować ścisłą pracę z przyszłymi i bieżącymi partnerami, aby zapewnić bezproblemowe przejście.

## <a name="future-partner-tasks"></a>Przyszłe zadania partnerów 

Przyszły partner subskrypcji musi wypełnić formularz żądania przeniesienia z Partner Center żądania przeniesienia subskrypcji:

1.  W okienku po lewej Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, dla którego chcesz ukończyć żądanie przeniesienia.
2.  W menu specyficznym dla klienta wybierz **pozycję Subskrypcje.**
3.  Na karcie **Żądania przeniesienia** wybierz pozycję Dodaj **nowe żądanie:**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Zrzut ekranu przedstawiający kartę Żądania przeniesienia.":::

5.  Wypełnij formularz **Nowe żądanie przeniesienia:**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Zrzut ekranu przedstawiający formularz Nowe żądanie przeniesienia.":::

6.  Wybierz **pozycję Wyślij żądanie przeniesienia**  >  **Wyślij**.

7.  Przejrzyj potwierdzenie żądania przeniesienia:

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Zrzut ekranu przedstawiający potwierdzenie żądania przeniesienia.":::

    > [!NOTE]
    > Przyszły partner może anulować żądanie przeniesienia, wybierając pozycję **Anuluj** żądanie w prawym górnym rogu okna tylko wtedy, gdy żądanie przeniesienia ma stan "oczekujące". Gdy stan żądania przeniesienia będzie "w toku" lub "ukończony", anulowanie nie będzie możliwe.

## <a name="current-partner-tasks"></a>Bieżące zadania partnerów 

Agent administratora bieżącego partnera dla klienta otrzyma wiadomość e-mail z informacją, że klient żąda przeniesienia subskrypcji:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Zrzut ekranu przedstawiający powiadomienie e-mail o żądaniu przeniesienia przez klienta.":::

Bieżący partner musi przejrzeć i zaakceptować formularz żądania przeniesienia od Partner Center, aby ukończyć przenoszenie subskrypcji.

> [!NOTE]  
> Jeśli bieżący partner nie odpowie w ciągu 30 dni, żądanie wygaśnie, a przyszły partner będzie musiał utworzyć nowe żądanie przeniesienia.

1. Wykonaj jedno z następujących działań: 
   - Wybierz **pozycję Przejrzyj żądanie przeniesienia w** wiadomości e-mail.

     lub

    - W okienku po lewej Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, dla którego przesłano żądanie przeniesienia.
      1. W menu specyficznym dla klienta wybierz **pozycję Subskrypcje.**
      1. Na karcie **Żądania przeniesienia** rozwiń informacje o transferze, wybierając pozycję Identyfikator żądania przeniesienia **w** obszarze **Odebrane żądania:**

      :::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Zrzut ekranu przedstawiający kartę Żądania przeniesienia, widzianą przez bieżącego partnera.":::

5. Przejrzyj żądanie przeniesienia. Wybierz żądane subskrypcje platformy Azure do przeniesienia.
 
   Przed kontynuowaniem zwróć uwagę na:
   - Nie będziesz już mieć dostępu do wybranych subskrypcji.
   - Dalsze użycie nie zostanie zafakturowane.
   - Rezerwacje platformy Azure nie są transferowe z subskrypcjami.

6. Wybierz **pozycję Akceptuj i przenieś,** aby zakończyć proces transferu:

   :::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Zrzut ekranu przedstawiający ekran Przeglądanie żądania przeniesienia.":::

   Jeśli masz klienta z poprzednimi subskrypcjami ofert platformy Azure (MS-AZR-0145p), kontynuuj w ten sam sposób, wybierając subskrypcje do przeniesienia, a następnie wybierając pozycję **Akceptuj** i przenieś, aby zakończyć proces przenoszenia.

7. Wyświetl potwierdzenie akceptacji przeniesienia.

   W tym momencie wiadomość e-mail powiadamia przyszłego partnera, klienta i bieżącego partnera o zaakceptowanym żądaniu przeniesienia.

   Po zaakceptowaniu przeniesienia stan transferu może pozostać "oczekujący" przez maksymalnie 15 minut podczas aktualizowania systemu. Jeśli ten proces trwa dłużej, system będzie próbował przez trzy dni. Jeśli stan przeniesienia pozostanie w stanie "oczekujące" przez dłużej niż trzy dni, partner powinien przesłać żądanie obsługi.

   Po zakończeniu przenoszenia subskrypcje uwzględnione w żądaniu pojawią się w planie platformy Azure przyszłego partnera. Nie będzie ona już wymieniona u bieżącego partnera.

>[!Note]  
>Dostawcy pośredni powinni poinformować odsprzedawców pośrednich, że żądanie przeniesienia zostało zaakceptowane.

### <a name="managing-your-transferred-customer-subscriptions"></a>Zarządzanie przeniesionymi subskrypcjami klientów

Przejście nie wpływa na dostęp do istniejących użytkowników, grup lub jednostki usługi, które zostały przypisane za pośrednictwem kontroli dostępu na poziomie ról platformy Azure. [Usługa Azure RBAC](/azure/role-based-access-control/overview) pomaga klientom zarządzać tym, kto ma dostęp do zasobów platformy Azure, co może zrobić z tymi zasobami i do jakich obszarów ma dostęp. 

Jako nowy partner nie będziesz mieć żadnego dostępu RBAC do zasobów klienta po przeniesieniu subskrypcji. Poprzedni partner klienta zachowuje dostęp RBAC. We współpracy z klientem dowiedz się, kto ma wgląd w subskrypcje i jak wprowadzić wszelkie potrzebne zmiany.

Klient będzie musiał usunąć dostęp RBAC platformy Azure dla poprzedniego partnera i dodać dostęp dla Ciebie. Aby uzyskać więcej informacji na temat zapewniania dostępu, zobacz Co to jest kontrola dostępu na podstawie ról [(RBAC) platformy Azure?.](/azure/role-based-access-control/overview) Aby uzyskać więcej informacji na temat usuwania dostępu, [zobacz Usuwanie przypisania roli](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

Ponadto nie uzyskujesz automatycznie dostępu [administratora w imieniu (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) do subskrypcji. Usługa AOBO jest niezbędna, aby można było zarządzać subskrypcjami platformy Azure klienta. Aby uzyskać więcej informacji na temat uprawnień platformy Azure, zobacz [Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta](./customers-revoke-admin-privileges.md).

## <a name="next-steps"></a>Następne kroki

- [Kontrola dostępu na podstawie ról platformy Azure](/azure/role-based-access-control/overview)
- [Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta](./customers-revoke-admin-privileges.md)
