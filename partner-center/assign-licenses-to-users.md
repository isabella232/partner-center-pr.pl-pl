---
title: Zarządzanie użytkownikami na kontach klientów
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Zarządzanie użytkownikami dla klientów w Partner Center — tworzenie kont użytkowników, dodawanie lub usuwanie licencji użytkowników, resetowanie haseł oraz usuwanie lub przywracanie kont użytkowników.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1c346e5e680fdd0b0b82715160b238e1e6b6a9a9
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959158"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Zarządzanie użytkownikami i licencjami użytkowników dla kont klientów 

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent administracyjny


Możesz tworzyć i usuwać nowych użytkowników na koncie klienta. Możesz również przywrócić co najmniej jedno konto użytkownika, które zostało wcześniej usunięte w ciągu 30 dni od usunięcia. Zostaną również przywrócone poprzednie przypisania subskrypcji użytkownika (przy założeniu, że są dostępne jego poprzednie alokacje).

Gdy kupujesz nowe subskrypcje dla klienta, klient powinien podać listę wszystkich użytkowników, którzy będą potrzebować kont, ich uprawnień użytkowników i usług, których potrzebuje każdy użytkownik.  

>[!NOTE]
>Sekcja **Użytkownicy i** licencje  na karcie Klient zawiera wszystkich użytkowników utworzonych w dzierżawie określonego klienta, w tym użytkowników, którzy mają licencje zakupione od innego partnera CSP lub innego kanału zakupu.

Subskrypcje [można przypisać do](bulk-license-provisioning-for-multiple-users.md) wielu użytkowników jednocześnie, importując nazwy przy użyciu zgodnego Excel pliku .csv arkusza [kalkulacyjnego.](adding-multiple-users-to-a-customer-account.md)

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Tworzenie kont użytkowników dla klienta

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. W menu klienta wybierz pozycję **Użytkownicy i licencje.**

4. Dla każdego użytkownika, który dodajesz, wybierz **pozycję Dodaj subskrypcję,** a następnie wypełnij informacje, w tym uprawnienia i licencje. **Zapisz** zmiany.

5. Pamiętaj, aby zarejestrować nazwę użytkownika i hasło tymczasowe do wysłania do użytkownika.

6. Jeśli dodajesz wielu użytkowników po jednym na raz, użyj **opcji Dodaj innego użytkownika.**

7. Można również dodać wielu użytkowników jednocześnie, importując plik [Excel zgodny z .csv arkusza kalkulacyjnego.](adding-multiple-users-to-a-customer-account.md) Przed wysyłaniem wiadomości e-mail lub drukowaniem nazw i haseł z ekranu potwierdzenia możesz poczekać, aż wszystko będzie gotowe.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Dodawanie lub usuwanie licencji użytkowników dla klienta

Poniższe kroki dotyczą dodawania lub usuwania licencji użytkowników dla produktów firmy Microsoft. Aby dodać lub usunąć licencje użytkowników dla opartych na licencjach subskrypcji SaaS na platformie handlowej, zobacz Dodawanie lub usuwanie licencji dla subskrypcji [SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.

3. W menu klienta wybierz pozycję **Użytkownicy i licencje.**

4. Wybierz co najmniej jednego użytkownika z listy. Jeśli na przykład klient właśnie zakupił nowe licencje i chcesz przypisać je do osób, które ich jeszcze nie mają, możesz użyć opcji Filtruj użytkowników **według...,** aby znaleźć właściwą grupę.

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

3. Wybierz **kartę Usunięci użytkownicy (** ). Powinien być **odczytywany (1)** lub większy w przypadku usunięcia użytkowników, których można przywrócić.

4. Zaznacz co najmniej jedno pole wyboru usuniętych użytkowników, a następnie wybierz pozycję **Przywróć**.

    Wszystkie wybrane konta użytkowników będą ponownie pojawiać się na **stronie Użytkownicy i licencje.**

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie lub odwoływanie licencji dla wielu użytkowników](bulk-license-provisioning-for-multiple-users.md)

- [Tworzenie wielu użytkowników dla konta klienta](adding-multiple-users-to-a-customer-account.md)