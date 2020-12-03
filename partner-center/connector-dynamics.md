---
title: Łącznik współsprzedającego dla Centrum partnerskiego programu Dynamics 365 CRM
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj odwołania w centrum partnerskim z łącznikiem współsprzedawanym dla programu Dynamics 365 CRM. Sprzedawcy mogą następnie współsprzedawać z firmą Microsoft w ramach systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556365"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="55e3b-104">Łącznik współsprzedawanych produktów Dynamics 365 CRM — Omówienie</span><span class="sxs-lookup"><span data-stu-id="55e3b-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="55e3b-105">Odpowiednie role</span><span class="sxs-lookup"><span data-stu-id="55e3b-105">Appropriate roles</span></span>

- <span data-ttu-id="55e3b-106">Administrator odwołań</span><span class="sxs-lookup"><span data-stu-id="55e3b-106">Referrals admin</span></span>
- <span data-ttu-id="55e3b-107">Administrator systemu lub Konfigurator systemu w programie CRM</span><span class="sxs-lookup"><span data-stu-id="55e3b-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="55e3b-108">Łącznik współpracujący z centrum partnerskim umożliwia sprzedającym współsprzedaż z firmą Microsoft w ramach systemów CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="55e3b-109">Nie trzeba ich przeszkoleć w celu zarządzania pozostałymi ofertami przy użyciu Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="55e3b-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="55e3b-110">Użyj łączników współsprzedania, aby utworzyć nowe odwołanie do współsprzedaży, aby skontaktować się z sprzedawcą firmy Microsoft, otrzymywać odwołania od sprzedawcy firmy Microsoft, akceptować/odrzucać odwołania, modyfikować dane dotyczące transakcji, takie jak wartość transakcji i Data zamknięcia.</span><span class="sxs-lookup"><span data-stu-id="55e3b-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="55e3b-111">Możesz również otrzymywać wszelkie aktualizacje od sprzedawcy firmy Microsoft w ramach tych transakcji związanych z współsprzedażą.</span><span class="sxs-lookup"><span data-stu-id="55e3b-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="55e3b-112">Wszystkie odwołania można wykonać w wybranym przez siebie programie CRM, a nie w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="55e3b-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="55e3b-113">Rozwiązanie jest oparte na rozwiązaniu Microsoft energooszczędne i korzysta z interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="55e3b-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="55e3b-114">Przed zainstalowaniem — wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="55e3b-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="55e3b-115">**Tematy**</span><span class="sxs-lookup"><span data-stu-id="55e3b-115">**Topics**</span></span>   |<span data-ttu-id="55e3b-116">**Szczegóły**</span><span class="sxs-lookup"><span data-stu-id="55e3b-116">**Details**</span></span>   |<span data-ttu-id="55e3b-117">**Linki**</span><span class="sxs-lookup"><span data-stu-id="55e3b-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="55e3b-118">Identyfikator Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="55e3b-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="55e3b-119">Potrzebujesz prawidłowego identyfikatora MPN</span><span class="sxs-lookup"><span data-stu-id="55e3b-119">You need a valid MPN ID</span></span>|<span data-ttu-id="55e3b-120">Aby dołączyć [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="55e3b-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="55e3b-121">Gotowe do rozsprzedaj</span><span class="sxs-lookup"><span data-stu-id="55e3b-121">Cosell ready</span></span>|<span data-ttu-id="55e3b-122">Twoje rozwiązanie do adresów IP/usług musi być gotowe do współpracy.</span><span class="sxs-lookup"><span data-stu-id="55e3b-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="55e3b-123">Sprzedawanie z firmą Microsoft</span><span class="sxs-lookup"><span data-stu-id="55e3b-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="55e3b-124">Konto Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="55e3b-124">Partner Center account</span></span>|<span data-ttu-id="55e3b-125">IDENTYFIKATOR MPN skojarzony z dzierżawcą Centrum partnerskiego musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współsprzedażu.</span><span class="sxs-lookup"><span data-stu-id="55e3b-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="55e3b-126">Przed wdrożeniem łączników Sprawdź, czy w portalu Centrum partnerskiego są widoczne swoje odwołania do współsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="55e3b-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="55e3b-127">Zarządzanie kontem</span><span class="sxs-lookup"><span data-stu-id="55e3b-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="55e3b-128">Role użytkowników Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="55e3b-128">Partner Center user roles</span></span>|<span data-ttu-id="55e3b-129">Pracownik, który zainstaluje łączniki i korzysta z nich, musi być administratorem odwołań</span><span class="sxs-lookup"><span data-stu-id="55e3b-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="55e3b-130">Przypisywanie ról i uprawnień użytkowników</span><span class="sxs-lookup"><span data-stu-id="55e3b-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="55e3b-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="55e3b-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="55e3b-132">Rola użytkownika programu CRM to administrator systemu lub Konfigurator systemu</span><span class="sxs-lookup"><span data-stu-id="55e3b-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="55e3b-133">Przypisywanie ról w usłudze Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="55e3b-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="55e3b-134">Konto przepływu automatyzacji</span><span class="sxs-lookup"><span data-stu-id="55e3b-134">Power Automate Flow Account</span></span>|<span data-ttu-id="55e3b-135">Aktywne konto usługi [Automatyzowanie](https://flow.microsoft.com) dla administratora systemu lub konfiguratora systemu programu CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="55e3b-136">Ten użytkownik powinien zalogować się do programu w celu [automatyzacji](https://flow.microsoft.com) co najmniej raz przed instalacją.</span><span class="sxs-lookup"><span data-stu-id="55e3b-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="55e3b-137">Zainstaluj synchronizację odwołań Centrum partnerskiego dla programu Dynamics 365 (rozwiązanie do automatyzowania zarządzania)</span><span class="sxs-lookup"><span data-stu-id="55e3b-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="55e3b-138">Przejdź do pozycji [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **środowiska** w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="55e3b-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="55e3b-139">W tym kroku przedstawiono dostępne wystąpienia programu CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="55e3b-140">Wybierz odpowiednie wystąpienie programu CRM z listy rozwijanej w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="55e3b-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="55e3b-141">Wybierz pozycję **rozwiązania** na lewym pasku nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="55e3b-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="55e3b-142">Kliknij link **Otwórz AppSource** w górnym menu.</span><span class="sxs-lookup"><span data-stu-id="55e3b-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz AppSource":::

