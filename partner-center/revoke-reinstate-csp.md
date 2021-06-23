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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Przywróć uprawnienia administratora dla subskrypcji Azure CSP klienta  

**Odpowiednie role:** Administrator globalny | Agent administracyjny

Jako Dostawca rozwiązań w chmurze (CSP), klienci często oczekują, że będziesz zarządzać ich użyciem platformy Azure i ich systemami. Musisz mieć do tego uprawnienia administratora. Niektóre uprawnienia są przyznawane, gdy relacja odsprzedawcy z klientem zostanie ustanowiona. Inne osoby są udzielane przez klienta.

## <a name="admin-privileges-for-azure-in-csp"></a>Uprawnienia administratora dla Platforma Azure w programie CSP

Istnieją dwa poziomy uprawnień administratora dla Platforma Azure w programie CSP.

- **Uprawnienia administratora na poziomie dzierżawy (delegowane uprawnienia administratora):** partnerzy programu CSP uzyskają te uprawnienia podczas ustanawiania relacji odsprzedawcy programu CSP z klientami. Delegowane uprawnienia administratora zapewniają partnerom programu CSP dostęp do dzierżaw ich klientów. Ten dostęp umożliwia im korzystanie z funkcji administracyjnych, takich jak dodawanie użytkowników i zarządzanie nimi, resetowanie haseł i zarządzanie licencjami użytkowników.
- **Uprawnienia administratora na poziomie subskrypcji:** partnerzy programu CSP uzyskają te uprawnienia podczas tworzenia Azure CSP subskrypcji dla swoich klientów. Te uprawnienia umożliwiają partnerom programu CSP pełny dostęp do tych subskrypcji, co pozwala im aprowizować zasoby platformy Azure i zarządzać nimi.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Przywróć uprawnienia administratora partnera w programie CSP

Klient może ponownie utworzyć przypisanie roli CSP, jeśli udostępnisz klientowi grupę `object ID` AdminAgents. Aby odzyskać delegowane uprawnienia administratora, musisz współpracować z klientem, aby wykonać następujące kroki.

1. Zaloguj się do pulpitu Partner Center nawigacyjnego.

2. W menu Partner Center wybierz pozycję **Klienci.**

3. Wybierz klienta, z który pracujesz, i **zażądaj relacji odsprzedawcy.** Ta akcja generuje link do klienta, który ma uprawnienia administratora dzierżawy.

4. Klient musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład tworzenia relacji odsprzedawcy w wiadomości e-mail.":::

5. Ty, partner, musisz nawiązać połączenie z dzierżawą partnera, aby uzyskać identyfikator obiektu grupy AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Następnie klient musi wykonać poniższe kroki przy użyciu programu PowerShell lub interfejsu wiersza polecenia platformy Azure. Klient musi mieć:

- Rola właściciela **lub** **administratora dostępu użytkowników** 
- Uprawnienia do tworzenia przypisań ról na poziomie subskrypcji

   a. Tylko w przypadku programu PowerShell klient musi zaktualizować `Az.Resources` moduł.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Klient łączy się z dzierżawą, w której istnieje subskrypcja CSP.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Klient łączy się z subskrypcją. Ma to *zastosowanie tylko* wtedy, gdy użytkownik ma uprawnienia do przypisywania ról w wielu subskrypcjach w dzierżawie.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Następnie klient tworzy przypisanie roli.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Zamiast udzielać uprawnień właściciela w zakresie subskrypcji, możesz udzielić uprawnień na poziomie grupy zasobów lub zasobu. 

- Na poziomie grupy zasobów

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Na poziomie zasobu

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Jeśli powyższe kroki nie działają lub występują błędy podczas próby ich uzyskania, spróbuj wykonać następującą procedurę "catch-all", aby przywrócić prawa administratora dla klienta.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Rozwiązywanie problemów

Jeśli klient nie może wykonać kroku 6 powyżej, niech spróbuje wykonać następujące polecenie:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Udostępnij wynikowy `newRoleAssignment.log` plik firmie Microsoft w celu dalszej analizy.

Jeśli procedura "catch-all" nie powiedzie się podczas `Import-Module` , spróbuj wykonać następujące czynności:
- Jeśli importowanie nie powiedzie się, ponieważ moduł jest w użyciu, uruchom ponownie sesję programu PowerShell, zamykając i ponownie otwierając wszystkie okna.
- Sprawdź wersję programu za `Az.Resources` pomocą . `Get-Module Az.Resources -ListAvailable`
- Jeśli wersja 4.1.1 nie znajduje się na liście dostępnych, należy użyć `Update-Module Az.Resources -Force` .
- Jeśli błąd będzie zawierał konkretną wersję, zaktualizuj również ten moduł, zastępując `Az.Accounts` wartość `Az.Resources` . `Az.Accounts` Następnie należy ponownie uruchomić sesję programu PowerShell.


## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
