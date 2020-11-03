---
title: Centrum partnerskie — szczegółowe raporty CloudAscent
description: Dowiedz się więcej o CloudAscentych raportach dotyczących propiór w centrum partnerskim. Zawiera informacje o promiarach klienta do kupowania produktów firmy Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530579"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent raporty z pulpitu nawigacyjnego Centrum partnerskiego

**Odpowiednie role**
- Executive — Podgląd raportów
- Podgląd raportów

Pulpit nawigacyjny Centrum partnerskiego udostępnia dane umożliwiające pobranie z programu CloudAscent. Dane przedstawiają ofertę klientów, którzy kupują produkty firmy Microsoft.  W tym artykule opisano podział tych danych, sposób wykorzystania oceny i znaczenie.

## <a name="summary-definitions"></a>Definicje podsumowania

- **Klienci** z systemem SMC — jest to całkowita liczba klientów w ramach pobierania.  Klient jest identyfikowany przez partnera rekordu.
- **Umowy wygasają** — w ramach bieżącego roku obrachunkowego firma Microsoft udostępnia liczbę umów wygasających.
- **Przychód** z tytułu wygaśnięcia — przychód związany z umowami wygasania.
- **Otwórz przychód** z tytułu wygaśnięcia — przychód związany z otwartymi umowami o wygaśnięciu.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny podsumowania możliwości klientów.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent segmentacji SMB

Segment małych i średnich firm (SMB) jest dalej podzielony na trzy odrębne Podsegmenty.

1. **Najważniejsze niezarządzane** obejmują największych klientów SMB z największą możliwością dla firmy Microsoft. Typowi niezarządzani klienci mają podobną charakterystykę jako konta zarządzane, za pomocą dużej liczby pracowników, dużych budżetów IT i wydatków oraz dużych ilości potencjalnych przychodów firmy Microsoft.

   Definiujemy najwyższe niezarządzane dwa sposoby:

   - **Najpopularniejszy niezarządzany użytkownik** — obejmuje konta z 300 lub większą liczbą pracowników. Konta User-Based to doskonałe cele zakupu po raz pierwszy lub rozszerzenie produktów subskrypcji opartych na użytkownikach, takich jak M365, D365 lub Surface.
   - W **oparciu o najpopularniejsze niezarządzane obliczenia** — w tym konta o możliwości platformy Azure większej niż $10 tys. Konta oparte na obliczeniach obejmują istniejące platformy Azure. konta z znacznymi możliwościami w przyszłości i kontami, które jeszcze nie kupują platformy Azure, ale mogą korzystać z platformy Azure większej niż $10 tys.

2. **Średnia firma** obejmuje istniejących klientów i konta klientów od 25 do 300 pracowników.

3. **Małe firmy** obejmuje wszystkie pozostałe firmy zatrudniające mniej niż 25 pracowników.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny podsumowania możliwości klientów.":::

**Najpopularniejsze** Podsegmenty niezarządzanych i **średnich firm** przedstawiają klientów z dużą wartością czasu życia (LTV) dla firmy Microsoft i partnerów firmy Microsoft. Z tego względu są to obszary potencjalnego zainteresowania, które koncentrują się na rozwoju w tym segmencie. W tych dwóch podsegmentach lepszym rozwiązaniem jest zdobycie gniazda z M365, Zarabiaj z D365/Azure line of Business (LOB) i zrealizowanie wysokiej LTV dla firmy Microsoft.

Dzisiaj mamy dwa kluczowe obszary szansy sprzedaży — 1. Nasz klient dodaje wzrost; dwóch. Mimo że będziemy dobrze zdobywać gniazda w chmurze wiodące w usłudze M365, mamy dużą okazję w D365 i platformie Azure.

Poniższy zrzut ekranu przedstawia trzy Podsegmenty protokołu SMB i zoptymalizowane trasy do rynku. CloudAscent ustalanie priorytetów profilowania, oceniania i modelowania wszystkich najważniejszych kont niezarządzanych i średnich firm.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny podsumowania możliwości klientów.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

Protokół SMB korzysta z technologii uczenia maszynowego do obsługi prognoz klientów sprzedaży i marketingu w ramach najważniejszych segmentów niezarządzanych i średnich firm. Jak są zbierane sygnały i włączane są zalecenia dotyczące zaleceń?

- **Zbieranie danych** : przeszukiwanie sieci Web skanuje i zbiera miliardy sygnałów klientów przez pingowanie domen firmy i monitorowanie: wpisy w blogu, wersje prasowe, strumienie społecznościowe i fora techniczne.  Oprócz zebranych sygnałów informacje firmographics są zbierane ze źródeł wewnętrznych i zewnętrznych, takich jak D&B, wewnętrzna subskrypcja firmy Microsoft i dane transakcyjne.

