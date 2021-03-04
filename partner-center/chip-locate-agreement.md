---
title: Znajdź liczbę komputerów i poziom opłat
ms.topic: how-to
ms.date: 02/18/2021
description: Dowiedz się, jak korzystać z platformy zachęt w kanale (MIKROUKŁAD), aby znaleźć informacje o liczbie komputerów i poziomie opłaty dla umowy.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756110"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Lokalizowanie liczby komputerów i poziomu opłat dla umowy

**Odpowiednie role**

- Podstawowy kontakt lub administrator programu

Możesz zalogować się do usługi [Explore.MS](https://www.explore.ms/) , aby zapoznać się z umową, lub pobrać plik zawierający szczegóły umowy dotyczącej liczby komputerów i poziomu opłat.

## <a name="to-locate-the-information"></a>Aby zlokalizować informacje

### <a name="method-1--explorems"></a>Metoda 1 – Explore.ms

1. Otwórz program [Explore.MS](https://www.explore.ms/) w programie Internet Explorer. 

>[!Note]
>Nie można wykonać tej funkcji w przeglądarce Google Chrome lub Microsoft Edge.

2. Zaloguj się przy użyciu konta służbowego lub identyfikatora na żywo.  

3. W polu **raporty** wybierz pozycję **umowy**.

4. Na stronie wyników wprowadź numer umowy w polu **wyszukiwania** , a następnie wybierz pozycję **kolumny wybierz/Zamów**.

5. W oknie podręcznym wybierz pozycję **Liczba pulpitów umowy** z listy Dostępne kolumny, a następnie wybierz strzałkę w prawo, aby dodać kolumnę. Wybierz przycisk **OK**.

6. Wybierz pozycję **Wyszukaj.**

7. Na wynikowym ekranie Przewiń wyniki, aby znaleźć kolumnę **liczba komputerów z umową** . 

8. Użyj liczby pulpitów, aby określić poziom opłat w oparciu o tabelę stawek poniżej.  

| Poziom opłat | Liczba komputerów |
| ------ | :-----------: |
|  A | 0 – 2 399    |
|  B | 2 400 – 5 999    |
|  C | 6 000 – 14 999    |
|  D | 15000 +   |

>[!NOTE]
>Poziom zachęty dla przedsiębiorstw jest oparty na liczbie komputerów stacjonarnych lub użytkowników (w zależności od tego, który jest wyższy) w przypadku rejestracji w sektorach komercyjnych i publicznych (PS). W przypadku rejestracji bez fizycznej liczby skojarzonych komputerów osobistych i użytkowników firma Microsoft stosuje liczbę komputerów w zależności od liczby komputerów lub liczby użytkowników towarzyszącej umowie EA. <br><br>W przypadku braku towarzyszącej umowy EA poziom opłat jest oparty na poziomie cennika rejestracji. Poziom cen transakcji można także wyświetlić w witrynie [www.Explore.MS](https://www.explore.ms/). <br><br>Jeśli istnieje wiele poziomów puli i/lub cen na istniejącym EA/EAS, firma Microsoft będzie zapłaciła zachęty na najwyższy przypisany poziom cen/puli, a poziom A jest najniższym i wyższym niż poziom D.

#### <a name="pool-and-pricing-levels"></a>Poziomy puli i cennika

Po wyszukaniu numeru umowy w explore.ms, korzystając z kroków opisanych powyżej, wybierz numer umowy. Spowoduje to przejście do strony szczegóły umowy, która będzie zawierać **Podsumowanie umów** i **oferty**. Sekcja oferty zawiera poziomy cen.

## <a name="method-2---chip"></a>Metoda 2 — MIKROUKŁAD

1. Zaloguj się do układu i wybierz opcję zachęty dla dostawcy LSP.

2. Na stronie **Podsumowanie płatności dla partnerów** wybierz miesiąc sprawozdawczy, który chcesz wyświetlić, a następnie wybierz pozycję **szczegóły obliczeń** z listy rozwijanej w obszarze **Eksportuj do programu Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Znajdź szczegóły programu":::

3. Zostanie rozpoczęty eksport i można otworzyć plik lub zapisać/zapisać jako miejsce docelowe.

4. Gdy raport jest otwarty, przejdź do karty **DetailReport-Flatfile** w lewym dolnym rogu:

:::image type="content" source="images/chip/flatfile.png" alt-text="Pobieranie pliku prostego":::

Możesz teraz wyszukać numer umowy, którego szukasz, w kolumnie J. w kolumnie R oznaczonej jako liczba przypisanych pulpitów znajdziesz przypisaną liczbę komputerów, która ma Agreement_DesktopCount. Możesz również potwierdzić poziom opłat dla tej umowy w kolumnie "AI" z etykietą.

## <a name="next-steps"></a>Następne kroki

- [Rozwiązywanie problemów z dostępem do układu scalonego](chip-access-trouble.md)
