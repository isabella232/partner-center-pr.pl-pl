---
title: Tworzenie prywatnych Azure Marketplace i zarządzanie nimi w Azure Portal
description: Dowiedz się więcej o tworzeniu prywatnych Azure Marketplace (wersja zapoznawcza) i zarządzaniu nimi w Azure Portal widoku w starszej wersji. Prywatne Azure Marketplace (wersja zapoznawcza) umożliwiają administratorom określenie rozwiązań innych firm, których mogą używać ich użytkownicy.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 08/10/2021
ms.openlocfilehash: da44807519f18d6aa17e41d8e81b9ad774e40d2d
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246676"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Tworzenie prywatnych Azure Marketplace i zarządzanie nimi w Azure Portal

> [!NOTE]
> W tym artykule o mowa w starszej wersji Azure Marketplace. Nowy widok Kolekcje można znaleźć w tym [nowym artykule.](create-manage-private-azure-marketplace-new.md)

Zasady Azure Marketplace umożliwiają administratorom określenie, z których rozwiązań innych firm mogą korzystać ich użytkownicy. W tym celu użytkownik może wdrażać tylko oferty zatwierdzone przez administratora i zgodne z zasadami przedsiębiorstwa. W przypadku Azure Marketplace prywatnych użytkownicy mogą wyszukiwać w sklepie online zgodne oferty do zakupu i wdrożenia.

Jako administrator witryny Marketplace (przypisana rola) zaczniesz od wyłączonego i pustego sklepu prywatnego, w którym możesz dodać zatwierdzone oferty i plany. W tym artykule wyjaśniono, jak przypisać potrzebną rolę, utworzyć magazyn prywatny, zarządzać elementami, zatwierdzać żądania użytkowników i włączać prywatne Azure Marketplace dla użytkowników.

> [!NOTE]
> - Prywatne Azure Marketplace na poziomie dzierżawy, więc wszyscy użytkownicy w ramach tej dzierżawy będą widzieć tę samą listę nadzorowanych.
> - Wszystkie rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux)](/azure/virtual-machines/linux/endorsed-distros)są automatycznie dodawane do prywatnych Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Przypisywanie roli administratora witryny Marketplace

Administrator dzierżawy administrator globalny przypisać rolę administratora witryny **Marketplace** do administratora Azure Marketplace magazynu prywatnego, który będzie zarządzać sklepem prywatnym.

>[!IMPORTANT]
> Dostęp do zarządzania Azure Marketplace prywatnymi jest dostępny tylko dla administratorów IT z przypisaną rolą administratora witryny Marketplace.

### <a name="prerequisites"></a>Wymagania wstępne

Te wymagania wstępne są wymagane, aby można było przypisać rolę administratora witryny Marketplace do użytkownika w zakresie dzierżawy:

- Masz dostęp do konta **administrator globalny** użytkownika.
- Dzierżawa ma co najmniej jedną subskrypcję (może być dowolnym typem).
- Użytkownik administrator globalny ma przypisaną rolę **Współautor** lub wyższą dla wybranej subskrypcji.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Przypisywanie roli administratora witryny Marketplace przy użyciu kontroli dostępu (IAM)

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).

1. Wybierz **pozycję Wszystkie usługi,** a następnie pozycję **Marketplace.**

1. Wybierz **pozycję Prywatna platforma** handlowa z menu po lewej stronie.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Wyświetla opcję menu prywatnej witryny Marketplace po lewej stronie witryny Marketplace.":::

1. Wybierz **pozycję Kontrola dostępu (IAM),** aby przypisać rolę administratora witryny Marketplace.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Wyświetla ekran kontrola dostępu do aplikacji I A M.":::

1. Wybierz pozycję **+ Dodaj** > **Dodaj przypisanie roli**.

1. W **obszarze Rola** wybierz pozycję Administrator witryny **Marketplace.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Wyświetla menu Przypisanie roli.":::

1. Wybierz żądanego użytkownika z listy rozwijanej, a następnie wybierz pozycję **Gotowe.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Przypisywanie roli administratora witryny Marketplace przy użyciu programu PowerShell

