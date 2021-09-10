---
title: Znajdowanie liczby komputerów stacjonarnych i poziomu opłat
ms.topic: how-to
ms.date: 02/18/2021
description: Dowiedz się, jak za pomocą platformy Channel Incentives (CHIP) znaleźć informacje o liczbach pulpitów i poziomie opłat dla umowy.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959482"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Lokalizowanie liczby komputerów i poziomu opłat dla umowy

**Odpowiednie role:** Podstawowy kontakt lub administrator programu

Możesz zalogować się do [explore.ms,](https://www.explore.ms/) aby zapoznać się z umową, lub pobrać plik ze szczegółami umowy dla liczby komputerów stacjonarnych i poziomu opłat.

## <a name="to-locate-the-information"></a>Aby zlokalizować informacje

### <a name="method-1--explorems"></a>Metoda 1 – Explore.ms

1. Otwórz [explore.ms](https://www.explore.ms/) w Internet Explorer. 

>[!Note]
>Tej funkcji nie można wykonywać w przeglądarce Google Chrome ani Microsoft Edge.

2. Zaloguj się przy użyciu konta służbowego lub identyfikatora na żywo.  

3. W polu **Raporty** wybierz pozycję **Umowy**.

4. Na stronie wynikowej wprowadź numer umowy w polu **Wyszukaj,** a następnie wybierz **pozycję Wybierz/zamów kolumny.**

5. W oknie podręcznym wybierz pozycję **Umowa —** liczba komputerów stacjonarnych z listy dostępnych kolumn, a następnie wybierz strzałkę w prawo, aby dodać kolumnę. Wybierz przycisk **OK**.

6. Wybierz **pozycję Wyszukaj.**

7. Na ekranie wynikowym przewiń wyniki, aby znaleźć kolumnę **Liczba pulpitów umowy.** 

8. Użyj licznika pulpitu, aby określić poziom opłaty na podstawie poniższej tabeli stawek.  

| Poziom opłaty | Liczba komputerów stacjonarnych |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Enterprise Poziomy zachęt są oparte na liczby komputerów stacjonarnych lub użytkowników (w zależności od tego, która wartość jest wyższa) w rejestracjach w sektorze komercyjnym i publicznym (PS). W przypadku rejestracji bez naturalnie skojarzonej liczby komputerów stacjonarnych lub użytkowników firma Microsoft stosuje liczbę komputerów stacjonarnych na podstawie liczby komputerów stacjonarnych lub liczby użytkowników towarzyszącej umowy EA. <br><br>Jeśli nie ma towarzyszącej umowy EA, poziom opłaty jest oparty na poziomie cen rejestracji. Poziom cen transakcji można również wyświetlić na stronie [www.explore.ms.](https://www.explore.ms/) <br><br>Jeśli na istniejącej platformie EA/EAS istnieje wiele poziomów puli i/lub cen, firma Microsoft zapłaci zachęty na najwyższym przypisanym poziomie cen/puli, a poziom A będzie najniższy, a poziom D będzie najwyższy.

#### <a name="pool-and-pricing-levels"></a>Pula i poziomy cen

Po wyszukaniu numeru umowy w explore.ms krokach opisanych powyżej wybierz numer umowy. Spowoduje to dostęp do strony szczegółów umowy, na której będą wyświetlane podsumowanie **umowy** i **oferty**. Sekcja ofert zawiera poziomy cen.

## <a name="method-2---chip"></a>Metoda 2 — CHIP

1. Zaloguj się do chipu i wybierz pozycję LSP Incentives (Zachęty LSP).

2. Na stronie **Podsumowanie płatności** partnera wybierz miesiąc raportowania, który  chcesz wyświetlić, a następnie wybierz pozycję Szczegóły obliczeń z listy rozwijanej w obszarze Eksportuj do **Excel:**

:::image type="content" source="images/chip/chiplocate.png" alt-text="Zlokalizuj szczegóły programu.":::

3. Eksport zostanie rozpocznie się i będzie można otworzyć plik lub zapisać/zapisać jako miejsce docelowe.

4. Po otwarciu raportu przejdź do karty **DetailReport-FlatFile** w lewym dolnym rogu:

:::image type="content" source="images/chip/flatfile.png" alt-text="Pobieranie pliku płaskiego.":::

Teraz możesz wyszukać numer umowy, którego szukasz, w kolumnie J. Przypisana liczba pulpitów znajduje się w kolumnie R z etykietą Agreement_DesktopCount. Poziom opłaty dla tej umowy można również potwierdzić w kolumnie "AI" z etykietą Warstwa.

## <a name="next-steps"></a>Następne kroki

- [Rozwiązywanie problemów z dostępem do mikroukładu](chip-access-trouble.md)
