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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Utwórz prywatną witrynę Azure Marketplace i zarządzaj nią w Azure Portal

Prywatny Portal Azure Marketplace umożliwia administratorom zarządzanie rozwiązaniami innych firm, które mogą być używane przez użytkowników. Jest to możliwe dzięki umożliwieniu użytkownikowi wdrożenia tylko ofert zatwierdzonych przez administratora i przestrzegania zasad obowiązujących w przedsiębiorstwie. Korzystając z prywatnego portalu Azure Marketplace, użytkownicy mogą przeszukiwać oferty zgodne ze sklepem online, aby móc kupować i wdrażać.

Jako Administrator portalu Marketplace (przypisana rola) rozpocznie się z wyłączonym i pustym magazynem prywatnym, w którym można dodać zatwierdzone oferty i plany. W tym artykule wyjaśniono, jak przypisać potrzebną rolę, utworzyć magazyn prywatny, zarządzać elementami, zatwierdzać żądania użytkowników i włączać prywatne witryny Azure Marketplace dla użytkowników.

> [!NOTE]
> - Prywatny Portal Azure Marketplace jest na poziomie dzierżawy, dlatego wszyscy użytkownicy w ramach dzierżawy będą widzieć tę samą listę nadzorowana.
> - Wszystkie rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) są automatycznie dodawane do prywatnego portalu Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Przypisywanie roli administratora portalu Marketplace

Administrator globalny dzierżawy musi przypisać rolę **administratora portalu Marketplace** do prywatnego administratora portalu Azure Marketplace, który będzie zarządzać magazynem prywatnym.

>[!IMPORTANT]
> Dostęp do prywatnego zarządzania w portalu Azure Marketplace jest dostępny tylko dla administratorów IT z przypisaną rolą administratora portalu Marketplace.

### <a name="prerequisites"></a>Wymagania wstępne

Te wymagania wstępne są wymagane przed przypisaniem roli administratora portalu Marketplace do użytkownika w zakresie dzierżawy:

