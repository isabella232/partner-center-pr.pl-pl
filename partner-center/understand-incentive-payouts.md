---
title: Wyświetlanie informacji o zachętach i programach
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Użyj tych stron do wyświetlania stanu Program zachęt zarządzania nimi
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 33ec3befdc4b2bab2f31d25d210679594debbbf1
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277253"
---
# <a name="view-your-incentives-program-details"></a>Wyświetlanie szczegółów programu zachęt

**Odpowiednie role:** Zachęty dla administratorów | Zachęty dla użytkowników | Administrator globalny | Administrator partnera MPN

W tym artykule  wyjaśniono stronę Przeglądu moich zachęt, na której przedstawiono ogólny stan programów zachęt, a także stan poszczególnych programów w każdej lokalizacji. Zapewnia również różne stany rejestracji.

>[!NOTE]
>Aby uzyskać więcej informacji na temat zachęt i funkcji zachęt w Partner Center, zobacz [Partner Investments and Incentives](https://partner.microsoft.com/membership/partner-incentives) (Wymagane logowanie).

## <a name="access-the-incentives-overview-page"></a>Uzyskiwanie dostępu do strony przeglądu zachęt

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard) Centrum partnerskiego.
1. Wybierz **pozycję Zachęty,** a następnie **pozycję** Przegląd z menu.
1. Przejrzyj podsumowanie zarobków i płatności w górnej części strony, a następnie więcej szczegółowych informacji w tabeli poniżej. Możesz również sortować, grupować i rozwijać towarzyszącej tabeli:

   - Aby posortować według kolumny, wybierz nazwę kolumny.
   - Aby grupować według programu, wybierz **kartę Według programu** nad tabelą.
   - Aby grupować według lokalizacji, wybierz **kartę Według lokalizacji** nad tabelą.
   - Aby wyświetlić więcej szczegółów na temat rejestracji w określonej grupie, wybierz symbol szewronu na końcu danego wiersza. Ten szewron rozszerza widok.
1. Jeśli do zarejestrowania się w programie wymagane jest wykonanie dodatkowych czynności, odpowiednie informacje zostaną wyświetlone w kolumnie **Stan**. W takim przypadku wybierz symbol cudzysłowu ostrokątnego, aby dowiedzieć się więcej o następnych krokach, które należy wykonać.

## <a name="enrollment-status"></a>Stan rejestracji

W poniższej tabeli wyjaśniono różne stany rejestracji wyświetlane w **kolumnie** Stan.

| **Stan**         | **Pojawia się, gdy** |
|:------------------------------------|:------------------|
| Wymagana akcja  | Partner zaakceptował zaproszenie do zarejestrowania się w programie zachęt, ale może być konieczne zaktualizowanie informacji bankowych lub podatkowych. Zobacz **kolumnę Wymagane akcje,** aby uzyskać informacje o kolejnych krokach lub linki do aktualizowania informacji bankowych lub podatkowych w Partner Center. |
| Przerwać  | Określony program zachęt nie jest już oferowany w systemie zachęt. |
| Zarejestrowano  | Wszystkie informacje podatkowe i bankowe zostały zweryfikowane. Partner nie wymaga żadnej dalszej akcji rejestracji. |
| Rejestrowanie  | Użytkownik nie jest administratorem zachęt, a rejestracja znajduje się w wymaganym działaniu **lub** sprawdzania **poprawności stanów** rejestracji.|
| Nieaktywny/nieaktywny | Program zachęt może nie być obecnie otwarty na rejestrację lub partner nie spełnia warunków bieżących uprawnień do rejestracji lub ponownej rejestracji. <br><br> Jeśli stan to **Niekwalifikuje się**, partner nie spełnia bieżących wymagań dotyczących uprawnień do programu; Wybranie **linku Zobacz wymagania dotyczące uprawnień** poniżej stanu rejestracji spowoduje pokazanie wymagań dotyczących uprawnień i tego, które z tych wymagań zostały spełnione. <br><br> Może być również  wyświetlony stan Nieaktywny dla rejestracji organizacji wirtualnej (VORG) lub globalnego konta partnera (PGA), które nie są już aktywne w programie zachęt.  |
| Zaproszony  | Zaproszenie do rejestracji nowego programu zachęt zostało wysłane do partnera, ale partner nie rozpoczął jeszcze procesu rejestracji. Sąsiadująca kolumna **Wymagane akcje** zawiera następne kroki i wszelkie powiązane linki.  |
| Sprawdzania poprawności rejestracji  | Partner zakończył już lub zaktualizował informacje bankowe i podatkowe dotyczące nowej lub istniejącej rejestracji i czeka, aż firma Microsoft zweryfikuje te informacje. Podczas procesu walidacji **walidacja rejestracji** może być wyświetlana przez maksymalnie 48 godzin.  |

## <a name="see-your-payment-information"></a>Wyświetlanie informacji o płatności

Wybierz ikonę wypłaty w prawym górnym rogu ekranu, aby uzyskać dostęp do tych różnych podsumowań:

- Historia transakcji
- Płatności
- Eksportowanie danych

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ilustruje ikonę Wypłaty w prawym górnym rogu Partner Center portalu.":::

Te informacje obejmują łączne płatności i zarobki związane z zachętami od momentu zarejestrowania w programach zachęt. Na tej stronie podano też zarobki i płatności według lokalizacji lub programu, a także wszelkie dalsze czynności, które należy wykonać, aby zarejestrować się w programie w określonej lokalizacji. 

Możesz również użyć interfejsu API wypłat [partnera,](https://apidocs.microsoft.com/services/partnerpayouts) aby bezpośrednio nawiązać połączenie i uzyskać dane dotyczące transakcji wypłat i płatności. Aby [dowiedzieć się więcej,](payout-statement.md) zobacz Wypłaty.

## <a name="next-steps"></a>Następne kroki

- [Zestawienia wypłat](payout-statement.md)
