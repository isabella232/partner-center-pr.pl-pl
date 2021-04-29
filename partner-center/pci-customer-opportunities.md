---
title: Partner Center Insights — raporty cloudAscent Propensity
description: Dowiedz się więcej o raportach platformy CloudAscent Propensity w Partner Center. Zawiera informacje o tym, czy klient jest podatny na zakup produktów firmy Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213468"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Raporty cloudAscent Propensity dostępne na Partner Center nawigacyjnym

**Odpowiednie role**

- Przeglądarka raportów dla kierownictwa
- Przeglądarka raportów

Pulpit Partner Center udostępnia dane dotyczące proporcjonalności do pobrania z programu CloudAscent. Dane pokazują prawdopodobieństwo zakupu produktów firmy Microsoft przez klientów.  W tym artykule opisano podział tych danych, sposób korzystania z oceniania i jego opis.

## <a name="summary-definitions"></a>Definicje podsumowania

- **Klienci SMC**— jest to łączna liczba klientów w pobranej wersji propensity.  Klienci są identyfikowani przez partnera rekordów.
- **Wygasanie umów**— w bieżącym roku obrachunkowym podamy liczbę wygasających umów.
- **Open Expiring Revenue**— przychód skojarzony z wygasającą umowami otwartymi.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Zrzut ekranu przedstawiający pulpit nawigacyjny Podsumowanie możliwości klientów.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentacja SMB usługi CloudAscent

Segment małych i średnich firm (SMB) jest podzielony na trzy odrębne segmenty podrzędne.

1. **Najliczniejsi** klienci niezamażni obejmują największych klientów SMB z największą szansą dla firmy Microsoft. Typowi klienci z najlepszymi nieza zarządzaniem mają cechy podobne do kont zarządzanych, z dużą liczbą pracowników, dużymi budżetami i wydatkami IT oraz dużymi kwotami potencjalnych przychodów dla firmy Microsoft.

   Zdefiniujmy typ Top Unmanaged na dwa sposoby:

   - **Top Unmanaged User Based**— obejmuje konta z co najmniej 300 pracownikami. User-Based są doskonałymi celami w przypadku zakupu po raz pierwszy lub rozszerzania produktów subskrypcji opartych na użytkownikach, takich jak Microsoft 365, Dynamics 365 lub Surface.
   - **Top Unmanaged Compute Based** — obejmuje konta z możliwością platformy Azure większą niż 10 tys. USD. Konta oparte na obliczeniach obejmują istniejącą platformę Azure. konta ze znaczącym potencjałem przyszłego roku i konta, które jeszcze nie zakupiły platformy Azure, ale mają potencjał platformy Azure większy niż 10 tys. USD.

2. **Średnia firma** obejmuje istniejących klientów i konta potencjalnych klientów od 25 do 300 pracowników.

3. **Małe firmy** obejmują firmy z 10–25 pracownikami.

4. **Bardzo mała firma obejmuje** firmy z 1–9 pracownikami.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Klient według typu kontrolera SMC.":::

**Podsieć Top Unmanaged** and **Medium Business** (Najlepsze podsegmenty dla niezaiemianych i średnich firm) reprezentuje klientów z wysoką wartością czasu życia (LTV, high life-time value) dla firmy Microsoft i partnerów firmy Microsoft. W związku z tym są one głównymi obszarami ukierunkowania na rozwój w tym segmencie. W tych dwóch podsegmentach lepiej jest uzyskać gniazda za pomocą platformy Microsoft 365, dodatkowo nabyć zysk dzięki aplikacjom biznesowym D365/Azure oraz zrealizować wysoką wartość LTV dla firmy Microsoft.

Obecnie mamy dwa kluczowe obszary możliwości — 1. nasz klient zwiększa rozwój; 2. Chociaż dobrze pozyskujemy gniazda w chmurze wiodące w Microsoft 365, mamy duże możliwości w usłudze Dynamics 365 i na platformie Azure.

Poniższy zrzut ekranu przedstawia cztery podsegmenty SMB. Usługa CloudAscent określa priorytety profilowania, oceniania i modelowania dla wszystkich kont z najwyższymi poziomami zarządzania i średniej firmy.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Zrzut ekranu przedstawiający podsegmenty SMB.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

Technologia SMB wykorzystuje technologię uczenia maszynowego do prognozowania sprzedaży i marketingu klientów w segmentach Najważniejsze niezamażowane i Średnie firmy. W jaki sposób sygnały są zbierane i przekształcone w zalecenia dotyczące proporcjonalności?

- **Zbieranie danych:** przeszukiwacze sieci Web skanują i zbierają miliardy sygnałów klientów, wysyłając polecenia ping do domen firmowych oraz monitorując wpisy w blogu, informacje techniczne, strumienie społecznościowe i fora techniczne.  Oprócz zebranych sygnałów informacje firmograficzne są zbierane zarówno ze źródeł wewnętrznych, jak i zewnętrznych, takich jak D&B, wewnętrzna subskrypcja firmy Microsoft i dane transakcyjne.

