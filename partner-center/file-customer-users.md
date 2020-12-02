---
title: Pola pliku CSV do importowania wielu użytkowników dla konta klienta
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aby dodać wielu użytkowników do konta klienta, Utwórz plik z wartościami rozdzielanymi przecinkami (CSV) z odpowiednimi polami.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/03/2020
ms.locfileid: "92529433"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Dodawanie wielu użytkowników do konta klienta przez utworzenie pliku CSV

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Administrator globalny

Jednocześnie Dodaj wielu użytkowników do konta klienta, przekazując plik danych w formacie pliku wartości rozdzielanych przecinkami (CSV) do Centrum partnerskiego. Możesz pobrać przykładowy plik danych z Centrum partnerskiego, a następnie edytować go w celu użycia lub utworzyć nowy plik danych przy użyciu modelu danych zdefiniowanego poniżej.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Wymagania dotyczące pliku danych

Aby dodać wielu użytkowników do konta klienta przy użyciu procesu przekazywania zbiorczego, należy spełnić następujące wymagania:

- Użytkownik musi mieć uprawnienia administratora globalnego do konta klienta.
- Każdy użytkownik musi mieć unikatowy adres e-mail dołączony do domen poczty e-mail klienta;
- Jednocześnie można przekazać do 100 rekordów. Jeśli musisz dodać więcej niż 100 użytkowników, Utwórz i przekaż dodatkowe pliki danych.
- Wszyscy użytkownicy muszą znajdować się w tej samej **lokalizacji** geograficznej.
- Wprowadź tylko dane opisane poniżej. Dane nadmiarowe spowodują, że przekazywanie zakończy się niepowodzeniem.

Wprowadź następujące dane w pliku danych:

| **Nazwa kolumny** | **Opis**  | **Ograniczenie**  |
|:-------- |:------  |:----- |
| Imię  | Imię użytkownika (pole opcjonalne)  | 50 — limit znaków  |
| Nazwisko  | Nazwisko użytkownika (pole opcjonalne)  | 50 — limit znaków  |
| Nazwa wyświetlana    | Nazwa wyświetlana w centrum partnerskim (pole wymagane)                            | 50 — limit znaków                         |
| E-mail   | Służbowy adres e-mail użytkownika w firmie klienta (wymagane pole)           | Każdy użytkownik musi mieć unikatowy adres e-mail |
| Aktualizacja stanu   | Służy do wskazania, czy nowy rekord użytkownika został pomyślnie utworzony | \*\*Pozostaw puste\*\*                        |

## <a name="next-steps"></a>Następne kroki

- [Jak dodać wielu użytkowników dla klienta](adding-multiple-users-to-a-customer-account.md)