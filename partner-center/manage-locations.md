---
title: Zarządzanie lokalizacjami na koncie partnerskim
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak używać identyfikatora MPN Location w programach zachęty, biznesie CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925037"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="27abd-103">Zarządzanie lokalizacjami kont MPN i Dodawanie nowej lokalizacji</span><span class="sxs-lookup"><span data-stu-id="27abd-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="27abd-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="27abd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="27abd-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="27abd-105">Global admin</span></span>
- <span data-ttu-id="27abd-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="27abd-106">Account admin</span></span>

<span data-ttu-id="27abd-107">IDENTYFIKATOR MPN lokalizacji identyfikuje każdą konkretną lokalizację firmy.</span><span class="sxs-lookup"><span data-stu-id="27abd-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="27abd-108">IDENTYFIKATOR MPN Location służy do rejestrowania w programach zachęty, do firmowego dostawcy rozwiązań w chmurze (CSP) i innych transakcji roboczych.</span><span class="sxs-lookup"><span data-stu-id="27abd-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="27abd-109">Globalny identyfikator MPN jest używany dla działań nietransakcyjnych, takich jak żądania pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="27abd-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="27abd-110">Poniżej przedstawiono typowy scenariusz:</span><span class="sxs-lookup"><span data-stu-id="27abd-110">The following is a typical scenario:</span></span>

<span data-ttu-id="27abd-111">Firma Contoso ma swoje konto globalne partnera (PGA) w Wielkiej Brytanii.</span><span class="sxs-lookup"><span data-stu-id="27abd-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="27abd-112">Jest to zarejestrowana firma prawna, a jej globalny identyfikator MPN jest używany do zarządzania wszystkimi nietransakcyjnymi biznesowymi.</span><span class="sxs-lookup"><span data-stu-id="27abd-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="27abd-113">Firma Contoso ma także równorzędne konta firmowe lub działy w innej lokalizacji w Wielkiej Brytanii, Francji i w USA.</span><span class="sxs-lookup"><span data-stu-id="27abd-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="27abd-114">W strukturze konta MPN te PLAs są reprezentowane jako unikatowe lokalizacje MPN identyfikatory.</span><span class="sxs-lookup"><span data-stu-id="27abd-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="27abd-115">PLAs są używane dla transakcji transakcyjnych, takich jak CSP lub programy zachęt.</span><span class="sxs-lookup"><span data-stu-id="27abd-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="27abd-116">Wypłaty są powiązane z określonymi lokalizacjami.</span><span class="sxs-lookup"><span data-stu-id="27abd-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="27abd-117">Istnieje relacja 1-1 między dzierżawą dostawcy usług kryptograficznych i IDENTYFIKATORem lokalizacji MPN.</span><span class="sxs-lookup"><span data-stu-id="27abd-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="27abd-119">Wymagania wstępne w celu dodania nowego konta dla firmy dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="27abd-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="27abd-120">Aby dodać nowe konto biznesowe dostawcy usług kryptograficznych, Zacznij od upewnienia się, że spełniono wymagania wstępne.</span><span class="sxs-lookup"><span data-stu-id="27abd-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="27abd-121">W kraju, w którym ma być prowadzone biznesowe Oprogramowanie CSP, musi znajdować się identyfikator MPN.</span><span class="sxs-lookup"><span data-stu-id="27abd-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="27abd-122">Aby utworzyć nową lokalizację MPN, przeczytaj sekcję "Dodawanie lokalizacji MPN" poniżej.</span><span class="sxs-lookup"><span data-stu-id="27abd-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="27abd-123">Aby utworzyć nową dostawcę CSP pośredniego rejestracji odsprzedawcy, przeczytaj artykuł [współpraca z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="27abd-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="27abd-124">Pamiętaj, aby zalogować się przy użyciu **nowych** poświadczeń dla **nowego** konta dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="27abd-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="27abd-125">Nie używaj istniejących poświadczeń, ponieważ centrum partnerskie sprawdzi, czy masz już konto.</span><span class="sxs-lookup"><span data-stu-id="27abd-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="27abd-126">Zaakceptuj umowę partnera firmy Microsoft i aktywuj konto.</span><span class="sxs-lookup"><span data-stu-id="27abd-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="27abd-127">Dodaj lokalizację MPN</span><span class="sxs-lookup"><span data-stu-id="27abd-127">Add an MPN location</span></span>

