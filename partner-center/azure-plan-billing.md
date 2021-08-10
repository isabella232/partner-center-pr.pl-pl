---
title: Rozliczenia planu platformy Azure — pliki & rekonfigurowane
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Dowiedz się, jak uzyskać dostęp do struktury plików faktur i uzgodnień związanej z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ece8323ba8943ab7615b65fe02834db086b5eac
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/04/2021
ms.locfileid: "115102373"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure 

**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny

W tym artykule wyjaśniono, jak uzyskać dostęp do struktury plików faktur i uzgodnień związanej z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć. Rozliczenia w ramach planu platformy Azure to uproszczone środowisko rozliczeniowe korzystające ze dostosowanej pojedynczej daty rozliczeniowej i okresu rozliczeniowego opartego na miesiącu kalendarzowym.

## <a name="summary-of-billing-essentials"></a>Podsumowanie podstawowych informacji dotyczących rozliczeń

- **Data faktury:** faktura i plik uzgodnień będą dostępne na pulpicie nawigacyjnym Partner Center nawigacyjnym/interfejsie API do 8 dnia (północ czasu UTC).

- **Okres rozliczeniowy** faktury: okres rozliczeniowy faktury jest dopasowany do miesiąca kalendarzowego, na przykład 10/1-10/31, 11/1-11/30.

- **Okresy obsługi opłat:** opłaty będą zgodne z miesiącem kalendarzowym. Jeśli na przykład rozliczany partner dodaje usługi platformy Azure za pośrednictwem planu platformy Azure 10/15 i klient rozpocznie korzystanie z usług platformy Azure 10/15, rozliczany partner otrzyma fakturę/rekonesję w dniu 8.11.2015 r. za zużycie przez klienta w okresie 10/15 – 10/31. Faktura za następny miesiąc, która zostanie wygenerowana w dniu 8.12.2018, zawiera wszystkie opłaty za okres 11/1– 11/31.

- **Termin płatności faktury:** 60 dni netto.

- Waluta **faktury:** od 28 stycznia 2021 r. partnerzy w regionie Unii Europejskiej/DSM i Zjednoczonego Królestwa, którzy mają nowych klientów i istniejących klientów programu CSP, którzy po raz pierwszy kupują nowe oferty handlowe, których dzierżawy zostały utworzone przed 11 maja 2020 r., będą rozliczani za te zakupy w walucie lokalizacji partnera. Partnerzy znajdujący się poza regionem Unii Europejskiej/DSM i Zjednoczonego Królestwa będą nadal rozliczani w walucie lokalizacji partnera.

- **Zachęty dla partnerów:** Zapłacono 45 dni od końca miesiąca na fakturze.

## <a name="access-your-invoices-and-reconciliation-files"></a>Uzyskiwanie dostępu do faktur i plików uzgodnień

Gdy faktura będzie gotowa do wyświetlenia, administrator globalny lub administrator rozliczeń w firmie otrzyma wiadomość e-mail.

Aby uzyskać dostęp do pliku faktury i uzgodnień:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. Z menu Partner Center wybierz pozycję **Rozliczenia.**

3. Wybierz kartę **Cykliczne** **i Jednorazowa** oraz walutę, która Cię interesuje.

   :::image type="content" source="images/azure/billing3.png" alt-text="Rozliczeń.":::

4. Wybierz **pozycję Plik** faktury lub **uzgodnień.**  

   Aby wyświetlić historyczne faktury i ponownie rozbudować pliki, rozwiń wiersz Historia rozliczeń poniżej.

## <a name="understanding-usage-data"></a>Informacje o danych użycia 

1. Plan platformy Azure to główny lub najwyższego poziomu kontener do użycia. Całe użycie jest powiązane z pojedynczym planem platformy Azure.

2. W ramach planu będzie co najmniej jedna subskrypcja platformy Azure. Są to kontenery używane do zarządzania zasobami i ich wdrażania. 