Użyj następującego skryptu programu PowerShell, aby przypisać rolę administratora witryny Marketplace. Wymaga on następujących parametrów:

- **TenantId:** Identyfikator dzierżawy w zakresie (rolę administratora witryny Marketplace można przypisać w zakresie dzierżawy).
- **SubscriptionId:** Subskrypcja, do której administrator globalny ma **przypisaną rolę współautora** lub wyższą.
- **GlobalAdminUsername:** Nazwa użytkownika administratora globalnego.
- **UsernameToAssignRoleFor:** Nazwa użytkownika, do którego zostanie przypisana rola administratora witryny Marketplace.

> [!NOTE]
> W przypadku użytkowników-gości zaproszonych do dzierżawy przypisanie roli administratora witryny Marketplace może potrwać do 48 godzin. Aby uzyskać więcej informacji, zobacz Properties of an Azure Active Directory B2B collaboration user (Właściwości użytkownika współpracy [B2B).](/azure/active-directory/b2b/user-properties)

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

Aby uzyskać więcej informacji na temat poleceń cmdlet zawartych w module Az.Portal programu PowerShell, [zobacz Microsoft Azure PowerShell: Polecenia cmdlet](/powershell/module/az.portal/)pulpitu nawigacyjnego portalu.

## <a name="create-private-azure-marketplace"></a>Tworzenie prywatnych Azure Marketplace

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com/).
2. Wybierz **pozycję Wszystkie usługi,** a następnie pozycję **Marketplace.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Pokazuje Azure Portal okno główne.":::

3. Wybierz **pozycję Prywatna platforma** handlowa z menu po lewej stronie.

4. Wybierz **Wprowadzenie,** aby utworzyć Azure Marketplace prywatne (należy to zrobić tylko raz).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Pokazuje, jak wybrać pozycję Wprowadzenie w Azure Portal głównym.":::

    Jeśli dla tej Azure Marketplace już istnieje tryb prywatny, domyślnie zostanie wybrana opcja Zarządzaj platformą **Marketplace.**

5. Po zakończeniu będziesz mieć puste i wyłączone prywatne Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Wyświetla pusty ekran Azure Marketplace prywatnego.":::

## <a name="add-items-from-gallery"></a>Dodawanie elementów z galerii

Element jest kombinacją oferty i planu. Elementy można wyszukiwać i dodawać na stronie Zarządzanie platformą Marketplace.

1. Wybierz **pozycję Dodaj elementy.**

2. Przejrzyj **galerię** lub użyj pola wyszukiwania, aby znaleźć szukany element.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Pokazuje, jak przeglądać galerię lub używać pola wyszukiwania.":::

3. Domyślnie podczas dodawania nowej oferty wszystkie bieżące plany zostaną dodane do listy zatwierdzonych. Aby zmodyfikować wybór planu przed dodaniem wybranych elementów, wybierz menu rozwijane na kafelku oferty i zaktualizuj wymagane plany.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Pokazuje, jak zaktualizować wymagane plany.":::

4. Po **wybraniu** opcji wybierz pozycję Gotowe w lewym dolnym rogu.

>[!Note]
> **Dodawanie elementów** do witryny Marketplace będzie dostępne tylko dla ofert innych niż firmy Microsoft. Rozwiązania firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux)](/azure/virtual-machines/linux/endorsed-distros)będą oznaczone jako "Zatwierdzone domyślnie" i nie będzie można nimi zarządzać w prywatnej witrynie Marketplace.

## <a name="edit-items-plans"></a>Edytowanie planów elementu

Plany elementu można edytować na stronie Zarządzanie platformą Marketplace.

1. W **kolumnie Plany** przejrzyj dostępne plany z menu rozwijanego dla tego elementu.

