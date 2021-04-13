---
title: Przywracanie uprawnień administratora dla programu CSP platformy Azure
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak pomóc klientom w przywracaniu uprawnień administratora partnera, aby partner mógł pomóc w zarządzaniu subskrypcjami CSP dostawcy platformy Azure.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315851"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Przywracanie uprawnień administratora dla subskrypcji dostawcy CSP platformy Azure klienta  

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny

Jako partner programu CSP klienci często oczekują, że będziesz zarządzać użyciem platformy Azure i ich systemami. Wykonanie tej czynności wymaga uprawnień administratora. Niektóre uprawnienia są udzielane w przypadku ustanowienia relacji odsprzedawcy z klientem. Inne osoby są udzielane użytkownikowi przez klienta.

## <a name="admin-privileges-for-azure-in-csp"></a>Uprawnienia administratora platformy Azure w programie CSP

Istnieją dwa poziomy uprawnień administratora dla platformy Azure w programie CSP.

**Uprawnienia administratora na poziomie dzierżawy** (**uprawnienia administratora delegowanego**) — partnerzy CSP uzyskują te uprawnienia podczas ustanawiania relacji odsprzedawcy dostawcy CSP z klientami. Uprawnienia administratora delegowanego umożliwiają partnerom CSP dostęp do dzierżawców klientów, co umożliwia im wykonywanie funkcji administracyjnych, takich jak dodawanie/zarządzanie użytkownikami, resetowanie haseł i zarządzanie licencjami użytkowników.

**Uprawnienia administratora na poziomie subskrypcji** — partnerzy programu CSP uzyskują te uprawnienia podczas tworzenia subskrypcji dostawcy usług kryptograficznych platformy Azure dla swoich klientów. Posiadanie tych uprawnień zapewnia partnerom CSP pełny dostęp do tych subskrypcji, co umożliwia im udostępnianie zasobów platformy Azure i zarządzanie nimi.

## <a name="reinstate-csp-partners-admin-privileges"></a>Przywracanie uprawnień administratora partnerów CSP

Klient może ponownie utworzyć przypisanie roli dostawcy usług kryptograficznych, o ile podano identyfikator obiektu grupy AdminAgents dla klienta. Aby odzyskać uprawnienia administratora delegowanego, musisz skontaktować się z klientem.

1. Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego i w menu Centrum partnerskiego wybierz pozycję **klienci**.

2. Wybierz klienta, z którym pracujesz, i **Zażądaj relacji odsprzedawcy.** Spowoduje to wygenerowanie linku do klienta z uprawnieniami administratora dzierżawy.

3. Ten klient musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład wiadomości e-mail dotyczącej tworzenia relacji odsprzedawcy":::

4. Partner musi połączyć się z dzierżawcą partnera, aby uzyskać identyfikator obiektu grupy AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Klient, który ma rolę **właściciela lub administratora dostępu użytkowników** i ma uprawnienia do tworzenia przypisania roli na poziomie subskrypcji, wykonuje następujące czynności:


    1. Nawiązuje połączenie z dzierżawą, w której istnieje subskrypcja dostawcy usług kryptograficznych.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Nawiązuje połączenie z subskrypcją (dotyczy tylko sytuacji, gdy użytkownik ma uprawnienia do przypisywania ról w ramach wielu subskrypcji w dzierżawie).
   
         PS C:\WINDOWS\system32> Set-AzContext-subskrypcji CSP o IDENTYFIKATORze ""


    3. Tworzy przypisanie roli
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Jeśli wolisz przyznać uprawnienia roli właściciela na poziomie grupy zasobów lub poziomu zasobów zamiast zakresu subskrypcji, następujące polecenia mogą obsłużyć:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
