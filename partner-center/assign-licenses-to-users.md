---
title: Zarządzanie użytkownikami dla kont klientów
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zarządzanie użytkownikami dla klientów w Partner Center — tworzenie kont użytkowników, dodawanie lub usuwanie licencji użytkowników, resetowanie haseł oraz usuwanie lub przywracanie kont użytkowników.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149897"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="c431a-103">Zarządzanie użytkownikami i licencjami użytkowników dla kont klientów</span><span class="sxs-lookup"><span data-stu-id="c431a-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="c431a-104">**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="c431a-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="c431a-105">Możesz tworzyć i usuwać nowych użytkowników na koncie klienta.</span><span class="sxs-lookup"><span data-stu-id="c431a-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="c431a-106">Możesz również przywrócić co najmniej jedno konto użytkownika, które zostało wcześniej usunięte w ciągu 30 dni od usunięcia.</span><span class="sxs-lookup"><span data-stu-id="c431a-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="c431a-107">Zostaną również przywrócone poprzednie przypisania subskrypcji użytkownika (przy założeniu, że są dostępne jego poprzednie alokacje).</span><span class="sxs-lookup"><span data-stu-id="c431a-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="c431a-108">Gdy kupujesz nowe subskrypcje dla klienta, klient powinien podać listę wszystkich użytkowników, którzy będą potrzebować kont, ich uprawnień użytkownika i usług, których potrzebuje każdy użytkownik.</span><span class="sxs-lookup"><span data-stu-id="c431a-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="c431a-109">Sekcja **Użytkownicy i** licencje  na karcie Klient zawiera wszystkich użytkowników utworzonych w dzierżawie określonego klienta, w tym użytkowników, którzy mają licencje zakupione od innego partnera CSP lub z innego kanału zakupów.</span><span class="sxs-lookup"><span data-stu-id="c431a-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="c431a-110">Subskrypcje [można przypisywać do wielu użytkowników](bulk-license-provisioning-for-multiple-users.md) jednocześnie, importując nazwy przy użyciu pliku arkusza kalkulacyjnego CSV zgodnego z programem [Excel.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="c431a-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="c431a-111">Tworzenie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="c431a-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="c431a-112">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="c431a-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c431a-113">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c431a-114">W menu klienta wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="c431a-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="c431a-115">Dla każdego dodawania użytkownika wybierz pozycję **Dodaj subskrypcję,** a następnie podaj informacje, w tym uprawnienia i licencje.</span><span class="sxs-lookup"><span data-stu-id="c431a-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="c431a-116">**Zapisz** zmiany.</span><span class="sxs-lookup"><span data-stu-id="c431a-116">**Save** your changes.</span></span>

5. <span data-ttu-id="c431a-117">Pamiętaj, aby zarejestrować nazwę użytkownika i hasło tymczasowe do wysłania do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c431a-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="c431a-118">Jeśli dodajesz wielu użytkowników po jednym na raz, użyj **opcji Dodaj innego użytkownika.**</span><span class="sxs-lookup"><span data-stu-id="c431a-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="c431a-119">Można również dodać wielu użytkowników jednocześnie, importując plik arkusza kalkulacyjnego CSV zgodny z [programem Excel.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="c431a-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="c431a-120">Możesz poczekać, aż cały zestaw będzie już gotowe, zanim napisze wiadomość e-mail lub będzie drukować nazwy i hasła z ekranu potwierdzenia.</span><span class="sxs-lookup"><span data-stu-id="c431a-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="c431a-121">Dodawanie lub usuwanie licencji użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="c431a-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="c431a-122">Poniższe kroki dotyczą dodawania lub usuwania licencji użytkowników dla produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c431a-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="c431a-123">Aby dodać lub usunąć licencje użytkowników dla opartych na licencjach subskrypcji SaaS na platformie handlowej, zobacz Dodawanie lub usuwanie licencji dla subskrypcji [SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)</span><span class="sxs-lookup"><span data-stu-id="c431a-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="c431a-124">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="c431a-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c431a-125">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c431a-126">W menu klienta wybierz pozycję **Użytkownicy i licencje.**</span><span class="sxs-lookup"><span data-stu-id="c431a-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="c431a-127">Wybierz co najmniej jednego użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-127">Choose one or more users from the list.</span></span> <span data-ttu-id="c431a-128">Jeśli na przykład klient właśnie zakupił nowe licencje i chcesz przypisać je do osób, które jeszcze ich nie mają, możesz użyć opcji Filtruj użytkowników **według...,** aby znaleźć odpowiednią grupę.</span><span class="sxs-lookup"><span data-stu-id="c431a-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="c431a-129">Wybierz pozycję **Zarządzaj licencjami**.</span><span class="sxs-lookup"><span data-stu-id="c431a-129">Select **Manage licenses**.</span></span> <span data-ttu-id="c431a-130">Dokonaj zmian, a następnie **zapisz .**</span><span class="sxs-lookup"><span data-stu-id="c431a-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="c431a-131">W [Azure Marketplace produktu](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)przypisanie licencji i aktywacja są zarządzane za pośrednictwem niezależnego dostawcy oprogramowania, który opublikował produkt.</span><span class="sxs-lookup"><span data-stu-id="c431a-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="c431a-132">Resetowanie hasła użytkownika dla klienta</span><span class="sxs-lookup"><span data-stu-id="c431a-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="c431a-133">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="c431a-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c431a-134">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c431a-135">W menu klienta wybierz pozycję **Użytkownicy i licencje.**</span><span class="sxs-lookup"><span data-stu-id="c431a-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="c431a-136">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="c431a-137">W dolnej części ekranu wybierz pozycję **Resetuj hasło.**</span><span class="sxs-lookup"><span data-stu-id="c431a-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="c431a-138">Wyślij nowe hasło tymczasowe do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c431a-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="c431a-139">Usuwanie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="c431a-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="c431a-140">Z menu **Partner Center** wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="c431a-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="c431a-141">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="c431a-142">W menu klienta wybierz pozycję **Użytkownicy i licencje.**</span><span class="sxs-lookup"><span data-stu-id="c431a-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="c431a-143">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="c431a-144">W dolnej części ekranu wybierz pozycję **Usuń konto użytkownika.**</span><span class="sxs-lookup"><span data-stu-id="c431a-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="c431a-145">Jeśli musisz przywrócić to konto, możesz  je znaleźć na karcie Usunięci użytkownicy na liście **Użytkownicy i licencje** klienta.</span><span class="sxs-lookup"><span data-stu-id="c431a-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="c431a-146">Masz 30 dni na przywrócenie usuniętego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c431a-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="c431a-147">Przywracanie usuniętych kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="c431a-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="c431a-148">Z **Partner Center** wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="c431a-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="c431a-149">Wybierz **pozycję Użytkownicy i licencje.**</span><span class="sxs-lookup"><span data-stu-id="c431a-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="c431a-150">Wybierz **kartę Usunięci użytkownicy (** ). Powinien być **odczytywany (1)** lub większy, gdy istnieją usunięci użytkownicy, którzy mogą zostać przywróconi.</span><span class="sxs-lookup"><span data-stu-id="c431a-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="c431a-151">Zaznacz co najmniej jedno pole wyboru usuniętego użytkownika, a następnie wybierz pozycję **Przywróć.**</span><span class="sxs-lookup"><span data-stu-id="c431a-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="c431a-152">Wszystkie wybrane konta użytkowników zostaną ponownie pojawiające się na **stronie Użytkownicy i licencje.**</span><span class="sxs-lookup"><span data-stu-id="c431a-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c431a-153">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="c431a-153">Next steps</span></span>

- [<span data-ttu-id="c431a-154">Przypisywanie lub odwoływanie licencji dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="c431a-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="c431a-155">Tworzenie wielu użytkowników dla konta klienta</span><span class="sxs-lookup"><span data-stu-id="c431a-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)