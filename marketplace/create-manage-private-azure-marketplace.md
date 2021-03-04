---
title: Utwórz prywatną witrynę Azure Marketplace i zarządzaj nią w Azure Portal
description: Dowiedz się więcej na temat tworzenia prywatnego portalu Azure Marketplace (wersja zapoznawcza) i zarządzania nim w Azure Portal. Prywatny Portal Azure Marketplace (wersja zapoznawcza) umożliwia administratorom zarządzanie rozwiązaniami innych firm, które mogą być używane przez użytkowników.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101757078"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="6ac20-104">Utwórz prywatną witrynę Azure Marketplace i zarządzaj nią w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="6ac20-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="6ac20-105">Prywatny Portal Azure Marketplace umożliwia administratorom zarządzanie rozwiązaniami innych firm, które mogą być używane przez użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6ac20-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="6ac20-106">Jest to możliwe dzięki umożliwieniu użytkownikowi wdrożenia tylko ofert zatwierdzonych przez administratora i przestrzegania zasad obowiązujących w przedsiębiorstwie.</span><span class="sxs-lookup"><span data-stu-id="6ac20-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="6ac20-107">Korzystając z prywatnego portalu Azure Marketplace, użytkownicy mogą przeszukiwać oferty zgodne ze sklepem online, aby móc kupować i wdrażać.</span><span class="sxs-lookup"><span data-stu-id="6ac20-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="6ac20-108">Jako Administrator portalu Marketplace (przypisana rola) rozpocznie się z wyłączonym i pustym magazynem prywatnym, w którym można dodać zatwierdzone oferty i plany.</span><span class="sxs-lookup"><span data-stu-id="6ac20-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="6ac20-109">W tym artykule wyjaśniono, jak przypisać potrzebną rolę, utworzyć magazyn prywatny, zarządzać elementami, zatwierdzać żądania użytkowników i włączać prywatne witryny Azure Marketplace dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6ac20-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="6ac20-110">Prywatny Portal Azure Marketplace jest na poziomie dzierżawy, dlatego wszyscy użytkownicy w ramach dzierżawy będą widzieć tę samą listę nadzorowana.</span><span class="sxs-lookup"><span data-stu-id="6ac20-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="6ac20-111">Wszystkie rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) są automatycznie dodawane do prywatnego portalu Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="6ac20-112">Przypisywanie roli administratora portalu Marketplace</span><span class="sxs-lookup"><span data-stu-id="6ac20-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="6ac20-113">Administrator globalny dzierżawy musi przypisać rolę **administratora portalu Marketplace** do prywatnego administratora portalu Azure Marketplace, który będzie zarządzać magazynem prywatnym.</span><span class="sxs-lookup"><span data-stu-id="6ac20-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="6ac20-114">Dostęp do prywatnego zarządzania w portalu Azure Marketplace jest dostępny tylko dla administratorów IT z przypisaną rolą administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="6ac20-115">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="6ac20-115">Prerequisites</span></span>

