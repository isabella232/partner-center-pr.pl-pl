---
title: Zarządzanie lokalizacjami na koncie partnerskim
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak używać identyfikatora MPN Location w programach zachęty, biznesie CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441335"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="38b88-103">Zarządzanie lokalizacjami kont MPN i Dodawanie (usuwanie) lokalizacji</span><span class="sxs-lookup"><span data-stu-id="38b88-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="38b88-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="38b88-104">**Appropriate roles**</span></span>

- <span data-ttu-id="38b88-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="38b88-105">Global admin</span></span>
- <span data-ttu-id="38b88-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="38b88-106">Account admin</span></span>

<span data-ttu-id="38b88-107">IDENTYFIKATOR MPN lokalizacji identyfikuje każdą konkretną lokalizację firmy.</span><span class="sxs-lookup"><span data-stu-id="38b88-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="38b88-108">IDENTYFIKATOR MPN Location służy do rejestrowania w programach zachęty, do firmowego dostawcy rozwiązań w chmurze (CSP) i innych transakcji roboczych.</span><span class="sxs-lookup"><span data-stu-id="38b88-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="38b88-109">Globalny identyfikator MPN jest używany dla działań nietransakcyjnych, takich jak żądania pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="38b88-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="38b88-110">Poniżej przedstawiono typowy scenariusz:</span><span class="sxs-lookup"><span data-stu-id="38b88-110">The following scenario is typical:</span></span>

<span data-ttu-id="38b88-111">Firma Contoso ma swoje konto globalne partnera (PGA) w Wielkiej Brytanii.</span><span class="sxs-lookup"><span data-stu-id="38b88-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="38b88-112">PGA jest zarejestrowaną firmą prawną, a jej globalny identyfikator MPN jest używany do zarządzania wszystkimi nietransakcyjnymi biznesowymi.</span><span class="sxs-lookup"><span data-stu-id="38b88-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="38b88-113">Firma Contoso ma także równorzędne konta firmowe lub działy w innej lokalizacji w Wielkiej Brytanii, Francji i w USA.</span><span class="sxs-lookup"><span data-stu-id="38b88-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="38b88-114">W strukturze konta MPN te PLAs są reprezentowane jako unikatowe lokalizacje MPN identyfikatory.</span><span class="sxs-lookup"><span data-stu-id="38b88-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="38b88-115">PLAs są używane dla transakcji transakcyjnych, takich jak CSP lub programy zachęt.</span><span class="sxs-lookup"><span data-stu-id="38b88-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="38b88-116">Wypłaty są powiązane z określonymi lokalizacjami.</span><span class="sxs-lookup"><span data-stu-id="38b88-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="38b88-117">Istnieje relacja 1-1 między dzierżawą dostawcy usług kryptograficznych i IDENTYFIKATORem lokalizacji MPN.</span><span class="sxs-lookup"><span data-stu-id="38b88-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="38b88-119">Wymagania wstępne w celu dodania nowego konta dla firmy dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="38b88-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="38b88-120">Aby dodać nowe konto biznesowe dostawcy usług kryptograficznych, Zacznij od upewnienia się, że spełniono wymagania wstępne.</span><span class="sxs-lookup"><span data-stu-id="38b88-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="38b88-121">W kraju, w którym ma być prowadzone biznesowe Oprogramowanie CSP, musi znajdować się identyfikator MPN.</span><span class="sxs-lookup"><span data-stu-id="38b88-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="38b88-122">Aby utworzyć nową lokalizację MPN, przeczytaj sekcję "Dodawanie lokalizacji MPN" poniżej.</span><span class="sxs-lookup"><span data-stu-id="38b88-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="38b88-123">Aby utworzyć nową dostawcę CSP pośredniego rejestracji odsprzedawcy, przeczytaj artykuł [współpraca z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="38b88-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="38b88-124">Pamiętaj, aby zalogować się przy użyciu **nowych** poświadczeń dla **nowego** konta dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="38b88-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="38b88-125">Nie używaj istniejących poświadczeń, ponieważ centrum partnerskie sprawdzi, czy masz już konto.</span><span class="sxs-lookup"><span data-stu-id="38b88-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="38b88-126">Zaakceptuj umowę partnera firmy Microsoft i aktywuj konto.</span><span class="sxs-lookup"><span data-stu-id="38b88-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="38b88-127">Jeśli chcesz zarejestrować się jako partner bezpośredniego rozliczania, zapoznaj się z [wymaganiami dotyczącymi bezpośrednich partnerów rozliczeniowych](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="38b88-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="38b88-128">Wyświetlanie lokalizacji MPN</span><span class="sxs-lookup"><span data-stu-id="38b88-128">View your MPN locations</span></span>

