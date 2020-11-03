---
title: Wypłaty i profile podatkowe w Centrum partnerskim
ms.topic: how-to
ms.date: 09/11/2020
description: Utwórz wypłatę i profil podatkowy i zarządzaj nimi, aby otrzymywać opłaty za Twoje zachęty. Obejmuje tworzenie i używanie różnych profilów oraz zarządzanie nimi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ca2ffe992ff92b98546934f4a249779f39179acb
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530603"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="9080e-104">Twórz wypłaty i profile podatków w centrum partnerskim i zarządzaj nimi</span><span class="sxs-lookup"><span data-stu-id="9080e-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="9080e-105">**Dotyczy:**</span><span class="sxs-lookup"><span data-stu-id="9080e-105">**Applies to:**</span></span>

- <span data-ttu-id="9080e-106">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="9080e-106">Partner Center</span></span>

<span data-ttu-id="9080e-107">**Odpowiednie role:**</span><span class="sxs-lookup"><span data-stu-id="9080e-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="9080e-108">Administrator zachęt</span><span class="sxs-lookup"><span data-stu-id="9080e-108">Incentives admin</span></span>
- <span data-ttu-id="9080e-109">Administrator rozliczeń</span><span class="sxs-lookup"><span data-stu-id="9080e-109">Billing admin</span></span>
- <span data-ttu-id="9080e-110">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="9080e-110">Global admin</span></span>

<span data-ttu-id="9080e-111">Aby można było otrzymać płatność z tytułu programów zachęt dla konkretnej lokalizacji MPN, należy ukończyć rejestrację, dokonując skojarzenia prawidłowego profilu wypłaty i profilu podatkowego z programem i lokalizacją MPN.</span><span class="sxs-lookup"><span data-stu-id="9080e-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="9080e-112">Firma Microsoft będzie korzystać z tego profilu wypłaty i profilu podatkowego w celu realizacji płatności.</span><span class="sxs-lookup"><span data-stu-id="9080e-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="9080e-113">W zależności od zasad programu zachęt może być możliwe wykorzystanie elektronicznego przelewu bankowego lub noty kredytowej przy płatności.</span><span class="sxs-lookup"><span data-stu-id="9080e-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="9080e-114">Role, waluty i inne programy firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="9080e-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="9080e-115">Ważne jest zapoznanie się z poniższymi informacjami przed rozpoczęciem pracy z wypłatą i profilem podatkowym.</span><span class="sxs-lookup"><span data-stu-id="9080e-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="9080e-116">Role i uprawnienia</span><span class="sxs-lookup"><span data-stu-id="9080e-116">Roles and permissions</span></span>

