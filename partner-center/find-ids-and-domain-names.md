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
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360075"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="c1fe7-104">Lokalizowanie ważnych identyfikatorów dla użytkownika</span><span class="sxs-lookup"><span data-stu-id="c1fe7-104">Locate important IDs for a user</span></span>

<span data-ttu-id="c1fe7-105">W tym artykule opisano, jak za pomocą [Azure Portal](https://portal.azure.com/) zlokalizować następujące informacje dla użytkownika:</span><span class="sxs-lookup"><span data-stu-id="c1fe7-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="c1fe7-106">Identyfikator dzierżawy usługi Microsoft Azure Active Directory (Azure AD) organizacji lub firmy użytkownika</span><span class="sxs-lookup"><span data-stu-id="c1fe7-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="c1fe7-107">Podstawowa nazwa domeny organizacji lub firmy skojarzonej z dzierżawą usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="c1fe7-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="c1fe7-108">Identyfikator obiektu użytkownika</span><span class="sxs-lookup"><span data-stu-id="c1fe7-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="c1fe7-109">Znajdź Microsoft Azure AD identyfikator dzierżawy i nazwę domeny podstawowej</span><span class="sxs-lookup"><span data-stu-id="c1fe7-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="c1fe7-110">Wykonaj następujące kroki, aby zlokalizować identyfikator dzierżawy usługi Azure AD lub nazwę domeny podstawowej w ramach Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="c1fe7-111">(Jeśli chcesz programowo znaleźć identyfikator dzierżawy, zobacz [Znajdowanie identyfikatora dzierżawy przy użyciu programu PowerShell lub interfejsu wiersza polecenia](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)).</span><span class="sxs-lookup"><span data-stu-id="c1fe7-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="c1fe7-112">Identyfikator dzierżawy może być nazywany różnymi nazwami w różnych aplikacjach lub zasobach.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="c1fe7-113">Na przykład identyfikator dzierżawy może być określany jako identyfikator katalogu, dzierżawa usługi Azure Active Directory (Azure AD), identyfikator firmy Microsoft lub dla niektórych raportów, nawet *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="c1fe7-114">Zaloguj się do [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c1fe7-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="c1fe7-115">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Pokazuje Azure Portal wybranie opcji Azure Active Directory z menu.":::

3. <span data-ttu-id="c1fe7-117">Zostanie wyświetlona strona **przeglądu** Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="c1fe7-118">Aby znaleźć identyfikator dzierżawy usługi Azure AD lub podstawową nazwę domeny, Wyszukaj pole **Identyfikator dzierżawy** i pole **domena podstawowa** .</span><span class="sxs-lookup"><span data-stu-id="c1fe7-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="c1fe7-119">Te pola są wyświetlane w sekcji Informacje o dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Pokazuje stronę przegląd z dwoma wyróżnionymi polami, IDENTYFIKATORem dzierżawy i nazwą domeny podstawowej.":::

4. <span data-ttu-id="c1fe7-121">Identyfikator dzierżawy można znaleźć w Azure Portal na kilka innych sposobów.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="c1fe7-122">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="c1fe7-123">Następnie odszukaj sekcję **Zarządzanie** w menu i wybierz pozycję **Właściwości**.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="c1fe7-124">Na stronie właściwości jest również wyświetlany identyfikator dzierżawy skojarzonej z użytkownikiem.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Pokazuje stronę właściwości z wyróżnionym polem identyfikatora dzierżawy.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="c1fe7-126">Znajdowanie identyfikatora obiektu użytkownika</span><span class="sxs-lookup"><span data-stu-id="c1fe7-126">Find the user object ID</span></span>

<span data-ttu-id="c1fe7-127">Po prostu znalezienie nazwy domeny i identyfikatora dzierżawy może nie zawsze być wystarczające.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="c1fe7-128">Może być również konieczne znalezienie określonego identyfikatora obiektu przypisanego do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="c1fe7-129">Wykonaj następujące kroki, aby znaleźć identyfikator obiektu użytkownika w Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="c1fe7-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="c1fe7-130">Zaloguj się do [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c1fe7-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="c1fe7-131">Wybierz **Azure Active Directory** z menu.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="c1fe7-132">Znajdź sekcję **Zarządzanie** w menu, a następnie wybierz pozycję **Użytkownicy**.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Pokazuje menu Azure Active Directory z wyróżnionymi opcjami użytkownicy.":::

4. <span data-ttu-id="c1fe7-134">Na stronie użytkownicy wpisz nazwę użytkownika w polu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Wyświetla stronę użytkownicy z polem wyszukiwania, aby wyszukać określonego użytkownika.":::

5. <span data-ttu-id="c1fe7-136">Wybierz nazwę użytkownika, która pojawia się na liście.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Pokazuje stronę użytkownika wyświetlającą wiersz dla przeszukanego użytkownika.":::

6. <span data-ttu-id="c1fe7-138">Znajdź sekcję tożsamość na stronie profil użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="c1fe7-139">Pole Identyfikator obiektu zostanie wyświetlone w tym miejscu z unikatowym IDENTYFIKATORem obiektu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c1fe7-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Pokazuje stronę profilu użytkownika z sekcją tożsamość i jedno wyróżnione pole dla identyfikatora obiektu.":::

## <a name="next-steps"></a><span data-ttu-id="c1fe7-141">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="c1fe7-141">Next steps</span></span>

- [<span data-ttu-id="c1fe7-142">Programowe Znajdowanie identyfikatora dzierżawy za pomocą programu PowerShell lub interfejsu wiersza polecenia</span><span class="sxs-lookup"><span data-stu-id="c1fe7-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="c1fe7-143">Dowiedz się więcej o profilach użytkowników w Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c1fe7-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="c1fe7-144">Dowiedz się, w jaki sposób partnerzy mogą zobaczyć lub wyeksportować szczegóły klienta w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="c1fe7-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)