- **Machine Learning:** Sygnały są podawane do modelu uczenia maszynowego, który wyprowadza ustrukturyzowany zestaw danych przewidywań sprzedaży i marketingu dla każdego klienta według produktu w chmurze i klastra.  Każdy klient jest punktowany przy użyciu modelu podobnego do najlepszego rozwiązania SMB firmy Microsoft, które określa dopasowanie klienta, oraz algorytmów uczenia maszynowego, które integrują zachowanie online klienta, definiując je jako intencję. Ocenianie jest scalane w klastry, które pokazują, że klient jest podatny na zakup produktów w chmurze firmy Microsoft.

- **Optymalizacja:** system Machine Learning optymalizuje modele, zużywając dane transakcji co miesiąc i dane subskrypcji co kwartał.  Korzystając z danych o wygranej/utracie, Machine Learning dostosowuje algorytmy i sprawdza, czy modele działają zgodnie z oczekiwaniami, porównując zalecenia dotyczące klastrów z szansami sprzedaży, na których działa usługa MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Zrzut ekranu przedstawiający uczenie maszynowe SMB.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

W jaki sposób są tworzone rekomendacje dotyczące proporcjonalności?

Używając sygnałów zebranych za pośrednictwem przeszukiwarów sieci Web i danych dostarczanych z różnych źródeł, konsolidujemy dane firmographics i sygnały mediów społecznościowych klienta.  Ocenianie używa tych sygnałów i danych w modelach porównywania do dopasowania i oceniania modeli intencji.

1. Dopasowanie konta klienta

   - Wewnętrzne i zewnętrzne punkty danych definiujące firmographics.

   - Ocenianie dopasowania wykorzystuje model podobny do naszego najlepszego SMB, aby porównać klientów i sprawdzić, czy są potencjalnie odpowiedni dla produktów w chmurze firmy Microsoft.

   - Ocenianie dopasowania jest aktualizowane co kwartał

2. Intencja konta klienta

   - Sygnały związane z mediami społecznościowymi i zachowaniem online klienta definiują intencję.

   - Ocenianie intencji jest nałogowe na dopasowanie w celu zdefiniowania klastrów.

   - Ocenianie intencji jest aktualizowane co miesiąc.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modele predykcyjne SMB cloudAscent.":::

3. Klastrowanie

   Sygnały dopasowania i intencji są konsolidowane w wyniku klastrowania. CloudAscent ma cztery klastry:

      - Działanie teraz — klienci gotowi do sprzedaży
      - Ocena — klienci gotowi do marketingu
      - Świadomość — wspieranie kampanii świadomości
      - Edukowanie — edukowanie i monitorowanie intencji

   Klastrowanie umożliwia użytkownikom ukierunkowanie określonych klientów na inicjatywy sprzedażowe i marketingowe na podstawie czynników segmentu, takich jak produkt, obszar geograficzny, branża i pionowa.

   Karta **Model proporcjonalności** w skoroszytach CloudAscent udostępnia proporcjonalność i szacowany przychód z białych znaków. Aby zdefiniować klastrowanie dopasowania i intencji, należy wykonać następujące kroki:

      1. Korzystając z modeli uczenia maszynowego, najpierw obliczamy współczynnik dopasowania klienta i wynik intencji w skali 100.  Dokładne wyniki będą się różnić w zależności od modeli uczenia maszynowego.  Przykładowe wyniki poniżej:

         |**Klasyfikacja**|**Ocena**|
         |---------|:---------|
         |Wys.|75 - 100|
         |Śred.|55 - 74|
         |Niski|30 - 54|
         |Bardzo niska|0 - 29|

      2. Korzystając z powyższej reguły, klasyfikujemy firmy jako wysokie, średnie, niskie i bardzo niskie zarówno dla sygnałów dopasowania klienta, jak i intencji.

      3. Wykreślamy sygnały dopasowania i intencji klienta na macierzy 2D z każdym przecięciem reprezentującym proporcjonalność. Na przykład High Fit + High Intent = A1, reprezentujący najwyższą wartość.

      4. Na koniec te segmenty grupuje się w celu tworzenia klastrów.  Na przykład A1, A2, A3, A4 tworzą klaster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modele CloudAscent.":::

   W przypadku tych klientów zalecamy ukierunkowanie działań Na teraz i Ocena klientów.

## <a name="cloudascent-products--models"></a>Modele produktów CloudAscent & Model

Na poniższej ilustracji przedstawiono widok każdego modelu proporcjonalności w aplikacji CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Model proporcjonalności CloudAscent.":::

Modele odstępów składają się z przewidywań dla istniejących klientów firmy Microsoft, którzy nie mają produktu i/lub są nowymi klientami potencjalnymi klientami netto.

Modele sprzedaży upsell używają danych transakcji do przewidywania potencjalnej sprzedaży upsell na platformie Azure i Microsoft 365 SKU.

Ci klienci będą już mieć platformę Azure lub Microsoft 365, a model sprzedaży upsell wskazuje, że prawdopodobnie kupi więcej swojej istniejącej wersji SKU.

System EOS udostępnia klientów końcowych usług (EOS) dla systemów Win 7, Office 2010, SQL Server i Windows Server. Dane systemu EOS są ściągane z usługi MS Sales i są nałożyne na modelowanie proporcjonalności CloudAscent, jeśli jest dostępne. Dane systemu EOS są wykorzystywane w nowoczesnego rozwiązaniach pracy i sprzedaży na platformie Azure.