- Masz dostęp do użytkownika **administratora globalnego** .
- Dzierżawca ma co najmniej jedną subskrypcję (może być dowolnego typu).
- Użytkownikowi administratora globalnego przypisano rolę **współautor** lub wyższą dla wybranej subskrypcji.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Przypisywanie roli administratora portalu Marketplace przy użyciu kontroli dostępu (IAM)

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).
1. Wybierz pozycję **wszystkie usługi** , a następnie **Marketplace**.
1. Wybierz opcję **prywatny Portal Marketplace** z menu po lewej stronie.

    [![Pokazuje prywatną opcję menu Marketplace po lewej stronie portalu Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Wybierz pozycję **Kontrola dostępu (IAM)** , aby przypisać rolę administratora portalu Marketplace.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Pokazuje ekran kontroli dostępu M.":::

1. Wybierz pozycję **+ Dodaj** > **Dodaj przypisanie roli**.
1. W obszarze **rola** wybierz pozycję **administrator witryny Marketplace**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Pokazuje menu przypisania roli.":::

1. Wybierz żądanego użytkownika z listy rozwijanej, a następnie wybierz pozycję **gotowe**.

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

Aby uzyskać więcej informacji o poleceniach cmdlet zawartych w module AZ. Portal PowerShell, zobacz [Microsoft Azure PowerShell: polecenia cmdlet pulpitu nawigacyjnego portalu](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Tworzenie prywatnego portalu Azure Marketplace

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).
2. Wybierz pozycję **wszystkie usługi** , a następnie **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Wyświetla okno główne Azure Portal.":::

3. Wybierz opcję **prywatny Portal Marketplace** z menu po lewej stronie.

4. Wybierz pozycję **Rozpocznij** , aby utworzyć prywatny Portal Azure Marketplace (należy to zrobić tylko raz).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Pokazuje, jak wybrać okno główne &quot;Rozpocznij pracę w Azure Portal&quot;.":::

    Jeśli prywatny Portal Azure Marketplace już istnieje dla tej dzierżawy, domyślnie wybierz pozycję Zarządzaj portalem **Marketplace** .

5. Po zakończeniu będziesz mieć pusty i wyłączony prywatny Portal Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Pokazuje pusty prywatny ekran portalu Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Dodaj elementy z galerii

Element jest kombinacją oferty i planu. Możesz wyszukiwać i dodawać elementy na stronie zarządzanie rynkiem Marketplace.

1. Wybierz pozycję **Dodaj elementy**.

2. Przejrzyj **galerię** lub użyj pola wyszukiwania, aby znaleźć żądany element.

    [![Pokazuje, jak przeglądać galerię lub użyć pola wyszukiwania.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Domyślnie podczas dodawania nowej oferty wszystkie bieżące plany zostaną dodane do listy zatwierdzonych. Aby zmodyfikować wybór planu przed dodaniem wybranych elementów, wybierz menu rozwijane na kafelku oferty i zaktualizuj wymagane plany.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Pokazuje, jak aktualizować wymagane plany.":::

4. Wybierz pozycję **gotowe** w lewym dolnym rogu po dokonaniu wyboru.

>[!Note]
> **Dodawanie elementów** do portalu Marketplace będzie możliwe tylko dla ofert innych niż firmy Microsoft. Rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) będą znakowane jako "zatwierdzone domyślnie" i nie mogą być zarządzane w ramach prywatnego portalu Marketplace.

## <a name="edit-items-plans"></a>Edytuj plany elementu

Plany elementu można edytować na stronie zarządzanie rynkiem Marketplace.

1. W kolumnie **plany** Przejrzyj dostępne plany z menu rozwijanego dla tego elementu.
2. Zaznacz lub wyczyść pola wyboru, aby wybrać, które plany mają być dostępne dla użytkowników.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Pokazuje, jak zaznaczyć lub wyczyścić pole wyboru dla wymaganego elementu.":::

> [!NOTE]
> Każda oferta wymaga co najmniej jednego planu wybranego na potrzeby aktualizacji. Aby usunąć wszystkie plany związane z ofertą, Usuń całą ofertę (zobacz następną sekcję).

## <a name="delete-offers"></a>Usuń oferty

Na stronie zarządzanie rynkiem Marketplace zaznacz pole wyboru obok nazwy oferty (zobacz ekran powyżej) i wybierz pozycję **Usuń elementy**.

## <a name="enabledisable-private-azure-marketplace"></a>Włączanie/wyłączanie prywatnego portalu Azure Marketplace

Na stronie zarządzanie rynkiem Marketplace zostanie wyświetlony jeden z następujących transparentów, który pokazuje bieżący stan prywatnego portalu Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Pokazuje transparent &quot;Disable State&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Pokazuje transparent &quot;Enable State&quot;.":::

Możesz włączyć lub wyłączyć prywatny Portal Azure Marketplace zgodnie z wymaganiami.

- Jeśli ta opcja jest wyłączona, wybierz pozycję **Włącz prywatną witrynę Marketplace** , aby włączyć.
- Jeśli ta opcja jest włączona, wybierz pozycję **Wyłącz prywatną witrynę Marketplace** , aby wyłączyć.

## <a name="private-azure-marketplace-notification-center"></a>Prywatne centrum powiadomień portalu Azure Marketplace

Centrum powiadomień składa się z trzech typów powiadomień i umożliwia administratorowi portalu Marketplace podejmowanie działań na podstawie powiadomienia:

- Żądania zatwierdzenia od użytkowników dla elementów, które nie znajdują się na liście zatwierdzonych (zobacz [żądanie dodania ofert lub planów](#request-to-add-offers-or-plans) poniżej).
- Nowe powiadomienia dotyczące planu dla ofert, które mają już jeden lub więcej planów na liście zatwierdzonych.
- Usunięto powiadomienia dotyczące planu dla elementów, które znajdują się na liście zatwierdzonych, ale zostały usunięte z globalnego portalu Azure Marketplace.

Aby uzyskać dostęp do centrum powiadomień:

1. Z menu po lewej stronie wybierz pozycję **powiadomienia** .

    [![Pokazuje menu powiadomienia.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Wybierz menu wielokropka, aby uzyskać więcej akcji.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Wyświetla wyniki menu Więcej opcji.":::

1. W przypadku żądań planu **Pokaż żądania** powoduje otwarcie formularza żądania zatwierdzenia, w którym można przejrzeć wszystkie żądania użytkowników dotyczące konkretnej oferty.
1. Wybierz pozycję **Zatwierdź** lub **Odrzuć**.

    [![Wyświetla opcje Zatwierdź i Odrzuć.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Wybierz plan do zatwierdzenia z menu rozwijanego.
1. Dodaj komentarz i wybierz pozycję **Prześlij**.

## <a name="browsing-private-azure-marketplace"></a>Przeglądanie prywatnego portalu Azure Marketplace

Po włączeniu prywatnego portalu Azure Marketplace użytkownicy zobaczą plany zatwierdzone przez administratora portalu Marketplace.

- Zielona **zatwierdzona** informacja wskazuje ofertę partnera (firmy innej niż Microsoft), która została zatwierdzona.
- Niebieska **zatwierdzona** informacja wskazuje na ofertę firmy Microsoft (w tym zatwierdzone [dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)).

Użytkownicy mogą filtrować między ofertami, które nie są zatwierdzone:

[![Wyświetla opcję filtrowania.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Kup lub Wdróż w prywatnym portalu Azure Marketplace

Chociaż środowisko strony szczegółów produktu jest podobne do globalnego portalu Azure Marketplace, istnieją trzy scenariusze specyficzne dla platformy Azure Marketplace.

- Gdy użytkownik wybierze zatwierdzony plan, przycisk **Utwórz** jest włączony:

    [![Pokazuje baner oferty z uwzględnieniem planu, który można utworzyć.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Jeśli wybór planu produktu nie jest wyświetlany na stronie Szczegóły produktu, ale administrator zatwierdził jeden lub więcej planów, transparent, które plany zostały zatwierdzone i jest włączony przycisk **Utwórz** :

    [![Pokazuje baner oferty z informacją, że można utworzyć plan i wyświetlić dostępne plany.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Gdy użytkownik wybierze niezatwierdzony plan, transparent zauważa, że plan jako niezatwierdzony i przycisk **Utwórz** jest wyłączony. Użytkownik nadal może zażądać dodania planu do zatwierdzonej listy (zobacz następną sekcję).

## <a name="request-to-add-offers-or-plans"></a>Żądanie dodania ofert lub planów

Możesz poprosić o dodanie publicznej oferty lub planu, który nie jest obecnie zatwierdzony w prywatnym portalu Azure Marketplace.

1. Wybierz pozycję **żądanie do dodania** na banerze, aby otworzyć **formularz żądania dostępu**.

    [![Wyświetla transparent z linkiem "żądanie do dodania".](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Pokazuje formularz żądania dostępu dla ofert lub planów.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Wybierz, które plany dodać do żądania (**dowolny plan** informuje administratora portalu Marketplace, że nie masz preferencji dotyczących planu w ramach oferty).

1. Dodaj **uzasadnienie** i wybierz **żądanie** przesłania żądania.
  
    [![Przedstawia formularz żądania dostępu dla ofert lub planów z przykładowymi wpisami.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Wskazanie oczekującego żądania pojawi się w formularzu żądania dostępu z opcją **wycofania żądania**.

    [![Przedstawia listę zatwierdzonych lub oczekujących planów z linkiem żądania wycofania.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Po przesłaniu formularz żądania zatwierdzenia zostanie wysłany do [centrum powiadomień](#private-azure-marketplace-notification-center) dla administratora portalu Marketplace, aby przejrzeć żądanie i podjąć odpowiednie działania.

## <a name="frequently-asked-questions-faqs"></a>Często zadawane pytania

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Mam już blokadę aplikacji innych firm za poorednictwem Azure Policy. Czym różnią się?

Obecnie istnieją dwa sposoby ograniczania usług innych firm w witrynie Marketplace:

1. Za pomocą portalu EA lub Azure Portal należy wyłączyć usługi innych firm lub ograniczyć je tylko do wersji "Free or BYOL SKU".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Pokazuje, jak ograniczyć usługi w Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Pokazuje, jak ograniczyć usługi w portalu E.":::

2. Utwórz zasady platformy Azure, aby zezwalać tylko na określone maszyny wirtualne. Aby uzyskać szczegółowe informacje dotyczące wymuszania zasad na maszynach wirtualnych z systemem Windows, zobacz [stosowanie zasad do maszyn wirtualnych z systemem Windows za pomocą Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).

Prywatny Portal Azure Marketplace zapewnia większą elastyczność w zakresie ograniczania i zezwalania na konkretne oferty i plany. Informuje użytkowników końcowych o dostępności wdrożenia w galerii Marketplace nawet przed podjęciem próby wdrożenia usług innych firm. Aby zezwolić na wdrażanie usług innych firm, ustaw witrynę Azure Marketplace na włączona/włączona w witrynie EA Portal i Azure Portal.

- Prywatny Portal Azure Marketplace może nadzorować rozwiązania partnerskie, które nie są ograniczone do maszyn wirtualnych.
- Prywatny Portal Azure Marketplace może być nadzorowany na poziomie planu i można również ustawić "bieżący i przyszły plan".
- Prywatny Portal Azure Marketplace może informować użytkowników końcowych o tym, co można i których nie można wdrożyć.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Jaka jest różnica między prywatną ofertą a prywatnym portalem Azure Marketplace?

**Oferta prywatna** umożliwia wydawcom tworzenie planów, które są widoczne tylko dla klientów skierowanych do określonych. Dzięki temu można prywatnie udostępniać dostosowane rozwiązania z negocjowanymi cenami, warunkami prywatnymi i warunkami oraz wyspecjalizowanymi konfiguracjami. Aby uzyskać szczegółowe informacje, zobacz [prywatne oferty w komercyjnej witrynie Marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).

**Prywatna witryna Azure Marketplace** w Azure Portal umożliwia administratorom wstępne zatwierdzanie rozwiązań innych firm, które użytkownicy mogą wdrażać. Korzystając z prywatnego portalu Azure Marketplace, użytkownicy mogą korzystać z zalet platformy Azure Marketplace, wyszukując, kupując i wdrażając zgodne oferty. Aby zarządzać ofertami prywatnymi opartymi na subskrypcji w prywatnej witrynie Marketplace, Administrator portalu Marketplace musi mieć co najmniej rolę "Odczyt" w danej subskrypcji.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Dlaczego została dodana prywatna oferta do prywatnego portalu Azure Marketplace, dlaczego nie jest wyświetlana na karcie zarządzanie rynkiem Marketplace?

Oferty prywatne oparte na subskrypcji są widoczne tylko dla subskrypcji w ustawieniach oferty prywatnej. Aby wyświetlić ofertę prywatną, upewnij się, że globalny filtr subskrypcji wyświetla wszystkie subskrypcje.

[![Pokazuje prywatny filtr portalu Marketplace.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Czy można dołączać niestandardowe obrazy do prywatnego portalu Azure Marketplace?

Nie. Prywatna witryna Azure Marketplace pozwala administratorom IT zarządzać rozwiązaniami innych firm w witrynie Azure Marketplace i nadzorować je. Ponieważ obrazy niestandardowe nie znajdują się w globalnej witrynie Azure Marketplace, administrator IT nie może wybierać i wybierać obrazów niestandardowych. Jeśli chcesz udostępnić niestandardowe obrazy, użyj [galerii obrazów udostępnionych](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).

1. Przewodnik krok po kroku tworzenie udostępnionej galerii obrazów (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).
2. Utwórz definicję obrazu w ramach SIG. Klient powinien wybrać opcję **uogólnione** dla pola stan systemu operacyjnego. ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Przenoszenie zarządzanego obrazu do galerii obrazów udostępnionych ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).
4. Obrazy maszyn wirtualnych SIG mogą znajdować się w jednej subskrypcji. Aby udostępnić je innym subskrypcjom, należy użyć rejestracji aplikacji ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Dlaczego widzę pewne oferty, które są **Domyślnie zatwierdzane** mimo tego, że Wydawca nie jest firmą Microsoft?

Firma Microsoft obsługuje technologie dla systemów Linux i Open Source na platformie Azure. Na platformie Azure obsługiwane są [rozpowszechniane dystrybucje systemu Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) , a cena jest zintegrowana z maszynami wirtualnymi. Ponieważ Agent systemu Linux Azure jest już wstępnie zainstalowany w witrynie Azure Marketplace, jest traktowany jak oferta firmy Microsoft. Ponieważ oferty firmy Microsoft są domyślnie zatwierdzane, nie można zarządzać potwierdzoną dystrybucją systemu Linux w prywatnym portalu Azure Marketplace i są one domyślnie zatwierdzane.

## <a name="contact-support"></a>Kontakt z pomocą techniczną

- Aby uzyskać pomoc techniczną dotyczącą platformy Azure Marketplace, odwiedź stronę [Microsoft Q&A](/answers/products/).
