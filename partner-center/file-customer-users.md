---
title: Pola dla pliku CSV do importowania wielu użytkowników dla konta klienta
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aby dodać wielu użytkowników do konta klienta, utwórz plik wartości rozdzielanych przecinkami (CSV) z odpowiednimi polami.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150985"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Dodawanie wielu użytkowników do konta klienta przez utworzenie pliku CSV

**Odpowiednie role:** Administrator globalny

Dodaj wielu użytkowników do konta klienta jednocześnie, przesyłając plik danych w formacie pliku wartości rozdzielanych przecinkami (csv) do Partner Center. Możesz pobrać przykładowy plik danych z usługi Partner Center następnie edytować go do własnego użytku lub utworzyć nowy plik danych przy użyciu modelu danych zdefiniowanego poniżej.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Wymagania dotyczące pliku danych

Aby dodać wielu użytkowników do konta klienta przy użyciu procesu przekazywania zbiorczego, należy spełnić następujące wymagania:

- Musisz mieć uprawnienia administratora globalnego do konta klienta;
- Każdy użytkownik musi mieć unikatowy adres e-mail dołączony do domen poczty e-mail klienta;
- Jednocześnie można przekazać maksymalnie 100 rekordów. Jeśli musisz dodać więcej niż 100 użytkowników, utwórz i przekaż dodatkowe pliki danych.
- Wszyscy użytkownicy muszą znajdować się w tej samej lokalizacji **geograficznej.**
- Wprowadź tylko dane opisane poniżej. Extraneous data will cause the upload to fail.

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