---
title: Azure plan rozliczania — faktury & pliki Rekonesans
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak uzyskać dostęp do struktury plików faktur i uzgodnień uzgadniania dla planu platformy Azure i zrozumieć ją.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: e230cc0d8ff3afea4bf2cc7b55d3847814696af6
ms.sourcegitcommit: f99424919f0d77bbe4f44293d84f9ea1e3317f13
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/21/2021
ms.locfileid: "98658437"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure 

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Administrator globalny

W tym artykule wyjaśniono, jak uzyskać dostęp do struktury pliku faktury i uzgodnienia dotyczącej rozliczeń dla planu platformy Azure i zrozumieć ją. Rozliczenia zgodnie z planem platformy Azure to uproszczone środowisko rozliczeniowe korzystające z wyrównanej pojedynczej daty rozliczania i okresu rozliczeniowego w kalendarzu.

## <a name="summary-of-billing-essentials"></a>Podsumowanie podstawy rozliczeń

- **Data faktury**: plik faktury i uzgodnienia będą dostępne na pulpicie nawigacyjnym/interfejsie API Centrum partnerskiego przez 8 (północy czasu UTC).

- **Okres rozliczeniowy faktury**: okres rozliczeniowy faktury jest wyrównany do miesiąca kalendarzowego, na przykład 10/1-10/31, 11/1-11/30.

- **Opłaty za okresy usługi**: opłaty zostaną wyrównane do miesiąca kalendarzowego. Na przykład jeśli Partner rozliczeń dodaje usługi platformy Azure w ramach planu platformy Azure w dniu 10/15, a klient zacznie zużywać usługi platformy Azure w dniu 10/15, wówczas rozliczenia partner otrzymają faktury/Rekonesans na 11/8 w celu użycia przez klienta okresu usługi 10/15-10/31. Faktury w następnym miesiącu, które mają zostać wygenerowane w dniu 12/8, zawierają wszystkie opłaty za okres usługi 11/1-11/31.

- **Termin płatności faktury**: NET 60 dni.

- **Waluta faktury**: partnerzy będą nadal rozliczani w country'sej walucie klienta. Na przykład jeśli Partner rozliczy jest w Irlandii z klientami w Wielkiej Brytanii, Norwegii i Niemczech, wówczas rozliczka będzie otrzymywać GBP, NOK i fakturę w EUR/rekonesans.

- **Zachęty dla partnerów**: płatne 45 dni od końca miesiąca faktury.

## <a name="access-your-invoices-and-reconciliation-files"></a>Uzyskiwanie dostępu do faktur i plików uzgadniania

Administrator globalny lub administrator rozliczeń dla Twojej firmy otrzyma wiadomość e-mail, gdy faktura będzie gotowa do wyświetlenia.

Aby uzyskać dostęp do pliku faktury i uzgodnienia:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. W menu Centrum partnerskiego wybierz pozycję **rozliczenia**.

3. Wybierz kartę **cykliczną** i **jednorazową** oraz daną walutę.

   :::image type="content" source="images/azure/billing3.png" alt-text="godzin":::

4. Wybierz pozycję **Faktura** lub **plik uzgadniania**.  

   Aby wyświetlić historyczne faktury i pliki Rekonesans, rozwiń wiersz historia rozliczeń poniżej.

## <a name="understanding-usage-data"></a>Informacje o użyciu 

1. Azure plan to główny lub najwyższego poziomu kontenera do użycia. Całe użycie jest powiązane z powrotem z jednym planem platformy Azure.

2. W ramach planu będzie co najmniej jedna subskrypcja platformy Azure. Są to kontenery używane do zarządzania zasobami i ich wdrażania. 

3. W ramach subskrypcji grupy zasobów dodają do zasobów grupy. Każdy zasób jest wdrażany w jednej grupie zasobów. 

4. Przykłady zasobów obejmują maszyny wirtualne i konta magazynu. 

5. Liczniki emisji zasobów: Liczniki są pomiary zużycia zasobu, a jeden zasób może emitować użycie dla wielu liczników. Liczniki są identyfikowane przez ProductId, identyfikatora skuId i AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarchia grup zasobów i pomiarów subskrypcji

**Konto platformy Azure (dzierżawca)**

- Subskrypcja A
    - Przesourceing 1
        - Maszyna wirtualna (zasób)
            - Licznik obliczeń
        - Sieć wirtualna (zasób)
            - Brak licznika rozliczeń

    - Przesourceing 2
        - Maszyna wirtualna (zasób)
            - Licznik komputera
        - Dysk zarządzany przez SSD w warstwie Premium (zasób)
            - Licznik pojemności magazynu
            - Licznik operacji magazynu

- Subskrypcja B — resourceing 1 — Azure SQL (Resource) — metry jednostek DTU-VPN Gateway (zasób) — licznik bramy sieci VPN

    - Przesourceing 2
        - Interfejs Virtual Network (zasób)
            - Brak licznika rozliczeń

## <a name="read-the-invoice"></a>Przeczytaj fakturę

1. Faktura będzie dostępna nie później niż w ciągu każdego miesiąca.

2. Partnerzy mają 60 dni, aby przekazać płatność.

3. Okres rozliczeniowy będzie obejmować dany miesiąc kalendarzowy, na przykład 10/1-10/31.

