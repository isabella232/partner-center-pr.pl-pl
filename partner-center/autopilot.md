---
title: Dostosowywanie wbudowanego środowiska urządzenia
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Przed dostarczeniem nowego urządzenia klienta można użyć profilów autopilotażu systemu Windows do dostosowania lub wstępnego skonfigurowania gotowego do użycia środowiska (OOBE) urządzenia.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 0ae61db0ca040afe67faa3a0883ea033b8f67562
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529838"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="4d2d2-103">Używanie profilów rozwiązania Windows Autopilot na nowych urządzeniach w celu dostosowania środowiska gotowego do użycia dla klienta</span><span class="sxs-lookup"><span data-stu-id="4d2d2-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="4d2d2-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="4d2d2-104">**Applies to**</span></span>

- <span data-ttu-id="4d2d2-105">Partnerzy bezpośrednich rachunków dostawcy usług kryptograficznych, dostawcy pośrednich i odsprzedawcy pośrednim</span><span class="sxs-lookup"><span data-stu-id="4d2d2-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="4d2d2-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="4d2d2-106">**Appropriate roles**</span></span>

- <span data-ttu-id="4d2d2-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="4d2d2-107">Admin agent</span></span>
- <span data-ttu-id="4d2d2-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="4d2d2-108">Global admin</span></span>
- <span data-ttu-id="4d2d2-109">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="4d2d2-109">Sales agent</span></span>
- <span data-ttu-id="4d2d2-110">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="4d2d2-110">User management admin</span></span>

<span data-ttu-id="4d2d2-111">Jeśli zarządzasz urządzeniami klienta, może być konieczne dostosowanie środowiska OOBE (out-of-Box Experience) dla użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="4d2d2-112">Można wstępnie skonfigurować nowe urządzenia z profilami autopilotażu systemu Windows przed dostarczeniem urządzeń do klientów i zastosować nowe profile do urządzeń, które zostały już zakupione.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="4d2d2-113">Należy pamiętać, że producenci OEM, którzy uruchomili etykietę wysyłkową na zewnątrz pola urządzenie pilotażowe, pokazujący **Identyfikator klucza produktu (PKID)** urządzenia.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="4d2d2-114">Ten 1-wymiarowy, czytelny kod kreskowy zapewnia partnerom podrzędnym możliwość rejestrowania urządzeń dla autopilotażu bez konieczności Unbox urządzeń i zbierania identyfikatorów urządzeń przy użyciu alternatywnych metod.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="4d2d2-115">W tym artykule wyjaśniono, jak utworzyć i zastosować profile autopilotażu na urządzeniach w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="4d2d2-116">Jeśli nie znasz już programu pilotażowego, zapoznaj się z informacjami w poniższych artykułach:</span><span class="sxs-lookup"><span data-stu-id="4d2d2-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="4d2d2-117">Omówienie funkcji autopilotażu systemu Windows</span><span class="sxs-lookup"><span data-stu-id="4d2d2-117">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="4d2d2-118">Przewodnik dotyczący wdrażania w programie autopilotaż</span><span class="sxs-lookup"><span data-stu-id="4d2d2-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="4d2d2-119">Omówienie</span><span class="sxs-lookup"><span data-stu-id="4d2d2-119">Overview</span></span>

