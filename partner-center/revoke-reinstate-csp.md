---
title: Przywróć uprawnienia administratora dla Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak pomóc klientom w przywróceniu uprawnień administratora partnera, aby pomóc partnerowi w zarządzaniu subskrypcjami Azure Cloud Solution Provider (CSP).
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d784aef33cce2a722583a77e73c35d5fc8136b1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551592"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="7fce2-103">Przywróć uprawnienia administratora dla subskrypcji Azure CSP klienta</span><span class="sxs-lookup"><span data-stu-id="7fce2-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="7fce2-104">**Odpowiednie role:** Administrator globalny | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="7fce2-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="7fce2-105">Jako Dostawca rozwiązań w chmurze (CSP), klienci często oczekują, że będziesz zarządzać ich użyciem platformy Azure i ich systemami.</span><span class="sxs-lookup"><span data-stu-id="7fce2-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="7fce2-106">Musisz mieć do tego uprawnienia administratora.</span><span class="sxs-lookup"><span data-stu-id="7fce2-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="7fce2-107">Niektóre uprawnienia są przyznawane, gdy relacja odsprzedawcy z klientem zostanie ustanowiona.</span><span class="sxs-lookup"><span data-stu-id="7fce2-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="7fce2-108">Inne osoby są udzielane przez klienta.</span><span class="sxs-lookup"><span data-stu-id="7fce2-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="7fce2-109">Uprawnienia administratora dla Platforma Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="7fce2-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="7fce2-110">Istnieją dwa poziomy uprawnień administratora dla Platforma Azure w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="7fce2-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="7fce2-111">**Uprawnienia administratora na poziomie dzierżawy (delegowane uprawnienia administratora):** partnerzy programu CSP uzyskają te uprawnienia podczas ustanawiania relacji odsprzedawcy programu CSP z klientami.</span><span class="sxs-lookup"><span data-stu-id="7fce2-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="7fce2-112">Delegowane uprawnienia administratora zapewniają partnerom programu CSP dostęp do dzierżaw ich klientów.</span><span class="sxs-lookup"><span data-stu-id="7fce2-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="7fce2-113">Ten dostęp umożliwia im korzystanie z funkcji administracyjnych, takich jak dodawanie użytkowników i zarządzanie nimi, resetowanie haseł i zarządzanie licencjami użytkowników.</span><span class="sxs-lookup"><span data-stu-id="7fce2-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="7fce2-114">**Uprawnienia administratora na poziomie subskrypcji:** partnerzy programu CSP uzyskają te uprawnienia podczas tworzenia Azure CSP subskrypcji dla swoich klientów.</span><span class="sxs-lookup"><span data-stu-id="7fce2-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="7fce2-115">Te uprawnienia umożliwiają partnerom programu CSP pełny dostęp do tych subskrypcji, co pozwala im aprowizować zasoby platformy Azure i zarządzać nimi.</span><span class="sxs-lookup"><span data-stu-id="7fce2-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="7fce2-116">Przywróć uprawnienia administratora partnera w programie CSP</span><span class="sxs-lookup"><span data-stu-id="7fce2-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="7fce2-117">Klient może ponownie utworzyć przypisanie roli CSP, jeśli udostępnisz klientowi grupę `object ID` AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="7fce2-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="7fce2-118">Aby odzyskać delegowane uprawnienia administratora, musisz współpracować z klientem, aby wykonać następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="7fce2-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="7fce2-119">Zaloguj się do pulpitu Partner Center nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="7fce2-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="7fce2-120">W menu Partner Center wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="7fce2-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="7fce2-121">Wybierz klienta, z który pracujesz, i **zażądaj relacji odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="7fce2-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="7fce2-122">Ta akcja generuje link do klienta, który ma uprawnienia administratora dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="7fce2-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="7fce2-123">Klient musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="7fce2-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład tworzenia relacji odsprzedawcy w wiadomości e-mail.":::

5. <span data-ttu-id="7fce2-125">Ty, partner, musisz nawiązać połączenie z dzierżawą partnera, aby uzyskać identyfikator obiektu grupy AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="7fce2-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="7fce2-126">Następnie klient musi wykonać poniższe kroki przy użyciu programu PowerShell lub interfejsu wiersza polecenia platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="7fce2-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="7fce2-127">Klient musi mieć:</span><span class="sxs-lookup"><span data-stu-id="7fce2-127">Your customer must have:</span></span>

