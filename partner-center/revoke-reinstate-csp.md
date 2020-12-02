---
title: Przywracanie uprawnień administratora dla programu CSP platformy Azure
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak pomóc klientom w przywracaniu uprawnień administratora partnera, aby partner mógł pomóc w zarządzaniu subskrypcjami CSP dostawcy platformy Azure.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c694f48fb62fc031bfaf78be6a1c4e43629a7adb
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2020
ms.locfileid: "92529498"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Przywracanie uprawnień administratora dla subskrypcji dostawcy CSP platformy Azure klienta  

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny

Jako partner programu CSP klienci często oczekują, że będziesz zarządzać użyciem platformy Azure i ich systemami. Wykonanie tej czynności wymaga uprawnień administratora. Niektóre uprawnienia są przyznawane w przypadku ustanowienia relacji odsprzedawcy z klientem. Inne osoby są udzielane użytkownikowi przez klienta.

## <a name="admin-privileges-for-azure-in-csp"></a>Uprawnienia administratora platformy Azure w programie CSP

Istnieją dwa poziomy uprawnień administratora dla platformy Azure w programie CSP.

**Uprawnienia administratora na poziomie dzierżawy** (**uprawnienia administratora delegowanego**) — partnerzy CSP uzyskują te uprawnienia podczas ustanawiania relacji odsprzedawcy dostawcy CSP z klientami. Zapewnia to partnerom CSP dostęp do dzierżawców klientów, co umożliwia im wykonywanie funkcji administracyjnych, takich jak dodawanie/zarządzanie użytkownikami, resetowanie haseł i zarządzanie licencjami użytkowników.

**Uprawnienia administratora na poziomie subskrypcji** — partnerzy programu CSP uzyskują te uprawnienia podczas tworzenia subskrypcji dostawcy usług kryptograficznych platformy Azure dla swoich klientów. Posiadanie tych uprawnień zapewnia partnerom CSP pełny dostęp do tych subskrypcji, co umożliwia im udostępnianie zasobów platformy Azure i zarządzanie nimi.

## <a name="reinstate-csp-partners-admin-privileges"></a>Przywracanie uprawnień administratora partnerów CSP

Aby odzyskać uprawnienia administratora delegowanego, musisz skontaktować się z klientem.

1. Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego i w menu Centrum partnerskiego wybierz pozycję **klienci**.

2. Wybierz klienta, z którym pracujesz, i **Zażądaj relacji odsprzedawcy.** Spowoduje to wygenerowanie linku do klienta z uprawnieniami administratora dzierżawy.

3. Użytkownik musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Relacja odsprzedawcy":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Dodawanie grupy agentów administracyjnych jako właściciela subskrypcji CSP platformy Azure

Klient będzie musiał dodać grupę agentów administracyjnych jako właściciela subskrypcji dostawcy CSP platformy Azure.

1. Użyj konsoli programu PowerShell lub środowiska PowerShell Integrated Scripting Environment (ISE). Upewnij się, że moduły AzureAD są zainstalowane.

2. Nawiąż połączenie z dzierżawą usługi Azure AD.

   ```powershell
   Connect-AzureAD
   ```

3. Uzyskaj identyfikator ObjectId grup agentów administracyjnych.

   ```powershell
   Get-AzureADGroup
   ```
   Następujące kroki są wykonywane przez użytkownika w firmie klienta, który ma dostęp właściciela do subskrypcji dostawcy CSP platformy Azure.

4. Użytkownik z dostępem właściciela do subskrypcji CSP platformy Azure loguje się do platformy Azure przy użyciu swoich poświadczeń.

   ```powershell
   Connect-AzAccount
   ```

5. Następnie może dodać grupę agentów administracyjnych jako właściciela do subskrypcji platformy Azure dostawcy CSP.

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a>Następne kroki

[Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure](azure-plan-manage.md)
