---
title: Tworzenie kont użytkowników i przypisywanie ról
description: Każdy pracownik musi mieć przypisaną rolę, aby mógł uzyskać dostęp do Centrum partnerskiego. Dowiedz się, jak tworzyć konta użytkowników, przypisywać role i ustawiać uprawnienia.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530249"
---
# <a name="create-user-accounts"></a>Tworzenie kont użytkowników  

**Odpowiednie role**

- Administrator konta
- Administrator globalny
- Administrator zarządzania użytkownikami

Utwórz konta użytkowników dla pracowników, którzy potrzebują dostępu do Centrum partnerskiego. Te zadania muszą zostać wykonane przez administratora zarządzania użytkownikami, administratora kont lub administratora globalnego. Użytkownik wykonujący te zadania musi mieć również przypisane role Azure Active Directory (AAD) administratora lub administratora globalnego. Aby uzyskać więcej informacji na temat ról usługi AAD, zobacz [uprawnienia roli administrator w Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Dodawanie nowego użytkownika

1. Na ikonie **ustawień** w prawym górnym rogu Centrum partnerskiego wybierz pozycję **Ustawienia konta** , a następnie wybierz pozycję **Zarządzanie użytkownikami** .

2. Wybierz pozycję **Dodaj użytkownika** .

3. Wprowadź pełną nazwę i unikatowy adres e-mail użytkownika.

4. Wybierz typ agenta i/lub typ administratora, który ma zostać przypisany do użytkownika. Dostęp do Centrum partnerskiego jest oparty na rolach, dzięki czemu można przypisywać uprawnienia do dostosowywania widoku użytkownika w celu wyświetlenia tylko tych funkcji, których użytkownik potrzebuje do wykonania określonych zadań.  Jeśli użytkownik chce przypisywać rolę, może znaleźć administratorów globalnych, aby skontaktować się z **zarządzaniem użytkownikami** i filtrowaniem w Administrator globalny.

5. Wybierz pozycję **Dodaj** , aby utworzyć konto użytkownika. Potwierdź szczegóły użytkownika na następnej stronie.

> [!IMPORTANT]  
> Zanotuj informacje logowania nowego użytkownika wyświetlane na tej stronie. Pamiętaj o skopiowaniu i wysłaniu tych informacji do nowego użytkownika, ponieważ nie będzie można uzyskać do niego dostępu później. 

Użytkownik będzie musiał zalogować się do Centrum partnerskiego przy użyciu nazwy użytkownika i hasła tymczasowego. Gdy użytkownik loguje się do Centrum partnerskiego po raz pierwszy, zostanie wyświetlony monit o zmianę hasła.

## <a name="assign-user-roles"></a>Przypisywanie ról użytkownika

Aby móc korzystać z Centrum partnerskiego, musisz mieć przypisaną rolę.  Obecnie role Azure Active Directory obejmują role dzierżawy, role dostawcy rozwiązań w chmurze (CSP) i role firmy inne niż AAD. Dla wszystkich tych ról może być wymagana konkretna firma.

>[!Important]
>Aby można było uzyskać dostęp do Centrum partnerskiego, osoby muszą być wymienione w dzierżawie. Przypisania ról zapewniają dodatkowy dostęp.

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień użytkowników potrzebnych pracownikom w centrum partnerskim](permissions-overview.md)
