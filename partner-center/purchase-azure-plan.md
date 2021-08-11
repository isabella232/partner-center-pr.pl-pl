---
title: Kupowanie planu platformy Azure
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Korzystając z planu platformy Azure, dowiedz się, jak kupić pojedynczą lub wiele subskrypcji platformy Azure, rezerwacji platformy Azure, skonfigurować zasoby oraz wyświetlić lub dodać subskrypcje.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: af098c9ef57a9a40badded40cb457f8c8fd4855185ae6f10dfb71e51689994ea
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693912"
---
# <a name="purchase-the-azure-plan-for-customers-and-access-the-latest-azure-services"></a>Kupowanie planu platformy Azure dla klientów i uzyskiwanie dostępu do najnowszych usług platformy Azure

**Dotyczy:** Partner Center 

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent sprzedaży

Po zakupie planu platformy Azure dla klientów w ramach usługi Umowa z Klientem Microsoft masz dostęp do pełnego katalogu najnowszych usług platformy Azure po stawkach płatności zgodnie z użyciem. Dostawca rozwiązań w chmurze (CSP) będą teraz mogli uzyskać dostęp do dowolnej usługi platformy Azure, gdy stanie się ona ogólnie dostępna. Partner może mieć wiele subskrypcji platformy Azure w ramach planu platformy Azure. 

## <a name="countryregion-availability"></a>Dostępność kraju/regionu

Nowe środowisko handlowe w programie CSP dla platformy Azure jest obecnie dostępne w 137 krajach. Zobacz pełną listę tych [krajów/regionów.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x) 

## <a name="how-to-purchase-azure-plan"></a>Jak kupić plan platformy Azure

Sposób zakupu planu platformy Azure jest podobny do zakupu dowolnej innej subskrypcji. Kluczowa różnica polega na tym, że przed rzeczywiście zamówieniem należy potwierdzić, że klient podpisał umowę Umowa z Klientem Microsoft.

1. Wybierz **pozycję Segment komercyjne,** a następnie wpisz "Microsoft Azure".
2. W **obszarze Plan platformy Azure** wybierz pozycję Dodaj do **koszyka.**

   :::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Zakupu.":::

Partner musi potwierdzić, że klient przejmuje i zaakceptował Umowa z Klientem Microsoft warunki. Aby uzyskać więcej informacji na temat sposobu, w jaki partner może to zrobić, przeczytaj potwierdzanie akceptacji przez klienta [Umowa z Klientem Microsoft](./confirm-customer-agreement.md). Inne zasoby są dostępne w [galerii zasobów](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/).

Następnie potwierdź cyfrowo lub zaproś klienta do podpisania Umowa z Klientem Microsoft bezpośrednio z firmą Microsoft. 

### <a name="to-invite-the-customer-to-sign-the-agreement-directly"></a>Aby zaprosić klienta do bezpośredniego podpisania umowy 

1. Na stronie Konto **klienta wybierz** pozycję Aktualizuj obok **Umowa z Klientem Microsoft**. 

2. Podaj informacje o poszczególnych osobach w firmie klienta, która zaakceptowała projekt MCuA.

3. Wybierz przycisk **Zapisz i kontynuuj**.  

