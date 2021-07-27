---
title: Przenoszenie subskrypcji platformy Azure w ramach planu platformy Azure do innego partnera CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak Dostawca rozwiązań w chmurze programu partnerskiego skojarzonego z subskrypcjami platformy Azure klienta w ramach planu platformy Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 258b593935e9fd599e0f5c524cd7ec935c50bcad
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434136"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-in-csp-under-an-azure-plan"></a>Przenoszenie subskrypcji platformy Azure klienta do innego partnera w programie CSP (w ramach planu platformy Azure)

**Odpowiednie role:** Administrator konta | Agent sprzedaży | Agent rozliczeń

W tym artykule opisano, jak klient może przełączać swoje subskrypcje platformy Azure z jednego partnera w ramach Dostawca rozwiązań w chmurze (CSP) na innego w ramach planu platformy Azure.

Aby przełączyć subskrypcje platformy Azure klienta z innego partnera, wykonaj następujące kroki. Zarówno partner, jak i klient mają kroki do wykonania.

> [!Note]  
> Tylko partnerzy z bezpośrednią relacją rozliczeń z firmą Microsoft mogą uzyskać dostęp do narzędzi przejścia. Odsprzedawcy pośredni muszą współpracować z dostawcami pośrednimi, aby korzystać z tego narzędzia przejściowego.

Przed rozpoczęciem tego narzędzia klient musi być w rozmowie z partnerami (bieżącymi i przyszłymi). Konwersacja w trybie offline musi wymagać uniknięcia nieporozumień i rezygnacji. Ponadto partnerzy i klienci powinni zrozumieć te zagadnienia i wymagania wstępne przed zainicjowanie przejścia:

**Najważniejsze kwestie do rozważenia:**