2. Zaznacz lub wyczyść pola wyboru, aby wybrać plany, które mają być dostępne dla użytkowników.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Pokazuje, jak zaznaczyć lub wyczyścić pole wyboru dla wymaganego elementu.":::

   > [!NOTE]
   > Każda oferta wymaga co najmniej jednego planu wybranego do aktualizacji. Aby usunąć wszystkie plany związane z ofertą, usuń całą ofertę (zobacz następną sekcję).

## <a name="delete-offers"></a>Usuwanie ofert

Na stronie Zarządzanie platformą Marketplace zaznacz pole wyboru obok nazwy oferty (zobacz ekran powyżej), a następnie wybierz **pozycję Usuń elementy.**

## <a name="enabledisable-private-azure-marketplace"></a>Włączanie/wyłączanie prywatnych Azure Marketplace

Na stronie Zarządzanie platformą Marketplace zobaczysz jeden z tych banerów, które pokazują bieżący stan prywatnych Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Wyświetla transparent &quot;Wyłącz stan&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Wyświetla transparent &quot;Włącz stan&quot;.":::

W razie potrzeby można włączyć lub Azure Marketplace prywatne.

- Jeśli ta ustawienie jest wyłączone, wybierz **pozycję Włącz prywatną platformę Marketplace,** aby ją włączyć.
- Jeśli ta opcja jest włączona, **wybierz pozycję Wyłącz prywatną platformę Marketplace,** aby ją wyłączyć.

## <a name="private-azure-marketplace-notification-center"></a>Prywatne Azure Marketplace powiadomień

Centrum powiadomień składa się z trzech typów powiadomień i umożliwia administratorowi witryny Marketplace działanie na podstawie powiadomienia:

