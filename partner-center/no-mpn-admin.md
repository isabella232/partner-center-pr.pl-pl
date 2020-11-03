---
title: Co należy zrobić, jeśli tylko administrator programu MPN opuścił firmę?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, co należy zrobić, aby znaleźć nowego administratora MPN lub uzyskać pomoc od administratora globalnego firmy. Dowiedz się również, jak dodać nowego administratora globalnego Centrum partnerskiego.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03cd603cf65b1e999cf95fd10d76e6ccc6c403e8
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529810"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Co należy zrobić, jeśli tylko administrator programu MPN opuścił firmę?

**Dotyczy**

- Centrum partnerskie

W poniższym artykule przedstawiono trzy typowe scenariusze dotyczące tego, co należy zrobić, jeśli administrator MPN opuścił firmę.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenariusz 1: administrator partnera MPN/administrator konta opuścił firmę, ale nadal istnieją Administratorzy globalni w ramach konta

W takim przypadku inną osobą w firmie może być przypisana rola administratora partnera MPN. Aby przypisać rolę określonej roli administratora partnera MPN/administratora konta:

1. Zaloguj się do konta Centrum partnerskiego przy użyciu swojego konta służbowego (np. tom@contoso.com ).
1. Na stronie **Zarządzanie użytkownikami** filtru na administratorze globalnym, aby zobaczyć, kto ma Administratorzy globalni firmy. 
1. Skontaktuj się z jedną z administratorów globalnych i poproś o przypisanie Ci wymaganej roli MPN. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenariusz 2: administrator partnera MPN/administrator konta opuścił firmę, a na koncie nie ma administratorów globalnych 

Jeśli przejdziesz do strony **zarządzania użytkownikami** i odfiltrusz administratora globalnego, ale okażesz, że w firmie nie ma administratora globalnego, który może pomóc Ci uzyskać rolę MPN, wykonaj następujące kroki:

1. Przejdź do [Portal.Azure.com](https://ms.portal.azure.com/), zaloguj się przy użyciu konta służbowego (na przykład tom@contoso.com ). 
1. Wybierz opcję **Pomoc i obsługa techniczna** na pasku nawigacyjnym po lewej stronie.
1. Na następnej stronie wybierz pozycję **nowy support Request** i typ **problemu technicznego** w menu rozwijanym, Wstaw dodatkowe szczegóły i kliknij przycisk **Dalej: rozwiązania.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Znajdź administratora w Azure Portal":::

4. Po przejrzeniu zalecanych rozwiązań na następnej stronie wybierz pozycję **Dalej: szczegóły** i Wypełnij wymagane pola.
1. Przejrzyj i Utwórz żądanie pomocy technicznej.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenariusz 3: administrator partnera MPN/administrator konta/Administrator globalny opuścił firmę i nie ma innych użytkowników, którzy mają dostęp do usługi Azure AD firmy. Jest to pełna utrata dostępu.

Postępuj zgodnie z procedurą [przejęcia przez administratora](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) , aby przejąć niezarządzany katalog jako administrator Azure Active Directory.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nie masz pewności, czy Twoja firma ma już konto służbowe?

Jeśli nie masz pewności, czy firma ma konto służbowe, wykonaj następujące kroki, aby je sprawdzić.

1. Zaloguj się do [portalu administracyjnego platformy Azure](https://ms.portal.azure.com).
2. Wybierz **Azure Active Directory** z menu po lewej stronie, a następnie wybierz pozycję **nazwy domen**.
Jeśli masz już konto służbowe, nazwa domeny zostanie wyświetlona.

>[!Note]
>Jeśli masz aktywną subskrypcję do Microsoft Azure lub pakietu Office 365, masz już konto służbowe, a poświadczenia logowania powinny być takie same jak te, które są używane do uzyskiwania dostępu do tych usług.