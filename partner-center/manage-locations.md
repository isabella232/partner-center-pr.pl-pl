---
title: Zarządzanie lokalizacjami na koncie partnerskim
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak używać identyfikatora MPN Location w programach zachęty, biznesie CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/15/2020
ms.locfileid: "92530429"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="987f3-103">Zarządzanie lokalizacjami kont MPN i Dodawanie nowej lokalizacji</span><span class="sxs-lookup"><span data-stu-id="987f3-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="987f3-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="987f3-104">**Applies to**</span></span>

- <span data-ttu-id="987f3-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="987f3-105">Partner Center</span></span>

<span data-ttu-id="987f3-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="987f3-106">**Appropriate roles**</span></span>

- <span data-ttu-id="987f3-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="987f3-107">Global admin</span></span>
- <span data-ttu-id="987f3-108">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="987f3-108">Account admin</span></span>

<span data-ttu-id="987f3-109">IDENTYFIKATOR MPN lokalizacji identyfikuje każdą konkretną lokalizację firmy.</span><span class="sxs-lookup"><span data-stu-id="987f3-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="987f3-110">IDENTYFIKATOR MPN Location służy do rejestrowania w programach zachęty, do firmowego dostawcy rozwiązań w chmurze (CSP) i innych transakcji roboczych.</span><span class="sxs-lookup"><span data-stu-id="987f3-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="987f3-111">Globalny identyfikator MPN jest używany dla działań nietransakcyjnych, takich jak żądania pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="987f3-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="987f3-112">Poniżej przedstawiono typowy scenariusz:</span><span class="sxs-lookup"><span data-stu-id="987f3-112">The following is a typical scenario:</span></span>

<span data-ttu-id="987f3-113">Firma Contoso ma swoje konto globalne partnera (PGA) w Wielkiej Brytanii.</span><span class="sxs-lookup"><span data-stu-id="987f3-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="987f3-114">Jest to zarejestrowana firma prawna, a jej globalny identyfikator MPN jest używany do zarządzania wszystkimi nietransakcyjnymi biznesowymi.</span><span class="sxs-lookup"><span data-stu-id="987f3-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="987f3-115">Firma Contoso ma także równorzędne konta firmowe lub działy w innej lokalizacji w Wielkiej Brytanii, Francji i w USA.</span><span class="sxs-lookup"><span data-stu-id="987f3-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="987f3-116">W strukturze konta MPN te PLAs są reprezentowane jako unikatowe lokalizacje MPN identyfikatory.</span><span class="sxs-lookup"><span data-stu-id="987f3-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="987f3-117">PLAs są używane dla transakcji transakcyjnych, takich jak CSP lub programy zachęt.</span><span class="sxs-lookup"><span data-stu-id="987f3-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="987f3-118">Wypłaty są powiązane z określonymi lokalizacjami.</span><span class="sxs-lookup"><span data-stu-id="987f3-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="987f3-119">Istnieje relacja 1-1 między dzierżawą dostawcy usług kryptograficznych i IDENTYFIKATORem lokalizacji MPN.</span><span class="sxs-lookup"><span data-stu-id="987f3-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="987f3-121">Wymagania wstępne w celu dodania nowej lokalizacji dla firmy dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="987f3-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="987f3-122">Aby dodać nową lokalizację biznesową programu CSP, istnieje kilka wymagań wstępnych:</span><span class="sxs-lookup"><span data-stu-id="987f3-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="987f3-123">W kraju, w którym chcesz przeprowadzić działalność biznesową, musisz mieć identyfikator MPN lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="987f3-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="987f3-124">Potrzebna jest nowa dzierżawa usługi Azure AD w [regionie firmy](regional-authorization-overview.md) , która nie została już zarejestrowana w dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="987f3-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="987f3-125">Utwórz to po zarejestrowaniu w dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="987f3-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="987f3-126">Użyj nowej dzierżawy usługi AAD, aby zarejestrować się w programie CSP w regionie.</span><span class="sxs-lookup"><span data-stu-id="987f3-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="987f3-127">Dostarczenie szczegółowych informacji o firmie, takich jak imię i nazwisko, adres, podstawowe informacje kontaktowe firmy.</span><span class="sxs-lookup"><span data-stu-id="987f3-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="987f3-128">To konto zostanie poddane weryfikacji, dlatego należy dodać prawidłowe informacje.</span><span class="sxs-lookup"><span data-stu-id="987f3-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="987f3-129">Pamiętaj, aby zalogować się przy użyciu **nowych** poświadczeń dla **nowej** dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="987f3-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="987f3-130">Nie używaj istniejących poświadczeń, ponieważ centrum partnerskie sprawdzi, czy masz już konto.</span><span class="sxs-lookup"><span data-stu-id="987f3-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="987f3-131">Zaakceptuj umowę partnera firmy Microsoft i aktywuj konto.</span><span class="sxs-lookup"><span data-stu-id="987f3-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="987f3-132">Dodaj lokalizację MPN</span><span class="sxs-lookup"><span data-stu-id="987f3-132">Add an MPN location</span></span>

