---
title: Tworzenie kont użytkowników i przypisywanie ról
description: Każdy pracownik musi mieć przypisaną rolę, aby uzyskać dostęp do Partner Center. Dowiedz się, jak tworzyć konta użytkowników, przypisywać role i ustawiać uprawnienia.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-account
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 7aacaa04beb0aaa80ff40b1ba5bb2bb419c464904379e6737e55b387cce3bf3d
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691093"
---
# <a name="create-user-accounts"></a>Tworzenie kont użytkowników  

**Odpowiednie role:** Administrator konta | Administrator globalny | Administrator zarządzania użytkownikami

Tworzenie kont użytkowników dla pracowników, którzy potrzebują dostępu do Partner Center. Te zadania muszą być wykonywane przez administratora zarządzania użytkownikami, administratora kont lub administratora globalnego. Użytkownik wykonujący te zadania musi również mieć przypisane Azure Active Directory (AAD) administratora użytkowników lub administrator globalny. Aby uzyskać więcej informacji na temat ról usługi AAD, zobacz [Uprawnienia roli administratora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)w u Azure Active Directory .

## <a name="add-a-new-user"></a>Dodawanie nowego użytkownika

1. Na **ikonie Ustawienia** w prawym górnym rogu strony Partner Center wybierz pozycję Ustawienia **konta,** a następnie wybierz **pozycję Zarządzanie użytkownikami.**

2. Wybierz pozycję **Dodaj użytkownika**.

3. Wprowadź pełną nazwę użytkownika i unikatowy adres e-mail.

4. Wybierz typ agenta i/lub typ administratora, który chcesz przypisać do użytkownika. Partner Center jest oparty na rolach, więc można przypisać uprawnienia w celu dostosowania widoku użytkownika w celu wyświetlenia tylko tych funkcji, których użytkownik potrzebuje do wykonywania określonych zadań.  Jeśli użytkownicy chcą mieć przypisanie roli, mogą znaleźć administratorów globalnych, z którym mają się kontaktować, przechodząc do tematu **Zarządzanie** użytkownikami i filtrowanie według administratora globalnego.

5. Wybierz pozycję **Dodaj**, aby utworzyć konto użytkownika. Potwierdź szczegóły użytkownika na następnej stronie.

> [!IMPORTANT]  
> Zanotuj informacje logowania nowego użytkownika wyświetlane na tej stronie. Pamiętaj, aby skopiować te informacje i wysłać je do nowego użytkownika, ponieważ nie będzie można później uzyskać do nich dostępu ponownie. 

Użytkownik musi zalogować się do aplikacji przy użyciu Partner Center użytkownika i hasła tymczasowego. Gdy użytkownik po raz pierwszy Partner Center do aplikacji, zostanie wyświetlony monit o zmianę hasła.

## <a name="assign-user-roles"></a>Przypisywanie ról użytkowników

Aby pracować w Partner Center, musisz mieć przypisaną rolę.  Obecnie role obejmują Azure Active Directory dzierżawy, Dostawca rozwiązań w chmurze (CSP) i role firmy spoza usługi AAD. Każda firma może potrzebować wszystkich tych ról.

>[!Important]
>Aby uzyskać dostęp do aplikacji, należy znajdować się na liście Partner Center. Przypisania ról zapewniają dodatkowy dostęp.

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień użytkowników pracownikom, którzy muszą pracować w Partner Center](permissions-overview.md)