W ramach nowego rozwiązania handlowego dla Platforma Azure w programie CSP wprowadziliśmy [nową ofertę platformy Azure.](./azure-plan-lp.md) Ważne daty związane z poprzednią ofertą platformy Azure (MS-AZR-0145p) można znaleźć w [dokumencie oferty](https://go.microsoft.com/fwlink/p/?linkid=2164140).

**W przypadku zarejestrowania *się przed* 21 lipca 2021 r.**
- Będzie można dodać poprzednią ofertę platformy Azure do koszyka dla klientów, którzy kupili ją w przeszłości.
- Jeśli jesteś zarejestrowanym przed *21* lipca i masz klientów zarejestrowanych po 21 lipca, nie będziesz mieć możliwości dodania poprzedniej oferty platformy Azure do koszyka.

**Partnerzy zarejestrowani w *dniu* 21 lipca 2021 r. lub później**
- Nie będzie można dodać poprzedniej oferty platformy Azure do koszyka.

Jeśli spróbujesz dodać poprzednią ofertę platformy Azure, ale nie kwalifikujesz się z powodu powyższych zasad biznesowych, zostanie napotkany następujący błąd. 

:::image type="content" source="images/add-products.png" alt-text="Zrzut ekranu przedstawiający ekran Dodawanie produktów.":::

Aby znaleźć nowy plan platformy Azure z Partner Center API, zobacz [Tworzenie planu platformy Azure.](/partner-center/develop/create-azure-plan#get-the-catalog-item-for-azure-plan)

## <a name="review-and-buy"></a>Przeglądanie i kupowanie

Wróć do **strony Dodawanie produktu,** na której widać, że plan platformy Azure został dodany. Wybierz **pozycję Przejrzyj,** aby przejrzeć zakup, a następnie wybierz **pozycję Kup**. 

> [!NOTE]
> Po zakupie planu platformy Azure dla klienta nie będzie można już kupić planu Microsoft Azure (0145p) dla tego klienta. Konieczne będzie utworzenie przyszłych subskrypcji za pośrednictwem planu platformy Azure.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Kupowanie rezerwacji platformy Azure w ramach planu platformy Azure 
  
Możesz również kupić rezerwacje Microsoft Azure planie platformy Azure w imieniu klientów w Partner Center. (Lub, jeśli wolisz, możesz udzielić swoim klientom uprawnień do zakupu własnych rezerwacji platformy [Azure](give-customers-permission.md) z wcześniejszej subskrypcji, która została dla nich zakupiona).

1. Z menu Partner Center pulpitu [nawigacyjnego](https://partner.microsoft.com/dashboard/)wybierz pozycję **Klienci.** Znajdź klienta, który chce kupić rezerwacje platformy Azure, a następnie wybierz strzałkę w dół, aby rozwinąć wiersz klienta.

2. Wybierz **pozycję Dodaj produkty,** a następnie wybierz pozycję **Azure.** 

   - Wybierz segment rynku klienta z **listy Segment.**
   - Wybierz **pozycję Rezerwacje** z **listy Typ** produktu.
   - Wybierz typ rezerwacji, który klient chce wybrać z **listy Typ rezerwacji.**

Rezerwacje platformy Azure muszą być skojarzone z aktywnym planem platformy Azure. Z listy Subskrypcja klienta wybierz plan platformy Azure, do którego chcesz dodać rezerwacje platformy Azure. 

> [!IMPORTANT] 
> Jeśli klient nie ma jeszcze aktywnego planu platformy Azure, wybierz pozycję Azure, aby dodać go teraz. Aby uzyskać dalsze [instrukcje, zobacz Kupowanie rezerwacji platformy Azure.](azure-reservations-buying.md#purchase-azure-reservations)

> [!NOTE]
> Zakres rezerwacji można ustawić tylko na wartość **Udostępnione**, obecnie w Partner Center. Aby wybrać zakres pojedynczej subskrypcji lub zaktualizować zakres z udostępnionego na zakres pojedynczej subskrypcji, przejdź **do Microsoft Azure Management Portal,** korzystając z poniższych instrukcji. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Ustawienie rezerwacji zakresu współużytkowego.":::

Aby zarządzać rezerwacją klienta w Azure Portal: 

1. Z **opcji** Klienci wybierz klienta, którym chcesz zarządzać. 

2. Za pomocą strzałki w dół rozwiń wiersz klienta i wybierz pozycję **Microsoft Azure Management Portal.**  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Wyświetlanie subskrypcji platformy Azure w ramach planu platformy Azure

Na **stronie Subskrypcje** w sekcji opartej na użyciu rozwiń plan platformy **Azure,** aby wyświetlić skojarzone subskrypcje platformy Azure w ramach planu platformy Azure.

:::image type="content" source="images/azure/addprods2.png" alt-text="Wyświetl listę subskrypcji platformy Azure."::: 

## <a name="add-subscriptions-and-configure-resources"></a>Dodawanie subskrypcji i konfigurowanie zasobów

Dodasz subskrypcje i skonfigurujesz zasoby dla klienta w Azure Portal. Możesz również oddzielić środowisko klienta według obciążenia lub projektu. Subskrypcjami można zarządzać za [pośrednictwem Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) i Azure Portal. 

Aby zarządzać zasobami i subskrypcjami klienta, musisz mieć uprawnienia **Administratora w imieniu** (AOBO). Aby uzyskać informacje na temat zarządzania dostępem, przeczytaj [zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure.](azure-plan-manage.md)

## <a name="next-steps"></a>Następne kroki

- [Przejścia klientów do planu platformy Azure](azure-plan-transition.md)

- [Środków uzyskane przez partnerów — omówienie](partner-earned-credit.md)
