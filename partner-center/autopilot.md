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
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534997"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="661f4-103">Używanie profilów rozwiązania Windows Autopilot na nowych urządzeniach w celu dostosowania środowiska gotowego do użycia dla klienta</span><span class="sxs-lookup"><span data-stu-id="661f4-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="661f4-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="661f4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="661f4-105">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="661f4-105">Admin agent</span></span>
- <span data-ttu-id="661f4-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="661f4-106">Global admin</span></span>
- <span data-ttu-id="661f4-107">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="661f4-107">Sales agent</span></span>
- <span data-ttu-id="661f4-108">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="661f4-108">User management admin</span></span>

<span data-ttu-id="661f4-109">Jeśli zarządzasz urządzeniami klienta, może być konieczne dostosowanie środowiska OOBE (out-of-Box Experience) dla użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="661f4-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="661f4-110">Można wstępnie skonfigurować nowe urządzenia z profilami autopilotażu systemu Windows przed dostarczeniem urządzeń do klientów i zastosować nowe profile do urządzeń, które zostały już zakupione.</span><span class="sxs-lookup"><span data-stu-id="661f4-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="661f4-111">Należy pamiętać, że producenci OEM, którzy uruchomili etykietę wysyłkową na zewnątrz pola urządzenie pilotażowe, pokazujący **Identyfikator klucza produktu (PKID)** urządzenia.</span><span class="sxs-lookup"><span data-stu-id="661f4-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="661f4-112">Ten 1-wymiarowy, czytelny kod kreskowy zapewnia partnerom podrzędnym możliwość rejestrowania urządzeń dla autopilotażu bez konieczności Unbox urządzeń i zbierania identyfikatorów urządzeń przy użyciu alternatywnych metod.</span><span class="sxs-lookup"><span data-stu-id="661f4-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="661f4-113">W tym artykule wyjaśniono, jak utworzyć i zastosować profile autopilotażu na urządzeniach w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="661f4-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="661f4-114">Jeśli nie znasz już programu pilotażowego, zapoznaj się z informacjami w poniższych artykułach:</span><span class="sxs-lookup"><span data-stu-id="661f4-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="661f4-115">Omówienie rozwiązania Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="661f4-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="661f4-116">Przewodnik dotyczący wdrażania w programie autopilotaż</span><span class="sxs-lookup"><span data-stu-id="661f4-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="661f4-117">Omówienie</span><span class="sxs-lookup"><span data-stu-id="661f4-117">Overview</span></span>

