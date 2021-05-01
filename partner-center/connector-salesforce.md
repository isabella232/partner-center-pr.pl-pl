---
title: Łącznik do współsprzedaży dla usługi Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj polecenia w Partner Center z crm usługi Salesforce. Sprzedawcy mogą następnie sprzedawać z firmą Microsoft z poziomu systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284387"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="f9103-104">Łącznik do współsprzedaży dla rozwiązania Salesforce CRM — omówienie</span><span class="sxs-lookup"><span data-stu-id="f9103-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="f9103-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="f9103-105">**Appropriate roles**</span></span>

- <span data-ttu-id="f9103-106">Administrator poleceń</span><span class="sxs-lookup"><span data-stu-id="f9103-106">Referrals admin</span></span>
- <span data-ttu-id="f9103-107">Administrator systemu lub customizer systemu w systemie CRM</span><span class="sxs-lookup"><span data-stu-id="f9103-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="f9103-108">Partner Center łącznika do współpracy sprzedaży umożliwia sprzedawcom sprzedawanie z firmą Microsoft z poziomu systemów CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="f9103-109">Nie trzeba ich szkolić do używania Partner Center do zarządzania transakcjami sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="f9103-110">Za pomocą łączników do współpracy sprzedaży możesz utworzyć nowe polecenie do współpracy sprzedaży, aby angażować sprzedawcę firmy Microsoft, otrzymywać polecenia od sprzedawcy firmy Microsoft, akceptować/odrzucać polecenia, modyfikować dane transakcji, takie jak wartość transakcji i data zamknięcia.</span><span class="sxs-lookup"><span data-stu-id="f9103-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="f9103-111">Możesz również otrzymywać wszelkie aktualizacje od sprzedawców firmy Microsoft dotyczące tych transakcji sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="f9103-112">Wszystkie polecenia można wykonać podczas pracy w ramach wybranego rozwiązania CRM, a nie w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f9103-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="f9103-113">Rozwiązanie jest oparte na rozwiązaniu Microsoft Power Automate Solution i używa Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="f9103-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="f9103-114">Przed zainstalowaniem — wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="f9103-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="f9103-115">**Tematy**</span><span class="sxs-lookup"><span data-stu-id="f9103-115">**Topics**</span></span>   |<span data-ttu-id="f9103-116">**Szczegóły**</span><span class="sxs-lookup"><span data-stu-id="f9103-116">**Details**</span></span>   |<span data-ttu-id="f9103-117">**Linki**</span><span class="sxs-lookup"><span data-stu-id="f9103-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="f9103-118">Microsoft Partner Network identyfikator</span><span class="sxs-lookup"><span data-stu-id="f9103-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="f9103-119">Potrzebny jest prawidłowy identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="f9103-119">You need a valid MPN ID</span></span>|<span data-ttu-id="f9103-120">Aby dołączyć [do programu MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="f9103-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="f9103-121">Gotowość do współpracy sprzedaży</span><span class="sxs-lookup"><span data-stu-id="f9103-121">Co-sell ready</span></span>|<span data-ttu-id="f9103-122">Twoje rozwiązanie ip/usług musi być gotowe do współs sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="f9103-123">Sell with Microsoft</span><span class="sxs-lookup"><span data-stu-id="f9103-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="f9103-124">Konto Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="f9103-124">Partner Center account</span></span>|<span data-ttu-id="f9103-125">Identyfikator MPN skojarzony z dzierżawą Partner Center musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współs sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="f9103-126">Przed wdrożeniem łączników sprawdź, czy polecenia dotyczące współpracy sprzedaży są Partner Center portalu.</span><span class="sxs-lookup"><span data-stu-id="f9103-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="f9103-127">Zarządzanie kontem</span><span class="sxs-lookup"><span data-stu-id="f9103-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f9103-128">Partner Center ról użytkownika</span><span class="sxs-lookup"><span data-stu-id="f9103-128">Partner Center user roles</span></span>|<span data-ttu-id="f9103-129">Pracownik, który zainstaluje łączniki i będzie z nich korzystać, musi być administratorem poleceń</span><span class="sxs-lookup"><span data-stu-id="f9103-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="f9103-130">Przypisywanie ról i uprawnień użytkowników</span><span class="sxs-lookup"><span data-stu-id="f9103-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f9103-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f9103-131">Salesforce CRM</span></span>|<span data-ttu-id="f9103-132">Rola użytkownika CRM to Administrator systemu lub Customizer systemu</span><span class="sxs-lookup"><span data-stu-id="f9103-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="f9103-133">Przypisywanie ról w programie Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f9103-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="f9103-134">Power Automate Flow Account</span><span class="sxs-lookup"><span data-stu-id="f9103-134">Power Automate Flow Account</span></span>|<span data-ttu-id="f9103-135">Aktywne konto [Power Automate](https://flow.microsoft.com) administratora systemu CRM lub customizera systemu.</span><span class="sxs-lookup"><span data-stu-id="f9103-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="f9103-136">Ten użytkownik powinien zalogować się [Power Automate](https://flow.microsoft.com) co najmniej raz przed instalacją.</span><span class="sxs-lookup"><span data-stu-id="f9103-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="f9103-137">Instalacja pakietu Salesforce dla pól niestandardowych firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="f9103-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="f9103-138">Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, rozwiązanie Power Automate musi jasno identyfikować pola poleceń specyficzne dla firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f9103-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="f9103-139">To oznaczanie daje zespołom sprzedawców partnerów możliwość decydowania o tym, które polecenia chcą udostępnić firmie Microsoft w celu współpracy sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="f9103-140">W u usługi Salesforce aktywuj pozycję **Notatki** i dodaj ją do listy powiązanych szans sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="f9103-141">Odwołanie</span><span class="sxs-lookup"><span data-stu-id="f9103-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="f9103-142">**Aktywuj zespoły szans** sprzedaży, wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="f9103-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="f9103-143">W instalatorze użyj pola **Szybkie wyszukiwanie,** aby zlokalizować ustawienia zespołu szans sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="f9103-144">Zdefiniuj ustawienia zgodnie z potrzebami.</span><span class="sxs-lookup"><span data-stu-id="f9103-144">Define the settings as needed.</span></span>
[<span data-ttu-id="f9103-145">Odwołanie</span><span class="sxs-lookup"><span data-stu-id="f9103-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="f9103-146">W uakiecie Salesforce zainstaluj niestandardowe pola i obiekty przy użyciu [instalatora pakietu](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="f9103-146">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="f9103-147">Użyj tej funkcji, aby zainstalować pakiet w dowolnej firmie.</span><span class="sxs-lookup"><span data-stu-id="f9103-147">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="f9103-148">Jeśli instalujesz w piaskownicy, musisz zastąpić początkową część adresu URL wartością http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="f9103-148">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="f9103-149">W uwitrynie Salesforce dodaj pozycję Microsoft Solutions do listy Opportunity related **(Powiązane z szansami** sprzedaży).</span><span class="sxs-lookup"><span data-stu-id="f9103-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="f9103-150">Po dodaniu wybierz **ikonę klucza** i zaktualizuj właściwości</span><span class="sxs-lookup"><span data-stu-id="f9103-150">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="f9103-151">Najlepsze rozwiązanie: Testowanie przed rozpoczęciem transmisji na żywo</span><span class="sxs-lookup"><span data-stu-id="f9103-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="f9103-152">Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania Power Automate w środowisku produkcyjnym należy przetestować rozwiązanie w przejściowym wystąpieniu crm.</span><span class="sxs-lookup"><span data-stu-id="f9103-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="f9103-153">Zainstaluj rozwiązanie Microsoft Power Automate w środowisku przejściowym/wystąpieniu crm.</span><span class="sxs-lookup"><span data-stu-id="f9103-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="f9103-154">Zrób kopię rozwiązania i uruchom konfigurację oraz Power Automate dostosowywania przepływu w środowisku przejściowym.</span><span class="sxs-lookup"><span data-stu-id="f9103-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="f9103-155">Przetestuj rozwiązanie w wystąpieniu przejściowym/CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="f9103-156">W przypadku powodzenia zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.</span><span class="sxs-lookup"><span data-stu-id="f9103-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="f9103-157">Instalowanie Partner Center poleceń usługi Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f9103-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="f9103-158">Przejdź do [Power Automate](https://flow.microsoft.com) i wybierz **pozycję Środowiska** w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="f9103-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="f9103-159">Spowoduje to pokazanie dostępnych wystąpień CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="f9103-160">Wybierz odpowiednie wystąpienie crm z listy rozwijanej w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="f9103-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="f9103-161">Wybierz **pozycję Rozwiązania** na pasku nawigacyjnym po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="f9103-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="f9103-162">Wybierz link **Open AppSource (Otwórz usługę AppSource)** w górnym menu.</span><span class="sxs-lookup"><span data-stu-id="f9103-162">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwieranie usługi AppSource":::

5. <span data-ttu-id="f9103-164">Wyszukaj Partner Center **Referrals Connectors for Salesforce** w oknie podręcznym.</span><span class="sxs-lookup"><span data-stu-id="f9103-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="f9103-166">Wybierz przycisk **Pobierz teraz, a** następnie pozycję **Kontynuuj.**</span><span class="sxs-lookup"><span data-stu-id="f9103-166">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="f9103-167">Spowoduje to otwarcie strony, na której można wybrać środowisko CRM usługi Salesforce w celu zainstalowania aplikacji.</span><span class="sxs-lookup"><span data-stu-id="f9103-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="f9103-168">Wyrażanie zgody na warunki i postanowienia.</span><span class="sxs-lookup"><span data-stu-id="f9103-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostępne rozwiązania CRMS":::

8. <span data-ttu-id="f9103-170">Następnie zostaniesz skierowany do strony **Zarządzanie rozwiązaniami.**</span><span class="sxs-lookup"><span data-stu-id="f9103-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="f9103-171">Przejdź do pozycji "Partner Center polecenia", używając przycisków strzałek w dolnej części strony.</span><span class="sxs-lookup"><span data-stu-id="f9103-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="f9103-172">**Zaplanowana instalacja** powinna pojawić się obok Partner Center polecenia.</span><span class="sxs-lookup"><span data-stu-id="f9103-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="f9103-173">Instalacja potrwa 10–15 minut.</span><span class="sxs-lookup"><span data-stu-id="f9103-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="f9103-174">Po zakończeniu instalacji wróć do strony Power Automate [i](https://flow.microsoft.com) wybierz pozycję **Rozwiązania w** obszarze nawigacji po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="f9103-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="f9103-175">Zwróć **uwagę Partner Center że synchronizacja poleceń dla usługi Salesforce** jest dostępna na liście Rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="f9103-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="f9103-176">Wybierz **Partner Center polecenia dla usługi Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="f9103-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="f9103-177">Dostępne są Power Automate przepływów i jednostek:</span><span class="sxs-lookup"><span data-stu-id="f9103-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Przepływy usługi Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="f9103-179">Konfigurowanie rozwiązania</span><span class="sxs-lookup"><span data-stu-id="f9103-179">Configure the solution</span></span>

1. <span data-ttu-id="f9103-180">Po zainstalowaniu rozwiązania w wystąpieniu crm wróć do Power Automate [.](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="f9103-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="f9103-181">Z **listy rozwijanej** Środowiska w prawym górnym rogu wybierz wystąpienie crm, w którym zainstalowano Power Automate rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="f9103-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="f9103-182">Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:</span><span class="sxs-lookup"><span data-stu-id="f9103-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="f9103-183">Partner Center z poświadczeniami administratora poleceń</span><span class="sxs-lookup"><span data-stu-id="f9103-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="f9103-184">Zdarzenia Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="f9103-184">Partner Center Events</span></span>
    - <span data-ttu-id="f9103-185">Administrator CRM z przepływami Power Automate w rozwiązaniu.</span><span class="sxs-lookup"><span data-stu-id="f9103-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="f9103-186">Wybierz **pozycję** Połączenia na pasku nawigacyjnym po lewej stronie i wybierz z listy Partner Center "Polecenia polecenia".</span><span class="sxs-lookup"><span data-stu-id="f9103-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="f9103-187">Utwórz połączenie, klikając pozycję **Utwórz połączenie.**</span><span class="sxs-lookup"><span data-stu-id="f9103-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Tworzenie połączenia":::

- <span data-ttu-id="f9103-189">Wyszukaj Partner Center polecenia (wersja zapoznawcza) na pasku wyszukiwania w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="f9103-189">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="f9103-190">Utwórz połączenie dla użytkownika Partner Center z rolą poświadczeń administratora poleceń.</span><span class="sxs-lookup"><span data-stu-id="f9103-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="f9103-191">Następnie utwórz połączenie Partner Center zdarzeń usługi Partner Center użytkownika przy użyciu poświadczeń administratora poleceń.</span><span class="sxs-lookup"><span data-stu-id="f9103-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="f9103-192">Utwórz połączenie dla usługi Salesforce dla użytkownika administratora CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="f9103-193">Po dodaniu wszystkich połączeń w środowisku powinny zostać wyświetlony następujące połączenia:</span><span class="sxs-lookup"><span data-stu-id="f9103-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Obserwowanie połączeń":::

### <a name="edit-the-connections"></a><span data-ttu-id="f9103-195">Edytowanie połączeń</span><span class="sxs-lookup"><span data-stu-id="f9103-195">Edit the connections</span></span>

1. <span data-ttu-id="f9103-196">Wróć do strony Rozwiązania i wybierz pozycję **Rozwiązanie domyślne.**</span><span class="sxs-lookup"><span data-stu-id="f9103-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="f9103-197">Wybierz **pozycję Odwołanie do połączenia (wersja zapoznawcza),** klikając pozycję **Wszystkie.**</span><span class="sxs-lookup"><span data-stu-id="f9103-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Rozpoczynanie edycji łącznika":::

2. <span data-ttu-id="f9103-199">Edytuj poszczególne połączenia, wybierając ikonę z trzema kropkami.</span><span class="sxs-lookup"><span data-stu-id="f9103-199">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="f9103-200">Dodaj odpowiednie połączenia.</span><span class="sxs-lookup"><span data-stu-id="f9103-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edytowanie łączników":::

3. <span data-ttu-id="f9103-202">Włącz przepływy w następującej kolejności:</span><span class="sxs-lookup"><span data-stu-id="f9103-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="f9103-203">Partner Center rejestracji webhook (niejawny program testów w wersji zapoznawczej)</span><span class="sxs-lookup"><span data-stu-id="f9103-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="f9103-204">Tworzenie poleceń do współpracy sprzedaży — salesforce do Partner Center (insider preview)</span><span class="sxs-lookup"><span data-stu-id="f9103-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f9103-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f9103-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f9103-206">Partner Center do usługi Salesforce (niejawny program testów w wersji zapoznawczej)</span><span class="sxs-lookup"><span data-stu-id="f9103-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f9103-207">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f9103-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f9103-208">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f9103-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f9103-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="f9103-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="f9103-210">Używanie interfejsów API elementy webhook do rejestrowania zdarzeń zmiany zasobów</span><span class="sxs-lookup"><span data-stu-id="f9103-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="f9103-211">Interfejsy API Partner Center webhook umożliwiają rejestrowanie zdarzeń zmiany zasobów.</span><span class="sxs-lookup"><span data-stu-id="f9103-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="f9103-212">Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.</span><span class="sxs-lookup"><span data-stu-id="f9103-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="f9103-213">Aby zarejestrować swój adres URL, wybierz **Partner Center webhook Registration (Insider Preview)** Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="f9103-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="f9103-214">Dodaj połączenia dla (a.) Partner Center z poświadczeniami administratora poleceń (b.) Partner Center zdarzenia, jak wyróżnione poniżej</span><span class="sxs-lookup"><span data-stu-id="f9103-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz":::

3. <span data-ttu-id="f9103-216">Po wywłaszceniom tych aktualizacji zobaczysz</span><span class="sxs-lookup"><span data-stu-id="f9103-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Elementy webhook":::

4. <span data-ttu-id="f9103-218">Zapisz zmiany i wybierz pozycję **Włącz.**</span><span class="sxs-lookup"><span data-stu-id="f9103-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="f9103-219">Aby umożliwić Partner Center webhook nasłuchiwać zmian zdarzeń, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="f9103-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="f9103-220">Wybierz **pozycję Partner Center do programu Salesforce CRM (niejawny program testów w wersji zapoznawczej).**</span><span class="sxs-lookup"><span data-stu-id="f9103-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="f9103-221">Wybierz **ikonę Edytuj** i wybierz pozycję **Po otrzymaniu żądania HTTP.**</span><span class="sxs-lookup"><span data-stu-id="f9103-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="f9103-222">Wybierz **ikonę Kopiuj,** aby skopiować podany adres URL żądania HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="f9103-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopiowanie adresu URL":::

8. <span data-ttu-id="f9103-224">Teraz wybierz przepływ "Rejestracja Partner Center webhook (niejawny program testów)" i wybierz Power Automate **Uruchom.**</span><span class="sxs-lookup"><span data-stu-id="f9103-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="f9103-225">Upewnij się, że w okienku po prawej stronie zostanie otwarte okno "Uruchom przepływ", a następnie wybierz pozycję **Kontynuuj.**</span><span class="sxs-lookup"><span data-stu-id="f9103-225">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="f9103-226">Wprowadź następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="f9103-226">Enter the following details:</span></span>

    1. <span data-ttu-id="f9103-227">**Punkt końcowy wyzwalacza HTTP:** adres URL skopiowany z wcześniejszego kroku</span><span class="sxs-lookup"><span data-stu-id="f9103-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="f9103-228">**Zdarzenia do zarejestrowania:**"utworzono polecenie" i "polecenie-zaktualizowane"</span><span class="sxs-lookup"><span data-stu-id="f9103-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="f9103-229">**Zastąp istniejące punkty końcowe wyzwalacza, jeśli są obecne:** Tak (spowoduje to zastąpienie wszystkich istniejących punktów końcowych).</span><span class="sxs-lookup"><span data-stu-id="f9103-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="f9103-230">Wybierz **pozycję Uruchom,** a następnie wybierz pozycję **Gotowe.**</span><span class="sxs-lookup"><span data-stu-id="f9103-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="f9103-231">Teraz może nasłuchiwać zdarzeń tworzenia i aktualizowania.</span><span class="sxs-lookup"><span data-stu-id="f9103-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="f9103-232">Dostosowywanie kroków synchronizacji</span><span class="sxs-lookup"><span data-stu-id="f9103-232">Customize synchronization steps</span></span>

<span data-ttu-id="f9103-233">Gdy polecenia do współpracy sprzedaży są synchronizowane między Partner Center i systemem CRM, pola, które są synchronizowane na Partner Center PC, są wymienione tutaj.</span><span class="sxs-lookup"><span data-stu-id="f9103-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="f9103-234">Często systemy CRM są wysoce dostosowane.</span><span class="sxs-lookup"><span data-stu-id="f9103-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="f9103-235">Możesz dostosować przepływy Power Automate przepływów.</span><span class="sxs-lookup"><span data-stu-id="f9103-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="f9103-236">Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wyprowadź odpowiednie zmiany w krokach Power Automate przepływów.</span><span class="sxs-lookup"><span data-stu-id="f9103-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="f9103-237">Dostępne są mapowania w centrach partnerskich firmy Microsoft na mapowania CRM, ale w zależności od środowiska CRM możesz zdecydować się na dalsze dostosowywanie pól.</span><span class="sxs-lookup"><span data-stu-id="f9103-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="f9103-238">Wiele kroków każdego z przepływów Power Automate można dostosować w zależności od potrzeb.</span><span class="sxs-lookup"><span data-stu-id="f9103-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="f9103-239">Poniżej przedstawiono przykłady dostępnych dostosowań:</span><span class="sxs-lookup"><span data-stu-id="f9103-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="f9103-240">Aby dostosować pola dla zdarzeń tworzenia lub aktualizacji w Partner Center do synchronizacji od skierowań CRM:</span><span class="sxs-lookup"><span data-stu-id="f9103-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="f9103-241">Wybierz pozycję Partner Center do programu Salesforce CRM (niejawny program testów w wersji zapoznawczej).</span><span class="sxs-lookup"><span data-stu-id="f9103-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="f9103-242">Wybierz **pozycję Edytuj,** aby edytować/dostosować Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="f9103-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="f9103-243">Wybierz **pozycję (Zakres) Synchronizuj potencjalnego klienta lub szansę sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="f9103-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="f9103-244">Aby dostosować mapowania pól CRM dla zdarzeń tworzenia, wybierz pozycję Jeśli jest to nowa udostępniona szansa **sprzedaży, a następnie pozycję**.</span><span class="sxs-lookup"><span data-stu-id="f9103-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="f9103-245">Wybierz podetap, **jeśli tak,** a następnie rozwiń **pozycję Tworzenie nowej szansy** sprzedaży w programie CRM .</span><span class="sxs-lookup"><span data-stu-id="f9103-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="f9103-246">Mapowania można edytować w tej sekcji, korzystając z przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="f9103-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="f9103-247">Aby dostosować mapowania pól CRM dla zdarzeń aktualizacji, wybierz krok "(Zakres) Synchronizowanie potencjalnego klienta lub szansy sprzedaży".</span><span class="sxs-lookup"><span data-stu-id="f9103-247">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="f9103-248">Wybierz **pozycję Jeśli jest to aktualizacja szansy sprzedaży, a następnie pozycję**.</span><span class="sxs-lookup"><span data-stu-id="f9103-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="f9103-249">Wybierz podetap, jeśli **tak, a** następnie rozwiń pozycję Jeśli różnica między obiektami szansy sprzedaży w **programie Partner Center CRM,** a następnie pozycję .</span><span class="sxs-lookup"><span data-stu-id="f9103-249">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="f9103-250">Wybierz **pozycję Jeśli tak, a** następnie zaktualizuj **istniejącą szansę sprzedaży**</span><span class="sxs-lookup"><span data-stu-id="f9103-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="f9103-251">Aby dostosować pola synchronizacji poleceń systemu CRM na komputerze dla zdarzeń aktualizacji:</span><span class="sxs-lookup"><span data-stu-id="f9103-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="f9103-252">Wybierz **pozycję Edytuj,**  aby edytować/dostosować Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="f9103-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f9103-253">Wybierz **pozycję (Zakres) Zsynchronizuj szansę sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="f9103-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="f9103-254">W przypadku dostosowywania mapowań pól CRM (na podstawie przewodnika mapowania pól) dla zdarzeń aktualizacji wybierz opcję Jeśli istnieje różnica między obiektami potencjalnych klientów w programie **Partner Center i CRM,** a następnie wybierz pozycję .</span><span class="sxs-lookup"><span data-stu-id="f9103-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="f9103-255">Wybierz krok podrzędny, **jeśli tak,** a następnie rozwiń krok Aktualizuj odwołanie **przy użyciu danych szansy sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="f9103-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="f9103-256">Mapowania można edytować w tej sekcji na podstawie przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="f9103-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="f9103-257">Aby dostosować pola dla synchronizacji poleceń crm na komputer w celu utworzenia zdarzeń?</span><span class="sxs-lookup"><span data-stu-id="f9103-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="f9103-258">Wybierz **pozycję Edytuj,**  aby edytować/dostosować Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="f9103-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f9103-259">Wybierz **pozycję (zakres) Synchronizowanie poleceń.**</span><span class="sxs-lookup"><span data-stu-id="f9103-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="f9103-260">W celu dostosowywania mapowań pól CRM (na podstawie przewodnika mapowania pól) dla zdarzeń tworzenia wybierz pozycję **Utwórz polecenie firmy Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="f9103-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="f9103-261">Mapowania można edytować w tej sekcji na podstawie przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="f9103-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="f9103-262">End-to-end bi-directional co-sell referral synchronization</span><span class="sxs-lookup"><span data-stu-id="f9103-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="f9103-263">Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania Power Automate można przetestować synchronizację poleceń współsprzedaży między usługą Salesforce CRM i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f9103-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f9103-264">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="f9103-264">Pre-requisites</span></span>

<span data-ttu-id="f9103-265">Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, Power Automate rozwiązanie musi wyraźnie rozdysmarować pola poleceń specyficzne dla firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f9103-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="f9103-266">Ta identyfikacja zapewnia zespołom sprzedawców możliwość decydowania o tym, które polecenia chcą udostępnić firmie Microsoft w celu współpracy sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f9103-267">Zestaw pól niestandardowych jest dostępny w ramach jednostki Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** (Synchronizacja poleceń dla rozwiązania CRM usługi Salesforce).</span><span class="sxs-lookup"><span data-stu-id="f9103-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="f9103-268">Administrator systemu CRM musi utworzyć oddzielną sekcję CRM z niestandardowymi polami **Szansa** sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="f9103-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="f9103-269">Następujące pola niestandardowe powinny być częścią sekcji CRM:</span><span class="sxs-lookup"><span data-stu-id="f9103-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f9103-270">**Synchronizacja z Partner Center:** czy zsynchronizować możliwość sprzedaży z usługą Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f9103-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="f9103-271">**Identyfikator polecenia:** pole identyfikatora tylko do odczytu dla poleceń Partner Center Microsoft</span><span class="sxs-lookup"><span data-stu-id="f9103-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f9103-272">**Link do poleceń:** link tylko do odczytu do polecenia w aplikacji Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="f9103-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="f9103-273">**Jak firma Microsoft może pomóc:** wymagana przez firmę Microsoft pomoc w przypadku polecenia</span><span class="sxs-lookup"><span data-stu-id="f9103-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="f9103-274">**Produkty:** lista produktów skojarzonych z tą szansą sprzedaży</span><span class="sxs-lookup"><span data-stu-id="f9103-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="f9103-275">**Inspekcja:** dziennik inspekcji tylko do odczytu do synchronizacji z Partner Center poleceniami</span><span class="sxs-lookup"><span data-stu-id="f9103-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="f9103-276">Scenariuszy:</span><span class="sxs-lookup"><span data-stu-id="f9103-276">SCENARIOS:</span></span>

1. <span data-ttu-id="f9103-277">Synchronizacja poleceń, gdy polecenia są tworzone lub aktualizowane w systemie CRM i synchronizowane w Partner Center:</span><span class="sxs-lookup"><span data-stu-id="f9103-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="f9103-278">Zaloguj się do środowiska CRM usługi Salesforce przy użyciu użytkownika, który ma wgląd w **sekcję Opportunity** (Szansa sprzedaży) w chmurze CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="f9103-279">Upewnij się, że podczas tworzenia nowej szansy sprzedaży w środowisku CRM usługi Salesforce jest obecna następująca sekcja</span><span class="sxs-lookup"><span data-stu-id="f9103-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Środowisko usługi Salesforce":::

   3. <span data-ttu-id="f9103-281">Aby zsynchronizować tę możliwość z usługą Microsoft Partner Center, należy ustawić następujące pola w widoku karty:</span><span class="sxs-lookup"><span data-stu-id="f9103-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="f9103-282">"Synchronizuj z Partner Center": Tak</span><span class="sxs-lookup"><span data-stu-id="f9103-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="f9103-283">"Jak firma Microsoft może pomóc?": Wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="f9103-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="f9103-284">Produkty: identyfikatory rozwiązań produktu</span><span class="sxs-lookup"><span data-stu-id="f9103-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="f9103-285">Po skonfigurowaniu opcji synchronizacji szansy sprzedaży  **z opcją Partner Center** tak zaczekaj 10 minut, zaloguj się do Partner Center magazynu.</span><span class="sxs-lookup"><span data-stu-id="f9103-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="f9103-286">Twoje polecenia zostaną zsynchronizowane z programem Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="f9103-287">Gdy opcja "Synchronizuj z Partner Center" jest ustawiona na wartość "Tak", jeśli zaktualizujemy możliwość w programie Salesforce CRM, zmiany zostaną zsynchronizowane z twoim Partner Center magazynu.</span><span class="sxs-lookup"><span data-stu-id="f9103-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="f9103-288">Szanse sprzedaży, które zostały pomyślnie zsynchronizowane z Partner Center, zostaną zidentyfikowane za pomocą ✔icon w programie Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="f9103-289">Synchronizacja poleceń, gdy polecenia są tworzone lub aktualizowane w programie Microsoft Partner Center i synchronizowane w środowisku CRM usługi Salesforce:</span><span class="sxs-lookup"><span data-stu-id="f9103-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="f9103-290">Zaloguj się do swojego Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="f9103-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="f9103-291">Wybierz **pozycję Polecenia** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="f9103-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="f9103-292">Utwórz nowe polecenie co-sell z Partner Center klikając opcję "Nowa transakcja".</span><span class="sxs-lookup"><span data-stu-id="f9103-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="f9103-293">Zaloguj się do środowiska CRM usługi Salesforce.</span><span class="sxs-lookup"><span data-stu-id="f9103-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="f9103-294">Przejdź do **okna Otwarte szanse sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="f9103-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="f9103-295">Polecenia utworzone w programie Microsoft Partner Center są teraz synchronizowane w programie Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f9103-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Ekran szans sprzedaży usługi Salesforce":::

    6. <span data-ttu-id="f9103-297">Po wybraniu zsynchronizowanego polecenia zostaną wypełnione szczegóły widoku karty.</span><span class="sxs-lookup"><span data-stu-id="f9103-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9103-298">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="f9103-298">Next steps</span></span>

- [<span data-ttu-id="f9103-299">Zarządzanie potencjalnymi klientami</span><span class="sxs-lookup"><span data-stu-id="f9103-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="f9103-300">Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)</span><span class="sxs-lookup"><span data-stu-id="f9103-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="f9103-301">Elementy webhook Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="f9103-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