<span data-ttu-id="9080e-117">Musisz być administratorem zachęty, aby wprowadzać informacje o banku i podatku na potrzeby zachęt.</span><span class="sxs-lookup"><span data-stu-id="9080e-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="9080e-118">Jeśli jesteś administratorem konta MPN/, możesz przypisać siebie i/lub współpracownikowi administratora zachęt.</span><span class="sxs-lookup"><span data-stu-id="9080e-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="9080e-119">Jeśli musisz zażądać uprawnień administratora programu zachęty, skontaktuj się z administratorem MPN lub administratorem globalnym. Aby dowiedzieć się, kto w firmie ma te role, zaloguj się na [pulpicie nawigacyjnym Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9080e-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="9080e-120">Na ikonie **ustawień** w prawym górnym rogu wybierz pozycję **Zarządzanie użytkownikami** , a następnie odfiltruj uprawnienia administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="9080e-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="9080e-121">Zachęcaj użytkowników do wyświetlania zarobków i szczegółów płatności oraz raportów, ale nie możesz edytować informacji o banku i podatku.</span><span class="sxs-lookup"><span data-stu-id="9080e-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="9080e-122">Wybierz walutę płatności</span><span class="sxs-lookup"><span data-stu-id="9080e-122">Choose your disbursement currency</span></span>

<span data-ttu-id="9080e-123">Domyślnie opłaty za zachęty są dokonywane w lokalnej walucie każdej jednostki.</span><span class="sxs-lookup"><span data-stu-id="9080e-123">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="9080e-124">Podczas konfigurowania profilu można określić inną walutę.</span><span class="sxs-lookup"><span data-stu-id="9080e-124">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="9080e-125">Płatności będą obliczane przy użyciu stawki wymiany ustawionej miesięcznie przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9080e-125">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="9080e-126">Użytkownik jest odpowiedzialny za wszelkie zmiany wartości ze względu na wybraną walutę.</span><span class="sxs-lookup"><span data-stu-id="9080e-126">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="9080e-127">Informacje dotyczące banku i podatku oraz inne programy</span><span class="sxs-lookup"><span data-stu-id="9080e-127">Bank and tax information and other programs</span></span>

<span data-ttu-id="9080e-128">Podaj informacje opisane poniżej, nawet jeśli firma Microsoft używa już danych bankowych do płatności.</span><span class="sxs-lookup"><span data-stu-id="9080e-128">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="9080e-129">Pozwala to zapewnić prywatność i bezpieczeństwo danych firmy, ponieważ kopiowanie profilu do nowego narzędzia może ujawnić poufne informacje.</span><span class="sxs-lookup"><span data-stu-id="9080e-129">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="9080e-130">Przechodzenie przez ten proces jest również dobrym sposobem upewnienia się, że dane są kompletne i dokładne.</span><span class="sxs-lookup"><span data-stu-id="9080e-130">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="9080e-131">Używanie różnych profilów dla różnych programów firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="9080e-131">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="9080e-132">W ramach sprzedaży detalicznej opłaty za każdy z pięciu programów zachęty sprzedaży detalicznej mogą przejść do tego samego konta bankowego.</span><span class="sxs-lookup"><span data-stu-id="9080e-132">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="9080e-133">Alternatywnie możesz wybrać opcję, aby płatności za pośrednictwem usługi w wersji zakupionej w sieci sprzedaży były dostępne na jednym koncie bankowym.</span><span class="sxs-lookup"><span data-stu-id="9080e-133">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="9080e-134">Utwórz wypłaty i profile podatków w centrum partnerskim i zarządzaj nimi</span><span class="sxs-lookup"><span data-stu-id="9080e-134">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="9080e-135">Poniższe sekcje przeprowadzą Cię przez proces tworzenia i zarządzania profilami płatności i podatków w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="9080e-135">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="9080e-136">Aby tworzyć profile płatności w centrum partnerskim lub zarządzać nimi, musisz być administratorem zachęty.</span><span class="sxs-lookup"><span data-stu-id="9080e-136">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="9080e-137">Role zachęty muszą być przypisane do każdej lokalizacji MPN w ramach każdego programu zachęty.</span><span class="sxs-lookup"><span data-stu-id="9080e-137">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="9080e-138">Aby uzyskać więcej informacji na temat dodawania administratorów zachęty w centrum partnerskim, zobacz [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="9080e-138">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="9080e-139">Dostęp do sekcji wypłaty i opodatkowania w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="9080e-139">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="9080e-140">Zaloguj się na [pulpicie nawigacyjnym Centrum partnerskiego](https://partner.microsoft.com/dashboard/) przy użyciu konta Azure Active Directory (Azure AD) (konta firmowego) lub odpowiedniego adresu e-mail, jeśli został przypisany.</span><span class="sxs-lookup"><span data-stu-id="9080e-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="9080e-141">W ramach jednego konta usługi Azure AD można zarejestrować wiele domen.</span><span class="sxs-lookup"><span data-stu-id="9080e-141">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="9080e-142">Skontaktuj się z administratorem globalnym, aby określić, które domeny są skojarzone.</span><span class="sxs-lookup"><span data-stu-id="9080e-142">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="9080e-143">Jeśli możesz zalogować się tylko za pomocą @onmicrosoft.com domeny, skontaktuj się z administratorem konta w celu dodania dodatkowych domen do konta usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9080e-143">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="9080e-144">Jeśli zostanie wyświetlony monit o wybranie **konta służbowego** lub **konta osobistego** , wybierz pozycję **konto służbowe** .</span><span class="sxs-lookup"><span data-stu-id="9080e-144">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account** .</span></span>

2. <span data-ttu-id="9080e-145">Wybierz ikonę koła zębatego, aby otworzyć menu **Ustawienia** , a następnie wybierz pozycję **Ustawienia partnera** .</span><span class="sxs-lookup"><span data-stu-id="9080e-145">Select the gear icon to open the **Settings** menu, and then select **Partner settings** .</span></span>

3. <span data-ttu-id="9080e-146">W menu **Ustawienia konta** wybierz pozycję **wypłata i podatek** .</span><span class="sxs-lookup"><span data-stu-id="9080e-146">In the **Account settings** menu, select **Payout and tax** .</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="9080e-147">Przypisywanie wypłat i profilów podatkowych do poszczególnych programów</span><span class="sxs-lookup"><span data-stu-id="9080e-147">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="9080e-148">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/), a następnie wybierz ikonę koła zębatego, aby otworzyć menu **Ustawienia** .</span><span class="sxs-lookup"><span data-stu-id="9080e-148">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="9080e-149">Wybierz pozycję **Ustawienia partnera** , rozwiń **sekcję wypłata i podatek** , a następnie wybierz pozycję **wypłata i przypisanie profilu podatku** .</span><span class="sxs-lookup"><span data-stu-id="9080e-149">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment** .</span></span> 
   
   <span data-ttu-id="9080e-150">Zostanie wyświetlona lista programów.</span><span class="sxs-lookup"><span data-stu-id="9080e-150">A list of your programs will be displayed.</span></span> <span data-ttu-id="9080e-151">Wybierz strzałkę obok programu, aby wyświetlić szczegóły profilu.</span><span class="sxs-lookup"><span data-stu-id="9080e-151">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="9080e-152">W menu rozwijanym **profil podatkowy** wybierz odpowiedni profil podatkowy lub wybierz opcję utworzenia nowego profilu.</span><span class="sxs-lookup"><span data-stu-id="9080e-152">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="9080e-153">Po wybraniu opcji tworzenia nowego profilu nastąpi odpowiednie przekierowanie.</span><span class="sxs-lookup"><span data-stu-id="9080e-153">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="9080e-154">W oknie podręcznym wybierz pozycję Kontynuuj.</span><span class="sxs-lookup"><span data-stu-id="9080e-154">Select Continue in the pop-up window.</span></span> <span data-ttu-id="9080e-155">Proces tworzenia nowego profilu podatkowego został podany poniżej.</span><span class="sxs-lookup"><span data-stu-id="9080e-155">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="9080e-156">Wybierz pozycję **płatność** .</span><span class="sxs-lookup"><span data-stu-id="9080e-156">Select **Payment method** .</span></span>

   - <span data-ttu-id="9080e-157">Jeśli jako formę płatności wybrano opcję **elektronicznego transferu banku** , wybierz odpowiedni profil płatności lub wybierz opcję utworzenia nowego profilu.</span><span class="sxs-lookup"><span data-stu-id="9080e-157">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="9080e-158">Po wybraniu opcji tworzenia nowego profilu nastąpi odpowiednie przekierowanie.</span><span class="sxs-lookup"><span data-stu-id="9080e-158">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="9080e-159">W oknie podręcznym wybierz pozycję Kontynuuj.</span><span class="sxs-lookup"><span data-stu-id="9080e-159">Select Continue in the pop-up window.</span></span> <span data-ttu-id="9080e-160">Proces tworzenia nowego profilu płatności został przedstawiony poniżej.</span><span class="sxs-lookup"><span data-stu-id="9080e-160">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="9080e-161">Jeśli jako formę płatności została wybrana **Nota kredytowa** , wykonaj weryfikację.</span><span class="sxs-lookup"><span data-stu-id="9080e-161">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="9080e-162">Pozwala to upewnić się, że przywoływany numer SAP należy do organizacji.</span><span class="sxs-lookup"><span data-stu-id="9080e-162">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="9080e-163">Jeśli na liście znajduje się wiele jednostek firmy Microsoft, należy wybrać profil płatności dla każdej jednostki.</span><span class="sxs-lookup"><span data-stu-id="9080e-163">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="9080e-164">Dostępność metody płatności zależy od reguł programu zachęty.</span><span class="sxs-lookup"><span data-stu-id="9080e-164">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="9080e-165">Wybierz **walutę** .</span><span class="sxs-lookup"><span data-stu-id="9080e-165">Select the **Currency** .</span></span>

6. <span data-ttu-id="9080e-166">Po zakończeniu wszystkich pól płatności wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="9080e-166">When you’ve completed all of the payment fields, select **Submit** .</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="9080e-167">Tworzenie profilu bankowego</span><span class="sxs-lookup"><span data-stu-id="9080e-167">Create your bank profile</span></span>

<span data-ttu-id="9080e-168">Profile bankowe są tworzone na poziomie organizacji.</span><span class="sxs-lookup"><span data-stu-id="9080e-168">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="9080e-169">Umożliwia to przypisanie jednego profilu bankowego do wielu programów MPN ID i zachęt w organizacji.</span><span class="sxs-lookup"><span data-stu-id="9080e-169">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="9080e-170">W przypadku zastosowania profilu bankowego do różnych krajów mogą wystąpić wyjątki, ponieważ mogą być stosowane różne reguły bankowości i podatkowej.</span><span class="sxs-lookup"><span data-stu-id="9080e-170">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="9080e-171">Na następujących stronach wymagane są pola z gwiazdką.</span><span class="sxs-lookup"><span data-stu-id="9080e-171">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="9080e-172">Jeśli nie wiesz, co to jest pole, wybierz ikonę informacji.</span><span class="sxs-lookup"><span data-stu-id="9080e-172">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="9080e-173">Na stronie **szczegóły** wypełnij następujące pola: **Nazwa profilu:** wprowadź unikatową nazwę identyfikującą ten profil płatności.</span><span class="sxs-lookup"><span data-stu-id="9080e-173">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="9080e-174">**Lokalizacja konta bankowego:** Kraj, w którym znajduje się bank firmy.</span><span class="sxs-lookup"><span data-stu-id="9080e-174">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="9080e-175">**Forma płatności:** Preferowana metoda płatności w centrum partnerskim to elektroniczny transfer bankowy.</span><span class="sxs-lookup"><span data-stu-id="9080e-175">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="9080e-176">Wybierz pozycję **Dalej** .</span><span class="sxs-lookup"><span data-stu-id="9080e-176">Select **Next** .</span></span>

3. <span data-ttu-id="9080e-177">Na stronie **konto bankowe** wprowadź informacje.</span><span class="sxs-lookup"><span data-stu-id="9080e-177">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="9080e-178">Pola wyświetlane na tej stronie różnią się w zależności od kraju.</span><span class="sxs-lookup"><span data-stu-id="9080e-178">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="9080e-179">Wybierz pozycję **Dalej** .</span><span class="sxs-lookup"><span data-stu-id="9080e-179">Select **Next** .</span></span>

5. <span data-ttu-id="9080e-180">Na stronie **beneficjent** wprowadź odpowiednie informacje.</span><span class="sxs-lookup"><span data-stu-id="9080e-180">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="9080e-181">Beneficjentem jest osoba w firmie, którą będzie mogła skontaktować się z kontem, jeśli trzeba omówić Twoje konto.</span><span class="sxs-lookup"><span data-stu-id="9080e-181">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="9080e-182">Po zakończeniu pól wybierz pozycję **Zakończ** , a następnie wybierz pozycję **Potwierdź** , aby utworzyć profil banku.</span><span class="sxs-lookup"><span data-stu-id="9080e-182">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="9080e-183">Nastąpi przekierowanie do strony z **profilami wypłaty i podatkiem** .</span><span class="sxs-lookup"><span data-stu-id="9080e-183">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="9080e-184">Stan nowego profilu będzie odzwierciedlać **oczekiwanie na zweryfikowanie firmy Microsoft** , dopóki weryfikacja nie zostanie ukończona.</span><span class="sxs-lookup"><span data-stu-id="9080e-184">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="9080e-185">Ten proces może potrwać do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="9080e-185">This process may take up to 48 hours.</span></span> <span data-ttu-id="9080e-186">Po zakończeniu walidacji stan Twojego profilu będzie odzwierciedlać **zatwierdzenie** lub **wymagane działanie** .</span><span class="sxs-lookup"><span data-stu-id="9080e-186">Once validation has been completed, your profile status will reflect either **Approved** or **Action required** .</span></span> <span data-ttu-id="9080e-187">Jeśli **wymagana jest akcja** , powtórz powyższe kroki, podając wymagane informacje.</span><span class="sxs-lookup"><span data-stu-id="9080e-187">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="9080e-188">Utwórz swój profil podatkowy</span><span class="sxs-lookup"><span data-stu-id="9080e-188">Create your tax profile</span></span>

<span data-ttu-id="9080e-189">Poniższa procedura umożliwia firmie Microsoft podanie informacji podatkowych wymaganych przez organizację.</span><span class="sxs-lookup"><span data-stu-id="9080e-189">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="9080e-190">Strony w tej sekcji są dynamiczne i różnią się w zależności od kraju lub regionu.</span><span class="sxs-lookup"><span data-stu-id="9080e-190">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="9080e-191">Jeśli potrzebujesz pomocy przy identyfikacji poprawnych informacji podatkowych, skontaktuj się z odpowiednimi źródłami rządowymi w danym kraju.</span><span class="sxs-lookup"><span data-stu-id="9080e-191">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="9080e-192">W przypadku firm partnerskich u Ameryki Północnej, jeśli potrzebne są informacje dotyczące kończenia formularzy W8 lub W9, następujące adresy przekazują użytkownika do lokacji urzędu skarbowego:</span><span class="sxs-lookup"><span data-stu-id="9080e-192">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="9080e-193">Wprowadź tylko szczegóły dla swojej firmy.</span><span class="sxs-lookup"><span data-stu-id="9080e-193">Enter only details for your company.</span></span> <span data-ttu-id="9080e-194">Nigdy nie wprowadzaj szczegółów osobistych.</span><span class="sxs-lookup"><span data-stu-id="9080e-194">Never enter personal details.</span></span>

1. <span data-ttu-id="9080e-195">Na stronie **profil biznesowy** Wypełnij wymagane pola, a następnie wybierz przycisk **dalej** .</span><span class="sxs-lookup"><span data-stu-id="9080e-195">On the **Business Profile** page, complete the required fields and then select **Next** .</span></span> 

2. <span data-ttu-id="9080e-196">Na stronie **Instalator** wybierz opcję, która ma zastosowanie do Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="9080e-196">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="9080e-197">Wybierz opcję po lewej stronie, jeśli Twoja firma jest włączona tylko do Stany Zjednoczone lub jeśli ten profil jest przeznaczony dla osoby.</span><span class="sxs-lookup"><span data-stu-id="9080e-197">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="9080e-198">Wybierz opcję po prawej stronie, jeśli Twoja firma jest wbudowana poza Stany Zjednoczone, a następnie wybierz z listy swój kraj/region.</span><span class="sxs-lookup"><span data-stu-id="9080e-198">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="9080e-199">Wybierz pozycję **Dalej** .</span><span class="sxs-lookup"><span data-stu-id="9080e-199">Select **Next** .</span></span> 

4. <span data-ttu-id="9080e-200">Na stronie **stan podatkowy** wprowadź wymagane informacje, a następnie wybierz przycisk **dalej** .</span><span class="sxs-lookup"><span data-stu-id="9080e-200">On the **Tax status** page, enter the required information, and then select **Next** .</span></span> <span data-ttu-id="9080e-201">Pola na tej stronie różnią się w zależności od kraju.</span><span class="sxs-lookup"><span data-stu-id="9080e-201">Fields on this page will vary by country.</span></span> <span data-ttu-id="9080e-202">Twoje szczegóły.</span><span class="sxs-lookup"><span data-stu-id="9080e-202">your details.</span></span> 

5. <span data-ttu-id="9080e-203">Na stronie **dodatkowe dokumenty** wymagane pola i wybierz przycisk **dalej** .</span><span class="sxs-lookup"><span data-stu-id="9080e-203">On the **Additional documentation** page, the required fields and select **Next** .</span></span> 

6. <span data-ttu-id="9080e-204">Wybierz pozycję **Przeglądaj** , aby przekazać dokumenty wymagane przez kraj lub region.</span><span class="sxs-lookup"><span data-stu-id="9080e-204">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="9080e-205">Gdy zostanie wyświetlona nazwa dokumentu, wybierz pozycję **Przekaż** .</span><span class="sxs-lookup"><span data-stu-id="9080e-205">When the document name is shown, select **Upload** .</span></span> 

7. <span data-ttu-id="9080e-206">Jeśli musisz usunąć dokument, wybierz pozycję **Usuń** .</span><span class="sxs-lookup"><span data-stu-id="9080e-206">If you need to remove the document, select **Remove** .</span></span>

8. <span data-ttu-id="9080e-207">Aby zapisać i kontynuować, wybierz pozycję **Zakończ** .</span><span class="sxs-lookup"><span data-stu-id="9080e-207">To save and continue, select **Finish** .</span></span>

9. <span data-ttu-id="9080e-208">W oknie podręcznym wybierz pozycję **Potwierdź** .</span><span class="sxs-lookup"><span data-stu-id="9080e-208">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="9080e-209">Nastąpi powrót do strony **konfiguracji wypłaty i podatku** .</span><span class="sxs-lookup"><span data-stu-id="9080e-209">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9080e-210">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="9080e-210">Next steps</span></span>

- [<span data-ttu-id="9080e-211">Zachęty wypłaty i profil podatkowy — często zadawane pytania</span><span class="sxs-lookup"><span data-stu-id="9080e-211">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
