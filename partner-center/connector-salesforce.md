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
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276981"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="34e05-104">Łącznik do współsprzedaży dla rozwiązania Salesforce CRM — omówienie</span><span class="sxs-lookup"><span data-stu-id="34e05-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="34e05-105">**Odpowiednie role:** Administrator poleceń | Administrator systemu lub customizer systemu w systemie CRM</span><span class="sxs-lookup"><span data-stu-id="34e05-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="34e05-106">Partner Center łącznika do współpracy sprzedaży umożliwia sprzedawcom sprzedawanie z firmą Microsoft z poziomu systemów CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="34e05-107">Nie trzeba ich szkolić do używania Partner Center do zarządzania transakcjami sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="34e05-108">Za pomocą łączników do współpracy sprzedaży możesz utworzyć nowe polecenie współpracy sprzedaży, aby zaangażować sprzedawcę firmy Microsoft, otrzymać polecenia od sprzedawcy firmy Microsoft, zaakceptować/odrzucić polecenia, zmodyfikować dane transakcji, takie jak wartość transakcji i data zamknięcia.</span><span class="sxs-lookup"><span data-stu-id="34e05-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="34e05-109">Możesz również otrzymywać wszelkie aktualizacje od sprzedawców firmy Microsoft dotyczące tych transakcji sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="34e05-110">Wszystkie polecenia można wykonać podczas pracy w ramach wybranego rozwiązania CRM, a nie w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="34e05-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="34e05-111">Rozwiązanie jest oparte na rozwiązaniu Microsoft Power Automate i używa Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="34e05-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="34e05-112">Przed zainstalowaniem — wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="34e05-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="34e05-113">**Tematy**</span><span class="sxs-lookup"><span data-stu-id="34e05-113">**Topics**</span></span>   |<span data-ttu-id="34e05-114">**Szczegóły**</span><span class="sxs-lookup"><span data-stu-id="34e05-114">**Details**</span></span>   |<span data-ttu-id="34e05-115">**Linki**</span><span class="sxs-lookup"><span data-stu-id="34e05-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="34e05-116">Microsoft Partner Network identyfikator</span><span class="sxs-lookup"><span data-stu-id="34e05-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="34e05-117">Potrzebny jest prawidłowy identyfikator MPN</span><span class="sxs-lookup"><span data-stu-id="34e05-117">You need a valid MPN ID</span></span>|<span data-ttu-id="34e05-118">Aby dołączyć [do programu MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="34e05-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="34e05-119">Gotowość do współs sprzedaży</span><span class="sxs-lookup"><span data-stu-id="34e05-119">Co-sell ready</span></span>|<span data-ttu-id="34e05-120">Twoje rozwiązanie ip/usług musi być gotowe do współpracy.</span><span class="sxs-lookup"><span data-stu-id="34e05-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="34e05-121">Sell with Microsoft</span><span class="sxs-lookup"><span data-stu-id="34e05-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="34e05-122">Konto Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="34e05-122">Partner Center account</span></span>|<span data-ttu-id="34e05-123">Identyfikator MPN skojarzony z dzierżawą Partner Center musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współs sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="34e05-124">Przed wdrożeniem łączników sprawdź, czy polecenia dotyczące współpracy sprzedaży są Partner Center portalu.</span><span class="sxs-lookup"><span data-stu-id="34e05-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="34e05-125">Zarządzanie kontem</span><span class="sxs-lookup"><span data-stu-id="34e05-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="34e05-126">Partner Center ról użytkownika</span><span class="sxs-lookup"><span data-stu-id="34e05-126">Partner Center user roles</span></span>|<span data-ttu-id="34e05-127">Pracownik, który zainstaluje łączniki i użyje ich, musi być administratorem poleceń</span><span class="sxs-lookup"><span data-stu-id="34e05-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="34e05-128">Przypisywanie ról i uprawnień użytkowników</span><span class="sxs-lookup"><span data-stu-id="34e05-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="34e05-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="34e05-129">Salesforce CRM</span></span>|<span data-ttu-id="34e05-130">Rola użytkownika CRM to administrator systemu lub customizer systemu</span><span class="sxs-lookup"><span data-stu-id="34e05-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="34e05-131">Przypisywanie ról w programie Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="34e05-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="34e05-132">Power Automate Flow Account</span><span class="sxs-lookup"><span data-stu-id="34e05-132">Power Automate Flow Account</span></span>|<span data-ttu-id="34e05-133">Aktywne konto [Power Automate](https://flow.microsoft.com) administratora systemu CRM lub customizera systemu.</span><span class="sxs-lookup"><span data-stu-id="34e05-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="34e05-134">Ten użytkownik powinien zalogować się [Power Automate](https://flow.microsoft.com) co najmniej raz przed instalacją.</span><span class="sxs-lookup"><span data-stu-id="34e05-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="34e05-135">Instalacja pakietu Salesforce dla pól niestandardowych firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="34e05-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="34e05-136">Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, rozwiązanie Power Automate musi jasno identyfikować pola poleceń specyficzne dla firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34e05-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="34e05-137">To oznaczanie zapewnia zespołom sprzedawców partnerskich możliwość decydowania o tym, które polecenia mają być współużytkowania przez nich udostępnianie firmie Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34e05-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="34e05-138">W u usługi Salesforce aktywuj pozycję **Notatki** i dodaj ją do listy powiązanych szans sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="34e05-139">Odwołanie</span><span class="sxs-lookup"><span data-stu-id="34e05-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="34e05-140">**Aktywuj zespoły szans** sprzedaży, wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="34e05-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="34e05-141">W instalatorze użyj pola **Szybkie wyszukiwanie,** aby zlokalizować ustawienia zespołu szans sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="34e05-142">Zdefiniuj ustawienia zgodnie z potrzebami.</span><span class="sxs-lookup"><span data-stu-id="34e05-142">Define the settings as needed.</span></span>
[<span data-ttu-id="34e05-143">Odwołanie</span><span class="sxs-lookup"><span data-stu-id="34e05-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="34e05-144">W uakiecie Salesforce zainstaluj niestandardowe pola i obiekty przy użyciu [instalatora pakietu](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="34e05-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="34e05-145">Użyj tej funkcji, aby zainstalować pakiet w dowolnej firmie.</span><span class="sxs-lookup"><span data-stu-id="34e05-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="34e05-146">Jeśli instalujesz w piaskownicy, musisz zastąpić początkową część adresu URL wartością http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="34e05-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="34e05-147">W u usługi Salesforce dodaj rozwiązania firmy Microsoft do listy Opportunity related **(Powiązane z szansą** sprzedaży).</span><span class="sxs-lookup"><span data-stu-id="34e05-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="34e05-148">Po dodaniu wybierz **ikonę klucza** i zaktualizuj właściwości</span><span class="sxs-lookup"><span data-stu-id="34e05-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="34e05-149">Najlepsze rozwiązanie: Testowanie przed rozpoczęciem transmisji na żywo</span><span class="sxs-lookup"><span data-stu-id="34e05-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="34e05-150">Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania Power Automate w środowisku produkcyjnym należy przetestować rozwiązanie w przejściowym wystąpieniu crm.</span><span class="sxs-lookup"><span data-stu-id="34e05-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="34e05-151">Zainstaluj rozwiązanie Microsoft Power Automate w środowisku przejściowym/wystąpieniu crm.</span><span class="sxs-lookup"><span data-stu-id="34e05-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="34e05-152">Zrób kopię rozwiązania, a następnie uruchom konfigurację i Power Automate dostosowywania przepływu w środowisku przejściowym.</span><span class="sxs-lookup"><span data-stu-id="34e05-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="34e05-153">Przetestuj rozwiązanie w wystąpieniu przejściowym/CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="34e05-154">W przypadku powodzenia zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.</span><span class="sxs-lookup"><span data-stu-id="34e05-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="34e05-155">Instalowanie Partner Center poleceń usługi Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="34e05-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="34e05-156">Przejdź do [Power Automate](https://flow.microsoft.com) i wybierz **pozycję Środowiska** w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="34e05-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="34e05-157">Spowoduje to pokazanie dostępnych wystąpień CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="34e05-158">Wybierz odpowiednie wystąpienie crm z listy rozwijanej w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="34e05-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="34e05-159">Wybierz **pozycję Rozwiązania** na pasku nawigacyjnym po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="34e05-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="34e05-160">Wybierz link **Otwórz usługę AppSource** w górnym menu.</span><span class="sxs-lookup"><span data-stu-id="34e05-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz usługę AppSource.":::

5. <span data-ttu-id="34e05-162">Wyszukaj **łączniki poleceń Partner Center dla usługi Salesforce** w oknie podręcznym.</span><span class="sxs-lookup"><span data-stu-id="34e05-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. <span data-ttu-id="34e05-164">Wybierz przycisk **Pobierz teraz, a** następnie pozycję **Kontynuuj.**</span><span class="sxs-lookup"><span data-stu-id="34e05-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="34e05-165">Spowoduje to otwarcie strony, na której można wybrać środowisko CRM usługi Salesforce do zainstalowania aplikacji.</span><span class="sxs-lookup"><span data-stu-id="34e05-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="34e05-166">Wyrażanie zgody na warunki i postanowienia.</span><span class="sxs-lookup"><span data-stu-id="34e05-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Dostępne rozwiązania CRMS.":::

8. <span data-ttu-id="34e05-168">Następnie zostaniesz skierowany do strony **Zarządzanie rozwiązaniami.**</span><span class="sxs-lookup"><span data-stu-id="34e05-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="34e05-169">Przejdź do pozycji "Partner Center polecenia" przy użyciu przycisków strzałek w dolnej części strony.</span><span class="sxs-lookup"><span data-stu-id="34e05-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="34e05-170">**Instalacja zaplanowana** powinna być wyświetlana obok Partner Center polecenia.</span><span class="sxs-lookup"><span data-stu-id="34e05-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="34e05-171">Instalacja potrwa 10–15 minut.</span><span class="sxs-lookup"><span data-stu-id="34e05-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="34e05-172">Po zakończeniu instalacji wróć do strony Power Automate [i](https://flow.microsoft.com) wybierz pozycję **Rozwiązania** w obszarze nawigacji po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="34e05-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="34e05-173">Zwróć **uwagę Partner Center że synchronizacja poleceń dla usługi Salesforce** jest dostępna na liście Rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="34e05-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="34e05-174">Wybierz **Partner Center polecenia dla usługi Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="34e05-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="34e05-175">Dostępne są Power Automate przepływów i jednostek:</span><span class="sxs-lookup"><span data-stu-id="34e05-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Przepływy usługi Salesforce.":::



## <a name="configure-the-solution"></a><span data-ttu-id="34e05-177">Konfigurowanie rozwiązania</span><span class="sxs-lookup"><span data-stu-id="34e05-177">Configure the solution</span></span>

1. <span data-ttu-id="34e05-178">Po zainstalowaniu rozwiązania w wystąpieniu crm przejdź z powrotem do Power Automate [.](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="34e05-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="34e05-179">Z **listy rozwijanej** Środowiska w prawym górnym rogu wybierz wystąpienie crm, w którym zainstalowano Power Automate rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="34e05-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="34e05-180">Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:</span><span class="sxs-lookup"><span data-stu-id="34e05-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="34e05-181">Partner Center z poświadczeniami administratora poleceń</span><span class="sxs-lookup"><span data-stu-id="34e05-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="34e05-182">Zdarzenia Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="34e05-182">Partner Center Events</span></span>
    - <span data-ttu-id="34e05-183">Administrator CRM z przepływami Power Automate w rozwiązaniu.</span><span class="sxs-lookup"><span data-stu-id="34e05-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="34e05-184">Wybierz **pozycję** Połączenia na pasku nawigacyjnym po lewej stronie i wybierz rozwiązanie "Partner Center polecenia" z listy.</span><span class="sxs-lookup"><span data-stu-id="34e05-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="34e05-185">Utwórz połączenie, klikając **pozycję Utwórz połączenie.**</span><span class="sxs-lookup"><span data-stu-id="34e05-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Utwórz połączenie.":::

- <span data-ttu-id="34e05-187">Wyszukaj Partner Center poleceń (wersja zapoznawcza) na pasku wyszukiwania w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="34e05-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="34e05-188">Utwórz połączenie dla użytkownika Partner Center z rolą poświadczeń administratora poleceń.</span><span class="sxs-lookup"><span data-stu-id="34e05-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="34e05-189">Następnie utwórz połączenie Partner Center zdarzeń sieciowych dla Partner Center użytkownika przy użyciu poświadczeń administratora poleceń.</span><span class="sxs-lookup"><span data-stu-id="34e05-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="34e05-190">Utwórz połączenie dla usługi Salesforce dla użytkownika administratora CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="34e05-191">Po dodaniu wszystkich połączeń w środowisku powinny zostać wyświetlony następujące połączenia:</span><span class="sxs-lookup"><span data-stu-id="34e05-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Obserwuj połączenia.":::

### <a name="edit-the-connections"></a><span data-ttu-id="34e05-193">Edytowanie połączeń</span><span class="sxs-lookup"><span data-stu-id="34e05-193">Edit the connections</span></span>

1. <span data-ttu-id="34e05-194">Wróć do strony Rozwiązania i wybierz pozycję **Rozwiązanie domyślne.**</span><span class="sxs-lookup"><span data-stu-id="34e05-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="34e05-195">Wybierz **pozycję Odwołanie do połączenia (wersja zapoznawcza),** klikając pozycję **Wszystkie.**</span><span class="sxs-lookup"><span data-stu-id="34e05-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Rozpocznij edytowanie łącznika.":::

2. <span data-ttu-id="34e05-197">Edytuj poszczególne połączenia, wybierając ikonę z trzema kropkami.</span><span class="sxs-lookup"><span data-stu-id="34e05-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="34e05-198">Dodaj odpowiednie połączenia.</span><span class="sxs-lookup"><span data-stu-id="34e05-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edytowanie łączników.":::

3. <span data-ttu-id="34e05-200">Włącz przepływy w następującej kolejności:</span><span class="sxs-lookup"><span data-stu-id="34e05-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="34e05-201">Partner Center Webhook Registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="34e05-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="34e05-202">Tworzenie polecenia do współpracy sprzedaży — salesforce do Partner Center (niejawny program testów w wersji zapoznawczej)</span><span class="sxs-lookup"><span data-stu-id="34e05-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="34e05-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="34e05-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="34e05-204">Partner Center do usługi Salesforce (niejawny program testów w wersji zapoznawczej)</span><span class="sxs-lookup"><span data-stu-id="34e05-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="34e05-205">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="34e05-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="34e05-206">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="34e05-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="34e05-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="34e05-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="34e05-208">Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementy webhook</span><span class="sxs-lookup"><span data-stu-id="34e05-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="34e05-209">Interfejsy API Partner Center Webhook umożliwiają rejestrowanie zdarzeń zmiany zasobów.</span><span class="sxs-lookup"><span data-stu-id="34e05-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="34e05-210">Te zdarzenia zmiany są wysyłane na twój adres URL jako wpisy HTTP.</span><span class="sxs-lookup"><span data-stu-id="34e05-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="34e05-211">Aby zarejestrować swój adres URL, wybierz **Partner Center webhook Registration (Insider Preview)** Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="34e05-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="34e05-212">Dodaj połączenia dla (a.) Partner Center z poświadczeniami administratora poleceń (b.) Partner Center zdarzenia, jak wyróżnione poniżej</span><span class="sxs-lookup"><span data-stu-id="34e05-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz.":::

3. <span data-ttu-id="34e05-214">Po wdowy tych aktualizacjach zobaczysz</span><span class="sxs-lookup"><span data-stu-id="34e05-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook ( Webhook).":::

4. <span data-ttu-id="34e05-216">Zapisz zmiany i wybierz pozycję **Włącz.**</span><span class="sxs-lookup"><span data-stu-id="34e05-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="34e05-217">Aby umożliwić Partner Center webhook nasłuchiwać zmian zdarzeń, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="34e05-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="34e05-218">Wybierz **Partner Center do programu Salesforce CRM (niejawny program zapoznawczy).**</span><span class="sxs-lookup"><span data-stu-id="34e05-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="34e05-219">Wybierz **ikonę Edytuj** i wybierz pozycję **Po otrzymaniu żądania HTTP.**</span><span class="sxs-lookup"><span data-stu-id="34e05-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="34e05-220">Wybierz **ikonę Kopiuj,** aby skopiować podany adres URL żądania HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="34e05-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Skopiuj adres URL.":::

8. <span data-ttu-id="34e05-222">Teraz wybierz przepływ "Rejestracja Partner Center webhook (niejawny program testów)" i wybierz Power Automate **Uruchom.**</span><span class="sxs-lookup"><span data-stu-id="34e05-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="34e05-223">Upewnij się, że w okienku po prawej stronie zostanie otwarte okno "Uruchom przepływ", a następnie wybierz pozycję **Kontynuuj.**</span><span class="sxs-lookup"><span data-stu-id="34e05-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="34e05-224">Wprowadź następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="34e05-224">Enter the following details:</span></span>

    1. <span data-ttu-id="34e05-225">**Punkt końcowy wyzwalacza HTTP:** adres URL skopiowany z wcześniejszego kroku</span><span class="sxs-lookup"><span data-stu-id="34e05-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="34e05-226">**Zdarzenia do zarejestrowania:**"utworzono polecenie" i "polecenie-zaktualizowane"</span><span class="sxs-lookup"><span data-stu-id="34e05-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="34e05-227">**Zastąp istniejące punkty końcowe wyzwalacza, jeśli są obecne:** Tak (spowoduje to zastąpienie wszystkich istniejących punktów końcowych).</span><span class="sxs-lookup"><span data-stu-id="34e05-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="34e05-228">Wybierz **pozycję Uruchom,** a następnie wybierz pozycję **Gotowe.**</span><span class="sxs-lookup"><span data-stu-id="34e05-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="34e05-229">Teraz może nasłuchiwać zdarzeń tworzenia i aktualizowania.</span><span class="sxs-lookup"><span data-stu-id="34e05-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="34e05-230">Dostosowywanie kroków synchronizacji</span><span class="sxs-lookup"><span data-stu-id="34e05-230">Customize synchronization steps</span></span>

<span data-ttu-id="34e05-231">Gdy polecenia dotyczące współpracy sprzedaży są synchronizowane między Partner Center i systemem CRM, pola, które są synchronizowane na Partner Center PC, są wymienione tutaj.</span><span class="sxs-lookup"><span data-stu-id="34e05-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="34e05-232">Często systemy CRM są wysoce dostosowane.</span><span class="sxs-lookup"><span data-stu-id="34e05-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="34e05-233">Możesz dostosować przepływy Power Automate przepływów.</span><span class="sxs-lookup"><span data-stu-id="34e05-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="34e05-234">Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w krokach Power Automate przepływów.</span><span class="sxs-lookup"><span data-stu-id="34e05-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="34e05-235">Dostępne są mapowania rozwiązań Microsoft Partner Centers do crm, ale w zależności od środowiska CRM można dostosować pola.</span><span class="sxs-lookup"><span data-stu-id="34e05-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="34e05-236">Wiele kroków każdego z przepływów Power Automate można dostosować w zależności od potrzeb.</span><span class="sxs-lookup"><span data-stu-id="34e05-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="34e05-237">Poniżej przedstawiono przykłady dostępnych dostosowań:</span><span class="sxs-lookup"><span data-stu-id="34e05-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="34e05-238">Aby dostosować pola dla zdarzeń tworzenia lub aktualizowania w Partner Center do synchronizacji poleceń CRM:</span><span class="sxs-lookup"><span data-stu-id="34e05-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="34e05-239">Wybierz pozycję Partner Center do programu Salesforce CRM (niejawny program zapoznawczy).</span><span class="sxs-lookup"><span data-stu-id="34e05-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="34e05-240">Wybierz **pozycję Edytuj,** aby edytować/dostosować Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="34e05-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="34e05-241">Wybierz **pozycję (Zakres) Synchronizuj potencjalnego klienta lub szansę sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="34e05-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="34e05-242">Aby dostosować mapowania pól CRM dla tworzenia zdarzeń, wybierz pozycję Jeśli jest to nowa szansa sprzedaży **udostępnionej, a następnie pozycję**.</span><span class="sxs-lookup"><span data-stu-id="34e05-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="34e05-243">Wybierz krok podrzędny, **jeśli tak,** a następnie rozwiń pozycję **Tworzenie nowej szansy sprzedaży w crm**.</span><span class="sxs-lookup"><span data-stu-id="34e05-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="34e05-244">Mapowania można edytować w tej sekcji, korzystając z przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="34e05-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="34e05-245">Aby dostosować mapowania pól CRM dla zdarzeń aktualizacji, wybierz krok "(Zakres) Synchronizowanie potencjalnego klienta lub szansy sprzedaży".</span><span class="sxs-lookup"><span data-stu-id="34e05-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="34e05-246">Wybierz **pozycję Jeśli jest to aktualizacja szansy sprzedaży, a następnie .**</span><span class="sxs-lookup"><span data-stu-id="34e05-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="34e05-247">Wybierz krok podrzędny, **jeśli tak,** a następnie rozwiń pozycję Jeśli różnica między obiektami szansy sprzedaży w **programie Partner Center crm,** a następnie .</span><span class="sxs-lookup"><span data-stu-id="34e05-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="34e05-248">Wybierz **pozycję Jeśli tak, a** następnie zaktualizuj **istniejącą szansę sprzedaży**</span><span class="sxs-lookup"><span data-stu-id="34e05-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="34e05-249">Aby dostosować pola synchronizacji poleceń crm na komputer dla zdarzeń aktualizacji:</span><span class="sxs-lookup"><span data-stu-id="34e05-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="34e05-250">Wybierz **pozycję Edytuj,**  aby edytować/dostosować Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="34e05-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="34e05-251">Wybierz **pozycję (Zakres) Zsynchronizuj szansę sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="34e05-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="34e05-252">W przypadku dostosowywania mapowań pól CRM (na podstawie przewodnika mapowania pól) dla zdarzeń aktualizacji wybierz opcję Jeśli istnieje różnica między obiektami potencjalnych klientów w systemach **Partner Center i CRM,** a następnie .</span><span class="sxs-lookup"><span data-stu-id="34e05-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="34e05-253">Wybierz krok podrzędny, **jeśli tak,** a następnie rozwiń krok Aktualizuj odwołanie **przy użyciu danych szansy sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="34e05-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="34e05-254">Mapowania można edytować w tej sekcji na podstawie przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="34e05-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="34e05-255">Aby dostosować pola synchronizacji poleceń z systemu CRM do komputera w celu utworzenia zdarzeń?</span><span class="sxs-lookup"><span data-stu-id="34e05-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="34e05-256">Wybierz **pozycję Edytuj,**  aby edytować/dostosować Power Automate przepływu.</span><span class="sxs-lookup"><span data-stu-id="34e05-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="34e05-257">Wybierz **pozycję (zakres) Synchronizowanie poleceń.**</span><span class="sxs-lookup"><span data-stu-id="34e05-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="34e05-258">W celu dostosowywania mapowań pól CRM (na podstawie przewodnika mapowania pól) dla zdarzeń tworzenia wybierz pozycję **Utwórz polecenie firmy Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="34e05-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="34e05-259">Mapowania można edytować w tej sekcji na podstawie przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="34e05-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="34e05-260">End-to-end bi-directional co-sell referral synchronization</span><span class="sxs-lookup"><span data-stu-id="34e05-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="34e05-261">Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania Power Automate można przetestować synchronizację poleceń współsprzedaży między usługą Salesforce CRM i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="34e05-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="34e05-262">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="34e05-262">Pre-requisites</span></span>

<span data-ttu-id="34e05-263">Aby zsynchronizować polecenia w usługach Partner Center i Salesforce CRM, Power Automate rozwiązanie musi wyraźnie rozdysmarować pola poleceń specyficzne dla firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34e05-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="34e05-264">Ta identyfikacja zapewnia zespołom sprzedawców możliwość decydowania o tym, które polecenia chcą udostępnić firmie Microsoft w celu współpracy sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="34e05-265">Zestaw pól niestandardowych jest dostępny w ramach jednostki Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** (Synchronizacja poleceń dla rozwiązania CRM usługi Salesforce).</span><span class="sxs-lookup"><span data-stu-id="34e05-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="34e05-266">Administrator crm musi utworzyć oddzielną sekcję CRM z **niestandardowymi** polami Szansa sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="34e05-267">Następujące pola niestandardowe powinny być częścią sekcji CRM:</span><span class="sxs-lookup"><span data-stu-id="34e05-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="34e05-268">**Synchronizacja z Partner Center:** czy zsynchronizować możliwość sprzedaży z usługą Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="34e05-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="34e05-269">**Identyfikator polecenia:** pole identyfikatora tylko do odczytu dla poleceń Partner Center Microsoft</span><span class="sxs-lookup"><span data-stu-id="34e05-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="34e05-270">**Link do poleceń:** link tylko do odczytu do polecenia w aplikacji Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="34e05-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="34e05-271">**Jak firma Microsoft może pomóc:** wymagana przez firmę Microsoft pomoc w przypadku polecenia</span><span class="sxs-lookup"><span data-stu-id="34e05-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="34e05-272">**Produkty:** lista produktów skojarzonych z tą szansą sprzedaży</span><span class="sxs-lookup"><span data-stu-id="34e05-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="34e05-273">**Inspekcja:** dziennik inspekcji tylko do odczytu do synchronizacji z Partner Center poleceniami</span><span class="sxs-lookup"><span data-stu-id="34e05-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="34e05-274">Scenariuszy:</span><span class="sxs-lookup"><span data-stu-id="34e05-274">SCENARIOS:</span></span>

1. <span data-ttu-id="34e05-275">Synchronizacja poleceń, gdy polecenie jest tworzone lub aktualizowane w systemie CRM i synchronizowane w Partner Center:</span><span class="sxs-lookup"><span data-stu-id="34e05-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="34e05-276">Zaloguj się do środowiska CRM usługi Salesforce przy użyciu użytkownika, który ma wgląd w sekcję **Szansa** sprzedaży w systemie CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="34e05-277">Upewnij się, że podczas tworzenia nowej szansy sprzedaży w środowisku CRM usługi Salesforce jest obecna następująca sekcja</span><span class="sxs-lookup"><span data-stu-id="34e05-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Środowisko usługi Salesforce.":::

   3. <span data-ttu-id="34e05-279">Aby zsynchronizować tę możliwość z usługą Microsoft Partner Center, należy ustawić następujące pola w widoku karty:</span><span class="sxs-lookup"><span data-stu-id="34e05-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="34e05-280">"Synchronizuj z Partner Center": Tak</span><span class="sxs-lookup"><span data-stu-id="34e05-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="34e05-281">"Jak może pomóc firma Microsoft?": wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="34e05-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="34e05-282">Produkty: identyfikatory rozwiązań produktu</span><span class="sxs-lookup"><span data-stu-id="34e05-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="34e05-283">Po skonfigurowaniu opcji synchronizacji szansy sprzedaży  **Partner Center** na wartość **Tak,** poczekaj 10 minut, zaloguj się do Partner Center konta.</span><span class="sxs-lookup"><span data-stu-id="34e05-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="34e05-284">Twoje polecenia zostaną zsynchronizowane z programem Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="34e05-285">Gdy opcja "Synchronizuj z Partner Center" jest ustawiona na wartość "Tak", jeśli zaktualizujemy możliwość sprzedaży w programie Salesforce CRM, zmiany zostaną zsynchronizowane z kontem Partner Center sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="34e05-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="34e05-286">Szanse sprzedaży, które zostały pomyślnie zsynchronizowane z Partner Center zostaną zidentyfikowane za pomocą ✔icon w programie Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="34e05-287">Synchronizacja poleceń, gdy polecenie jest tworzone lub aktualizowane w programie Microsoft Partner Center i synchronizowane w środowisku CRM usługi Salesforce:</span><span class="sxs-lookup"><span data-stu-id="34e05-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="34e05-288">Zaloguj się do swojego Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="34e05-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="34e05-289">Wybierz **pozycję Polecenia** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="34e05-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="34e05-290">Utwórz nowe polecenie co-sell z Partner Center klikając opcję "Nowa transakcja".</span><span class="sxs-lookup"><span data-stu-id="34e05-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="34e05-291">Zaloguj się do środowiska CRM usługi Salesforce.</span><span class="sxs-lookup"><span data-stu-id="34e05-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="34e05-292">Przejdź do okna **Otwieranie szans sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="34e05-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="34e05-293">Polecenie utworzone w programie Microsoft Partner Center jest teraz synchronizowane w programie Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="34e05-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Ekran szans sprzedaży usługi Salesforce.":::

    6. <span data-ttu-id="34e05-295">Po wybraniu zsynchronizowanego polecenia zostaną wypełnione szczegóły widoku karty.</span><span class="sxs-lookup"><span data-stu-id="34e05-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="34e05-296">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="34e05-296">Next steps</span></span>

- [<span data-ttu-id="34e05-297">Zarządzanie potencjalnymi klientami</span><span class="sxs-lookup"><span data-stu-id="34e05-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="34e05-298">Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)</span><span class="sxs-lookup"><span data-stu-id="34e05-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="34e05-299">Elementy webhook Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="34e05-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
