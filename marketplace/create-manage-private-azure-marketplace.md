---
title: Tworzenie prywatnych Azure Marketplace i zarządzanie nimi w Azure Portal
description: Dowiedz się więcej na temat tworzenia prywatnych Azure Marketplace (wersja zapoznawcza) i zarządzania nimi w Azure Portal. Prywatne Azure Marketplace (wersja zapoznawcza) umożliwiają administratorom określenie, z których rozwiązań innych firm mogą korzystać ich użytkownicy.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431668"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="c8901-104">Tworzenie prywatnych Azure Marketplace i zarządzanie nimi w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="c8901-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="c8901-105">Prywatne Azure Marketplace administratorzy mogą zarządzać rozwiązaniami innych firm, których mogą używać ich użytkownicy.</span><span class="sxs-lookup"><span data-stu-id="c8901-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="c8901-106">W tym celu użytkownik może wdrażać tylko te oferty, które zostały zatwierdzone przez administratora i są zgodne z zasadami przedsiębiorstwa.</span><span class="sxs-lookup"><span data-stu-id="c8901-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="c8901-107">W przypadku Azure Marketplace użytkownicy mogą wyszukiwać w sklepie online zgodne oferty zakupu i wdrożenia.</span><span class="sxs-lookup"><span data-stu-id="c8901-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="c8901-108">Jako administrator witryny Marketplace (przypisana rola) zaczniesz od wyłączonego i pustego sklepu prywatnego, w którym możesz dodać zatwierdzone oferty i plany.</span><span class="sxs-lookup"><span data-stu-id="c8901-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="c8901-109">W tym artykule wyjaśniono, jak przypisać potrzebną rolę, utworzyć magazyn prywatny, zarządzać elementami, zatwierdzać żądania użytkowników i włączać prywatne Azure Marketplace dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="c8901-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="c8901-110">Prywatne Azure Marketplace na poziomie dzierżawy, więc wszyscy użytkownicy w ramach dzierżawy będą widzieć tę samą nadzorowana listę.</span><span class="sxs-lookup"><span data-stu-id="c8901-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="c8901-111">Wszystkie rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux)](/azure/virtual-machines/linux/endorsed-distros)są automatycznie dodawane do usługi Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="c8901-112">Przypisywanie roli administratora witryny Marketplace</span><span class="sxs-lookup"><span data-stu-id="c8901-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="c8901-113">Administrator dzierżawy administrator globalny przypisać rolę administratora witryny **Marketplace** administratorowi usługi Azure Marketplace prywatnego, który będzie zarządzać sklepem prywatnym.</span><span class="sxs-lookup"><span data-stu-id="c8901-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="c8901-114">Dostęp do zarządzania Azure Marketplace prywatnymi jest dostępny tylko dla administratorów IT z przypisaną rolą administratora witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="c8901-115">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="c8901-115">Prerequisites</span></span>

