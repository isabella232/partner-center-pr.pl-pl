---
title: Łącznik współsprzedającego dla Centrum partnerskiego programu Dynamics 365 CRM
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zsynchronizuj swoje odwołania w centrum partnerskim z łącznikiem do współsprzedażu dla programu Dynamics 365 CRM. Sprzedawcy mogą następnie współsprzedawać z firmą Microsoft w ramach systemów CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8ea803e675ce7c2d21d680491bbdaedf792e631f
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530315"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="9dbdf-104">Łącznik współsprzedawanych produktów Dynamics 365 CRM — Omówienie</span><span class="sxs-lookup"><span data-stu-id="9dbdf-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="9dbdf-105">Odpowiednie role</span><span class="sxs-lookup"><span data-stu-id="9dbdf-105">Appropriate roles</span></span>

- <span data-ttu-id="9dbdf-106">Administrator odwołań</span><span class="sxs-lookup"><span data-stu-id="9dbdf-106">Referrals admin</span></span>
- <span data-ttu-id="9dbdf-107">Administrator systemu lub Konfigurator systemu w programie CRM</span><span class="sxs-lookup"><span data-stu-id="9dbdf-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="9dbdf-108">Łącznik współpracujący z centrum partnerskim umożliwia sprzedającym współsprzedaż z firmą Microsoft w ramach systemów CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="9dbdf-109">Nie trzeba ich przeszkoleć w celu zarządzania pozostałymi ofertami przy użyciu Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="9dbdf-110">Użyj łączników współsprzedania, aby utworzyć nowe odwołanie do współsprzedaży, aby skontaktować się z sprzedawcą firmy Microsoft, otrzymywać odwołania od sprzedawcy firmy Microsoft, akceptować/odrzucać odwołania, modyfikować dane dotyczące transakcji, takie jak wartość transakcji i Data zamknięcia.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="9dbdf-111">Możesz również otrzymywać wszelkie aktualizacje od sprzedawcy firmy Microsoft w ramach tych transakcji związanych z współsprzedażą.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="9dbdf-112">Wszystkie odwołania można wykonać w wybranym przez siebie programie CRM, a nie w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="9dbdf-113">Rozwiązanie jest oparte na rozwiązaniu Microsoft energooszczędne i korzysta z interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="9dbdf-114">Przed zainstalowaniem — wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="9dbdf-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="9dbdf-115">**Tematy**</span><span class="sxs-lookup"><span data-stu-id="9dbdf-115">**Topics**</span></span>   |<span data-ttu-id="9dbdf-116">**Szczegóły**</span><span class="sxs-lookup"><span data-stu-id="9dbdf-116">**Details**</span></span>   |<span data-ttu-id="9dbdf-117">**Linki**</span><span class="sxs-lookup"><span data-stu-id="9dbdf-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="9dbdf-118">Identyfikator Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="9dbdf-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="9dbdf-119">Potrzebujesz prawidłowego identyfikatora MPN</span><span class="sxs-lookup"><span data-stu-id="9dbdf-119">You need a valid MPN ID</span></span>|<span data-ttu-id="9dbdf-120">Aby dołączyć [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="9dbdf-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="9dbdf-121">Gotowe do rozsprzedaj</span><span class="sxs-lookup"><span data-stu-id="9dbdf-121">Cosell ready</span></span>|<span data-ttu-id="9dbdf-122">Twoje rozwiązanie do adresów IP/usług musi być gotowe do współpracy.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="9dbdf-123">Sprzedawanie z firmą Microsoft</span><span class="sxs-lookup"><span data-stu-id="9dbdf-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="9dbdf-124">Konto Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="9dbdf-124">Partner Center account</span></span>|<span data-ttu-id="9dbdf-125">IDENTYFIKATOR MPN skojarzony z dzierżawcą Centrum partnerskiego musi być taki sam jak identyfikator MPN skojarzony z rozwiązaniem do współsprzedażu.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="9dbdf-126">Przed wdrożeniem łączników Sprawdź, czy w portalu Centrum partnerskiego są widoczne swoje odwołania do współsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="9dbdf-127">Zarządzanie kontem</span><span class="sxs-lookup"><span data-stu-id="9dbdf-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="9dbdf-128">Role użytkowników Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="9dbdf-128">Partner Center user roles</span></span>|<span data-ttu-id="9dbdf-129">Pracownik, który zainstaluje łączniki i korzysta z nich, musi być administratorem odwołań</span><span class="sxs-lookup"><span data-stu-id="9dbdf-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="9dbdf-130">Przypisywanie ról i uprawnień użytkowników</span><span class="sxs-lookup"><span data-stu-id="9dbdf-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="9dbdf-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="9dbdf-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="9dbdf-132">Rola użytkownika programu CRM to administrator systemu lub Konfigurator systemu</span><span class="sxs-lookup"><span data-stu-id="9dbdf-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="9dbdf-133">Przypisywanie ról w usłudze Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9dbdf-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="9dbdf-134">Konto przepływu automatyzacji</span><span class="sxs-lookup"><span data-stu-id="9dbdf-134">Power Automate Flow Account</span></span>|<span data-ttu-id="9dbdf-135">Aktywne konto usługi [Automatyzowanie](https://flow.microsoft.com) dla administratora systemu lub konfiguratora systemu programu CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="9dbdf-136">Ten użytkownik powinien zalogować się do programu w celu [automatyzacji](https://flow.microsoft.com) co najmniej raz przed instalacją.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="9dbdf-137">Zainstaluj synchronizację odwołań Centrum partnerskiego dla programu Dynamics 365 (rozwiązanie do automatyzowania zarządzania)</span><span class="sxs-lookup"><span data-stu-id="9dbdf-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="9dbdf-138">Przejdź do pozycji [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **środowiska** w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="9dbdf-139">W tym kroku przedstawiono dostępne wystąpienia programu CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="9dbdf-140">Wybierz odpowiednie wystąpienie programu CRM z listy rozwijanej w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="9dbdf-141">Wybierz pozycję **rozwiązania** na lewym pasku nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="9dbdf-142">Kliknij link **Otwórz AppSource** w górnym menu.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Otwórz AppSource":::

5. <span data-ttu-id="9dbdf-144">Wyszukaj **Łączniki dla usługi Partner Center dla Dynamics365** na ekranie podręcznym.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="9dbdf-145">Kliknij przycisk **Pobierz teraz** , a następnie **Kontynuuj** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-145">Click the **Get it now** button and then **Continue** .</span></span>

7. <span data-ttu-id="9dbdf-146">Spowoduje to otwarcie strony, na której można wybrać środowisko CRM (Dynamics 365), aby zainstalować aplikację.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="9dbdf-147">Zgadzam się na warunki i postanowienia.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="9dbdf-148">Następnie nastąpi przekierowanie do strony **zarządzanie rozwiązaniami** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="9dbdf-149">Przejdź do pozycji "referencje do Centrum partnerskiego" przy użyciu przycisków strzałek u dołu strony.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="9dbdf-150">**Zaplanowana instalacja** powinna pojawić się obok rozwiązania do tworzenia odwołań do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="9dbdf-151">Instalacja zajmie 10-15 minut.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="9dbdf-152">Po zakończeniu instalacji przejdź z powrotem do strony [Automatyzacja](https://flow.microsoft.com) i wybierz pozycję **rozwiązania** z lewego obszaru nawigacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="9dbdf-153">Zwróć uwagę na to, że w ramach listy rozwiązań jest dostępny komunikat **dotyczący usługi Partner Center dotyczącej synchronizacji dla usługi Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="9dbdf-154">Wybierz pozycję **Centrum partnerskie — synchronizacja dla programu Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-154">Select **Partner Center Referrals Synchronization for Dynamics 365** .</span></span> <span data-ttu-id="9dbdf-155">Dostępne są następujące przepływy automatyzacji i jednostki:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Dostępne CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="9dbdf-157">Najlepsze rozwiązanie: testowanie przed rzeczywistym użyciem</span><span class="sxs-lookup"><span data-stu-id="9dbdf-157">Best practice: test before you go live</span></span>

<span data-ttu-id="9dbdf-158">Przed zainstalowaniem, skonfigurowaniem i dostosowaniem rozwiązania do automatyzowania w środowisku produkcyjnym należy przetestować rozwiązanie w tymczasowym wystąpieniu programu CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="9dbdf-159">Zainstaluj rozwiązanie Microsoft PowerShell automatyzuje w wystąpieniu środowiska przejściowego/programu CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="9dbdf-160">Utwórz kopię rozwiązania i przeprowadź konfigurację i uruchom dostosowania przepływu w środowisku przejściowym.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="9dbdf-161">Przetestuj rozwiązanie w wystąpieniu przemieszczania/programu CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="9dbdf-162">W przypadku powodzenia zaimportuj jako rozwiązanie zarządzane do wystąpienia produkcyjnego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="9dbdf-163">Skonfiguruj rozwiązanie</span><span class="sxs-lookup"><span data-stu-id="9dbdf-163">Configure the solution</span></span>

1. <span data-ttu-id="9dbdf-164">Po zainstalowaniu rozwiązania w wystąpieniu programu CRM przejdź z powrotem do narzędzia do [automatyzacji](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="9dbdf-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="9dbdf-165">Z listy rozwijanej **środowiska** w prawym górnym rogu wybierz wystąpienie programu CRM, na którym zainstalowano rozwiązanie do automatyzowania.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="9dbdf-166">Należy utworzyć połączenia, które kojarzą trzy konta użytkowników:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="9dbdf-167">Użytkownik Centrum partnerskiego z poświadczeniami administratora</span><span class="sxs-lookup"><span data-stu-id="9dbdf-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="9dbdf-168">Zdarzenia Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="9dbdf-168">Partner Center Events</span></span>

   - <span data-ttu-id="9dbdf-169">Administrator programu CRM z przepływem automatyzacji w rozwiązaniu.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="9dbdf-170">Wybierz pozycję **połączenia** na lewym pasku nawigacyjnym i wybierz z listy rozwiązanie "referencje do Centrum partnerskiego".</span><span class="sxs-lookup"><span data-stu-id="9dbdf-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="9dbdf-171">Utwórz połączenie, klikając pozycję **Utwórz połączenie** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-171">Create a connection by clicking **Create a connection** .</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Tworzenie połączenia":::

      3. <span data-ttu-id="9dbdf-173">Wyszukaj **Referencje Centrum partnerskiego (wersja zapoznawcza)** na pasku wyszukiwania w prawym górnym rogu.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="9dbdf-174">Utwórz połączenie dla użytkownika Centrum partnerskiego z rolą poświadczeń administratora.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="9dbdf-175">Następnie utwórz połączenie zdarzeń Centrum partnerskiego dla użytkownika Centrum partnerskiego z poświadczeniami administratora odwołań.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="9dbdf-176">Utwórz połączenie dla Common Data Service (bieżące środowisko) dla użytkownika Administrator programu CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="9dbdf-177">Aby skojarzyć automatyczne przepływy z połączeniami, należy edytować wszystkie przepływy automatyzacji, aby połączyć się z odwołaniami Common Data Service i Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-177">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="9dbdf-178">Zapisz zmiany.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-178">Save the changes.</span></span>

5. <span data-ttu-id="9dbdf-179">**Włącz** przepływy automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-179">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="9dbdf-180">Rejestrowanie zdarzeń zmiany zasobów przy użyciu interfejsów API elementu webhook</span><span class="sxs-lookup"><span data-stu-id="9dbdf-180">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="9dbdf-181">Interfejsy API elementu webhook Centrum partnerskiego umożliwiają rejestrację zdarzeń zmiany zasobów.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-181">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="9dbdf-182">Te zdarzenia zmiany są wysyłane na adres URL jako wpisy HTTP.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-182">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="9dbdf-183">Aby zarejestrować adres URL, wybierz pozycję **rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza)** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-183">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="9dbdf-184">Dodaj połączenia dla (a) użytkownika Centrum partnerskiego z poświadczeniami administratora (b.) Centrum partnerskiego, jak zostało to wyróżnione poniżej</span><span class="sxs-lookup"><span data-stu-id="9dbdf-184">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Wyzwalacz":::

3. <span data-ttu-id="9dbdf-186">Po wprowadzeniu tych aktualizacji zobaczysz</span><span class="sxs-lookup"><span data-stu-id="9dbdf-186">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Elementy webhook":::

4. <span data-ttu-id="9dbdf-188">Zapisz zmiany i wybierz pozycję **Włącz** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-188">Save your changes and select **Turn on** .</span></span>

   <span data-ttu-id="9dbdf-189">Aby włączyć elementy webhook Centrum partnerskiego do nasłuchiwania zmian w zdarzeniach, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-189">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="9dbdf-190">Wybierz pozycję **Centrum partnerskie do systemu Dynamics 365 (wersja zapoznawcza programu testowego)** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-190">Select **Partner Center to Dynamics 365 (Insider Preview)** .</span></span>

6. <span data-ttu-id="9dbdf-191">Wybierz ikonę **Edytuj** i wybierz, **kiedy zostanie odebrane żądanie HTTP** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-191">Select the **Edit** icon and select **When a HTTP request is received** .</span></span>

7. <span data-ttu-id="9dbdf-192">Wybierz ikonę **kopiowania** , aby skopiować podany adres URL post protokołu HTTP.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-192">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopiowanie adresu URL":::

8. <span data-ttu-id="9dbdf-194">Teraz wybierz pozycję "Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)", a następnie wybierz pozycję **Uruchom** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-194">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run** .</span></span>

9. <span data-ttu-id="9dbdf-195">Upewnij się, że okno "przebieg przepływu" otwiera się w okienku po prawej stronie, a następnie kliknij przycisk **Kontynuuj** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-195">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue** .</span></span>

10. <span data-ttu-id="9dbdf-196">Wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-196">Enter the following details:</span></span>

    1. <span data-ttu-id="9dbdf-197">**Punkt końcowy wyzwalacza http** : adres URL skopiowany z wcześniejszego kroku</span><span class="sxs-lookup"><span data-stu-id="9dbdf-197">**Http Trigger Endpoint** : URL copied from earlier step</span></span>

    2. <span data-ttu-id="9dbdf-198">**Zdarzenia do zarejestrowania** : "utworzono odwołanie" i "odwołanie-zaktualizowane"</span><span class="sxs-lookup"><span data-stu-id="9dbdf-198">**Events to Register** : “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="9dbdf-199">**Zastąp istniejące punkty końcowe wyzwalacza, jeśli istnieją** : tak (spowoduje to zastąpienie wszystkich istniejących punktów końcowych).</span><span class="sxs-lookup"><span data-stu-id="9dbdf-199">**Overwrite existing trigger endpoints if present** : Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="9dbdf-200">Wybierz pozycję **Uruchom** , a następnie wybierz pozycję **gotowe.**</span><span class="sxs-lookup"><span data-stu-id="9dbdf-200">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="9dbdf-201">Element webhook może teraz nasłuchiwać zdarzeń tworzenia i aktualizowania.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-201">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="9dbdf-202">Dostosowywanie kroków synchronizacji</span><span class="sxs-lookup"><span data-stu-id="9dbdf-202">Customize synchronization steps</span></span>

<span data-ttu-id="9dbdf-203">Po zsynchronizowaniu odwołań między centrum partnerskim i systemem CRM pola, które są synchronizowane na komputerze Centrum partnerskiego, są wyświetlane w tym miejscu.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-203">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="9dbdf-204">Często Systemy CRM są wysoce dostosowane.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-204">Often CRM systems are highly customized.</span></span> <span data-ttu-id="9dbdf-205">Można dostosować przepływy automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-205">You can customize the Power Automate flows.</span></span> <span data-ttu-id="9dbdf-206">Postępuj zgodnie z przewodnikiem mapowania pól i w razie potrzeby wprowadź odpowiednie zmiany w krokach przepływów automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-206">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="9dbdf-207">Dostępne są mapowania centrów partnerskich firmy Microsoft do programu CRM, ale w oparciu o środowisko programu CRM można wybrać dalsze Dostosowywanie pól.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-207">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="9dbdf-208">W zależności od potrzeb można dostosować wiele kroków poszczególnych przepływów automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-208">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="9dbdf-209">Poniżej przedstawiono przykłady dostępnych dostosowań:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-209">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="9dbdf-210">Aby dostosować pola dla zdarzeń tworzenia lub aktualizacji w centrum partnerskim do synchronizacji odwołań CRM:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-210">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="9dbdf-211">a.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-211">a.</span></span> <span data-ttu-id="9dbdf-212">Wybierz pozycję Centrum partnerskie do usługi Dynamics 365 (wersja zapoznawcza programu testowego) lub Centrum partnerskiego w usłudze Salesforce (wersja zapoznawcza programu testowego).</span><span class="sxs-lookup"><span data-stu-id="9dbdf-212">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="9dbdf-213">b.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-213">b.</span></span> <span data-ttu-id="9dbdf-214">Wybierz pozycję **Edytuj** , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-214">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="9dbdf-215">c.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-215">c.</span></span> <span data-ttu-id="9dbdf-216">Wybierz **(zakres) zsynchronizuj potencjalnego klienta lub szansę sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-216">Select **(Scope) Synchronize the lead or opportunity** .</span></span>

2. <span data-ttu-id="9dbdf-217">Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz opcję **Jeśli jest to nowa udostępniona okazja, a następnie** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-217">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then** .</span></span> <span data-ttu-id="9dbdf-218">Wybierz podkrok, **Jeśli tak** , a następnie rozwiń pozycję **Tworzenie nowej szansy sprzedaży w programie CRM** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-218">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM** .</span></span> <span data-ttu-id="9dbdf-219">Mapowania w tej sekcji można edytować za pomocą przewodnika mapowania pól.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-219">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="9dbdf-220">d.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-220">d.</span></span> <span data-ttu-id="9dbdf-221">Aby dostosować mapowania pól programu CRM (na podstawie przewodnika po mapowaniach pól) dla zdarzeń aktualizacji, kliknij krok "(zakres) zsynchronizuj lidera lub szansę sprzedaży".</span><span class="sxs-lookup"><span data-stu-id="9dbdf-221">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="9dbdf-222">e.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-222">e.</span></span> <span data-ttu-id="9dbdf-223">Wybierz **, czy jest to aktualizacja szansy sprzedaży, a następnie** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-223">Select **If it’s an update to an opportunity, then** .</span></span> <span data-ttu-id="9dbdf-224">Wybierz podkrok, **Jeśli tak** , a następnie rozwiń **, jeśli różnica między obiektami szansy sprzedaży w centrum partnerskim i CRM** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-224">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then** .</span></span>  

    <span data-ttu-id="9dbdf-225">f.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-225">f.</span></span> <span data-ttu-id="9dbdf-226">Wybierz opcję **tak** , po której następuje **Aktualizacja istniejącej szansy sprzedaży**</span><span class="sxs-lookup"><span data-stu-id="9dbdf-226">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="9dbdf-227">Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla zdarzeń aktualizacji:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-227">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="9dbdf-228">a.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-228">a.</span></span> <span data-ttu-id="9dbdf-229">Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="9dbdf-230">b.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-230">b.</span></span> <span data-ttu-id="9dbdf-231">Wybierz **(zakres) zsynchronizuj szansę sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-231">Select **(Scope) Synchronize the opportunity** .</span></span>

    <span data-ttu-id="9dbdf-232">c.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-232">c.</span></span> <span data-ttu-id="9dbdf-233">Aby dostosować mapowania pól programu CRM dla zdarzeń aktualizacji, należy wybrać, **czy istnieje różnica między obiektami lidera w centrum partnerskim i CRM, a następnie** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-233">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then** .</span></span> 

    <span data-ttu-id="9dbdf-234">d.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-234">d.</span></span> <span data-ttu-id="9dbdf-235">Wybierz krok podrzędny, **Jeśli tak** , a następnie rozwiń krok **Aktualizuj odwołanie z danymi o szansie sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-235">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data** .</span></span>

   <span data-ttu-id="9dbdf-236">Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-236">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="9dbdf-237">Aby dostosować pola dla programu CRM do synchronizacji odwołań komputera dla tworzenia zdarzeń?</span><span class="sxs-lookup"><span data-stu-id="9dbdf-237">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="9dbdf-238">a.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-238">a.</span></span> <span data-ttu-id="9dbdf-239">Wybierz pozycję **Edytuj**  , aby edytować/dostosować przepływ automatyzacji.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="9dbdf-240">b.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-240">b.</span></span> <span data-ttu-id="9dbdf-241">Wybierz **(zakres) synchronizowanie odwołań.**</span><span class="sxs-lookup"><span data-stu-id="9dbdf-241">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="9dbdf-242">c.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-242">c.</span></span> <span data-ttu-id="9dbdf-243">Aby dostosować mapowania pól programu CRM (w oparciu o Przewodnik po mapowaniu pól) dla zdarzeń tworzenia, wybierz pozycję **Utwórz odwołanie do firmy Microsoft** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-243">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral** .</span></span>

   <span data-ttu-id="9dbdf-244">Mapowania w tej sekcji można edytować w oparciu o Przewodnik po mapowaniu pól.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="9dbdf-245">Kompleksowa synchronizacja odwołań dwukierunkowych</span><span class="sxs-lookup"><span data-stu-id="9dbdf-245">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="9dbdf-246">Po zainstalowaniu, skonfigurowaniu i dostosowaniu rozwiązania do automatyzowania gotowości można testować synchronizację odwołań między programem Dynamics 365 i centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-246">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="9dbdf-247">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="9dbdf-247">Pre-requisites</span></span>

<span data-ttu-id="9dbdf-248">Aby synchronizować odwołania w centrum partnerskim i Dynamics 365 CRM, rozwiązanie do automatyzowania, które wyraźnie określa pola odwołań specyficzne dla firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-248">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="9dbdf-249">Dzięki tej identyfikacji sprzedawca może określić, które odwołania mają być udostępniane firmie Microsoft w celu współsprzedaży.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-249">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="9dbdf-250">Zestaw pól niestandardowych jest dostępny w ramach jednostki **szansy sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-250">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="9dbdf-251">Użytkownik będący administratorem programu CRM musi utworzyć osobną sekcję CRM z polami niestandardowymi **szansy sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-251">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="9dbdf-252">Następujące pola niestandardowe powinny być częścią sekcji CRM:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-252">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="9dbdf-253">**Synchronizuj z centrum partnerskim** : czy synchronizować szansę sprzedaży z Centrum partnerskiego firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="9dbdf-253">**Sync with Partner Center** : Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="9dbdf-254">**Identyfikator odwołania** : pole identyfikatora tylko do odczytu dla odwołania do Centrum partnerskiego firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="9dbdf-254">**Referral Identifier** : A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="9dbdf-255">**Link do odwołania** : link tylko do odczytu do odwołania w centrum partnerskim firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="9dbdf-255">**Referral Link** : A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="9dbdf-256">**Jak może pomóc firma Microsoft?** : pomoc wymagana przez firmę Microsoft do odwołania</span><span class="sxs-lookup"><span data-stu-id="9dbdf-256">**How can Microsoft help?** : Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="9dbdf-257">**Produkty** : Lista produktów skojarzonych z tą szansą sprzedaży</span><span class="sxs-lookup"><span data-stu-id="9dbdf-257">**Products** : List of products associated with this opportunity</span></span>

- <span data-ttu-id="9dbdf-258">**Inspekcja** : dziennik inspekcji tylko do odczytu na potrzeby synchronizacji z odwołaniami do Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="9dbdf-258">**Audit** : A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="9dbdf-259">SYTUACJI</span><span class="sxs-lookup"><span data-stu-id="9dbdf-259">SCENARIOS:</span></span>

1. <span data-ttu-id="9dbdf-260">Synchronizacja odwołań podczas tworzenia lub aktualizowania odwołania w programie CRM oraz synchronizowanie w centrum partnerskim:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-260">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="9dbdf-261">Zaloguj się do środowiska Dynamics 365 CRM przy użyciu użytkownika, który ma wgląd w sekcję **szansa sprzedaży** w programie CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-261">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="9dbdf-262">Upewnij się, że Poniższa sekcja jest obecna podczas tworzenia "nowej szansy" w środowisku Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9dbdf-262">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Sekcja Przykładowa okazja przedstawiająca informacje Centrum partnerskiego firmy Microsoft w usłudze Dynamics 365.":::

   3. <span data-ttu-id="9dbdf-264">Aby zsynchronizować tę szansę sprzedaży z centrum partnerskim firmy Microsoft, upewnij się, że ustawisz następujące pola w widoku karty:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-264">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="9dbdf-265">**Synchronizuj z centrum partnerskim** : tak</span><span class="sxs-lookup"><span data-stu-id="9dbdf-265">**Sync with Partner Center** : Yes</span></span>

      - <span data-ttu-id="9dbdf-266">**Jak może pomóc firma Microsoft?** : Wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-266">**How can Microsoft help?** : Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sekcja przykładowej szansy sprzedaży w usłudze Dynamics 365, która zawiera opcje pomocy Centrum partnerskiego firmy Microsoft obok pola o nazwie jak może pomóc firma Microsoft?":::

      - <span data-ttu-id="9dbdf-268">**Produkty** : identyfikatory rozwiązań produktu</span><span class="sxs-lookup"><span data-stu-id="9dbdf-268">**Products** : Solution IDs of the product</span></span>

   4. <span data-ttu-id="9dbdf-269">Po utworzeniu szansy sprzedaży w usłudze Dynamics 365 z opcją **Synchronizuj z centrum partnerskim** ustawionym na **wartość tak** , odczekaj 10 minut, a następnie zaloguj się do konta Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-269">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes** , wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="9dbdf-270">Twoje odwołania zostaną zsynchronizowane z usługą Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-270">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="9dbdf-271">Podobnie w przypadku opcji "Synchronizuj z centrum partnerskim" o wartości "tak" w przypadku zaktualizowania szansy sprzedaży w programie Dynamics 365 CRM zmiany zostaną zsynchronizowane na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-271">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="9dbdf-272">Prospekty, które zostały pomyślnie zsynchronizowane z centrum partnerskim, zostaną zidentyfikowane przy użyciu ikony ✔ w usłudze Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-272">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="9dbdf-273">Synchronizacja odwołań po utworzeniu lub zaktualizowaniu odwołania w centrum partnerskim firmy Microsoft i zsynchronizowaniu w środowisku Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="9dbdf-273">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="9dbdf-274">Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home)Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-274">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="9dbdf-275">Wybierz **odwołania** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-275">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="9dbdf-276">Utwórz nowe odwołanie towarzyszące w centrum partnerskim, klikając pozycję "Nowa transakcja".</span><span class="sxs-lookup"><span data-stu-id="9dbdf-276">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="9dbdf-277">Zaloguj się do środowiska programu Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-277">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="9dbdf-278">Przejdź do **okna Otwórz szanse sprzedaży** .</span><span class="sxs-lookup"><span data-stu-id="9dbdf-278">Navigate to **Open Opportunities** .</span></span> <span data-ttu-id="9dbdf-279">Odwołanie utworzone w Centrum partnerskiego firmy Microsoft jest teraz synchronizowane w programie Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-279">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="9dbdf-280">Po wybraniu synchronizowanego odwołania są wypełniane szczegóły widoku karty.</span><span class="sxs-lookup"><span data-stu-id="9dbdf-280">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9dbdf-281">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="9dbdf-281">Next steps</span></span>

- [<span data-ttu-id="9dbdf-282">Zarządzanie potencjalnymi klientami</span><span class="sxs-lookup"><span data-stu-id="9dbdf-282">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="9dbdf-283">Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)</span><span class="sxs-lookup"><span data-stu-id="9dbdf-283">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="9dbdf-284">Więcej informacji na temat platformy Microsoft energooszczędnej?</span><span class="sxs-lookup"><span data-stu-id="9dbdf-284">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="9dbdf-285">Elementy webhook Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="9dbdf-285">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)