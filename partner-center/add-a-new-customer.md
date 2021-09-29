---
title: Jak dodać nowy rekord klienta
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak dodać nowy rekord klienta w Partner Center. Następnie możesz sprzedawać subskrypcje klientów, zarządzać rozliczeniami lub zapewniać pomoc techniczną dla klientów.
author: parthp
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 0d3b7787cf0f41a04f0a662450040802d74e9ef7
ms.sourcegitcommit: 1e616b52d55eff41d67a081ba3f4a8370a49e027
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/29/2021
ms.locfileid: "129191445"
---
# <a name="how-to-add-a-new-customer-record-in-partner-center"></a>Jak dodać nowy rekord klienta w Partner Center

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny | Agent sprzedaży

W tym artykule opisano sposób dodawania nowego klienta w Partner Center. Te kroki są wymagane, aby można było sprzedawać subskrypcje, zarządzać rozliczeniami lub udzielać pomocy technicznej klientowi.

## <a name="considerations"></a>Zagadnienia do rozważenia

Podczas dodawania nowego rekordu klienta w Partner Center:

- **Użyj poprawnego identyfikatora rejestracji:** podczas wprowadzania identyfikatora rejestracji firmy należy użyć identyfikatora podatkowego firmy, a nie osobistego identyfikatora klienta.

