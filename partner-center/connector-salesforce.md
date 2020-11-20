---
title: Łącznik współsprzedawanego Centrum partnerskiego usług Salesforce CRM
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj swoje odwołania w centrum partnerskim z Twoim programem Salesforce CRM. Sprzedawcy mogą następnie współsprzedawać z firmą Microsoft w ramach systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b73f0b24538daa18b93fa206fce5eda1ab9bc9b9
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947855"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="ea25c-104">Łącznik współpracujący z usługą Salesforce CRM — Omówienie</span><span class="sxs-lookup"><span data-stu-id="ea25c-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="ea25c-105">Odpowiednie role</span><span class="sxs-lookup"><span data-stu-id="ea25c-105">Appropriate roles</span></span>

- <span data-ttu-id="ea25c-106">Administrator odwołań</span><span class="sxs-lookup"><span data-stu-id="ea25c-106">Referrals admin</span></span>
- <span data-ttu-id="ea25c-107">Administrator systemu lub Konfigurator systemu w programie CRM</span><span class="sxs-lookup"><span data-stu-id="ea25c-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="ea25c-108">Łącznik współpracujący z centrum partnerskim umożliwia sprzedającym współsprzedaż z firmą Microsoft w ramach systemów CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="ea25c-109">Nie trzeba ich przeszkoleć w celu zarządzania pozostałymi ofertami przy użyciu Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ea25c-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="ea25c-110">Korzystając z łączników współsprzedających, można utworzyć nowe odwołanie do sprzedaży, aby skontaktować się z sprzedającym firmy Microsoft, otrzymać odwołania od sprzedawcy firmy Microsoft, zaakceptować/odrzucić odwołania, zmodyfikować dane dotyczące transakcji, takie jak wartość transakcji i Data zamknięcia.</span><span class="sxs-lookup"><span data-stu-id="ea25c-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="ea25c-111">Możesz również otrzymywać wszelkie aktualizacje od sprzedawcy firmy Microsoft w ramach tych transakcji związanych z współsprzedażą.</span><span class="sxs-lookup"><span data-stu-id="ea25c-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="ea25c-112">Wszystkie odwołania można wykonywać podczas pracy w wybranym programie CRM, a nie w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="ea25c-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="ea25c-113">Rozwiązanie jest oparte na rozwiązaniu Microsoft energooszczędne i korzysta z interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ea25c-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="ea25c-114">Przed zainstalowaniem — wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="ea25c-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="ea25c-115">**Tematy**</span><span class="sxs-lookup"><span data-stu-id="ea25c-115">**Topics**</span></span>   |<span data-ttu-id="ea25c-116">**Szczegóły**</span><span class="sxs-lookup"><span data-stu-id="ea25c-116">**Details**</span></span>   |<span data-ttu-id="ea25c-117">**Linki**</span><span class="sxs-lookup"><span data-stu-id="ea25c-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="ea25c-118">Identyfikator Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="ea25c-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="ea25c-119">Potrzebujesz prawidłowego identyfikatora MPN</span><span class="sxs-lookup"><span data-stu-id="ea25c-119">You need a valid MPN ID</span></span>|<span data-ttu-id="ea25c-120">Aby dołączyć [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="ea25c-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="ea25c-121">Gotowe do rozłożenia</span><span class="sxs-lookup"><span data-stu-id="ea25c-121">Co-sell ready</span></span>|<span data-ttu-id="ea25c-122">Twoje rozwiązanie do adresów IP/usług musi być gotowe do współpracy.</span><span class="sxs-lookup"><span data-stu-id="ea25c-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="ea25c-123">Sprzedawanie z firmą Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea25c-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="ea25c-124">Konto Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="ea25c-124">Partner Center account</span></span>|<span data-ttu-id="ea25c-125">IDENTYFIKATOR MPN skojarzony z dzierżawcą Centrum partnerskiego musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współsprzedażu.</span><span class="sxs-lookup"><span data-stu-id="ea25c-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="ea25c-126">Przed wdrożeniem łączników Sprawdź, czy w portalu Centrum partnerskiego są widoczne swoje odwołania do współsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="ea25c-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="ea25c-127">Zarządzanie kontem</span><span class="sxs-lookup"><span data-stu-id="ea25c-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="ea25c-128">Role użytkowników Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="ea25c-128">Partner Center user roles</span></span>|<span data-ttu-id="ea25c-129">Pracownik, który zainstaluje łączniki i korzysta z nich, musi być administratorem odwołań</span><span class="sxs-lookup"><span data-stu-id="ea25c-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="ea25c-130">Przypisywanie ról i uprawnień użytkowników</span><span class="sxs-lookup"><span data-stu-id="ea25c-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="ea25c-131">Aplikacja Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ea25c-131">Salesforce CRM</span></span>|<span data-ttu-id="ea25c-132">Rola użytkownika programu CRM to administrator systemu lub Konfigurator systemu</span><span class="sxs-lookup"><span data-stu-id="ea25c-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="ea25c-133">Przypisywanie ról w programie Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ea25c-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="ea25c-134">Konto przepływu automatyzacji</span><span class="sxs-lookup"><span data-stu-id="ea25c-134">Power Automate Flow Account</span></span>|<span data-ttu-id="ea25c-135">Aktywne konto usługi [Automatyzowanie](https://flow.microsoft.com) dla administratora systemu lub konfiguratora systemu programu CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="ea25c-136">Ten użytkownik powinien zalogować się do programu w celu [automatyzacji](https://flow.microsoft.com) co najmniej raz przed instalacją.</span><span class="sxs-lookup"><span data-stu-id="ea25c-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="ea25c-137">Instalacja pakietu Salesforce dla pól niestandardowych firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea25c-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="ea25c-138">Aby zsynchronizować odwołania w centrum partnerskim i programie Salesforce CRM, rozwiązanie do automatyzowania oprogramowania musi jasno identyfikować pola odwołań określonych przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea25c-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="ea25c-139">To rozgraniczenie zapewnia zespołom sprzedawcy partnerskiego możliwość decydowania, które odwołania chcą udostępnić firmie Microsoft w celu współsprzedaży.</span><span class="sxs-lookup"><span data-stu-id="ea25c-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="ea25c-140">W usłudze Salesforce Aktywuj **uwagi** i Dodaj je do listy powiązane szanse sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="ea25c-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="ea25c-141">Odwołanie</span><span class="sxs-lookup"><span data-stu-id="ea25c-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="ea25c-142">Aktywuj **zespoły szans sprzedaży** , wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ea25c-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="ea25c-143">W obszarze Konfiguracja Użyj pola **szybkiego wyszukiwania** , aby zlokalizować ustawienia zespołu szans sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="ea25c-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="ea25c-144">Zdefiniuj ustawienia zgodnie z wymaganiami.</span><span class="sxs-lookup"><span data-stu-id="ea25c-144">Define the settings as needed.</span></span>
[<span data-ttu-id="ea25c-145">Odwołanie</span><span class="sxs-lookup"><span data-stu-id="ea25c-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="ea25c-146">W usłudze Salesforce Zainstaluj pola niestandardowe i obiekty przy użyciu Instalatora pakietów poniżej.</span><span class="sxs-lookup"><span data-stu-id="ea25c-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="ea25c-147">Przejdź [tutaj](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) , aby zainstalować pakiet w dowolnej firmie:</span><span class="sxs-lookup"><span data-stu-id="ea25c-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="ea25c-148">Uwaga: w przypadku instalowania w piaskownicy należy zamienić początkową część adresu URL na http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="ea25c-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="ea25c-149">W usłudze Salesforce Dodaj rozwiązania firmy Microsoft do listy powiązanej z **szansą sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="ea25c-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="ea25c-150">Po dodaniu **kliknij ikonę klucza** i zaktualizuj właściwości.</span><span class="sxs-lookup"><span data-stu-id="ea25c-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="ea25c-151">Najlepsze rozwiązanie: testowanie przed rzeczywistym użyciem</span><span class="sxs-lookup"><span data-stu-id="ea25c-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="ea25c-152">Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania do automatyzowania w środowisku produkcyjnym należy przetestować rozwiązanie w tymczasowym wystąpieniu programu CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="ea25c-153">Zainstaluj rozwiązanie Microsoft PowerShell automatyzuje w wystąpieniu środowiska przejściowego/programu CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="ea25c-154">Utwórz kopię rozwiązania i przeprowadź konfigurację i uruchom dostosowania przepływu w środowisku przejściowym.</span><span class="sxs-lookup"><span data-stu-id="ea25c-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="ea25c-155">Przetestuj rozwiązanie w wystąpieniu przemieszczania/programu CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="ea25c-156">Po pomyślnym zaimportowaniu jako rozwiązania zarządzanego do wystąpienia produkcyjnego.</span><span class="sxs-lookup"><span data-stu-id="ea25c-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="ea25c-157">Zainstaluj synchronizację odwołań Centrum partnerskiego dla programu Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ea25c-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="ea25c-158">Przejdź do pozycji [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **środowiska** w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="ea25c-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="ea25c-159">Spowoduje to wyświetlenie dostępnych wystąpień programu CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="ea25c-160">Wybierz odpowiednie wystąpienie programu CRM z listy rozwijanej w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="ea25c-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="ea25c-161">Wybierz pozycję **rozwiązania** na lewym pasku nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="ea25c-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="ea25c-162">Kliknij link **Otwórz AppSource** w górnym menu.</span><span class="sxs-lookup"><span data-stu-id="ea25c-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz AppSource":::

5. <span data-ttu-id="ea25c-164">Wyszukaj **Łączniki dla Centrum partnerskiego dla usługi Salesforce** na ekranie podręcznym.</span><span class="sxs-lookup"><span data-stu-id="ea25c-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="ea25c-166">Kliknij przycisk **Pobierz teraz** , a następnie **Kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="ea25c-167">Spowoduje to otwarcie strony, na której można wybrać środowisko CRM programu Salesforce do zainstalowania aplikacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="ea25c-168">Zgadzam się na warunki i postanowienia.</span><span class="sxs-lookup"><span data-stu-id="ea25c-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostępne CRMS":::

8. <span data-ttu-id="ea25c-170">Następnie nastąpi przekierowanie do strony **zarządzanie rozwiązaniami** .</span><span class="sxs-lookup"><span data-stu-id="ea25c-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="ea25c-171">Przejdź do pozycji "referencje do Centrum partnerskiego" przy użyciu przycisków strzałek u dołu strony.</span><span class="sxs-lookup"><span data-stu-id="ea25c-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="ea25c-172">**Zaplanowana instalacja** powinna pojawić się obok rozwiązania do tworzenia odwołań do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ea25c-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="ea25c-173">Instalacja zajmie 10-15 minut.</span><span class="sxs-lookup"><span data-stu-id="ea25c-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="ea25c-174">Po zakończeniu instalacji przejdź z powrotem do strony [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **rozwiązania** z lewego obszaru nawigacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="ea25c-175">Zwróć uwagę na to, że na liście rozwiązań jest dostępna informacja **dotycząca usługi Partner Center dotyczącej synchronizacji dla usługi Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="ea25c-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="ea25c-176">Wybierz pozycję **Centrum partnerskie — synchronizacja** z usługą Salesforce.</span><span class="sxs-lookup"><span data-stu-id="ea25c-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="ea25c-177">Dostępne są następujące przepływy automatyzacji i jednostki:</span><span class="sxs-lookup"><span data-stu-id="ea25c-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Przepływy usług Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="ea25c-179">Skonfiguruj rozwiązanie</span><span class="sxs-lookup"><span data-stu-id="ea25c-179">Configure the solution</span></span>

1. <span data-ttu-id="ea25c-180">Po zainstalowaniu rozwiązania w wystąpieniu programu CRM przejdź z powrotem do narzędzia do [automatyzacji](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="ea25c-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="ea25c-181">Z listy rozwijanej **środowiska** w prawym górnym rogu wybierz wystąpienie programu CRM, na którym zainstalowano rozwiązanie do automatyzowania.</span><span class="sxs-lookup"><span data-stu-id="ea25c-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="ea25c-182">Konieczne będzie utworzenie połączeń, które kojarzą trzy konta użytkowników:</span><span class="sxs-lookup"><span data-stu-id="ea25c-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="ea25c-183">Użytkownik Centrum partnerskiego z poświadczeniami administratora</span><span class="sxs-lookup"><span data-stu-id="ea25c-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="ea25c-184">Zdarzenia Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="ea25c-184">Partner Center Events</span></span>
    - <span data-ttu-id="ea25c-185">Administrator programu CRM z przepływem automatyzacji w rozwiązaniu.</span><span class="sxs-lookup"><span data-stu-id="ea25c-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="ea25c-186">Wybierz pozycję **połączenia** na lewym pasku nawigacyjnym i wybierz z listy rozwiązanie "referencje do Centrum partnerskiego".</span><span class="sxs-lookup"><span data-stu-id="ea25c-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="ea25c-187">Utwórz połączenie, klikając pozycję **Utwórz połączenie**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Tworzenie połączenia":::

- <span data-ttu-id="ea25c-189">Wyszukaj Referencje Centrum partnerskiego (wersja zapoznawcza) na pasku wyszukiwania w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="ea25c-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="ea25c-190">Utwórz połączenie dla użytkownika Centrum partnerskiego z rolą poświadczeń administratora.</span><span class="sxs-lookup"><span data-stu-id="ea25c-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="ea25c-191">Następnie utwórz połączenie zdarzeń Centrum partnerskiego dla użytkownika Centrum partnerskiego z poświadczeniami administratora odwołań.</span><span class="sxs-lookup"><span data-stu-id="ea25c-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="ea25c-192">Utwórz połączenie usługi Salesforce dla użytkownika administratora programu CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="ea25c-193">Po dodaniu wszystkich połączeń powinny zostać wyświetlone następujące połączenia w danym środowisku:</span><span class="sxs-lookup"><span data-stu-id="ea25c-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Obserwuj połączenia":::

### <a name="edit-the-connections"></a><span data-ttu-id="ea25c-195">Edytuj połączenia</span><span class="sxs-lookup"><span data-stu-id="ea25c-195">Edit the connections</span></span>

1. <span data-ttu-id="ea25c-196">Wróć do strony rozwiązania i wybierz pozycję **domyślne rozwiązanie**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="ea25c-197">Wybierz pozycję **odwołanie do połączenia (wersja zapoznawcza)** , klikając pozycję **wszystkie**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Rozpocznij edycję łącznika":::

2. <span data-ttu-id="ea25c-199">Edytuj poszczególne połączenia po jednym, wybierając ikonę z trzema kropkami.</span><span class="sxs-lookup"><span data-stu-id="ea25c-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="ea25c-200">Dodaj odpowiednie połączenia.</span><span class="sxs-lookup"><span data-stu-id="ea25c-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edytuj łączniki":::

3. <span data-ttu-id="ea25c-202">Włącz przepływy w następującej kolejności:</span><span class="sxs-lookup"><span data-stu-id="ea25c-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="ea25c-203">Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="ea25c-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="ea25c-204">Utwórz odwołanie do towarzyszącej usługi Salesforce do Centrum partnerskiego (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="ea25c-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ea25c-205">Centrum partnerskie — aktualizacje referencyjne firmy Microsoft do usługi Salesforce (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="ea25c-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ea25c-206">Centrum partnerskie do usługi Salesforce (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="ea25c-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ea25c-207">Centrum usług Salesforce dla partnerów partnerskich (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="ea25c-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ea25c-208">Okazja do Centrum partnerskiego w usłudze Salesforce (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="ea25c-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ea25c-209">Rozwiązania firmy Microsoft do Centrum partnerskiego (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="ea25c-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="ea25c-210">Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementu webhook</span><span class="sxs-lookup"><span data-stu-id="ea25c-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="ea25c-211">Interfejsy API elementu webhook Centrum partnerskiego umożliwiają rejestrację zdarzeń zmiany zasobów.</span><span class="sxs-lookup"><span data-stu-id="ea25c-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="ea25c-212">Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.</span><span class="sxs-lookup"><span data-stu-id="ea25c-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="ea25c-213">Aby zarejestrować adres URL, wybierz pozycję **rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza)** .</span><span class="sxs-lookup"><span data-stu-id="ea25c-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="ea25c-214">Dodaj połączenia dla (a) użytkownika Centrum partnerskiego z poświadczeniami administratora (b.) Centrum partnerskiego, jak zostało to wyróżnione poniżej</span><span class="sxs-lookup"><span data-stu-id="ea25c-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz":::

3. <span data-ttu-id="ea25c-216">Po wprowadzeniu tych aktualizacji zobaczysz</span><span class="sxs-lookup"><span data-stu-id="ea25c-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Elementy webhook":::

4. <span data-ttu-id="ea25c-218">Zapisz zmiany i wybierz pozycję **Włącz**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="ea25c-219">Aby włączyć elementy webhook Centrum partnerskiego do nasłuchiwania zmian zdarzeń, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ea25c-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="ea25c-220">Wybierz pozycję **Centrum partnerskie w programie Salesforce CRM (wersja zapoznawcza programu testowego)**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="ea25c-221">Wybierz ikonę **Edytuj** i wybierz, **kiedy zostanie odebrane żądanie HTTP**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="ea25c-222">Wybierz ikonę **kopiowania** , aby skopiować podany adres URL post protokołu HTTP.</span><span class="sxs-lookup"><span data-stu-id="ea25c-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopiowanie adresu URL":::

8. <span data-ttu-id="ea25c-224">Teraz wybierz pozycję "Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)", a następnie wybierz pozycję **Uruchom**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="ea25c-225">Upewnij się, że okno "przebieg przepływu" otwiera się w okienku po prawej stronie, a następnie kliknij przycisk **Kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="ea25c-226">Wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="ea25c-226">Enter the following details:</span></span>

    1. <span data-ttu-id="ea25c-227">**Punkt końcowy wyzwalacza http**: adres URL skopiowany z wcześniejszego kroku</span><span class="sxs-lookup"><span data-stu-id="ea25c-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="ea25c-228">**Zdarzenia do zarejestrowania**: "utworzono odwołanie" i "odwołanie-zaktualizowane"</span><span class="sxs-lookup"><span data-stu-id="ea25c-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="ea25c-229">**Zastąp istniejące punkty końcowe wyzwalacza, jeśli istnieją**: tak (spowoduje to zastąpienie wszystkich istniejących punktów końcowych).</span><span class="sxs-lookup"><span data-stu-id="ea25c-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="ea25c-230">Wybierz pozycję **Uruchom** , a następnie wybierz pozycję **gotowe.**</span><span class="sxs-lookup"><span data-stu-id="ea25c-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="ea25c-231">Element webhook może teraz nasłuchiwać zdarzeń tworzenia i aktualizowania.</span><span class="sxs-lookup"><span data-stu-id="ea25c-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="ea25c-232">Dostosowywanie kroków synchronizacji</span><span class="sxs-lookup"><span data-stu-id="ea25c-232">Customize synchronization steps</span></span>

<span data-ttu-id="ea25c-233">Po zsynchronizowaniu odwołań między centrum partnerskim i systemem CRM pola, które są synchronizowane na komputerze Centrum partnerskiego, są wyświetlane w tym miejscu.</span><span class="sxs-lookup"><span data-stu-id="ea25c-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="ea25c-234">Często Systemy CRM są wysoce dostosowane.</span><span class="sxs-lookup"><span data-stu-id="ea25c-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="ea25c-235">Można dostosować przepływy automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="ea25c-236">Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w krokach przepływów automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="ea25c-237">Dostępne są mapowania centrów partnerskich firmy Microsoft do programu CRM, ale w oparciu o środowisko programu CRM można wybrać dalsze Dostosowywanie pól.</span><span class="sxs-lookup"><span data-stu-id="ea25c-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="ea25c-238">W zależności od potrzeb można dostosować wiele kroków poszczególnych przepływów automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="ea25c-239">Poniżej przedstawiono przykłady dostępnych dostosowań:</span><span class="sxs-lookup"><span data-stu-id="ea25c-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="ea25c-240">Aby dostosować pola dla zdarzeń tworzenia lub aktualizacji w centrum partnerskim do synchronizacji odwołań CRM:</span><span class="sxs-lookup"><span data-stu-id="ea25c-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="ea25c-241">Wybierz pozycję Centrum partnerskie w programie Salesforce CRM (wersja zapoznawcza programu testowego).</span><span class="sxs-lookup"><span data-stu-id="ea25c-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="ea25c-242">Wybierz pozycję **Edytuj** , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="ea25c-243">Wybierz **(zakres) zsynchronizuj potencjalnego klienta lub szansę sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="ea25c-244">Aby dostosować mapowania pól programu CRM dla zdarzeń tworzenia, wybierz opcję **Jeśli jest to nowa udostępniona okazja, a następnie**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="ea25c-245">Wybierz podkrok, **Jeśli tak** , a następnie rozwiń pozycję **Tworzenie nowej szansy sprzedaży w programie CRM**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="ea25c-246">Mapowania w tej sekcji można edytować za pomocą przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="ea25c-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="ea25c-247">Aby dostosować mapowania pól programu CRM dla zdarzeń aktualizacji, kliknij krok "(zakres) zsynchronizuj potencjalny klient lub szansę".</span><span class="sxs-lookup"><span data-stu-id="ea25c-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="ea25c-248">Wybierz **, czy jest to aktualizacja szansy sprzedaży, a następnie**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="ea25c-249">Wybierz podkrok, **Jeśli tak** , a następnie rozwiń **, jeśli różnica między obiektami szansy sprzedaży w centrum partnerskim i CRM**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="ea25c-250">Wybierz opcję **tak** , po której następuje **Aktualizacja istniejącej szansy sprzedaży**</span><span class="sxs-lookup"><span data-stu-id="ea25c-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="ea25c-251">Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla zdarzeń aktualizacji:</span><span class="sxs-lookup"><span data-stu-id="ea25c-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="ea25c-252">Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ea25c-253">Wybierz **(zakres) zsynchronizuj szansę sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="ea25c-254">Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń aktualizacji, należy wybrać, **czy istnieje różnica między obiektami lidera w centrum partnerskim i CRM, a następnie**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="ea25c-255">Wybierz krok podrzędny, **Jeśli tak** , a następnie rozwiń krok **Aktualizuj odwołanie z danymi o szansie sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="ea25c-256">Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.</span><span class="sxs-lookup"><span data-stu-id="ea25c-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="ea25c-257">Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla tworzenia zdarzeń?</span><span class="sxs-lookup"><span data-stu-id="ea25c-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="ea25c-258">Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="ea25c-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ea25c-259">Wybierz **(zakres) synchronizowanie odwołań.**</span><span class="sxs-lookup"><span data-stu-id="ea25c-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="ea25c-260">Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz pozycję **Utwórz odwołanie do firmy Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="ea25c-261">Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.</span><span class="sxs-lookup"><span data-stu-id="ea25c-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="ea25c-262">Kompleksowa synchronizacja odwołań dwukierunkowych</span><span class="sxs-lookup"><span data-stu-id="ea25c-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="ea25c-263">Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania do automatyzowania gotowości można testować synchronizację odwołań między programem Salesforce CRM a centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="ea25c-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="ea25c-264">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="ea25c-264">Pre-requisites</span></span>

<span data-ttu-id="ea25c-265">Aby zsynchronizować odwołania w centrum partnerskim i programie Salesforce CRM, rozwiązanie do automatyzowania oprogramowania musi wyraźnie oddzielić pola referencyjne specyficzne dla firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea25c-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="ea25c-266">Ta identyfikacja zapewnia zespołom sprzedawcy możliwość decydowania, które odwołania chcą udostępnić firmie Microsoft w celu współsprzedaży.</span><span class="sxs-lookup"><span data-stu-id="ea25c-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="ea25c-267">Zestaw pól niestandardowych jest dostępny w ramach synchronizacji odwołań Centrum partnerskiego dla jednostki **szansy sprzedaży** rozwiązania w usłudze Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="ea25c-268">Użytkownik będący administratorem programu CRM musi utworzyć osobną sekcję CRM z polami niestandardowymi **szansy sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="ea25c-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="ea25c-269">Następujące pola niestandardowe powinny być częścią sekcji CRM:</span><span class="sxs-lookup"><span data-stu-id="ea25c-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="ea25c-270">**Synchronizuj z centrum partnerskim**: czy synchronizować szansę sprzedaży z Centrum partnerskiego firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea25c-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="ea25c-271">**Identyfikator odwołania**: pole identyfikatora tylko do odczytu dla odwołania do Centrum partnerskiego firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea25c-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="ea25c-272">**Link do odwołania**: link tylko do odczytu do odwołania w centrum partnerskim firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea25c-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="ea25c-273">**Jak może pomóc firma Microsoft**: pomoc wymagana przez firmę Microsoft do odwołania</span><span class="sxs-lookup"><span data-stu-id="ea25c-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="ea25c-274">**Produkty**: Lista produktów skojarzonych z tą szansą sprzedaży</span><span class="sxs-lookup"><span data-stu-id="ea25c-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="ea25c-275">**Inspekcja**: dziennik inspekcji tylko do odczytu na potrzeby synchronizacji z odwołaniami do Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="ea25c-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="ea25c-276">SYTUACJI</span><span class="sxs-lookup"><span data-stu-id="ea25c-276">SCENARIOS:</span></span>

1. <span data-ttu-id="ea25c-277">Synchronizacja odwołań podczas tworzenia lub aktualizowania odwołania w programie CRM oraz synchronizowanie w centrum partnerskim:</span><span class="sxs-lookup"><span data-stu-id="ea25c-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="ea25c-278">Zaloguj się do środowiska usługi Salesforce CRM przy użyciu użytkownika, który ma widoczność w sekcji **szansa sprzedaży** w programie CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="ea25c-279">Upewnij się, że Poniższa sekcja jest obecna podczas tworzenia nowej szansy sprzedaży w środowisku programu Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ea25c-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Środowisko Salesforce":::

   3. <span data-ttu-id="ea25c-281">Aby zsynchronizować tę szansę sprzedaży z centrum partnerskim firmy Microsoft, upewnij się, że ustawisz następujące pola w widoku karty:</span><span class="sxs-lookup"><span data-stu-id="ea25c-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="ea25c-282">"Synchronizuj z centrum partnerskim": tak</span><span class="sxs-lookup"><span data-stu-id="ea25c-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="ea25c-283">"Jak mogę pomóc firmie Microsoft?": Wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="ea25c-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="ea25c-284">Produkty: identyfikatory rozwiązań produktu</span><span class="sxs-lookup"><span data-stu-id="ea25c-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="ea25c-285">Po ustawieniu opcji  **Synchronizuj z centrum partnerskim** na **wartość tak**, odczekaj 10 minut, zaloguj się na swoim koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ea25c-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="ea25c-286">Twoje odwołania zostaną zsynchronizowane z programem Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="ea25c-287">Jeśli opcja "Synchronizuj z centrum partnerskim" jest ustawiona na wartość "tak", po zaktualizowaniu szansy sprzedaży w programie Salesforce CRM zmiany zostaną zsynchronizowane z kontem Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ea25c-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="ea25c-288">Pomyślnie zsynchronizowane szanse sprzedaży z Centrum partnerskiego zostaną oznaczone ikoną ✔ w programie Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="ea25c-289">Synchronizacja odwołań po utworzeniu lub zaktualizowaniu odwołania w centrum partnerskim firmy Microsoft i zsynchronizowaniu w środowisku usługi Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="ea25c-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="ea25c-290">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ea25c-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="ea25c-291">Wybierz **odwołania** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="ea25c-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="ea25c-292">Utwórz nowe odwołanie towarzyszące w centrum partnerskim, klikając pozycję "Nowa transakcja".</span><span class="sxs-lookup"><span data-stu-id="ea25c-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="ea25c-293">Zaloguj się do środowiska usługi Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="ea25c-294">Przejdź do **okna Otwórz szanse sprzedaży**.</span><span class="sxs-lookup"><span data-stu-id="ea25c-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="ea25c-295">Odwołanie utworzone w Centrum partnerskiego firmy Microsoft jest teraz synchronizowane w programie Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ea25c-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Ekran możliwości usługi Salesforce":::

    6. <span data-ttu-id="ea25c-297">Po wybraniu synchronizowanego odwołania są wypełniane szczegóły widoku karty.</span><span class="sxs-lookup"><span data-stu-id="ea25c-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ea25c-298">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="ea25c-298">Next steps</span></span>

- [<span data-ttu-id="ea25c-299">Zarządzanie potencjalnymi klientami</span><span class="sxs-lookup"><span data-stu-id="ea25c-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="ea25c-300">Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)</span><span class="sxs-lookup"><span data-stu-id="ea25c-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="ea25c-301">Elementy webhook Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="ea25c-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
