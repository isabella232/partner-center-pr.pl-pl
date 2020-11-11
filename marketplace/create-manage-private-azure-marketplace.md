---
title: Utwórz prywatną witrynę Azure Marketplace i zarządzaj nią w Azure Portal
description: Dowiedz się więcej na temat tworzenia prywatnego portalu Azure Marketplace (wersja zapoznawcza) i zarządzania nim w Azure Portal.
ms.prod: marketplace-customer
ms.topic: article
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 1333bb2c8830cec83d7b7f05890af818d5c0ce5b
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/11/2020
ms.locfileid: "94487707"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Tworzenie prywatnego portalu Azure Marketplace (wersja zapoznawcza) i zarządzanie nim w Azure Portal

Prywatny Portal Azure Marketplace (wersja zapoznawcza) umożliwia administratorom zarządzanie rozwiązaniami innych firm, które mogą być używane przez użytkowników. W tym celu można wdrożyć tylko oferty zatwierdzane i zgodne z zasadami obowiązującymi w przedsiębiorstwie. Korzystając z prywatnego portalu Azure Marketplace, użytkownicy mogą wyszukiwać oferty zgodne ze sklepem online, aby móc kupować i wdrażać. 

Jako Administrator portalu Marketplace (przypisana rola) rozpocznie się z wyłączonym i pustym magazynem prywatnym, w którym można dodać zatwierdzone oferty i plany. W tym artykule opisano sposób tworzenia i włączania prywatnego portalu Azure Marketplace dla użytkowników oraz zarządzania nimi.

Uwagi:

- Prywatny Portal Azure Marketplace jest na poziomie dzierżawy, dlatego wszyscy użytkownicy w ramach dzierżawy będą widzieć tę samą listę nadzorowana.
- Wszystkie rozwiązania firmy Microsoft są automatycznie dodawane do prywatnego portalu Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Przypisywanie roli administratora portalu Marketplace

Administrator globalny dzierżawy musi przypisać rolę **administratora portalu Marketplace** do prywatnego administratora portalu Azure Marketplace, który będzie zarządzać magazynem prywatnym.

>[!IMPORTANT]
> Dostęp do prywatnego zarządzania w portalu Azure Marketplace jest dostępny tylko dla administratorów IT z przypisaną rolą administratora portalu Marketplace.

### <a name="prerequisites"></a>Wymagania wstępne

Aby można było przypisać rolę administratora portalu Marketplace do użytkownika w zakresie dzierżawy, należy spełnić te wymagania wstępne:

