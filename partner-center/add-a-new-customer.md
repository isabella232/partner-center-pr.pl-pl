---
title: Jak dodać nowy rekord klienta
ms.topic: how-to
ms.date: 09/07/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak dodać nowy rekord klienta w Partner Center. Następnie możesz sprzedawać subskrypcje klientów, zarządzać rozliczeniami lub zapewniać pomoc techniczną dla klientów.
author: parthp
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 7995ee8f4da20d80fd260bcb77665e244e448227
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958210"
---
# <a name="how-to-add-a-new-customer-record-in-partner-center"></a>Jak dodać nowy rekord klienta w Partner Center

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny | Agent sprzedaży

W tym artykule opisano sposób dodawania nowego klienta w Partner Center. Te kroki są wymagane, aby można było sprzedawać subskrypcje, zarządzać rozliczeniami lub zapewniać pomoc techniczną klientowi.

## <a name="considerations"></a>Zagadnienia do rozważenia

**Podczas dodawania nowego rekordu klienta w Partner Center:**

- **Użyj poprawnego identyfikatora rejestracji:** podczas wprowadzania identyfikatora rejestracji firmy należy użyć identyfikatora podatkowego firmy, a nie osobistego identyfikatora klienta.

- **Wprowadź dodatkowe informacje dla niektórych krajów:** [identyfikator](#company-registration-id-and-phone-number-required-for-some-countries) rejestracji firmy i numer telefonu są wymagane w niektórych krajach, jeśli jesteś partnerem rozliczania bezpośredniego lub dostawcą pośrednim
- **Potwierdź** Umowa z Klientem Microsoft: przed zamówieniem w imieniu klienta należy potwierdzić, że klient zaakceptował [Umowa z Klientem Microsoft](confirm-customer-agreement.md).
- **** Użyj różnych kroków dla istniejących klientów: W przypadku istniejących klientów, w tym [](multichannel.md) tych, [](multipartner.md) którzy już mają rekordy klientów w uciecie Partner Center w scenariuszu obejmującym wiele kanałów lub wiele partnerów, [](request-a-relationship-with-a-customer.md)zażądaj relacji z nimi , zamiast wykonać kroki opisane tutaj.
- **Wprowadź szczegółowe, dokładne informacje o kliencie:** aby weryfikacja klienta klientów, upewnij się, że:
  - Wprowadź dokładną nazwę prawna/oficjalną, która będzie wyświetlana w oficjalnych dokumentach.
  - Unikaj używania akronimów lub krótkich formularzy.
  - Nie używaj nazw testów.
  - Podaj pełne, dokładne informacje o adresie (na przykład szczegóły lokalizacji, miasto, stan, kraj i kod pocztowy/pocztowy).

## <a name="new-rules-for-company-name-and-email-address"></a>Nowe reguły dotyczące nazwy firmy i adresu e-mail

Od 22 września 2021 r. będą stosowane następujące nowe reguły weryfikacji.

Podczas wprowadzania nazwy firmy następujące elementy nie będą dozwolone:
- Przy użyciu tylko jednego znaku.
- Używanie tylko znaków specjalnych, takich jak &$^# (zobacz [tabelę](#table-of-special-characters) poniżej).
- Używanie tylko spacji i/lub tabulatorów.
- Używanie autonomicznych skrótów z listy z ograniczeniami, takich jak LLC, Inc itp. (patrz [tabela](#table-of-abbreviations) poniżej).
- Używanie nazw z rozszerzeniami domeny internetowej Top-Level (TDL), takich jak ".com", ".org", ".edu", [](#table-of-top-level-domain-extensions) ".club" itp. (zobacz tabelę poniżej).

- Używanie tego samego znaku powtórzone trzy lub więcej razy bez innych znaków, takich jak 999.

- Używanie spacji i/lub tabulatorów mieszanych z poszczególnymi znakami, takimi jak 1 2 3.

Podczas wprowadzania adresu e-mail klienta następujące warunki nie będą dozwolone:

- Adres e-mail nie może zawierać adresu @microsoft.com .
- Adres e-mail klienta nie może zawierać tej samej nazwy domeny co partner. Na przykład partner o nazwie ABC nie może utworzyć wiadomości e-mail klienta za @abc.com pomocą .

## <a name="to-add-a-new-customer-in-partner-center"></a>Aby dodać nowego klienta w Centrum partnerskim

1. W menu Partner Center wybierz pozycję **Klienci,** a następnie wybierz **pozycję Dodaj klienta.**
2. Jeśli Klient jest instytucją edukacyjną, [zobacz, jak utworzyć klienta zedukcją](sell-to-education-customers.md).

3. Na stronie **Informacje o koncie** wprowadź szczegóły klienta i podstawowe informacje kontaktowe.
   >[!IMPORTANT]
   >Partnerzy muszą mieć następujące atesty:
   >
   >Potwierdzam, że moja organizacja działa jako partner pośredni podczas wybierania odsprzedawcy i partnera bezpośredniego w przypadku braku odsprzedawcy
   >
   >Potwierdzam, że nie odsprzedaję produktów zakupionych w ramach tego zamówienia innym partnerom powiązanym z moją organizacją nadrzędną

   >[!NOTE]
   >Prawo UNII EUROPEJSKIEJ/EFTA stanowi, że partnerzy transakcyjni w tych krajach muszą zadeklarować dodatkowych odsprzedawców skojarzonych w ramach transakcji. Będą stosowane następujące reguły:
   >- Przed żadnymi dodatkowymi odsprzedawcami należy wybrać początkowego odsprzedawcę
   >- Dodatkowi odsprzedawcy nie będą uprawnieni do żadnych dodatkowych zachęt, ofert itp.
   >- Dodatkowi sprzedawcy zostaną zweryfikowani, aby upewnić się, że wprowadzono prawidłowy identyfikator MPN tam, gdzie ma to zastosowanie, oraz że odsprzedawca podpisał umowę MPA.
   >- W ramach transakcji można wprowadzić maksymalnie 5 dodatkowych odsprzedawców 

4. Jeśli jesteś dostawcą pośrednim, wybierz z listy odsprzedawcę pośredniego, który chcesz skojarzyć z subskrypcjami tego klienta.

5. Po zakończeniu wprowadzania wymaganych informacji wybierz pozycję **Dalej: Subskrypcje.**

6. Na **stronie Subskrypcje** wybierz oferty, które klient chce kupić od Ciebie, wprowadź liczbę licencji, a następnie wybierz pozycję **Dalej: Przejrzyj**.

7. Na stronie **Przegląd** sprawdź dokładność wpisów, a następnie wybierz pozycję **Prześlij.**

8. Po zakończeniu dodawania informacji o kliencie i zakupienia wymaganych subskrypcji wybierz pozycję **Gotowe.**

## <a name="company-registration-id-and-phone-number-required-for-some-countries"></a>Identyfikator rejestracji firmy i numer telefonu wymagany w niektórych krajach

Partnerzy z rozliczeniami bezpośrednimi i dostawcy pośredni dodający rekordy dla klientów w następujących krajach muszą również wprowadzić firmowy numer telefonu i identyfikator rejestracji (znany również jako organizacja THE):

W tym celu można chcieć odeznać się w imieniu stanów azji i obronnych.

## <a name="company-name-and-email-characters-abbreviations-and-extensions"></a>Nazwa firmy i znaki wiadomości e-mail, skróty i rozszerzenia

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

| Skrót. | Skrót. | Skrót. | Skrót. |
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
| .ad | .bb | .cc | .zajmij się tym, |
| .ae | .bd | .cd | .dk |
| .af | .be | .cf | .dm |
| .ag | .bf | .cg | .do |
| .ai | .bg | .ch | .zajmij się tym, |
| .al | .bh | .ci | .fm |
| .am | .bi | .ck | .fo |
| .an | .bj | .cl | .fr |
| .ao | .bl | Cm | Ga |
| .aq | .bm | .cn | .gb |
| .ar | .bn | .co | .gd |
| .as | .bo | .cr | .ge |
| .at | .bq | .cu | .gf |
| .au | .br | Cv | .gg |
| .aw | .bs | .cw | .gh |
| .ax | .bt | .cx | .gi |
| .az | .zajmij się tym, | .cy | .gl |
| .ec | .bw | .cz | Gm. |
| .ee | .by | .eu | .gn |
| .np. | .bz | .fi | .gp |
| .eh | .es | .fj | .gq |
| .er | .et | .fk | .gr |
| .gs | .gw | .hm | .ht |
| .gt | .gy | .hn | .hu |
| .gu | .hk | godz. | .id |
| .ie | .kz | Mo | .nz |
| .il | .la | .mp | .om |
| .im | .lb | .mq | .pa |
| .in | .lc | .mr | .pe |
| .io | .li | ms | Plik PF |
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
| .zajmij się tym, | .me | .nf | .py |
| .ki | .mf | .ng | qa |
| km | .mg | .ni | .re |
| .kn | .mh | .nl | .ro |
| .kp | .mk | .no | .rs |
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
| .sj | .tn | .ws | .भारोत |
| .sk | .to | .ಭಾರತ | .укр |
| .sl | Tp | .한국 | .香港 |
| .sm | .tr | .ଭାରତ | .台湾 |
| .sn | .tt | .ভাৰত | .台灣 |
| .so | Tv (tv) | .ভারত | .мон |
| .sr | .tw | .சிங்கப்பூர் | .tc |
| .ss | .tz | .sz | .td |
| .st | .ua | .বাংলা | .uz |
| .su | .ug | .қаз | .va |
| Plik sv | .uk | .срб | .мкд |
| .sx | .um | .бг | .ею |
| .sy | .us | .бел | Uy |
| .tc | .uz | .мкд |  |

## <a name="next-steps"></a>Następne kroki

- Aby uzyskać więcej informacji o tym, co można sprzedawać klientom za pośrednictwem programu Dostawca rozwiązań w chmurze, zobacz Oferty partnerów [w Dostawca rozwiązań w chmurze programu](csp-offers.md)
