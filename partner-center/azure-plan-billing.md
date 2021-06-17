---
title: Rozliczenia planu platformy Azure — pliki & ponownego rozliczania
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak uzyskać dostęp do struktury pliku faktur i uzgodnień związanej z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 725050d370d1266205f979aa6317768d05ae5c4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277185"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure 

**Odpowiednie role:** Agent administracyjny | Administrator rozliczeń | Administrator globalny

W tym artykule wyjaśniono, jak uzyskać dostęp do struktury plików faktur i uzgodnień związanych z rozliczeniami dla planu platformy Azure oraz jak je zrozumieć. Rozliczenia w ramach planu platformy Azure to uproszczone środowisko rozliczeniowe korzystające ze dostosowanej pojedynczej daty rozliczeniowej i okresu rozliczeniowego opartego na miesiącu kalendarzowym.

## <a name="summary-of-billing-essentials"></a>Podsumowanie podstawowych informacji o rozliczeniach

- **Data faktury:** faktura i plik uzgodnień będą dostępne na Partner Center nawigacyjnym/interfejsie API do 8 (północ czasu UTC).

- **Okres rozliczeniowy** faktury: okres rozliczeniowy faktury jest dopasowany do miesiąca kalendarzowego, na przykład 10/1-10/31, 11/1-11/30.

- **Okresy obsługi opłat:** Opłaty będą zgodne z miesiącem kalendarzowym. Jeśli na przykład rozliczany partner dodaje usługi platformy Azure za pośrednictwem planu platformy Azure 10/15 i klient rozpocznie korzystanie z usług platformy Azure 10/15, wówczas rozliczany partner otrzyma fakturę/rekonesję 11/8 za zużycie przez klienta w okresie 10/15–10/31. Faktura za następny miesiąc, która zostanie wygenerowana w dniu 8.12.2018, zawiera wszystkie opłaty za okres 11/1– 11/31.

- **Termin płatności faktury:** 60 dni netto.

- Waluta **faktury:** od 28 stycznia 2021 r. partnerzy w regionie UNII EUROPEJSKIEJ/EFTA i Zjednoczonego Królestwa, którzy mają nowych klientów i istniejących klientów programu CSP, którzy kupują nowe oferty handlowe po raz pierwszy, których dzierżawy zostały utworzone przed 11 maja 2020 r., będą rozliczani za te zakupy w walucie lokalizacji partnera. Partnerzy znajdujący się poza regionem Unii Europejskiej/EFTA i Zjednoczonego Królestwa będą nadal rozliczani w walucie lokalizacji partnera.

- **Zachęty dla partnerów:** Zapłacono 45 dni od końca miesiąca na fakturze.

## <a name="access-your-invoices-and-reconciliation-files"></a>Uzyskiwanie dostępu do faktur i plików uzgodnień

Administrator globalny lub administrator rozliczeń w firmie otrzyma wiadomość e-mail, gdy faktura będzie gotowa do wyświetlenia.

Aby uzyskać dostęp do pliku faktury i uzgodnień:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. Z menu Partner Center wybierz pozycję **Rozliczenia.**

3. Wybierz kartę **Cykliczne** i **Jednorazowa** oraz walutę, która Cię interesuje.

   :::image type="content" source="images/azure/billing3.png" alt-text="Rozliczeń.":::

4. Wybierz **pozycję Plik** faktury lub **uzgodnień.**  

   Aby wyświetlić faktury historyczne i ponownie rozbudować pliki, rozwiń wiersz Historia rozliczeń poniżej.

## <a name="understanding-usage-data"></a>Informacje o danych użycia 

1. Plan platformy Azure jest kontenerem głównym lub najwyższego poziomu do użycia. Całe użycie jest powiązane z pojedynczym planem platformy Azure.

2. W ramach planu będzie co najmniej jedna subskrypcja platformy Azure. Są to kontenery używane do zarządzania zasobami i wdrażania ich. 

3. W ramach subskrypcji grupy zasobów są dodawania do zasobów grupy. Każdy zasób jest wdrażany w jednej grupie zasobów. 

4. Przykładami zasobów są maszyny wirtualne i konta magazynu. 

5. Mierniki emisji zasobów: mierniki to pomiary zużycia zasobu, a jeden zasób może emitować użycie dla wielu mierników. Mierniki są identyfikowane przez productId, SKUId i AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarchia grup zasobów subskrypcji i pomiary

**Konto platformy Azure (dzierżawa)**

- Subskrypcja A
    - ResourceGroup 1
        - Maszyna wirtualna (zasób)
            - Miernik obliczeniowy
        - Sieć wirtualna (zasób)
            - Brak miernika rozliczeń

    - ResourceGroup 2
        - Maszyna wirtualna (zasób)
            - Miernik komputera
        - SSD w warstwie Premium dysku zarządzanego (zasób)
            - Miernik pojemności magazynu
            - Miernik operacji magazynu

- Subskrypcja B — ResourceGroup 1 — Azure SQL (zasób) — miernik jednostek DTU — VPN Gateway (zasób) — miernik bramy sieci VPN

    - ResourceGroup 2
        - Virtual Network interfejs (zasób)
            - Brak miernika rozliczeń

## <a name="read-the-invoice"></a>Odczytywanie faktury

1. Faktura będzie dostępna nie później niż ósmą część każdego miesiąca.

2. Partnerzy mają 60 dni na odmówienie płatności.

3. Okres rozliczeniowy będzie obejmować dany miesiąc kalendarzowy, na przykład 10/1-10/31.

4. Opłaty są naliczane bez korekt (kwota jest netto "środki uzyskane przez partnerów dla zarządzanych usług").

