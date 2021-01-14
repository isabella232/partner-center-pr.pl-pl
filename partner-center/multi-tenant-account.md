---
title: Dodawanie dodatkowych dzierżawców do konta Centrum partnerskiego
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodawać i konsolidować wiele dzierżawców usługi Azure AD na koncie Centrum partnerskiego oraz zarządzać nimi. Dowiedz się również kilka przyczyn, które warto wykonać.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182441"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Dodawanie wielu dzierżawców i zarządzanie nimi na koncie Centrum partnerskiego


**Odpowiednie role**

- Administrator globalny
- Administrator konta

Ta funkcja pozwala zarządzać wieloma dzierżawami dla firmy i konsolidować je na koncie Centrum partnerskiego. Istnieje wiele powodów, dla których może być konieczne zarządzanie wieloma dzierżawami usługi Azure AD na koncie Centrum partnerskiego. Na przykład:

- Firma może zakupić inną firmę i chce, aby pracownicy w nowej firmie mogli korzystać z Centrum partnerskiego. Jednak dwie firmy powinny pozostać osobne. W takim przypadku należy skojarzyć dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA). To skojarzenie umożliwi użytkownikom w obu firmach działanie w centrum partnerskim.

- Jeśli masz więcej niż jedną dzierżawę do uruchomienia Twojej firmy (np. contoso.com, contoso.uk, contoso.in), możesz użyć wielu dzierżawców, aby powiązać je w ramach tego samego konta komputera.

- Fuzje i przejęcia wymagają pracy z więcej niż jedną dzierżawą (np. Jeśli firma Contoso uzyska Fabrikam, musi być w stanie użyć zarówno Constoso.com, jak i Fabrikam.com odpowiednich dzierżawców).

- Użytkownicy z dowolnego dzierżawy muszą mieć możliwość:
    1.  Centrum partnerskie dostępu do szkoleń, pobierania cyfrowego, skojarzenia MCP
    2.  Do przypisywania ról Centrum partnerskiego, takich jak MPN administrator, zachęty administratora itp.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Dodaj kolejną dzierżawę usługi Azure AD do swojego konta

1. Jako Administrator globalny Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.
1. Na ikonie **ustawień** wybierz pozycję **Ustawienia konta** , a następnie wybierz pozycję **dzierżawy**.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Kojarzenie dzierżawców"::: 

3. Wybierz pozycję **Skojarz inną dzierżawę usługi AD** i wskaż dzierżawcę, którą chcesz skojarzyć.

1. Jako Administrator globalny Zaloguj się do dzierżawy, którą chcesz skojarzyć, i Potwierdź skojarzenie. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Potwierdź kojarzenie dzierżawców"::: 

5. Po potwierdzeniu zostanie wyświetlona informacja o **zestawie** .  Wybierz pozycję **Wróć do zarządzania dzierżawcą** i zobaczysz nowo dodaną dzierżawę na liście. 
 

>[!NOTE]
>Nie można skojarzyć dzierżawy z kontem, jeśli jest ono już skojarzone z innym kontem Centrum partnerskiego.


## <a name="remove-a-tenant-from-your-account"></a>Usuwanie dzierżawy z konta
 
1. Jako Administrator globalny Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.

1. Na ikonie **ustawień** wybierz pozycję **ustawienia konta** — > dzierżawców i kliknij kartę **partner** .
 
3. Kliknij pozycję Usuń dla dzierżawy, którą chcesz **usunąć** skojarzenie.

4. Skojarzenie dzierżawy oznacza, że użytkownicy tej dzierżawy nie będą już mieli dostępu do konta Centrum partnerskiego i mogą mieć wpływ na swoje kompetencje. 

Przycisk **Usuń** jest włączony dla wszystkich skojarzonych dzierżawców, z wyjątkiem głównej dzierżawy i dzierżawy, do której użytkownik jest obecnie zalogowany.

:::image type="content" source="images/disassociate.png" alt-text="dzierżawcy z przyciskiem Usuń":::
 

## <a name="next-steps"></a>Następne kroki

- [Dodaj użytkowników](create-user-accounts-and-set-permissions.md)






