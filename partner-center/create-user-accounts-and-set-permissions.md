---
title: Tworzenie kont użytkowników i przypisywanie ról
description: Każdy pracownik musi mieć przypisaną rolę, aby uzyskać dostęp do Partner Center. Dowiedz się, jak tworzyć konta użytkowników, przypisywać role i ustawiać uprawnienia.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148146"
---
# <a name="create-user-accounts"></a><span data-ttu-id="daf74-104">Tworzenie kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="daf74-104">Create user accounts</span></span>  

<span data-ttu-id="daf74-105">**Odpowiednie role:** Administrator konta | Administrator globalny | Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="daf74-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="daf74-106">Tworzenie kont użytkowników dla pracowników, którzy potrzebują dostępu do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="daf74-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="daf74-107">Te zadania muszą być wykonywane przez administratora zarządzania użytkownikami, administratora kont lub administratora globalnego. Użytkownik wykonujący te zadania musi również mieć przypisane Azure Active Directory (AAD) administratora użytkowników lub administrator globalny.</span><span class="sxs-lookup"><span data-stu-id="daf74-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="daf74-108">Aby uzyskać więcej informacji na temat ról usługi AAD, zobacz [Uprawnienia ról administratorów](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)w u Azure Active Directory .</span><span class="sxs-lookup"><span data-stu-id="daf74-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="daf74-109">Dodawanie nowego użytkownika</span><span class="sxs-lookup"><span data-stu-id="daf74-109">Add a new user</span></span>

1. <span data-ttu-id="daf74-110">Z **ikony** Ustawienia w prawym górnym rogu ekranu Partner Center **pozycję Ustawienia konta,** a następnie pozycję **Zarządzanie użytkownikami.**</span><span class="sxs-lookup"><span data-stu-id="daf74-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="daf74-111">Wybierz pozycję **Dodaj użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="daf74-111">Select **Add user**.</span></span>

3. <span data-ttu-id="daf74-112">Wprowadź pełną nazwę użytkownika i unikatowy adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="daf74-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="daf74-113">Wybierz typ agenta i/lub typ administratora, który chcesz przypisać do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="daf74-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="daf74-114">Partner Center jest oparty na rolach, dlatego można przypisać uprawnienia w celu dostosowania widoku użytkownika w celu wyświetlenia tylko tych funkcji, których użytkownik potrzebuje do wykonania określonych zadań.</span><span class="sxs-lookup"><span data-stu-id="daf74-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="daf74-115">Jeśli użytkownicy chcą mieć przypisanie roli, mogą znaleźć administratorów globalnych, z którym mają się kontaktować, przechodząc do tematu **Zarządzanie** użytkownikami i filtrowanie według administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="daf74-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="daf74-116">Wybierz pozycję **Dodaj**, aby utworzyć konto użytkownika.</span><span class="sxs-lookup"><span data-stu-id="daf74-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="daf74-117">Potwierdź szczegóły użytkownika na następnej stronie.</span><span class="sxs-lookup"><span data-stu-id="daf74-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="daf74-118">Zanotuj informacje logowania nowego użytkownika wyświetlane na tej stronie.</span><span class="sxs-lookup"><span data-stu-id="daf74-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="daf74-119">Pamiętaj, aby skopiować i wysłać te informacje do nowego użytkownika, ponieważ nie będzie można później uzyskać do nich dostępu ponownie.</span><span class="sxs-lookup"><span data-stu-id="daf74-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="daf74-120">Użytkownik musi zalogować się do aplikacji przy użyciu Partner Center użytkownika i hasła tymczasowego.</span><span class="sxs-lookup"><span data-stu-id="daf74-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="daf74-121">Gdy użytkownik po raz pierwszy Partner Center do aplikacji, zostanie wyświetlony monit o zmianę hasła.</span><span class="sxs-lookup"><span data-stu-id="daf74-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="daf74-122">Przypisywanie ról użytkowników</span><span class="sxs-lookup"><span data-stu-id="daf74-122">Assign user roles</span></span>

<span data-ttu-id="daf74-123">Aby pracować w Partner Center, musisz mieć przypisaną rolę.</span><span class="sxs-lookup"><span data-stu-id="daf74-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="daf74-124">Obecnie role obejmują Azure Active Directory dzierżawy, Dostawca rozwiązań w chmurze (CSP) i role firmowe spoza usługi AAD.</span><span class="sxs-lookup"><span data-stu-id="daf74-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="daf74-125">Każda firma może potrzebować wszystkich tych ról.</span><span class="sxs-lookup"><span data-stu-id="daf74-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="daf74-126">Aby uzyskać dostęp do aplikacji, należy znajdować się na liście Partner Center.</span><span class="sxs-lookup"><span data-stu-id="daf74-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="daf74-127">Przypisania ról zapewniają dodatkowy dostęp.</span><span class="sxs-lookup"><span data-stu-id="daf74-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="daf74-128">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="daf74-128">Next steps</span></span>

- [<span data-ttu-id="daf74-129">Przypisywanie ról i uprawnień użytkowników pracownikom, którzy muszą pracować w Partner Center</span><span class="sxs-lookup"><span data-stu-id="daf74-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
