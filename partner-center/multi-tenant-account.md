---
title: Dodawanie dzierżaw do konta Partner Center dzierżawy
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodawać i konsolidować wiele dzierżaw usługi Azure AD Partner Center konta usługi Azure AD oraz jak nimi zarządzać, i dowiedz się, dlaczego warto to zrobić.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151206"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="216ab-103">Dodawanie wielu dzierżaw na koncie usługi Partner Center zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="216ab-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="216ab-104">**Odpowiednie role:** Administrator globalny | Administrator konta</span><span class="sxs-lookup"><span data-stu-id="216ab-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="216ab-105">W tym artykule omówiono sposób konsolidowania wielu dzierżaw usługi Azure Active Directory (Azure AD) dla firmy, a następnie dodawania ich i zarządzania nimi na koncie Partner Center dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="216ab-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="216ab-106">Istnieje wiele powodów, aby to zrobić.</span><span class="sxs-lookup"><span data-stu-id="216ab-106">There are many reasons to do so.</span></span> <span data-ttu-id="216ab-107">Na przykład:</span><span class="sxs-lookup"><span data-stu-id="216ab-107">For example:</span></span>

- <span data-ttu-id="216ab-108">Załóżmy, że Twoja firma, Contoso, nabyła inną firmę, Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="216ab-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="216ab-109">Chcesz, aby obie firmy pozostały oddzielone, ale chcesz, aby nowi pracownicy mogli korzystać z Partner Center.</span><span class="sxs-lookup"><span data-stu-id="216ab-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="216ab-110">W takim przypadku skojarzysz dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="216ab-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="216ab-111">To skojarzenie umożliwia użytkownikom w obu firmach pracę w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="216ab-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="216ab-112">Jeśli firma działa z więcej niż jedną dzierżawą (na przykład *contoso.com*, *contoso.uk* i *contoso.in*), można użyć wielodostępności, aby zgrupować je na tym samym koncie komputera.</span><span class="sxs-lookup"><span data-stu-id="216ab-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="216ab-113">Jeśli wytyczne dotyczące koncentracji i pozyskiwania wymagają współpracy z dzierżawami  obu firm, należy użyć zarówno constoso.com, *jak i fabrikam.com* dzierżawców.</span><span class="sxs-lookup"><span data-stu-id="216ab-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="216ab-114">Użytkownicy dowolnej dzierżawy muszą mieć możliwość:</span><span class="sxs-lookup"><span data-stu-id="216ab-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="216ab-115">Dostęp Partner Center do szkoleń, pobierania cyfrowego lub skojarzenia Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="216ab-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="216ab-116">Mieć przypisane Partner Center, takie jak Microsoft Partner Network (MPN) lub administrator zachęt.</span><span class="sxs-lookup"><span data-stu-id="216ab-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="216ab-117">Dodawanie dzierżawy usługi Azure AD do konta</span><span class="sxs-lookup"><span data-stu-id="216ab-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="216ab-118">Zaloguj się jako administrator globalny w aplikacji [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="216ab-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="216ab-119">W prawym górnym rogu wybierz pozycję **Ustawienia,** wybierz **pozycję Ustawienia konta,** a następnie wybierz **pozycję Dzierżawy.**</span><span class="sxs-lookup"><span data-stu-id="216ab-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Zrzut ekranu przedstawiający przycisk Skojarz w okienku Profil usługi Azure AD."::: 

1. <span data-ttu-id="216ab-121">Wybierz **pozycję Skojarz,** a następnie wskaż dzierżawę, którą chcesz skojarzyć.</span><span class="sxs-lookup"><span data-stu-id="216ab-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="216ab-122">Po wyświetleniu monitu zaloguj się jako administrator globalny do dzierżawy, którą chcesz skojarzyć, a następnie wybierz pozycję **Potwierdź.**</span><span class="sxs-lookup"><span data-stu-id="216ab-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zrzut ekranu przedstawiający przycisk Potwierdź w okienku Potwierdzanie nowego skojarzenia usługi Azure AD."::: 

   <span data-ttu-id="216ab-124">Po potwierdzeniu skojarzenia zostanie wyświetlony **komunikat Wszystkie** zestawy.</span><span class="sxs-lookup"><span data-stu-id="216ab-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="216ab-125">Aby wyświetlić nowo dodaną dzierżawę, wybierz pozycję **Powrót do zarządzania dzierżawą.**</span><span class="sxs-lookup"><span data-stu-id="216ab-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="216ab-126">Nie można skojarzyć dzierżawy z kontem, jeśli jest ona już skojarzona z innym Partner Center kontem.</span><span class="sxs-lookup"><span data-stu-id="216ab-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="216ab-127">Usuwanie dzierżawy z konta</span><span class="sxs-lookup"><span data-stu-id="216ab-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="216ab-128">Zaloguj się jako administrator globalny w aplikacji [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="216ab-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="216ab-129">W prawym górnym rogu wybierz **ikonę Ustawienia,** a następnie wybierz **pozycję Ustawienia konta.**</span><span class="sxs-lookup"><span data-stu-id="216ab-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="216ab-130">W okienku po lewej stronie wybierz **pozycję Dzierżawy.**</span><span class="sxs-lookup"><span data-stu-id="216ab-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="216ab-131">W **obszarze Zarządzanie dzierżawami usługi Azure AD** wybierz **kartę Partner.**</span><span class="sxs-lookup"><span data-stu-id="216ab-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="216ab-132">Wybierz **pozycję Usuń** obok dzierżawy, której skojarzenie chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="216ab-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Zrzut ekranu przedstawiający bieżące skojarzenia dzierżawy i ich linki Usuń.":::

   <span data-ttu-id="216ab-134">Jak pokazano na poprzednim  zrzucie ekranu, linki Usuń są włączone dla wszystkich skojarzonych dzierżaw, z wyjątkiem dzierżawy podstawowej i dzierżawy, do których aktualnie się zalogowano.</span><span class="sxs-lookup"><span data-stu-id="216ab-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="216ab-135">Po usunięciu dzierżawy użytkownicy w tej dzierżawie nie mają już dostępu do konta usługi Partner Center, a usunięcie może mieć wpływ na Twoje kompetencje.</span><span class="sxs-lookup"><span data-stu-id="216ab-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="216ab-136">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="216ab-136">Next steps</span></span>

- [<span data-ttu-id="216ab-137">Tworzenie kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="216ab-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






