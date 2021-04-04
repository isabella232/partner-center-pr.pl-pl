---
title: Opis faktur rozliczania Centrum partnerskiego
ms.topic: article
ms.date: 05/18/2020
description: Poznaj pola w pliku faktury dotyczące rozliczeń Centrum partnerskiego. Uwzględniono pola i definicje dla wszystkich pól faktury i pól o jednorazowej opłacie.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44bda5256b14722f143a5bf937e73b2533b8c9f5
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178905"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Informacje o rozliczeniach pól faktury Centrum partnerskiego

**Odpowiednie role**

- Administrator globalny
- Administrator zarządzania użytkownikami
- Administrator rozliczeń
- Agent pomocy technicznej

Poniższe tabele służą do zrozumienia pól w plikach faktury Centrum partnerskiego.

## <a name="invoice-file-fields"></a>Pola pliku faktury

Następujące pola są wyświetlane w plikach faktury.

| Pole | Definicja |
| ----- | ---------- |
| US FEIN | Numer identyfikacyjny federalnego pracodawcy (FEIN). Jest to Stany Zjednoczone numer NIP. |
| Numer klienta | Twój numer klienta. |
| Rachunek dla | Adres, na który wysyłamy fakturę. Nazwę firmy i adres można zmienić w profilu rozliczania Centrum partnerskiego. |
| Opłaty oparte na licencji | Miesięczne lub roczne opłaty za zakupione licencje oparte na użyciu są naliczane z góry usługi. Ta liczba jest sumą wszystkich opłat w kolumnie **sum częściowych** (kolumna **T**) w pliku uzgadniania na podstawie licencji. |
| Opłaty oparte na użyciu | Twoje użycie platformy Azure. Obejmuje to nowe usługi lub aplikacje włączone i używane w okresie rozliczeniowym. Ta liczba jest sumą wszystkich opłat w kolumnie **PretaxCharges** (kolumna **Z**) w pliku uzgadniania opartym na użyciu. |
| Rabaty | Rabat otrzymany od normalnego kosztu subskrypcji przez klienta. Ta liczba jest pokazywana jako stała *Kwota*, a nie cena jednostkowa lub licencja. |
| Środki | Kredyty lub korekty dotyczące zmian wprowadzonych w subskrypcjach (na przykład zwiększenie lub zmniejszenie licencji). |
| Suma częściowa | Suma przed podatkami i opłatami wyłącznymi i kredytami. |
| Podatek | Łączny podatek dla bieżących opłat zgodnie z podsumowaniem w sekcji **szczegółów** , zaczynając od strony 2 faktury. Ta liczba jest sumą wszystkich opłat w kolumnie **TaxAmount** (kolumna **AA**) w pliku uzgadniania opartym na użyciu i kolumnie **podatek** (kolumna **U**) w pliku uzgadniania opartego na licencji. |
| Inne środki | Kredyty z wyłączeniem podatku. |
| Łączna liczba bieżących opłat | Kwota należna w walucie rozliczeniowej dla okresu rozliczeniowego. Opłaty są naliczane z powodu terminu płatności. |
| Instrukcje dokonywania płatności | Opis sposobu płacenia faktury w zależności od regionu. *Zawsze pamiętaj o uwzględnieniu numeru faktury podczas dokonywania płatności.* |
| Nr faktury | Numer faktury. |
| Okres rozliczeniowy | Miesięczny okres wiodący na datę faktury. Jest to okres, w którym korzysta się z usług opartych na użyciu, a usługi oparte na licencji są uzgadniane w celu dokonania korekt lub zmian w liczbie licencji. |
| Data faktury | Data rozliczenia lub Data rocznicy, w której faktura jest generowana co miesiąc. |
| Warunki płatności | Termin płatności. Dla jednorazowych zakupów będzie to zawsze 60 dni. |
| Termin płatności | Data, o którą należy otrzymać płatność. |
| Klient PO | Zamówienie numeru zakupu. |
| Obsługa klienta | Adres witryny sieci Web, na której można uzyskać dostęp do usługi klienta. |
| Odbiorca usługi | Adres, w którym usługa jest używana. (Jest to prawny adres firmy skojarzony z przed sprawdzeniem firmy). |

## <a name="one-time-charges-fields"></a>Pola opłat jednorazowych

Następujące pola mają zastosowanie tylko do **opłat jednorazowych** w centrum partnerskim:

| Pole | Definicja |
| ----- | ---------- |
| Data | Data zakupu. |
| Opis | Nazwa produktu. |
| Liczba | Liczba zakupionych produktów (takich jak rezerwacje). |
| Cena jednostkowa | Cena za produkt (na przykład rezerwacja). |
| Rabaty | Wszelkie stosowne rabaty. |
| Kwota przed opodatkowaniem | Suma częściowa zakupów przed opodatkowaniem. |
| Podatek od sprzedaży | Kwota podatku. |
| Łącznie | Łączna kwota do zapłacenia. |
