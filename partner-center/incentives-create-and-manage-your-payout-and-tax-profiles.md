---
title: Wypłaty i profile podatkowe w Centrum partnerskim
ms.topic: how-to
ms.date: 11/12/2020
description: Utwórz wypłatę i profil podatkowy i zarządzaj nimi, aby otrzymywać opłaty za Twoje zachęty. Obejmuje tworzenie i używanie różnych profilów oraz zarządzanie nimi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624242"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="8a566-104">Twórz wypłaty i profile podatków w centrum partnerskim i zarządzaj nimi</span><span class="sxs-lookup"><span data-stu-id="8a566-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="8a566-105">**Odpowiednie role:**</span><span class="sxs-lookup"><span data-stu-id="8a566-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="8a566-106">Administrator zachęt</span><span class="sxs-lookup"><span data-stu-id="8a566-106">Incentives admin</span></span>
- <span data-ttu-id="8a566-107">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="8a566-107">Account admin</span></span>
- <span data-ttu-id="8a566-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="8a566-108">Global admin</span></span>

<span data-ttu-id="8a566-109">Aby można było otrzymać płatność z tytułu programów zachęt dla konkretnej lokalizacji MPN, należy ukończyć rejestrację, dokonując skojarzenia prawidłowego profilu wypłaty i profilu podatkowego z programem i lokalizacją MPN.</span><span class="sxs-lookup"><span data-stu-id="8a566-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="8a566-110">Firma Microsoft będzie korzystać z tego profilu wypłaty i profilu podatkowego w celu realizacji płatności.</span><span class="sxs-lookup"><span data-stu-id="8a566-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="8a566-111">W zależności od zasad programu zachęt może być możliwe wykorzystanie elektronicznego przelewu bankowego lub noty kredytowej przy płatności.</span><span class="sxs-lookup"><span data-stu-id="8a566-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="8a566-112">Role, waluty i inne programy firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="8a566-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="8a566-113">Ważne jest zapoznanie się z poniższymi informacjami przed rozpoczęciem pracy z wypłatą i profilem podatkowym.</span><span class="sxs-lookup"><span data-stu-id="8a566-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="8a566-114">Role i uprawnienia</span><span class="sxs-lookup"><span data-stu-id="8a566-114">Roles and permissions</span></span>

