---
title: Przywróć uprawnienia administratora dla Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak pomóc klientom w przywróceniu uprawnień administratora partnera, dzięki czemu partner może pomóc w zarządzaniu subskrypcjami Azure CSP klienta.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855424"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Przywróć uprawnienia administratora dla subskrypcji Azure CSP klienta  

**Odpowiednie role:** Administrator globalny | Agent administracyjny

Jako partner CSP klienci często oczekują, że będziesz zarządzać ich użyciem platformy Azure i ich systemami. Wymaga to uprawnień administratora. Niektóre uprawnienia są przyznawane, gdy relacja odsprzedawcy z klientem zostanie ustanowiona. Inne osoby są przyznawane przez klienta.

## <a name="admin-privileges-for-azure-in-csp"></a>Uprawnienia administratora dla Platforma Azure w programie CSP

Istnieją dwa poziomy uprawnień administratora dla Platforma Azure w programie CSP.

**Uprawnienia administratora na poziomie dzierżawy** **(delegowane uprawnienia** administratora) — partnerzy programu CSP uzyskają te uprawnienia podczas ustanawiania relacji odsprzedawcy programu CSP z klientami. Delegowane uprawnienia administratora zapewniają partnerom programu CSP dostęp do dzierżaw ich klientów, co umożliwia im wykonywanie funkcji administracyjnych, takich jak dodawanie użytkowników i zarządzanie nimi, resetowanie haseł i zarządzanie licencjami użytkowników.

**Uprawnienia administratora na poziomie subskrypcji** — partnerzy programu CSP uzyskają te uprawnienia podczas tworzenia Azure CSP subskrypcji dla swoich klientów. Te uprawnienia dają partnerom programu CSP pełny dostęp do tych subskrypcji, co pozwala im aprowizować zasoby platformy Azure i zarządzać nimi.

## <a name="reinstate-csp-partners-admin-privileges"></a>Przywróć uprawnienia administratora partnerów programu CSP

Klient może ponownie utworzyć przypisanie roli CSP, o ile podaniu klientowi identyfikatora obiektu grupy AdminAgents. Aby odzyskać delegowane uprawnienia administratora, musisz współpracować z klientem.

1. Zaloguj się do pulpitu Partner Center nawigacyjnego, a następnie z menu Partner Center wybierz pozycję **Klienci.**

2. Wybierz klienta, z który pracujesz, i **zażądaj relacji odsprzedawcy.** Ta akcja generuje link do klienta, który ma uprawnienia administratora dzierżawy.

3. Ten klient musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład tworzenia relacji odsprzedawcy w wiadomości e-mail":::

4. Ty, partner, musisz nawiązać połączenie z dzierżawą partnera, aby uzyskać identyfikator obiektu grupy AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Klient, który ma  rolę właściciela lub administratora dostępu użytkowników i ma uprawnienia do tworzenia przypisania roli na poziomie subskrypcji, robi następujące czynności:


    1. Nawiązuje połączenie z dzierżawą, w której istnieje subskrypcja CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Nawiązuje połączenie z subskrypcją (ma zastosowanie tylko wtedy, gdy użytkownik ma uprawnienia do przypisywania ról w wielu subskrypcjach w dzierżawie).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "Identyfikator subskrypcji CSP"'


    3. Tworzy przypisanie roli
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Jeśli chcesz przyznać uprawnienia roli właściciela na poziomie grupy zasobów lub zasobu zamiast w zakresie subskrypcji, następujące polecenia mogą działać:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Następne kroki

- [Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
