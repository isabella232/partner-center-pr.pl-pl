---
title: Znajdź identyfikator dzierżawy, nazwę domeny, identyfikator obiektu użytkownika
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak znaleźć identyfikatory w Azure Portal — identyfikator dzierżawy usługi Azure AD w organizacji, nazwę domeny lub określony identyfikator obiektu użytkownika. Niektóre zadania wymagają tych informacji.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439241"
---
# <a name="locate-important-ids-for-a-user"></a>Lokalizowanie ważnych identyfikatorów dla użytkownika

W tym artykule opisano, jak za pomocą [Azure Portal](https://portal.azure.com/) zlokalizować następujące informacje dla użytkownika:

- Identyfikator dzierżawy usługi Microsoft Azure Active Directory (Azure AD) organizacji lub firmy użytkownika

- Podstawowa nazwa domeny organizacji lub firmy skojarzonej z dzierżawą usługi Azure AD

- Identyfikator obiektu użytkownika

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Znajdź Microsoft Azure AD identyfikator dzierżawy i nazwę domeny podstawowej

Wykonaj następujące kroki, aby zlokalizować identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej w ramach Azure Portal. (Jeśli chcesz programowo znaleźć identyfikator dzierżawy, zobacz [Znajdowanie identyfikatora dzierżawy przy użyciu programu PowerShell lub interfejsu wiersza polecenia](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)).

> [!NOTE]
> Identyfikator dzierżawy może być nazywany różnymi nazwami w różnych aplikacjach lub zasobach. Na przykład identyfikator dzierżawy może być określany jako identyfikator katalogu, dzierżawa usługi Azure Active Directory (Azure AD), identyfikator firmy Microsoft lub dla niektórych raportów, nawet *tenantguid*.

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).

2. Wybierz **Azure Active Directory** z menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Pokazuje Azure Portal wybranie opcji Azure Active Directory z menu.":::

3. Zostanie wyświetlona strona **przeglądu** Azure Active Directory. Aby znaleźć identyfikator dzierżawy usługi Azure AD lub podstawową nazwę domeny, Wyszukaj pole **Identyfikator dzierżawy** i pole **domena podstawowa** . Te pola są wyświetlane w sekcji Informacje o dzierżawie.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Pokazuje stronę przegląd z dwoma wyróżnionymi polami, IDENTYFIKATORem dzierżawy i nazwą domeny podstawowej.":::

4. Identyfikator dzierżawy można znaleźć w Azure Portal na kilka innych sposobów. Wybierz **Azure Active Directory** z menu. Następnie odszukaj sekcję **Zarządzanie** w menu i wybierz pozycję **Właściwości**.

   Na stronie właściwości jest również wyświetlany identyfikator dzierżawy skojarzonej z użytkownikiem.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Pokazuje stronę właściwości z wyróżnionym polem identyfikatora dzierżawy.":::

## <a name="find-the-user-object-id"></a>Znajdowanie identyfikatora obiektu użytkownika

Po prostu znalezienie nazwy domeny i identyfikatora dzierżawy może nie zawsze być wystarczające. Może być również konieczne znalezienie określonego identyfikatora obiektu przypisanego do użytkownika. Wykonaj następujące kroki, aby znaleźć identyfikator obiektu użytkownika w Azure Portal:

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).

2. Wybierz **Azure Active Directory** z menu.

3. Znajdź sekcję **Zarządzanie** w menu, a następnie wybierz pozycję **Użytkownicy**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Pokazuje menu Azure Active Directory z wyróżnionymi opcjami użytkownicy.":::

4. Na stronie użytkownicy wpisz nazwę użytkownika w polu wyszukiwania.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Wyświetla stronę użytkownicy z polem wyszukiwania, aby wyszukać określonego użytkownika.":::

5. Wybierz nazwę użytkownika, która pojawia się na liście.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Pokazuje stronę użytkownika wyświetlającą wiersz dla przeszukanego użytkownika.":::

6. Znajdź sekcję tożsamość na stronie profil użytkownika. Pole Identyfikator obiektu zostanie wyświetlone w tym miejscu z unikatowym IDENTYFIKATORem obiektu użytkownika.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Pokazuje stronę profilu użytkownika z sekcją tożsamość i jedno wyróżnione pole dla identyfikatora obiektu.":::

## <a name="next-steps"></a>Następne kroki

- [Programowe Znajdowanie identyfikatora dzierżawy za pomocą programu PowerShell lub interfejsu wiersza polecenia](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Dowiedz się więcej o profilach użytkowników w Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Dowiedz się, w jaki sposób partnerzy mogą zobaczyć lub wyeksportować szczegóły klienta w centrum partnerskim](see-your-customer-list.md)

