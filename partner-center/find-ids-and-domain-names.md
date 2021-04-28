---
title: Znajdowanie identyfikatora dzierżawy, nazwy domeny, identyfikatora obiektu użytkownika
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak znaleźć identyfikatory w Azure Portal — identyfikator dzierżawy usługi Azure AD organizacji, nazwę domeny lub identyfikator konkretnego obiektu użytkownika. Niektóre zadania wymagają tych informacji.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172255"
---
# <a name="locate-important-ids-for-a-user"></a>Lokalizowanie ważnych identyfikatorów dla użytkownika

**Odpowiednie role**

- Administrator globalny

W tym artykule opisano, jak [za pomocą Azure Portal](https://portal.azure.com/) zlokalizować następujące informacje dla użytkownika:

- Identyfikator Microsoft Azure Active Directory (Azure AD) organizacji lub firmy użytkownika

- Podstawowa nazwa domeny organizacji lub firmy skojarzonej z dzierżawą usługi Azure AD

- Identyfikator obiektu użytkownika

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Znajdowanie identyfikatora Microsoft Azure AD dzierżawy i nazwy domeny podstawowej

Wykonaj następujące kroki, aby zlokalizować identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej w Azure Portal. (Jeśli chcesz znaleźć identyfikator dzierżawy programowo, zobacz Znajdowanie identyfikatora dzierżawy za pomocą programu [PowerShell lub interfejsu wiersza polecenia).](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)

> [!NOTE]
> Identyfikator dzierżawy może być nazywany różnymi nazwami w różnych aplikacjach lub zasobach. Na przykład identyfikator dzierżawy może być określany jako identyfikator katalogu, dzierżawa usługi Azure Active Directory (Azure AD), identyfikator firmy Microsoft lub w przypadku niektórych raportów, nawet identyfikator *tenantguid*.

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).

2. Wybierz **Azure Active Directory** z menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Pokazuje Azure Portal wybranie Azure Active Directory z menu.":::

3. Zostanie Azure Active Directory **strona** Przegląd. Aby znaleźć identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej, odszukaj pole **Identyfikator dzierżawy** i pole **Domena podstawowa.** Te pola są wyświetlane w sekcji Informacje o dzierżawie.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Przedstawia stronę Przegląd z dwoma wyróżnione polami: identyfikatorem dzierżawy i nazwą domeny podstawowej.":::

4. Identyfikator dzierżawy można znaleźć w Azure Portal na kilka innych sposobów. Wybierz **Azure Active Directory** z menu. Następnie znajdź **sekcję Zarządzanie** w menu i wybierz pozycję **Właściwości.**

   Na stronie Właściwości jest również wyświetlany identyfikator dzierżawy skojarzony z użytkownikiem.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Wyświetla stronę Właściwości z wyróżnione polem Identyfikator dzierżawy.":::

## <a name="find-the-user-object-id"></a>Znajdowanie identyfikatora obiektu użytkownika

Samo znalezienie nazwy domeny i identyfikatora dzierżawy może nie być wystarczające. Może być również konieczne zlokalizowanie określonego identyfikatora obiektu przypisanego do użytkownika. Wykonaj następujące kroki, aby znaleźć identyfikator obiektu użytkownika w Azure Portal:

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).

2. Wybierz **Azure Active Directory** z menu.

3. Znajdź **sekcję Zarządzanie** w menu, a następnie wybierz pozycję **Użytkownicy.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Wyświetla Azure Active Directory menu z wyróżnione, opcja Użytkownicy.":::

4. Na stronie Użytkownicy wpisz nazwę użytkownika w polu wyszukiwania.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Wyświetla stronę Użytkownicy z polem wyszukiwania w celu wyszukania określonego użytkownika.":::

5. Wybierz nazwę użytkownika wyświetlaną na liście.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Wyświetla stronę użytkownik wyświetlający wiersz dla wyszukiwanych użytkowników.":::

6. Znajdź sekcję Tożsamość na stronie profilu użytkownika. W tym miejscu zostanie wyświetlone pole Identyfikator obiektu z unikatowym identyfikatorem obiektu użytkownika.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Przedstawia stronę Profilu użytkownika z sekcją Tożsamość i jednym wyróżnione polem identyfikatora obiektu.":::

## <a name="next-steps"></a>Następne kroki

- [Programowe znajdowanie identyfikatora dzierżawy przy użyciu programu PowerShell lub interfejsu wiersza polecenia](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Dowiedz się więcej o profilach użytkowników w Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Dowiedz się, jak partnerzy mogą zobaczyć lub wyeksportować szczegóły klientów w Partner Center](see-your-customer-list.md)

