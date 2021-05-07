---
title: Zarządzanie lokalizacjami na koncie partnera
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak identyfikator MPN lokalizacji jest używany w programach zachęt, firmach CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702896"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="30c67-103">Zarządzanie lokalizacjami konta MPN i dodawanie (usuwanie) lokalizacji</span><span class="sxs-lookup"><span data-stu-id="30c67-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="30c67-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="30c67-104">**Appropriate roles**</span></span>

- <span data-ttu-id="30c67-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="30c67-105">Global admin</span></span>
- <span data-ttu-id="30c67-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="30c67-106">Account admin</span></span>

<span data-ttu-id="30c67-107">Identyfikator MPN lokalizacji identyfikuje każdą określoną lokalizację firmy.</span><span class="sxs-lookup"><span data-stu-id="30c67-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="30c67-108">Identyfikator MPN lokalizacji umożliwia rejestrację w programach zachęt, transakcje Dostawca rozwiązań w chmurze (CSP) i inne transakcje biznesowe.</span><span class="sxs-lookup"><span data-stu-id="30c67-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="30c67-109">Globalny identyfikator MPN jest używany w przypadku działań nie transakcyjnych, takich jak żądania pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="30c67-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="30c67-110">Typowy jest następujący scenariusz:</span><span class="sxs-lookup"><span data-stu-id="30c67-110">The following scenario is typical:</span></span>

<span data-ttu-id="30c67-111">Firma Contoso ma swoje globalne konto partnera (PGA) w Zjednoczonym Królestwie.</span><span class="sxs-lookup"><span data-stu-id="30c67-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="30c67-112">PgA to zarejestrowana firma prawna, a jej globalny identyfikator MPN jest używany do zarządzania całą działalnością nie transakcyjną.</span><span class="sxs-lookup"><span data-stu-id="30c67-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="30c67-113">Firma Contoso ma również konta lokalizacji partnera (PLA) równoważne przedstawicielsjom lub oddziałom w innej lokalizacji w Zjednoczonym Królestwie, Francji i Stanach Zjednoczonych.</span><span class="sxs-lookup"><span data-stu-id="30c67-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="30c67-114">W strukturze konta MPN te plasy są reprezentowane jako unikatowe identyfikatory MPN lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="30c67-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="30c67-115">Plas są używane dla transakcji biznesowych, takich jak CSP lub programy zachęt.</span><span class="sxs-lookup"><span data-stu-id="30c67-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="30c67-116">Wypłaty są powiązane z określonymi lokalizacjami.</span><span class="sxs-lookup"><span data-stu-id="30c67-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="30c67-117">Istnieje relacja 1–1 między dzierżawą CSP i identyfikatorem lokalizacji MPN.</span><span class="sxs-lookup"><span data-stu-id="30c67-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="30c67-119">Wymagania wstępne dotyczące dodawania nowego konta dla firmy CSP</span><span class="sxs-lookup"><span data-stu-id="30c67-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="30c67-120">Aby dodać nowe konto biznesowe programu CSP, rozpocznij od upewniania się, że spełniliśmy wymagania wstępne.</span><span class="sxs-lookup"><span data-stu-id="30c67-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="30c67-121">Musisz mieć identyfikator MPN lokalizacji w kraju, w którym chcesz wykonać działalność w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="30c67-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="30c67-122">Aby utworzyć nową lokalizację MPN, przeczytaj "Dodaj lokalizację MPN" poniżej.</span><span class="sxs-lookup"><span data-stu-id="30c67-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="30c67-123">Aby utworzyć nową rejestrację CSP Indirect Reseller, przeczytaj [Temat Praca z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="30c67-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="30c67-124">Pamiętaj, aby zalogować się **przy użyciu nowych** poświadczeń dla nowego **konta** CSP.</span><span class="sxs-lookup"><span data-stu-id="30c67-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="30c67-125">Nie używaj istniejących poświadczeń, ponieważ Partner Center rozpozna, że masz już konto.</span><span class="sxs-lookup"><span data-stu-id="30c67-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="30c67-126">Zaakceptuj Microsoft Partner Agreement i aktywuj konto.</span><span class="sxs-lookup"><span data-stu-id="30c67-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="30c67-127">Jeśli chcesz zarejestrować się jako partner z rozliczeniami bezpośrednimi, przeczytaj [wymagania dotyczące partnerów rozliczanych bezpośrednio](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="30c67-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="30c67-128">Wyświetlanie i aktualizowanie lokalizacji MPN</span><span class="sxs-lookup"><span data-stu-id="30c67-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="30c67-129">Zaloguj się do Partner Center [nawigacyjnego przy](https://partner.microsoft.com/dashboard/home) użyciu poświadczeń konta MPN.</span><span class="sxs-lookup"><span data-stu-id="30c67-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="30c67-130">(Twoje poświadczenia MPN mogą różnić się od poświadczeń CSP)</span><span class="sxs-lookup"><span data-stu-id="30c67-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="30c67-131">Z **ikony Ustawienia** wybierz pozycję **Ustawienia konta,** **Profil organizacji,** **Prawne.**</span><span class="sxs-lookup"><span data-stu-id="30c67-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="30c67-132">Na karcie **Partner** sprawdź, czy nie ma komunikatu o błędzie baneru z prośbą o naprawienie lokalizacji zmigrowanych z centrum PMC.</span><span class="sxs-lookup"><span data-stu-id="30c67-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="30c67-133">Jeśli lokalizacje nie zostały poprawnie skonfigurowane w centrum PMC i nie zostały jeszcze przejść na komputer, należy zaktualizować te lokalizacje.</span><span class="sxs-lookup"><span data-stu-id="30c67-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap pokazuje, jak zaktualizować lokalizację.":::
 
