---
title: Dodawanie dodatkowych dzierżawców do konta Centrum partnerskiego
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodawać i konsolidować wiele dzierżawców usługi Azure AD na koncie Centrum partnerskiego oraz zarządzać nimi. Dowiedz się również kilka przyczyn, które warto wykonać.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530513"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="1848e-104">Dodawanie wielu dzierżawców i zarządzanie nimi na koncie Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="1848e-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="1848e-105">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="1848e-105">**Applies to**</span></span>

- <span data-ttu-id="1848e-106">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="1848e-106">Partner Center</span></span>

<span data-ttu-id="1848e-107">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="1848e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="1848e-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="1848e-108">Global admin</span></span>

<span data-ttu-id="1848e-109">Ta funkcja pozwala zarządzać wieloma dzierżawami dla firmy i konsolidować je na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="1848e-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="1848e-110">Istnieje wiele powodów, dla których może być konieczne zarządzanie wieloma dzierżawami usługi Azure AD na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="1848e-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="1848e-111">Na przykład:</span><span class="sxs-lookup"><span data-stu-id="1848e-111">For example:</span></span>

- <span data-ttu-id="1848e-112">Firma może zakupić inną firmę i chce, aby pracownicy w nowej firmie mogli korzystać z Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="1848e-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="1848e-113">Jednak dwie firmy powinny pozostać osobne.</span><span class="sxs-lookup"><span data-stu-id="1848e-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="1848e-114">W takim przypadku należy skojarzyć dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="1848e-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="1848e-115">To skojarzenie umożliwi użytkownikom w obu firmach działanie w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="1848e-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="1848e-116">Jeśli masz więcej niż jedną dzierżawę do uruchomienia Twojej firmy (np. contoso.com, contoso.uk, contoso.in), możesz użyć wielu dzierżawców, aby powiązać je w ramach tego samego konta komputera.</span><span class="sxs-lookup"><span data-stu-id="1848e-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="1848e-117">Fuzje i przejęcia wymagają pracy z więcej niż jedną dzierżawą (np. Jeśli firma Contoso uzyska Fabrikam, musi być w stanie użyć zarówno Constoso.com, jak i Fabrikam.com odpowiednich dzierżawców).</span><span class="sxs-lookup"><span data-stu-id="1848e-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="1848e-118">Użytkownicy z dowolnego dzierżawy muszą mieć możliwość:</span><span class="sxs-lookup"><span data-stu-id="1848e-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="1848e-119">Centrum partnerskie dostępu do szkoleń, pobierania cyfrowego, skojarzenia MCP</span><span class="sxs-lookup"><span data-stu-id="1848e-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="1848e-120">Do przypisywania ról Centrum partnerskiego, takich jak MPN administrator, zachęty administratora itp.</span><span class="sxs-lookup"><span data-stu-id="1848e-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="1848e-121">Dodaj kolejną dzierżawę usługi Azure AD do swojego konta</span><span class="sxs-lookup"><span data-stu-id="1848e-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="1848e-122">Jako Administrator globalny Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="1848e-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="1848e-123">Na ikonie **ustawień** wybierz pozycję **Ustawienia konta** , a następnie wybierz pozycję **dzierżawy** .</span><span class="sxs-lookup"><span data-stu-id="1848e-123">From the **Settings** icon, select **Account settings** and then select **Tenants** .</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Kojarzenie dzierżawców"::: 

3. <span data-ttu-id="1848e-125">Wybierz pozycję **Skojarz inną dzierżawę usługi AD** i wskaż dzierżawcę, którą chcesz skojarzyć.</span><span class="sxs-lookup"><span data-stu-id="1848e-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="1848e-126">Jako Administrator globalny Zaloguj się do dzierżawy, którą chcesz skojarzyć, i Potwierdź skojarzenie.</span><span class="sxs-lookup"><span data-stu-id="1848e-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Potwierdź kojarzenie dzierżawców"::: 

5. <span data-ttu-id="1848e-128">Po potwierdzeniu zostanie wyświetlona informacja o **zestawie** .</span><span class="sxs-lookup"><span data-stu-id="1848e-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="1848e-129">Wybierz opcję **Wróć do zarządzania dzierżawcą** i zobaczysz nowo dodaną dzierżawę na liście.</span><span class="sxs-lookup"><span data-stu-id="1848e-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="1848e-130">Nie można skojarzyć dzierżawy z kontem, jeśli jest ono już skojarzone z innym kontem Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="1848e-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="1848e-131">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="1848e-131">Next steps</span></span>

- [<span data-ttu-id="1848e-132">Dodaj użytkowników</span><span class="sxs-lookup"><span data-stu-id="1848e-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
