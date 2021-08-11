---
title: Pola dla .csv do importowania wielu użytkowników dla konta klienta
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Aby dodać wielu użytkowników do konta klienta, utwórz plik wartości rozdzielanych przecinkami (.csv) z odpowiednimi polami.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4774b0056ff650c64fc8a2f0bbdaa6b888151aacb3418823cd15cdbe4110bd3e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115687795"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Dodawanie wielu użytkowników do konta klienta przez utworzenie .csv klienta

**Odpowiednie role:** Administrator globalny

Dodaj jednocześnie wielu użytkowników do konta klienta, przesyłając plik danych w formacie pliku wartości rozdzielanych przecinkami (.csv) do Partner Center. Możesz pobrać przykładowy plik danych z Partner Center a następnie edytować go do własnego użytku lub utworzyć nowy plik danych przy użyciu modelu danych zdefiniowanego poniżej.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Wymagania dotyczące pliku danych

Aby dodać wielu użytkowników do konta klienta przy użyciu procesu przekazywania zbiorczego, należy spełnić następujące wymagania:

- Musisz mieć uprawnienia administratora globalnego do konta klienta;
- Każdy użytkownik musi mieć unikatowy adres e-mail dołączony do domen poczty e-mail klienta.
- Jednocześnie można przekazać maksymalnie 100 rekordów. Jeśli musisz dodać więcej niż 100 użytkowników, utwórz i przekaż dodatkowe pliki danych.
- Wszyscy użytkownicy muszą znajdować się w tej samej lokalizacji **geograficznej.**
- Wprowadź tylko dane opisane poniżej. Dane ekstraneiczne spowodą niepowodzenie przekazywania.

Wprowadź następujące dane w pliku danych:

| **Nazwa kolumny** | **Opis**  | **Ograniczenie**  |
|:-------- |:------  |:----- |
| Imię  | Imię użytkownika (pole opcjonalne)  | Limit 50 znaków  |
| Nazwisko  | Nazwisko użytkownika (pole opcjonalne)  | Limit 50 znaków  |
| Nazwa wyświetlana    | Nazwa wyświetlana w Partner Center (pole wymagane)                            | Limit 50 znaków                         |
| E-mail   | Służbowy adres e-mail użytkownika w firmie klienta (pole wymagane)           | Każdy użytkownik musi mieć unikatowy adres e-mail |
| Aktualizacja stanu   | Służy do wskazywania, czy nowy rekord użytkownika został pomyślnie utworzony | \*\*Pozostaw puste\*\*                        |

## <a name="next-steps"></a>Następne kroki

- [Jak dodać wielu użytkowników dla klienta](adding-multiple-users-to-a-customer-account.md)