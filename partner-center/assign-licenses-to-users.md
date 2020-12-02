---
title: Zarządzanie użytkownikami i licencjami użytkowników dla kont klientów
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak zarządzać użytkownikami dla klientów w centrum partnerskim, takich jak tworzenie kont użytkowników, Dodawanie lub usuwanie licencji użytkowników, resetowanie haseł użytkowników oraz usuwanie lub przywracanie kont użytkowników.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb7906b006540ef939e443a21855488e9d2c36f9
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474074"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="77b81-103">Zarządzanie użytkownikami i licencjami użytkowników dla kont klientów</span><span class="sxs-lookup"><span data-stu-id="77b81-103">Manage users and user licenses for customer accounts</span></span>

<span data-ttu-id="77b81-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="77b81-104">**Appropriate roles**</span></span>

- <span data-ttu-id="77b81-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="77b81-105">Global admin</span></span>
- <span data-ttu-id="77b81-106">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="77b81-106">User management admin</span></span>
- <span data-ttu-id="77b81-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="77b81-107">Admin agent</span></span>


<span data-ttu-id="77b81-108">Możesz tworzyć i usuwać nowych użytkowników na koncie klienta.</span><span class="sxs-lookup"><span data-stu-id="77b81-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="77b81-109">Można również przywrócić co najmniej jedno konto użytkownika, które zostało wcześniej usunięte w ciągu 30 dni od usunięcia.</span><span class="sxs-lookup"><span data-stu-id="77b81-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="77b81-110">Zostaną również przywrócone poprzednie przypisania subskrypcji użytkownika (przy założeniu, że ich poprzednie alokacje są dostępne).</span><span class="sxs-lookup"><span data-stu-id="77b81-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="77b81-111">Gdy kupisz nowe subskrypcje dla klienta, klient powinien podać listę wszystkich użytkowników, którzy będą potrzebować kont, ich uprawnień użytkowników i usług, których potrzebuje każdy użytkownik.</span><span class="sxs-lookup"><span data-stu-id="77b81-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="77b81-112">Możesz jednocześnie [przypisać subskrypcje do wielu użytkowników](bulk-license-provisioning-for-multiple-users.md) , importując nazwy przy użyciu [pliku arkusza kalkulacyjnego zgodnego z programem Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="77b81-112">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="77b81-113">Tworzenie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="77b81-113">Create user accounts for a customer</span></span>

1. <span data-ttu-id="77b81-114">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="77b81-114">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="77b81-115">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="77b81-116">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="77b81-116">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="77b81-117">Dla każdego dodawanego użytkownika wybierz pozycję **Dodaj subskrypcję**, a następnie wprowadź informacje, w tym uprawnienia i licencje.</span><span class="sxs-lookup"><span data-stu-id="77b81-117">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="77b81-118">**Zapisz** zmiany.</span><span class="sxs-lookup"><span data-stu-id="77b81-118">**Save** your changes.</span></span>

5. <span data-ttu-id="77b81-119">Pamiętaj o zarejestrowaniu nazwy użytkownika i hasła tymczasowego do wysłania do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="77b81-119">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="77b81-120">W przypadku dodawania wielu użytkowników pojedynczo przy użyciu **Dodaj innego użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="77b81-120">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="77b81-121">Możesz również jednocześnie dodać wielu użytkowników, [importując plik arkusza kalkulacyjnego zgodnego z programem Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="77b81-121">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="77b81-122">Możesz poczekać, aż wszystko będzie gotowe z całego zestawu przed wysłaniem poczty e-mail lub wydrukowaniem nazw i haseł na ekranie potwierdzenia.</span><span class="sxs-lookup"><span data-stu-id="77b81-122">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="77b81-123">Dodawanie lub usuwanie licencji użytkownika dla klienta</span><span class="sxs-lookup"><span data-stu-id="77b81-123">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="77b81-124">Poniższe kroki dotyczą dodawania lub usuwania licencji użytkowników dla produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="77b81-124">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="77b81-125">Aby dodać lub usunąć licencje użytkowników dla subskrypcji SaaS opartych na licencjach w komercyjnej witrynie Marketplace, zobacz [Dodawanie lub usuwanie licencji dla subskrypcji SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="77b81-125">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="77b81-126">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="77b81-126">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="77b81-127">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-127">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="77b81-128">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="77b81-128">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="77b81-129">Wybierz co najmniej jednego użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-129">Choose one or more users from the list.</span></span> <span data-ttu-id="77b81-130">Jeśli na przykład klient zakupił nowe licencje i chcesz przypisać je do osób, które ich nie mają jeszcze, możesz użyć opcji **Filtruj użytkowników przez...** , aby znaleźć odpowiednią grupę.</span><span class="sxs-lookup"><span data-stu-id="77b81-130">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="77b81-131">Wybierz pozycję **Zarządzaj licencjami**.</span><span class="sxs-lookup"><span data-stu-id="77b81-131">Select **Manage licenses**.</span></span> <span data-ttu-id="77b81-132">Wprowadź zmiany, a następnie **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="77b81-132">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="77b81-133">W przypadku [produktów portalu Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)przypisanie licencji i aktywacja jest zarządzane za pomocą niezależnego dostawcy oprogramowania (ISV), który opublikował produkt.</span><span class="sxs-lookup"><span data-stu-id="77b81-133">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="77b81-134">Resetowanie hasła użytkownika dla klienta</span><span class="sxs-lookup"><span data-stu-id="77b81-134">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="77b81-135">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="77b81-135">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="77b81-136">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-136">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="77b81-137">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="77b81-137">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="77b81-138">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-138">Choose the user from the list.</span></span>

4.  <span data-ttu-id="77b81-139">W dolnej części ekranu wybierz pozycję **Resetuj hasło**.</span><span class="sxs-lookup"><span data-stu-id="77b81-139">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="77b81-140">Wyślij nowe hasło tymczasowe do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="77b81-140">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="77b81-141">Usuwanie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="77b81-141">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="77b81-142">W menu **Centrum partnerskiego** wybierz pozycję **Customers**.</span><span class="sxs-lookup"><span data-stu-id="77b81-142">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="77b81-143">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-143">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="77b81-144">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="77b81-144">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="77b81-145">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-145">Choose the user from the list.</span></span>

3.  <span data-ttu-id="77b81-146">W dolnej części ekranu wybierz pozycję **Usuń konto użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="77b81-146">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="77b81-147">Jeśli musisz przywrócić to konto, możesz je znaleźć na karcie **usunięci użytkownicy** na liście **Użytkownicy i licencje** klienta.</span><span class="sxs-lookup"><span data-stu-id="77b81-147">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="77b81-148">Użytkownik ma 30 dni na przywrócenie usuniętego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="77b81-148">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="77b81-149">Przywracanie usuniętych kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="77b81-149">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="77b81-150">W menu **Centrum partnerskiego** wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="77b81-150">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="77b81-151">Wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="77b81-151">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="77b81-152">Wybierz kartę **usunięci użytkownicy ()** . Po usunięciu użytkowników, które mogą zostać przywrócone, należy przeczytać **(1)** lub więcej.</span><span class="sxs-lookup"><span data-stu-id="77b81-152">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="77b81-153">Wybierz co najmniej jeden z pól wyboru usuniętych użytkowników, a następnie wybierz pozycję **Przywróć**.</span><span class="sxs-lookup"><span data-stu-id="77b81-153">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="77b81-154">Wszystkie wybrane konta użytkowników zostaną wyświetlone na stronie **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="77b81-154">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="77b81-155">Powiązane tematy</span><span class="sxs-lookup"><span data-stu-id="77b81-155">Related topics</span></span>


[<span data-ttu-id="77b81-156">Przypisywanie lub odwoływanie licencji dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="77b81-156">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="77b81-157">Tworzenie wielu użytkowników dla konta klienta</span><span class="sxs-lookup"><span data-stu-id="77b81-157">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)