4.  <span data-ttu-id="30c67-135">Na **ekranie Review PMC locations (Przejrzyj lokalizacje PMC)** wybierz pozycję **Update (Aktualizuj).**</span><span class="sxs-lookup"><span data-stu-id="30c67-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="30c67-136">Zaktualizuj następujące pola:</span><span class="sxs-lookup"><span data-stu-id="30c67-136">Update the following fields:</span></span>

- <span data-ttu-id="30c67-137">**Pole Nazwa:** upewnij się, że nazwa lokalizacji firmy jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="30c67-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="30c67-138">Jeśli zostanie wyświetlony zduplikowany błąd, spróbuj zmienić adres, na przykład Contoso na Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="30c67-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="30c67-139">**Pole Jednostka prawna:** upewnij się, że została wybrana jednostka prawna, z którym jest powiązana lokalizacja</span><span class="sxs-lookup"><span data-stu-id="30c67-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="30c67-140">**Wiersz adresu 1 & 2 pola:** upewnij się, że adres jest poprawny</span><span class="sxs-lookup"><span data-stu-id="30c67-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="30c67-141">**Pola & Stan/Województwo:** upewnij się, że kombinacja miasta i województwa jest poprawna.</span><span class="sxs-lookup"><span data-stu-id="30c67-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="30c67-142">Istnieją kraje, w których będzie stosowane menu rozwijane służące do wybierania województwa, a w innych krajach należy ręcznie wstawić to pole.</span><span class="sxs-lookup"><span data-stu-id="30c67-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="30c67-143">**Zip/Postal code field (Kod** pocztowy): upewnij się, że pole Kod pocztowy jest zgodne ze wskazanym polem Country (Kraj), Region (Region), City (Miasto) lub Address (Adres).</span><span class="sxs-lookup"><span data-stu-id="30c67-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="30c67-144">**Pola podstawowych** informacji kontaktowych: upewnij się, że pola imienia i nazwiska zostały wypełnione, a wskazany adres e-mail jest służbowym adresem e-mail, a nie osobistym (na przykład @outlook.com , @live.com itp.)</span><span class="sxs-lookup"><span data-stu-id="30c67-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="30c67-145">**Pole Numeru telefonu:** upewnij się, że numer telefonu NIE zawiera znaków specjalnych, spacji ani kodu kraju.</span><span class="sxs-lookup"><span data-stu-id="30c67-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="30c67-146">Wartość wprowadzona w polu Numer telefonu zawsze będzie zawierać maksymalnie 10 znaków.</span><span class="sxs-lookup"><span data-stu-id="30c67-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="30c67-147">Jeśli nie ma komunikatu o błędzie, w menu Ustawienia wybierz pozycję **Ustawienia konta,** **Profil organizacji,** **Identyfikatory**. </span><span class="sxs-lookup"><span data-stu-id="30c67-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="30c67-148">Znajdź identyfikator MPN z typem "Location" (Lokalizacja), który pasuje do kraju tego konta CSP, i użyj go do ukończenia skojarzenia.</span><span class="sxs-lookup"><span data-stu-id="30c67-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="30c67-149">Jeśli nie możesz znaleźć identyfikatora MPN lokalizacji, który pasuje do konta CSP, którego chcesz użyć, możesz dodać nową lokalizację, co spowoduje utworzenie nowego identyfikatora MPN.</span><span class="sxs-lookup"><span data-stu-id="30c67-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="30c67-150">Zobacz **Dodawanie lokalizacji MPN** poniżej.</span><span class="sxs-lookup"><span data-stu-id="30c67-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="30c67-151">Dodawanie lokalizacji MPN</span><span class="sxs-lookup"><span data-stu-id="30c67-151">Add an MPN location</span></span>