5. <span data-ttu-id="55e3b-144">Wyszukaj **Łączniki dla usługi Partner Center dla Dynamics365** na ekranie podręcznym.</span><span class="sxs-lookup"><span data-stu-id="55e3b-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="55e3b-145">Kliknij przycisk **Pobierz teraz** , a następnie **Kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="55e3b-146">Spowoduje to otwarcie strony, na której można wybrać środowisko CRM (Dynamics 365), aby zainstalować aplikację.</span><span class="sxs-lookup"><span data-stu-id="55e3b-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="55e3b-147">Zgadzam się na warunki i postanowienia.</span><span class="sxs-lookup"><span data-stu-id="55e3b-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="55e3b-148">Następnie nastąpi przekierowanie do strony **zarządzanie rozwiązaniami** .</span><span class="sxs-lookup"><span data-stu-id="55e3b-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="55e3b-149">Przejdź do pozycji "referencje do Centrum partnerskiego" przy użyciu przycisków strzałek u dołu strony.</span><span class="sxs-lookup"><span data-stu-id="55e3b-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="55e3b-150">**Zaplanowana instalacja** powinna pojawić się obok rozwiązania do tworzenia odwołań do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="55e3b-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="55e3b-151">Instalacja zajmie 10-15 minut.</span><span class="sxs-lookup"><span data-stu-id="55e3b-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="55e3b-152">Po zakończeniu instalacji przejdź z powrotem do strony [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **rozwiązania** z lewego obszaru nawigacji.</span><span class="sxs-lookup"><span data-stu-id="55e3b-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="55e3b-153">Zwróć uwagę na to, że w ramach listy rozwiązań jest dostępny komunikat **dotyczący usługi Partner Center dotyczącej synchronizacji dla usługi Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="55e3b-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="55e3b-154">Wybierz pozycję **Centrum partnerskie — synchronizacja dla programu Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="55e3b-155">Dostępne są następujące przepływy automatyzacji i jednostki:</span><span class="sxs-lookup"><span data-stu-id="55e3b-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Dostępne CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="55e3b-157">Najlepsze rozwiązanie: testowanie przed rzeczywistym użyciem</span><span class="sxs-lookup"><span data-stu-id="55e3b-157">Best practice: test before you go live</span></span>