3. W ramach subskrypcji grupy zasobów są dodawania do zasobów grupy. Każdy zasób jest wdrażany w jednej grupie zasobów. 

4. Przykłady zasobów obejmują maszyny wirtualne i konta magazynu. 

5. Mierniki emisji zasobów: mierniki to pomiary zużycia zasobu, a jeden zasób może emitować użycie dla wielu mierników. Mierniki są identyfikowane przez productId, SKUId i AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarchia grup zasobów subskrypcji i pomiary

**Konto platformy Azure (dzierżawa)**

- Subskrypcja A
    - ResourceGroup 1
        - Maszyna wirtualna (zasób)
            - Miernik zasobów obliczeniowych
        - Sieć wirtualna (zasób)
            - Brak miernika rozliczeń

    - ResourceGroup 2
        - Maszyna wirtualna (zasób)
            - Miernik komputera
        - Premium Dysk zarządzany przez dysk SSD (zasób)
            - Storage miernik pojemności
            - Storage operacyjny

- Subskrypcja B — ResourceGroup 1 — azure SQL (zasób) — miernik jednostek DTU — VPN Gateway (zasób) — miernik bramy sieci VPN

    - ResourceGroup 2
        - Virtual Network interfejs (zasób)
            - Brak miernika rozliczeń

## <a name="read-the-invoice"></a>Odczytywanie faktury

1. Faktura będzie dostępna nie później niż w ósmej części każdego miesiąca.

2. Partnerzy mają 60 dni na odmówienie płatności.

3. Okres rozliczeniowy będzie obejmować dany miesiąc kalendarzowy, na przykład 10/1-10/31.

4. Opłaty są naliczane netto korekt (kwota wynosi net "Środki uzyskane przez partnerów dla zarządzanych usług").

5. Zapoznaj się z plikiem rekonesfiguracji faktury i plikiem dziennego użycia, aby uzyskać dodatkowe szczegóły rozliczeń.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktury.":::

## <a name="read-the-invoice-reconciliation-file"></a>Odczytywanie pliku uzgodnień faktur

1. Każda kombinacja planu i miernika platformy Azure może zawierać maksymalnie dwa wiersze rozliczeń w pliku rekonesfigurowania.

2. Jeśli miernik kwalifikował się do dowolnego typu rabatu lub środków (takich jak rabaty warstwowe lub środki uzyskane przez partnera dla usług zarządzanych przez partnera) w całym miesiącu kalendarzowym, plik rekonesfiguracji będzie zawierać tylko jedną linię rozliczeniową. Kolumna **PriceAdjusmentDescription** będzie odwoływać się do rabatu lub środków zdobytych.

3. Jeśli nie ma żadnych zasobów dla określonego miernika, który kwalifikował się do rabatu lub środków uzyskane przez partnera, plik rekonescji będzie zawierać tylko jedną linię rozliczeniową, a efektywną ceną jednostkową będzie cena detaliczna (czyli cena jednostkowa).

4. Jeśli miernik lub jakiekolwiek zasoby emitujące ten  licznik kwalifikowały się do środków uzyskane przez partnera dla usług zarządzanych przez część miesiąca, plik rekonescji będzie zawierać dwa wiersze rozliczeń. Jeden wiersz będzie reprezentować dni, w których miernik został zakwalifikowany, a drugi wiersz będzie reprezentować dni, w których miernik się nie kwalifikował.

>[!NOTE]
>Możesz uzgodnić zużycie platformy Azure w pliku ponownego zakupu w ramach jednego zakupu. W tym celu przejdź do pliku z rekonescją dziennego użycia i wyszukaj swój subscriptionID. Spowoduje to wyświetlenie wszystkich kosztów skojarzonych z identyfikatorem planu platformy Azure. Twoja subskrypcja platformy Azure jest wyświetlana jako entitlementID.

## <a name="read-the-daily-usage-file"></a>Odczytywanie pliku dziennego użycia