<span data-ttu-id="4d2d2-120">Dzięki funkcji autopilotażu systemu Windows w centrum partnerskim można tworzyć niestandardowe profile, które mają zastosowanie do urządzeń klienckich.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="4d2d2-121">Następujące ustawienia profilu były dostępne po opublikowaniu tego artykułu:</span><span class="sxs-lookup"><span data-stu-id="4d2d2-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="4d2d2-122">Pomiń ustawienia prywatności.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-122">Skip privacy settings.</span></span> <span data-ttu-id="4d2d2-123">To opcjonalne ustawienie profilu autopilotażu pozwala organizacjom nie żądać ustawień prywatności podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="4d2d2-124">Wyłącz tworzenie konta administratora lokalnego na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="4d2d2-125">Organizacje mogą zdecydować, czy użytkownik konfigurujący urządzenie powinien mieć dostęp administratora po zakończeniu procesu.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="4d2d2-126">Automatycznie Skonfiguruj urządzenie pod kątem pracy lub szkoły.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="4d2d2-127">Wszystkie urządzenia zarejestrowane za pomocą autopilotażu będą automatycznie uznawane za urządzenia służbowe, więc nie będzie to konieczne w trakcie procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="4d2d2-128">Pomiń strony konfiguracji Cortany, OneDrive i rejestracji OEM.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="4d2d2-129">Wszystkie urządzenia zarejestrowane za pomocą autopilotażu automatycznie pomijają te strony podczas procesu OOBE (out-of-Box Experience).</span><span class="sxs-lookup"><span data-stu-id="4d2d2-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="4d2d2-130">Pomiń umowę licencyjną użytkownika oprogramowania (EULA).</span><span class="sxs-lookup"><span data-stu-id="4d2d2-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="4d2d2-131">Począwszy od systemu Windows 10 w wersji 1709, organizacje mogą zdecydować o pominięciu strony umów EULA przedstawionych podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="4d2d2-132">Aby zapoznać się z ważnymi informacjami na temat pomijania strony umów EULA podczas instalacji systemu Windows, zobacz sekcję dotyczącą [umowy EULA systemu Windows](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="4d2d2-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="4d2d2-133">Mają zastosowanie następujące uprawnienia i ograniczenia dotyczące zarządzania profilami i urządzeniami:</span><span class="sxs-lookup"><span data-stu-id="4d2d2-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="4d2d2-134">Partnerzy programu CSP mogą nadal zarządzać profilami rozwiązania Autopilot dla istniejących klientów, z którymi mają relacje odsprzedawcy, nawet jeśli klienci usunęli uprawnienia administracji delegowanej dla partnerów.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="4d2d2-135">Możesz zarządzać istniejącymi urządzeniami dla dodanych przez Ciebie klientów.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="4d2d2-136">Nie możesz zarządzać urządzeniami przekazanymi przez Twojego klienta do sklepu Microsoft Store dla firm lub portalu usługi Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="4d2d2-137">Tworzenie profilów autopilotażu i zarządzanie nimi w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="4d2d2-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="4d2d2-138">W centrum partnerskim można utworzyć profile wdrażania systemu Windows i zastosować je do urządzeń.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="4d2d2-139">Tylko agenci administracyjni mogą tworzyć i stosować profile.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="4d2d2-140">Utwórz nowy profil autopilotażu</span><span class="sxs-lookup"><span data-stu-id="4d2d2-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="4d2d2-141">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego tworzysz profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="4d2d2-142">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-142">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="4d2d2-143">W obszarze **Profile autopilotaż systemu Windows** wybierz pozycję **Dodaj nowy profil**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-143">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="4d2d2-144">Wprowadź nazwę i opis profilu, a następnie skonfiguruj ustawienia OOBE.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="4d2d2-145">Wybierz spośród opcji:</span><span class="sxs-lookup"><span data-stu-id="4d2d2-145">Choose from:</span></span>  

   - <span data-ttu-id="4d2d2-146">Pomiń ustawienia prywatności w instalatorze</span><span class="sxs-lookup"><span data-stu-id="4d2d2-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="4d2d2-147">Wyłącz konto administratora lokalnego w instalatorze</span><span class="sxs-lookup"><span data-stu-id="4d2d2-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="4d2d2-148">Automatycznie Pomijaj strony w instalatorze</span><span class="sxs-lookup"><span data-stu-id="4d2d2-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="4d2d2-149">(Obejmuje *Automatyczne wybieranie ustawień dotyczących pracy lub szkoły* oraz *pomijanie stron ustawień rejestracji Cortany, OneDrive i OEM* )</span><span class="sxs-lookup"><span data-stu-id="4d2d2-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages* )</span></span>
  
   - <span data-ttu-id="4d2d2-150">Pomiń umowę licencyjną użytkownika oprogramowania (EULA)</span><span class="sxs-lookup"><span data-stu-id="4d2d2-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="4d2d2-151">Aby zapoznać się z ważnymi informacjami na temat pomijania strony umów EULA podczas instalacji systemu Windows, zobacz sekcję dotyczącą [umowy EULA systemu Windows](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="4d2d2-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="4d2d2-152">Po zakończeniu wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="4d2d2-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="4d2d2-153">Stosowanie profilu autopilotażu do urządzeń klienckich</span><span class="sxs-lookup"><span data-stu-id="4d2d2-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="4d2d2-154">W poniższych instrukcjach przyjęto założenie, że urządzenia klienta zostały już dodane do Centrum partnerskiego i że można uzyskać dostęp do listy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="4d2d2-155">Jeśli urządzenia klienta nie zostały jeszcze dodane, postępuj zgodnie z instrukcjami w temacie [Dodawanie urządzeń do konta klienta](#add-devices-to-a-customers-account) , a następnie wykonaj poniższe kroki.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="4d2d2-156">Po utworzeniu profilu programu pilotażowego dla klienta można go zastosować na urządzeniach klienta.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="4d2d2-157">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego został utworzony profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="4d2d2-158">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-158">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="4d2d2-159">W obszarze **Zastosuj profile do urządzeń** wybierz urządzenia lub grupy urządzeń, do których chcesz dodać profile, a następnie wybierz pozycję **Zastosuj profil**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="4d2d2-160">Właśnie stosowany profil zostanie wyświetlony w kolumnie **profil** .</span><span class="sxs-lookup"><span data-stu-id="4d2d2-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="4d2d2-161">Wykonaj poniższe kroki, aby sprawdzić, czy profil zostanie pomyślnie zastosowany do urządzenia.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="4d2d2-162">a.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-162">a.</span></span>  <span data-ttu-id="4d2d2-163">Podłącz urządzenie do sieci i włącz je.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="4d2d2-164">b.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-164">b.</span></span>  <span data-ttu-id="4d2d2-165">Sprawdź, czy są wyświetlane odpowiednie ekrany OOBE (jeśli istnieją).</span><span class="sxs-lookup"><span data-stu-id="4d2d2-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="4d2d2-166">c.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-166">c.</span></span>  <span data-ttu-id="4d2d2-167">Po zatrzymaniu procesu OOBE Zresetuj urządzenie do domyślnych ustawień fabrycznych, aby przygotować je do nowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="4d2d2-168">Usuwanie profilu autopilotażu z urządzenia klienta</span><span class="sxs-lookup"><span data-stu-id="4d2d2-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="4d2d2-169">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego został utworzony profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="4d2d2-170">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-170">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="4d2d2-171">W obszarze **Zastosuj profile do urządzeń** wybierz urządzenia, z których chcesz usunąć profil, a następnie wybierz pozycję **Usuń profil**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="4d2d2-172">Usunięcie profilu z urządzenia nie powoduje usunięcia go z listy.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="4d2d2-173">Jeśli chcesz usunąć profil, postępuj zgodnie z instrukcjami w temacie [Aktualizowanie lub usuwanie profilu autopilotażu](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="4d2d2-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="4d2d2-174">Aktualizowanie lub usuwanie profilu autopilotażu</span><span class="sxs-lookup"><span data-stu-id="4d2d2-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="4d2d2-175">Jeśli klient chce zmienić wbudowane środowisko po wysłaniu do nich urządzeń, można zmienić profil w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="4d2d2-176">Gdy urządzenie klienta nawiązuje połączenie z Internetem, pobiera najnowsze wersje profilu podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="4d2d2-177">Ponadto w przypadku gdy klient przywraca domyślne ustawienia fabryczne urządzenia, urządzenie powróci do najnowszej wersji profilu podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="4d2d2-178">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, który chce zmienić profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="4d2d2-179">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-179">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="4d2d2-180">W obszarze **Profile autopilotaż systemu Windows** wybierz profil, który ma zostać zaktualizowany.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="4d2d2-181">Wprowadź wymagane zmiany, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-181">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="4d2d2-182">Aby usunąć ten profil, wybierz pozycję **Usuń profil** w prawym górnym rogu strony.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="4d2d2-183">Dodawanie urządzeń do konta klienta</span><span class="sxs-lookup"><span data-stu-id="4d2d2-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="4d2d2-184">Agenci sprzedaży i agenci administracyjni mogą dodawać urządzenia do konta klienta.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="4d2d2-185">Aby można było zastosować niestandardowe profile autopilotażu na urządzeniach klienckich, musisz mieć dostęp do listy urządzeń klienta.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="4d2d2-186">Jeśli planujesz użycie nazwy producenta OEM, numeru seryjnego i kombinacji modelu, należy pamiętać o następujących ograniczeniach:</span><span class="sxs-lookup"><span data-stu-id="4d2d2-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="4d2d2-187">Ta krotka działa tylko w przypadku nowszych urządzeń (na przykład skrótów 4K) i nie jest obsługiwana w przypadku skrótów 128B (RS2 i starszych urządzeń).</span><span class="sxs-lookup"><span data-stu-id="4d2d2-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="4d2d2-188">W rejestracji spójnej kolekcji jest uwzględniana wielkość liter, dlatego dane w pliku muszą być zgodne z nazwą modelu i producenta, ***tak jak to*** zostało podane przez dostawcę OEM (dostawca sprzętu).</span><span class="sxs-lookup"><span data-stu-id="4d2d2-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="4d2d2-189">Postępuj zgodnie z poniższymi instrukcjami, aby dodać urządzenia do konta klienta w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="4d2d2-190">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, którego urządzenia chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="4d2d2-191">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-191">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="4d2d2-192">W obszarze **Zastosuj profile do urządzeń** wybierz pozycję **Dodaj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-192">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="4d2d2-193">Wprowadź nazwę listy urządzeń, a następnie wybierz pozycję **Przeglądaj** , aby przekazać listę klientów (w formacie pliku CSV) do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="4d2d2-194">Plik CSV powinien zostać odebrany przy użyciu zakupu urządzenia.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="4d2d2-195">Jeśli plik CSV nie został odebrany, możesz go utworzyć, wykonując czynności opisane w temacie [Dodawanie urządzeń do systemu Windows autopilotaż](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="4d2d2-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="4d2d2-196">Przekaż plik CSV, a następnie wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-196">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="4d2d2-197">Jeśli podczas próby przekazania pliku CSV zostanie wyświetlony komunikat o błędzie, sprawdź format pliku.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="4d2d2-198">Możesz użyć samego skrótu sprzętu lub nazwy producenta OEM, numeru seryjnego i modelu (w tej kolejności kolumn) lub identyfikatora produktu systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="4d2d2-199">Możesz również użyć pliku CSV z linkiem obok pozycji **Dodaj urządzenia** , aby utworzyć listę urządzeń.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="4d2d2-200">Plik CSV powinien wyglądać następująco:</span><span class="sxs-lookup"><span data-stu-id="4d2d2-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="4d2d2-201">**Numer seryjny urządzenia, identyfikator produktu systemu Windows, skrót sprzętu, nazwa producenta, model urządzenia**</span><span class="sxs-lookup"><span data-stu-id="4d2d2-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="4d2d2-202">**{numer_seryjny},,, Microsoft Corporation, Surface laptop**</span><span class="sxs-lookup"><span data-stu-id="4d2d2-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="4d2d2-203">"Nazwa producenta" i "model urządzenia" są rozróżniana wielkość liter.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="4d2d2-204">Jeśli nie wiesz, jakie wartości należy umieścić w polu Nazwa producenta i model urządzenia, możesz uruchomić to urządzenie, aby zebrać poprawne wartości:</span><span class="sxs-lookup"><span data-stu-id="4d2d2-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="4d2d2-205">Odrzucanie umowy EULA systemu Windows</span><span class="sxs-lookup"><span data-stu-id="4d2d2-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="4d2d2-206">WAŻNE INFORMACJE</span><span class="sxs-lookup"><span data-stu-id="4d2d2-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="4d2d2-207">Program Windows automatycznie pilotaż umożliwia skonfigurowanie dostosowanych instalacji systemu Windows na urządzeniach zarządzanych przez klientów.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="4d2d2-208">Jeśli klient zezwoli na to w tym celu, można pominąć lub ukryć niektóre ekrany skonfigurowane, które są zwykle prezentowane użytkownikom podczas konfigurowania systemu Windows, w tym na ekranie akceptacji umowy licencyjnej użytkownika oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="4d2d2-209">Za pomocą tej funkcji, użytkownik wyraża zgodę na pominięcie lub ukrycie wszelkich ekranów, które zostały zaprojektowane w celu udostępnienia użytkownikom informacji lub akceptacji warunków oznacza, że uzyskano wystarczającą zgodę i autoryzację od klienta, aby ukryć warunki i w imieniu klienta (czy organizacja lub indywidualny użytkownik może mieć możliwość), wyrazić zgodę na wszelkie powiadomienia i zaakceptować warunki, które są odpowiednie dla klienta.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="4d2d2-210">Obejmuje to umowę dotyczącą warunków i postanowień licencyjnych lub informacji, które byłyby widoczne dla użytkownika, jeśli nie została pominięta lub ukryta przy użyciu tego narzędzia.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="4d2d2-211">Klient nie może używać oprogramowania systemu Windows na tych urządzeniach, jeśli klient nie uzyskał ważnej licencji na oprogramowanie firmy Microsoft lub jej licencjonowanych dystrybutorów.</span><span class="sxs-lookup"><span data-stu-id="4d2d2-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>