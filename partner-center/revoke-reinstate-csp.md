---
title: Przywróć uprawnienia administratora dla Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak pomóc klientom w przywróceniu uprawnień administratora partnera, dzięki czemu partner może pomóc w zarządzaniu subskrypcjami Azure CSP klienta.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ca4c8323562e6c6f1d762465cad86e7ae113eb19
ms.sourcegitcommit: beba696954b62ab5396a893d050d0c2c211aeafc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/28/2021
ms.locfileid: "110601430"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="56556-103">Przywróć uprawnienia administratora dla subskrypcji Azure CSP klienta</span><span class="sxs-lookup"><span data-stu-id="56556-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="56556-104">**Odpowiednie role:** Administrator globalny | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="56556-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="56556-105">Jako partner CSP klienci często oczekują, że będziesz zarządzać ich użyciem platformy Azure i ich systemami.</span><span class="sxs-lookup"><span data-stu-id="56556-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="56556-106">Musisz mieć do tego uprawnienia administratora.</span><span class="sxs-lookup"><span data-stu-id="56556-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="56556-107">Niektóre uprawnienia są przyznawane, gdy relacja odsprzedawcy z klientem zostanie ustanowiona.</span><span class="sxs-lookup"><span data-stu-id="56556-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="56556-108">Inne osoby są udzielane przez klienta.</span><span class="sxs-lookup"><span data-stu-id="56556-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="56556-109">Uprawnienia administratora dla Platforma Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="56556-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="56556-110">Istnieją dwa poziomy uprawnień administratora dla Platforma Azure w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="56556-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="56556-111">**Uprawnienia administratora na poziomie dzierżawy (delegowane uprawnienia administratora):** partnerzy programu CSP uzyskają te uprawnienia podczas ustanawiania relacji odsprzedawcy programu CSP z klientami.</span><span class="sxs-lookup"><span data-stu-id="56556-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="56556-112">Delegowane uprawnienia administratora zapewniają partnerom programu CSP dostęp do dzierżaw ich klientów.</span><span class="sxs-lookup"><span data-stu-id="56556-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="56556-113">Ten dostęp umożliwia im korzystanie z funkcji administracyjnych, takich jak dodawanie użytkowników i zarządzanie nimi, resetowanie haseł i zarządzanie licencjami użytkowników.</span><span class="sxs-lookup"><span data-stu-id="56556-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="56556-114">**Uprawnienia administratora na poziomie subskrypcji:** partnerzy programu CSP uzyskają te uprawnienia podczas tworzenia Azure CSP subskrypcji dla swoich klientów.</span><span class="sxs-lookup"><span data-stu-id="56556-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="56556-115">Te uprawnienia umożliwiają partnerom programu CSP pełny dostęp do tych subskrypcji, co pozwala im aprowizować zasoby platformy Azure i zarządzać nimi.</span><span class="sxs-lookup"><span data-stu-id="56556-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="56556-116">Przywróć uprawnienia administratora partnera w programie CSP</span><span class="sxs-lookup"><span data-stu-id="56556-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="56556-117">Klient może ponownie utworzyć przypisanie roli CSP, jeśli udostępnisz klientowi grupę `object ID` AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="56556-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="56556-118">Aby odzyskać delegowane uprawnienia administratora, musisz współpracować z klientem, aby wykonać następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="56556-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="56556-119">Zaloguj się do pulpitu Partner Center nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="56556-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="56556-120">W menu Partner Center wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="56556-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="56556-121">Wybierz klienta, z który pracujesz, **i zażądaj relacji odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="56556-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="56556-122">Ta akcja generuje link do klienta, który ma uprawnienia administratora dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="56556-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="56556-123">Klient musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="56556-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład tworzenia relacji odsprzedawcy w wiadomości e-mail":::

5. <span data-ttu-id="56556-125">Ty, partner, musisz nawiązać połączenie z dzierżawą partnera, aby uzyskać identyfikator obiektu grupy AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="56556-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="56556-126">Klient musi następnie wykonać poniższe kroki przy użyciu programu PowerShell lub interfejsu wiersza polecenia platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="56556-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="56556-127">Klient musi mieć:</span><span class="sxs-lookup"><span data-stu-id="56556-127">Your customer must have:</span></span>

- <span data-ttu-id="56556-128">Rola właściciela **lub administratora** dostępu **użytkowników**</span><span class="sxs-lookup"><span data-stu-id="56556-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="56556-129">Uprawnienia do tworzenia przypisań ról na poziomie subskrypcji</span><span class="sxs-lookup"><span data-stu-id="56556-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="56556-130">a.</span><span class="sxs-lookup"><span data-stu-id="56556-130">a.</span></span> <span data-ttu-id="56556-131">Tylko w przypadku programu PowerShell klient musi zaktualizować `Az.Resources` moduł.</span><span class="sxs-lookup"><span data-stu-id="56556-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="56556-132">b.</span><span class="sxs-lookup"><span data-stu-id="56556-132">b.</span></span> <span data-ttu-id="56556-133">Klient łączy się z dzierżawą, w której istnieje subskrypcja CSP.</span><span class="sxs-lookup"><span data-stu-id="56556-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="56556-134">c.</span><span class="sxs-lookup"><span data-stu-id="56556-134">c.</span></span> <span data-ttu-id="56556-135">Klient łączy się z subskrypcją.</span><span class="sxs-lookup"><span data-stu-id="56556-135">The customer connects to the subscription.</span></span> <span data-ttu-id="56556-136">Ma to *zastosowanie tylko* wtedy, gdy użytkownik ma uprawnienia do przypisywania ról w wielu subskrypcjach w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="56556-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="56556-137">d.</span><span class="sxs-lookup"><span data-stu-id="56556-137">d.</span></span> <span data-ttu-id="56556-138">Następnie klient tworzy przypisanie roli.</span><span class="sxs-lookup"><span data-stu-id="56556-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="56556-139">Zamiast udzielać uprawnień właściciela w zakresie subskrypcji, możesz udzielić uprawnień na poziomie grupy zasobów lub zasobu.</span><span class="sxs-lookup"><span data-stu-id="56556-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="56556-140">Na poziomie grupy zasobów</span><span class="sxs-lookup"><span data-stu-id="56556-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="56556-141">Na poziomie zasobu</span><span class="sxs-lookup"><span data-stu-id="56556-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

## <a name="next-steps"></a><span data-ttu-id="56556-142">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="56556-142">Next steps</span></span>

- [<span data-ttu-id="56556-143">Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="56556-143">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
