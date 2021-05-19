---
title: Tworzenie kont użytkowników i przypisywanie ról
description: Każdy pracownik musi mieć przypisaną rolę, aby uzyskać dostęp do Partner Center. Dowiedz się, jak tworzyć konta użytkowników, przypisywać role i ustawiać uprawnienia.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148146"
---
# <a name="create-user-accounts"></a>Tworzenie kont użytkowników  

**Odpowiednie role:** Administrator konta | Administrator globalny | Administrator zarządzania użytkownikami

Tworzenie kont użytkowników dla pracowników, którzy potrzebują dostępu do Partner Center. Te zadania muszą być wykonywane przez administratora zarządzania użytkownikami, administratora kont lub administratora globalnego. Użytkownik wykonujący te zadania musi również mieć przypisane Azure Active Directory (AAD) administratora użytkowników lub administrator globalny. Aby uzyskać więcej informacji na temat ról usługi AAD, zobacz [Uprawnienia ról administratorów](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)w u Azure Active Directory .

## <a name="add-a-new-user"></a>Dodawanie nowego użytkownika

1. Z **ikony** Ustawienia w prawym górnym rogu ekranu Partner Center **pozycję Ustawienia konta,** a następnie pozycję **Zarządzanie użytkownikami.**

2. Wybierz pozycję **Dodaj użytkownika**.

3. Wprowadź pełną nazwę użytkownika i unikatowy adres e-mail.

4. Wybierz typ agenta i/lub typ administratora, który chcesz przypisać do użytkownika. Partner Center jest oparty na rolach, dlatego można przypisać uprawnienia w celu dostosowania widoku użytkownika w celu wyświetlenia tylko tych funkcji, których użytkownik potrzebuje do wykonania określonych zadań.  Jeśli użytkownicy chcą mieć przypisanie roli, mogą znaleźć administratorów globalnych, z którym mają się kontaktować, przechodząc do tematu **Zarządzanie** użytkownikami i filtrowanie według administratora globalnego.

5. Wybierz pozycję **Dodaj**, aby utworzyć konto użytkownika. Potwierdź szczegóły użytkownika na następnej stronie.

> [!IMPORTANT]  
> Zanotuj informacje logowania nowego użytkownika wyświetlane na tej stronie. Pamiętaj, aby skopiować i wysłać te informacje do nowego użytkownika, ponieważ nie będzie można później uzyskać do nich dostępu ponownie. 

Użytkownik musi zalogować się do aplikacji przy użyciu Partner Center użytkownika i hasła tymczasowego. Gdy użytkownik po raz pierwszy Partner Center do aplikacji, zostanie wyświetlony monit o zmianę hasła.

## <a name="assign-user-roles"></a>Przypisywanie ról użytkowników

Aby pracować w Partner Center, musisz mieć przypisaną rolę.  Obecnie role obejmują Azure Active Directory dzierżawy, Dostawca rozwiązań w chmurze (CSP) i role firmowe spoza usługi AAD. Każda firma może potrzebować wszystkich tych ról.

>[!Important]
>Aby uzyskać dostęp do aplikacji, należy znajdować się na liście Partner Center. Przypisania ról zapewniają dodatkowy dostęp.

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień użytkowników pracownikom, którzy muszą pracować w Partner Center](permissions-overview.md)
