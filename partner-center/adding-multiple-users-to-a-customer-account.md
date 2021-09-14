---
title: Dodawanie wielu użytkowników dla konta klienta
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Aby dodać wielu użytkowników do konta klienta, przekaż plik danych do usługi Partner Center format pliku wartości rozdzielanych przecinkami (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 907d1267164df267acab08675b4b9388fbf14474
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247198"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Upload pliku .csv użytkowników na konto klienta


**Odpowiednie role:** Administrator globalny

Dodaj wielu użytkowników do konta klienta jednocześnie, przesyłając plik danych w formacie pliku wartości rozdzielanych przecinkami (.csv) do Partner Center. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Tworzenie pliku użytkowników klienta i przekazywanie go do konta klienta

1. Utwórz plik danych wartości rozdzielanych przecinkami (.csv) z danymi opisanymi powyżej. Zapisz plik, aby można było przejść do niego w późniejszym kroku. Zobacz [Pola dla .csv, aby zaimportować wielu użytkowników dla konta klienta.](file-customer-users.md) 

2. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

3. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

4. Wybierz kartę Użytkownicy **i** licencje klienta, a następnie wybierz pozycję **Upload użytkowników.**

5. W **Upload informacji o użytkowniku** wybierz pozycję **Przeglądaj.**

6. W selektorze plików wybierz plik danych, a następnie wybierz pozycję **Otwórz**.

7. Wybierz przycisk **Weryfikuj**.

    **Uwaga**  Większość błędów tworzenia konta jest spowodowana przez problemy z plikami danych, w tym brakujące informacje, źle sformułowane lub zduplikowane adresy e-mail albo zbyt wiele rekordów w pliku.

8. Po Partner Center pliku wybierz lokalizację geograficzną **dla** nowych użytkowników.
9. Wybierz pozycję **Zapisz**.
10. Pobierz tymczasowe informacje o hasłach dla użytkowników.

    >[!IMPORTANT]
    > Pamiętaj, aby teraz pobrać plik z hasłami tymczasowymi, ponieważ nie będzie można tego zrobić później. Nowi użytkownicy muszą zalogować się do nowego konta przy użyciu hasła tymczasowego dla nowych kont.

11. Nowym użytkownikom są automatycznie przypisywane uprawnienia z listy **Może korzystać z licencji i usług.** 

## <a name="next-steps"></a>Następne kroki

- [Nadaj klientom uprawnienia Partner Center do kupowania własnych produktów lub usług](give-customers-permission.md)
