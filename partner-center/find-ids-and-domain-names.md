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
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="f8694-104">Lokalizowanie ważnych identyfikatorów dla użytkownika</span><span class="sxs-lookup"><span data-stu-id="f8694-104">Locate important IDs for a user</span></span>

<span data-ttu-id="f8694-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="f8694-105">**Appropriate roles**</span></span>

- <span data-ttu-id="f8694-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="f8694-106">Global admin</span></span>

<span data-ttu-id="f8694-107">W tym artykule opisano, jak [za pomocą Azure Portal](https://portal.azure.com/) zlokalizować następujące informacje dla użytkownika:</span><span class="sxs-lookup"><span data-stu-id="f8694-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="f8694-108">Identyfikator Microsoft Azure Active Directory (Azure AD) organizacji lub firmy użytkownika</span><span class="sxs-lookup"><span data-stu-id="f8694-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="f8694-109">Podstawowa nazwa domeny organizacji lub firmy skojarzonej z dzierżawą usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="f8694-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="f8694-110">Identyfikator obiektu użytkownika</span><span class="sxs-lookup"><span data-stu-id="f8694-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="f8694-111">Znajdowanie identyfikatora Microsoft Azure AD dzierżawy i nazwy domeny podstawowej</span><span class="sxs-lookup"><span data-stu-id="f8694-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="f8694-112">Wykonaj następujące kroki, aby zlokalizować identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="f8694-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="f8694-113">(Jeśli chcesz znaleźć identyfikator dzierżawy programowo, zobacz Znajdowanie identyfikatora dzierżawy za pomocą programu [PowerShell lub interfejsu wiersza polecenia).](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="f8694-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="f8694-114">Identyfikator dzierżawy może być nazywany różnymi nazwami w różnych aplikacjach lub zasobach.</span><span class="sxs-lookup"><span data-stu-id="f8694-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="f8694-115">Na przykład identyfikator dzierżawy może być określany jako identyfikator katalogu, dzierżawa usługi Azure Active Directory (Azure AD), identyfikator firmy Microsoft lub w przypadku niektórych raportów, nawet identyfikator *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="f8694-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="f8694-116">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f8694-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="f8694-117">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="f8694-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Pokazuje Azure Portal wybranie Azure Active Directory z menu.":::

3. <span data-ttu-id="f8694-119">Zostanie Azure Active Directory **strona** Przegląd.</span><span class="sxs-lookup"><span data-stu-id="f8694-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="f8694-120">Aby znaleźć identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej, odszukaj pole **Identyfikator dzierżawy** i pole **Domena podstawowa.**</span><span class="sxs-lookup"><span data-stu-id="f8694-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="f8694-121">Te pola są wyświetlane w sekcji Informacje o dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="f8694-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Przedstawia stronę Przegląd z dwoma wyróżnione polami: identyfikatorem dzierżawy i nazwą domeny podstawowej.":::

4. <span data-ttu-id="f8694-123">Identyfikator dzierżawy można znaleźć w Azure Portal na kilka innych sposobów.</span><span class="sxs-lookup"><span data-stu-id="f8694-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="f8694-124">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="f8694-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="f8694-125">Następnie znajdź **sekcję Zarządzanie** w menu i wybierz pozycję **Właściwości.**</span><span class="sxs-lookup"><span data-stu-id="f8694-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="f8694-126">Na stronie Właściwości jest również wyświetlany identyfikator dzierżawy skojarzony z użytkownikiem.</span><span class="sxs-lookup"><span data-stu-id="f8694-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Wyświetla stronę Właściwości z wyróżnione polem Identyfikator dzierżawy.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="f8694-128">Znajdowanie identyfikatora obiektu użytkownika</span><span class="sxs-lookup"><span data-stu-id="f8694-128">Find the user object ID</span></span>

<span data-ttu-id="f8694-129">Samo znalezienie nazwy domeny i identyfikatora dzierżawy może nie być wystarczające.</span><span class="sxs-lookup"><span data-stu-id="f8694-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="f8694-130">Może być również konieczne zlokalizowanie określonego identyfikatora obiektu przypisanego do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f8694-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="f8694-131">Wykonaj następujące kroki, aby znaleźć identyfikator obiektu użytkownika w Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="f8694-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="f8694-132">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f8694-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="f8694-133">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="f8694-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="f8694-134">Znajdź **sekcję Zarządzanie** w menu, a następnie wybierz pozycję **Użytkownicy.**</span><span class="sxs-lookup"><span data-stu-id="f8694-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Wyświetla Azure Active Directory menu z wyróżnione, opcja Użytkownicy.":::

4. <span data-ttu-id="f8694-136">Na stronie Użytkownicy wpisz nazwę użytkownika w polu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="f8694-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Wyświetla stronę Użytkownicy z polem wyszukiwania w celu wyszukania określonego użytkownika.":::

5. <span data-ttu-id="f8694-138">Wybierz nazwę użytkownika wyświetlaną na liście.</span><span class="sxs-lookup"><span data-stu-id="f8694-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Wyświetla stronę użytkownik wyświetlający wiersz dla wyszukiwanych użytkowników.":::

6. <span data-ttu-id="f8694-140">Znajdź sekcję Tożsamość na stronie profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f8694-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="f8694-141">W tym miejscu zostanie wyświetlone pole Identyfikator obiektu z unikatowym identyfikatorem obiektu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f8694-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Przedstawia stronę Profilu użytkownika z sekcją Tożsamość i jednym wyróżnione polem identyfikatora obiektu.":::

## <a name="next-steps"></a><span data-ttu-id="f8694-143">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="f8694-143">Next steps</span></span>

- [<span data-ttu-id="f8694-144">Programowe znajdowanie identyfikatora dzierżawy przy użyciu programu PowerShell lub interfejsu wiersza polecenia</span><span class="sxs-lookup"><span data-stu-id="f8694-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="f8694-145">Dowiedz się więcej o profilach użytkowników w Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f8694-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="f8694-146">Dowiedz się, jak partnerzy mogą zobaczyć lub wyeksportować szczegóły klientów w Partner Center</span><span class="sxs-lookup"><span data-stu-id="f8694-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