1. <span data-ttu-id="987f3-133">Zaloguj się przy użyciu konta MPN w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="987f3-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="987f3-134">Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta.</span><span class="sxs-lookup"><span data-stu-id="987f3-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="987f3-135">Na **ikonie ustawienia** wybierz pozycję **Ustawienia partnera** .</span><span class="sxs-lookup"><span data-stu-id="987f3-135">From the **Setting icon** , select the **Partner settings** .</span></span>

2. <span data-ttu-id="987f3-136">Wybierz **lokalizacje.**</span><span class="sxs-lookup"><span data-stu-id="987f3-136">Select **Locations.**</span></span>

3. <span data-ttu-id="987f3-137">Wybierz pozycję **Dodaj lokalizację** i Wstaw szczegóły adresu lokalizacji, która ma zostać dodana do firmy, a także główną osobę kontaktową dla tej lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="987f3-137">Select **Add a location** , and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="987f3-138">Po dodaniu lokalizacji w centrum partnerskim nie można jej usunąć.</span><span class="sxs-lookup"><span data-stu-id="987f3-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="987f3-139">Aby zalogować się, zobaczysz **MPN** w menu po lewej stronie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="987f3-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="987f3-140">Zmień lokalizację globalnego konta partnera</span><span class="sxs-lookup"><span data-stu-id="987f3-140">Change Global partner account location</span></span>

1. <span data-ttu-id="987f3-141">Na stronie **[lokalizacje](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** Sprawdź listę lokalizacji, aby upewnić się, że podano lokalizację, w której znajduje się Twoja firma.</span><span class="sxs-lookup"><span data-stu-id="987f3-141">On the **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="987f3-142">Jeśli nie, Dodaj ją.</span><span class="sxs-lookup"><span data-stu-id="987f3-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Zrzut ekranu przedstawiający stronę lokalizacje konta Centrum partnerskiego z listą wszystkich bieżących lokalizacji.":::

2. <span data-ttu-id="987f3-144">Wybierz pozycję **Profil partnera** , a następnie wybierz opcję **Aktualizuj profil prawny firmy**</span><span class="sxs-lookup"><span data-stu-id="987f3-144">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Zrzut ekranu przedstawiający informacje o profilu partnera kont Centrum partnerskiego z wybraną opcją aktualizacji.":::

3. <span data-ttu-id="987f3-146">Wybierz region i jednostkę prawną i **Prześlij** ją.</span><span class="sxs-lookup"><span data-stu-id="987f3-146">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Zrzut ekranu, aby zaktualizować profil biznesowy dla partnera zawiera listę rozwijaną, aby zaktualizować kraj lub region oraz jednostkę prawną.":::

## <a name="next-steps"></a><span data-ttu-id="987f3-148">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="987f3-148">Next steps</span></span>

- <span data-ttu-id="987f3-149">Dowiedz się więcej na temat [procesu weryfikacji](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="987f3-149">Learn about the [verification process](verification-responses.md).</span></span>
