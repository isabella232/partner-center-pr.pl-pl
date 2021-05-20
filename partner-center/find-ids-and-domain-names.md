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
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150866"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="cf130-104">Lokalizowanie ważnych identyfikatorów dla użytkownika</span><span class="sxs-lookup"><span data-stu-id="cf130-104">Locate important IDs for a user</span></span>

<span data-ttu-id="cf130-105">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="cf130-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="cf130-106">W tym artykule opisano, jak [za pomocą Azure Portal](https://portal.azure.com/) zlokalizować następujące informacje dla użytkownika:</span><span class="sxs-lookup"><span data-stu-id="cf130-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="cf130-107">Identyfikator Microsoft Azure Active Directory (Azure AD) organizacji lub firmy użytkownika</span><span class="sxs-lookup"><span data-stu-id="cf130-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="cf130-108">Podstawowa nazwa domeny organizacji lub firmy skojarzonej z dzierżawą usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="cf130-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="cf130-109">Identyfikator obiektu użytkownika</span><span class="sxs-lookup"><span data-stu-id="cf130-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="cf130-110">Znajdowanie identyfikatora Microsoft Azure AD dzierżawy i nazwy domeny podstawowej</span><span class="sxs-lookup"><span data-stu-id="cf130-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="cf130-111">Wykonaj następujące kroki, aby zlokalizować identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="cf130-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="cf130-112">(Jeśli chcesz znaleźć identyfikator dzierżawy programowo, zobacz Znajdowanie identyfikatora dzierżawy za pomocą programu [PowerShell lub interfejsu wiersza polecenia).](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="cf130-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="cf130-113">Identyfikator dzierżawy może być nazywany różnymi nazwami w różnych aplikacjach lub zasobach.</span><span class="sxs-lookup"><span data-stu-id="cf130-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="cf130-114">Na przykład identyfikator dzierżawy może być określany jako identyfikator katalogu, dzierżawa usługi Azure Active Directory (Azure AD), identyfikator firmy Microsoft lub w przypadku niektórych raportów, nawet identyfikator *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="cf130-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="cf130-115">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cf130-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="cf130-116">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="cf130-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Pokazuje Azure Portal wybranie Azure Active Directory z menu.":::

3. <span data-ttu-id="cf130-118">Zostanie Azure Active Directory **strona** Przegląd.</span><span class="sxs-lookup"><span data-stu-id="cf130-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="cf130-119">Aby znaleźć identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej, odszukaj pole **Identyfikator dzierżawy** i pole **Domena podstawowa.**</span><span class="sxs-lookup"><span data-stu-id="cf130-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="cf130-120">Te pola są wyświetlane w sekcji Informacje o dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="cf130-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Przedstawia stronę Przegląd z dwoma wyróżnione polami: identyfikatorem dzierżawy i nazwą domeny podstawowej.":::

4. <span data-ttu-id="cf130-122">Identyfikator dzierżawy można znaleźć w Azure Portal na kilka innych sposobów.</span><span class="sxs-lookup"><span data-stu-id="cf130-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="cf130-123">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="cf130-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="cf130-124">Następnie znajdź sekcję **Zarządzanie** w menu i wybierz pozycję **Właściwości**.</span><span class="sxs-lookup"><span data-stu-id="cf130-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="cf130-125">Na stronie Właściwości jest również wyświetlany skojarzony z użytkownikiem identyfikator dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="cf130-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Wyświetla stronę Właściwości z wyróżnione polem Identyfikator dzierżawy.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="cf130-127">Znajdowanie identyfikatora obiektu użytkownika</span><span class="sxs-lookup"><span data-stu-id="cf130-127">Find the user object ID</span></span>

<span data-ttu-id="cf130-128">Samo znalezienie nazwy domeny i identyfikatora dzierżawy może nie być wystarczające.</span><span class="sxs-lookup"><span data-stu-id="cf130-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="cf130-129">Może być również konieczne zlokalizowanie określonego identyfikatora obiektu przypisanego do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="cf130-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="cf130-130">Wykonaj następujące kroki, aby znaleźć identyfikator obiektu użytkownika w Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="cf130-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="cf130-131">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cf130-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="cf130-132">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="cf130-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="cf130-133">Znajdź **sekcję Zarządzanie** w menu, a następnie wybierz pozycję **Użytkownicy.**</span><span class="sxs-lookup"><span data-stu-id="cf130-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Wyświetla Azure Active Directory menu z wyróżnione, opcja Użytkownicy.":::

4. <span data-ttu-id="cf130-135">Na stronie Użytkownicy wpisz nazwę użytkownika w polu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="cf130-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Wyświetla stronę Użytkownicy z polem wyszukiwania w celu wyszukania określonego użytkownika.":::

5. <span data-ttu-id="cf130-137">Wybierz nazwę użytkownika wyświetlaną na liście.</span><span class="sxs-lookup"><span data-stu-id="cf130-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Wyświetla stronę użytkownik wyświetlający wiersz dla wyszukiwanych użytkowników.":::

6. <span data-ttu-id="cf130-139">Znajdź sekcję Tożsamość na stronie profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="cf130-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="cf130-140">W tym miejscu zostanie wyświetlone pole Identyfikator obiektu z unikatowym identyfikatorem obiektu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="cf130-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Wyświetla stronę Profil użytkownika z sekcją Tożsamość i jednym wyróżnione polem identyfikatora obiektu.":::

## <a name="next-steps"></a><span data-ttu-id="cf130-142">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cf130-142">Next steps</span></span>

- [<span data-ttu-id="cf130-143">Programowe znajdowanie identyfikatora dzierżawy przy użyciu programu PowerShell lub interfejsu wiersza polecenia</span><span class="sxs-lookup"><span data-stu-id="cf130-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="cf130-144">Dowiedz się więcej o profilach użytkowników w Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cf130-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="cf130-145">Dowiedz się, jak partnerzy mogą zobaczyć lub wyeksportować szczegóły klientów w Partner Center</span><span class="sxs-lookup"><span data-stu-id="cf130-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

