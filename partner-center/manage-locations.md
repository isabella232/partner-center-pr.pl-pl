---
title: Zarządzanie lokalizacjami na koncie partnerskim
ms.topic: how-to
ms.date: 02/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak używać identyfikatora MPN Location w programach zachęty, biznesie CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c5ac31b772c6757468c5ea9d463643731571b31f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624276"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="01815-103">Zarządzanie lokalizacjami kont MPN i Dodawanie nowej lokalizacji</span><span class="sxs-lookup"><span data-stu-id="01815-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="01815-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="01815-104">**Appropriate roles**</span></span>

- <span data-ttu-id="01815-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="01815-105">Global admin</span></span>
- <span data-ttu-id="01815-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="01815-106">Account admin</span></span>

<span data-ttu-id="01815-107">IDENTYFIKATOR MPN lokalizacji identyfikuje każdą konkretną lokalizację firmy.</span><span class="sxs-lookup"><span data-stu-id="01815-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="01815-108">IDENTYFIKATOR MPN Location służy do rejestrowania w programach zachęty, do firmowego dostawcy rozwiązań w chmurze (CSP) i innych transakcji roboczych.</span><span class="sxs-lookup"><span data-stu-id="01815-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="01815-109">Globalny identyfikator MPN jest używany dla działań nietransakcyjnych, takich jak żądania pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="01815-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="01815-110">Poniżej przedstawiono typowy scenariusz:</span><span class="sxs-lookup"><span data-stu-id="01815-110">The following is a typical scenario:</span></span>

<span data-ttu-id="01815-111">Firma Contoso ma swoje konto globalne partnera (PGA) w Wielkiej Brytanii.</span><span class="sxs-lookup"><span data-stu-id="01815-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="01815-112">Jest to zarejestrowana firma prawna, a jej globalny identyfikator MPN jest używany do zarządzania wszystkimi nietransakcyjnymi biznesowymi.</span><span class="sxs-lookup"><span data-stu-id="01815-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="01815-113">Firma Contoso ma także równorzędne konta firmowe lub działy w innej lokalizacji w Wielkiej Brytanii, Francji i w USA.</span><span class="sxs-lookup"><span data-stu-id="01815-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="01815-114">W strukturze konta MPN te PLAs są reprezentowane jako unikatowe lokalizacje MPN identyfikatory.</span><span class="sxs-lookup"><span data-stu-id="01815-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="01815-115">PLAs są używane dla transakcji transakcyjnych, takich jak CSP lub programy zachęt.</span><span class="sxs-lookup"><span data-stu-id="01815-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="01815-116">Wypłaty są powiązane z określonymi lokalizacjami.</span><span class="sxs-lookup"><span data-stu-id="01815-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="01815-117">Istnieje relacja 1-1 między dzierżawą dostawcy usług kryptograficznych i IDENTYFIKATORem lokalizacji MPN.</span><span class="sxs-lookup"><span data-stu-id="01815-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="01815-119">Wymagania wstępne w celu dodania nowego konta dla firmy dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="01815-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="01815-120">Aby dodać nowe konto biznesowe dostawcy usług kryptograficznych, Zacznij od upewnienia się, że spełniono wymagania wstępne.</span><span class="sxs-lookup"><span data-stu-id="01815-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="01815-121">W kraju, w którym ma być prowadzone biznesowe Oprogramowanie CSP, musi znajdować się identyfikator MPN.</span><span class="sxs-lookup"><span data-stu-id="01815-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="01815-122">Aby utworzyć nową lokalizację MPN, przeczytaj sekcję "Dodawanie lokalizacji MPN" poniżej.</span><span class="sxs-lookup"><span data-stu-id="01815-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="01815-123">Aby utworzyć nową dostawcę CSP pośredniego rejestracji odsprzedawcy, przeczytaj artykuł [współpraca z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="01815-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="01815-124">Pamiętaj, aby zalogować się przy użyciu **nowych** poświadczeń dla **nowego** konta dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="01815-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="01815-125">Nie używaj istniejących poświadczeń, ponieważ centrum partnerskie sprawdzi, czy masz już konto.</span><span class="sxs-lookup"><span data-stu-id="01815-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="01815-126">Zaakceptuj umowę partnera firmy Microsoft i aktywuj konto.</span><span class="sxs-lookup"><span data-stu-id="01815-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="01815-127">Jeśli chcesz zarejestrować się jako partner bezpośredniego rozliczania, zapoznaj się z [wymaganiami dotyczącymi bezpośrednich partnerów rozliczeniowych](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="01815-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="01815-128">Wyświetlanie lokalizacji MPN</span><span class="sxs-lookup"><span data-stu-id="01815-128">View your MPN locations</span></span>