- Rezerwacje platformy Azure nie zostaną przeniesiene z subskrypcją do przyszłego partnera
- Cennik programu CSP dla usług platformy Azure w ramach bieżącego partnera nie zostanie przejściowy
- Przeniesienie poprzednich subskrypcji oferty platformy [Azure (MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) spowoduje jednoczesne przekonwertowanie tych subskrypcji platformy Azure na nowe subskrypcje ofert platformy Azure w ramach planu platformy Azure
- Obowiązki pomocy technicznej dla klienta zostaną przeniesieni do przyszłego partnera
- Rozliczenia i fakturowanie zostaną przeniesieni do przyszłego partnera w momencie przeniesienia
- Transfer Role-Based Access Control nie ma wpływu na usługę Azure Role-Based Access Control (RBAC)
- Administrator w imieniu (AOBO) nie zostanie przyznany domyślnie przyszłego partnera
- Produkty innych firm na platformie handlowej zostaną przesłonene tak długo, jak długo produkty przejdą sprawdzanie uprawnień do korzystania z witryny Marketplace.
    - Nie ma żadnych specjalnych rabatów ani ograniczeń regionalnych
    - Produkty nie są oparte na subskrypcji
    - Przyszły partner powinien współpracować z wydawcą, aby upewnić się, że jest na liście zezwalania na wdrożenie produktu
    - Jeśli nie wszystkie z tych warunków zostaną spełnione, aby przenieść produkty z witryny Marketplace, należy je anulować, przenieść subskrypcje platformy Azure, a następnie ponownie wykupić produkty z witryny Marketplace u nowego partnera

**Wymagania wstępne:**

- Klient kontaktuje się z bieżącym partnerem CSP w sprawie zamiaru przejścia
- Przyszły partner CSP współpracuje z klientem w celu zapewnienia, że można spełnić potrzeby klientów
- Przyszły partner CSP ustanawia relację z klientem i kupuje plan platformy Azure przed rozpoczęciem przejścia  
- Klient musi podpisać umowę Umowa z Klientem Microsoft z przyszłym partnerem CSP
- Aby można było korzystać z tego narzędzia, przyszły Microsoft Partner Agreement CSP musi podpisać umowę

> [!NOTE]
> Tych samoobsługowych narzędzi można używać, gdy bieżący partner klienta ma poprzednią ofertę platformy Azure (MS-AZR-0145p) lub nową ofertę platformy Azure (plan platformy Azure). W obu przypadkach ukończenie tego przeniesienia spowoduje subskrypcje platformy Azure w ramach planu platformy Azure z przyszłym partnerem.

## <a name="customer-tasks-to-be-completed"></a>Zadania klienta do wykonania

Aby przenieść subskrypcje platformy Azure, klient musi rozpocząć proces, kontaktując się ze swoim bieżącym partnerem. Powinni zebrać nazwę firmy i identyfikator Microsoft bieżącego partnera, aby przyszły partner może wypełnić formularz żądania przeniesienia w jego imieniu.

Klient musi również zidentyfikować subskrypcje, które chce przenieść od bieżącego partnera. Nie można zmieniać partnerów dla Office 365, Enterprise Mobility Suite ani Microsoft Dynamics CRM subskrypcji.

> [!NOTE]  
> Odpowiedzialność za ukończenie formularza żądania przeniesienia, który inicjuje proces transferu, spoczywa na przyszłym partnerze. Firma Microsoft nie może interweniować w imieniu klienta lub bieżącego partnera. Klient powinien zaplanować ścisłą współpracę ze swoim przyszłym i bieżącym partnerem, aby przejście przebiegało bezproblemowo.

## <a name="future-partner-tasks-to-be-completed"></a>Przyszłe zadania partnerów do wykonania

Przyszły partner subskrypcji musi wypełnić formularz żądania przeniesienia od firmy Partner Center zażądać przeniesienia subskrypcji:

1.  Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, dla których chcesz wypełnić formularz żądania przeniesienia.
2.  W menu Customer (Klient) wybierz **pozycję Subscriptions (Subskrypcje).**
3.  Wybierz **sekcję Żądanie** przeniesienia.
4.  W **sekcji Żądanie przeniesienia wybierz** pozycję **Dodaj nowe żądanie.**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sekcja Transfery.":::

5.  Wypełnij formularz **Nowe żądanie przeniesienia.**

6.  Wybierz **pozycję Wyślij żądanie przeniesienia**  >  **Wyślij**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Wypełnij formularz żądania przeniesienia.":::

7.  Przegląd potwierdzenia żądania przeniesienia

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Przejrzyj oczekujące przeniesienie.":::

    > [!NOTE]
    > Przyszły partner może anulować żądanie przeniesienia, wybierając **pozycję** Anuluj żądanie w prawym górnym rogu tylko wtedy, gdy stan żądania przeniesienia to "oczekujące". Gdy stan żądania przeniesienia będzie "w toku" lub "ukończony", anulowanie nie będzie możliwe.

## <a name="current-partner-tasks-to-be-completed"></a>Bieżące zadania partnerów do wykonania

Agent administracyjny bieżącego partnera klienta otrzyma wiadomość e-mail z żądaniem przeniesienia subskrypcji przez klienta:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Który napisze recenzję.":::

Przejrzyj i zaakceptuj formularz żądania przeniesienia od Partner Center, aby ukończyć przenoszenie subskrypcji.

> [!NOTE]  
> Jeśli bieżący partner nie zostanie podjęty w ciągu 30 dni, żądanie wygaśnie, a przyszły partner będzie miał żądanie utworzenia nowego żądania przeniesienia.

- Wybierz **pozycję Przejrzyj żądanie przeniesienia w** wiadomości e-mail

   -lub-

1. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta, w imieniu których przesłano żądanie przeniesienia.
2. W menu Customer (Klient) wybierz **pozycję Subscriptions (Subskrypcje).**
3. Wybierz **sekcję Żądanie** przeniesienia.
4.Rozwiń informacje o transferze, wybierając wybrany **identyfikator żądania przeniesienia w** obszarze **Odebrane żądania**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Żądanie przeniesienia przeglądów źródła.":::

5. Przejrzyj żądanie przeniesienia. Wybierz żądane subskrypcje platformy Azure do przeniesienia.
 
Przed przystąpieniem do pracy należy pamiętać, że:
- Nie będziesz już mieć dostępu do wybranych subskrypcji.
- Dalsze użycie nie zostanie zafakturowane.
- Rezerwacje platformy Azure nie są transferowe z subskrypcjami.

6. Następnie wybierz **pozycję Zaakceptuj i przenieś,** aby zakończyć proces przenoszenia.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Wybierz subskrypcje do przeniesienia w ramach planów platformy Azure.":::

Jeśli bieżący partner ma klienta z poprzednimi subskrypcjami ofert platformy Azure (MS-AZR-0145p), będzie on kontynuować w ten sam sposób, wybierając subskrypcje do przeniesienia, a następnie wybierając pozycję Akceptuj i przenieś, aby zakończyć proces przenoszenia.

7. Wyświetlanie potwierdzenia akceptacji przeniesienia.

   W tym momencie przyszły partner, klient i bieżący partner zostaną powiadomieni o zaakceptowanym żądaniu przeniesienia za pośrednictwem poczty e-mail.

   Po zaakceptowaniu przeniesienia może on pozostać w stanie Oczekujące przez maksymalnie 15 minut podczas aktualizowania systemu. Jeśli trwa to dłużej, system będzie próbować przez trzy dni. Jeśli stan przeniesienia nadal będzie mieć stan Oczekujące, partner powinien przesłać żądanie obsługi.

   Po zakończeniu przenoszenia subskrypcje uwzględnione w żądaniu będą wyświetlane w planie platformy Azure przyszłego partnera i nie będą już wyświetlane w nim.

>[!Note]  
>W przypadku dostawców pośrednich: poinformuj odsprzedawcę pośredniego, że żądanie przeniesienia zostało zaakceptowane.

### <a name="managing-your-transferred-customer-subscriptions"></a>Zarządzanie przeniesionymi subskrypcjami klientów

- Przejście nie wpływa na dostęp do istniejących użytkowników, grup lub jednostek usługi, które zostały przypisane przy użyciu kontroli dostępu na podstawie ról (RBAC) na platformie Azure. Kontrola dostępu oparta na rolach [(RBAC)](/azure/role-based-access-control/overview) platformy Azure pomaga klientom zarządzać tym, kto ma dostęp do zasobów platformy Azure, co może zrobić z tymi zasobami i do jakich obszarów ma dostęp. Jako nowy partner nie masz dostępu RBAC do zasobów klienta po przeniesieniu subskrypcji. Poprzedni partner klienta zachowuje dostęp RBAC. We współpracy z klientem dowiedz się, kto ma wgląd w swoje subskrypcje i jak wprowadzać dowolne zmiany.

- W związku z tym ważne jest, aby klient usuał dostęp RBAC platformy Azure dla poprzedniego partnera i dodał dostęp dla nowego partnera. Aby uzyskać więcej informacji na temat nowego dostępu klienta, zobacz Co to jest kontrola dostępu na podstawie ról [(RBAC) platformy Azure?](/azure/role-based-access-control/overview) Aby uzyskać więcej informacji na temat usuwania dostępu RBAC poprzedniego partnera przez klienta, [zobacz Usuwanie przypisania roli](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Ponadto nie uzyskujesz automatycznie dostępu [administratora w imieniu (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) do subskrypcji. AOBO jest niezbędne, aby partner zarządzał subskrypcjami platformy Azure swoich klientów w ich imieniu. Aby uzyskać więcej informacji na temat uprawnień platformy Azure, zobacz Uzyskiwanie uprawnień do zarządzania [usługą lub subskrypcją klienta.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Następne kroki:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta.](./customers-revoke-admin-privileges.md)