1. <span data-ttu-id="38b88-129">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego przy użyciu poświadczeń konta MPN.</span><span class="sxs-lookup"><span data-stu-id="38b88-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="38b88-130">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP)</span><span class="sxs-lookup"><span data-stu-id="38b88-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="38b88-131">Na ikonie **ustawień** wybierz kolejno pozycje **Ustawienia konta**, **profil organizacji** i informacje **prawne**.</span><span class="sxs-lookup"><span data-stu-id="38b88-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="38b88-132">Na karcie **partner** Sprawdź, czy nie jest wyświetlany komunikat o błędzie transparentu z prośbą o naprawienie zmigrowanych lokalizacji z PMC.</span><span class="sxs-lookup"><span data-stu-id="38b88-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="38b88-133">Jeśli lokalizacje nie zostały poprawnie skonfigurowane w kryterium PMC i nie zostały jeszcze przenoszone na komputer, musisz zaktualizować te lokalizacje.</span><span class="sxs-lookup"><span data-stu-id="38b88-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Zrzut ekranu przedstawiający pokazuje, jak aktualizować lokalizację.":::
 
4.  <span data-ttu-id="38b88-135">Na ekranie **Przejrzyj lokalizacje PMC** wybierz pozycję **Aktualizuj**.</span><span class="sxs-lookup"><span data-stu-id="38b88-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="38b88-136">Zaktualizuj następujące pola:</span><span class="sxs-lookup"><span data-stu-id="38b88-136">Update the following fields:</span></span>

- <span data-ttu-id="38b88-137">**Nazwa pola**: Upewnij się, że nazwa lokalizacji firmy jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="38b88-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="38b88-138">Jeśli zostanie wyświetlony zduplikowany błąd, spróbuj zmienić z, na przykład contoso na contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="38b88-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="38b88-139">**Pole podmiotu prawnego**: Upewnij się, że wybrano jednostkę prawną, z którą jest powiązana lokalizacja</span><span class="sxs-lookup"><span data-stu-id="38b88-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="38b88-140">**Wiersz adresu 1 & 2 pola**: Upewnij się, że adres jest poprawny</span><span class="sxs-lookup"><span data-stu-id="38b88-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="38b88-141">**Pola stanu/prowincji & miasto**: Upewnij się, że kombinacja między miastem a stanem jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="38b88-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="38b88-142">Istnieją kraje, w których zostanie zastosowane menu rozwijane służące do wybierania stanu/prowincji, a w innych krajach, w których pole będzie musiało zostać wstawione ręcznie.</span><span class="sxs-lookup"><span data-stu-id="38b88-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="38b88-143">**Pole kod** pocztowy: Upewnij się, że pole kod pocztowy jest zgodne z określonym krajem, regionem, miastom lub adresem.</span><span class="sxs-lookup"><span data-stu-id="38b88-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="38b88-144">**Podstawowe pola informacji kontaktowych**: Upewnij się, że pola Imię i nazwisko są wypełnione oraz że wskazany adres e-mail to służbowy adres e-mail, a nie osobisty (na przykład @outlook.com @live.com itp.).</span><span class="sxs-lookup"><span data-stu-id="38b88-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="38b88-145">**Pole numeru telefonu**: Upewnij się, że numer telefonu nie zawiera znaków specjalnych, spacji ani kodu kraju.</span><span class="sxs-lookup"><span data-stu-id="38b88-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="38b88-146">Wartość wprowadzona w polu numer telefonu zawsze będzie zawierać maksymalnie 10 znaków.</span><span class="sxs-lookup"><span data-stu-id="38b88-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="38b88-147">Jeśli nie ma komunikatu o błędzie, w obszarze  **Ustawienia** wybierz pozycję  **Ustawienia konta**, **profil organizacji**, **identyfikatory**.</span><span class="sxs-lookup"><span data-stu-id="38b88-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="38b88-148">Znajdź identyfikator MPN z typem "Location", który jest zgodny z krajem tego konta dostawcy CSP, i użyj go, aby zakończyć skojarzenie.</span><span class="sxs-lookup"><span data-stu-id="38b88-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="38b88-149">Jeśli nie możesz znaleźć MPN identyfikatora lokalizacji pasującego do konta dostawcy CSP, którego chcesz użyć, możesz dodać nową lokalizację, która utworzy nowy identyfikator MPN.</span><span class="sxs-lookup"><span data-stu-id="38b88-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="38b88-150">Zobacz **Dodaj lokalizację MPN** poniżej.</span><span class="sxs-lookup"><span data-stu-id="38b88-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="38b88-151">Dodaj lokalizację MPN</span><span class="sxs-lookup"><span data-stu-id="38b88-151">Add an MPN location</span></span>

