---
title: Zarządzanie użytkownikami dla kont klientów
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zarządzanie użytkownikami dla klientów w centrum partnerskim — tworzenie kont użytkowników, Dodawanie lub usuwanie licencji użytkowników, resetowanie haseł oraz usuwanie lub przywracanie kont użytkowników.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756076"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="eecd8-103">Zarządzanie użytkownikami i licencjami użytkowników dla kont klientów</span><span class="sxs-lookup"><span data-stu-id="eecd8-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="eecd8-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="eecd8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="eecd8-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="eecd8-105">Global admin</span></span>
- <span data-ttu-id="eecd8-106">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="eecd8-106">User management admin</span></span>
- <span data-ttu-id="eecd8-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="eecd8-107">Admin agent</span></span>


<span data-ttu-id="eecd8-108">Możesz tworzyć i usuwać nowych użytkowników na koncie klienta.</span><span class="sxs-lookup"><span data-stu-id="eecd8-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="eecd8-109">Można również przywrócić co najmniej jedno konto użytkownika, które zostało wcześniej usunięte w ciągu 30 dni od usunięcia.</span><span class="sxs-lookup"><span data-stu-id="eecd8-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="eecd8-110">Zostaną również przywrócone poprzednie przypisania subskrypcji użytkownika (przy założeniu, że ich poprzednie alokacje są dostępne).</span><span class="sxs-lookup"><span data-stu-id="eecd8-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="eecd8-111">Gdy kupisz nowe subskrypcje dla klienta, klient powinien podać listę wszystkich użytkowników, którzy będą potrzebować kont, ich uprawnień użytkowników i usług, których potrzebuje każdy użytkownik.</span><span class="sxs-lookup"><span data-stu-id="eecd8-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="eecd8-112">Sekcja **Użytkownicy i licencje** na karcie **Klient** pokazuje wszystkich użytkowników utworzonych w dzierżawie określonego klienta, w tym użytkowników, którzy mają licencje zakupione od innego partnera CSP lub z innego kanału zakupu.</span><span class="sxs-lookup"><span data-stu-id="eecd8-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="eecd8-113">Możesz jednocześnie [przypisać subskrypcje do wielu użytkowników](bulk-license-provisioning-for-multiple-users.md) , importując nazwy przy użyciu [pliku arkusza kalkulacyjnego zgodnego z programem Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="eecd8-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="eecd8-114">Tworzenie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="eecd8-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="eecd8-115">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="eecd8-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="eecd8-116">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="eecd8-117">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="eecd8-118">Dla każdego dodawanego użytkownika wybierz pozycję **Dodaj subskrypcję**, a następnie wprowadź informacje, w tym uprawnienia i licencje.</span><span class="sxs-lookup"><span data-stu-id="eecd8-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="eecd8-119">**Zapisz** zmiany.</span><span class="sxs-lookup"><span data-stu-id="eecd8-119">**Save** your changes.</span></span>

5. <span data-ttu-id="eecd8-120">Pamiętaj o zarejestrowaniu nazwy użytkownika i hasła tymczasowego do wysłania do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eecd8-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="eecd8-121">W przypadku dodawania wielu użytkowników pojedynczo przy użyciu **Dodaj innego użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="eecd8-122">Możesz również jednocześnie dodać wielu użytkowników, [importując plik arkusza kalkulacyjnego zgodnego z programem Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="eecd8-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="eecd8-123">Możesz poczekać, aż wszystko będzie gotowe z całego zestawu przed wysłaniem poczty e-mail lub wydrukowaniem nazw i haseł na ekranie potwierdzenia.</span><span class="sxs-lookup"><span data-stu-id="eecd8-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="eecd8-124">Dodawanie lub usuwanie licencji użytkownika dla klienta</span><span class="sxs-lookup"><span data-stu-id="eecd8-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="eecd8-125">Poniższe kroki dotyczą dodawania lub usuwania licencji użytkowników dla produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="eecd8-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="eecd8-126">Aby dodać lub usunąć licencje użytkowników dla subskrypcji SaaS opartych na licencjach w komercyjnej witrynie Marketplace, zobacz [Dodawanie lub usuwanie licencji dla subskrypcji SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="eecd8-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="eecd8-127">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="eecd8-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="eecd8-128">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="eecd8-129">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="eecd8-130">Wybierz co najmniej jednego użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-130">Choose one or more users from the list.</span></span> <span data-ttu-id="eecd8-131">Jeśli na przykład klient zakupił nowe licencje i chcesz przypisać je do osób, które ich nie mają jeszcze, możesz użyć opcji **Filtruj użytkowników przez...** , aby znaleźć odpowiednią grupę.</span><span class="sxs-lookup"><span data-stu-id="eecd8-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="eecd8-132">Wybierz pozycję **Zarządzaj licencjami**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-132">Select **Manage licenses**.</span></span> <span data-ttu-id="eecd8-133">Wprowadź zmiany, a następnie **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="eecd8-134">W przypadku [produktów portalu Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)przypisanie licencji i aktywacja jest zarządzane za pomocą niezależnego dostawcy oprogramowania (ISV), który opublikował produkt.</span><span class="sxs-lookup"><span data-stu-id="eecd8-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="eecd8-135">Resetowanie hasła użytkownika dla klienta</span><span class="sxs-lookup"><span data-stu-id="eecd8-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="eecd8-136">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard) Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="eecd8-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="eecd8-137">W menu Centrum partnerskiego wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="eecd8-138">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="eecd8-139">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="eecd8-140">W dolnej części ekranu wybierz pozycję **Resetuj hasło**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="eecd8-141">Wyślij nowe hasło tymczasowe do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eecd8-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="eecd8-142">Usuwanie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="eecd8-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="eecd8-143">W menu **Centrum partnerskiego** wybierz pozycję **Customers**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="eecd8-144">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="eecd8-145">W menu Klient wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="eecd8-146">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="eecd8-147">W dolnej części ekranu wybierz pozycję **Usuń konto użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="eecd8-148">Jeśli musisz przywrócić to konto, możesz je znaleźć na karcie **usunięci użytkownicy** na liście **Użytkownicy i licencje** klienta.</span><span class="sxs-lookup"><span data-stu-id="eecd8-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="eecd8-149">Użytkownik ma 30 dni na przywrócenie usuniętego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="eecd8-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="eecd8-150">Przywracanie usuniętych kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="eecd8-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="eecd8-151">W menu **Centrum partnerskiego** wybierz pozycję **klienci**, a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="eecd8-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="eecd8-152">Wybierz pozycję **Użytkownicy i licencje**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="eecd8-153">Wybierz kartę **usunięci użytkownicy ()** . Po usunięciu użytkowników, które mogą zostać przywrócone, należy przeczytać **(1)** lub więcej.</span><span class="sxs-lookup"><span data-stu-id="eecd8-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="eecd8-154">Wybierz co najmniej jeden z pól wyboru usuniętych użytkowników, a następnie wybierz pozycję **Przywróć**.</span><span class="sxs-lookup"><span data-stu-id="eecd8-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="eecd8-155">Wszystkie wybrane konta użytkowników zostaną wyświetlone na stronie **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="eecd8-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eecd8-156">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="eecd8-156">Next steps</span></span>

- [<span data-ttu-id="eecd8-157">Przypisywanie lub odwoływanie licencji dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="eecd8-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="eecd8-158">Tworzenie wielu użytkowników dla konta klienta</span><span class="sxs-lookup"><span data-stu-id="eecd8-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)