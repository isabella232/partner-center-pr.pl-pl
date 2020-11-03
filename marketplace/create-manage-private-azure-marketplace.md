---
title: Utwórz prywatną witrynę Azure Marketplace i zarządzaj nią w Azure Portal
description: Dowiedz się więcej na temat tworzenia prywatnego portalu Azure Marketplace (wersja zapoznawcza) i zarządzania nim w Azure Portal.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: c0a395a7c5bfe926cdc56d7386aaaebb0305fb68
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/19/2020
ms.locfileid: "92529758"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="f2e82-103">Tworzenie prywatnego portalu Azure Marketplace (wersja zapoznawcza) i zarządzanie nim w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="f2e82-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="f2e82-104">Prywatny Portal Azure Marketplace (wersja zapoznawcza) umożliwia administratorom zarządzanie rozwiązaniami innych firm, które mogą być używane przez użytkowników.</span><span class="sxs-lookup"><span data-stu-id="f2e82-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="f2e82-105">W tym celu można wdrożyć tylko oferty zatwierdzane i zgodne z zasadami obowiązującymi w przedsiębiorstwie.</span><span class="sxs-lookup"><span data-stu-id="f2e82-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="f2e82-106">Korzystając z prywatnego portalu Azure Marketplace, użytkownicy mogą wyszukiwać oferty zgodne ze sklepem online, aby móc kupować i wdrażać.</span><span class="sxs-lookup"><span data-stu-id="f2e82-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="f2e82-107">Jako Administrator portalu Marketplace (przypisana rola) rozpocznie się z wyłączonym i pustym magazynem prywatnym, w którym można dodać zatwierdzone oferty i plany.</span><span class="sxs-lookup"><span data-stu-id="f2e82-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="f2e82-108">W tym artykule opisano sposób tworzenia i włączania prywatnego portalu Azure Marketplace dla użytkowników oraz zarządzania nimi.</span><span class="sxs-lookup"><span data-stu-id="f2e82-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="f2e82-109">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="f2e82-109">Notes:</span></span>

- <span data-ttu-id="f2e82-110">Prywatny Portal Azure Marketplace jest na poziomie dzierżawy, dlatego wszyscy użytkownicy w ramach dzierżawy będą widzieć tę samą listę nadzorowana.</span><span class="sxs-lookup"><span data-stu-id="f2e82-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="f2e82-111">Wszystkie rozwiązania firmy Microsoft są automatycznie dodawane do prywatnego portalu Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="f2e82-112">Przypisywanie roli administratora portalu Marketplace</span><span class="sxs-lookup"><span data-stu-id="f2e82-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="f2e82-113">Administrator globalny dzierżawy musi przypisać rolę **administratora portalu Marketplace** do prywatnego administratora portalu Azure Marketplace, który będzie zarządzać magazynem prywatnym.</span><span class="sxs-lookup"><span data-stu-id="f2e82-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="f2e82-114">Dostęp do prywatnego zarządzania w portalu Azure Marketplace jest dostępny tylko dla administratorów IT z przypisaną rolą administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="f2e82-115">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="f2e82-115">Prerequisites</span></span>

