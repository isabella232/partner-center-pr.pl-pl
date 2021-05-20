---
title: Zarządzanie użytkownikami dla kont klientów
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zarządzanie użytkownikami dla klientów w Partner Center — tworzenie kont użytkowników, dodawanie lub usuwanie licencji użytkowników, resetowanie haseł oraz usuwanie lub przywracanie kont użytkowników.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149897"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Zarządzanie użytkownikami i licencjami użytkowników dla kont klientów 

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny


Możesz tworzyć i usuwać nowych użytkowników na koncie klienta. Możesz również przywrócić co najmniej jedno konto użytkownika, które zostało wcześniej usunięte w ciągu 30 dni od usunięcia. Zostaną również przywrócone poprzednie przypisania subskrypcji użytkownika (przy założeniu, że są dostępne jego poprzednie alokacje).

Gdy kupujesz nowe subskrypcje dla klienta, klient powinien podać listę wszystkich użytkowników, którzy będą potrzebować kont, ich uprawnień użytkownika i usług, których potrzebuje każdy użytkownik.  

>[!NOTE]
>Sekcja **Użytkownicy i** licencje  na karcie Klient zawiera wszystkich użytkowników utworzonych w dzierżawie określonego klienta, w tym użytkowników, którzy mają licencje zakupione od innego partnera CSP lub z innego kanału zakupów.

Subskrypcje [można przypisywać do wielu użytkowników](bulk-license-provisioning-for-multiple-users.md) jednocześnie, importując nazwy przy użyciu pliku arkusza kalkulacyjnego CSV zgodnego z programem [Excel.](adding-multiple-users-to-a-customer-account.md)

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Tworzenie kont użytkowników dla klienta

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. W menu klienta wybierz pozycję **Użytkownicy i licencje**.

4. Dla każdego dodawania użytkownika wybierz pozycję **Dodaj subskrypcję,** a następnie podaj informacje, w tym uprawnienia i licencje. **Zapisz** zmiany.

5. Pamiętaj, aby zarejestrować nazwę użytkownika i hasło tymczasowe do wysłania do użytkownika.

6. Jeśli dodajesz wielu użytkowników po jednym na raz, użyj **opcji Dodaj innego użytkownika.**

7. Można również dodać wielu użytkowników jednocześnie, importując plik arkusza kalkulacyjnego CSV zgodny z [programem Excel.](adding-multiple-users-to-a-customer-account.md) Możesz poczekać, aż cały zestaw będzie już gotowe, zanim napisze wiadomość e-mail lub będzie drukować nazwy i hasła z ekranu potwierdzenia.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Dodawanie lub usuwanie licencji użytkowników dla klienta

Poniższe kroki dotyczą dodawania lub usuwania licencji użytkowników dla produktów firmy Microsoft. Aby dodać lub usunąć licencje użytkowników dla opartych na licencjach subskrypcji SaaS na platformie handlowej, zobacz Dodawanie lub usuwanie licencji dla subskrypcji [SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. W menu klienta wybierz pozycję **Użytkownicy i licencje.**

4. Wybierz co najmniej jednego użytkownika z listy. Jeśli na przykład klient właśnie zakupił nowe licencje i chcesz przypisać je do osób, które jeszcze ich nie mają, możesz użyć opcji Filtruj użytkowników **według...,** aby znaleźć odpowiednią grupę.

5. Wybierz pozycję **Zarządzaj licencjami**. Dokonaj zmian, a następnie **zapisz .**

> [!NOTE]
> W [Azure Marketplace produktu](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)przypisanie licencji i aktywacja są zarządzane za pośrednictwem niezależnego dostawcy oprogramowania, który opublikował produkt.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Resetowanie hasła użytkownika dla klienta

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard) Centrum partnerskiego.

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. W menu klienta wybierz pozycję **Użytkownicy i licencje.** Wybierz użytkownika z listy.

4. W dolnej części ekranu wybierz pozycję **Resetuj hasło.** 

5. Wyślij nowe hasło tymczasowe do użytkownika.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Usuwanie kont użytkowników dla klienta

1. Z menu **Partner Center** wybierz pozycję **Klienci.** Wybierz klienta z listy.

2. W menu klienta wybierz pozycję **Użytkownicy i licencje.** Wybierz użytkownika z listy.

3. W dolnej części ekranu wybierz pozycję **Usuń konto użytkownika.**

Jeśli musisz przywrócić to konto, możesz  je znaleźć na karcie Usunięci użytkownicy na liście **Użytkownicy i licencje** klienta. Masz 30 dni na przywrócenie usuniętego użytkownika.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Przywracanie usuniętych kont użytkowników

1. Z **Partner Center** wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

2. Wybierz **pozycję Użytkownicy i licencje.**

3. Wybierz **kartę Usunięci użytkownicy (** ). Powinien być **odczytywany (1)** lub większy, gdy istnieją usunięci użytkownicy, którzy mogą zostać przywróconi.

4. Zaznacz co najmniej jedno pole wyboru usuniętego użytkownika, a następnie wybierz pozycję **Przywróć.**

    Wszystkie wybrane konta użytkowników zostaną ponownie pojawiające się na **stronie Użytkownicy i licencje.**

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie lub odwoływanie licencji dla wielu użytkowników](bulk-license-provisioning-for-multiple-users.md)

- [Tworzenie wielu użytkowników dla konta klienta](adding-multiple-users-to-a-customer-account.md)