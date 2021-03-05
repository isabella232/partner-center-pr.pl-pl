---
title: Dodawanie dzierżawców do konta Centrum partnerskiego
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodawać i konsolidować wiele dzierżawców usługi Azure AD na koncie Centrum partnerskiego oraz zarządzać nimi, a także dowiedzieć się, dlaczego warto to zrobić.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124809"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="72d21-103">Dodawanie wielu dzierżawców i zarządzanie nimi na koncie Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="72d21-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="72d21-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="72d21-104">**Appropriate roles**</span></span>

- <span data-ttu-id="72d21-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="72d21-105">Global admin</span></span>
- <span data-ttu-id="72d21-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="72d21-106">Account admin</span></span>

<span data-ttu-id="72d21-107">W tym artykule omówiono sposób konsolidowania wielu dzierżaw Azure Active Directory (Azure AD) dla Twojej firmy, a następnie dodawania ich i zarządzania nimi na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="72d21-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="72d21-108">Istnieje wiele powodów, dla których należy to zrobić.</span><span class="sxs-lookup"><span data-stu-id="72d21-108">There are many reasons to do so.</span></span> <span data-ttu-id="72d21-109">Na przykład:</span><span class="sxs-lookup"><span data-stu-id="72d21-109">For example:</span></span>

- <span data-ttu-id="72d21-110">Załóżmy, że firma Contoso uzyska kolejną firmę, firmę fabrikam.</span><span class="sxs-lookup"><span data-stu-id="72d21-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="72d21-111">Chcesz, aby dwie firmy pozostały do oddzielenia, ale chcesz, aby nowi pracownicy mogli korzystać z Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="72d21-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="72d21-112">W takim przypadku należy skojarzyć dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="72d21-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="72d21-113">To skojarzenie umożliwia użytkownikom w obu firmach działanie w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="72d21-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="72d21-114">Jeśli uruchamiasz swoją firmę z więcej niż jedną dzierżawą (na przykład *contoso.com*, *contoso.uk* i *contoso.in*), możesz użyć wielodostępności, aby ZGRUPOWAĆ je na tym samym koncie komputera.</span><span class="sxs-lookup"><span data-stu-id="72d21-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="72d21-115">Jeśli fuzje i wskazówki dotyczące pozyskiwania wymagają pracy z dzierżawcami obu firm, należy użyć zarówno dzierżaw *constoso.com* , jak i *fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="72d21-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="72d21-116">Użytkownicy dowolnych dzierżawców muszą mieć możliwość:</span><span class="sxs-lookup"><span data-stu-id="72d21-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="72d21-117">Centrum partnerskie dostępu do szkoleń, plików cyfrowych i skojarzeń Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="72d21-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="72d21-118">Należy przypisać role Centrum partnerskiego, takie jak administrator Microsoft Partner Network (MPN) lub administrator zachęt.</span><span class="sxs-lookup"><span data-stu-id="72d21-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="72d21-119">Dodawanie dzierżawy usługi Azure AD do konta</span><span class="sxs-lookup"><span data-stu-id="72d21-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="72d21-120">Zaloguj się jako Administrator globalny do [Centrum partnerskiego firmy Microsoft](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="72d21-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="72d21-121">W prawym górnym rogu wybierz pozycję **Ustawienia**, wybierz pozycję **Ustawienia konta**, a następnie wybierz pozycję **dzierżawy**.</span><span class="sxs-lookup"><span data-stu-id="72d21-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Zrzut ekranu przedstawiający przycisk Skojarz w okienku profil usługi Azure AD."::: 

1. <span data-ttu-id="72d21-123">Wybierz pozycję **Skojarz**, a następnie wskaż dzierżawcę, który chcesz skojarzyć.</span><span class="sxs-lookup"><span data-stu-id="72d21-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="72d21-124">W wierszu polecenia Zaloguj się jako Administrator globalny do dzierżawy, którą chcesz skojarzyć, a następnie wybierz pozycję **Potwierdź**.</span><span class="sxs-lookup"><span data-stu-id="72d21-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zrzut ekranu przedstawiający przycisk Potwierdź w okienku Potwierdź nowe skojarzenie usługi Azure AD."::: 

   <span data-ttu-id="72d21-126">Po potwierdzeniu skojarzenia zostanie wyświetlony komunikat **cała grupa** .</span><span class="sxs-lookup"><span data-stu-id="72d21-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="72d21-127">Aby wyświetlić nowo dodaną dzierżawę, wybierz pozycję **Wróć do zarządzania dzierżawcą**.</span><span class="sxs-lookup"><span data-stu-id="72d21-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="72d21-128">Nie można skojarzyć dzierżawy z kontem, jeśli jest ono już skojarzone z innym kontem Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="72d21-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="72d21-129">Usuwanie dzierżawy z konta</span><span class="sxs-lookup"><span data-stu-id="72d21-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="72d21-130">Zaloguj się jako Administrator globalny do [Centrum partnerskiego firmy Microsoft](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="72d21-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="72d21-131">W prawym górnym rogu wybierz ikonę **Ustawienia** , a następnie wybierz pozycję **Ustawienia konta**.</span><span class="sxs-lookup"><span data-stu-id="72d21-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="72d21-132">W okienku po lewej stronie wybierz pozycję **dzierżawy**.</span><span class="sxs-lookup"><span data-stu-id="72d21-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="72d21-133">W obszarze **Zarządzanie dzierżawami usługi Azure AD** wybierz kartę **partner** .</span><span class="sxs-lookup"><span data-stu-id="72d21-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="72d21-134">Wybierz pozycję **Usuń** obok dzierżawy, której skojarzenie chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="72d21-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Zrzut ekranu przedstawiający bieżące skojarzenia dzierżawców i ich linki do usunięcia.":::

   <span data-ttu-id="72d21-136">Jak pokazano na poprzednim zrzucie ekranu, łącza **Usuń** są włączone dla wszystkich skojarzonych dzierżawców, z wyjątkiem głównej dzierżawy i dzierżawy, do której użytkownik jest aktualnie zalogowany.</span><span class="sxs-lookup"><span data-stu-id="72d21-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="72d21-137">Po usunięciu dzierżawy użytkownicy tej dzierżawy nie mają już dostępu do konta Centrum partnerskiego, a usunięcie może mieć wpływ na swoje kompetencje.</span><span class="sxs-lookup"><span data-stu-id="72d21-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="72d21-138">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="72d21-138">Next steps</span></span>

- [<span data-ttu-id="72d21-139">Tworzenie kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="72d21-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