<span data-ttu-id="f2e82-116">Aby można było przypisać rolę administratora portalu Marketplace do użytkownika w zakresie dzierżawy, należy spełnić te wymagania wstępne:</span><span class="sxs-lookup"><span data-stu-id="f2e82-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="f2e82-117">Masz dostęp do użytkownika **administratora globalnego** .</span><span class="sxs-lookup"><span data-stu-id="f2e82-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="f2e82-118">Dzierżawca ma co najmniej jedną subskrypcję (może być dowolnego typu).</span><span class="sxs-lookup"><span data-stu-id="f2e82-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="f2e82-119">Użytkownikowi administratora globalnego przypisano rolę **współautor** lub wyższą dla subskrypcji wybranej w kroku 2.</span><span class="sxs-lookup"><span data-stu-id="f2e82-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="f2e82-120">Użytkownik Administrator globalny ma podwyższony poziom dostępu do wartości **tak** (zobacz [podnoszenie uprawnień dostępu-globalny-administrator](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="f2e82-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="f2e82-121">Przypisywanie roli administratora portalu Marketplace przy użyciu programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="f2e82-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="f2e82-122">Aby przypisać rolę administratora portalu Marketplace, użyj następującego skryptu programu PowerShell: wymaga następujących parametrów:</span><span class="sxs-lookup"><span data-stu-id="f2e82-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="f2e82-123">**TenantId:** Identyfikator dzierżawy w zakresie (rola administratora portalu Marketplace można przypisać do zakresu dzierżawy).</span><span class="sxs-lookup"><span data-stu-id="f2e82-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="f2e82-124">**Identyfikator subskrypcji:** Subskrypcja, której administrator globalny ma przypisaną rolę **współautora** lub wyższą.</span><span class="sxs-lookup"><span data-stu-id="f2e82-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="f2e82-125">**GlobalAdminUsername:** Nazwa użytkownika administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="f2e82-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="f2e82-126">**UsernameToAssignRoleFor:** Nazwa użytkownika, do którego zostanie przypisana rola administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="f2e82-127">Użytkownicy-Goście zaproszeni do dzierżawy mogą zająć do 48 godzin, dopóki ich konto nie będzie dostępne do przypisywania roli administratora portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="f2e82-128">Aby uzyskać więcej informacji, zobacz [właściwości Azure Active Directory użytkownika współpracy B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="f2e82-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="f2e82-129">Aby uzyskać więcej informacji o poleceniach cmdlet zawartych w module AZ. Portal PowerShell, zobacz [Microsoft Azure PowerShell: polecenia cmdlet pulpitu nawigacyjnego portalu](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="f2e82-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="f2e82-130">Tworzenie prywatnego portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f2e82-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="f2e82-131">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f2e82-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f2e82-132">Wybierz pozycję **wszystkie usługi** , a następnie **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="f2e82-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal głównego okna.":::

3. <span data-ttu-id="f2e82-134">Wybierz opcję **prywatny Portal Marketplace** z opcji po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="f2e82-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Wybieranie opcji prywatny Portal Marketplace w oknie głównym Azure Portal.":::

4. <span data-ttu-id="f2e82-136">Wybierz pozycję **Rozpocznij** , aby utworzyć prywatny Portal Azure Marketplace (należy to zrobić tylko raz).</span><span class="sxs-lookup"><span data-stu-id="f2e82-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Wybieranie pozycji Rozpocznij pracę w oknie głównym Azure Portal.":::

    <span data-ttu-id="f2e82-138">Jeśli prywatny Portal Azure Marketplace już istnieje dla tej dzierżawy, domyślnie wybierz pozycję Zarządzaj portalem **Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="f2e82-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="f2e82-139">Po zakończeniu będziesz mieć pusty i wyłączony prywatny Portal Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Pusty ekran prywatnego portalu Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="f2e82-141">Dodaj elementy z galerii</span><span class="sxs-lookup"><span data-stu-id="f2e82-141">Add items from gallery</span></span>

<span data-ttu-id="f2e82-142">Element jest kombinacją oferty i planu.</span><span class="sxs-lookup"><span data-stu-id="f2e82-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="f2e82-143">Możesz wyszukiwać i dodawać elementy na stronie zarządzanie rynkiem Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f2e82-144">Wybierz pozycję **Dodaj elementy**.</span><span class="sxs-lookup"><span data-stu-id="f2e82-144">Select **Add items**.</span></span>

2. <span data-ttu-id="f2e82-145">Przejrzyj **galerię** lub użyj pola wyszukiwania, aby znaleźć żądany element.</span><span class="sxs-lookup"><span data-stu-id="f2e82-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Przeglądanie galerii lub używanie pola wyszukiwania.":::

3. <span data-ttu-id="f2e82-147">Domyślnie podczas dodawania nowej oferty wszystkie bieżące plany zostaną dodane do listy dozwolonych.</span><span class="sxs-lookup"><span data-stu-id="f2e82-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="f2e82-148">Aby zmodyfikować wybór planu przed dodaniem wybranych elementów, wybierz menu rozwijane na kafelku oferty i zaktualizuj wymagane plany.</span><span class="sxs-lookup"><span data-stu-id="f2e82-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aktualizuj wymagane plany.":::

4. <span data-ttu-id="f2e82-150">Wybierz pozycję **gotowe** w lewym dolnym rogu po dokonaniu wyboru.</span><span class="sxs-lookup"><span data-stu-id="f2e82-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="f2e82-151">**Dodawanie elementów** do portalu Marketplace będzie możliwe tylko dla ofert innych niż firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2e82-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="f2e82-152">Oferty firmy Microsoft są domyślnie dozwolone.</span><span class="sxs-lookup"><span data-stu-id="f2e82-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="f2e82-153">Edytuj plany elementów</span><span class="sxs-lookup"><span data-stu-id="f2e82-153">Edit item plans</span></span>

<span data-ttu-id="f2e82-154">Plany elementu można edytować na stronie zarządzanie rynkiem Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f2e82-155">W kolumnie **plany** Przejrzyj dostępne plany z menu rozwijanego dla tego elementu.</span><span class="sxs-lookup"><span data-stu-id="f2e82-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="f2e82-156">Zaznacz lub wyczyść pola wyboru, aby wybrać, które plany mają być dostępne dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="f2e82-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zaznaczanie lub czyszczenie pola wyboru dla wymaganego elementu.":::

> [!NOTE]
> <span data-ttu-id="f2e82-158">Każda oferta wymaga co najmniej jednego planu, aby można było przeprowadzić aktualizację.</span><span class="sxs-lookup"><span data-stu-id="f2e82-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="f2e82-159">Aby usunąć wszystkie plany związane z ofertą, Usuń całą ofertę (zobacz następną sekcję).</span><span class="sxs-lookup"><span data-stu-id="f2e82-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="f2e82-160">Usuń oferty</span><span class="sxs-lookup"><span data-stu-id="f2e82-160">Delete offers</span></span>

<span data-ttu-id="f2e82-161">Na stronie zarządzanie rynkiem Marketplace zaznacz pole wyboru obok nazwy oferty (zobacz ekran powyżej) i wybierz pozycję **Usuń elementy**.</span><span class="sxs-lookup"><span data-stu-id="f2e82-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="f2e82-162">Włączanie/wyłączanie prywatnego portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f2e82-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="f2e82-163">Na stronie zarządzanie rynkiem Marketplace zostanie wyświetlony jeden z następujących transparentów, który pokazuje bieżący stan prywatnego portalu Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="f2e82-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Wyłącz transparent stanu":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Włącz transparent stanu":::

<span data-ttu-id="f2e82-166">Możesz włączyć lub wyłączyć prywatny Portal Azure Marketplace zgodnie z wymaganiami.</span><span class="sxs-lookup"><span data-stu-id="f2e82-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="f2e82-167">Jeśli ta opcja jest wyłączona, wybierz pozycję **Włącz prywatną witrynę Marketplace** , aby włączyć.</span><span class="sxs-lookup"><span data-stu-id="f2e82-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="f2e82-168">Jeśli ta opcja jest włączona, wybierz pozycję **Wyłącz prywatną witrynę Marketplace** , aby wyłączyć.</span><span class="sxs-lookup"><span data-stu-id="f2e82-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="f2e82-169">Przeglądanie prywatnego portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f2e82-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="f2e82-170">Po włączeniu prywatnego portalu Azure Marketplace użytkownicy będą widzieć, które plany mogą być dozwolone dla administratorów portalu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="f2e82-171">Zielona **dozwolona** informacja to oferta partnera (firmy innej niż Microsoft), która jest dozwolona.</span><span class="sxs-lookup"><span data-stu-id="f2e82-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="f2e82-172">Niebieska **dopuszczalna** informacja wskazuje, że oferta firmy Microsoft jest dozwolona.</span><span class="sxs-lookup"><span data-stu-id="f2e82-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="f2e82-173">Użytkownicy mogą filtrować między ofertami, które są niedozwolone:</span><span class="sxs-lookup"><span data-stu-id="f2e82-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opcja filtrowania.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="f2e82-175">Kup lub Wdróż w prywatnym portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f2e82-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="f2e82-176">Chociaż środowisko strony szczegółów produktu przypomina publiczną witrynę Azure Marketplace, istnieją trzy scenariusze specyficzne dla platformy Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2e82-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="f2e82-177">Gdy użytkownik wybierze dozwolony plan, przycisk **Utwórz** jest włączony:</span><span class="sxs-lookup"><span data-stu-id="f2e82-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Baner oferty z uwzględnieniem planu można utworzyć.":::

- <span data-ttu-id="f2e82-179">Gdy użytkownik wybierze niedozwolony plan, transparent nie jest dozwolony, a przycisk **Utwórz** jest wyłączony.</span><span class="sxs-lookup"><span data-stu-id="f2e82-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Baner oferty nie można utworzyć planu.":::

- <span data-ttu-id="f2e82-181">Jeśli wybór planu produktu nie jest wyświetlany na stronie Szczegóły produktu, ale administrator zatwierdził jeden lub więcej planów, transparenty, które plany są dozwolone i przycisk **Utwórz** jest włączony:</span><span class="sxs-lookup"><span data-stu-id="f2e82-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Baner oferty z uwzględnieniem planu można utworzyć i pokazać dostępne plany.":::

## <a name="contact-support"></a><span data-ttu-id="f2e82-183">Kontakt z pomocą techniczną</span><span class="sxs-lookup"><span data-stu-id="f2e82-183">Contact support</span></span>

<span data-ttu-id="f2e82-184">Aby uzyskać pomoc techniczną dotyczącą platformy Azure Marketplace, odwiedź stronę [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="f2e82-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