1. <span data-ttu-id="30c67-152">Zaloguj się przy użyciu konta MPN w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30c67-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="30c67-153">(Poświadczenia MPN mogą różnić się od poświadczeń CSP).</span><span class="sxs-lookup"><span data-stu-id="30c67-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="30c67-154">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="30c67-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="30c67-155">Z **ikony Ustawienia wybierz** pozycję **Ustawienia konta,** a następnie wybierz **pozycję Profil organizacji.**</span><span class="sxs-lookup"><span data-stu-id="30c67-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="30c67-156">Wybierz **pozycję Prawne,** a następnie na karcie **Partner** wybierz pozycję **Lokalizacje biznesowe i** kliknij pozycję Dodaj **lokalizację.**</span><span class="sxs-lookup"><span data-stu-id="30c67-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="30c67-157">Podaj wymagane szczegóły, w tym nazwę firmy, adres i kontakt dla lokalizacji, którą chcesz dodać do firmy.</span><span class="sxs-lookup"><span data-stu-id="30c67-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="30c67-158">Kliknij **pozycję Dodaj lokalizację**.</span><span class="sxs-lookup"><span data-stu-id="30c67-158">Click **Add location**.</span></span> <span data-ttu-id="30c67-159">Spowoduje to utworzenie nowego identyfikatora MPN dla nowej lokalizacji, której można użyć na użytek transakcji i zachęt CSP.</span><span class="sxs-lookup"><span data-stu-id="30c67-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Dodawanie nowej firmy prawnej":::

> [!NOTE]
> <span data-ttu-id="30c67-161">Po dodaniu lokalizacji w Partner Center nie można jej usunąć.</span><span class="sxs-lookup"><span data-stu-id="30c67-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="30c67-162">Jeśli do logowania używasz poprawnego identyfikatora **MPN,** w menu po lewej stronie Partner Center po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="30c67-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="30c67-163">Dodawanie identyfikatora numeru rejestracji</span><span class="sxs-lookup"><span data-stu-id="30c67-163">Add the registration number ID</span></span>

<span data-ttu-id="30c67-164">Jeśli jesteś dostawcą pośrednim, partnerem rozliczania bezpośredniego lub odsprzedawcą pośrednim i współpracujesz z nowymi lub istniejącymi klientami w następujących krajach, musisz podać numery identyfikatorów rejestracji dla swojej firmy.</span><span class="sxs-lookup"><span data-stu-id="30c67-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="30c67-165">Jeśli kraj, w którym prowadzenia działalności biznesowej, nie jest wymieniony poniżej, identyfikator rejestracji jest opcjonalny.</span><span class="sxs-lookup"><span data-stu-id="30c67-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="30c67-166">Armenia</span><span class="sxs-lookup"><span data-stu-id="30c67-166">Armenia</span></span> 
- <span data-ttu-id="30c67-167">Azerbejdżan</span><span class="sxs-lookup"><span data-stu-id="30c67-167">Azerbaijan</span></span> 
- <span data-ttu-id="30c67-168">Białoruś</span><span class="sxs-lookup"><span data-stu-id="30c67-168">Belarus</span></span> 
- <span data-ttu-id="30c67-169">Brazylia</span><span class="sxs-lookup"><span data-stu-id="30c67-169">Brazil</span></span> 
- <span data-ttu-id="30c67-170">Węgry</span><span class="sxs-lookup"><span data-stu-id="30c67-170">Hungary</span></span> 
- <span data-ttu-id="30c67-171">Indie</span><span class="sxs-lookup"><span data-stu-id="30c67-171">India</span></span> 
- <span data-ttu-id="30c67-172">Irak</span><span class="sxs-lookup"><span data-stu-id="30c67-172">Iraq</span></span> 
- <span data-ttu-id="30c67-173">Kazachstan</span><span class="sxs-lookup"><span data-stu-id="30c67-173">Kazakhstan</span></span> 
- <span data-ttu-id="30c67-174">Kirgistan</span><span class="sxs-lookup"><span data-stu-id="30c67-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="30c67-175">Mołdawia</span><span class="sxs-lookup"><span data-stu-id="30c67-175">Moldova</span></span> 
- <span data-ttu-id="30c67-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="30c67-176">Myanmar</span></span> 
- <span data-ttu-id="30c67-177">Polska</span><span class="sxs-lookup"><span data-stu-id="30c67-177">Poland</span></span> 
- <span data-ttu-id="30c67-178">Rosja</span><span class="sxs-lookup"><span data-stu-id="30c67-178">Russia</span></span> 
- <span data-ttu-id="30c67-179">Arabia Saudyjska</span><span class="sxs-lookup"><span data-stu-id="30c67-179">Saudi Arabia</span></span> 
- <span data-ttu-id="30c67-180">Republika Południowej Afryki</span><span class="sxs-lookup"><span data-stu-id="30c67-180">South Africa</span></span> 
- <span data-ttu-id="30c67-181">Sudan Południowy</span><span class="sxs-lookup"><span data-stu-id="30c67-181">South Sudan</span></span>  
- <span data-ttu-id="30c67-182">Tadżykistan</span><span class="sxs-lookup"><span data-stu-id="30c67-182">Tajikistan</span></span> 
- <span data-ttu-id="30c67-183">Tajlandia</span><span class="sxs-lookup"><span data-stu-id="30c67-183">Thailand</span></span>
- <span data-ttu-id="30c67-184">Turcja</span><span class="sxs-lookup"><span data-stu-id="30c67-184">Turkey</span></span> 
- <span data-ttu-id="30c67-185">Ukraina</span><span class="sxs-lookup"><span data-stu-id="30c67-185">Ukraine</span></span> 
- <span data-ttu-id="30c67-186">Zjednoczone Emiraty Arabskie</span><span class="sxs-lookup"><span data-stu-id="30c67-186">United Arab Emirates</span></span> 
- <span data-ttu-id="30c67-187">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="30c67-187">Uzbekistan</span></span> 
- <span data-ttu-id="30c67-188">Wenezuela</span><span class="sxs-lookup"><span data-stu-id="30c67-188">Venezuela</span></span>
- <span data-ttu-id="30c67-189">Wietnam</span><span class="sxs-lookup"><span data-stu-id="30c67-189">Vietnam</span></span> 


