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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="244ce-103">Przywróć uprawnienia administratora dla subskrypcji Azure CSP klienta</span><span class="sxs-lookup"><span data-stu-id="244ce-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="244ce-104">**Odpowiednie role:** Administrator globalny | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="244ce-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="244ce-105">Jako partner CSP klienci często oczekują, że będziesz zarządzać ich użyciem platformy Azure i ich systemami.</span><span class="sxs-lookup"><span data-stu-id="244ce-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="244ce-106">Wymaga to uprawnień administratora.</span><span class="sxs-lookup"><span data-stu-id="244ce-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="244ce-107">Niektóre uprawnienia są przyznawane, gdy relacja odsprzedawcy z klientem zostanie ustanowiona.</span><span class="sxs-lookup"><span data-stu-id="244ce-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="244ce-108">Inne osoby są przyznawane przez klienta.</span><span class="sxs-lookup"><span data-stu-id="244ce-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="244ce-109">Uprawnienia administratora dla Platforma Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="244ce-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="244ce-110">Istnieją dwa poziomy uprawnień administratora dla Platforma Azure w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="244ce-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="244ce-111">**Uprawnienia administratora na poziomie dzierżawy** **(delegowane uprawnienia** administratora) — partnerzy programu CSP uzyskają te uprawnienia podczas ustanawiania relacji odsprzedawcy programu CSP z klientami.</span><span class="sxs-lookup"><span data-stu-id="244ce-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="244ce-112">Delegowane uprawnienia administratora zapewniają partnerom programu CSP dostęp do dzierżaw ich klientów, co umożliwia im wykonywanie funkcji administracyjnych, takich jak dodawanie użytkowników i zarządzanie nimi, resetowanie haseł i zarządzanie licencjami użytkowników.</span><span class="sxs-lookup"><span data-stu-id="244ce-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="244ce-113">**Uprawnienia administratora na poziomie subskrypcji** — partnerzy programu CSP uzyskają te uprawnienia podczas tworzenia Azure CSP subskrypcji dla swoich klientów.</span><span class="sxs-lookup"><span data-stu-id="244ce-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="244ce-114">Te uprawnienia dają partnerom programu CSP pełny dostęp do tych subskrypcji, co pozwala im aprowizować zasoby platformy Azure i zarządzać nimi.</span><span class="sxs-lookup"><span data-stu-id="244ce-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="244ce-115">Przywróć uprawnienia administratora partnerów programu CSP</span><span class="sxs-lookup"><span data-stu-id="244ce-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="244ce-116">Klient może ponownie utworzyć przypisanie roli CSP, o ile podaniu klientowi identyfikatora obiektu grupy AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="244ce-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="244ce-117">Aby odzyskać delegowane uprawnienia administratora, musisz współpracować z klientem.</span><span class="sxs-lookup"><span data-stu-id="244ce-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="244ce-118">Zaloguj się do pulpitu Partner Center nawigacyjnego, a następnie z menu Partner Center wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="244ce-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="244ce-119">Wybierz klienta, z który pracujesz, i **zażądaj relacji odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="244ce-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="244ce-120">Ta akcja generuje link do klienta, który ma uprawnienia administratora dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="244ce-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="244ce-121">Ten klient musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="244ce-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Przykład tworzenia relacji odsprzedawcy w wiadomości e-mail":::

4. <span data-ttu-id="244ce-123">Ty, partner, musisz nawiązać połączenie z dzierżawą partnera, aby uzyskać identyfikator obiektu grupy AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="244ce-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="244ce-124">Klient, który ma  rolę właściciela lub administratora dostępu użytkowników i ma uprawnienia do tworzenia przypisania roli na poziomie subskrypcji, robi następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="244ce-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="244ce-125">Nawiązuje połączenie z dzierżawą, w której istnieje subskrypcja CSP.</span><span class="sxs-lookup"><span data-stu-id="244ce-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="244ce-126">Nawiązuje połączenie z subskrypcją (ma zastosowanie tylko wtedy, gdy użytkownik ma uprawnienia do przypisywania ról w wielu subskrypcjach w dzierżawie).</span><span class="sxs-lookup"><span data-stu-id="244ce-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="244ce-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "Identyfikator subskrypcji CSP"'</span><span class="sxs-lookup"><span data-stu-id="244ce-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="244ce-128">Tworzy przypisanie roli</span><span class="sxs-lookup"><span data-stu-id="244ce-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="244ce-129">Jeśli chcesz przyznać uprawnienia roli właściciela na poziomie grupy zasobów lub zasobu zamiast w zakresie subskrypcji, następujące polecenia mogą działać:</span><span class="sxs-lookup"><span data-stu-id="244ce-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="244ce-130">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="244ce-130">Next steps</span></span>

- [<span data-ttu-id="244ce-131">Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="244ce-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
