---
title: Informacje Partner Center faktur rozliczeniowych
ms.topic: article
ms.date: 05/18/2020
description: Informacje o polach w pliku faktury na Partner Center rozliczeniowego. Uwzględnione są pola i definicje dla wszystkich pól faktur i pól opłat tylko raz.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c741caa6993a5da415d3a94d541bf10c21470889
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840080"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Informacje Partner Center faktur rozliczeniowych

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Administrator rozliczeń | Agent pomocy technicznej

Poniższe tabele zawierają informacje o polach w Partner Center faktur.

## <a name="invoice-file-fields"></a>Pola pliku faktury

W plikach faktur są wyświetlane następujące pola.

| Pole | Definicja |
| ----- | ---------- |
| US FEIN | Numer identyfikacyjny federalnego pracodawcy (FEIN, Federal Employer Identification Number). Jest to Twój Stany Zjednoczone federalnego identyfikatora podatkowego. |
| Numer klienta | Numer klienta. |
| Rachunek dla | Adres, na który wysyłamy fakturę. Nazwę i adres firmy można zmienić w profilu Partner Center rozliczeniowego. |
| Opłaty na podstawie licencji | Płaskie miesięczne lub roczne opłaty za zakupione licencje na podstawie użycia, rozliczane z góry za usługę. Ta liczba jest sumą wszystkich opłat w kolumnie **Suma** częściowa (kolumna **T**) w pliku uzgodnień opartym na licencjach. |
| Opłaty na podstawie użycia | Użycie platformy Azure. Obejmuje to nowe usługi lub aplikacje włączone i używane w okresie rozliczeniowym. Ta liczba jest sumą wszystkich opłat w kolumnie **PretaxCharges** (kolumna **Z**) w pliku uzgodnień opartym na użyciu. |
| Rabaty | Rabat, który klient otrzymuje ze zwykłej ceny subskrypcji. Ta liczba jest wyświetlana jako *kwota płaska,* a nie jako cena za jednostkę lub licencję. |
| Środki | Środki lub korekty dotyczące zmian wprowadzonych w subskrypcjach (na przykład zwiększenie lub zmniejszenie liczby licencji). |
| Suma częściowa | Suma przed podatkami oraz opłaty i środki z tytułu zwolnienia z podatku. |
| Podatek | Łączny podatek dla bieżących opłat, zgodnie z sumą w sekcji **Szczegóły,** począwszy od strony 2 faktury. Ta liczba jest sumą wszystkich opłat w kolumnie **TaxAmount** (kolumna **AA**)  w pliku uzgodnień na podstawie użycia oraz kolumną Tax **(kolumna U)** w pliku uzgodnień opartym na licencjach. |
| Inne środki | Środki z wyłączności podatkowej. |
| Łączne bieżące opłaty | Kwota należna w walucie rozliczeniowej dla okresu rozliczeniowego. Te opłaty są należne w terminie płatności. |
| Instrukcje dokonywania płatności | Opis sposobu płacenia za fakturę w zależności od regionu. *Zawsze pamiętaj, aby podczas dokonywania płatności dołączyć numer faktury.* |
| Faktura nie | Numer faktury. |
| Okres rozliczeniowy | Miesięczny okres przed datą faktury. Jest to okres, w którym są używane usługi oparte na użyciu, a usługi oparte na licencjach są uzgadniane na wszelkie korekty środków lub zmiany liczby licencji. |
| Data faktury | Data rozliczeniowa lub data rocznicy, w której faktura jest generowana w każdym miesiącu. |
| Warunki płatności | Okres płatności. W przypadku zakupów jednego typu zawsze będzie to 60 dni. |
| Termin płatności | Data, do której należy odebrać płatność. |
| Customer PO | Twoje zamówienie numeru zakupu. |
| Obsługa klienta | Adres witryny internetowej, pod którym można uzyskać dostęp do obsługi klienta. |
| Odbiorca usługi | Adres, pod którym jest używana usługa. (Jest to legalny adres firmy skojarzony z vetting firmy). |

## <a name="one-time-charges-fields"></a>Pola opłat tylko raz

Następujące pola dotyczą tylko **opłat tylko raz w Partner Center:**

| Pole | Definicja |
| ----- | ---------- |
| Data | Data zakupu. |
| Opis | Nazwa produktu. |
| Liczba | Liczba zakupionych produktów (takich jak rezerwacje). |
| Cena jednostkowa | Cena za produkt (na przykład rezerwacja). |
| Rabaty | Wszelkie odpowiednie rabaty. |
| Kwota przed opodatkowaniem | Suma częściowa zakupów przed podatkami. |
| Podatku | Kwota podatku. |
| Łącznie | Łączna kwota do zapłaty. |
