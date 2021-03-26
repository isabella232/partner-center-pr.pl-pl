---
title: Typy opłat za pliki uzgodnień
ms.topic: article
ms.date: 06/05/2020
description: Wykrywaj typy opłat (takie jak oparte na licencji, oparte na użyciu i jednorazowe), kredyty i rabaty w plikach uzgadniania Centrum partnerskiego.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549230"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Informacje o różnych typach opłat w plikach uzgadniania Centrum partnerskiego

**Dotyczy**

- Centrum partnerskie w chmurze firmy Microsoft dla instytucji rządowych

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Administrator globalny

W tym artykule opisano mapowania między sekcją faktury i skojarzonymi typami opłat, które mogą znajdować się w pliku uzgadniania. Faktura zawiera podsumowanie opłat. Plik uzgadniania zawiera szczegółowy podział transakcji elementu wiersza, w tym typów opłat. Aby uzyskać więcej informacji dotyczących plików uzgadniania, zobacz [jak używać plików uzgadniania](use-the-reconciliation-files.md).

W przypadku [plików uzgadniania opartych na użyciu](usage-based-recon-files.md) i [plików uzgadniania opartych na licencji](license-based-recon-files.md) są wyświetlane tylko transakcje związane z użyciem i opłaty (zużyte jednostki i powiązane opłaty).

> [!NOTE]
> Kredyty jednorazowe, zniżki lub zwroty, które są wyświetlane na fakturze, jako **korekty** nie są wyświetlane w pliku uzgadniania.

## <a name="map-charge-types-to-invoice-charges"></a>Mapuj typy opłat na faktury

Aby uzyskać informacje o opłatach za odwołania między fakturą i plikiem uzgadniania, użyj opcji filtru w programie Microsoft Excel. Filtruj według typów opłat w pliku uzgadniania, aby zamapować opłaty za faktury na zestaw podziałów opłat w pliku uzgadniania.

## <a name="license-based-charges"></a>Opłaty oparte na licencji

Aby zmapować opłaty na podstawie licencji na fakturę, należy zsumować **wartość kolumny kwota** z pliku opartego na licencji.

| Opis opłaty (kolumna opłaty) w pliku uzgadniania | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Opłata za aktywację | Kwota naliczana dla klienta w przypadku korzystania z subskrypcji po zakupie. |
| Opłata za anulowanie | Opłata naliczana proporcjonalnie do klienta po zmianie skojarzonych licencji. |
| Anuluj częstotliwość wystąpień | Opłata naliczana proporcjonalnie do liczby dni, gdy klient z subskrypcją miesięczną ma zawieszoną subskrypcję, a skojarzone licencje zmieniają się w tym samym miesiącu. |
| Opłata za cykl | Opłaty okresowe za subskrypcję. |
| Tempo wystąpienia cyklu | Opłata naliczana proporcjonalnie do liczby opłat naliczanych od klienta po zmianie skojarzonych licencji. |
| Oceń opłaty po anulowaniu | Naoprocentowanie proporcjonalnie do nieużywanej części usługi po anulowaniu. |
| Opłata proporcjonalna za konwersję z bieżącej oferty | Naliczanie opłat naliczane po przeprowadzeniu konwersji z bieżącej subskrypcji miesięcznej na roczną subskrypcję. |
| Opłaty naliczane za konwersję na nową ofertę | Opłaty naliczane proporcjonalnie po przeprowadzeniu konwersji miesięcznej subskrypcji na nową roczną subskrypcję. |
| Opłata proporcjonalna przy zakupie | Typ opłaty dla subskrypcji w przypadku comiesięcznego lub rocznego rozliczania. |
| Opłata proporcjonalna przy odnowieniu | Opłata naliczana proporcjonalnie przy odnowieniu subskrypcji. |
| Odnawianie opłaty | Opłata za odnowienie subskrypcji |
| Oceń opłaty przy aktywacji | Opłata naliczana proporcjonalnie od aktywacji do końca okresu rozliczeniowego. |

## <a name="one-time-charges"></a>Opłaty jednorazowe

Aby zmapować te jednorazowe opłaty na fakturę, należy zsumować **wartość kolumny kwota** z pliku opartego na licencji.

| Opis opłaty (kolumna opłaty) w pliku uzgadniania | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Nowy | Używany podczas tworzenia nowego zakupu. |
| addilooć | Używany w refund oryginalnego zakupu i nowej ilości po zwiększeniu. |
| removeQuantity | Używany w refund oryginalnego zakupu i nowej ilości po zmniejszeniu. |
| Anuluj | Używany, gdy subskrypcja została anulowana. |
| Convert | Używany podczas uaktualniania licencji, ale liczba licencji pozostaje niezmieniona. |

## <a name="usage-charges"></a>Opłaty za zużycie

Aby zmapować te opłaty za korzystanie z faktury, należy zsumować kolumny **PretaxCharges** z pliku opartego na użyciu.

| Opis opłaty (kolumna opłaty) w pliku uzgadniania | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Oceń opłatę za użycie po anulowaniu | Uzyskaj dostęp do opłat za użycie w przypadku anulowania Niepłatnego użycia w bieżącym okresie rozliczeniowym. |
| Ocenianie opłaty za użycie dla bieżącego cyklu | Opłata za użycie w bieżącym okresie rozliczeniowym. |

### <a name="credits"></a>Środki

Aby zamapować te kredyty na fakturę:

- Zasumuj **TotalForCustomer** z pliku opartego na licencji.
- Suma kolumny **PostTaxTotal** z pliku opartego na użyciu.

| Opis opłaty (kolumna opłaty) w pliku uzgadniania | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Przesunięcie elementu wiersza | Częściowe lub całkowite zwrotne do elementu wiersza, w tym podatki. |

### <a name="usage-based-discounts"></a>Rabaty oparte na użyciu

Aby zmapować te rabaty oparte na użyciu na fakturze, należy zsumować kolumny **PretaxCharges** z pliku opartego na użyciu.

| Opis opłaty (kolumna opłaty) w pliku uzgadniania | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Rabat aktywacji | Rabat stosowany po aktywowaniu subskrypcji. |
| Rabat dla cyklu | Rabat stosowany do opłat okresowych. |
| Odnów rabat | Rabat stosowany w przypadku odnowienia subskrypcji. |
| Anuluj rabat | Opłaty są naliczane po anulowaniu rabatów. |

### <a name="license-based-discounts"></a>Rabaty na podstawie licencji

Aby zmapować rabaty na podstawie licencji na fakturę, należy zsumować kolumny **TotalOtherDiscount** z pliku opartego na licencji.

*Rabaty oparte na licencjach mogą być stosowane do wielu typów opłat.*
