---
title: Dodawanie dodatkowych dzierżawców do konta Centrum partnerskiego
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodawać i konsolidować wiele dzierżawców usługi Azure AD na koncie Centrum partnerskiego oraz zarządzać nimi. Dowiedz się również kilka przyczyn, które warto wykonać.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105560"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="22b5e-104">Dodawanie wielu dzierżawców i zarządzanie nimi na koncie Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="22b5e-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="22b5e-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="22b5e-105">**Appropriate roles**</span></span>

- <span data-ttu-id="22b5e-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="22b5e-106">Global admin</span></span>

<span data-ttu-id="22b5e-107">Ta funkcja pozwala zarządzać wieloma dzierżawami dla firmy i konsolidować je na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="22b5e-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="22b5e-108">Istnieje wiele powodów, dla których może być konieczne zarządzanie wieloma dzierżawami usługi Azure AD na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="22b5e-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="22b5e-109">Na przykład:</span><span class="sxs-lookup"><span data-stu-id="22b5e-109">For example:</span></span>

- <span data-ttu-id="22b5e-110">Firma może zakupić inną firmę i chce, aby pracownicy w nowej firmie mogli korzystać z Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="22b5e-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="22b5e-111">Jednak dwie firmy powinny pozostać osobne.</span><span class="sxs-lookup"><span data-stu-id="22b5e-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="22b5e-112">W takim przypadku należy skojarzyć dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="22b5e-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="22b5e-113">To skojarzenie umożliwi użytkownikom w obu firmach działanie w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="22b5e-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="22b5e-114">Jeśli masz więcej niż jedną dzierżawę do uruchomienia Twojej firmy (np. contoso.com, contoso.uk, contoso.in), możesz użyć wielu dzierżawców, aby powiązać je w ramach tego samego konta komputera.</span><span class="sxs-lookup"><span data-stu-id="22b5e-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="22b5e-115">Fuzje i przejęcia wymagają pracy z więcej niż jedną dzierżawą (np. Jeśli firma Contoso uzyska Fabrikam, musi być w stanie użyć zarówno Constoso.com, jak i Fabrikam.com odpowiednich dzierżawców).</span><span class="sxs-lookup"><span data-stu-id="22b5e-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="22b5e-116">Użytkownicy z dowolnego dzierżawy muszą mieć możliwość:</span><span class="sxs-lookup"><span data-stu-id="22b5e-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="22b5e-117">Centrum partnerskie dostępu do szkoleń, pobierania cyfrowego, skojarzenia MCP</span><span class="sxs-lookup"><span data-stu-id="22b5e-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="22b5e-118">Do przypisywania ról Centrum partnerskiego, takich jak MPN administrator, zachęty administratora itp.</span><span class="sxs-lookup"><span data-stu-id="22b5e-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="22b5e-119">Dodaj kolejną dzierżawę usługi Azure AD do swojego konta</span><span class="sxs-lookup"><span data-stu-id="22b5e-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="22b5e-120">Jako Administrator globalny Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="22b5e-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="22b5e-121">Na ikonie **ustawień** wybierz pozycję **Ustawienia konta** , a następnie wybierz pozycję **dzierżawy**.</span><span class="sxs-lookup"><span data-stu-id="22b5e-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Kojarzenie dzierżawców"::: 

3. <span data-ttu-id="22b5e-123">Wybierz pozycję **Skojarz inną dzierżawę usługi AD** i wskaż dzierżawcę, którą chcesz skojarzyć.</span><span class="sxs-lookup"><span data-stu-id="22b5e-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="22b5e-124">Jako Administrator globalny Zaloguj się do dzierżawy, którą chcesz skojarzyć, i Potwierdź skojarzenie.</span><span class="sxs-lookup"><span data-stu-id="22b5e-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Potwierdź kojarzenie dzierżawców"::: 

5. <span data-ttu-id="22b5e-126">Po potwierdzeniu zostanie wyświetlona informacja o **zestawie** .</span><span class="sxs-lookup"><span data-stu-id="22b5e-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="22b5e-127">Wybierz pozycję **Wróć do zarządzania dzierżawcą** i zobaczysz nowo dodaną dzierżawę na liście.</span><span class="sxs-lookup"><span data-stu-id="22b5e-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="22b5e-128">Nie można skojarzyć dzierżawy z kontem, jeśli jest ono już skojarzone z innym kontem Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="22b5e-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="22b5e-129">Usuwanie dzierżawy z konta</span><span class="sxs-lookup"><span data-stu-id="22b5e-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="22b5e-130">Jako Administrator globalny Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="22b5e-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="22b5e-131">Na ikonie **ustawień** wybierz pozycję **ustawienia konta** — > dzierżawców i kliknij kartę **partner** .</span><span class="sxs-lookup"><span data-stu-id="22b5e-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="22b5e-132">Kliknij pozycję Usuń dla dzierżawy, którą chcesz **usunąć** skojarzenie.</span><span class="sxs-lookup"><span data-stu-id="22b5e-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="22b5e-133">Skojarzenie dzierżawy oznacza, że użytkownicy tej dzierżawy nie będą już mieli dostępu do konta Centrum partnerskiego i mogą mieć wpływ na swoje kompetencje.</span><span class="sxs-lookup"><span data-stu-id="22b5e-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="22b5e-134">Przycisk **Usuń** jest włączony dla wszystkich skojarzonych dzierżawców, z wyjątkiem głównej dzierżawy i dzierżawy, do której użytkownik jest obecnie zalogowany.</span><span class="sxs-lookup"><span data-stu-id="22b5e-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="dzierżawcy z przyciskiem Usuń":::
 

## <a name="next-steps"></a><span data-ttu-id="22b5e-136">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="22b5e-136">Next steps</span></span>

- [<span data-ttu-id="22b5e-137">Dodaj użytkowników</span><span class="sxs-lookup"><span data-stu-id="22b5e-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