5. Przejrzyj plik rekonesji faktury i plik dziennego użycia z ocenami, aby uzyskać dodatkowe szczegóły rozliczeń.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktury.":::

## <a name="read-the-invoice-reconciliation-file"></a>Odczytywanie pliku uzgodnień faktur

1. Każda kombinacja planu i miernika platformy Azure może zawierać maksymalnie dwa wiersze rozliczeń w pliku rekonescji.

2. Jeśli miernik kwalifikował się do dowolnego typu rabatu lub środków (takich jak rabaty warstwowe lub środki uzyskane przez partnera dla zarządzanych usług) w całym miesiącu kalendarzowym, plik rekonescji będzie zawierać tylko jeden wiersz rozliczeniowy. Kolumna **PriceAdjusmentDescription** będzie odwoływać się do rabatu lub środków zdobytych.

3. Jeśli nie ma żadnych zasobów dla określonego miernika, który kwalifikował się do rabatu lub środków uzyskane przez partnera, plik rekonescji będzie zawierać tylko jedną linię rozliczeniową, a efektywną ceną jednostkową będzie cena detaliczna (czyli cena jednostkowa).

4. Jeśli miernik lub jakiekolwiek zasoby emitujące ten  miernik kwalifikowały się do środków uzyskane przez partnerów dla usług zarządzanych przez część miesiąca, plik rekonescji będzie zawierać dwa wiersze rozliczeń. Jeden wiersz będzie reprezentować dni, w których miernik został zakwalifikowany, a drugi wiersz będzie reprezentować dni, w których miernik nie został zakwalifikowany.

>[!NOTE]
>Możesz uzgodnić zużycie platformy Azure w pliku rekonescji zakupu w ramach jednego zakupu. W tym celu przejdź do pliku rekonescji dziennego użycia ocenianego codziennie i wyszukaj swój subscriptionID. Spowoduje to wyświetlenie wszystkich kosztów skojarzonych z Twoim identyfikatorem planu platformy Azure. Twój azure subscriptionID jest wyświetlany jako EntitlementID.

## <a name="read-the-daily-usage-file"></a>Odczytywanie pliku dziennego użycia

- Mierniki subskrypcji w ramach planu platformy Azure są codziennie oceniane i skumulowane.

- **Środków uzyskane przez partnerów na usługi zarządzane** są określane i stosowane codziennie.

- Każdy miernik subskrypcji będzie miał wiersz dla każdego dnia miesiąca, w którym było zużycie.

- W poniższym przykładzie:

  - Miernik zakwalifikowany do środków **uzyskane przez** partnerów dla usług zarządzanych w okresie od 7/1 do 7/3 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniej środków uzyskane przez partnerów.

  - Miernik nie kwalifikował  się do środków uzyskane przez partnera dla usług zarządzanych w dniach 7/4–7(należy pamiętać, że efektywna cena jednostkowa to cena detaliczna).

  - Miernik zakwalifikowany do środków **zdobytych** przez partnera dla usług zarządzanych w dniach 7/8–7/31 (należy pamiętać, że efektywna cena jednostkowa to cena detaliczna mniej środków uzyskane przez partnerów).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Faktura w walucie klienta

Opłaty za usługi platformy Azure za pośrednictwem planu platformy Azure będą naliczane w USD i rozliczane w walucie przypisanej do kraju klienta. Jeśli waluta rozliczeniowa nie jest w USD, używany kurs wymiany walut (FX) zostanie pokazany na ostatniej stronie faktury. Stawki FX są określane co miesiąc i stosowane do poniższej faktury. Aby uzyskać pełną listę walut krajów, zapoznaj się z nową ofertą handlową na temat dostępności kraju [i macierzą walut klientów.](https://go.microsoft.com/fwlink/?linkid=2112354)

Firma Microsoft obserwuje giełdę w Londynie w celu konwersji. Używamy kursu wymiany, który jest równy kursowi wymiany przechwyconej w ostatniej sekundzie ostatniego dnia biznesowego miesiąca na giełdzie w Londynie. Stawki FX zostaną odświeżone i udostępnione w dniu przed pierwszym miesiącem, którego dotyczą.

## <a name="azure-reservations"></a>Rezerwacje platformy Azure


W przypadku zakupu [rezerwacji platformy Azure](azure-reservations.md) za pośrednictwem planu platformy Azure możesz wybrać rozliczenia godzinowe lub miesięczne.


## <a name="azure-spending"></a>Wydatki na platformie Azure

Istniejące środowisko wydatków na platformę Azure jest aktualizowane w celu obsługi nowych rozliczeń planu platformy Azure w Partner Center. Dzięki temu partnerzy mogą:

- Wyświetlanie i odbieranie alertów dotyczących budżetu ustawionego na poziomie klienta oraz zarządzanie nimi 

- Wyświetlanie łącznych szacowanych wydatków w ramach planu platformy Azure (podzielone według poziomu zasobu i miernika)

Ponieważ model rozliczeń usług platformy Azure za pośrednictwem planu platformy Azure to użycie po płatności, aby uniknąć większego rachunku, niż oczekiwano, partnerzy mogą zastosować miesięczny budżet i śledzić procent użycia. Budżet można zastosować do jednego klienta lub wielu klientów jednocześnie. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Wydatki na platformę Azure.":::

## <a name="next-steps"></a>Następne kroki

- Zobacz, jak są obliczane punkty uzyskane przez partnerów. Zaloguj się na Partner Center [nawigacyjnym i](https://partner.microsoft.com/dashboard/) znajdź dostępny cennik.

- Dowiedz się więcej [o zakupie planu platformy Azure](purchase-azure-plan.md)

- Zobacz cennik nowego doświadczenia handlowego w [programie CSP](azure-plan-price-list.md)