1. <span data-ttu-id="27abd-128">Zaloguj się przy użyciu konta MPN w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="27abd-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="27abd-129">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP).</span><span class="sxs-lookup"><span data-stu-id="27abd-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="27abd-130">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="27abd-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="27abd-131">Na **ikonie ustawień** wybierz **Ustawienia konta** , a następnie wybierz pozycję **profil organizacji**.</span><span class="sxs-lookup"><span data-stu-id="27abd-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="27abd-132">Wybierz pozycję **Legal** , a następnie na karcie **partner** wybierz pozycję **lokalizacje biznesowe,** a następnie kliknij pozycję **Dodaj lokalizację.**</span><span class="sxs-lookup"><span data-stu-id="27abd-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="27abd-133">Podaj wymagane szczegóły, takie jak nazwa firmy, adres i kontakt, dla lokalizacji, która ma zostać dodana do firmy.</span><span class="sxs-lookup"><span data-stu-id="27abd-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="27abd-134">Kliknij pozycję **Dodaj lokalizację**.</span><span class="sxs-lookup"><span data-stu-id="27abd-134">Click **Add location**.</span></span> <span data-ttu-id="27abd-135">Spowoduje to utworzenie nowego identyfikatora MPN dla nowej lokalizacji, z której można korzystać w przypadku transakcji i zachęt dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="27abd-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Dodaj nową firmę prawną":::

> [!NOTE]
> <span data-ttu-id="27abd-137">Po dodaniu lokalizacji w centrum partnerskim nie można jej usunąć.</span><span class="sxs-lookup"><span data-stu-id="27abd-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="27abd-138">Aby zalogować się, zobaczysz **MPN** w menu po lewej stronie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="27abd-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="27abd-139">Zmień kraj konta partnera globalnego</span><span class="sxs-lookup"><span data-stu-id="27abd-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="27abd-140">Zaloguj się przy użyciu konta MPN w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="27abd-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="27abd-141">(Poświadczenia MPN mogą się różnić od poświadczeń programu CSP).</span><span class="sxs-lookup"><span data-stu-id="27abd-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="27abd-142">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="27abd-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="27abd-143">Na karcie **partner** przejdź do **lokalizacji biznesowej** i sprawdź listę lokalizacji, aby upewnić się, że lokalizacja, która ma się pojawić jako podmiot prawny, jest wyświetlana.</span><span class="sxs-lookup"><span data-stu-id="27abd-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="27abd-144">Aby dodać lokalizację, kliknij pozycję **Dodaj lokalizację**, a następnie w polu wylot wprowadź wymagane szczegóły, takie jak nazwa firmy, adres i kontakt podstawowy dla lokalizacji, która ma zostać dodana do firmy.</span><span class="sxs-lookup"><span data-stu-id="27abd-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="27abd-145">Wybierz pozycję **Zmień kraj** obok listy rozwijanej **kraj/region** i postępuj zgodnie z instrukcjami.</span><span class="sxs-lookup"><span data-stu-id="27abd-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Brak danych profilu biznesowego firmy":::

5. <span data-ttu-id="27abd-147">Kliknij pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="27abd-147">Click **Save**.</span></span>

6. <span data-ttu-id="27abd-148">Globalny kraj konta MPN zostanie zmieniony na nowy kraj prawny.</span><span class="sxs-lookup"><span data-stu-id="27abd-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="27abd-149">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="27abd-149">Next steps</span></span>

- <span data-ttu-id="27abd-150">Dowiedz się więcej na temat [procesu weryfikacji](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="27abd-150">Learn about the [verification process](verification-responses.md).</span></span>
