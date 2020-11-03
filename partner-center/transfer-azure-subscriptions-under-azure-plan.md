---
title: Przenoszenie subskrypcji platformy Azure w ramach planu platformy Azure do innego partnera CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak zmienić partnera programu Cloud Solution Provider skojarzonego z subskrypcjami platformy Azure klienta w ramach planu platformy Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530232"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Przenoszenie subskrypcji planu platformy Azure klienta na innego partnera

## <a name="applies-to"></a>Dotyczy

- Partnerzy w programie dostawcy rozwiązań w chmurze (CSP)

W tym artykule opisano, jak klient może przełączyć swoje subskrypcje platformy Azure w ramach planu platformy Azure z jednego dostawcy rozwiązań w chmurze (CSP) na inny.

Aby przełączyć subskrypcje platformy Azure klienta z innego partnera, wykonaj następujące kroki. Zarówno partner, jak i klient mają kroki do wykonania.

>[!Note]  
>Tylko partnerzy z bezpośrednią relacją rozliczeniową z firmą Microsoft mogą uzyskać dostęp do narzędzi przejścia. Pośrednicy odsprzedawcy muszą współpracować z dostawcami pośrednimi, aby korzystać z tego narzędzia przejścia.

Klient musi znajdować się w konwersacji z partnerami (bieżący i przyszły) przed użyciem tego narzędzia. Konwersacja w trybie offline musi mieć na celu uniknięcie pomyłek i zmian. Ponadto partnerzy i klienci powinni zrozumieć te zagadnienia i wymagania wstępne przed zainicjowaniem przejścia:

**Kluczowe zagadnienia:**

- Azure Reservations nie zostanie przeniesiona z subskrypcją do przyszłego partnera
- Cennik CSP dla usług platformy Azure w ramach bieżącego partnera nie zostanie przenoszony  
- Odpowiedzialność za pomoc techniczną dla klienta przejdzie do przyszłego partnera
- Rozliczanie i fakturowanie będzie przenoszone do przyszłego partnera w czasie transferu
- Transfer nie ma wpływ na usługę Azure Role-Based Access Control (RBAC)
- Administrator w imieniu (AOBO) nie zostanie domyślnie udzielony dla przyszłego partnera
- Produkty z witryny Marketplace innych firm zostaną przetransferowane, o ile produkty przechodzą przez sprawdzanie uprawnień witryny Marketplace.
    - Nie ma specjalnych rabatów ani ograniczeń regionalnych
    - Produkty nie są oparte na subskrypcji
    - W przyszłości Partner powinien współpracować z wydawcą, aby upewnić się, że znajdują się na liście dozwolonych dla wdrożenia produktu
    - Jeśli nie wszystkie te warunki zostaną spełnione, aby można było przenieść produkty z portalu Marketplace, przetransferowane subskrypcje platformy Azure, a następnie zakupione produkty Marketplace z nowym partnerem

**Wymagania wstępne:**

- Klient angażuje bieżącego partnera CSP w celu przejścia
- W przyszłości partner CSP współpracuje z klientem w celu zapewnienia, że potrzeby klientów mogą być spełnione
- W przyszłości partner CSP nawiązuje relację z klientem przed rozpoczęciem przejścia  
- Klient musi podpisać umowę klienta firmy Microsoft, korzystając z przyszłego partnera CSP
- W przyszłości partner CSP musi mieć podpisaną umowę partner firmy Microsoft, aby móc korzystać z tego narzędzia

## <a name="customer-tasks-to-be-completed"></a>Zadania klienta do ukończenia

Aby przenieść subskrypcję platformy Azure w ramach planu platformy Azure, klient musi rozpocząć proces, kontaktując się z bieżącym partnerem. Powinny one zbierać nazwę firmy i domenę bieżącego partnera, aby w przyszłości wszyscy partnerzy mogli zakończyć formularz żądania przeniesienia w ich imieniu.

Klient musi także zidentyfikować subskrypcje, które chcą przenieść z bieżącego partnera. Nie można zmienić partnerów dla pakietów Office 365, Enterprise Mobility Suite ani Microsoft Dynamics CRM.

>[!Note]  
>W przyszłości jest odpowiedzialny za wykonanie formularza żądania przeniesienia, który inicjuje proces transferu. Firma Microsoft nie może interweniować w imieniu klienta lub bieżącego partnera. Klient powinien zaplanować ścisłą pracę z przyszłymi i bieżącymi partnerami, aby zapewnić płynność przejścia.

## <a name="future-partner-tasks-to-be-completed"></a>Przyszłe zadania partnerskie do ukończenia

Przyszły partner subskrypcji musi ukończyć formularz żądania przeniesienia z Centrum partnerskiego, aby zażądać przeniesienia subskrypcji:

1.  W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta, który ma zostać ukończony w formularzu żądania przeniesienia w imieniu.
2.  W menu Klient wybierz pozycję **subskrypcje** .
3.  Wybierz sekcję **żądanie przeniesienia** .
4.  W **sekcji żądanie transferu** wybierz pozycję **Dodaj nowe żądanie** .

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sekcja Transfers":::