<span data-ttu-id="8a566-115">Musisz być administratorem zachęty, aby wprowadzać informacje o banku i podatku na potrzeby zachęt.</span><span class="sxs-lookup"><span data-stu-id="8a566-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="8a566-116">Jeśli jesteś administratorem konta MPN/, możesz przypisać siebie i/lub współpracownikowi administratora zachęt.</span><span class="sxs-lookup"><span data-stu-id="8a566-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="8a566-117">Jeśli musisz zażądać uprawnień administratora programu zachęty, skontaktuj się z administratorem MPN lub administratorem globalnym. Aby dowiedzieć się, kto w firmie ma te role, zaloguj się na [pulpicie nawigacyjnym Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8a566-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="8a566-118">Na ikonie **ustawień** w prawym górnym rogu wybierz pozycję **Zarządzanie użytkownikami** , a następnie odfiltruj uprawnienia administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="8a566-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="8a566-119">Zachęcaj użytkowników do wyświetlania zarobków i szczegółów płatności oraz raportów, ale nie możesz edytować informacji o banku i podatku.</span><span class="sxs-lookup"><span data-stu-id="8a566-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="8a566-120">Wybierz walutę płatności</span><span class="sxs-lookup"><span data-stu-id="8a566-120">Choose your disbursement currency</span></span>

<span data-ttu-id="8a566-121">Płatności zachęty są wprowadzane w walucie wybranej podczas konfigurowania profilu płatności.</span><span class="sxs-lookup"><span data-stu-id="8a566-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="8a566-122">Płatności będą obliczane przy użyciu stawki wymiany ustawionej miesięcznie przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8a566-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="8a566-123">Użytkownik jest odpowiedzialny za wszelkie zmiany wartości ze względu na wybraną walutę.</span><span class="sxs-lookup"><span data-stu-id="8a566-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="8a566-124">Używanie różnych profilów dla różnych programów firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="8a566-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="8a566-125">Jeśli Twoja firma jest zarejestrowana w wielu programach zachęty, możesz użyć tego samego konta płatności dla wszystkich z nich lub użyć różnych kont płatności dla różnych programów.</span><span class="sxs-lookup"><span data-stu-id="8a566-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="8a566-126">Utwórz wypłaty i profile podatków w centrum partnerskim i zarządzaj nimi</span><span class="sxs-lookup"><span data-stu-id="8a566-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="8a566-127">Poniższe sekcje przeprowadzą Cię przez proces tworzenia i zarządzania profilami płatności i podatków w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="8a566-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="8a566-128">Aby tworzyć profile płatności w centrum partnerskim lub zarządzać nimi, musisz być administratorem zachęty.</span><span class="sxs-lookup"><span data-stu-id="8a566-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="8a566-129">Role zachęty muszą być przypisane do każdej lokalizacji MPN w ramach każdego programu zachęty.</span><span class="sxs-lookup"><span data-stu-id="8a566-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="8a566-130">Aby uzyskać więcej informacji na temat dodawania administratorów zachęty w centrum partnerskim, zobacz [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="8a566-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="8a566-131">Dostęp do sekcji wypłaty i opodatkowania w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="8a566-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="8a566-132">Zaloguj się na [pulpicie nawigacyjnym Centrum partnerskiego](https://partner.microsoft.com/dashboard/) przy użyciu konta Azure Active Directory (Azure AD) (konta firmowego) lub odpowiedniego adresu e-mail, jeśli został przypisany.</span><span class="sxs-lookup"><span data-stu-id="8a566-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="8a566-133">W ramach jednego konta usługi Azure AD można zarejestrować wiele domen.</span><span class="sxs-lookup"><span data-stu-id="8a566-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="8a566-134">Skontaktuj się z administratorem globalnym, aby określić, które domeny są skojarzone.</span><span class="sxs-lookup"><span data-stu-id="8a566-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="8a566-135">Jeśli możesz zalogować się tylko za pomocą @onmicrosoft.com domeny, skontaktuj się z administratorem konta w celu dodania dodatkowych domen do konta usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a566-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="8a566-136">Jeśli zostanie wyświetlony monit o wybranie **konta służbowego** lub **konta osobistego**, wybierz pozycję **konto służbowe**.</span><span class="sxs-lookup"><span data-stu-id="8a566-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="8a566-137">Wybierz ikonę koła zębatego, aby otworzyć menu **Ustawienia** , a następnie wybierz pozycję **Ustawienia konta**.</span><span class="sxs-lookup"><span data-stu-id="8a566-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="8a566-138">W menu **Ustawienia konta** wybierz pozycję **wypłata i podatek**.</span><span class="sxs-lookup"><span data-stu-id="8a566-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="8a566-139">Przypisywanie wypłat i profilów podatkowych do poszczególnych programów</span><span class="sxs-lookup"><span data-stu-id="8a566-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="8a566-140">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/), a następnie wybierz ikonę koła zębatego, aby otworzyć menu **Ustawienia** .</span><span class="sxs-lookup"><span data-stu-id="8a566-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="8a566-141">Wybierz pozycję **Ustawienia konta**, rozwiń **sekcję wypłata i podatek**, a następnie wybierz pozycję **wypłata i przypisywanie profilów podatkowych**.</span><span class="sxs-lookup"><span data-stu-id="8a566-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="8a566-142">Zostanie wyświetlona lista programów.</span><span class="sxs-lookup"><span data-stu-id="8a566-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="8a566-143">Wybierz strzałkę obok programu, aby wyświetlić szczegóły profilu.</span><span class="sxs-lookup"><span data-stu-id="8a566-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="8a566-144">W menu rozwijanym **profil podatkowy** wybierz odpowiedni profil podatkowy lub wybierz opcję utworzenia nowego profilu.</span><span class="sxs-lookup"><span data-stu-id="8a566-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="8a566-145">Po wybraniu opcji tworzenia nowego profilu nastąpi odpowiednie przekierowanie.</span><span class="sxs-lookup"><span data-stu-id="8a566-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="8a566-146">W oknie podręcznym wybierz pozycję Kontynuuj.</span><span class="sxs-lookup"><span data-stu-id="8a566-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="8a566-147">Proces tworzenia nowego profilu podatkowego został podany poniżej.</span><span class="sxs-lookup"><span data-stu-id="8a566-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="8a566-148">Wybierz pozycję **płatność**.</span><span class="sxs-lookup"><span data-stu-id="8a566-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="8a566-149">Jeśli jako formę płatności wybrano opcję **elektronicznego transferu banku** , wybierz odpowiedni profil płatności lub wybierz opcję utworzenia nowego profilu.</span><span class="sxs-lookup"><span data-stu-id="8a566-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="8a566-150">Po wybraniu opcji tworzenia nowego profilu nastąpi odpowiednie przekierowanie.</span><span class="sxs-lookup"><span data-stu-id="8a566-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="8a566-151">W oknie podręcznym wybierz pozycję Kontynuuj.</span><span class="sxs-lookup"><span data-stu-id="8a566-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="8a566-152">Proces tworzenia nowego profilu płatności został przedstawiony poniżej.</span><span class="sxs-lookup"><span data-stu-id="8a566-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="8a566-153">Jeśli jako formę płatności została wybrana **Nota kredytowa** , wykonaj weryfikację.</span><span class="sxs-lookup"><span data-stu-id="8a566-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="8a566-154">Pozwala to upewnić się, że przywoływany numer SAP należy do organizacji.</span><span class="sxs-lookup"><span data-stu-id="8a566-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8a566-155">Jeśli na liście znajduje się wiele jednostek firmy Microsoft, należy wybrać profil płatności dla każdej jednostki.</span><span class="sxs-lookup"><span data-stu-id="8a566-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8a566-156">Dostępność metody płatności zależy od reguł programu zachęty.</span><span class="sxs-lookup"><span data-stu-id="8a566-156">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="8a566-157">Wybierz **walutę**.</span><span class="sxs-lookup"><span data-stu-id="8a566-157">Select the **Currency**.</span></span>

6. <span data-ttu-id="8a566-158">Po zakończeniu wszystkich pól płatności wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="8a566-158">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="8a566-159">Tworzenie profilu bankowego</span><span class="sxs-lookup"><span data-stu-id="8a566-159">Create your bank profile</span></span>

<span data-ttu-id="8a566-160">Profile bankowe są tworzone na poziomie organizacji.</span><span class="sxs-lookup"><span data-stu-id="8a566-160">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="8a566-161">Umożliwia to przypisanie jednego profilu bankowego do wielu programów MPN ID i zachęt w organizacji.</span><span class="sxs-lookup"><span data-stu-id="8a566-161">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="8a566-162">W przypadku zastosowania profilu bankowego do różnych krajów mogą wystąpić wyjątki, ponieważ mogą być stosowane różne reguły bankowości i podatkowej.</span><span class="sxs-lookup"><span data-stu-id="8a566-162">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="8a566-163">Na następujących stronach wymagane są pola z gwiazdką.</span><span class="sxs-lookup"><span data-stu-id="8a566-163">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="8a566-164">Jeśli nie wiesz, co to jest pole, wybierz ikonę informacji.</span><span class="sxs-lookup"><span data-stu-id="8a566-164">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="8a566-165">Na stronie **szczegóły** wypełnij następujące pola: **Nazwa profilu:** wprowadź unikatową nazwę identyfikującą ten profil płatności.</span><span class="sxs-lookup"><span data-stu-id="8a566-165">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="8a566-166">**Lokalizacja konta bankowego:** Kraj, w którym znajduje się bank firmy.</span><span class="sxs-lookup"><span data-stu-id="8a566-166">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="8a566-167">**Forma płatności:** Preferowana metoda płatności w centrum partnerskim to elektroniczny transfer bankowy.</span><span class="sxs-lookup"><span data-stu-id="8a566-167">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="8a566-168">Wybierz opcję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="8a566-168">Select **Next**.</span></span>

3. <span data-ttu-id="8a566-169">Na stronie **konto bankowe** wprowadź informacje.</span><span class="sxs-lookup"><span data-stu-id="8a566-169">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="8a566-170">Pola wyświetlane na tej stronie różnią się w zależności od kraju.</span><span class="sxs-lookup"><span data-stu-id="8a566-170">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="8a566-171">Wybierz opcję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="8a566-171">Select **Next**.</span></span>

5. <span data-ttu-id="8a566-172">Na stronie **beneficjent** wprowadź odpowiednie informacje.</span><span class="sxs-lookup"><span data-stu-id="8a566-172">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="8a566-173">Beneficjentem jest osoba w firmie, którą będzie mogła skontaktować się z kontem, jeśli trzeba omówić Twoje konto.</span><span class="sxs-lookup"><span data-stu-id="8a566-173">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="8a566-174">Po zakończeniu pól wybierz pozycję **Zakończ**, a następnie wybierz pozycję **Potwierdź** , aby utworzyć profil banku.</span><span class="sxs-lookup"><span data-stu-id="8a566-174">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="8a566-175">Nastąpi przekierowanie do strony z **profilami wypłaty i podatkiem** .</span><span class="sxs-lookup"><span data-stu-id="8a566-175">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="8a566-176">Stan nowego profilu będzie odzwierciedlać **oczekiwanie na zweryfikowanie firmy Microsoft** , dopóki weryfikacja nie zostanie ukończona.</span><span class="sxs-lookup"><span data-stu-id="8a566-176">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="8a566-177">Ten proces może potrwać do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="8a566-177">This process may take up to 48 hours.</span></span> <span data-ttu-id="8a566-178">Po zakończeniu walidacji stan Twojego profilu będzie odzwierciedlać **zatwierdzenie** lub **wymagane działanie**.</span><span class="sxs-lookup"><span data-stu-id="8a566-178">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="8a566-179">Jeśli **wymagana jest akcja**, powtórz powyższe kroki, podając wymagane informacje.</span><span class="sxs-lookup"><span data-stu-id="8a566-179">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="8a566-180">Utwórz swój profil podatkowy</span><span class="sxs-lookup"><span data-stu-id="8a566-180">Create your tax profile</span></span>

<span data-ttu-id="8a566-181">Poniższa procedura umożliwia firmie Microsoft podanie informacji podatkowych wymaganych przez organizację.</span><span class="sxs-lookup"><span data-stu-id="8a566-181">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="8a566-182">Strony w tej sekcji są dynamiczne i różnią się w zależności od kraju lub regionu.</span><span class="sxs-lookup"><span data-stu-id="8a566-182">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="8a566-183">Jeśli potrzebujesz pomocy przy identyfikacji poprawnych informacji podatkowych, skontaktuj się z odpowiednimi źródłami rządowymi w danym kraju.</span><span class="sxs-lookup"><span data-stu-id="8a566-183">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="8a566-184">W przypadku firm partnerskich u Ameryki Północnej, jeśli potrzebne są informacje dotyczące kończenia formularzy W8 lub W9, następujące adresy przekazują użytkownika do lokacji urzędu skarbowego:</span><span class="sxs-lookup"><span data-stu-id="8a566-184">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="8a566-185">Wprowadź tylko szczegóły dla swojej firmy.</span><span class="sxs-lookup"><span data-stu-id="8a566-185">Enter only details for your company.</span></span> <span data-ttu-id="8a566-186">Nigdy nie wprowadzaj szczegółów osobistych.</span><span class="sxs-lookup"><span data-stu-id="8a566-186">Never enter personal details.</span></span>

1. <span data-ttu-id="8a566-187">Na stronie **profil biznesowy** Wypełnij wymagane pola, a następnie wybierz przycisk **dalej**.</span><span class="sxs-lookup"><span data-stu-id="8a566-187">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="8a566-188">Na stronie **Instalator** wybierz opcję, która ma zastosowanie do Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="8a566-188">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="8a566-189">Wybierz opcję po lewej stronie, jeśli Twoja firma jest włączona tylko do Stany Zjednoczone lub jeśli ten profil jest przeznaczony dla osoby.</span><span class="sxs-lookup"><span data-stu-id="8a566-189">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="8a566-190">Wybierz opcję po prawej stronie, jeśli Twoja firma jest wbudowana poza Stany Zjednoczone, a następnie wybierz z listy swój kraj/region.</span><span class="sxs-lookup"><span data-stu-id="8a566-190">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="8a566-191">Wybierz opcję **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="8a566-191">Select **Next**.</span></span> 

4. <span data-ttu-id="8a566-192">Na stronie **stan podatkowy** wprowadź wymagane informacje, a następnie wybierz przycisk **dalej**.</span><span class="sxs-lookup"><span data-stu-id="8a566-192">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="8a566-193">Pola na tej stronie różnią się w zależności od kraju.</span><span class="sxs-lookup"><span data-stu-id="8a566-193">Fields on this page will vary by country.</span></span> <span data-ttu-id="8a566-194">Twoje szczegóły.</span><span class="sxs-lookup"><span data-stu-id="8a566-194">your details.</span></span> 

5. <span data-ttu-id="8a566-195">Na stronie **dodatkowe dokumenty** wymagane pola i wybierz przycisk **dalej**.</span><span class="sxs-lookup"><span data-stu-id="8a566-195">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="8a566-196">Wybierz pozycję **Przeglądaj** , aby przekazać dokumenty wymagane przez kraj lub region.</span><span class="sxs-lookup"><span data-stu-id="8a566-196">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="8a566-197">Gdy zostanie wyświetlona nazwa dokumentu, wybierz pozycję **Przekaż**.</span><span class="sxs-lookup"><span data-stu-id="8a566-197">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="8a566-198">Jeśli musisz usunąć dokument, wybierz pozycję **Usuń**.</span><span class="sxs-lookup"><span data-stu-id="8a566-198">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="8a566-199">Aby zapisać i kontynuować, wybierz pozycję **Zakończ**.</span><span class="sxs-lookup"><span data-stu-id="8a566-199">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="8a566-200">W oknie podręcznym wybierz pozycję **Potwierdź** .</span><span class="sxs-lookup"><span data-stu-id="8a566-200">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="8a566-201">Nastąpi powrót do strony **konfiguracji wypłaty i podatku** .</span><span class="sxs-lookup"><span data-stu-id="8a566-201">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a566-202">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="8a566-202">Next steps</span></span>

- [<span data-ttu-id="8a566-203">Często zadawane pytania dotyczące wypłat i podatków</span><span class="sxs-lookup"><span data-stu-id="8a566-203">Common questions about payouts and taxes</span></span>](payout-faq.md)