- **Machine Learning** : sygnały są przekazywane do modelu uczenia maszynowego, który wyprowadza zestaw danych strukturalnych prognoz sprzedaży i marketingu dla każdego klienta przez produkt i klaster w chmurze.  Każdy klient jest oceniane w oparciu o model podobny do zgodnego protokołu SMB firmy Microsoft, który określa dopasowania klienta i algorytmy uczenia maszynowego, które integrują zachowanie w trybie online klienta zdefiniowane jako intencje. Ocenianie zostanie scalone z klastrami, które pokazują, jak nabycie klientom Microsoft Cloud produkty.

- **Optymalizacja** : system Machine Learning optymalizuje modele przez zużywanie danych transakcji miesięcznie i danych subskrypcji kwartalnie.  Korzystając z danych win/strat, Machine Learning dostosowuje algorytmy i sprawdza, czy modele działają zgodnie z oczekiwaniami, porównując zalecenia dotyczące klastrów z szansami na serwerze głównym.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny podsumowania możliwości klientów.":::

## <a name="cloudascent-propensity"></a>CloudAscent

Jak są tworzone rekomendacje proleceń?

Korzystając z sygnałów zbieranych za pośrednictwem przeszukiwania sieci Web i danych z różnych źródeł, konsolidujemy dane firmographics i sygnały mediów społecznościowych klienta.  Funkcja oceny używa tych sygnałów i danych w modelach porównania dla modeli dopasowania i oceniania dla zamiaru.

1. Dopasowanie konta klienta

   - Wewnętrzne i zewnętrzne punkty danych, które definiują firmographics.

   - Dopasowywanie oceniania przy użyciu modelu podobny do najlepszego protokołu SMB w celu porównania klientów i sprawdzenia, czy są one potencjalnie przydatne dla Microsoft Cloud produktów.

   - Punktacja dopasowania jest aktualizowana co kwartał

2. Cel konta klienta

   - Sygnały związane z mediami społecznościowymi i zachowaniem w trybie online klienta definiują cel.

   - Ocenianie intencji jest nadmiarowe w celu zdefiniowania klastrów.

   - Ocenianie intencji jest aktualizowane co miesiąc.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny podsumowania możliwości klientów.":::

3. Klastrowanie

   Sygnały dopasowania i intencji są konsolidowane do oceny klastrowania. CloudAscent ma cztery klastry:

      - Wykonaj teraz — klienci gotowi do sprzedaży
      - Obliczanie — klienci gotowi do marketingu
      - Kampanie informacyjna
      - Edukacja i monitorowanie zamiaru

   Klastrowanie pozwala użytkownikom na kierowanie określonych klientów do inicjatyw sprzedaży i marketingu na podstawie czynników segmentu, na przykład: produkt, geograficzna, branża i pionowa.

   Karta **model propióra** w skoroszytach CloudAscent udostępnia propozycję i szacowane przychody. Aby zdefiniować klaster dopasowania i zamierzania, wykonaj następujące czynności:

      1. Korzystając z modeli w sieci, najpierw obliczamy wynik i ocenę dopasowania klienta w skali 100.  Dokładne wyniki będą się różnić w zależności od modeli ML.  Przykładowe wyniki poniżej:

         |**Klasyfikacja**|**Dały**|
         |---------|:---------|
         |Wysoki|75 – 100|
         |Średniaa|55 – 74|
         |Niski|30 - 54|
         |Bardzo niski|0 - 29|

      2. Korzystając z powyższej reguły, firma Microsoft klasyfikuje firmy w taki sposób, aby były wysokie, średnie, niskie i bardzo niskie w przypadku sygnałów dopasowania klienta i przeznaczenie.

      3. Wykreślamy sygnały klientów i zamierzeń dla macierzy 2D z każdą wspólną częścią reprezentującą pióro.     Na przykład wysoki poziom dopasowania + wysoki cel = a1, reprezentujący najwyższą z postanowień.

      4. Na koniec te segmenty grupują się do klastrów formularzy.  Na przykład a1, a2, A3, A4 tworzą klaster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny podsumowania możliwości klientów.":::

   W przypadku tych klientów zalecamy teraz kierowanie działaniami i ocenę klientów.

## <a name="cloudascent-products--models"></a>CloudAscent produkty & modele

Poniższa ilustracja przedstawia widok każdego z modeli zapoznawczych w CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny podsumowania możliwości klientów.":::

Modele odstępów składają się z prognoz dla istniejących klientów firmy Microsoft, gdzie nie mają produktu i/lub są klientami usługi NET New potencjalni klienci.

Modele do zakupu wykorzystują dane transakcji, aby przewidzieć potencjalną sprzedaż na platformie Azure i M365 jednostek SKU.

EOS jest udostępniana klientom końca usługi dla win 7, Office 2010, SQL Server i Windows Server. Dane EOS są pobierane z sprzedaży firmy Microsoft i nałożone z użyciem modelowania CloudAscent, jeśli jest dostępny. EOS dane w nowoczesnych zadaniach i sprzedaży platformy Azure.