<span data-ttu-id="55e3b-158">Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania do automatyzowania w środowisku produkcyjnym należy przetestować rozwiązanie w tymczasowym wystąpieniu programu CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="55e3b-159">Zainstaluj rozwiązanie Microsoft PowerShell automatyzuje w wystąpieniu środowiska przejściowego/programu CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="55e3b-160">Utwórz kopię rozwiązania i przeprowadź konfigurację i uruchom dostosowania przepływu w środowisku przejściowym.</span><span class="sxs-lookup"><span data-stu-id="55e3b-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="55e3b-161">Przetestuj rozwiązanie w wystąpieniu przemieszczania/programu CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="55e3b-162">W przypadku powodzenia zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.</span><span class="sxs-lookup"><span data-stu-id="55e3b-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="55e3b-163">Skonfiguruj rozwiązanie</span><span class="sxs-lookup"><span data-stu-id="55e3b-163">Configure the solution</span></span>

1. <span data-ttu-id="55e3b-164">Po zainstalowaniu rozwiązania w wystąpieniu programu CRM przejdź z powrotem do narzędzia do [automatyzacji](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="55e3b-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="55e3b-165">Z listy rozwijanej **środowiska** w prawym górnym rogu wybierz wystąpienie programu CRM, na którym zainstalowano rozwiązanie do automatyzowania.</span><span class="sxs-lookup"><span data-stu-id="55e3b-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="55e3b-166">Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:</span><span class="sxs-lookup"><span data-stu-id="55e3b-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="55e3b-167">Użytkownik Centrum partnerskiego z poświadczeniami administratora</span><span class="sxs-lookup"><span data-stu-id="55e3b-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="55e3b-168">Zdarzenia Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="55e3b-168">Partner Center Events</span></span>

   - <span data-ttu-id="55e3b-169">Administrator programu CRM z przepływem automatyzacji w rozwiązaniu.</span><span class="sxs-lookup"><span data-stu-id="55e3b-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="55e3b-170">Wybierz pozycję **połączenia** na lewym pasku nawigacyjnym i wybierz z listy rozwiązanie "referencje do Centrum partnerskiego".</span><span class="sxs-lookup"><span data-stu-id="55e3b-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="55e3b-171">Utwórz połączenie, klikając pozycję **Utwórz połączenie**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Tworzenie połączenia":::

      3. <span data-ttu-id="55e3b-173">Wyszukaj **Referencje Centrum partnerskiego (wersja zapoznawcza)** na pasku wyszukiwania w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="55e3b-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="55e3b-174">Utwórz połączenie dla użytkownika Centrum partnerskiego z rolą poświadczeń administratora.</span><span class="sxs-lookup"><span data-stu-id="55e3b-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="55e3b-175">Następnie utwórz połączenie zdarzeń Centrum partnerskiego dla użytkownika Centrum partnerskiego z poświadczeniami administratora odwołań.</span><span class="sxs-lookup"><span data-stu-id="55e3b-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="55e3b-176">Utwórz połączenie dla Common Data Service (bieżące środowisko) dla użytkownika Administrator programu CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="55e3b-177">Po dodaniu wszystkich połączeń powinny zostać wyświetlone następujące połączenia w danym środowisku:</span><span class="sxs-lookup"><span data-stu-id="55e3b-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Połączenia":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="55e3b-179">Edytuj połączenia</span><span class="sxs-lookup"><span data-stu-id="55e3b-179">Edit the connections</span></span>

1. <span data-ttu-id="55e3b-180">Wróć do strony **rozwiązania** i wybierz pozycję **domyślne rozwiązanie**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="55e3b-181">Wybierz pozycję **odwołanie do połączenia (wersja zapoznawcza)** , klikając pozycję **wszystkie**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Połącz":::

2. <span data-ttu-id="55e3b-183">Edytuj poszczególne połączenia po jednym, wybierając ikonę z trzema kropkami.</span><span class="sxs-lookup"><span data-stu-id="55e3b-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="55e3b-184">Dodaj odpowiednie połączenia.</span><span class="sxs-lookup"><span data-stu-id="55e3b-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Wymienione połączenia"::: 

3.  <span data-ttu-id="55e3b-186">Włącz przepływy w następującej kolejności:</span><span class="sxs-lookup"><span data-stu-id="55e3b-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="55e3b-187">Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="55e3b-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="55e3b-188">Utwórz odwołanie do współsprzedawcy — Dynamics 365 do Centrum partnerskiego (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="55e3b-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="55e3b-189">Centrum partnerskie — aktualizacje odwołań do oprogramowania Dynamics 365 (wersja zapoznawcza programu Preview)</span><span class="sxs-lookup"><span data-stu-id="55e3b-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="55e3b-190">Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu Preview)</span><span class="sxs-lookup"><span data-stu-id="55e3b-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="55e3b-191">Dynamics 365 do Centrum partnerskiego (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="55e3b-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="55e3b-192">Dynamics 365 — szansa do Centrum partnerskiego (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="55e3b-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="55e3b-193">Dynamics 365 — rozwiązania firmy Microsoft do Centrum partnerskiego (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="55e3b-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="55e3b-194">Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementu webhook</span><span class="sxs-lookup"><span data-stu-id="55e3b-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="55e3b-195">Interfejsy API elementu webhook Centrum partnerskiego umożliwiają rejestrację zdarzeń zmiany zasobów.</span><span class="sxs-lookup"><span data-stu-id="55e3b-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="55e3b-196">Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.</span><span class="sxs-lookup"><span data-stu-id="55e3b-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="55e3b-197">Aby zarejestrować adres URL, wybierz pozycję **rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza)** .</span><span class="sxs-lookup"><span data-stu-id="55e3b-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="55e3b-198">Dodaj połączenia dla (a) użytkownika Centrum partnerskiego z poświadczeniami administratora (b.) Centrum partnerskiego, jak zostało to wyróżnione poniżej</span><span class="sxs-lookup"><span data-stu-id="55e3b-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz":::

3. <span data-ttu-id="55e3b-200">Po wprowadzeniu tych aktualizacji zobaczysz</span><span class="sxs-lookup"><span data-stu-id="55e3b-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Elementy webhook":::

4. <span data-ttu-id="55e3b-202">Zapisz zmiany i wybierz pozycję **Włącz**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="55e3b-203">Aby włączyć elementy webhook Centrum partnerskiego do nasłuchiwania zmian w zdarzeniach, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="55e3b-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="55e3b-204">Wybierz pozycję **Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu testowego)**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="55e3b-205">Wybierz ikonę **Edytuj** i wybierz, **kiedy zostanie odebrane żądanie HTTP**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="55e3b-206">Wybierz ikonę **kopiowania** , aby skopiować podany adres URL post protokołu HTTP.</span><span class="sxs-lookup"><span data-stu-id="55e3b-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopiowanie adresu URL":::

8. <span data-ttu-id="55e3b-208">Teraz wybierz pozycję "Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)", a następnie wybierz pozycję **Uruchom**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="55e3b-209">Upewnij się, że okno "przebieg przepływu" otwiera się w okienku po prawej stronie, a następnie kliknij przycisk **Kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="55e3b-210">Wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="55e3b-210">Enter the following details:</span></span>

    1. <span data-ttu-id="55e3b-211">**Punkt końcowy wyzwalacza http**: adres URL skopiowany z wcześniejszego kroku</span><span class="sxs-lookup"><span data-stu-id="55e3b-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="55e3b-212">**Zdarzenia do zarejestrowania**: "utworzono odwołanie" i "odwołanie-zaktualizowane"</span><span class="sxs-lookup"><span data-stu-id="55e3b-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="55e3b-213">**Zastąp istniejące punkty końcowe wyzwalacza, jeśli istnieją**: tak (spowoduje to zastąpienie wszystkich istniejących punktów końcowych).</span><span class="sxs-lookup"><span data-stu-id="55e3b-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="55e3b-214">Wybierz pozycję **Uruchom** , a następnie wybierz pozycję **gotowe.**</span><span class="sxs-lookup"><span data-stu-id="55e3b-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="55e3b-215">Element webhook może teraz nasłuchiwać zdarzeń tworzenia i aktualizowania.</span><span class="sxs-lookup"><span data-stu-id="55e3b-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="55e3b-216">Dostosowywanie kroków synchronizacji</span><span class="sxs-lookup"><span data-stu-id="55e3b-216">Customize synchronization steps</span></span>

<span data-ttu-id="55e3b-217">Po zsynchronizowaniu odwołań między centrum partnerskim i systemem CRM pola, które są synchronizowane na komputerze Centrum partnerskiego, są wyświetlane w tym miejscu.</span><span class="sxs-lookup"><span data-stu-id="55e3b-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="55e3b-218">Często Systemy CRM są wysoce dostosowane.</span><span class="sxs-lookup"><span data-stu-id="55e3b-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="55e3b-219">Można dostosować przepływy automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="55e3b-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="55e3b-220">Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w krokach przepływów automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="55e3b-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="55e3b-221">Dostępne są mapowania centrów partnerskich firmy Microsoft do programu CRM, ale w oparciu o środowisko programu CRM można wybrać dalsze Dostosowywanie pól.</span><span class="sxs-lookup"><span data-stu-id="55e3b-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="55e3b-222">W zależności od potrzeb można dostosować wiele kroków poszczególnych przepływów automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="55e3b-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="55e3b-223">Poniżej przedstawiono przykłady dostępnych dostosowań:</span><span class="sxs-lookup"><span data-stu-id="55e3b-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="55e3b-224">Aby dostosować pola dla zdarzeń tworzenia lub aktualizacji w centrum partnerskim do synchronizacji odwołań CRM:</span><span class="sxs-lookup"><span data-stu-id="55e3b-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="55e3b-225">a.</span><span class="sxs-lookup"><span data-stu-id="55e3b-225">a.</span></span> <span data-ttu-id="55e3b-226">Wybierz pozycję Centrum partnerskie do usługi Dynamics 365 (wersja zapoznawcza programu testowego) lub Centrum partnerskiego w usłudze Salesforce (wersja zapoznawcza programu testowego).</span><span class="sxs-lookup"><span data-stu-id="55e3b-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="55e3b-227">b.</span><span class="sxs-lookup"><span data-stu-id="55e3b-227">b.</span></span> <span data-ttu-id="55e3b-228">Wybierz pozycję **Edytuj** , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="55e3b-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="55e3b-229">c.</span><span class="sxs-lookup"><span data-stu-id="55e3b-229">c.</span></span> <span data-ttu-id="55e3b-230">Wybierz **(zakres) zsynchronizuj potencjalnego klienta lub szansę sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="55e3b-231">Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz opcję **Jeśli jest to nowa udostępniona okazja, a następnie**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="55e3b-232">Wybierz podkrok, **Jeśli tak** , a następnie rozwiń pozycję **Tworzenie nowej szansy sprzedaży w programie CRM**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="55e3b-233">Mapowania w tej sekcji można edytować za pomocą przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="55e3b-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="55e3b-234">d.</span><span class="sxs-lookup"><span data-stu-id="55e3b-234">d.</span></span> <span data-ttu-id="55e3b-235">Aby dostosować mapowania pól programu CRM (na podstawie przewodnika po mapowaniach pól) dla zdarzeń aktualizacji, kliknij krok "(zakres) zsynchronizuj lidera lub szansę sprzedaży".</span><span class="sxs-lookup"><span data-stu-id="55e3b-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="55e3b-236">e.</span><span class="sxs-lookup"><span data-stu-id="55e3b-236">e.</span></span> <span data-ttu-id="55e3b-237">Wybierz **, czy jest to aktualizacja szansy sprzedaży, a następnie**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="55e3b-238">Wybierz podkrok, **Jeśli tak** , a następnie rozwiń **, jeśli różnica między obiektami szansy sprzedaży w centrum partnerskim i CRM**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="55e3b-239">f.</span><span class="sxs-lookup"><span data-stu-id="55e3b-239">f.</span></span> <span data-ttu-id="55e3b-240">Wybierz opcję **tak** , po której następuje **Aktualizacja istniejącej szansy sprzedaży**</span><span class="sxs-lookup"><span data-stu-id="55e3b-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="55e3b-241">Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla zdarzeń aktualizacji:</span><span class="sxs-lookup"><span data-stu-id="55e3b-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="55e3b-242">a.</span><span class="sxs-lookup"><span data-stu-id="55e3b-242">a.</span></span> <span data-ttu-id="55e3b-243">Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="55e3b-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="55e3b-244">b.</span><span class="sxs-lookup"><span data-stu-id="55e3b-244">b.</span></span> <span data-ttu-id="55e3b-245">Wybierz **(zakres) zsynchronizuj szansę sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="55e3b-246">c.</span><span class="sxs-lookup"><span data-stu-id="55e3b-246">c.</span></span> <span data-ttu-id="55e3b-247">Aby dostosować mapowania pól programu CRM dla zdarzeń aktualizacji, należy wybrać, **czy istnieje różnica między obiektami lidera w centrum partnerskim i CRM, a następnie**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="55e3b-248">d.</span><span class="sxs-lookup"><span data-stu-id="55e3b-248">d.</span></span> <span data-ttu-id="55e3b-249">Wybierz krok podrzędny, **Jeśli tak** , a następnie rozwiń krok **Aktualizuj odwołanie z danymi o szansie sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="55e3b-250">Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.</span><span class="sxs-lookup"><span data-stu-id="55e3b-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="55e3b-251">Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla tworzenia zdarzeń?</span><span class="sxs-lookup"><span data-stu-id="55e3b-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="55e3b-252">a.</span><span class="sxs-lookup"><span data-stu-id="55e3b-252">a.</span></span> <span data-ttu-id="55e3b-253">Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="55e3b-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="55e3b-254">b.</span><span class="sxs-lookup"><span data-stu-id="55e3b-254">b.</span></span> <span data-ttu-id="55e3b-255">Wybierz **(zakres) synchronizowanie odwołań.**</span><span class="sxs-lookup"><span data-stu-id="55e3b-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="55e3b-256">c.</span><span class="sxs-lookup"><span data-stu-id="55e3b-256">c.</span></span> <span data-ttu-id="55e3b-257">Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz pozycję **Utwórz odwołanie do firmy Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="55e3b-258">Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.</span><span class="sxs-lookup"><span data-stu-id="55e3b-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="55e3b-259">Istnieją dwie zmienne środowiskowe, które zostały utworzone:</span><span class="sxs-lookup"><span data-stu-id="55e3b-259">There are two environment variables created:</span></span>

- <span data-ttu-id="55e3b-260">Znacznik wyboru: oznacza, czy potrzebna jest ikona znacznika wyboru poza szansami, które są synchronizowane dwukierunkowo między centrum partnerskim i Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="55e3b-261">Synchronizuj tylko okazje do sprzedaży: oznacza to, czy chcesz synchronizować tylko okazje do sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="55e3b-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="55e3b-262">Można edytować wartość domyślną zmiennych środowiskowych.</span><span class="sxs-lookup"><span data-stu-id="55e3b-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Pole edycji dla wartości domyślnych":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="55e3b-264">Kompleksowa synchronizacja odwołań dwukierunkowych</span><span class="sxs-lookup"><span data-stu-id="55e3b-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="55e3b-265">Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania do automatyzowania gotowości można testować synchronizację odwołań między programem Dynamics 365 i centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="55e3b-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="55e3b-266">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="55e3b-266">Pre-requisites</span></span>

<span data-ttu-id="55e3b-267">Aby synchronizować odwołania w centrum partnerskim i Dynamics 365 CRM, rozwiązanie do automatyzowania, które wyraźnie określa pola odwołań specyficzne dla firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="55e3b-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="55e3b-268">Dzięki tej identyfikacji sprzedawca może określić, które odwołania mają być udostępniane firmie Microsoft w celu współsprzedaży.</span><span class="sxs-lookup"><span data-stu-id="55e3b-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="55e3b-269">Zestaw pól niestandardowych jest dostępny w ramach jednostki **szansy sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="55e3b-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="55e3b-270">Użytkownik będący administratorem programu CRM musi utworzyć osobną sekcję CRM z polami niestandardowymi **szansy sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="55e3b-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="55e3b-271">Następujące pola niestandardowe powinny być częścią sekcji CRM:</span><span class="sxs-lookup"><span data-stu-id="55e3b-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="55e3b-272">**Synchronizuj z centrum partnerskim**: czy synchronizować szansę sprzedaży z Centrum partnerskiego firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="55e3b-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="55e3b-273">**Identyfikator odwołania**: pole identyfikatora tylko do odczytu dla odwołania do Centrum partnerskiego firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="55e3b-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="55e3b-274">**Link do odwołania**: link tylko do odczytu do odwołania w centrum partnerskim firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="55e3b-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="55e3b-275">**Jak może pomóc firma Microsoft?**: pomoc wymagana przez firmę Microsoft do odwołania</span><span class="sxs-lookup"><span data-stu-id="55e3b-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="55e3b-276">**Produkty**: Lista produktów skojarzonych z tą szansą sprzedaży</span><span class="sxs-lookup"><span data-stu-id="55e3b-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="55e3b-277">**Inspekcja**: dziennik inspekcji tylko do odczytu na potrzeby synchronizacji z odwołaniami do Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="55e3b-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="55e3b-278">Aktualizowanie formularza szansa sprzedaży w programie Dynamics 365 CRM w celu uwzględnienia rozwiązań dla produktów.</span><span class="sxs-lookup"><span data-stu-id="55e3b-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formularz szansy sprzedaży":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="55e3b-281">SYTUACJI</span><span class="sxs-lookup"><span data-stu-id="55e3b-281">SCENARIOS:</span></span>

1. <span data-ttu-id="55e3b-282">Synchronizacja odwołań podczas tworzenia lub aktualizowania odwołania w programie CRM oraz synchronizowanie w centrum partnerskim:</span><span class="sxs-lookup"><span data-stu-id="55e3b-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="55e3b-283">Zaloguj się do środowiska Dynamics 365 CRM przy użyciu użytkownika, który ma wgląd w sekcję **szansa sprzedaży** w programie CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="55e3b-284">Upewnij się, że Poniższa sekcja jest obecna podczas tworzenia "nowej szansy" w środowisku Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="55e3b-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Sekcja Przykładowa okazja przedstawiająca informacje Centrum partnerskiego firmy Microsoft w usłudze Dynamics 365.":::

   3. <span data-ttu-id="55e3b-286">Aby zsynchronizować tę szansę sprzedaży z centrum partnerskim firmy Microsoft, upewnij się, że ustawisz następujące pola w widoku karty:</span><span class="sxs-lookup"><span data-stu-id="55e3b-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="55e3b-287">**Synchronizuj z centrum partnerskim**: tak</span><span class="sxs-lookup"><span data-stu-id="55e3b-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="55e3b-288">**Jak może pomóc firma Microsoft?**: Wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="55e3b-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sekcja przykładowej szansy sprzedaży w usłudze Dynamics 365, która zawiera opcje pomocy Centrum partnerskiego firmy Microsoft obok pola o nazwie jak może pomóc firma Microsoft?":::

      - <span data-ttu-id="55e3b-290">**Produkty**: identyfikatory rozwiązań produktu</span><span class="sxs-lookup"><span data-stu-id="55e3b-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="55e3b-291">Po utworzeniu szansy sprzedaży w usłudze Dynamics 365 z opcją **Synchronizuj z centrum partnerskim** ustawionym na **wartość tak**, odczekaj 10 minut, a następnie zaloguj się do konta Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="55e3b-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="55e3b-292">Twoje odwołania zostaną zsynchronizowane z usługą Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="55e3b-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="55e3b-293">Podobnie w przypadku opcji "Synchronizuj z centrum partnerskim" o wartości "tak" w przypadku zaktualizowania szansy sprzedaży w programie Dynamics 365 CRM zmiany zostaną zsynchronizowane na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="55e3b-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="55e3b-294">Prospekty, które zostały pomyślnie zsynchronizowane z centrum partnerskim, zostaną zidentyfikowane przy użyciu ikony ✔ w usłudze Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="55e3b-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="55e3b-295">Synchronizacja odwołań po utworzeniu lub zaktualizowaniu odwołania w centrum partnerskim firmy Microsoft i zsynchronizowaniu w środowisku Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="55e3b-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="55e3b-296">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="55e3b-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="55e3b-297">Wybierz **odwołania** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="55e3b-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="55e3b-298">Utwórz nowe odwołanie towarzyszące w centrum partnerskim, klikając pozycję "Nowa transakcja".</span><span class="sxs-lookup"><span data-stu-id="55e3b-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="55e3b-299">Zaloguj się do środowiska programu Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="55e3b-300">Przejdź do **okna Otwórz szanse sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="55e3b-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="55e3b-301">Odwołanie utworzone w Centrum partnerskiego firmy Microsoft jest teraz synchronizowane w programie Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="55e3b-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="55e3b-302">Po wybraniu synchronizowanego odwołania są wypełniane szczegóły widoku karty.</span><span class="sxs-lookup"><span data-stu-id="55e3b-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="55e3b-303">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="55e3b-303">Next steps</span></span>

- [<span data-ttu-id="55e3b-304">Zarządzanie potencjalnymi klientami</span><span class="sxs-lookup"><span data-stu-id="55e3b-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="55e3b-305">Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)</span><span class="sxs-lookup"><span data-stu-id="55e3b-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="55e3b-306">Więcej informacji na temat platformy Microsoft energooszczędnej?</span><span class="sxs-lookup"><span data-stu-id="55e3b-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="55e3b-307">Elementy webhook Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="55e3b-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)