4. Opłaty są naliczane za liczbę netto korekt (kwota to netto za "Partner".

5. Aby uzyskać dodatkowe informacje dotyczące rozliczeń, zapoznaj się z plikiem faktury Rekonesans i dzienną oceną plików użycia.

   :::image type="content" source="images/azure/invoice1.png" alt-text="faktury":::

## <a name="read-the-invoice-reconciliation-file"></a>Przeczytaj plik uzgadniania faktur

1. Każda kombinacja planu i licznika platformy Azure może mieć do dwóch wierszy rozliczeń w pliku rekonesans.

2. Jeśli licznik zakwalifikowany dla dowolnego typu rabatu lub kredytu (na przykład rabaty warstwowe lub środki uzyskane przez partnera dla usług zarządzanych) w całym miesiącu kalendarzowym, plik Rekonesans będzie zawierać tylko jedną linię rozliczenia. Kolumna **PriceAdjusmentDescription** będzie odwoływać się do rabatu lub środków uzyskanych z tytułu uznania.

3. Jeśli nie ma zasobów dla określonego licznika, które kwalifikują się do rabatu lub dla partnerów, plik Rekonesans będzie zawierać tylko jedną linię rozliczeniową, a obowiązująca cena jednostkowa to cena detaliczna (czyli cena jednostkowa).

4. Jeśli licznik lub wszystkie zasoby emitujące Ten licznik są zakwalifikowane dla partnerów w ramach **usług zarządzanych** przez część miesiąca, plik Rekonesans będzie zawierać dwa wiersze rozliczania. Jeden wiersz będzie reprezentować dni kwalifikowane, a drugi wiersz będzie reprezentować dni, w których licznik nie kwalifikuje się.

## <a name="read-the-daily-usage-file"></a>Przeczytaj plik dziennego użycia

- Liczniki subskrypcji w ramach planu platformy Azure są klasyfikowane i są skumulowane w ujęciu dziennym.

- Środki na korzystanie z **usług zarządzanych przez partnerów** są określane i stosowane codziennie.

- Każdy miernik subskrypcji będzie miał wiersz na każdy dzień miesiąca, w którym wystąpiło zużycie.

- W poniższym przykładzie:

  - Zliczanie środków zakwalifikowanych dla **partnerów uzyskano środki dla usług zarządzanych** przez 7/1-7/3 (Zwróć uwagę na to, że obowiązująca cena jednostkowa to cena detaliczna pomniejszona o środki

  - Licznik nie kwalifikuje się do uzyskania środków w wysokości dla **partnerów zarządzanych** przez 7/4-7/7 (Zwróć uwagę na to, że obowiązująca cena jednostkowa to cena detaliczna).

  - Zliczanie środków zakwalifikowanych dla **partnerów w przypadku usług zarządzanych** przez 7/8-7/31 (Zwróć uwagę na to, że obowiązująca cena jednostkowa to cena detaliczna pomniejszona o środki na partnerów

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Faktura w walucie klienta

Opłaty za usługi platformy Azure za pomocą planu platformy Azure są naliczane w USD i rozliczone w walucie klienta przypisanej do kraju. Jeśli waluta rozliczeń jest niezerowa, na ostatniej stronie faktury zostanie wyświetlona stawka obcej wymiany (FX). Stawki FX są określane co miesiąc i stosowane do poniższej faktury. Aby zapoznać się z pełną listą walut krajów, zapoznaj się z tematem [dostępność nowych ofert handlowych i macierzami walutowymi klientów](https://go.microsoft.com/fwlink/?linkid=2112354).

Firma Microsoft postępuje zgodnie z wymianą giełdową na potrzeby konwersji. Korzystamy z kursu wymiany, który jest równy kursowi wymiany przechwyconemu w ostatnim dniu ostatniego miesiąca roboczego w wymianie giełdowej w Londynie. Stawki FX będą odświeżane i dostępne w dniu przed pierwszym miesiącem, dla którego mają zastosowanie.

## <a name="azure-reservations"></a>Rezerwacje platformy Azure


W przypadku kupowania [rezerwacji platformy Azure](azure-reservations.md) za pomocą planu platformy Azure można wybrać jednorazowe lub comiesięczne rozliczanie.


## <a name="azure-spending"></a>Wydatki na platformie Azure

Istniejące środowisko wydatków platformy Azure zostanie zaktualizowane, aby obsługiwało nowe rozliczenia planu platformy Azure w centrum partnerskim. Dzięki temu partnerzy mogą:

- Wyświetlanie i odbieranie alertów dotyczących zestawu budżetu na poziomie klienta oraz zarządzanie nimi 

- Wyświetl łączne szacowane wydatki w planie platformy Azure (podzielone według zasobów i poziomów licznika)

Ze względu na to, że model rozliczeń dla usług platformy Azure w ramach planu platformy Azure jest zużyciem po płatności, aby uniknąć wyższego rachunku niż przewidywane, partnerzy mogą stosować miesięczny budżet i śledzić procent użycia. Budżet można zastosować jednocześnie do jednego klienta lub wielu klientów. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Wydatki na platformie Azure":::

## <a name="next-steps"></a>Następne kroki

- Zobacz, w jaki sposób jest naliczany kredyt uzyskany przez partnera (PEC). Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego i Znajdź dostępną listę cenową.

- Dowiedz się więcej o [kupowaniu planu platformy Azure](purchase-azure-plan.md)

- Zobacz cennik [dla nowego środowiska handlowego w programie CSP](azure-plan-price-list.md)