- Mierniki subskrypcji w ramach planu platformy Azure są codziennie oceniane i skumulowane.

- **Środków uzyskane przez partnerów na usługi zarządzane** są określane i stosowane codziennie.

- Każdy licznik subskrypcji będzie miał wiersz dla każdego dnia miesiąca, w którym było zużycie.

- W poniższym przykładzie:

  - Miernik zakwalifikowany do środków **uzyskane** przez partnerów dla usług zarządzanych w okresie od 7/1 do 7/3 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniejsza niż kredyt uzyskane przez partnera.

  - Miernik nie kwalifikował  się do środków uzyskane przez partnerów na usługi zarządzane w okresie od 7/4 do 7/7 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna).

  - Miernik **zakwalifikowany** do środków uzyskane przez partnerów dla usług zarządzanych w okresie od 7/8 do 7/31 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniejsza niż kredyt uzyskane przez partnera).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Faktura w walucie klienta

Opłaty za usługi platformy Azure w ramach planu platformy Azure będą naliczane w USD w walucie przypisanej do kraju klienta. Jeśli waluta rozliczeniowa nie jest w USD, używany kurs wymiany walut (FX) będzie wyświetlany na ostatniej stronie faktury. Stawki FX są określane co miesiąc i stosowane do poniższej faktury. Aby uzyskać pełną listę walut krajów, zapoznaj się z nową ofertą handlową dla dostępności [kraju i macierzą walut klientów.](https://go.microsoft.com/fwlink/?linkid=2112354)

Firma Microsoft stosuje wstępnie określony kurs wymiany do podstawowych cen USD, aby uzyskać łączne opłaty naliczane za usługi platformy Azure zakupione lub zużyte w każdym miesiącu kalendarzowym. Miesięczny kurs wymiany to średni kurs opublikowany przez thomson Reuters (zazwyczaj) dwa dni robocze przed końcem poprzedniego miesiąca o godzinie 16:00 GMT. 

**Na przykład** Grudniowy kurs wymiany firmy Microsoft będzie wartością średniego kursu wymiany Thomson Reuters z 29 listopada lub około 29 listopada dla danej waluty. Ta stawka będzie stosowana do wszystkich zakupów w tej walucie od 1 grudnia do 31 grudnia. 

## <a name="azure-reservations"></a>Rezerwacje platformy Azure


W przypadku zakupu [rezerwacji platformy Azure](azure-reservations.md) za pośrednictwem planu platformy Azure możesz wybrać rozliczenia godzinowe lub miesięczne.


## <a name="azure-spending"></a>Wydatki na platformie Azure

Istniejące środowisko wydatków na platformę Azure jest aktualizowane w celu obsługi nowych rozliczeń planu platformy Azure w Partner Center. Dzięki temu partnerzy mogą:

- Wyświetlanie i odbieranie alertów dotyczących budżetu ustawionego na poziomie klienta oraz zarządzanie nimi 

- Wyświetlanie łącznych szacowanych wydatków w ramach planu platformy Azure (z podziałem na zasoby i poziom miernika)

Ponieważ model rozliczeń dla usług platformy Azure za pośrednictwem planu platformy Azure to użycie po płatności, aby uniknąć większego rachunku, niż oczekiwano, partnerzy mogą zastosować miesięczny budżet i śledzić procent użycia. Budżet można zastosować do jednego klienta lub wielu klientów jednocześnie. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Wydatki na platformę Azure.":::

## <a name="next-steps"></a>Następne kroki

- Zobacz, jak są obliczane punkty uzyskane przez partnerów. Zaloguj się na Partner Center [nawigacyjnym i](https://partner.microsoft.com/dashboard/) znajdź dostępny cennik.

- Dowiedz się więcej [o zakupie planu platformy Azure](purchase-azure-plan.md)

- Zobacz cennik nowego doświadczenia handlowego w [programie CSP](azure-plan-price-list.md)
