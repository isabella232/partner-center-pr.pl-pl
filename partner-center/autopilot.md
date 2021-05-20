---
title: Dostosowywanie out-of-box experience urządzenia
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Przed dostarczeniem nowego urządzenia klienta można użyć profilów usługi Windows Autopilot w celu dostosowania lub wstępnego skonfigurowania out-of-box experience (OOBE) urządzenia.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149829"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="5fd18-103">Używanie profilów rozwiązania Windows Autopilot na nowych urządzeniach w celu dostosowania środowiska gotowego do użycia dla klienta</span><span class="sxs-lookup"><span data-stu-id="5fd18-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="5fd18-104">**Odpowiednie role:** Administrator | Administrator globalny | Agent sprzedaży | Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="5fd18-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="5fd18-105">Jeśli zarządzasz urządzeniami klienta, może być konieczne dostosowanie out-of-box experience (OOBE) dla użytkowników klienta.</span><span class="sxs-lookup"><span data-stu-id="5fd18-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="5fd18-106">Nowe urządzenia można wstępnie skonfigurować przy użyciu profilów Windows Autopilot przed dostarczeniem urządzeń do klientów i zastosować nowe profile do już zakupionych urządzeń.</span><span class="sxs-lookup"><span data-stu-id="5fd18-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="5fd18-107">Należy pamiętać, że od producentów OEM rozpoczęto zawieranie etykiety wysyłkowej poza polem urządzenia rozwiązania Autopilot, które zawiera identyfikator klucza produktu **(PKID) urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="5fd18-108">Ten 1-wymiarowy, czytelny kod kreskowy zapewnia partnerom niższego szczebla możliwość rejestrowania urządzeń w programie Autopilot bez konieczności rozpakowania urządzeń i zbierania identyfikatorów urządzeń w alternatywny sposób.</span><span class="sxs-lookup"><span data-stu-id="5fd18-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="5fd18-109">W tym artykule wyjaśniono, jak tworzyć i stosować profile rozwiązania Autopilot do urządzeń w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5fd18-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="5fd18-110">Jeśli nie znasz jeszcze rozwiązania Autopilot, zapoznaj się z informacjami w tych artykułach:</span><span class="sxs-lookup"><span data-stu-id="5fd18-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="5fd18-111">Omówienie rozwiązania Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="5fd18-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="5fd18-112">Podręcznik wdrażania rozwiązania Autopilot</span><span class="sxs-lookup"><span data-stu-id="5fd18-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="5fd18-113">Omówienie</span><span class="sxs-lookup"><span data-stu-id="5fd18-113">Overview</span></span>