<span data-ttu-id="661f4-118">Dzięki funkcji autopilotażu systemu Windows w centrum partnerskim można tworzyć niestandardowe profile, które mają zastosowanie do urządzeń klienckich.</span><span class="sxs-lookup"><span data-stu-id="661f4-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="661f4-119">Następujące ustawienia profilu były dostępne po opublikowaniu tego artykułu:</span><span class="sxs-lookup"><span data-stu-id="661f4-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="661f4-120">Pomiń ustawienia prywatności.</span><span class="sxs-lookup"><span data-stu-id="661f4-120">Skip privacy settings.</span></span> <span data-ttu-id="661f4-121">To opcjonalne ustawienie profilu autopilotażu pozwala organizacjom nie żądać ustawień prywatności podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="661f4-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="661f4-122">Wyłącz tworzenie konta administratora lokalnego na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="661f4-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="661f4-123">Organizacje mogą zdecydować, czy użytkownik konfigurujący urządzenie powinien mieć dostęp administratora po zakończeniu procesu.</span><span class="sxs-lookup"><span data-stu-id="661f4-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="661f4-124">Automatycznie Skonfiguruj urządzenie pod kątem pracy lub szkoły.</span><span class="sxs-lookup"><span data-stu-id="661f4-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="661f4-125">Wszystkie urządzenia zarejestrowane za pomocą autopilotażu będą automatycznie uznawane za urządzenia służbowe, więc nie będzie to konieczne w trakcie procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="661f4-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="661f4-126">Pomiń strony konfiguracji Cortany, OneDrive i rejestracji OEM.</span><span class="sxs-lookup"><span data-stu-id="661f4-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="661f4-127">Wszystkie urządzenia zarejestrowane za pomocą autopilotażu automatycznie pomijają te strony podczas procesu OOBE (out-of-Box Experience).</span><span class="sxs-lookup"><span data-stu-id="661f4-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="661f4-128">Pomiń umowę licencyjną użytkownika oprogramowania (EULA).</span><span class="sxs-lookup"><span data-stu-id="661f4-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="661f4-129">Począwszy od systemu Windows 10 w wersji 1709, organizacje mogą zdecydować o pominięciu strony umów EULA przedstawionych podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="661f4-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="661f4-130">Aby zapoznać się z ważnymi informacjami na temat pomijania strony umów EULA podczas instalacji systemu Windows, zobacz sekcję dotyczącą [umowy EULA systemu Windows](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="661f4-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="661f4-131">Mają zastosowanie następujące uprawnienia i ograniczenia dotyczące zarządzania profilami i urządzeniami:</span><span class="sxs-lookup"><span data-stu-id="661f4-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="661f4-132">Partnerzy programu CSP mogą nadal zarządzać profilami rozwiązania Autopilot dla istniejących klientów, z którymi mają relacje odsprzedawcy, nawet jeśli klienci usunęli uprawnienia administracji delegowanej dla partnerów.</span><span class="sxs-lookup"><span data-stu-id="661f4-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="661f4-133">Możesz zarządzać istniejącymi urządzeniami dla dodanych przez Ciebie klientów.</span><span class="sxs-lookup"><span data-stu-id="661f4-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="661f4-134">Nie możesz zarządzać urządzeniami przekazanymi przez Twojego klienta do sklepu Microsoft Store dla firm lub portalu usługi Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="661f4-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="661f4-135">Tworzenie profilów autopilotażu i zarządzanie nimi w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="661f4-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="661f4-136">W centrum partnerskim można utworzyć profile wdrażania systemu Windows i zastosować je do urządzeń.</span><span class="sxs-lookup"><span data-stu-id="661f4-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="661f4-137">Tylko agenci administracyjni mogą tworzyć i stosować profile.</span><span class="sxs-lookup"><span data-stu-id="661f4-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="661f4-138">Utwórz nowy profil autopilotażu</span><span class="sxs-lookup"><span data-stu-id="661f4-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="661f4-139">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego tworzysz profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="661f4-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="661f4-140">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="661f4-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="661f4-141">W obszarze **Profile autopilotaż systemu Windows** wybierz pozycję **Dodaj nowy profil**.</span><span class="sxs-lookup"><span data-stu-id="661f4-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="661f4-142">Wprowadź nazwę i opis profilu, a następnie skonfiguruj ustawienia OOBE.</span><span class="sxs-lookup"><span data-stu-id="661f4-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="661f4-143">Wybierz spośród opcji:</span><span class="sxs-lookup"><span data-stu-id="661f4-143">Choose from:</span></span>  

   - <span data-ttu-id="661f4-144">Pomiń ustawienia prywatności w instalatorze</span><span class="sxs-lookup"><span data-stu-id="661f4-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="661f4-145">Wyłącz konto administratora lokalnego w instalatorze</span><span class="sxs-lookup"><span data-stu-id="661f4-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="661f4-146">Automatycznie Pomijaj strony w instalatorze</span><span class="sxs-lookup"><span data-stu-id="661f4-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="661f4-147">(Obejmuje *Automatyczne wybieranie ustawień dotyczących pracy lub szkoły* oraz *pomijanie stron ustawień rejestracji Cortany, OneDrive i OEM*)</span><span class="sxs-lookup"><span data-stu-id="661f4-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="661f4-148">Pomiń umowę licencyjną użytkownika oprogramowania (EULA)</span><span class="sxs-lookup"><span data-stu-id="661f4-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="661f4-149">Aby zapoznać się z ważnymi informacjami na temat pomijania strony umów EULA podczas instalacji systemu Windows, zobacz sekcję dotyczącą [umowy EULA systemu Windows](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="661f4-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="661f4-150">Po zakończeniu wybierz pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="661f4-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="661f4-151">Stosowanie profilu autopilotażu do urządzeń klienckich</span><span class="sxs-lookup"><span data-stu-id="661f4-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="661f4-152">W poniższych instrukcjach przyjęto założenie, że urządzenia klienta zostały już dodane do Centrum partnerskiego i że można uzyskać dostęp do listy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="661f4-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="661f4-153">Jeśli urządzenia klienta nie zostały jeszcze dodane, postępuj zgodnie z instrukcjami w temacie [Dodawanie urządzeń do konta klienta](#add-devices-to-a-customers-account) , a następnie wykonaj poniższe kroki.</span><span class="sxs-lookup"><span data-stu-id="661f4-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="661f4-154">Po utworzeniu profilu programu pilotażowego dla klienta można go zastosować na urządzeniach klienta.</span><span class="sxs-lookup"><span data-stu-id="661f4-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="661f4-155">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego został utworzony profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="661f4-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="661f4-156">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="661f4-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="661f4-157">W obszarze **Zastosuj profile do urządzeń** wybierz urządzenia lub grupy urządzeń, do których chcesz dodać profile, a następnie wybierz pozycję **Zastosuj profil**.</span><span class="sxs-lookup"><span data-stu-id="661f4-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="661f4-158">Właśnie stosowany profil zostanie wyświetlony w kolumnie **profil** .</span><span class="sxs-lookup"><span data-stu-id="661f4-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="661f4-159">Wykonaj poniższe kroki, aby sprawdzić, czy profil zostanie pomyślnie zastosowany do urządzenia.</span><span class="sxs-lookup"><span data-stu-id="661f4-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="661f4-160">a.</span><span class="sxs-lookup"><span data-stu-id="661f4-160">a.</span></span>  <span data-ttu-id="661f4-161">Podłącz urządzenie do sieci i włącz je.</span><span class="sxs-lookup"><span data-stu-id="661f4-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="661f4-162">b.</span><span class="sxs-lookup"><span data-stu-id="661f4-162">b.</span></span>  <span data-ttu-id="661f4-163">Sprawdź, czy są wyświetlane odpowiednie ekrany OOBE (jeśli istnieją).</span><span class="sxs-lookup"><span data-stu-id="661f4-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="661f4-164">c.</span><span class="sxs-lookup"><span data-stu-id="661f4-164">c.</span></span>  <span data-ttu-id="661f4-165">Po zatrzymaniu procesu OOBE Zresetuj urządzenie do domyślnych ustawień fabrycznych, aby przygotować je do nowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="661f4-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="661f4-166">Usuwanie profilu autopilotażu z urządzenia klienta</span><span class="sxs-lookup"><span data-stu-id="661f4-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="661f4-167">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego został utworzony profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="661f4-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="661f4-168">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="661f4-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="661f4-169">W obszarze **Zastosuj profile do urządzeń** wybierz urządzenia, z których chcesz usunąć profil, a następnie wybierz pozycję **Usuń profil**.</span><span class="sxs-lookup"><span data-stu-id="661f4-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="661f4-170">Usunięcie profilu z urządzenia nie powoduje usunięcia go z listy.</span><span class="sxs-lookup"><span data-stu-id="661f4-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="661f4-171">Jeśli chcesz usunąć profil, postępuj zgodnie z instrukcjami w temacie [Aktualizowanie lub usuwanie profilu autopilotażu](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="661f4-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="661f4-172">Aktualizowanie lub usuwanie profilu autopilotażu</span><span class="sxs-lookup"><span data-stu-id="661f4-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="661f4-173">Jeśli klient chce zmienić wbudowane środowisko po wysłaniu do nich urządzeń, można zmienić profil w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="661f4-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="661f4-174">Gdy urządzenie klienta nawiązuje połączenie z Internetem, pobiera najnowsze wersje profilu podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="661f4-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="661f4-175">Ponadto w przypadku gdy klient przywraca domyślne ustawienia fabryczne urządzenia, urządzenie powróci do najnowszej wersji profilu podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="661f4-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="661f4-176">Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, który chce zmienić profil autopilotażu.</span><span class="sxs-lookup"><span data-stu-id="661f4-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="661f4-177">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="661f4-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="661f4-178">W obszarze **Profile autopilotaż systemu Windows** wybierz profil, który ma zostać zaktualizowany.</span><span class="sxs-lookup"><span data-stu-id="661f4-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="661f4-179">Wprowadź wymagane zmiany, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="661f4-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="661f4-180">Aby usunąć ten profil, wybierz pozycję **Usuń profil** w prawym górnym rogu strony.</span><span class="sxs-lookup"><span data-stu-id="661f4-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="661f4-181">Dodawanie urządzeń do konta klienta</span><span class="sxs-lookup"><span data-stu-id="661f4-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="661f4-182">Agenci sprzedaży i agenci administracyjni mogą dodawać urządzenia do konta klienta.</span><span class="sxs-lookup"><span data-stu-id="661f4-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="661f4-183">Aby można było zastosować niestandardowe profile autopilotażu na urządzeniach klienckich, musisz mieć dostęp do listy urządzeń klienta.</span><span class="sxs-lookup"><span data-stu-id="661f4-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="661f4-184">Jeśli planujesz użycie nazwy producenta OEM, numeru seryjnego i kombinacji modelu, należy pamiętać o następujących ograniczeniach:</span><span class="sxs-lookup"><span data-stu-id="661f4-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="661f4-185">Ta krotka działa tylko w przypadku nowszych urządzeń (na przykład skrótów 4K) i nie jest obsługiwana w przypadku skrótów 128B (RS2 i starszych urządzeń).</span><span class="sxs-lookup"><span data-stu-id="661f4-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="661f4-186">Rejestracja spójnej kolekcji uwzględnia wielkość liter, dlatego dane w pliku muszą być zgodne z nazwą modelu i producenta \**_dokładnie_* znakiem dostarczonym przez dostawcę OEM (dostawca sprzętu).</span><span class="sxs-lookup"><span data-stu-id="661f4-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="661f4-187">Postępuj zgodnie z poniższymi instrukcjami, aby dodać urządzenia do konta klienta w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="661f4-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="661f4-188">Wybierz _ *Customers*\* z menu Centrum partnerskiego, a następnie wybierz klienta, którego urządzenia chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="661f4-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="661f4-189">Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="661f4-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="661f4-190">W obszarze **Zastosuj profile do urządzeń** wybierz pozycję **Dodaj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="661f4-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="661f4-191">Wprowadź nazwę listy urządzeń, a następnie wybierz pozycję **Przeglądaj** , aby przekazać listę klientów (w formacie pliku CSV) do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="661f4-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="661f4-192">Plik CSV powinien zostać odebrany przy użyciu zakupu urządzenia.</span><span class="sxs-lookup"><span data-stu-id="661f4-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="661f4-193">Jeśli plik CSV nie został odebrany, możesz go utworzyć, wykonując czynności opisane w temacie [Dodawanie urządzeń do systemu Windows autopilotaż](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="661f4-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="661f4-194">Przekaż plik CSV, a następnie wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="661f4-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="661f4-195">Jeśli podczas próby przekazania pliku CSV zostanie wyświetlony komunikat o błędzie, sprawdź format pliku.</span><span class="sxs-lookup"><span data-stu-id="661f4-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="661f4-196">Możesz użyć samego skrótu sprzętu lub nazwy producenta OEM, numeru seryjnego i modelu (w tej kolejności kolumn) lub identyfikatora produktu systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="661f4-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="661f4-197">Możesz również użyć pliku CSV z linkiem obok pozycji **Dodaj urządzenia** , aby utworzyć listę urządzeń.</span><span class="sxs-lookup"><span data-stu-id="661f4-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="661f4-198">Plik CSV powinien wyglądać następująco:</span><span class="sxs-lookup"><span data-stu-id="661f4-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="661f4-199">**Numer seryjny urządzenia, identyfikator produktu systemu Windows, skrót sprzętu, nazwa producenta, model urządzenia**</span><span class="sxs-lookup"><span data-stu-id="661f4-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="661f4-200">**{numer_seryjny},,, Microsoft Corporation, Surface laptop**</span><span class="sxs-lookup"><span data-stu-id="661f4-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="661f4-201">"Nazwa producenta" i "model urządzenia" są rozróżniana wielkość liter.</span><span class="sxs-lookup"><span data-stu-id="661f4-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="661f4-202">Jeśli nie wiesz, jakie wartości należy umieścić w polu Nazwa producenta i model urządzenia, możesz uruchomić to urządzenie, aby zebrać poprawne wartości:</span><span class="sxs-lookup"><span data-stu-id="661f4-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="661f4-203">Odrzucanie umowy EULA systemu Windows</span><span class="sxs-lookup"><span data-stu-id="661f4-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="661f4-204">WAŻNE INFORMACJE</span><span class="sxs-lookup"><span data-stu-id="661f4-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="661f4-205">Program Windows automatycznie pilotaż umożliwia skonfigurowanie dostosowanych instalacji systemu Windows na urządzeniach zarządzanych przez klientów.</span><span class="sxs-lookup"><span data-stu-id="661f4-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="661f4-206">Jeśli klient zezwoli na to w tym celu, można pominąć lub ukryć niektóre ekrany skonfigurowane, które są zwykle prezentowane użytkownikom podczas konfigurowania systemu Windows, w tym na ekranie akceptacji umowy licencyjnej użytkownika oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="661f4-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="661f4-207">Za pomocą tej funkcji, użytkownik wyraża zgodę na pominięcie lub ukrycie wszelkich ekranów, które zostały zaprojektowane w celu udostępnienia użytkownikom informacji lub akceptacji warunków oznacza, że uzyskano wystarczającą zgodę i autoryzację od klienta, aby ukryć warunki i w imieniu klienta (czy organizacja lub indywidualny użytkownik może mieć możliwość), wyrazić zgodę na wszelkie powiadomienia i zaakceptować warunki, które są odpowiednie dla klienta.</span><span class="sxs-lookup"><span data-stu-id="661f4-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="661f4-208">Obejmuje to umowę dotyczącą warunków i postanowień licencyjnych lub informacji, które byłyby widoczne dla użytkownika, jeśli nie została pominięta lub ukryta przy użyciu tego narzędzia.</span><span class="sxs-lookup"><span data-stu-id="661f4-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="661f4-209">Klient nie może używać oprogramowania systemu Windows na tych urządzeniach, jeśli klient nie uzyskał ważnej licencji na oprogramowanie firmy Microsoft lub jej licencjonowanych dystrybutorów.</span><span class="sxs-lookup"><span data-stu-id="661f4-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>