<span data-ttu-id="30c67-190">Aby uzyskać więcej informacji, przeczytaj [informacje o numerze identyfikatora rejestracji](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="30c67-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="30c67-191">Usuwanie lokalizacji</span><span class="sxs-lookup"><span data-stu-id="30c67-191">Delete a location</span></span>

<span data-ttu-id="30c67-192">Aby usunąć lokalizację z konta, należy skontaktować się z pomocą [techniczną partnera](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="30c67-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="30c67-193">Upewnij się, że rozumiesz wpływ tej akcji.</span><span class="sxs-lookup"><span data-stu-id="30c67-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="30c67-194">Nie można pobrać usuniętych lokalizacji i wszystkie elementy powiązane z tym konkretnym identyfikatorem MPN nie będą już rozpoznawane ani aktywne dla Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="30c67-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="30c67-195">Zmiana kraju konta globalnego partnera</span><span class="sxs-lookup"><span data-stu-id="30c67-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="30c67-196">Zaloguj się przy użyciu konta MPN w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="30c67-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="30c67-197">(Poświadczenia MPN mogą różnić się od poświadczeń CSP).</span><span class="sxs-lookup"><span data-stu-id="30c67-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="30c67-198">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="30c67-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="30c67-199">Na karcie **Partner** przejdź  do pozycji Lokalizacje biznesowe i sprawdź listę lokalizacji, aby upewnić się, że na liście znajduje się lokalizacja, której chcesz użyć jako jednostki prawnej.</span><span class="sxs-lookup"><span data-stu-id="30c67-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="30c67-200">Aby dodać lokalizację, kliknij pozycję Dodaj lokalizację i w wysuwanych menu podaj wymagane szczegóły, takie jak nazwa firmy, adres i podstawowy kontakt dla lokalizacji, którą chcesz dodać do firmy. </span><span class="sxs-lookup"><span data-stu-id="30c67-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="30c67-201">Wybierz **pozycję Zmień kraj** obok listy rozwijanej **Kraj/region** i wykonaj kroki.</span><span class="sxs-lookup"><span data-stu-id="30c67-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Wysuwają się dane legalnych profilów biznesowych":::

5. <span data-ttu-id="30c67-203">Kliknij pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="30c67-203">Click **Save**.</span></span>

6. <span data-ttu-id="30c67-204">Globalny kraj konta MPN zostanie zmieniony na nowy kraj prawny.</span><span class="sxs-lookup"><span data-stu-id="30c67-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="30c67-205">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="30c67-205">Next steps</span></span>

- <span data-ttu-id="30c67-206">Dowiedz się więcej o [procesie weryfikacji.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="30c67-206">Learn about the [verification process](verification-responses.md).</span></span>