5.  Wykonaj **nową formę żądania przeniesienia** .

6.  Wybierz pozycję **Wyślij żądanie wysłania żądania**  >  **Send** .

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Sekcja Transfers":::

7.  Sprawdź potwierdzenie żądania przeniesienia

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Sekcja Transfers" lub "ukończone", anulowanie nie będzie możliwe.

## <a name="current-partner-tasks-to-be-completed"></a>Bieżące zadania partnerskie do ukończenia

Agent administracyjny bieżącego partnera klienta otrzyma wiadomość e-mail z prośbą o przesłanie subskrypcji przez klienta:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Sekcja Transfers":::

Przejrzyj i zaakceptuj formularz żądania przeniesienia z Centrum partnerskiego, aby ukończyć transfer subskrypcji.

>[!Note]  
>Jeśli bieżący partner nie podejmie żadnych działań w ciągu 30 dni, żądanie wygaśnie, a w przyszłości Partner będzie musiał utworzyć nowe żądanie transferu.

1.  Wybierz pozycję **Przejrzyj żądanie przeniesienia** z wiadomości e-mail lub
1.  W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta, w imieniu którego zostało przesłane żądanie transferu.
2.  W menu Klient wybierz pozycję **subskrypcje** .
3.  Wybierz sekcję **żądanie przeniesienia** .
4.  Rozwiń węzeł informacje o transferze, wybierając wybrany **Identyfikator żądania transferu** w obszarze **odebrane żądania** .

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Sekcja Transfers":::

5.  Przejrzyj żądanie transferu. Wybierz żądane subskrypcje platformy Azure do przeniesienia.

>[!Note]  
> Przed kontynuowaniem Zwróć uwagę: nie będziesz już mieć dostępu do wybranych subskrypcji.
> Nie będzie ono zafakturowane do dalszych zastosowań.
> Rezerwacje platformy Azure nie są transferowane w ramach subskrypcji.

6.  Następnie wybierz pozycję **Zaakceptuj i Przenieś** , aby zakończyć proces transferu.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Sekcja Transfers":::

7.  Wyświetl potwierdzenie akceptacji transferu.

   W tym momencie przyszły partner, klient i bieżący partner będą powiadamiani o zaakceptowanym żądaniu transferu za pośrednictwem poczty e-mail.

   Po przeprowadzeniu przejścia stan transferu może potrwać do 15 minut, podczas gdy system zostanie zaktualizowany. Jeśli trwa dłużej, system będzie ponawiać próbę przez trzy dni. Jeśli stan transferu nadal pozostaje w stanie oczekiwania, Partner powinien przesłać żądanie obsługi.

   Po zakończeniu transferu subskrypcje zawarte w żądaniu będą widoczne w planie platformy Azure w przyszłości partnera i nie będą już wyświetlane.

>[!Note]  
>W przypadku dostawców pośrednich: Powiadom pośredni odsprzedawcę o zaakceptowaniu żądania transferu.

### <a name="managing-your-transferred-customer-subscriptions"></a>Zarządzanie przetransferowanymi subskrypcjami klientów
- Przejście nie wpływa na dostęp do istniejących użytkowników, grup lub jednostek usługi, które zostały przypisane przy użyciu kontroli dostępu na podstawie ról (RBAC) na platformie Azure. Funkcja kontroli dostępu opartej na rolach [(Azure RBAC)](/azure/role-based-access-control/overview) systemu Azure pomaga klientowi zarządzać dostępem do zasobów platformy Azure, co można zrobić z tymi zasobami i jakie obszary mają do nich dostęp. Nowy partner nie otrzymuje dostępu RBAC do zasobów klienta po jego przeniesieniu. Poprzedni partner klienta zachowuje dostęp do kontroli dostępu RBAC. Skontaktuj się z klientem, aby zrozumieć, kto ma wgląd w swoje subskrypcje i jak wprowadzać niepożądane zmiany.

- W związku z tym ważne jest, aby klient usuwał dostęp do usługi Azure RBAC dla swojego poprzedniego partnera i mógł dodać dostęp dla nowego partnera. Aby uzyskać więcej informacji na temat klienta dostarczającego nowy dostęp, zobacz [co to jest kontrola dostępu oparta na rolach (Azure RBAC)?](/azure/role-based-access-control/overview) Aby uzyskać więcej informacji na temat usuwania przez klienta dostępu RBAC z poprzedniego partnera, zobacz [usuwanie przypisania roli](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Ponadto nie otrzymujesz automatycznie dostępu [administratora w imieniu (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) do subskrypcji. AOBO jest konieczne, aby partner mógł zarządzać subskrypcjami platformy Azure klienta w ich imieniu. Aby uzyskać więcej informacji na temat uprawnień platformy Azure, zobacz [Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Następne kroki:

- [(RBAC na platformie Azure)](/azure/role-based-access-control/overview)
- [Uzyskaj uprawnienia do zarządzania usługą lub subskrypcją klienta.](./customers-revoke-admin-privileges.md)