- Żądania zatwierdzenia od użytkowników dotyczące elementów, które nie znajdują się na liście zatwierdzonych (zobacz [Żądanie dodania ofert lub planów poniżej).](#request-to-add-offers-or-plans)
- Powiadomienia o nowym planie dla ofert, które mają już co najmniej jeden plan na liście zatwierdzonych planów.
- Usunięto powiadomienia o planach dla elementów, które znajdują się na liście zatwierdzonych, ale zostały usunięte z globalnego Azure Marketplace.

Aby uzyskać dostęp do centrum powiadomień:

1. Wybierz **pozycję Powiadomienia** z menu po lewej stronie.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Wyświetla menu Powiadomienia.":::

1. Wybierz menu wielokropka, aby uzyskać więcej akcji.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Wyświetla wyniki menu Więcej opcji.":::

1. W przypadku żądań planu **show requests** (Pokaż żądania) otwiera formularz żądania zatwierdzenia, w którym można przejrzeć wszystkie żądania użytkowników dotyczące określonej oferty.
1. Wybierz pozycję **Zatwierdź** **lub Odrzuć.**

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Przedstawia opcje zatwierdzania i odrzucania.":::

1. Wybierz plan do zatwierdzenia z menu rozwijanego.
1. Dodaj komentarz i wybierz pozycję **Prześlij.**

## <a name="browsing-private-azure-marketplace"></a>Przeglądanie prywatnych Azure Marketplace

Po włączeniu Azure Marketplace prywatnego użytkownicy zobaczą plany zatwierdzone przez administratora witryny Marketplace.

- Zielone powiadomienie **Zatwierdzone** oznacza, że oferta partnera (spoza firmy Microsoft) została zatwierdzona.
- Niebieskie powiadomienie **Zatwierdzone** oznacza ofertę firmy Microsoft (w tym [zatwierdzone dystrybucje systemu Linux),](/azure/virtual-machines/linux/endorsed-distros)która została zatwierdzona.

Użytkownicy mogą filtrować między ofertami, które są zatwierdzone i nie zostały zatwierdzone:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Wyświetla opcję filtrowania.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Kupowanie lub wdrażanie w usługach prywatnych Azure Marketplace

Chociaż środowisko strony szczegółów produktu jest podobne do globalnego Azure Marketplace, istnieją trzy scenariusze Azure Marketplace scenariuszy.

- Gdy użytkownik wybierze zatwierdzony plan, zostanie **włączony** przycisk Utwórz:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Wyświetla transparent oferty z notą, że można utworzyć plan.":::

- Jeśli wybór planu produktu nie jest wyświetlany na stronie szczegółów produktu, ale administrator zatwierdził co  najmniej jeden plan, na banerze znajdują się informacje o zatwierdzonych planach i włączony przycisk Utwórz:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Przedstawia transparent oferty z dopisem, że można utworzyć plan i wyświetlać dostępne plany.":::

- Gdy użytkownik wybierze niezatwierdzoną plan, na banerze zostanie zaaprobowany plan, a przycisk **Utwórz** zostanie wyłączony. Użytkownik może nadal poprosić o dodanie planu do listy zatwierdzonych (zobacz następną sekcję).

## <a name="request-to-add-offers-or-plans"></a>Żądanie dodania ofert lub planów

Możesz poprosić o dodanie publicznej oferty lub planu, który nie jest obecnie zatwierdzony w prywatnej Azure Marketplace.

1. Wybierz **pozycję Żądanie, aby** dodać na banerze, aby otworzyć formularz żądania **dostępu**.

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Wyświetla transparent z linkiem &quot;Request to add&quot; (Żądanie dodania).":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Przedstawia formularz żądania dostępu dla ofert lub planów.":::

1. Wybierz plany do dodania do żądania (dowolny **plan** informuje administratora witryny Marketplace, że nie masz preferencji planu w ramach oferty).

1. Dodaj uzasadnienie **i** wybierz **pozycję Żądanie,** aby przesłać żądanie.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Przedstawia formularz żądania dostępu dla ofert lub planów z przykładami wpisów.":::

1. Wskazanie oczekującego żądania pojawi się w formularzu Żądanie dostępu z opcją **Żądanie odszukania**.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Przedstawia listę zatwierdzonych lub oczekujących planów z linkiem Żądanie zmiany.":::

> [!NOTE]
> Po przesłaniu formularz żądania zatwierdzenia zostanie [](#private-azure-marketplace-notification-center) wysłany do Centrum powiadomień dla administratora witryny Marketplace w celu przejrzenia żądania i podjęcia działania.

> [!CAUTION]
> Zatwierdzenie w prywatnej witrynie Marketplace nie wskazuje zakupu rozwiązania.

## <a name="frequently-asked-questions-faqs"></a>Często zadawane pytania

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Blokujem już aplikację innej firmy w witrynie Marketplace za pośrednictwem Azure Policy. Czym się to różni?

Obecnie istnieją dwa sposoby ograniczania usług innych firm w witrynie Marketplace:

1. Za pośrednictwem witryny EA Portal Azure Portal wyłącz usługi innych firm lub ogranicz je do opcji "Tylko jednostki SKU bezpłatna lub BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Pokazuje, jak ograniczyć usługi w Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Pokazuje, jak ograniczyć usługi w portalu E A.":::

2. Utwórz zasady platformy Azure, aby zezwalać tylko na określone maszyny wirtualne. Aby uzyskać szczegółowe informacje na temat wymuszania zasad Windows wirtualnych, zobacz [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy)(Stosowanie zasad do maszyn wirtualnych przy użyciu Azure Resource Manager).

Prywatne Azure Marketplace zapewniają większą elastyczność ograniczania i zezwalania na określone oferty i plany. Informuje ona użytkowników końcowych o dostępności wdrożenia w galerii marketplace jeszcze przed podjęciem próby wdrożenia usług innych firm. Aby zezwolić na wdrażanie usług innych firm, ustaw Azure Marketplace na Wł./Włączone w EA Portal i Azure Portal.

- Prywatne Azure Marketplace mogą curować rozwiązania partnerskie, nie tylko maszyny wirtualne.
- Prywatne Azure Marketplace mogą być na poziomie planu i mogą również ustawiać "Bieżący i przyszły plan".
- Prywatne Azure Marketplace z góry informować użytkowników końcowych o tym, co można i czego nie można wdrożyć.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Jaka jest różnica między ofertą prywatną i prywatną Azure Marketplace?

Oferta **prywatna** umożliwia wydawcom tworzenie planów, które są widoczne tylko dla klientów docelowych. Dzięki temu mogą prywatnie udostępniać dostosowane rozwiązania z wynegocjowaną ceną, prywatnymi warunkami i postanowieniami oraz wyspecjalizowanymi konfiguracjami. Aby uzyskać szczegółowe informacje, [zobacz Private offers in the commercial marketplace (Oferty prywatne na platformie handlowej).](/azure/marketplace/private-offers)

**Prywatne Azure Marketplace** w Azure Portal umożliwiają administratorom wstępne zatwierdzanie rozwiązań innych firm, które użytkownicy mogą wdrażać. Dzięki prywatnej Azure Marketplace użytkownicy mogą korzystać z zalet usługi Azure Marketplace znajdowania, kupowania i wdrażania zgodnych ofert. Aby zarządzać ofertami prywatnymi opartymi na subskrypcji w prywatnej witrynie Marketplace, administrator witryny Marketplace musi mieć co najmniej rolę "odczyt" dla określonej subskrypcji.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Dodano ofertę prywatną do usługi Azure Marketplace, dlaczego nie jest ona pokazywana na karcie zarządzania platformą marketplace?

Oferty prywatne oparte na subskrypcji są widoczne tylko dla subskrypcji wymienionych w ustawieniach oferty prywatnej. Aby wyświetlić ofertę prywatną, upewnij się, że globalny filtr subskrypcji pokazuje wszystkie subskrypcje.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Wyświetla filtr prywatnej witryny Marketplace.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Czy można uwzględnić obrazy niestandardowe w prywatnych Azure Marketplace?

Nie. Zarządzanie Azure Marketplace umożliwia dowolnemu administratorowi IT zarządzanie rozwiązaniami innych firm i zarządzanie nimi z globalnej Azure Marketplace. Ponieważ obrazy niestandardowe nie znajdują się Azure Marketplace globalnej, administrator IT nie może wybrać obrazów niestandardowych. Jeśli chcesz udostępnić obrazy niestandardowe, użyj [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).

1. Przewodnik krok po kroku Tworzenie Shared Image Gallery (CLI,[](/azure/virtual-machines/shared-images-cli) [PowerShell).](/azure/virtual-machines/shared-images-powershell)
2. Utwórz definicję obrazu w obrębie funkcji SIG. Klient powinien wybrać **pozycję Uogólnione** dla pola Stan systemu operacyjnego. (interfejs[wiersza polecenia,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [program PowerShell).](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)
3. Przekieruj obraz zarządzany do Shared Image Gallery[(interfejs wiersza polecenia,](/azure/virtual-machines/image-version-managed-image-cli) [program PowerShell).](/azure/virtual-machines/image-version-managed-image-powershell)
4. Obrazy maszyn wirtualnych SIG znajdowały się w jednej subskrypcji. Aby udostępnić ją innym subskrypcjom, użyj rejestracji aplikacji (interfejs wiersza[polecenia,](/azure/virtual-machines/linux/share-images-across-tenants) [program PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Dlaczego niektóre oferty są domyślnie **zatwierdzone,** mimo że wydawcą nie jest firma Microsoft?

Firma Microsoft obsługuje system Linux i technologię open source na platformie Azure. [Zatwierdzone dystrybucje systemu Linux](/azure/virtual-machines/linux/endorsed-distros) są obsługiwane na platformie Azure, a cena jest zintegrowana z maszynami wirtualnymi. Ponieważ agent systemu Linux platformy Azure jest już wstępnie zainstalowany na Azure Marketplace, jest traktowany jak oferta firmy Microsoft. Ponieważ oferty firmy Microsoft są domyślnie zatwierdzane, zatwierdzonych dystrybucji systemu Linux nie można zarządzać w prywatnej Azure Marketplace i są domyślnie zatwierdzane.

## <a name="contact-support"></a>Kontakt z pomocą techniczną

- Aby uzyskać Azure Marketplace pomocy technicznej, odwiedź [stronę microsoft Q&A.](/answers/products/)