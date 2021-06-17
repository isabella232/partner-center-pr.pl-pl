---
title: Co zrobić, jeśli jedyny administrator programu MPN opuścił firmę?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, co zrobić, aby znaleźć nowego administratora MPN lub uzyskać pomoc od administratora globalnego firmy. Dowiedz się również, jak dodać nową Partner Center administratora globalnego.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277678"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Co zrobić, jeśli jedyny administrator programu MPN opuścił firmę?

**Odpowiednie role:** Administrator partnera MPN | Konto administratora | Administrator globalny

W poniższym artykule przedstawiono trzy typowe scenariusze dotyczące czynności, które należy wykonać, jeśli administrator MPN opuścił firmę.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenariusz 1. Administrator partnera MPN/administrator konta opuścił firmę, ale na koncie nadal znajdują się administratorzy globalni

W takim przypadku innej osobie w firmie można przypisać rolę administratora partnera MPN. Aby przypisać rolę określonej roli administratora partnera MPN/administratora konta:

1. Zaloguj się do Partner Center konta służbowego (na przykład tom@contoso.com ).
1. Na stronie **Zarządzanie użytkownikami** filtruj pozycję Administrator globalny, aby zobaczyć, kim są administratorzy globalni Twojej firmy. 
1. Skontaktuj się z jednym z administratorów globalnych i poproś go o przypisanie Ci potrzebnej roli specyficznej dla programu MPN. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenariusz 2. Administrator partnera MPN/administrator konta opuścił firmę i na koncie nie ma administratorów globalnych 

Jeśli do strony  Zarządzanie użytkownikami zostanie odfiltrowany filtr Administrator globalny, ale w Twojej firmie nie ma administratora globalnego, który może pomóc Ci w zdobyciu roli specyficznej dla programu MPN, wykonaj następujące kroki:

1. Przejdź do [portal.azure.com](https://ms.portal.azure.com/), zaloguj się przy użyciu konta służbowego (na przykład tom@contoso.com ). 
1. Wybierz opcję **Pomoc i obsługa techniczna** na pasku nav menu po lewej stronie.
1. Na następnej stronie wybierz pozycję Nowy  **Support request** typ problemu technicznego z menu rozwijanego, wstaw wszelkie dodatkowe szczegóły i kliknij pozycję **Dalej: Rozwiązania.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Znajdź administratora w Azure Portal.":::

4. Po przejrzeniu zalecanych rozwiązań na następnej stronie wybierz pozycję **Dalej: Szczegóły** i wypełnij wymagane pola.
1. Przejrzyj i utwórz wniosek o pomoc techniczną.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenariusz 3. Administrator partnera MPN/administrator konta/administrator globalny opuścił firmę i nie ma żadnych innych użytkowników, którzy mogą uzyskać dostęp do usługi Azure AD firmy. Jest to całkowita utrata dostępu.

Postępuj zgodnie [z instrukcjami przejęcia](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) przez administratora, aby przejąć niezaiemowiony katalog jako Azure Active Directory administratora.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nie masz pewności, czy Twoja firma ma już konto służbowe?

Jeśli nie masz pewności, czy firma ma konto służbowe, wykonaj następujące kroki, aby to sprawdzić.

1. Zaloguj się do portalu [administracyjnego platformy Azure.](https://ms.portal.azure.com)
2. Wybierz **Azure Active Directory** menu po lewej stronie, a następnie wybierz **pozycję Nazwy domen**.
Jeśli masz już konto służbowe, nazwa domeny zostanie wymieniona.

>[!Note]
>Jeśli masz aktywną subskrypcję usługi Microsoft Azure lub Office 365, masz już konto służbowe, a poświadczenia logowania powinny być takie same jak te używane do uzyskiwania dostępu do tych usług.