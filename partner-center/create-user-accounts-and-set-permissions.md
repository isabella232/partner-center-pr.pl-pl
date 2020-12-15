---
title: Tworzenie kont użytkowników i przypisywanie ról
description: Każdy pracownik musi mieć przypisaną rolę, aby mógł uzyskać dostęp do Centrum partnerskiego. Dowiedz się, jak tworzyć konta użytkowników, przypisywać role i ustawiać uprawnienia.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492538"
---
# <a name="create-user-accounts"></a><span data-ttu-id="5177b-104">Tworzenie kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="5177b-104">Create user accounts</span></span>  

<span data-ttu-id="5177b-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="5177b-105">**Appropriate roles**</span></span>

- <span data-ttu-id="5177b-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="5177b-106">Account admin</span></span>
- <span data-ttu-id="5177b-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="5177b-107">Global admin</span></span>
- <span data-ttu-id="5177b-108">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="5177b-108">User management admin</span></span>

<span data-ttu-id="5177b-109">Utwórz konta użytkowników dla pracowników, którzy potrzebują dostępu do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="5177b-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="5177b-110">Te zadania muszą zostać wykonane przez administratora zarządzania użytkownikami, administratora kont lub administratora globalnego. Użytkownik wykonujący te zadania musi mieć również przypisane role Azure Active Directory (AAD) administratora lub administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="5177b-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="5177b-111">Aby uzyskać więcej informacji na temat ról usługi AAD, zobacz [uprawnienia roli administrator w Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="5177b-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="5177b-112">Dodawanie nowego użytkownika</span><span class="sxs-lookup"><span data-stu-id="5177b-112">Add a new user</span></span>

1. <span data-ttu-id="5177b-113">Na ikonie **ustawień** w prawym górnym rogu Centrum partnerskiego wybierz pozycję **Ustawienia konta** , a następnie wybierz pozycję **Zarządzanie użytkownikami**.</span><span class="sxs-lookup"><span data-stu-id="5177b-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="5177b-114">Wybierz pozycję **Dodaj użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="5177b-114">Select **Add user**.</span></span>

3. <span data-ttu-id="5177b-115">Wprowadź pełną nazwę i unikatowy adres e-mail użytkownika.</span><span class="sxs-lookup"><span data-stu-id="5177b-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="5177b-116">Wybierz typ agenta i/lub typ administratora, który ma zostać przypisany do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="5177b-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="5177b-117">Dostęp do Centrum partnerskiego jest oparty na rolach, dzięki czemu można przypisywać uprawnienia do dostosowywania widoku użytkownika w celu wyświetlenia tylko tych funkcji, których użytkownik potrzebuje do wykonania określonych zadań.</span><span class="sxs-lookup"><span data-stu-id="5177b-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="5177b-118">Jeśli użytkownik chce przypisywać rolę, może znaleźć administratorów globalnych, aby skontaktować się z **zarządzaniem użytkownikami** i filtrowaniem w Administrator globalny.</span><span class="sxs-lookup"><span data-stu-id="5177b-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="5177b-119">Wybierz pozycję **Dodaj**, aby utworzyć konto użytkownika.</span><span class="sxs-lookup"><span data-stu-id="5177b-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="5177b-120">Potwierdź szczegóły użytkownika na następnej stronie.</span><span class="sxs-lookup"><span data-stu-id="5177b-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="5177b-121">Zanotuj informacje logowania nowego użytkownika wyświetlane na tej stronie.</span><span class="sxs-lookup"><span data-stu-id="5177b-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="5177b-122">Pamiętaj o skopiowaniu i wysłaniu tych informacji do nowego użytkownika, ponieważ nie będzie można uzyskać do niego dostępu później.</span><span class="sxs-lookup"><span data-stu-id="5177b-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="5177b-123">Użytkownik będzie musiał zalogować się do Centrum partnerskiego przy użyciu nazwy użytkownika i hasła tymczasowego.</span><span class="sxs-lookup"><span data-stu-id="5177b-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="5177b-124">Gdy użytkownik loguje się do Centrum partnerskiego po raz pierwszy, zostanie wyświetlony monit o zmianę hasła.</span><span class="sxs-lookup"><span data-stu-id="5177b-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="5177b-125">Przypisywanie ról użytkownika</span><span class="sxs-lookup"><span data-stu-id="5177b-125">Assign user roles</span></span>

<span data-ttu-id="5177b-126">Aby móc korzystać z Centrum partnerskiego, musisz mieć przypisaną rolę.</span><span class="sxs-lookup"><span data-stu-id="5177b-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="5177b-127">Obecnie role Azure Active Directory obejmują role dzierżawy, role dostawcy rozwiązań w chmurze (CSP) i role firmy inne niż AAD.</span><span class="sxs-lookup"><span data-stu-id="5177b-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="5177b-128">Dla wszystkich tych ról może być wymagana konkretna firma.</span><span class="sxs-lookup"><span data-stu-id="5177b-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="5177b-129">Aby można było uzyskać dostęp do Centrum partnerskiego, osoby muszą być wymienione w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="5177b-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="5177b-130">Przypisania ról zapewniają dodatkowy dostęp.</span><span class="sxs-lookup"><span data-stu-id="5177b-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5177b-131">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="5177b-131">Next steps</span></span>

- [<span data-ttu-id="5177b-132">Przypisywanie ról i uprawnień użytkowników potrzebnych pracownikom w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="5177b-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
