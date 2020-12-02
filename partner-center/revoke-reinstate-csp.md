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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="5c3ae-103">Przywracanie uprawnień administratora dla subskrypcji dostawcy CSP platformy Azure klienta</span><span class="sxs-lookup"><span data-stu-id="5c3ae-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="5c3ae-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="5c3ae-104">**Applicable roles**</span></span>

- <span data-ttu-id="5c3ae-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="5c3ae-105">Global admin</span></span>
- <span data-ttu-id="5c3ae-106">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="5c3ae-106">Admin agent</span></span>

<span data-ttu-id="5c3ae-107">Jako partner programu CSP klienci często oczekują, że będziesz zarządzać użyciem platformy Azure i ich systemami.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="5c3ae-108">Wykonanie tej czynności wymaga uprawnień administratora.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="5c3ae-109">Niektóre uprawnienia są przyznawane w przypadku ustanowienia relacji odsprzedawcy z klientem.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="5c3ae-110">Inne osoby są udzielane użytkownikowi przez klienta.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="5c3ae-111">Uprawnienia administratora platformy Azure w programie CSP</span><span class="sxs-lookup"><span data-stu-id="5c3ae-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="5c3ae-112">Istnieją dwa poziomy uprawnień administratora dla platformy Azure w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="5c3ae-113">**Uprawnienia administratora na poziomie dzierżawy** (**uprawnienia administratora delegowanego**) — partnerzy CSP uzyskują te uprawnienia podczas ustanawiania relacji odsprzedawcy dostawcy CSP z klientami.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="5c3ae-114">Zapewnia to partnerom CSP dostęp do dzierżawców klientów, co umożliwia im wykonywanie funkcji administracyjnych, takich jak dodawanie/zarządzanie użytkownikami, resetowanie haseł i zarządzanie licencjami użytkowników.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="5c3ae-115">**Uprawnienia administratora na poziomie subskrypcji** — partnerzy programu CSP uzyskują te uprawnienia podczas tworzenia subskrypcji dostawcy usług kryptograficznych platformy Azure dla swoich klientów.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="5c3ae-116">Posiadanie tych uprawnień zapewnia partnerom CSP pełny dostęp do tych subskrypcji, co umożliwia im udostępnianie zasobów platformy Azure i zarządzanie nimi.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="5c3ae-117">Przywracanie uprawnień administratora partnerów CSP</span><span class="sxs-lookup"><span data-stu-id="5c3ae-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="5c3ae-118">Aby odzyskać uprawnienia administratora delegowanego, musisz skontaktować się z klientem.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="5c3ae-119">Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego i w menu Centrum partnerskiego wybierz pozycję **klienci**.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="5c3ae-120">Wybierz klienta, z którym pracujesz, i **Zażądaj relacji odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="5c3ae-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="5c3ae-121">Spowoduje to wygenerowanie linku do klienta z uprawnieniami administratora dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="5c3ae-122">Użytkownik musi wybrać link i zatwierdzić żądanie relacji odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Relacja odsprzedawcy":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="5c3ae-124">Dodawanie grupy agentów administracyjnych jako właściciela subskrypcji CSP platformy Azure</span><span class="sxs-lookup"><span data-stu-id="5c3ae-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="5c3ae-125">Klient będzie musiał dodać grupę agentów administracyjnych jako właściciela subskrypcji dostawcy CSP platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-125">Your customer will need to add your admin agent group as the owner of the Azure CSP subscription.</span></span>

1. <span data-ttu-id="5c3ae-126">Użyj konsoli programu PowerShell lub środowiska PowerShell Integrated Scripting Environment (ISE).</span><span class="sxs-lookup"><span data-stu-id="5c3ae-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="5c3ae-127">Upewnij się, że moduły AzureAD są zainstalowane.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-127">Ensure that AzureAD modules are installed.</span></span>

2. <span data-ttu-id="5c3ae-128">Nawiąż połączenie z dzierżawą usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="5c3ae-129">Uzyskaj identyfikator ObjectId grup agentów administracyjnych.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```
   <span data-ttu-id="5c3ae-130">Następujące kroki są wykonywane przez użytkownika w firmie klienta, który ma dostęp właściciela do subskrypcji dostawcy CSP platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-130">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="5c3ae-131">Użytkownik z dostępem właściciela do subskrypcji CSP platformy Azure loguje się do platformy Azure przy użyciu swoich poświadczeń.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-131">The user with owner access to the Azure CSP subscription, signs into Azure using her credentials.</span></span>

   ```powershell
   Connect-AzAccount
   ```

5. <span data-ttu-id="5c3ae-132">Następnie może dodać grupę agentów administracyjnych jako właściciela do subskrypcji platformy Azure dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="5c3ae-132">She can then add your admin agent group as owner to the CSP Azure subscription.</span></span>

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a><span data-ttu-id="5c3ae-133">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="5c3ae-133">Next steps</span></span>

[<span data-ttu-id="5c3ae-134">Zarządzanie subskrypcjami i zasobami w ramach planu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="5c3ae-134">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
