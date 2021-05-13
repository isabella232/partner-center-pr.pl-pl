---
title: Typy opłat za pliki uzgodnień
ms.topic: article
ms.date: 06/05/2020
description: Zapoznaj się z typami opłat (na przykład opartymi na licencjach, opartymi na użyciu i jednym czasem), kredytami i rabatami w Partner Center uzgadniania.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855883"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Opis różnych typów opłat w plikach Partner Center uzgodnień

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator | Administrator rozliczeń | Administrator globalny

W tym artykule opisano mapowania między sekcją faktury i skojarzonymi typami opłat, które mogą być w pliku uzgodnień. Faktura zawiera podsumowanie opłat. Plik uzgodnień zawiera szczegółowy podział transakcji elementów wiersza, w tym typy opłat. Aby uzyskać więcej informacji na temat plików uzgodnień, zobacz [jak używać plików uzgodnień](use-the-reconciliation-files.md).

Zarówno [pliki uzgodnień oparte na](usage-based-recon-files.md) użyciu, jak i pliki uzgodnień oparte na licencjach pokazują tylko transakcje i opłaty związane z użyciem (zużyte jednostki i powiązane opłaty). [](license-based-recon-files.md)

> [!NOTE]
> Środki, rabaty lub zwroty, które są  wyświetlane na fakturze jako Korekty, nie są wyświetlane w pliku uzgodnień.

## <a name="map-charge-types-to-invoice-charges"></a>Mapowanie typów opłat na opłaty na podstawie faktur

Aby odwoływać się do kwot opłat między fakturą i plikiem uzgodnień, użyj opcji filtrowania w programie Microsoft Excel. Filtruj według typów opłat w pliku uzgodnień, aby zamapować opłaty na zestaw podziałów opłat w pliku uzgodnień.

## <a name="license-based-charges"></a>Opłaty na podstawie licencji

Aby zamapować te opłaty na podstawie licencji na fakturę, zsuń **kolumnę Amount** (Kwota) z pliku opartego na licencjach.

| Opis opłaty (kolumna ChargeType w pliku uzgodnień) | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Opłata za aktywację | Kwota naliczana klientowi podczas korzystania z subskrypcji po zakupie. |
| Anulowanie opłaty | Naliczane proporcjonalnie opłaty są zwracane klientowi po zmianie skojarzonych licencji. |
| Anulowanie prorate wystąpienia | Opłaty proporcjonalnie anulowane, gdy klient z subskrypcją miesięczną ma wstrzymaną subskrypcję i skojarzone licencje zmieniły się w ciągu tego samego miesiąca. |
| Opłata za cykl | Okresowe opłaty za subskrypcję. |
| Cykl prorate wystąpienia | Naliczane proporcjonalnie opłaty naliczane od klienta w przypadku zmiany skojarzonych licencji. |
| Naliczanie opłat po anulowaniu | Proporcjonalny zwrot za nieużywaną część usługi po anulowaniu. |
| Naliczanie opłat w przypadku konwersji poza bieżącą ofertę | Opłaty naliczane proporcjonalnie po konwersji z bieżącej miesięcznej subskrypcji na roczną subskrypcję. |
| Naliczanie opłat w przypadku konwersji na nową ofertę | Opłaty naliczane proporcjonalnie po przekonwertowaniu miesięcznej subskrypcji na nową roczną subskrypcję. |
| Naliczanie opłat podczas zakupu | Typ opłaty za subskrypcję w przypadku korzystania z rozliczeń miesięcznych lub rocznych. |
| Opłata prorate podczas odnawiania | Opłaty proporcjonalnie po odnowieniu subskrypcji. |
| Odnawianie opłaty | Opłata za odnowienie subskrypcji |
| Naliczanie opłat po aktywowaniu | Opłaty naliczane proporcjonalnie od aktywacji do końca okresu rozliczeniowego. |

## <a name="one-time-charges"></a>Opłaty terminowe

Aby zamapować te opłaty raz na fakturę, zsuń **kolumnę Amount** (Kwota) z pliku opartego na licencjach.

| Opis opłaty (kolumna ChargeType w pliku uzgodnień) | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Nowy | Używany podczas tworzenia nowego zakupu. |
| addQuantity | Używane zarówno w przypadku zwrotu pierwotnego zakupu, jak i nowej ilości po zwiększeniu. |
| removeQuantity | Używane zarówno w przypadku zwrotu pierwotnego zakupu, jak i nowej ilości po zmniejszeniu. |
| Anuluj | Używane po anulowaniu subskrypcji. |
| Convert | Używany podczas uaktualnienia licencji, ale liczba licencji pozostaje niezmieniona. |

## <a name="usage-charges"></a>Opłaty za zużycie

Aby zamapować te opłaty za użycie na fakturę, zsuń kolumnę **PretaxCharges** z pliku opartego na użyciu.

| Opis opłaty (kolumna ChargeType w pliku uzgodnień) | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Ocenianie opłaty za użycie po anulowaniu | Uzyskaj dostęp do opłaty za użycie po anulowaniu za niezapłacone użycie w bieżącym okresie rozliczeniowym. |
| Ocena opłaty za użycie dla bieżącego cyklu | Dostęp do opłaty za użycie w bieżącym okresie rozliczeniowym. |

### <a name="credits"></a>Środki

Aby zamapować te środki na fakturę:

- **Zsumuj wartość TotalForCustomer** z pliku opartego na licencji.
- Zsuń kolumnę **PostTaxTotal** z pliku opartego na użyciu.

| Opis opłaty (kolumna ChargeType w pliku uzgodnień) | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Przesunięcie elementu wiersza | Częściowy lub cały zwrot do pozycji, w tym podatki. |

### <a name="usage-based-discounts"></a>Rabaty oparte na użyciu

Aby zamapować te rabaty na podstawie użycia na fakturę, zsuń kolumnę **PretaxCharges** z pliku opartego na użyciu.

| Opis opłaty (kolumna ChargeType w pliku uzgodnień) | Wyjaśnienie opłaty |
| ------------------------------------------------------------- | ------------------ |
| Rabat na aktywację | Rabat stosowany po aktywowaniu subskrypcji. |
| Rabat na cykl | Rabat stosowany do okresowych opłat. |
| Odnawianie rabatu | Rabat stosowany po odnowieniu subskrypcji. |
| Anulowanie rabatu | Opłaty stosowane w przypadku anulowania rabatów. |

### <a name="license-based-discounts"></a>Rabaty oparte na licencjach

Aby zamapować rabaty na podstawie licencji na fakturę, zsumuj kolumnę **TotalOtherDiscount** z pliku opartego na licencjach.

*Rabaty oparte na licencjach mogą być stosowane do wielu typów opłat.*