<span data-ttu-id="c8901-116">Te wymagania wstępne są wymagane, aby można było przypisać rolę administratora witryny Marketplace do użytkownika w zakresie dzierżawy:</span><span class="sxs-lookup"><span data-stu-id="c8901-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="c8901-117">Masz dostęp do konta **administrator globalny** użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c8901-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="c8901-118">Dzierżawa ma co najmniej jedną subskrypcję (może być dowolnym typem).</span><span class="sxs-lookup"><span data-stu-id="c8901-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="c8901-119">Użytkownik administrator globalny ma przypisaną rolę **Współautor** lub wyższą dla wybranej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="c8901-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="c8901-120">Przypisywanie roli administratora witryny Marketplace przy użyciu kontroli dostępu (IAM)</span><span class="sxs-lookup"><span data-stu-id="c8901-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="c8901-121">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c8901-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="c8901-122">Wybierz **pozycję Wszystkie usługi,** a następnie pozycję **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="c8901-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="c8901-123">Wybierz **pozycję Prywatna platforma** handlowa z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="c8901-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="c8901-124">[![Wyświetla opcję menu prywatnej witryny Marketplace po lewej stronie witryny Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="c8901-125">Wybierz **pozycję Kontrola dostępu (IAM),** aby przypisać rolę administratora witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Wyświetla ekran kontrola dostępu do aplikacji I A M.":::

1. <span data-ttu-id="c8901-127">Wybierz pozycję **+ Dodaj** > **Dodaj przypisanie roli**.</span><span class="sxs-lookup"><span data-stu-id="c8901-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="c8901-128">W **obszarze Rola** wybierz pozycję Administrator witryny **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="c8901-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Wyświetla menu Przypisanie roli.":::

1. <span data-ttu-id="c8901-130">Wybierz żądanego użytkownika z listy rozwijanej, a następnie wybierz pozycję **Gotowe.**</span><span class="sxs-lookup"><span data-stu-id="c8901-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="c8901-131">Przypisywanie roli administratora witryny Marketplace przy użyciu programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="c8901-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="c8901-132">Użyj następującego skryptu programu PowerShell, aby przypisać rolę administratora witryny Marketplace. Wymaga on następujących parametrów:</span><span class="sxs-lookup"><span data-stu-id="c8901-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="c8901-133">**TenantId:** Identyfikator dzierżawy w zakresie (rolę administratora witryny Marketplace można przypisać w zakresie dzierżawy).</span><span class="sxs-lookup"><span data-stu-id="c8901-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="c8901-134">**SubscriptionId:** Subskrypcja, do której administrator globalny ma **przypisaną rolę współautora** lub wyższą.</span><span class="sxs-lookup"><span data-stu-id="c8901-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="c8901-135">**GlobalAdminUsername:** Nazwa użytkownika administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="c8901-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="c8901-136">**UsernameToAssignRoleFor:** Nazwa użytkownika, do którego zostanie przypisana rola administratora witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="c8901-137">W przypadku użytkowników-gości zaproszonych do dzierżawy przypisanie roli administratora witryny Marketplace może potrwać do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="c8901-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="c8901-138">Aby uzyskać więcej informacji, [zobacz Properties of an Azure Active Directory B2B collaboration user (Właściwości](/azure/active-directory/b2b/user-properties)użytkownika współpracy B2B).</span><span class="sxs-lookup"><span data-stu-id="c8901-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="c8901-139">Aby uzyskać więcej informacji na temat poleceń cmdlet zawartych w module Az.Portal programu PowerShell, zobacz Microsoft Azure PowerShell: Polecenia [cmdlet](/powershell/module/az.portal/)pulpitu nawigacyjnego portalu.</span><span class="sxs-lookup"><span data-stu-id="c8901-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="c8901-140">Tworzenie prywatnych Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="c8901-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="c8901-141">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c8901-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="c8901-142">Wybierz **pozycję Wszystkie usługi,** a następnie pozycję **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="c8901-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Wyświetla Azure Portal główne.":::

3. <span data-ttu-id="c8901-144">Wybierz **pozycję Prywatna platforma** handlowa z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="c8901-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="c8901-145">Wybierz **Rozpocznij,** aby utworzyć Azure Marketplace prywatne (trzeba to zrobić tylko raz).</span><span class="sxs-lookup"><span data-stu-id="c8901-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Pokazuje, jak wybrać pozycję Rozpocznij w Azure Portal głównym.":::

    <span data-ttu-id="c8901-147">Jeśli dla Azure Marketplace już istnieje prywatny dostęp, domyślnie zostanie wybrana opcja Zarządzaj platformą **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="c8901-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="c8901-148">Po zakończeniu będziesz mieć pusty i wyłączony prywatny Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Wyświetla pusty ekran Azure Marketplace prywatnego.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="c8901-150">Dodawanie elementów z galerii</span><span class="sxs-lookup"><span data-stu-id="c8901-150">Add items from gallery</span></span>

<span data-ttu-id="c8901-151">Element jest kombinacją oferty i planu.</span><span class="sxs-lookup"><span data-stu-id="c8901-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="c8901-152">Elementy można wyszukiwać i dodawać na stronie Zarządzanie platformą Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="c8901-153">Wybierz **pozycję Dodaj elementy.**</span><span class="sxs-lookup"><span data-stu-id="c8901-153">Select **Add items**.</span></span>

2. <span data-ttu-id="c8901-154">Przejrzyj **galerię** lub użyj pola wyszukiwania, aby znaleźć szukany element.</span><span class="sxs-lookup"><span data-stu-id="c8901-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="c8901-155">[![Pokazuje, jak przeglądać galerię lub używać pola wyszukiwania.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="c8901-156">Domyślnie podczas dodawania nowej oferty wszystkie bieżące plany zostaną dodane do listy zatwierdzonych.</span><span class="sxs-lookup"><span data-stu-id="c8901-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="c8901-157">Aby zmodyfikować wybór planu przed dodaniem wybranych elementów, wybierz menu rozwijane na kafelku oferty i zaktualizuj wymagane plany.</span><span class="sxs-lookup"><span data-stu-id="c8901-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Pokazuje, jak zaktualizować wymagane plany.":::

4. <span data-ttu-id="c8901-159">Po **wybraniu** opcji wybierz pozycję Gotowe w lewym dolnym rogu.</span><span class="sxs-lookup"><span data-stu-id="c8901-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="c8901-160">**Dodawanie elementów** do witryny Marketplace będzie dostępne tylko dla ofert innych niż firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8901-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="c8901-161">Rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux)](/azure/virtual-machines/linux/endorsed-distros)będą oznaczone jako "Zatwierdzone domyślnie" i nie będzie można nimi zarządzać w prywatnej witrynie Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="c8901-162">Edytowanie planów elementu</span><span class="sxs-lookup"><span data-stu-id="c8901-162">Edit item's plans</span></span>

<span data-ttu-id="c8901-163">Plany elementu można edytować na stronie Zarządzanie platformą Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="c8901-164">W **kolumnie Plany** przejrzyj dostępne plany z menu rozwijanego dla tego elementu.</span><span class="sxs-lookup"><span data-stu-id="c8901-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="c8901-165">Zaznacz lub wyczyść pola wyboru, aby wybrać plany, które mają być dostępne dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="c8901-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Pokazuje, jak zaznaczyć lub wyczyścić pole wyboru dla wymaganego elementu.":::

> [!NOTE]
> <span data-ttu-id="c8901-167">Każda oferta wymaga co najmniej jednego planu wybranego do aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="c8901-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="c8901-168">Aby usunąć wszystkie plany związane z ofertą, usuń całą ofertę (zobacz następną sekcję).</span><span class="sxs-lookup"><span data-stu-id="c8901-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="c8901-169">Usuwanie ofert</span><span class="sxs-lookup"><span data-stu-id="c8901-169">Delete offers</span></span>

<span data-ttu-id="c8901-170">Na stronie Zarządzanie platformą Marketplace zaznacz pole wyboru obok nazwy oferty (zobacz ekran powyżej), a następnie wybierz **pozycję Usuń elementy.**</span><span class="sxs-lookup"><span data-stu-id="c8901-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="c8901-171">Włączanie/wyłączanie prywatnych Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="c8901-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="c8901-172">Na stronie Zarządzanie platformą Marketplace zobaczysz jeden z tych banerów, które pokazują bieżący stan prywatnych Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="c8901-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Wyświetla transparent &quot;Wyłącz stan&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Wyświetla transparent &quot;Włącz stan&quot;.":::

<span data-ttu-id="c8901-175">W razie potrzeby można włączyć lub Azure Marketplace prywatne.</span><span class="sxs-lookup"><span data-stu-id="c8901-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="c8901-176">Jeśli ta ustawienie jest wyłączone, wybierz **pozycję Włącz prywatną platformę Marketplace,** aby ją włączyć.</span><span class="sxs-lookup"><span data-stu-id="c8901-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="c8901-177">Jeśli ta opcja jest włączona, **wybierz pozycję Wyłącz prywatną platformę Marketplace,** aby ją wyłączyć.</span><span class="sxs-lookup"><span data-stu-id="c8901-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="c8901-178">Prywatne Azure Marketplace powiadomień</span><span class="sxs-lookup"><span data-stu-id="c8901-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="c8901-179">Centrum powiadomień składa się z trzech typów powiadomień i umożliwia administratorowi witryny Marketplace działanie na podstawie powiadomienia:</span><span class="sxs-lookup"><span data-stu-id="c8901-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="c8901-180">Żądania zatwierdzenia od użytkowników dotyczące elementów, które nie znajdują się na liście zatwierdzonych (zobacz [Żądanie dodania ofert lub planów poniżej).](#request-to-add-offers-or-plans)</span><span class="sxs-lookup"><span data-stu-id="c8901-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="c8901-181">Powiadomienia o nowym planie dla ofert, które mają już co najmniej jeden plan na liście zatwierdzonych planów.</span><span class="sxs-lookup"><span data-stu-id="c8901-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="c8901-182">Usunięto powiadomienia o planach dla elementów, które znajdują się na liście zatwierdzonych, ale zostały usunięte z globalnej Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="c8901-183">Aby uzyskać dostęp do centrum powiadomień:</span><span class="sxs-lookup"><span data-stu-id="c8901-183">To access the notification center:</span></span>

1. <span data-ttu-id="c8901-184">Wybierz **pozycję Powiadomienia** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="c8901-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="c8901-185">[![Wyświetla menu Powiadomienia.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="c8901-186">Wybierz menu wielokropka, aby uzyskać więcej akcji.</span><span class="sxs-lookup"><span data-stu-id="c8901-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Wyświetla wyniki menu Więcej opcji.":::

1. <span data-ttu-id="c8901-188">W przypadku żądań planu **show requests** otwiera formularz żądania zatwierdzenia, w którym można przejrzeć wszystkie żądania użytkowników dotyczące określonej oferty.</span><span class="sxs-lookup"><span data-stu-id="c8901-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="c8901-189">Wybierz pozycję **Zatwierdź** **lub Odrzuć.**</span><span class="sxs-lookup"><span data-stu-id="c8901-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="c8901-190">[![Przedstawia opcje zatwierdzania i odrzucania.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="c8901-191">Wybierz plan do zatwierdzenia z menu rozwijanego.</span><span class="sxs-lookup"><span data-stu-id="c8901-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="c8901-192">Dodaj komentarz i wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="c8901-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="c8901-193">Przeglądanie prywatnych Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="c8901-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="c8901-194">Po włączeniu Azure Marketplace prywatnego użytkownicy zobaczą plany zatwierdzone przez administratora witryny Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="c8901-195">Zielone powiadomienie **Zatwierdzone** oznacza, że oferta partnera (spoza firmy Microsoft) została zatwierdzona.</span><span class="sxs-lookup"><span data-stu-id="c8901-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="c8901-196">Niebieskie powiadomienie **Zatwierdzone** oznacza ofertę firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux),](/azure/virtual-machines/linux/endorsed-distros)która została zatwierdzona.</span><span class="sxs-lookup"><span data-stu-id="c8901-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="c8901-197">Użytkownicy mogą filtrować między ofertami, które są zatwierdzone i nie zostały zatwierdzone:</span><span class="sxs-lookup"><span data-stu-id="c8901-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="c8901-198">[![Wyświetla opcję filtrowania.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="c8901-199">Kupowanie lub wdrażanie w usługach prywatnych Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="c8901-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="c8901-200">Chociaż środowisko strony szczegółów produktu jest podobne do globalnego Azure Marketplace, istnieją trzy scenariusze Azure Marketplace scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="c8901-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="c8901-201">Gdy użytkownik wybierze zatwierdzony plan, zostanie **włączony** przycisk Utwórz:</span><span class="sxs-lookup"><span data-stu-id="c8901-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="c8901-202">[![Wyświetla transparent oferty z notą planu, który można utworzyć.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="c8901-203">Jeśli wybór planu produktu nie jest wyświetlany na stronie szczegółów produktu, ale administrator zatwierdził co  najmniej jeden plan, zostanie wyświetlony baner z informacjami o zatwierdzonych planach i włączonym przyciskiem Utwórz:</span><span class="sxs-lookup"><span data-stu-id="c8901-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="c8901-204">[![Wyświetla transparent oferty z dopisem, że można utworzyć plan i wyświetlać dostępne plany.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="c8901-205">Gdy użytkownik wybierze niezatwierdzoną plan, transparent zgłosi plan jako niezatwierdzoną i przycisk **Utwórz** zostanie wyłączony.</span><span class="sxs-lookup"><span data-stu-id="c8901-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="c8901-206">Użytkownik może nadal zażądać dodania planu do listy zatwierdzonych (zobacz następną sekcję).</span><span class="sxs-lookup"><span data-stu-id="c8901-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="c8901-207">Żądanie dodania ofert lub planów</span><span class="sxs-lookup"><span data-stu-id="c8901-207">Request to add offers or plans</span></span>

<span data-ttu-id="c8901-208">Możesz zażądać dodania publicznej oferty lub planu, który nie jest obecnie zatwierdzony w prywatnej Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="c8901-209">Wybierz **pozycję Żądanie, aby** dodać na banerze, aby otworzyć formularz żądania **dostępu**.</span><span class="sxs-lookup"><span data-stu-id="c8901-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="c8901-210">[![Wyświetla transparent z linkiem "Request to add" (Żądanie dodania).](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="c8901-211">[![Przedstawia formularz żądania dostępu dla ofert lub planów.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="c8901-212">Wybierz plany do dodania do żądania (dowolny **plan** informuje administratora witryny Marketplace, że nie masz preferencji dla planu w ramach oferty).</span><span class="sxs-lookup"><span data-stu-id="c8901-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="c8901-213">Dodaj uzasadnienie **i** wybierz **pozycję Żądanie,** aby przesłać żądanie.</span><span class="sxs-lookup"><span data-stu-id="c8901-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="c8901-214">[![Przedstawia formularz żądania dostępu dla ofert lub planów z przykładami wpisów.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="c8901-215">Wskazanie oczekującego żądania pojawi się w formularzu Żądanie dostępu z opcją **Żądanie wycofywu.**</span><span class="sxs-lookup"><span data-stu-id="c8901-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="c8901-216">[![Przedstawia listę zatwierdzonych lub oczekujących planów z linkiem Żądanie wycofywu.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="c8901-217">Po przesłaniu formularz żądania zatwierdzenia zostanie [](#private-azure-marketplace-notification-center) wysłany do Centrum powiadomień dla administratora witryny Marketplace w celu przejrzenia żądania i podjęcia działania.</span><span class="sxs-lookup"><span data-stu-id="c8901-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="c8901-218">Zatwierdzenie w prywatnej witrynie Marketplace nie wskazuje na zakup rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="c8901-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="c8901-219">Często zadawane pytania</span><span class="sxs-lookup"><span data-stu-id="c8901-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="c8901-220">Już blokujem aplikację innej firmy z witryny Marketplace za pośrednictwem Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="c8901-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="c8901-221">Czym się różni?</span><span class="sxs-lookup"><span data-stu-id="c8901-221">How is this different?</span></span>

<span data-ttu-id="c8901-222">Obecnie istnieją dwa sposoby ograniczania usług innych firm w witrynie Marketplace:</span><span class="sxs-lookup"><span data-stu-id="c8901-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="c8901-223">Za pośrednictwem witryny EA Portal lub Azure Portal wyłącz usługi innych firm lub ogranicz je do "Tylko bezpłatne jednostki SKU lub BYOL".</span><span class="sxs-lookup"><span data-stu-id="c8901-223">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Pokazuje, jak ograniczyć usługi w Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Pokazuje, jak ograniczyć usługi w portalu E A.":::

2. <span data-ttu-id="c8901-226">Utwórz zasady platformy Azure, aby zezwalać tylko na określone maszyny wirtualne.</span><span class="sxs-lookup"><span data-stu-id="c8901-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="c8901-227">Aby uzyskać szczegółowe informacje na temat wymuszania zasad dla maszyn wirtualnych z systemem Windows, zobacz [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy)(Stosowanie zasad do maszyn wirtualnych z systemem Windows przy użyciu Azure Resource Manager ).</span><span class="sxs-lookup"><span data-stu-id="c8901-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="c8901-228">Prywatne Azure Marketplace zapewniają większą elastyczność ograniczania i zezwalania na określone oferty i plany.</span><span class="sxs-lookup"><span data-stu-id="c8901-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="c8901-229">Informuje ona użytkowników końcowych o dostępności wdrożenia w galerii marketplace jeszcze przed podjęciem próby wdrożenia usług innych firm.</span><span class="sxs-lookup"><span data-stu-id="c8901-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="c8901-230">Aby zezwolić na wdrażanie usług innych firm, ustaw Azure Marketplace wł./włączone w EA Portal i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="c8901-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="c8901-231">Prywatne Azure Marketplace mogą curate rozwiązań partnerskich, nie tylko maszyn wirtualnych.</span><span class="sxs-lookup"><span data-stu-id="c8901-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="c8901-232">Prywatne Azure Marketplace można wywłaszczyć na poziomie planu, a także ustawić "Bieżący i przyszły plan".</span><span class="sxs-lookup"><span data-stu-id="c8901-232">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="c8901-233">Prywatne Azure Marketplace z góry informować użytkowników końcowych o tym, co można i czego nie można wdrożyć.</span><span class="sxs-lookup"><span data-stu-id="c8901-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="c8901-234">Jaka jest różnica między ofertą prywatną i prywatną Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="c8901-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="c8901-235">Oferta **prywatna** umożliwia wydawcom tworzenie planów, które są widoczne tylko dla klientów docelowych.</span><span class="sxs-lookup"><span data-stu-id="c8901-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="c8901-236">Dzięki temu mogą prywatnie udostępniać dostosowane rozwiązania z wynegocjowaną ceną, prywatnymi warunkami i postanowieniami oraz wyspecjalizowanymi konfiguracjami.</span><span class="sxs-lookup"><span data-stu-id="c8901-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="c8901-237">Aby uzyskać szczegółowe informacje, [zobacz Private offers in the commercial marketplace (Oferty prywatne na platformie handlowej).](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="c8901-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="c8901-238">**Prywatne Azure Marketplace** w Azure Portal umożliwiają administratorom wstępne zatwierdzanie rozwiązań innych firm, które mogą wdrażać ich użytkownicy.</span><span class="sxs-lookup"><span data-stu-id="c8901-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="c8901-239">Dzięki prywatnej Azure Marketplace użytkownicy mogą korzystać z zalet usługi Azure Marketplace znajdowania, kupowania i wdrażania zgodnych ofert.</span><span class="sxs-lookup"><span data-stu-id="c8901-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="c8901-240">Aby zarządzać ofertami prywatnymi opartymi na subskrypcji w prywatnej witrynie Marketplace, administrator witryny Marketplace musi mieć co najmniej rolę "odczyt" dla określonej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="c8901-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="c8901-241">Dodano ofertę prywatną do portalu Azure Marketplace, dlaczego nie jest ona wyświetlona na karcie zarządzania platformą marketplace?</span><span class="sxs-lookup"><span data-stu-id="c8901-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="c8901-242">Oferty prywatne oparte na subskrypcji są widoczne tylko dla subskrypcji wymienionych w ustawieniach oferty prywatnej.</span><span class="sxs-lookup"><span data-stu-id="c8901-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="c8901-243">Aby wyświetlić ofertę prywatną, upewnij się, że globalny filtr subskrypcji pokazuje wszystkie subskrypcje.</span><span class="sxs-lookup"><span data-stu-id="c8901-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="c8901-244">[![Wyświetla filtr prywatnej witryny Marketplace.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c8901-244">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="c8901-245">Czy możemy uwzględnić obrazy niestandardowe w prywatnych Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="c8901-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="c8901-246">Nie.</span><span class="sxs-lookup"><span data-stu-id="c8901-246">No.</span></span> <span data-ttu-id="c8901-247">Prywatne Azure Marketplace umożliwia dowolnemu administratorowi IT zarządzanie rozwiązaniami innych firm i zarządzanie nimi z globalnego Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c8901-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="c8901-248">Ponieważ obrazy niestandardowe nie znajdują się w globalnej Azure Marketplace, administrator IT nie może wybrać obrazów niestandardowych.</span><span class="sxs-lookup"><span data-stu-id="c8901-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="c8901-249">Jeśli chcesz udostępnić obrazy niestandardowe, użyj [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="c8901-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="c8901-250">Przewodnik krok po kroku Tworzenie interfejsu Shared Image Gallery[(CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell).](/azure/virtual-machines/shared-images-powershell)</span><span class="sxs-lookup"><span data-stu-id="c8901-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="c8901-251">Utwórz definicję obrazu w obrębie funkcji SIG.</span><span class="sxs-lookup"><span data-stu-id="c8901-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="c8901-252">Klient powinien **wybrać opcję Uogólnione** dla pola Stan systemu operacyjnego.</span><span class="sxs-lookup"><span data-stu-id="c8901-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="c8901-253">(interfejs[wiersza polecenia,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [program PowerShell).](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)</span><span class="sxs-lookup"><span data-stu-id="c8901-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="c8901-254">Przyniesienie obrazu zarządzanego do Shared Image Gallery[(interfejs wiersza polecenia,](/azure/virtual-machines/image-version-managed-image-cli) [program PowerShell).](/azure/virtual-machines/image-version-managed-image-powershell)</span><span class="sxs-lookup"><span data-stu-id="c8901-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="c8901-255">Obrazy maszyn wirtualnych SIG znajdowały się w jednej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="c8901-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="c8901-256">Aby udostępnić ją innym subskrypcjom, użyj rejestracji aplikacji (interfejs[wiersza polecenia,](/azure/virtual-machines/linux/share-images-across-tenants) [program PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)</span><span class="sxs-lookup"><span data-stu-id="c8901-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="c8901-257">Dlaczego niektóre oferty są **domyślnie zatwierdzone,** mimo że wydawcą nie jest firma Microsoft?</span><span class="sxs-lookup"><span data-stu-id="c8901-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="c8901-258">Firma Microsoft obsługuje system Linux i technologię open source na platformie Azure.</span><span class="sxs-lookup"><span data-stu-id="c8901-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="c8901-259">[Zatwierdzone dystrybucje systemu Linux](/azure/virtual-machines/linux/endorsed-distros) są obsługiwane na platformie Azure, a cena jest zintegrowana z maszynami wirtualnymi.</span><span class="sxs-lookup"><span data-stu-id="c8901-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="c8901-260">Ponieważ agent systemu Linux na platformie Azure jest już wstępnie zainstalowany na Azure Marketplace, jest traktowany jak oferta firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8901-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="c8901-261">Ponieważ oferty firmy Microsoft są domyślnie zatwierdzane, zatwierdzone dystrybucje systemu Linux nie mogą być zarządzane w trybie prywatnym Azure Marketplace i są domyślnie zatwierdzane.</span><span class="sxs-lookup"><span data-stu-id="c8901-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="c8901-262">Kontakt z pomocą techniczną</span><span class="sxs-lookup"><span data-stu-id="c8901-262">Contact support</span></span>

- <span data-ttu-id="c8901-263">Aby uzyskać Azure Marketplace pomocy technicznej, odwiedź [stronę Microsoft Q&A.](/answers/products/)</span><span class="sxs-lookup"><span data-stu-id="c8901-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>