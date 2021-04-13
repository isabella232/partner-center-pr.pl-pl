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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="97522-103">Przywracanie uprawnień administratora dla subskrypcji dostawcy CSP platformy Azure klienta</span><span class="sxs-lookup"><span data-stu-id="97522-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="97522-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="97522-104">**Applicable roles**</span></span>

- <span data-ttu-id="97522-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="97522-105">Global admin</span></span>
- <span data-ttu-id="97522-106">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="97522-106">Admin agent</span></span>

<span data-ttu-id="97522-107">Jako partner programu CSP klienci często oczekują, że będziesz zarządzać użyciem platformy Azure i ich systemami.</span><span class="sxs-lookup"><span data-stu-id="97522-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="97522-108">Wykonanie tej czynności wymaga uprawnień administratora.</span><span class="sxs-lookup"><span data-stu-id="97522-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="97522-109">Niektóre uprawnienia są udzielane w przypadku ustanowienia relacji odsprzedawcy z klientem.</span><span class="sxs-lookup"><span data-stu-id="97522-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="97522-110">Inne osoby są udzielane użytkownikowi przez klienta.</span><span class="sxs-lookup"><span data-stu-id="97522-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="97522-111">Uprawnienia administratora platformy Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="97522-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="97522-112">Istnieją dwa poziomy uprawnień administratora dla platformy Azure w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="97522-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="97522-113">**Uprawnienia administratora na poziomie dzierżawy** (**uprawnienia administratora delegowanego**) — partnerzy CSP uzyskują te uprawnienia podczas ustanawiania relacji odsprzedawcy dostawcy CSP z klientami.</span><span class="sxs-lookup"><span data-stu-id="97522-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="97522-114">Uprawnienia administratora delegowanego umożliwiają partnerom CSP dostęp do dzierżawców klientów, co umożliwia im wykonywanie funkcji administracyjnych, takich jak dodawanie/zarządzanie użytkownikami, resetowanie haseł i zarządzanie licencjami użytkowników.</span><span class="sxs-lookup"><span data-stu-id="97522-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="97522-115">**Uprawnienia administratora na poziomie subskrypcji** — partnerzy programu CSP uzyskują te uprawnienia podczas tworzenia subskrypcji dostawcy usług kryptograficznych platformy Azure dla swoich klientów.</span><span class="sxs-lookup"><span data-stu-id="97522-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="97522-116">Posiadanie tych uprawnień zapewnia partnerom CSP pełny dostęp do tych subskrypcji, co umożliwia im udostępnianie zasobów platformy Azure i zarządzanie nimi.</span><span class="sxs-lookup"><span data-stu-id="97522-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="97522-117">Przywracanie uprawnień administratora partnerów CSP</span><span class="sxs-lookup"><span data-stu-id="97522-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="97522-118">Klient może ponownie utworzyć przypisanie roli dostawcy usług kryptograficznych, o ile podano identyfikator obiektu grupy AdminAgents dla klienta.</span><span class="sxs-lookup"><span data-stu-id="97522-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="97522-119">Aby odzyskać uprawnienia administratora delegowanego, musisz skontaktować się z klientem.</span><span class="sxs-lookup"><span data-stu-id="97522-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="97522-120">Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego i w menu Centrum partnerskiego wybierz pozycję **klienci**.</span><span class="sxs-lookup"><span data-stu-id="97522-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="97522-121">Wybierz klienta, z którym pracujesz, i **Zażądaj relacji odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="97522-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="97522-122">Spowoduje to wygenerowanie linku do klienta z uprawnieniami administratora dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="97522-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="97522-123">Ten klient musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="97522-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład wiadomości e-mail dotyczącej tworzenia relacji odsprzedawcy":::

4. <span data-ttu-id="97522-125">Partner musi połączyć się z dzierżawcą partnera, aby uzyskać identyfikator obiektu grupy AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="97522-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="97522-126">Klient, który ma rolę **właściciela lub administratora dostępu użytkowników** i ma uprawnienia do tworzenia przypisania roli na poziomie subskrypcji, wykonuje następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="97522-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="97522-127">Nawiązuje połączenie z dzierżawą, w której istnieje subskrypcja dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="97522-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="97522-128">Nawiązuje połączenie z subskrypcją (dotyczy tylko sytuacji, gdy użytkownik ma uprawnienia do przypisywania ról w ramach wielu subskrypcji w dzierżawie).</span><span class="sxs-lookup"><span data-stu-id="97522-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="97522-129">PS C:\WINDOWS\system32> Set-AzContext-subskrypcji CSP o IDENTYFIKATORze ""</span><span class="sxs-lookup"><span data-stu-id="97522-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="97522-130">Tworzy przypisanie roli</span><span class="sxs-lookup"><span data-stu-id="97522-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="97522-131">Jeśli wolisz przyznać uprawnienia roli właściciela na poziomie grupy zasobów lub poziomu zasobów zamiast zakresu subskrypcji, następujące polecenia mogą obsłużyć:</span><span class="sxs-lookup"><span data-stu-id="97522-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="97522-132">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="97522-132">Next steps</span></span>

- [<span data-ttu-id="97522-133">Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="97522-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