<span data-ttu-id="6ac20-116">Te wymagania wstępne są wymagane przed przypisaniem roli administratora portalu Marketplace do użytkownika w zakresie dzierżawy:</span><span class="sxs-lookup"><span data-stu-id="6ac20-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="6ac20-117">Masz dostęp do użytkownika **administratora globalnego** .</span><span class="sxs-lookup"><span data-stu-id="6ac20-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="6ac20-118">Dzierżawca ma co najmniej jedną subskrypcję (może być dowolnego typu).</span><span class="sxs-lookup"><span data-stu-id="6ac20-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="6ac20-119">Użytkownikowi administratora globalnego przypisano rolę **współautor** lub wyższą dla wybranej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="6ac20-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="6ac20-120">Przypisywanie roli administratora portalu Marketplace przy użyciu kontroli dostępu (IAM)</span><span class="sxs-lookup"><span data-stu-id="6ac20-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="6ac20-121">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6ac20-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="6ac20-122">Wybierz pozycję **wszystkie usługi** , a następnie **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="6ac20-123">Wybierz opcję **prywatny Portal Marketplace** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="6ac20-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="6ac20-124">[![Pokazuje prywatną opcję menu Marketplace po lewej stronie portalu Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="6ac20-125">Wybierz pozycję **Kontrola dostępu (IAM)** , aby przypisać rolę administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Pokazuje ekran kontroli dostępu M.":::

1. <span data-ttu-id="6ac20-127">Wybierz pozycję **+ Dodaj** > **Dodaj przypisanie roli**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="6ac20-128">W obszarze **rola** wybierz pozycję **administrator witryny Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Pokazuje menu przypisania roli.":::

1. <span data-ttu-id="6ac20-130">Wybierz żądanego użytkownika z listy rozwijanej, a następnie wybierz pozycję **gotowe**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="6ac20-131">Przypisywanie roli administratora portalu Marketplace przy użyciu programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="6ac20-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="6ac20-132">Aby przypisać rolę administratora portalu Marketplace, użyj następującego skryptu programu PowerShell: wymaga następujących parametrów:</span><span class="sxs-lookup"><span data-stu-id="6ac20-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="6ac20-133">**TenantId:** Identyfikator dzierżawy w zakresie (rola administratora portalu Marketplace można przypisać do zakresu dzierżawy).</span><span class="sxs-lookup"><span data-stu-id="6ac20-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="6ac20-134">**Identyfikator subskrypcji:** Subskrypcja, której administrator globalny ma przypisaną rolę **współautora** lub wyższą.</span><span class="sxs-lookup"><span data-stu-id="6ac20-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="6ac20-135">**GlobalAdminUsername:** Nazwa użytkownika administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="6ac20-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="6ac20-136">**UsernameToAssignRoleFor:** Nazwa użytkownika, do którego zostanie przypisana rola administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="6ac20-137">Użytkownicy-Goście zaproszeni do dzierżawy mogą zająć do 48 godzin, dopóki ich konto nie będzie dostępne do przypisywania roli administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="6ac20-138">Aby uzyskać więcej informacji, zobacz [właściwości Azure Active Directory użytkownika współpracy B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="6ac20-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="6ac20-139">Aby uzyskać więcej informacji o poleceniach cmdlet zawartych w module AZ. Portal PowerShell, zobacz [Microsoft Azure PowerShell: polecenia cmdlet pulpitu nawigacyjnego portalu](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="6ac20-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="6ac20-140">Tworzenie prywatnego portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="6ac20-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="6ac20-141">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6ac20-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6ac20-142">Wybierz pozycję **wszystkie usługi** , a następnie **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Wyświetla okno główne Azure Portal.":::

3. <span data-ttu-id="6ac20-144">Wybierz opcję **prywatny Portal Marketplace** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="6ac20-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="6ac20-145">Wybierz pozycję **Rozpocznij** , aby utworzyć prywatny Portal Azure Marketplace (należy to zrobić tylko raz).</span><span class="sxs-lookup"><span data-stu-id="6ac20-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Pokazuje, jak wybrać okno główne &quot;Rozpocznij pracę w Azure Portal&quot;.":::

    <span data-ttu-id="6ac20-147">Jeśli prywatny Portal Azure Marketplace już istnieje dla tej dzierżawy, domyślnie wybierz pozycję Zarządzaj portalem **Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="6ac20-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="6ac20-148">Po zakończeniu będziesz mieć pusty i wyłączony prywatny Portal Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Pokazuje pusty prywatny ekran portalu Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="6ac20-150">Dodaj elementy z galerii</span><span class="sxs-lookup"><span data-stu-id="6ac20-150">Add items from gallery</span></span>

<span data-ttu-id="6ac20-151">Element jest kombinacją oferty i planu.</span><span class="sxs-lookup"><span data-stu-id="6ac20-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="6ac20-152">Możesz wyszukiwać i dodawać elementy na stronie zarządzanie rynkiem Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="6ac20-153">Wybierz pozycję **Dodaj elementy**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-153">Select **Add items**.</span></span>

2. <span data-ttu-id="6ac20-154">Przejrzyj **galerię** lub użyj pola wyszukiwania, aby znaleźć żądany element.</span><span class="sxs-lookup"><span data-stu-id="6ac20-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="6ac20-155">[![Pokazuje, jak przeglądać galerię lub użyć pola wyszukiwania.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="6ac20-156">Domyślnie podczas dodawania nowej oferty wszystkie bieżące plany zostaną dodane do listy zatwierdzonych.</span><span class="sxs-lookup"><span data-stu-id="6ac20-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="6ac20-157">Aby zmodyfikować wybór planu przed dodaniem wybranych elementów, wybierz menu rozwijane na kafelku oferty i zaktualizuj wymagane plany.</span><span class="sxs-lookup"><span data-stu-id="6ac20-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Pokazuje, jak aktualizować wymagane plany.":::

4. <span data-ttu-id="6ac20-159">Wybierz pozycję **gotowe** w lewym dolnym rogu po dokonaniu wyboru.</span><span class="sxs-lookup"><span data-stu-id="6ac20-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="6ac20-160">**Dodawanie elementów** do portalu Marketplace będzie możliwe tylko dla ofert innych niż firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6ac20-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="6ac20-161">Rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) będą znakowane jako "zatwierdzone domyślnie" i nie mogą być zarządzane w ramach prywatnego portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="6ac20-162">Edytuj plany elementu</span><span class="sxs-lookup"><span data-stu-id="6ac20-162">Edit item's plans</span></span>

<span data-ttu-id="6ac20-163">Plany elementu można edytować na stronie zarządzanie rynkiem Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="6ac20-164">W kolumnie **plany** Przejrzyj dostępne plany z menu rozwijanego dla tego elementu.</span><span class="sxs-lookup"><span data-stu-id="6ac20-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="6ac20-165">Zaznacz lub wyczyść pola wyboru, aby wybrać, które plany mają być dostępne dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6ac20-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Pokazuje, jak zaznaczyć lub wyczyścić pole wyboru dla wymaganego elementu.":::

> [!NOTE]
> <span data-ttu-id="6ac20-167">Każda oferta wymaga co najmniej jednego planu wybranego na potrzeby aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="6ac20-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="6ac20-168">Aby usunąć wszystkie plany związane z ofertą, Usuń całą ofertę (zobacz następną sekcję).</span><span class="sxs-lookup"><span data-stu-id="6ac20-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="6ac20-169">Usuń oferty</span><span class="sxs-lookup"><span data-stu-id="6ac20-169">Delete offers</span></span>

<span data-ttu-id="6ac20-170">Na stronie zarządzanie rynkiem Marketplace zaznacz pole wyboru obok nazwy oferty (zobacz ekran powyżej) i wybierz pozycję **Usuń elementy**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="6ac20-171">Włączanie/wyłączanie prywatnego portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="6ac20-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="6ac20-172">Na stronie zarządzanie rynkiem Marketplace zostanie wyświetlony jeden z następujących transparentów, który pokazuje bieżący stan prywatnego portalu Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="6ac20-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Pokazuje transparent &quot;Disable State&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Pokazuje transparent &quot;Enable State&quot;.":::

<span data-ttu-id="6ac20-175">Możesz włączyć lub wyłączyć prywatny Portal Azure Marketplace zgodnie z wymaganiami.</span><span class="sxs-lookup"><span data-stu-id="6ac20-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="6ac20-176">Jeśli ta opcja jest wyłączona, wybierz pozycję **Włącz prywatną witrynę Marketplace** , aby włączyć.</span><span class="sxs-lookup"><span data-stu-id="6ac20-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="6ac20-177">Jeśli ta opcja jest włączona, wybierz pozycję **Wyłącz prywatną witrynę Marketplace** , aby wyłączyć.</span><span class="sxs-lookup"><span data-stu-id="6ac20-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="6ac20-178">Prywatne centrum powiadomień portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="6ac20-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="6ac20-179">Centrum powiadomień składa się z trzech typów powiadomień i umożliwia administratorowi portalu Marketplace podejmowanie działań na podstawie powiadomienia:</span><span class="sxs-lookup"><span data-stu-id="6ac20-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="6ac20-180">Żądania zatwierdzenia od użytkowników dla elementów, które nie znajdują się na liście zatwierdzonych (zobacz [żądanie dodania ofert lub planów](#request-to-add-offers-or-plans) poniżej).</span><span class="sxs-lookup"><span data-stu-id="6ac20-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="6ac20-181">Nowe powiadomienia dotyczące planu dla ofert, które mają już jeden lub więcej planów na liście zatwierdzonych.</span><span class="sxs-lookup"><span data-stu-id="6ac20-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="6ac20-182">Usunięto powiadomienia dotyczące planu dla elementów, które znajdują się na liście zatwierdzonych, ale zostały usunięte z globalnego portalu Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="6ac20-183">Aby uzyskać dostęp do centrum powiadomień:</span><span class="sxs-lookup"><span data-stu-id="6ac20-183">To access the notification center:</span></span>

1. <span data-ttu-id="6ac20-184">Z menu po lewej stronie wybierz pozycję **powiadomienia** .</span><span class="sxs-lookup"><span data-stu-id="6ac20-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="6ac20-185">[![Pokazuje menu powiadomienia.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="6ac20-186">Wybierz menu wielokropka, aby uzyskać więcej akcji.</span><span class="sxs-lookup"><span data-stu-id="6ac20-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Wyświetla wyniki menu Więcej opcji.":::

1. <span data-ttu-id="6ac20-188">W przypadku żądań planu **Pokaż żądania** powoduje otwarcie formularza żądania zatwierdzenia, w którym można przejrzeć wszystkie żądania użytkowników dotyczące konkretnej oferty.</span><span class="sxs-lookup"><span data-stu-id="6ac20-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="6ac20-189">Wybierz pozycję **Zatwierdź** lub **Odrzuć**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="6ac20-190">[![Wyświetla opcje Zatwierdź i Odrzuć.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="6ac20-191">Wybierz plan do zatwierdzenia z menu rozwijanego.</span><span class="sxs-lookup"><span data-stu-id="6ac20-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="6ac20-192">Dodaj komentarz i wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="6ac20-193">Przeglądanie prywatnego portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="6ac20-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="6ac20-194">Po włączeniu prywatnego portalu Azure Marketplace użytkownicy zobaczą plany zatwierdzone przez administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="6ac20-195">Zielona **zatwierdzona** informacja wskazuje ofertę partnera (firmy innej niż Microsoft), która została zatwierdzona.</span><span class="sxs-lookup"><span data-stu-id="6ac20-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="6ac20-196">Niebieska **zatwierdzona** informacja wskazuje na ofertę firmy Microsoft (w tym zatwierdzone [dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)).</span><span class="sxs-lookup"><span data-stu-id="6ac20-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="6ac20-197">Użytkownicy mogą filtrować między ofertami, które nie są zatwierdzone:</span><span class="sxs-lookup"><span data-stu-id="6ac20-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="6ac20-198">[![Wyświetla opcję filtrowania.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="6ac20-199">Kup lub Wdróż w prywatnym portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="6ac20-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="6ac20-200">Chociaż środowisko strony szczegółów produktu jest podobne do globalnego portalu Azure Marketplace, istnieją trzy scenariusze specyficzne dla platformy Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="6ac20-201">Gdy użytkownik wybierze zatwierdzony plan, przycisk **Utwórz** jest włączony:</span><span class="sxs-lookup"><span data-stu-id="6ac20-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="6ac20-202">[![Pokazuje baner oferty z uwzględnieniem planu, który można utworzyć.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="6ac20-203">Jeśli wybór planu produktu nie jest wyświetlany na stronie Szczegóły produktu, ale administrator zatwierdził jeden lub więcej planów, transparent, które plany zostały zatwierdzone i jest włączony przycisk **Utwórz** :</span><span class="sxs-lookup"><span data-stu-id="6ac20-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="6ac20-204">[![Pokazuje baner oferty z informacją, że można utworzyć plan i wyświetlić dostępne plany.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="6ac20-205">Gdy użytkownik wybierze niezatwierdzony plan, transparent zauważa, że plan jako niezatwierdzony i przycisk **Utwórz** jest wyłączony.</span><span class="sxs-lookup"><span data-stu-id="6ac20-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="6ac20-206">Użytkownik nadal może zażądać dodania planu do zatwierdzonej listy (zobacz następną sekcję).</span><span class="sxs-lookup"><span data-stu-id="6ac20-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="6ac20-207">Żądanie dodania ofert lub planów</span><span class="sxs-lookup"><span data-stu-id="6ac20-207">Request to add offers or plans</span></span>

<span data-ttu-id="6ac20-208">Możesz poprosić o dodanie publicznej oferty lub planu, który nie jest obecnie zatwierdzony w prywatnym portalu Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6ac20-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="6ac20-209">Wybierz pozycję **żądanie do dodania** na banerze, aby otworzyć **formularz żądania dostępu**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="6ac20-210">[![Wyświetla transparent z linkiem "żądanie do dodania".](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="6ac20-211">[![Pokazuje formularz żądania dostępu dla ofert lub planów.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="6ac20-212">Wybierz, które plany dodać do żądania (**dowolny plan** informuje administratora portalu Marketplace, że nie masz preferencji dotyczących planu w ramach oferty).</span><span class="sxs-lookup"><span data-stu-id="6ac20-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="6ac20-213">Dodaj **uzasadnienie** i wybierz **żądanie** przesłania żądania.</span><span class="sxs-lookup"><span data-stu-id="6ac20-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="6ac20-214">[![Przedstawia formularz żądania dostępu dla ofert lub planów z przykładowymi wpisami.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="6ac20-215">Wskazanie oczekującego żądania pojawi się w formularzu żądania dostępu z opcją **wycofania żądania**.</span><span class="sxs-lookup"><span data-stu-id="6ac20-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="6ac20-216">[![Przedstawia listę zatwierdzonych lub oczekujących planów z linkiem żądania wycofania.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="6ac20-217">Po przesłaniu formularz żądania zatwierdzenia zostanie wysłany do [centrum powiadomień](#private-azure-marketplace-notification-center) dla administratora portalu Marketplace, aby przejrzeć żądanie i podjąć odpowiednie działania.</span><span class="sxs-lookup"><span data-stu-id="6ac20-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="6ac20-218">Często zadawane pytania</span><span class="sxs-lookup"><span data-stu-id="6ac20-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="6ac20-219">Mam już blokadę aplikacji innych firm za poorednictwem Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="6ac20-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="6ac20-220">Czym różnią się?</span><span class="sxs-lookup"><span data-stu-id="6ac20-220">How is this different?</span></span>

<span data-ttu-id="6ac20-221">Obecnie istnieją dwa sposoby ograniczania usług innych firm w witrynie Marketplace:</span><span class="sxs-lookup"><span data-stu-id="6ac20-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="6ac20-222">Za pomocą portalu EA lub Azure Portal należy wyłączyć usługi innych firm lub ograniczyć je tylko do wersji "Free or BYOL SKU".</span><span class="sxs-lookup"><span data-stu-id="6ac20-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Pokazuje, jak ograniczyć usługi w Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Pokazuje, jak ograniczyć usługi w portalu E.":::

2. <span data-ttu-id="6ac20-225">Utwórz zasady platformy Azure, aby zezwalać tylko na określone maszyny wirtualne.</span><span class="sxs-lookup"><span data-stu-id="6ac20-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="6ac20-226">Aby uzyskać szczegółowe informacje dotyczące wymuszania zasad na maszynach wirtualnych z systemem Windows, zobacz [stosowanie zasad do maszyn wirtualnych z systemem Windows za pomocą Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="6ac20-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="6ac20-227">Prywatny Portal Azure Marketplace zapewnia większą elastyczność w zakresie ograniczania i zezwalania na konkretne oferty i plany.</span><span class="sxs-lookup"><span data-stu-id="6ac20-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="6ac20-228">Informuje użytkowników końcowych o dostępności wdrożenia w galerii Marketplace nawet przed podjęciem próby wdrożenia usług innych firm.</span><span class="sxs-lookup"><span data-stu-id="6ac20-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="6ac20-229">Aby zezwolić na wdrażanie usług innych firm, ustaw witrynę Azure Marketplace na włączona/włączona w witrynie EA Portal i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="6ac20-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="6ac20-230">Prywatny Portal Azure Marketplace może nadzorować rozwiązania partnerskie, które nie są ograniczone do maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="6ac20-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="6ac20-231">Prywatny Portal Azure Marketplace może być nadzorowany na poziomie planu i można również ustawić "bieżący i przyszły plan".</span><span class="sxs-lookup"><span data-stu-id="6ac20-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="6ac20-232">Prywatny Portal Azure Marketplace może informować użytkowników końcowych o tym, co można i których nie można wdrożyć.</span><span class="sxs-lookup"><span data-stu-id="6ac20-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="6ac20-233">Jaka jest różnica między prywatną ofertą a prywatnym portalem Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="6ac20-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="6ac20-234">**Oferta prywatna** umożliwia wydawcom tworzenie planów, które są widoczne tylko dla klientów skierowanych do określonych.</span><span class="sxs-lookup"><span data-stu-id="6ac20-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="6ac20-235">Dzięki temu można prywatnie udostępniać dostosowane rozwiązania z negocjowanymi cenami, warunkami prywatnymi i warunkami oraz wyspecjalizowanymi konfiguracjami.</span><span class="sxs-lookup"><span data-stu-id="6ac20-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="6ac20-236">Aby uzyskać szczegółowe informacje, zobacz [prywatne oferty w komercyjnej witrynie Marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="6ac20-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="6ac20-237">**Prywatna witryna Azure Marketplace** w Azure Portal umożliwia administratorom wstępne zatwierdzanie rozwiązań innych firm, które użytkownicy mogą wdrażać.</span><span class="sxs-lookup"><span data-stu-id="6ac20-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="6ac20-238">Korzystając z prywatnego portalu Azure Marketplace, użytkownicy mogą korzystać z zalet platformy Azure Marketplace, wyszukując, kupując i wdrażając zgodne oferty.</span><span class="sxs-lookup"><span data-stu-id="6ac20-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="6ac20-239">Aby zarządzać ofertami prywatnymi opartymi na subskrypcji w prywatnej witrynie Marketplace, Administrator portalu Marketplace musi mieć co najmniej rolę "Odczyt" w danej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="6ac20-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="6ac20-240">Dlaczego została dodana prywatna oferta do prywatnego portalu Azure Marketplace, dlaczego nie jest wyświetlana na karcie zarządzanie rynkiem Marketplace?</span><span class="sxs-lookup"><span data-stu-id="6ac20-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="6ac20-241">Oferty prywatne oparte na subskrypcji są widoczne tylko dla subskrypcji w ustawieniach oferty prywatnej.</span><span class="sxs-lookup"><span data-stu-id="6ac20-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="6ac20-242">Aby wyświetlić ofertę prywatną, upewnij się, że globalny filtr subskrypcji wyświetla wszystkie subskrypcje.</span><span class="sxs-lookup"><span data-stu-id="6ac20-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="6ac20-243">[![Pokazuje prywatny filtr portalu Marketplace.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6ac20-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="6ac20-244">Czy można dołączać niestandardowe obrazy do prywatnego portalu Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="6ac20-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="6ac20-245">Nie.</span><span class="sxs-lookup"><span data-stu-id="6ac20-245">No.</span></span> <span data-ttu-id="6ac20-246">Prywatna witryna Azure Marketplace pozwala administratorom IT zarządzać rozwiązaniami innych firm w witrynie Azure Marketplace i nadzorować je.</span><span class="sxs-lookup"><span data-stu-id="6ac20-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="6ac20-247">Ponieważ obrazy niestandardowe nie znajdują się w globalnej witrynie Azure Marketplace, administrator IT nie może wybierać i wybierać obrazów niestandardowych.</span><span class="sxs-lookup"><span data-stu-id="6ac20-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="6ac20-248">Jeśli chcesz udostępnić niestandardowe obrazy, użyj [galerii obrazów udostępnionych](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="6ac20-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="6ac20-249">Przewodnik krok po kroku tworzenie udostępnionej galerii obrazów (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="6ac20-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="6ac20-250">Utwórz definicję obrazu w ramach SIG.</span><span class="sxs-lookup"><span data-stu-id="6ac20-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="6ac20-251">Klient powinien wybrać opcję **uogólnione** dla pola stan systemu operacyjnego.</span><span class="sxs-lookup"><span data-stu-id="6ac20-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="6ac20-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="6ac20-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="6ac20-253">Przenoszenie zarządzanego obrazu do galerii obrazów udostępnionych ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="6ac20-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="6ac20-254">Obrazy maszyn wirtualnych SIG mogą znajdować się w jednej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="6ac20-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="6ac20-255">Aby udostępnić je innym subskrypcjom, należy użyć rejestracji aplikacji ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="6ac20-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="6ac20-256">Dlaczego widzę pewne oferty, które są **Domyślnie zatwierdzane** mimo tego, że Wydawca nie jest firmą Microsoft?</span><span class="sxs-lookup"><span data-stu-id="6ac20-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="6ac20-257">Firma Microsoft obsługuje technologie dla systemów Linux i Open Source na platformie Azure.</span><span class="sxs-lookup"><span data-stu-id="6ac20-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="6ac20-258">Na platformie Azure obsługiwane są [rozpowszechniane dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) , a cena jest zintegrowana z maszynami wirtualnymi.</span><span class="sxs-lookup"><span data-stu-id="6ac20-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="6ac20-259">Ponieważ Agent systemu Linux Azure jest już wstępnie zainstalowany w witrynie Azure Marketplace, jest traktowany jak oferta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6ac20-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="6ac20-260">Ponieważ oferty firmy Microsoft są domyślnie zatwierdzane, nie można zarządzać potwierdzoną dystrybucją systemu Linux w prywatnym portalu Azure Marketplace i są one domyślnie zatwierdzane.</span><span class="sxs-lookup"><span data-stu-id="6ac20-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="6ac20-261">Kontakt z pomocą techniczną</span><span class="sxs-lookup"><span data-stu-id="6ac20-261">Contact support</span></span>

- <span data-ttu-id="6ac20-262">Aby uzyskać pomoc techniczną dotyczącą platformy Azure Marketplace, odwiedź stronę [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="6ac20-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