- **Wprowadź dodatkowe informacje dla niektórych krajów:** identyfikator rejestracji firmy i numer [telefonu](#company-registration-id-and-phone-number-required-for-some-countries) są wymagane w niektórych krajach, jeśli jesteś partnerem rozliczania bezpośredniego lub dostawcą pośrednim

- **Potwierdź** Umowa z Klientem Microsoft: Przed zamówieniem w imieniu klienta musisz potwierdzić, że klient zaakceptował Umowa z Klientem Microsoft [.](confirm-customer-agreement.md)

- **** Użyj różnych kroków dla istniejących klientów: W przypadku istniejących klientów, w tym [](multichannel.md) tych, [](multipartner.md) którzy już mają rekordy klientów w uciecie Partner Center w scenariuszu obejmującym wiele kanałów lub wiele partnerów, [](request-a-relationship-with-a-customer.md)zażądaj relacji z nimi , zamiast wykonać kroki opisane tutaj.

- **Wprowadź szczegółowe, dokładne informacje o kliencie:** aby weryfikacja klienta, upewnij się, że:
  - Wprowadź dokładną nazwę prawna/oficjalną, która będzie wyświetlana w oficjalnych dokumentach.
  - Unikaj używania skrótów lub krótkich formularzy.
  - Nie używaj nazw testów.
  - Podaj pełne, dokładne informacje o adresie (na przykład szczegóły lokalizacji, miasto, stan, kraj i kod pocztowy).

## <a name="new-rules-for-company-name-and-email-address"></a>Nowe reguły dotyczące nazwy firmy i adresu e-mail

Od 22 września 2021 r. będą stosowane następujące nowe reguły weryfikacji.

Podczas wprowadzania nazwy firmy następujące elementy nie będą dozwolone:
- Przy użyciu tylko jednego znaku.
- Używanie tylko znaków specjalnych, takich jak &$^# (zobacz [tabelę](#table-of-special-characters) poniżej).
- Używanie tylko spacji i/lub tabulatorów.
- Używanie skrótów autonomicznych z listy z ograniczeniami, takich jak LLC, Inc itp. (zobacz [tabelę](#table-of-abbreviations) poniżej).
- Używanie nazw z rozszerzeniami domeny internetowej Top-Level (TDL), takich jak ".com", ".org", ".edu", ".club" itp. (zobacz tabelę poniżej). [](#table-of-top-level-domain-extensions)

- Użycie tego samego znaku powtórzone trzy lub więcej razy bez innych znaków, takich jak 999.

- Używanie spacji i/lub tabulatorów mieszanych z poszczególnymi znakami, takimi jak 1 2 3.

Podczas wprowadzania adresu e-mail klienta następujące warunki nie będą dozwolone:

- Adres e-mail nie może zawierać adresu @microsoft.com .
- Adres e-mail klienta nie może zawierać tej samej nazwy domeny co partner. Na przykład partner o nazwie ABC nie może utworzyć wiadomości e-mail klienta za @abc.com pomocą .

## <a name="to-add-a-new-customer-in-partner-center"></a>Aby dodać nowego klienta w Centrum partnerskim

> [!NOTE]
> Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych, zobacz [Getting around Partner Center (Poruszanie się po Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off)).

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Zaloguj się do pulpitu [Partner Center,](https://partner.microsoft.com/dashboard)wybierz **kafelek Klienci,** a następnie wybierz **pozycję Dodaj klienta.**

2. Jeśli Klient jest instytucją edukacyjną, zobacz, [jak utworzyć klienta z opinią](sell-to-education-customers.md).

3. Na **stronie Informacje o koncie** wprowadź szczegóły klienta i podstawowe informacje kontaktowe.
   >[!IMPORTANT]
   >Partnerzy muszą potwierdzać, że:
   >
   >Potwierdzam, że moja organizacja działa jako partner pośredni podczas wybierania odsprzedawcy i partner bezpośredni w przypadku braku odsprzedawcy
   >
   >Potwierdzam, że nie odsprzedaję produktów zakupionych w ramach tego zamówienia innym partnerom powiązanym z moją organizacją nadrzędną

   >[!NOTE]
   >Przepisy prawne UNII/UNII EUROPEJSKIEJ stwierdzają, że partnerzy transakcyjni w tych krajach muszą zadeklarować dodatkowych odsprzedawców skojarzonych w ramach transakcji. Będą stosowane następujące reguły:
   >- Odsprzedawca początkowy musi zostać wybrany przed dodatkowymi odsprzedawcami
   >- Dodatkowi odsprzedawcy nie będą uprawnieni do żadnych dodatkowych zachęt, ofert itp.
   >- Dodatkowy wprowadzony sprzedawca zostanie zweryfikowany, aby upewnić się, że wprowadzono prawidłowy identyfikator MPN tam, gdzie ma to zastosowanie, a odsprzedawca podpisał umowę MPA.
   >- W ramach transakcji można wprowadzić maksymalnie 5 dodatkowych odsprzedawców

4. Jeśli jesteś dostawcą pośrednim, wybierz z listy odsprzedawcę pośredniego, który chcesz skojarzyć z subskrypcjami tego klienta.

5. Wybierz pozycję **Przejrzyj.**

6. Wybierz pozycję **Prześlij**.

7. Aby dodać subskrypcje, wybierz **pozycję Dodaj produkty.**

8. Po zakończeniu dodawania informacji o kliencie i zakupienia wymaganych subskrypcji wybierz pozycję **Gotowe.**

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Zaloguj się do pulpitu [Partner Center,](https://partner.microsoft.com/dashboard)wybierz pozycję **Klienci,** a następnie wybierz **pozycję Dodaj klienta.**

2. Jeśli Klient jest instytucją edukacyjną, zobacz, [jak utworzyć klienta z opinią](sell-to-education-customers.md).

3. Na **stronie Informacje o koncie** wprowadź szczegóły klienta i podstawowe informacje kontaktowe.
   >[!IMPORTANT]
   >Partnerzy muszą potwierdzać, że:
   >
   >Potwierdzam, że moja organizacja działa jako partner pośredni podczas wybierania odsprzedawcy i partner bezpośredni w przypadku braku odsprzedawcy
   >
   >Potwierdzam, że nie odsprzedaję produktów zakupionych w ramach tego zamówienia innym partnerom powiązanym z moją organizacją nadrzędną

   >[!NOTE]
   >Przepisy prawne UNII/UNII EUROPEJSKIEJ stwierdzają, że partnerzy transakcyjni w tych krajach muszą zadeklarować dodatkowych odsprzedawców skojarzonych w ramach transakcji. Będą stosowane następujące reguły:
   >- Odsprzedawca początkowy musi zostać wybrany przed dodatkowymi odsprzedawcami
   >- Dodatkowi odsprzedawcy nie będą uprawnieni do żadnych dodatkowych zachęt, ofert itp.
   >- Dodatkowy wprowadzony sprzedawca zostanie zweryfikowany, aby upewnić się, że wprowadzono prawidłowy identyfikator MPN tam, gdzie ma to zastosowanie, a odsprzedawca podpisał umowę MPA.
   >- W ramach transakcji można wprowadzić maksymalnie 5 dodatkowych odsprzedawców 

4. Jeśli jesteś dostawcą pośrednim, wybierz z listy odsprzedawcę pośredniego, który chcesz skojarzyć z subskrypcjami tego klienta.

5. Po zakończeniu wprowadzania wymaganych informacji wybierz pozycję **Dalej: Subskrypcje.**

6. Na **stronie Subskrypcje** wybierz oferty, które klient chce kupić od Ciebie, wprowadź liczbę licencji, a następnie wybierz pozycję **Dalej: Przejrzyj**.

7. Na stronie **Review (Przegląd)** sprawdź poprawność wpisów, a następnie wybierz pozycję **Submit (Prześlij).**

8. Po zakończeniu dodawania informacji o kliencie i zakupienia wymaganych subskrypcji wybierz pozycję **Gotowe.**

* * *

## <a name="company-registration-id-and-phone-number-required-for-some-countries"></a>Identyfikator rejestracji firmy i numer telefonu wymagany w niektórych krajach

Partnerzy z rozliczeniami bezpośrednimi i dostawcy pośredni dodający rekordy dla klientów w następujących krajach muszą również wprowadzić numer telefonu i identyfikator rejestracji firmy (nazywany również identyfikatorem REJESTRACJI organizacji):

W tym celu można chcieć odeznać się na przykład w takich regionach jak Brazylia Południowa, Brazylia, Brazylia Południowa, Brazylia Południowa, Tadżykistan, Dojdystan, Dominja, Zjednoczone Królestwo, Zjednoczone Królestwo, Chiny, Kolumbia i Wietnam.

## <a name="company-name-and-email-characters-abbreviations-and-extensions"></a>Nazwa firmy i znaki e-mail, skróty i rozszerzenia

W poniższych tabelach wymieniono elementy wymienione w [powyższej sekcji nowych](#new-rules-for-company-name-and-email-address) reguł.

### <a name="table-of-special-characters"></a>Tabela znaków specjalnych

| Znaków. | Znaków. | Znaków. | Znaków. |
| ----- | ----- | -----| ----- |
| '~' | '-' |  '=' |  '_' |
|  '#' | '.' |  '%' |  '-' |
|  '+' |  ':' |  '^' |  '[' |
|  '$' |  '–' |  "&" |  ']' |
|  '@' |  '—' |  '*' |  '(' |
|  ',' |  ')' |  '”' |  '⟩' |
|  '`' |  "<" |  '!' |  '\\' |
|  '(' |  ">" |  '“' |  '/' |
|  ')' |  '{' |  '‘' |  '\|' |
|  '\' |  '}' |  '،' |  ':' |
|  ';' |  '⟨' |  '’' | '?' |
|  '”' |  '⟩' |  '\\' |  |


### <a name="table-of-abbreviations"></a>Tabela skrótów

| Abbr. | Abbr. | Abbr. | Abbr. |
| ----- | ----- | ----- | ----- |
|" c p a" | "pty" | "l. l. c." | "gmbh" |
| "c.p.a." | "pty ltd" | "l.l.c." | "zajmij się" |
| "l.l.p." | "pte ltd" | " l l p" | "wll" |
| "c. p. a." | "private limited" | "corp" | "lda" |
| "l. l. p." | "pvt" | "corporation" | "sarl" |
| " l l c" | "pvt ltd" | "inc" | "kft" |
| "corp". | "zrt" | "włączone" | "ltd" |
| "llc". | "ooo" | "ograniczone" | "ltd." |
| "llp". | "llp" | "llc" | "sdn bhd"

### <a name="table-of-top-level-domain-extensions"></a>Tabela rozszerzeń domeny najwyższego poziomu

| Ext.  | Ext.  | Ext.  | Ext. |
| ----- | ----- | ----- | ----- |
| .ac | .ba | .ca | .de |
| .ad | .bb | .cc | .did |
| .ae | .bd | .cd | .dk |
| Af | .be | .cf | .dm |
| Ag | .bf | .cg | .do |
| .ai | .bg | .ch | .zajmij się tym, |
| .al | .bh | .ci | .fm |
| .am | .bi | .ck | .fo |
| .an | .bj | .cl | .fr |
| .ao | .bl | cm | Ga |
| .aq | .bm | .cn | Gb |
| .ar | .bn | .co | .gd |
| .as | .bo | Cr | .ge |
| .at | .bq | .cu | .gf |
| .au | .br | Cv | .gg |
| .aw | .bs | .cw | .gh |
| .ax | .bt | .cx | .gi |
| .az | .zajmij się tym, | .cy | .gl |
| .ec | .bw | .cz | Gm. |
| .ee | .by | .eu | .gn |
| .np. | .bz | .fi | .gp |
| .eh | .es | .fj | GQ |
| .er | .et | .fk | gr |
| .gs | .gw | .hm | .ht |
| .gt | .gy | .hn | .hu |
| .gu | .hk | godz. | .id |
| .ie | .kz | Mo | .nz |
| .il | .la | .mp | .om |
| .im | .lb | .mq | .pa |
| .in | .lc | .mr | .pe |
| .io | .li | Ms | Plik PF |
| .iq | .lk | .mt | .pg |
| .ir | .lr | .mu | .ph |
| .is | .ls | .mv | .pk |
| .it | .lt | .mw | .pl |
| .je | .lu | .mx | .pm |
| .jm | .lv | .my | .pn |
| .jo | .ly | .mz | .pr |
| .jp | .ma | .na | .ps |
| .ke | .mc | .nc | Pt |
| .kg | .md | .ne | .pw |
| .kh | .me | .nf | .py |
| .ki | .mf | .ng | .qa |
| km | .mg | .ni | .re |
| .kn | .mh | .nl | .ro |
| .kp | mk | .no | .rs |
| .kr | .ml | .np | .ru |
| Kw | .mm | .nr | .rw |
| .ky | .mn | .nu | .sa |
| .sb | .tf | .vc | .中国 |
| .sc | .tg | .ve | .中國 |
| .sd | .th | .vg | .భారత్ |
| .se | Tj. | .vi | .ලංකා |
| .sg | .tk | .vn | .ભારત |
| .sh | .tl | .vu | .भारतम् |
| .si | .tm | .wf | .भारत |
| .sj | TN | .ws | .भारोत |
| .sk | .to | .ಭಾರತ | .укр |
| .sl | Tp | .한국 | .香港 |
| .sm | .tr | .ଭାରତ | .台湾 |
| .sn | .tt | .ভাৰত | .台灣 |
| .so | Tv | .ভারত | .мон |
| .sr | .tw | .சிங்கப்பூர் | .tc |
| .ss | .tz | .sz | td |
| .st | .ua | .বাংলা | .uz |
| .su | .ug | .қаз | .va |
| .sv | .uk | .срб | .мкд |
| .sx | .um | .бг | .ею |
| .sy | .us | .бел | Uy |
| .tc | .uz | .мкд |  |

## <a name="next-steps"></a>Następne kroki

- Aby uzyskać więcej informacji o tym, co można sprzedawać klientom za pośrednictwem programu Dostawca rozwiązań w chmurze, zobacz Oferty partnerów w [Dostawca rozwiązań w chmurze programie](csp-offers.md).