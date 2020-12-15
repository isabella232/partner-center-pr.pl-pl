---
title: Wyświetl szczegóły zachęty i programu
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Użyj tych stron do wyświetlania stanu programu bodźce i zarządzania nim
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4bf1c7a2abceffc812666456ddae252fca70d8f1
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492725"
---
# <a name="view-your-incentives-program-details"></a>Wyświetl szczegóły programu zachęty

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Administrator zachęt
- Użytkownik zachęty
- Zachęta do przeglądania tylko do odczytu
- Administrator globalny
- Administrator partnerski MPN

W tym artykule wyjaśniono, jak uzyskać dostęp do strony **Przegląd moje zachęty** , która pokazuje ogólny stan programów zachęty, a także stan każdego programu w każdej lokalizacji. Zapewnia również różne stany rejestracji. 

>[!NOTE]
>Aby uzyskać więcej informacji na temat zachęt i funkcji zachęty w centrum partnerskim, zobacz temat [inwestycje i zachęty dla partnerów](https://partner.microsoft.com/membership/partner-incentives) (wymagane jest zalogowanie się).

## <a name="access-the-incentives-overview-page"></a>Dostęp do strony przeglądu zachęt

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard).
1. Wybierz opcję **zachęty**, a następnie pozycję **Przegląd** z menu.
1. Przejrzyj podsumowanie zarobków i płatności w górnej części strony, a następnie więcej szczegółowych informacji w tabeli poniżej. Można również sortować, grupować i rozszerzać dołączoną tabelę:

   - Aby sortować według kolumny, wybierz nazwę kolumny.
   - Aby grupować według programu, wybierz kartę **według programu** powyżej tabeli.
   - Aby grupować według lokalizacji, wybierz kartę **według lokalizacji** nad tabelą.
   - Aby wyświetlić więcej szczegółów na temat rejestracji w ramach określonej grupy, wybierz symbol ostrokątny na końcu danego wiersza. Ten cudzysłów ostrokątny rozszerza widok.
1. Jeśli do zarejestrowania się w programie wymagane jest wykonanie dodatkowych czynności, odpowiednie informacje zostaną wyświetlone w kolumnie **Stan**. W takim przypadku wybierz symbol cudzysłowu ostrokątnego, aby dowiedzieć się więcej o następnych krokach, które należy wykonać.

## <a name="enrollment-status"></a>Stan rejestracji

W poniższej tabeli objaśniono różne stany rejestracji widoczne w kolumnie **stan** .

| **Stan**         | **Pojawia się, gdy** |
|:------------------------------------|:------------------|
| Wymagana akcja  | Partner zaakceptował zaproszenie do rejestracji w programie zachęty, ale może być konieczne zaktualizowanie informacji o banku lub podatku. Aby zaktualizować dane bankowe lub podatkowe w centrum partnerskim, zapoznaj się z kolumną **wymagane akcje** . |
| Wycofane  | Konkretny program zachęty nie jest już oferowany w systemie zachęt. |
| Zarejestrowano  | Wszystkie informacje podatkowe i bankowe zostały zweryfikowane. Partner nie wymaga żadnych dalszych czynności rejestracyjnych. |
| Rejestrowanie  | Użytkownik nie jest administratorem zachęty, a rejestracja odbywa się w **wymaganej akcji** lub **sprawdza stan rejestracji** .|
| Nieaktywne/niekwalifikujące się | W tej chwili program zachęty może nie być otwarty do rejestracji lub partner nie spełnia bieżącego uprawnienia do rejestracji ani ponownego rejestrowania. <br><br> Jeśli stan jest **nieuprawniony**, partner nie spełnia aktualnych wymagań dotyczących uprawnień dla programu; wybranie linku **Zobacz wymagania dotyczące uprawnień** poniżej stanu rejestracji będzie zawierać wymagania dotyczące uprawnień oraz tego, jakie wymagania zostały spełnione. <br><br> W programie zachęty może być również wyświetlany stan **nieaktywności** usługi Virtual ORGANIZATION (VORG) lub konta globalnego partnera (PGA), które nie są już aktywne.  |
| Zaproszeni  | Do partnera wysłano nowe zaproszenie do rejestracji programu zachęty, ale nie uruchomiono jeszcze procesu rejestracji przez partnera. Sąsiadujące kolumny **wymagane akcje** przedstawiają następne kroki i powiązane linki.  |
| Weryfikowanie rejestracji  | Partner już zakończył lub zaktualizował informacje dotyczące banku i podatku dla nowej lub istniejącej rejestracji i czeka na zweryfikowanie tych informacji przez firmę Microsoft. W trakcie procesu weryfikacji **Sprawdzanie poprawności rejestracji** może się pojawić przez maksymalnie 48 godzin.  |

## <a name="see-your-payment-information"></a>Wyświetlanie informacji o płatności

Wybierz ikonę wypłaty w prawym górnym rogu ekranu, aby uzyskać dostęp do tych różnych podsumowań:

- Historia transakcji
- Płatności
- Eksportowanie danych

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Przedstawia ikonę wypłaty w prawym górnym rogu portalu Centrum partnerskiego":::

Te informacje obejmują łączne płatności i zarobki związane z zachętami od momentu zarejestrowania w programach zachęt. Na tej stronie podano też zarobki i płatności według lokalizacji lub programu, a także wszelkie dalsze czynności, które należy wykonać, aby zarejestrować się w programie w określonej lokalizacji. 

Możesz również użyć [interfejsu API wypłaty partnera](https://apidocs.microsoft.com/services/partnerpayouts) , aby połączyć się i uzyskać bezpośrednią transakcję oraz dane dotyczące płatności. Zobacz [instrukcje wypłaty](payout-statement.md) , aby dowiedzieć się więcej.

## <a name="next-steps"></a>Następne kroki
- [Zestawienia wypłat](payout-statement.md)