1. <span data-ttu-id="01815-129">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego przy użyciu poświadczeń konta MPN.</span><span class="sxs-lookup"><span data-stu-id="01815-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="01815-130">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP)</span><span class="sxs-lookup"><span data-stu-id="01815-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="01815-131">Na ikonie **ustawień** wybierz kolejno pozycje **Ustawienia konta**, **profil organizacji** i informacje **prawne**.</span><span class="sxs-lookup"><span data-stu-id="01815-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="01815-132">Na karcie **partner** Sprawdź, czy nie jest wyświetlany komunikat o błędzie transparentu z prośbą o naprawienie zmigrowanych lokalizacji z PMC.</span><span class="sxs-lookup"><span data-stu-id="01815-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="01815-133">Jeśli istnieje, postępuj zgodnie z instrukcjami i napraw te lokalizacje.</span><span class="sxs-lookup"><span data-stu-id="01815-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="01815-134">Jeśli nie ma komunikatu o błędzie, w obszarze  **Ustawienia** wybierz pozycję  **Ustawienia konta**, **profil organizacji**, **identyfikatory**.</span><span class="sxs-lookup"><span data-stu-id="01815-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="01815-135">Znajdź identyfikator MPN z typem "Location", który pasuje do kraju tego konta CSP, i użyj go do przeszukania poniżej i kompletnego skojarzenia.</span><span class="sxs-lookup"><span data-stu-id="01815-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="01815-136">Jeśli nie możesz znaleźć lokalizacji MPN identyfikator, która jest zgodna z kontem dostawcy CSP, którego chcesz użyć, możesz dodać nową lokalizację, która utworzy nowy identyfikator MPN.</span><span class="sxs-lookup"><span data-stu-id="01815-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="01815-137">Zobacz **Dodaj lokalizację MPN** poniżej.</span><span class="sxs-lookup"><span data-stu-id="01815-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="01815-138">Dodaj lokalizację MPN</span><span class="sxs-lookup"><span data-stu-id="01815-138">Add an MPN location</span></span>

1. <span data-ttu-id="01815-139">Zaloguj się przy użyciu konta MPN w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="01815-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="01815-140">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP).</span><span class="sxs-lookup"><span data-stu-id="01815-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="01815-141">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="01815-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="01815-142">Na **ikonie ustawień** wybierz **Ustawienia konta** , a następnie wybierz pozycję **profil organizacji**.</span><span class="sxs-lookup"><span data-stu-id="01815-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="01815-143">Wybierz pozycję **Legal** , a następnie na karcie **partner** wybierz pozycję **lokalizacje biznesowe,** a następnie kliknij pozycję **Dodaj lokalizację.**</span><span class="sxs-lookup"><span data-stu-id="01815-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="01815-144">Podaj wymagane szczegóły, takie jak nazwa firmy, adres i kontakt, dla lokalizacji, która ma zostać dodana do firmy.</span><span class="sxs-lookup"><span data-stu-id="01815-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="01815-145">Kliknij pozycję **Dodaj lokalizację**.</span><span class="sxs-lookup"><span data-stu-id="01815-145">Click **Add location**.</span></span> <span data-ttu-id="01815-146">Spowoduje to utworzenie nowego identyfikatora MPN dla nowej lokalizacji, z której można korzystać w przypadku transakcji i zachęt dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="01815-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Dodaj nową firmę prawną":::

> [!NOTE]
> <span data-ttu-id="01815-148">Po dodaniu lokalizacji w centrum partnerskim nie można jej usunąć.</span><span class="sxs-lookup"><span data-stu-id="01815-148">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="01815-149">Aby zalogować się, zobaczysz **MPN** w menu po lewej stronie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="01815-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="01815-150">Zmień kraj konta partnera globalnego</span><span class="sxs-lookup"><span data-stu-id="01815-150">Change country of Partner global account</span></span> 

1. <span data-ttu-id="01815-151">Zaloguj się przy użyciu konta MPN w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="01815-151">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="01815-152">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP).</span><span class="sxs-lookup"><span data-stu-id="01815-152">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="01815-153">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="01815-153">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="01815-154">Na karcie **partner** przejdź do **lokalizacji biznesowej** i sprawdź listę lokalizacji, aby upewnić się, że lokalizacja, która ma się pojawić jako podmiot prawny, jest wyświetlana.</span><span class="sxs-lookup"><span data-stu-id="01815-154">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="01815-155">Aby dodać lokalizację, kliknij pozycję **Dodaj lokalizację**, a następnie w polu wylot wprowadź wymagane szczegóły, takie jak nazwa firmy, adres i kontakt podstawowy dla lokalizacji, która ma zostać dodana do firmy.</span><span class="sxs-lookup"><span data-stu-id="01815-155">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="01815-156">Wybierz pozycję **Zmień kraj** obok listy rozwijanej **kraj/region** i postępuj zgodnie z instrukcjami.</span><span class="sxs-lookup"><span data-stu-id="01815-156">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Brak danych profilu biznesowego firmy":::

5. <span data-ttu-id="01815-158">Kliknij pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="01815-158">Click **Save**.</span></span>

6. <span data-ttu-id="01815-159">Globalny kraj konta MPN zostanie zmieniony na nowy kraj prawny.</span><span class="sxs-lookup"><span data-stu-id="01815-159">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="01815-160">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="01815-160">Next steps</span></span>

- <span data-ttu-id="01815-161">Dowiedz się więcej na temat [procesu weryfikacji](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="01815-161">Learn about the [verification process](verification-responses.md).</span></span>
