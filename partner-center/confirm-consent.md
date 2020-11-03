---
title: Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft
description: Dowiedz się, jak potwierdzić akceptację umowy klienta firmy Microsoft przez klienta. Może to być konieczne, aby zamówić produkty i usługi firmy Microsoft dla klientów.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530657"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Zaktualizowano metodę w celu potwierdzenia akceptacji przez klienta umowy klienta firmy Microsoft

**Dotyczy**

-  Centrum partnerskie

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży

> [!NOTE]
> Zasób z umową jest obecnie obsługiwany przez centrum partnerskie tylko w chmurze publicznej firmy Microsoft. Nie dotyczy:
> * Centrum partnerskie obsługiwane przez firmę 21Vianet
> * Centrum partnerskie dla Microsoft Cloud (Niemcy)
> * Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA

>[!NOTE]
>Od 31 stycznia 2020, wszyscy klienci, istniejące i nowe, muszą podpisać nową umowę klienta firmy Microsoft. Aby dowiedzieć się więcej, przeczytaj artykuł [potwierdzenie akceptacji klienta umowy dla klientów firmy Microsoft](confirm-customer-agreement.md).

Jako partner musisz uzyskać zgodę klienta firmy Microsoft, aby móc zamówić produkty i usługi firmy Microsoft dla tego klienta. Aby lepiej pomóc partnerom spełnić wymagania dotyczące zgodności, firma Microsoft prosi partnerów o potwierdzenie akceptacji, dostarczając następujące informacje dotyczące osoby, która zaakceptowali umowę:

- Imię

- Nazwisko

- Adres e-mail

- Numer telefonu (opcjonalnie)

- Data akceptacji

Bezpośredni partnerzy rozliczeń i dostawcy pośredniego muszą potwierdzić akceptację umowy klienta firmy Microsoft przez klienta podczas przeprowadzania transakcji za pośrednictwem usługi Partner Center lub interfejsu API Centrum partnerskiego. Potwierdzenie jest *obowiązkowe* .

Jeśli nie podano potwierdzenia dla danego klienta:

- Nie będzie można tworzyć nowych zamówień dla tego klienta.

- Nie będzie można zmienić liczby licencji istniejących subskrypcji opartych na licencji dla tego klienta.

Potwierdzenie akceptacji klienta można przeprowadzić za pośrednictwem Centrum partnerskiego lub interfejsu API Centrum partnerskiego. Aby to zrobić za pomocą interfejsu API Centrum partnerskiego, zobacz następujące tematy:

- [Uzyskaj potwierdzenie zgody klienta](/partner-center/develop/get-confirmation-of-customer-consent)

- [Pobierz metadane umowy](/partner-center/develop/get-agreement-metadata)

- [Potwierdź zgodę klienta](/partner-center/develop/confirm-customer-consent)

Dotyczy to zarówno środowiska produkcyjnego, jak i piaskownicy.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Potwierdź akceptację klienta dla nowego klienta

Poniższa procedura umożliwia potwierdzenie akceptacji klienta podczas tworzenia nowej dzierżawy klienta w centrum partnerskim. Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.

1. Wybierz pozycję **klienci** , a następnie **Nowy klient** , a następnie wybierz pozycję **Informacje o koncie** .

2. Wprowadź informacje o **firmie** i **kontakcie podstawowym** .

   :::image type="content" source="images/mca/mca1.png" alt-text="Informacje o firmie":::

3. W obszarze **Umowa klienta firmy Microsoft** wybierz pozycję **klient zaakceptował najnowszą umowę klienta firmy Microsoft** .

4. W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej wartości na datę przyszłą.

5. Wprowadź szczegółowe informacje o użytkowniku, który podał zatwierdzenie.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Informacje o firmie":::

   Domyślnie są wyświetlane podstawowe informacje o użytkowniku kontaktu. Jeśli to nie jest poprawne, wybierz pozycję **Aktualizuj** , a **First name** następnie wprowadź imię **, nazwisko** , **adres e-mail** i * *numer telefonu* (opcjonalnie) osoby, która zaakceptował umowę.

6. Wybierz pozycję **dalej** , aby kontynuować wykonywanie pozostałych kroków w celu utworzenia dzierżawy klienta.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Potwierdzenie akceptacji przez klienta dla istniejącego klienta

Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.

1. Wybierz pozycję **klienci** , a następnie Znajdź i wybierz klienta, który ma zostać wyświetlony.

2. Wybierz pozycję **Informacje o koncie** .

3. W obszarze **Umowa klienta firmy Microsoft** wybierz pozycję **Aktualizuj** .

   :::image type="content" source="images/mca/mca4.png" alt-text="Informacje o firmie":::

4. Wprowadź **imię** **, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) użytkownika, który zaakceptował umowę.

5. W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej wartości na datę przyszłą.

6. Wybierz przycisk **Zapisz i kontynuuj** .

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Potwierdź akceptację klienta podczas tworzenia nowego zamówienia dla istniejącego klienta

Jeśli spróbujesz utworzyć nowe zamówienie dla istniejącego klienta, który nie został wcześniej potwierdzony, zostanie wyświetlony monit o ukończenie potwierdzenia. Użyj poniższej procedury w tym celu.

1. Wprowadź **imię** **, nazwisko,** **adres e-mail** i **numer telefonu** (opcjonalnie) użytkownika, który zaakceptował umowę.

2. W obszarze **Data akceptacji umowy** wprowadź odpowiednią datę. Nie można ustawić tej wartości na datę przyszłą.

3. Wybierz przycisk **Zapisz i kontynuuj** .

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Pobierz potwierdzenie akceptacji klienta dla istniejącego klienta

Potwierdzenie akceptacji klienta dla istniejącego klienta zostało podane wcześniej przy użyciu poniższej procedury. Aby to zrobić, musisz być agentem administracyjnym lub agentem sprzedaży.

1. Wybierz pozycję **klienci** , a następnie Znajdź i wybierz klienta, który ma zostać wyświetlony.

2. Wybierz pozycję **Informacje o koncie** .

3. W ramach **umowy klienta firmy Microsoft** zobaczysz, czy dla tego klienta podano potwierdzenie.

## <a name="next-steps"></a>Następne kroki

- [Potwierdzenie akceptacji przez klienta umowy klienta firmy Microsoft w programie partnerskim programu CSP](confirm-customer-agreement.md)

- [Zaświadczenie akceptacji umowy klienta firmy Microsoft w imieniu klienta](attest-acceptance-customer-agreement.md)