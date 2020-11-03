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
ms.openlocfilehash: fc208283e0ed8c0f164a44cc9bd70260b8671c6e
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530628"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="fc76f-103">Zarządzanie użytkownikami i licencjami użytkowników dla kont klientów</span><span class="sxs-lookup"><span data-stu-id="fc76f-103">Manage users and user licenses for customer accounts</span></span>

<span data-ttu-id="fc76f-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="fc76f-104">**Applies to**</span></span>

- <span data-ttu-id="fc76f-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="fc76f-105">Partner Center</span></span>

<span data-ttu-id="fc76f-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="fc76f-106">**Appropriate roles**</span></span>

- <span data-ttu-id="fc76f-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="fc76f-107">Global admin</span></span>
- <span data-ttu-id="fc76f-108">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="fc76f-108">User management admin</span></span>
- <span data-ttu-id="fc76f-109">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="fc76f-109">Admin agent</span></span>
- <span data-ttu-id="fc76f-110">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="fc76f-110">Sales agent</span></span>
- <span data-ttu-id="fc76f-111">Agent pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="fc76f-111">Helpdesk agent</span></span>

<span data-ttu-id="fc76f-112">Możesz tworzyć i usuwać nowych użytkowników na koncie klienta.</span><span class="sxs-lookup"><span data-stu-id="fc76f-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="fc76f-113">Można również przywrócić co najmniej jedno konto użytkownika, które zostało wcześniej usunięte w ciągu 30 dni od usunięcia.</span><span class="sxs-lookup"><span data-stu-id="fc76f-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="fc76f-114">Zostaną również przywrócone poprzednie przypisania subskrypcji użytkownika (przy założeniu, że ich poprzednie alokacje są dostępne).</span><span class="sxs-lookup"><span data-stu-id="fc76f-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="fc76f-115">Gdy kupisz nowe subskrypcje dla klienta, klient powinien podać listę wszystkich użytkowników, którzy będą potrzebować kont, ich uprawnień użytkowników i usług, których potrzebuje każdy użytkownik.</span><span class="sxs-lookup"><span data-stu-id="fc76f-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="fc76f-116">Możesz jednocześnie [przypisać subskrypcje do wielu użytkowników](bulk-license-provisioning-for-multiple-users.md) , importując nazwy przy użyciu [pliku arkusza kalkulacyjnego zgodnego z programem Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="fc76f-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="fc76f-117">Tworzenie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="fc76f-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="fc76f-118">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="fc76f-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fc76f-119">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-119">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="fc76f-120">W menu Klient wybierz pozycję **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-120">In the customer menu, select **Users and licenses** .</span></span>

4. <span data-ttu-id="fc76f-121">Dla każdego dodawanego użytkownika wybierz pozycję **Dodaj subskrypcję** , a następnie wprowadź informacje, w tym uprawnienia i licencje.</span><span class="sxs-lookup"><span data-stu-id="fc76f-121">For each user you add, select **Add subscription** , then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="fc76f-122">**Zapisz** zmiany.</span><span class="sxs-lookup"><span data-stu-id="fc76f-122">**Save** your changes.</span></span>

5. <span data-ttu-id="fc76f-123">Pamiętaj o zarejestrowaniu nazwy użytkownika i hasła tymczasowego do wysłania do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="fc76f-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="fc76f-124">W przypadku dodawania wielu użytkowników pojedynczo przy użyciu **Dodaj innego użytkownika** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-124">If you are adding multiple users one at a time use **Add another user** .</span></span>

7. <span data-ttu-id="fc76f-125">Możesz również jednocześnie dodać wielu użytkowników, [importując plik arkusza kalkulacyjnego zgodnego z programem Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="fc76f-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="fc76f-126">Możesz poczekać, aż wszystko będzie gotowe z całego zestawu przed wysłaniem poczty e-mail lub wydrukowaniem nazw i haseł na ekranie potwierdzenia.</span><span class="sxs-lookup"><span data-stu-id="fc76f-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="fc76f-127">Dodawanie lub usuwanie licencji użytkownika dla klienta</span><span class="sxs-lookup"><span data-stu-id="fc76f-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="fc76f-128">Poniższe kroki dotyczą dodawania lub usuwania licencji użytkowników dla produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fc76f-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="fc76f-129">Aby dodać lub usunąć licencje użytkowników dla subskrypcji SaaS opartych na licencjach w komercyjnej witrynie Marketplace, zobacz [Dodawanie lub usuwanie licencji dla subskrypcji SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="fc76f-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="fc76f-130">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="fc76f-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fc76f-131">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-131">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="fc76f-132">W menu Klient wybierz pozycję **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-132">In the customer menu, select **Users and licenses** .</span></span>

4. <span data-ttu-id="fc76f-133">Wybierz co najmniej jednego użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-133">Choose one or more users from the list.</span></span> <span data-ttu-id="fc76f-134">Jeśli na przykład klient zakupił nowe licencje i chcesz przypisać je do osób, które ich nie mają jeszcze, możesz użyć opcji **Filtruj użytkowników przez...** , aby znaleźć odpowiednią grupę.</span><span class="sxs-lookup"><span data-stu-id="fc76f-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="fc76f-135">Wybierz pozycję **Zarządzaj licencjami** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-135">Select **Manage licenses** .</span></span> <span data-ttu-id="fc76f-136">Wprowadź zmiany, a następnie **Zapisz** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-136">Make your changes, then **Save** .</span></span>

> [!NOTE]
> <span data-ttu-id="fc76f-137">W przypadku [produktów portalu Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)przypisanie licencji i aktywacja jest zarządzane za pomocą niezależnego dostawcy oprogramowania (ISV), który opublikował produkt.</span><span class="sxs-lookup"><span data-stu-id="fc76f-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="fc76f-138">Resetowanie hasła użytkownika dla klienta</span><span class="sxs-lookup"><span data-stu-id="fc76f-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="fc76f-139">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="fc76f-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fc76f-140">W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-140">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3.  <span data-ttu-id="fc76f-141">W menu Klient wybierz pozycję **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-141">In the customer menu, select **Users and licenses** .</span></span> <span data-ttu-id="fc76f-142">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="fc76f-143">W dolnej części ekranu wybierz pozycję **Resetuj hasło** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-143">At the bottom of the screen, select **Reset password** .</span></span> 

5.  <span data-ttu-id="fc76f-144">Wyślij nowe hasło tymczasowe do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="fc76f-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="fc76f-145">Usuwanie kont użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="fc76f-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="fc76f-146">W menu **Centrum partnerskiego** wybierz pozycję **Customers** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-146">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="fc76f-147">Wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="fc76f-148">W menu Klient wybierz pozycję **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-148">In the customer menu, select **Users and licenses** .</span></span> <span data-ttu-id="fc76f-149">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="fc76f-150">W dolnej części ekranu wybierz pozycję **Usuń konto użytkownika** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-150">At the bottom of the screen, select **Delete user account** .</span></span>

<span data-ttu-id="fc76f-151">Jeśli musisz przywrócić to konto, możesz je znaleźć na karcie **usunięci użytkownicy** na liście **Użytkownicy i licencje** klienta.</span><span class="sxs-lookup"><span data-stu-id="fc76f-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="fc76f-152">Użytkownik ma 30 dni na przywrócenie usuniętego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="fc76f-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="fc76f-153">Przywracanie usuniętych kont użytkowników</span><span class="sxs-lookup"><span data-stu-id="fc76f-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="fc76f-154">W menu **Centrum partnerskiego** wybierz pozycję **klienci** , a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="fc76f-154">From the **Partner Center** menu, select **Customers** , then choose the customer from the list.</span></span>

2.  <span data-ttu-id="fc76f-155">Wybierz pozycję **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-155">Select **Users and licenses** .</span></span>

3.  <span data-ttu-id="fc76f-156">Wybierz kartę **usunięci użytkownicy ()** . Po usunięciu użytkowników, które mogą zostać przywrócone, należy przeczytać **(1)** lub więcej.</span><span class="sxs-lookup"><span data-stu-id="fc76f-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="fc76f-157">Wybierz co najmniej jeden z pól wyboru usuniętych użytkowników, a następnie wybierz pozycję **Przywróć** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-157">Select one or more of the deleted users' checkboxes and then select **Restore** .</span></span>

    <span data-ttu-id="fc76f-158">Wszystkie wybrane konta użytkowników zostaną wyświetlone na stronie **Użytkownicy i licencje** .</span><span class="sxs-lookup"><span data-stu-id="fc76f-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="fc76f-159">Powiązane tematy</span><span class="sxs-lookup"><span data-stu-id="fc76f-159">Related topics</span></span>


[<span data-ttu-id="fc76f-160">Przypisywanie lub odwoływanie licencji dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="fc76f-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="fc76f-161">Tworzenie wielu użytkowników dla konta klienta</span><span class="sxs-lookup"><span data-stu-id="fc76f-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)