- <span data-ttu-id="7fce2-128">Rola właściciela **lub** **administratora dostępu użytkowników**</span><span class="sxs-lookup"><span data-stu-id="7fce2-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="7fce2-129">Uprawnienia do tworzenia przypisań ról na poziomie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="7fce2-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="7fce2-130">a.</span><span class="sxs-lookup"><span data-stu-id="7fce2-130">a.</span></span> <span data-ttu-id="7fce2-131">Tylko w przypadku programu PowerShell klient musi zaktualizować `Az.Resources` moduł.</span><span class="sxs-lookup"><span data-stu-id="7fce2-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="7fce2-132">b.</span><span class="sxs-lookup"><span data-stu-id="7fce2-132">b.</span></span> <span data-ttu-id="7fce2-133">Klient łączy się z dzierżawą, w której istnieje subskrypcja CSP.</span><span class="sxs-lookup"><span data-stu-id="7fce2-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="7fce2-134">c.</span><span class="sxs-lookup"><span data-stu-id="7fce2-134">c.</span></span> <span data-ttu-id="7fce2-135">Klient łączy się z subskrypcją.</span><span class="sxs-lookup"><span data-stu-id="7fce2-135">The customer connects to the subscription.</span></span> <span data-ttu-id="7fce2-136">Ma to *zastosowanie tylko* wtedy, gdy użytkownik ma uprawnienia do przypisywania ról w wielu subskrypcjach w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="7fce2-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="7fce2-137">d.</span><span class="sxs-lookup"><span data-stu-id="7fce2-137">d.</span></span> <span data-ttu-id="7fce2-138">Następnie klient tworzy przypisanie roli.</span><span class="sxs-lookup"><span data-stu-id="7fce2-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="7fce2-139">Zamiast udzielać uprawnień właściciela w zakresie subskrypcji, możesz udzielić uprawnień na poziomie grupy zasobów lub zasobu.</span><span class="sxs-lookup"><span data-stu-id="7fce2-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="7fce2-140">Na poziomie grupy zasobów</span><span class="sxs-lookup"><span data-stu-id="7fce2-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="7fce2-141">Na poziomie zasobu</span><span class="sxs-lookup"><span data-stu-id="7fce2-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="7fce2-142">Jeśli powyższe kroki nie działają lub występują błędy podczas próby ich uzyskania, spróbuj wykonać następującą procedurę "catch-all", aby przywrócić prawa administratora dla klienta.</span><span class="sxs-lookup"><span data-stu-id="7fce2-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="7fce2-143">Rozwiązywanie problemów</span><span class="sxs-lookup"><span data-stu-id="7fce2-143">Troubleshooting</span></span>

<span data-ttu-id="7fce2-144">Jeśli klient nie może wykonać kroku 6 powyżej, niech spróbuje wykonać następujące polecenie:</span><span class="sxs-lookup"><span data-stu-id="7fce2-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="7fce2-145">Udostępnij wynikowy `newRoleAssignment.log` plik firmie Microsoft w celu dalszej analizy.</span><span class="sxs-lookup"><span data-stu-id="7fce2-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="7fce2-146">Jeśli procedura "catch-all" nie powiedzie się podczas `Import-Module` , spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="7fce2-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="7fce2-147">Jeśli importowanie nie powiedzie się, ponieważ moduł jest w użyciu, uruchom ponownie sesję programu PowerShell, zamykając i ponownie otwierając wszystkie okna.</span><span class="sxs-lookup"><span data-stu-id="7fce2-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="7fce2-148">Sprawdź wersję programu za `Az.Resources` pomocą . `Get-Module Az.Resources -ListAvailable`</span><span class="sxs-lookup"><span data-stu-id="7fce2-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="7fce2-149">Jeśli wersja 4.1.1 nie znajduje się na liście dostępnych, należy użyć `Update-Module Az.Resources -Force` .</span><span class="sxs-lookup"><span data-stu-id="7fce2-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="7fce2-150">Jeśli błąd będzie zawierał konkretną wersję, zaktualizuj również ten moduł, zastępując `Az.Accounts` wartość `Az.Resources` . `Az.Accounts`</span><span class="sxs-lookup"><span data-stu-id="7fce2-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="7fce2-151">Następnie należy ponownie uruchomić sesję programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7fce2-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="7fce2-152">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="7fce2-152">Next steps</span></span>

- [<span data-ttu-id="7fce2-153">Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="7fce2-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