1. <span data-ttu-id="38b88-152">Zaloguj się przy użyciu konta MPN w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="38b88-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="38b88-153">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP).</span><span class="sxs-lookup"><span data-stu-id="38b88-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="38b88-154">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="38b88-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="38b88-155">Na **ikonie ustawień** wybierz **Ustawienia konta** , a następnie wybierz pozycję **profil organizacji**.</span><span class="sxs-lookup"><span data-stu-id="38b88-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="38b88-156">Wybierz pozycję **Legal** , a następnie na karcie **partner** wybierz pozycję **lokalizacje biznesowe,** a następnie kliknij pozycję **Dodaj lokalizację.**</span><span class="sxs-lookup"><span data-stu-id="38b88-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="38b88-157">Podaj wymagane szczegóły, takie jak nazwa firmy, adres i kontakt, dla lokalizacji, która ma zostać dodana do firmy.</span><span class="sxs-lookup"><span data-stu-id="38b88-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="38b88-158">Kliknij pozycję **Dodaj lokalizację**.</span><span class="sxs-lookup"><span data-stu-id="38b88-158">Click **Add location**.</span></span> <span data-ttu-id="38b88-159">Spowoduje to utworzenie nowego identyfikatora MPN dla nowej lokalizacji, z której można korzystać w przypadku transakcji i zachęt dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="38b88-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Dodaj nową firmę prawną":::

> [!NOTE]
> <span data-ttu-id="38b88-161">Po dodaniu lokalizacji w centrum partnerskim nie można jej usunąć.</span><span class="sxs-lookup"><span data-stu-id="38b88-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="38b88-162">Aby zalogować się, zobaczysz **MPN** w menu po lewej stronie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="38b88-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="38b88-163">Usuwanie lokalizacji</span><span class="sxs-lookup"><span data-stu-id="38b88-163">Delete a location</span></span>

<span data-ttu-id="38b88-164">Aby usunąć lokalizację z konta, musisz skontaktować się z [pomocą techniczną partnera](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="38b88-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="38b88-165">Upewnij się, że rozumiesz wpływ tej akcji.</span><span class="sxs-lookup"><span data-stu-id="38b88-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="38b88-166">Nie można pobrać usuniętych lokalizacji i wszystkie powiązane z tym identyfikatorem MPN nie będą już rozpoznawane ani nieaktywne dla Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="38b88-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="38b88-167">Zmień kraj konta partnera globalnego</span><span class="sxs-lookup"><span data-stu-id="38b88-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="38b88-168">Zaloguj się przy użyciu konta MPN w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="38b88-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="38b88-169">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP).</span><span class="sxs-lookup"><span data-stu-id="38b88-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="38b88-170">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="38b88-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="38b88-171">Na karcie **partner** przejdź do **lokalizacji biznesowej** i sprawdź listę lokalizacji, aby upewnić się, że lokalizacja, która ma się pojawić jako podmiot prawny, jest wyświetlana.</span><span class="sxs-lookup"><span data-stu-id="38b88-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="38b88-172">Aby dodać lokalizację, kliknij pozycję **Dodaj lokalizację**, a następnie w polu wylot wprowadź wymagane szczegóły, takie jak nazwa firmy, adres i kontakt podstawowy dla lokalizacji, która ma zostać dodana do firmy.</span><span class="sxs-lookup"><span data-stu-id="38b88-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="38b88-173">Wybierz pozycję **Zmień kraj** obok listy rozwijanej **kraj/region** i postępuj zgodnie z instrukcjami.</span><span class="sxs-lookup"><span data-stu-id="38b88-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Brak danych profilu biznesowego firmy":::

5. <span data-ttu-id="38b88-175">Kliknij pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="38b88-175">Click **Save**.</span></span>

6. <span data-ttu-id="38b88-176">Globalny kraj konta MPN zostanie zmieniony na nowy kraj prawny.</span><span class="sxs-lookup"><span data-stu-id="38b88-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="38b88-177">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="38b88-177">Next steps</span></span>

- <span data-ttu-id="38b88-178">Dowiedz się więcej na temat [procesu weryfikacji](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="38b88-178">Learn about the [verification process](verification-responses.md).</span></span>
