---
title: Przywracanie uprawnień administratora w programie Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak pomóc klientom w przywróceniu uprawnień administratora partnera, dzięki czemu partner może pomóc w zarządzaniu subskrypcjami usługi Azure Dostawca rozwiązań w chmurze (CSP) klienta.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ec17a386e3ac6e9b41ce0582f0c55e424ce5e64
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128359435"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Przywróć uprawnienia administratora dla subskrypcji Azure CSP klienta  

**Odpowiednie role:** Administrator globalny | Agent administracyjny

Jako Dostawca rozwiązań w chmurze programu (CSP), klienci często polegają na Tym, że zarządzasz użyciem platformy Azure i ich systemami. Aby im pomóc, potrzebne są uprawnienia administratora. Jeśli nie masz jeszcze uprawnień administratora, możesz we współpracy z klientem przywrócić je.

## <a name="admin-privileges-for-azure-in-the-csp-program"></a>Uprawnienia administratora dla platformy Azure w programie CSP

Niektóre uprawnienia administratora są przyznawane automatycznie podczas ustanawiania relacji odsprzedawcy z klientem. Inne osoby muszą zostać ci przyznane przez klienta. Istnieją dwa poziomy uprawnień administratora dla Platforma Azure w programie CSP.

- **Uprawnienia administratora na poziomie dzierżawy (czyli delegowane** uprawnienia administratora) zapewniają dostęp do dzierżaw klientów. Ten dostęp umożliwia korzystanie z funkcji administracyjnych, takich jak dodawanie użytkowników i zarządzanie nimi, resetowanie haseł i zarządzanie licencjami użytkowników. Te uprawnienia można uzyskać podczas ustanawiania relacji odsprzedawcy CSP z klientami.
- **Uprawnienia administratora na poziomie subskrypcji** zapewniają pełny dostęp do subskrypcji Azure CSP klientów. Ten dostęp umożliwia aprowizować ich zasoby platformy Azure i zarządzać nimi. Te uprawnienia można uzyskać podczas tworzenia Azure CSP subskrypcji dla klientów.

## <a name="how-to-reinstate-your-csp-admin-privileges"></a>Jak przywrócić uprawnienia administratora programu CSP

Możesz współpracować z klientem, aby odzyskać delegowane uprawnienia administratora.

1. Zaloguj się do [pulpitu Partner Center nawigacyjnego.](https://partner.microsoft.com/dashboard)

2. Z menu Partner Center wybierz pozycję **Klienci.**

3. Wybierz klienta, z który pracujesz, i **zażądaj relacji odsprzedawcy.** Ta akcja wysyła wiadomość e-mail z linkiem do klienta.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład tworzenia relacji odsprzedawcy w wiadomości e-mail.":::

4. Gdy klient zatwierdzi żądanie relacji odsprzedawcy za pośrednictwem podanego linku, połącz się z dzierżawą partnera, aby uzyskać adres grupy `object ID` AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

5. Upewnij się, że klient ma:

   1. Rola właściciela **lub administratora** dostępu **użytkowników** 
   2. Uprawnienia do tworzenia przypisań ról na poziomie subskrypcji

6. Aby ukończyć ten proces, klient musi wykonać następujące czynności przy użyciu programu PowerShell lub interfejsu wiersza polecenia platformy Azure. 

   1. W przypadku korzystania z programu PowerShell klient musi zaktualizować `Az.Resources` moduł.

       ```powershell
       Update-Module Az.Resources
       ```

   2. Klient powinien połączyć się z dzierżawą, w której istnieje subskrypcja CSP.

      ```powershell
      Connect-AzAccount -TenantID "<Customer tenant>"
      ```

      ```azurecli
      az login --tenant <Customer tenant>
      ```

   3. Klient powinien następnie połączyć się z subskrypcją. Ma to *zastosowanie tylko* wtedy, gdy użytkownik ma uprawnienia do przypisywania ról w wielu subskrypcjach w dzierżawie.

      ```powershell
      Set-AzContext -SubscriptionID <"CSP Subscription ID">
      ```

      ```azurecli
      az account set --subscription <CSP Subscription ID>
      ```

   4. Klient może następnie utworzyć przypisanie roli.

      ```powershell
      New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
      ```

      ```azurecli
      az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>"
      ```

Zamiast udzielać uprawnień właściciela na poziomie subskrypcji, możesz udzielić im uprawnień na poziomie grupy zasobów lub zasobu: 

- Na poziomie grupy zasobów

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Na poziomie zasobu

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "<Resource URI>"
   ```

Jeśli powyższe kroki nie działają lub podczas próby ich próby występują błędy, spróbuj wykonać następującą procedurę "catch-all", aby przywrócić prawa administratora dla klienta:

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```
### <a name="troubleshooting"></a>Rozwiązywanie problemów
Jeśli klient nie może wykonać kroku 6, zasugeruj następujące polecenie i udostępnij wynikowy plik firmie Microsoft do `newRoleAssignment.log` dalszej analizy:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Jeśli procedura "catch-all" nie powiedzie się podczas `Import-Module` , spróbuj wykonać następujące czynności:
- Jeśli importowanie nie powiedzie się, ponieważ moduł jest w użyciu, uruchom ponownie sesję programu PowerShell, zamykając i ponownie otwierając wszystkie okna.
- Sprawdź wersję programu za `Az.Resources` pomocą . `Get-Module Az.Resources -ListAvailable`
- Jeśli wersja 4.1.1 nie znajduje się na liście dostępnych, należy `Update-Module Az.Resources -Force` użyć .
- Jeśli w błędzie zostanie określony stan, który musi być określoną wersją, zaktualizuj również ten moduł, zastępując `Az.Accounts` `Az.Resources` wartość . `Az.Accounts` Następnie należy ponownie uruchomić sesję programu PowerShell.


## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