- Masz dostęp do użytkownika **administratora globalnego** .
- Dzierżawca ma co najmniej jedną subskrypcję (może być dowolnego typu).
- Użytkownikowi administratora globalnego przypisano rolę **współautor** lub wyższą dla subskrypcji wybranej w kroku 2.
- Użytkownik Administrator globalny ma podwyższony poziom dostępu do wartości **tak** (zobacz [podnoszenie uprawnień dostępu-globalny-administrator](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Przypisywanie roli administratora portalu Marketplace przy użyciu programu PowerShell

Aby przypisać rolę administratora portalu Marketplace, użyj następującego skryptu programu PowerShell: wymaga następujących parametrów:

- **TenantId:** Identyfikator dzierżawy w zakresie (rola administratora portalu Marketplace można przypisać do zakresu dzierżawy).
- **Identyfikator subskrypcji:** Subskrypcja, której administrator globalny ma przypisaną rolę **współautora** lub wyższą.
- **GlobalAdminUsername:** Nazwa użytkownika administratora globalnego.
- **UsernameToAssignRoleFor:** Nazwa użytkownika, do którego zostanie przypisana rola administratora portalu Marketplace.

> [!NOTE]
> Użytkownicy-Goście zaproszeni do dzierżawy mogą zająć do 48 godzin, dopóki ich konto nie będzie dostępne do przypisywania roli administratora portalu Marketplace. Aby uzyskać więcej informacji, zobacz [właściwości Azure Active Directory użytkownika współpracy B2B](/azure/active-directory/b2b/user-properties).

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

Aby uzyskać więcej informacji o poleceniach cmdlet zawartych w module AZ. Portal PowerShell, zobacz [Microsoft Azure PowerShell: polecenia cmdlet pulpitu nawigacyjnego portalu](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Tworzenie prywatnego portalu Azure Marketplace

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).
2. Wybierz pozycję **wszystkie usługi** , a następnie **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal głównego okna.":::

3. Wybierz opcję **prywatny Portal Marketplace** z opcji po lewej stronie.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Wybieranie opcji prywatny Portal Marketplace w oknie głównym Azure Portal.":::

4. Wybierz pozycję **Rozpocznij** , aby utworzyć prywatny Portal Azure Marketplace (należy to zrobić tylko raz).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Wybieranie pozycji Rozpocznij pracę w oknie głównym Azure Portal.":::

    Jeśli prywatny Portal Azure Marketplace już istnieje dla tej dzierżawy, domyślnie wybierz pozycję Zarządzaj portalem **Marketplace** .

5. Po zakończeniu będziesz mieć pusty i wyłączony prywatny Portal Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Pusty ekran prywatnego portalu Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Dodaj elementy z galerii

Element jest kombinacją oferty i planu. Możesz wyszukiwać i dodawać elementy na stronie zarządzanie rynkiem Marketplace.

1. Wybierz pozycję **Dodaj elementy**.

2. Przejrzyj **galerię** lub użyj pola wyszukiwania, aby znaleźć żądany element.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Przeglądanie galerii lub używanie pola wyszukiwania.":::

3. Domyślnie podczas dodawania nowej oferty wszystkie bieżące plany zostaną dodane do listy dozwolonych. Aby zmodyfikować wybór planu przed dodaniem wybranych elementów, wybierz menu rozwijane na kafelku oferty i zaktualizuj wymagane plany.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aktualizuj wymagane plany.":::

4. Wybierz pozycję **gotowe** w lewym dolnym rogu po dokonaniu wyboru.

>[!Note]
> **Dodawanie elementów** do portalu Marketplace będzie możliwe tylko dla ofert innych niż firmy Microsoft. Oferty firmy Microsoft są domyślnie dozwolone.

## <a name="edit-item-plans"></a>Edytuj plany elementów

Plany elementu można edytować na stronie zarządzanie rynkiem Marketplace.

1. W kolumnie **plany** Przejrzyj dostępne plany z menu rozwijanego dla tego elementu.
2. Zaznacz lub wyczyść pola wyboru, aby wybrać, które plany mają być dostępne dla użytkowników.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zaznaczanie lub czyszczenie pola wyboru dla wymaganego elementu.":::

> [!NOTE]
> Każda oferta wymaga co najmniej jednego planu, aby można było przeprowadzić aktualizację. Aby usunąć wszystkie plany związane z ofertą, Usuń całą ofertę (zobacz następną sekcję).

## <a name="delete-offers"></a>Usuń oferty

Na stronie zarządzanie rynkiem Marketplace zaznacz pole wyboru obok nazwy oferty (zobacz ekran powyżej) i wybierz pozycję **Usuń elementy**.

## <a name="enabledisable-private-azure-marketplace"></a>Włączanie/wyłączanie prywatnego portalu Azure Marketplace

Na stronie zarządzanie rynkiem Marketplace zostanie wyświetlony jeden z następujących transparentów, który pokazuje bieżący stan prywatnego portalu Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Wyłącz transparent stanu":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Włącz transparent stanu":::

Możesz włączyć lub wyłączyć prywatny Portal Azure Marketplace zgodnie z wymaganiami.

1. Jeśli ta opcja jest wyłączona, wybierz pozycję **Włącz prywatną witrynę Marketplace** , aby włączyć.
2. Jeśli ta opcja jest włączona, wybierz pozycję **Wyłącz prywatną witrynę Marketplace** , aby wyłączyć.

## <a name="browsing-private-azure-marketplace"></a>Przeglądanie prywatnego portalu Azure Marketplace

Po włączeniu prywatnego portalu Azure Marketplace użytkownicy będą widzieć, które plany mogą być dozwolone dla administratorów portalu Marketplace.

- Zielona **dozwolona** informacja to oferta partnera (firmy innej niż Microsoft), która jest dozwolona.
- Niebieska **dopuszczalna** informacja wskazuje, że oferta firmy Microsoft jest dozwolona.

Użytkownicy mogą filtrować między ofertami, które są niedozwolone:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opcja filtrowania.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Kup lub Wdróż w prywatnym portalu Azure Marketplace

Chociaż środowisko strony szczegółów produktu przypomina publiczną witrynę Azure Marketplace, istnieją trzy scenariusze specyficzne dla platformy Azure Marketplace.

- Gdy użytkownik wybierze dozwolony plan, przycisk **Utwórz** jest włączony:

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Baner oferty z uwzględnieniem planu można utworzyć.":::

- Gdy użytkownik wybierze niedozwolony plan, transparent nie jest dozwolony, a przycisk **Utwórz** jest wyłączony.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Baner oferty nie można utworzyć planu.":::

- Jeśli wybór planu produktu nie jest wyświetlany na stronie Szczegóły produktu, ale administrator zatwierdził jeden lub więcej planów, transparenty, które plany są dozwolone i przycisk **Utwórz** jest włączony:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Baner oferty z uwzględnieniem planu można utworzyć i pokazać dostępne plany.":::

## <a name="contact-support"></a>Kontakt z pomocą techniczną

Aby uzyskać pomoc techniczną dotyczącą platformy Azure Marketplace, odwiedź stronę [Microsoft Q&A](/answers/products/). 