<span data-ttu-id="5fd18-114">Dzięki funkcji Windows Autopilot na Partner Center można tworzyć profile niestandardowe do zastosowania na urządzeniach klientów.</span><span class="sxs-lookup"><span data-stu-id="5fd18-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="5fd18-115">W momencie opublikowania tego artykułu były dostępne następujące ustawienia profilu:</span><span class="sxs-lookup"><span data-stu-id="5fd18-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="5fd18-116">Pomiń ustawienia prywatności.</span><span class="sxs-lookup"><span data-stu-id="5fd18-116">Skip privacy settings.</span></span> <span data-ttu-id="5fd18-117">To opcjonalne ustawienie profilu rozwiązania Autopilot pozwala organizacjom nie pytać o ustawienia prywatności podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="5fd18-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="5fd18-118">Wyłącz tworzenie konta administratora lokalnego na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="5fd18-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="5fd18-119">Organizacje mogą zdecydować, czy po zakończeniu procesu użytkownik konfiguracji urządzenia powinien mieć dostęp administratora.</span><span class="sxs-lookup"><span data-stu-id="5fd18-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="5fd18-120">Automatycznie skonfiguruj urządzenie do pracy lub nauki.</span><span class="sxs-lookup"><span data-stu-id="5fd18-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="5fd18-121">Wszystkie urządzenia zarejestrowane przy użyciu rozwiązania Autopilot zostaną automatycznie uznane za urządzenia służbowe, więc to pytanie nie zostanie zadane podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="5fd18-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="5fd18-122">Pomiń strony konfiguracji cortany, usługi OneDrive i rejestracji OEM.</span><span class="sxs-lookup"><span data-stu-id="5fd18-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="5fd18-123">Wszystkie urządzenia zarejestrowane przy użyciu rozwiązania Autopilot będą automatycznie pomijać te strony podczas procesu OOBE (out-of-box experience).</span><span class="sxs-lookup"><span data-stu-id="5fd18-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="5fd18-124">Pomiń umowę licencyjną użytkownika oprogramowania (EULA).</span><span class="sxs-lookup"><span data-stu-id="5fd18-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="5fd18-125">Począwszy od Windows 10 wersji 1709, organizacje mogą zdecydować się pominąć stronę eula przedstawioną podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="5fd18-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="5fd18-126">Zobacz [Windows Autopilot poniżej,](#windows-autopilot-eula-dismissal) aby uzyskać ważne informacje dotyczące pomijania strony eula podczas instalacji systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="5fd18-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="5fd18-127">Mają zastosowanie następujące uprawnienia i ograniczenia dotyczące zarządzania profilami i urządzeniami:</span><span class="sxs-lookup"><span data-stu-id="5fd18-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="5fd18-128">Partnerzy programu CSP mogą nadal zarządzać profilami rozwiązania Autopilot dla istniejących klientów, z którymi mają relacje odsprzedawcy, nawet jeśli klienci usunęli uprawnienia administracji delegowanej dla partnerów.</span><span class="sxs-lookup"><span data-stu-id="5fd18-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="5fd18-129">Możesz zarządzać istniejącymi urządzeniami dla dodanych przez Ciebie klientów.</span><span class="sxs-lookup"><span data-stu-id="5fd18-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="5fd18-130">Nie możesz zarządzać urządzeniami przekazanymi przez Twojego klienta do sklepu Microsoft Store dla firm lub portalu usługi Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="5fd18-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="5fd18-131">Tworzenie profilów rozwiązania Autopilot i zarządzanie nimi w Partner Center</span><span class="sxs-lookup"><span data-stu-id="5fd18-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="5fd18-132">W Partner Center można tworzyć Windows Autopilot wdrażania i stosować je do urządzeń.</span><span class="sxs-lookup"><span data-stu-id="5fd18-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="5fd18-133">Tylko agenci administracyjni mogą tworzyć i stosować profile.</span><span class="sxs-lookup"><span data-stu-id="5fd18-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="5fd18-134">Tworzenie nowego profilu rozwiązania Autopilot</span><span class="sxs-lookup"><span data-stu-id="5fd18-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="5fd18-135">Wybierz **pozycję** Klienci Partner Center menu, a następnie wybierz klienta, dla których tworzysz profil rozwiązania Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5fd18-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="5fd18-136">Na stronie szczegółów klienta wybierz pozycję **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="5fd18-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5fd18-137">W **Windows Autopilot profilów wybierz** pozycję Dodaj nowy **profil.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="5fd18-138">Wprowadź nazwę i opis profilu, a następnie skonfiguruj ustawienia OOBE.</span><span class="sxs-lookup"><span data-stu-id="5fd18-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="5fd18-139">Wybierz spośród opcji:</span><span class="sxs-lookup"><span data-stu-id="5fd18-139">Choose from:</span></span>  

   - <span data-ttu-id="5fd18-140">Pomijanie ustawień prywatności w konfiguracji</span><span class="sxs-lookup"><span data-stu-id="5fd18-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="5fd18-141">Wyłączanie konta administratora lokalnego w instalatorze</span><span class="sxs-lookup"><span data-stu-id="5fd18-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="5fd18-142">Automatyczne pomijanie stron w konfiguracji</span><span class="sxs-lookup"><span data-stu-id="5fd18-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="5fd18-143">(Obejmuje *automatyczne wybieranie ustawień dla służbowych* i *pomijanie cortany, usługi OneDrive* i stron konfiguracji rejestracji OEM)</span><span class="sxs-lookup"><span data-stu-id="5fd18-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="5fd18-144">Pomiń umowę licencyjną użytkownika końcowego (EULA)</span><span class="sxs-lookup"><span data-stu-id="5fd18-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="5fd18-145">Zobacz [Windows Autopilot poniżej,](#windows-autopilot-eula-dismissal) aby uzyskać ważne informacje dotyczące pomijania strony eula podczas instalacji systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="5fd18-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="5fd18-146">Po **zakończeniu wybierz** pozycję Prześlij.</span><span class="sxs-lookup"><span data-stu-id="5fd18-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="5fd18-147">Stosowanie profilu rozwiązania Autopilot do urządzeń klientów</span><span class="sxs-lookup"><span data-stu-id="5fd18-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="5fd18-148">W poniższych instrukcjach przyjęto założenie, że urządzenia klienta zostały już dodane do Partner Center i że możesz uzyskać dostęp do jego listy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="5fd18-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="5fd18-149">Jeśli urządzenia klienta nie zostały jeszcze dodane, postępuj zgodnie z instrukcjami w artykule Dodawanie urządzeń do konta klienta, [a](#add-devices-to-a-customers-account) następnie wykonaj poniższe kroki.</span><span class="sxs-lookup"><span data-stu-id="5fd18-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="5fd18-150">Po utworzeniu profilu rozwiązania Autopilot dla klienta można go zastosować do urządzeń klienta.</span><span class="sxs-lookup"><span data-stu-id="5fd18-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="5fd18-151">Wybierz **pozycję** Customers (Klienci) Partner Center menu aplikacji, a następnie wybierz klienta, dla których utworzono profil rozwiązania Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5fd18-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="5fd18-152">Na stronie szczegółów klienta wybierz pozycję **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="5fd18-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5fd18-153">W **obszarze Zastosuj profile do urządzeń** wybierz urządzenia lub grupy urządzeń, do których chcesz dodać profile, a następnie wybierz pozycję Zastosuj **profil.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="5fd18-154">Właśnie zastosowany profil zostanie wyświetlony w **kolumnie** Profil.</span><span class="sxs-lookup"><span data-stu-id="5fd18-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="5fd18-155">Wykonaj poniższe kroki, aby sprawdzić, czy profil zostanie pomyślnie zastosowany do urządzenia.</span><span class="sxs-lookup"><span data-stu-id="5fd18-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="5fd18-156">a.</span><span class="sxs-lookup"><span data-stu-id="5fd18-156">a.</span></span>  <span data-ttu-id="5fd18-157">Podłącz urządzenie do sieci i włącz je.</span><span class="sxs-lookup"><span data-stu-id="5fd18-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="5fd18-158">b.</span><span class="sxs-lookup"><span data-stu-id="5fd18-158">b.</span></span>  <span data-ttu-id="5fd18-159">Sprawdź, czy są wyświetlane odpowiednie ekrany OOBE (jeśli występują).</span><span class="sxs-lookup"><span data-stu-id="5fd18-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="5fd18-160">c.</span><span class="sxs-lookup"><span data-stu-id="5fd18-160">c.</span></span>  <span data-ttu-id="5fd18-161">Po zatrzymaniu procesu OOBE przywróć domyślne ustawienia fabryczne urządzenia, aby przygotować je dla nowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="5fd18-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="5fd18-162">Usuwanie profilu rozwiązania Autopilot z urządzenia klienta</span><span class="sxs-lookup"><span data-stu-id="5fd18-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="5fd18-163">Wybierz **pozycję** Customers (Klienci) Partner Center menu aplikacji, a następnie wybierz klienta, dla których utworzono profil rozwiązania Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5fd18-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="5fd18-164">Na stronie szczegółów klienta wybierz pozycję **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="5fd18-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5fd18-165">W **obszarze Zastosuj profile do urządzeń** wybierz urządzenia, z których chcesz usunąć profil, a następnie wybierz pozycję Usuń **profil.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="5fd18-166">Usunięcie profilu z urządzenia nie powoduje usunięcia profilu z listy.</span><span class="sxs-lookup"><span data-stu-id="5fd18-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="5fd18-167">Jeśli chcesz usunąć profil, postępuj zgodnie z instrukcjami w sekcji [Aktualizowanie lub usuwanie profilu rozwiązania Autopilot.](#update-or-delete-an-autopilot-profile)</span><span class="sxs-lookup"><span data-stu-id="5fd18-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="5fd18-168">Aktualizowanie lub usuwanie profilu rozwiązania Autopilot</span><span class="sxs-lookup"><span data-stu-id="5fd18-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="5fd18-169">Jeśli klient chce zmienić środowisko out-of-box po wysłaniu do nich urządzeń, możesz zmienić profil w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5fd18-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="5fd18-170">Gdy urządzenie klienta połączy się z Internetem, pobierze najnowszą wersję profilu podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="5fd18-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="5fd18-171">Ponadto za każdym razem, gdy klient przywróci urządzenie do domyślnych ustawień fabrycznych, urządzenie ponownie pobierze najnowszą wersję profilu podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="5fd18-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="5fd18-172">Wybierz **pozycję** Klienci z Partner Center, a następnie wybierz klienta, który chce, aby zmienić profil rozwiązania Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5fd18-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="5fd18-173">Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5fd18-174">W **Windows Autopilot profilów** wybierz profil, który chcesz zaktualizować.</span><span class="sxs-lookup"><span data-stu-id="5fd18-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="5fd18-175">Określ wymagane zmiany, a następnie wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="5fd18-176">Aby usunąć ten profil, wybierz **pozycję Usuń profil** w prawym górnym rogu strony.</span><span class="sxs-lookup"><span data-stu-id="5fd18-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="5fd18-177">Dodawanie urządzeń do konta klienta</span><span class="sxs-lookup"><span data-stu-id="5fd18-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="5fd18-178">Agenci sprzedaży i agenci administracyjni mogą dodawać urządzenia do konta klienta.</span><span class="sxs-lookup"><span data-stu-id="5fd18-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="5fd18-179">Aby można było zastosować niestandardowe profile rozwiązania Autopilot do urządzeń klientów, musisz mieć dostęp do listy urządzeń klienta.</span><span class="sxs-lookup"><span data-stu-id="5fd18-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="5fd18-180">Jeśli planujesz używać nazwy OEM, numeru seryjnego i kombinacji modelu, należy pamiętać o tych ograniczeniach:</span><span class="sxs-lookup"><span data-stu-id="5fd18-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="5fd18-181">Ta krotka działa tylko w przypadku urządzeń nowszej (na przykład 4k skrótów) i nie jest obsługiwana w przypadku skrótów 128b (RS2 i poprzednich urządzeń).</span><span class="sxs-lookup"><span data-stu-id="5fd18-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="5fd18-182">W rejestracji krotki jest wielkość liter, dlatego dane w pliku  muszą być zgodne z nazwami modelu i producenta dokładnie tak, jak podano w przypadku dostawcy OEM (dostawcy sprzętu).</span><span class="sxs-lookup"><span data-stu-id="5fd18-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="5fd18-183">Postępuj zgodnie z poniższymi instrukcjami, aby dodać urządzenia do konta klienta w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5fd18-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="5fd18-184">Wybierz **pozycję** Klienci z Partner Center, a następnie wybierz klienta, którego urządzeniami chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="5fd18-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="5fd18-185">Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5fd18-186">W **obszarze Zastosuj profile do urządzeń wybierz** pozycję Dodaj **urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="5fd18-187">Wprowadź nazwę listy urządzeń, a  następnie wybierz pozycję Przeglądaj, aby przekazać listę klientów (w formacie pliku CSV) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5fd18-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="5fd18-188">Ten plik CSV powinien zostać odebrany wraz z zakupem urządzenia.</span><span class="sxs-lookup"><span data-stu-id="5fd18-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="5fd18-189">Jeśli nie otrzymasz pliku CSV, możesz go utworzyć samodzielnie, korzystając z procedury opisanej w temacie [Dodawanie](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)urządzeń do Windows Autopilot .</span><span class="sxs-lookup"><span data-stu-id="5fd18-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="5fd18-190">Przekaż plik CSV, a następnie wybierz pozycję **Zapisz.**</span><span class="sxs-lookup"><span data-stu-id="5fd18-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="5fd18-191">Jeśli podczas próby przekazania pliku CSV zostanie wyświetlony komunikat o błędzie, sprawdź format pliku.</span><span class="sxs-lookup"><span data-stu-id="5fd18-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="5fd18-192">Możesz użyć samego skrótu sprzętu lub nazwy producenta OEM, numeru seryjnego i modelu (w tej kolejności kolumn) lub identyfikatora produktu systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="5fd18-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="5fd18-193">Możesz również użyć przykładowego pliku CSV dostarczonego za pomocą linku obok **przycisku Dodaj urządzenia,** aby utworzyć listę urządzeń.</span><span class="sxs-lookup"><span data-stu-id="5fd18-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="5fd18-194">Plik CSV powinien wyglądać podobnie do tego:</span><span class="sxs-lookup"><span data-stu-id="5fd18-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="5fd18-195">**Numer seryjny urządzenia,Identyfikator produktu systemu Windows,Skrót sprzętu,Nazwa producenta,Model urządzenia**</span><span class="sxs-lookup"><span data-stu-id="5fd18-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="5fd18-196">**{serialNumber},,,Microsoft Corporation, Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="5fd18-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="5fd18-197">W polach "Nazwa producenta" i "Model urządzenia" jest wielkość liter.</span><span class="sxs-lookup"><span data-stu-id="5fd18-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="5fd18-198">Jeśli nie wiesz, jaką wartość należy umieścić dla pól Nazwa producenta i Model urządzenia, możesz uruchomić tę wartość na urządzeniu, aby zebrać poprawne wartości:</span><span class="sxs-lookup"><span data-stu-id="5fd18-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="5fd18-199">Windows Autopilot odrzuć eula</span><span class="sxs-lookup"><span data-stu-id="5fd18-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="5fd18-200">WAŻNE INFORMACJE</span><span class="sxs-lookup"><span data-stu-id="5fd18-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="5fd18-201">Windows Autopilot umożliwia skonfigurowanie dostosowanych instalacji systemu Windows na urządzeniach, które są zarządzane dla klientów.</span><span class="sxs-lookup"><span data-stu-id="5fd18-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="5fd18-202">W przypadku autoryzacji klienta można pominąć lub ukryć niektóre ekrany konfiguracji, które są zwykle prezentowane użytkownikom podczas konfigurowania systemu Windows, w tym ekran akceptacji umowy licencyjnej użytkownika oprogramowania (EULA).</span><span class="sxs-lookup"><span data-stu-id="5fd18-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="5fd18-203">Korzystając z tej funkcji, użytkownik zgadza się, że pomijanie lub ukrywanie ekranów, które mają na celu powiadomienie lub akceptację warunków, oznacza, że klient uzyskał wystarczającą zgodę i autoryzację, aby ukryć warunki, oraz że w imieniu klienta (w zależności od przypadku organizacji lub użytkownika indywidualnego) wyraża zgodę na wszelkie powiadomienia i akceptuje wszelkie postanowienia dotyczące klienta.</span><span class="sxs-lookup"><span data-stu-id="5fd18-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="5fd18-204">Obejmuje to umowę z warunkami i postanowieniami licencji lub powiadomienie, które zostaną przedstawione użytkownikowi, jeśli użytkownik nie pominął ani nie ukrywał jej za pomocą tego narzędzia.</span><span class="sxs-lookup"><span data-stu-id="5fd18-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="5fd18-205">Klient nie może korzystać z oprogramowania systemu Windows na tych urządzeniach, jeśli klient nie uzyskał w prawidłowy sposób licencji na oprogramowanie od firmy Microsoft lub licencjonowanych dystrybutorów.</span><span class="sxs-lookup"><span data-stu-id="5fd18-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>