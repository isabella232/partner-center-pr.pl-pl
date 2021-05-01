---
title: Rozwiązywanie problemów z łącznikami poleceń do współpracy
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Poznaj odpowiedzi na często zadawane pytania dotyczące używania łączników wspólnej sprzedaży. Przeczytaj często zadawane pytania dotyczące rozwiązywania problemów z łącznikami do współs sprzedaży.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284217"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="bb782-104">Rozwiązywanie problemów z łącznikami poleceń do współpracy</span><span class="sxs-lookup"><span data-stu-id="bb782-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="bb782-105">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="bb782-105">**Applies to**</span></span>

- <span data-ttu-id="bb782-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="bb782-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="bb782-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="bb782-107">Salesforce CRM</span></span>

<span data-ttu-id="bb782-108">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="bb782-108">**Appropriate roles**</span></span>

- <span data-ttu-id="bb782-109">Administrator poleceń</span><span class="sxs-lookup"><span data-stu-id="bb782-109">Referrals admin</span></span>
- <span data-ttu-id="bb782-110">Administrator systemu lub customizer systemu w systemie CRM</span><span class="sxs-lookup"><span data-stu-id="bb782-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="bb782-111">Pytania i odpowiedzi dotyczące wymagań wstępnych</span><span class="sxs-lookup"><span data-stu-id="bb782-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="bb782-112">Czy w swoim środowisku możesz użyć rozwiązania łączników do współsieć poleceń w wersji próbnej?</span><span class="sxs-lookup"><span data-stu-id="bb782-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="bb782-113">Jeśli jesteś w środowisku testowym/przejściowym, możesz wybrać rozwiązanie w wersji próbnej.</span><span class="sxs-lookup"><span data-stu-id="bb782-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="bb782-114">Płatna wersja łączników jest dostępna w usłudze AppSource w cenie 15 USD/miesiąc.</span><span class="sxs-lookup"><span data-stu-id="bb782-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="bb782-115">W przypadku połączenia płatnego będziesz otrzymywać 10 000 wywołań interfejsu API dziennie.</span><span class="sxs-lookup"><span data-stu-id="bb782-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="bb782-116">Łączniki są otoką na Partner Center interfejsów API poleceń.</span><span class="sxs-lookup"><span data-stu-id="bb782-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="bb782-117">Za każdym razem,  gdy  rozwiązania łącznika uruchamiają zdarzenie Utwórz lub Aktualizuj w przypadku szans sprzedaży Partner Center lub po stronie CRM, jest uruchamiane wywołanie interfejsu API.</span><span class="sxs-lookup"><span data-stu-id="bb782-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="bb782-118">Jaka rola jest potrzebna do tworzenia sekcji w środowisku CRM?</span><span class="sxs-lookup"><span data-stu-id="bb782-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="bb782-119">Użytkownicy, którzy są administratorami systemu lub osobami modyfikujący system, mogą stosować zmiany dla wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="bb782-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="bb782-120">Jednak wszyscy użytkownicy aplikacji mogą spersonalizować system, a nawet udostępnić niektóre z ich dostosowań innym użytkownikom.</span><span class="sxs-lookup"><span data-stu-id="bb782-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="bb782-121">Czy sprzedawcy partnerscy potrzebują specjalnych ról do pracy nad Partner Center?</span><span class="sxs-lookup"><span data-stu-id="bb782-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="bb782-122">Sprzedawcy partnerscy muszą mieć przypisaną rolę "Administrator poleceń".</span><span class="sxs-lookup"><span data-stu-id="bb782-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="bb782-123">Aby uzyskać więcej informacji, zobacz [Omówienie uprawnień.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="bb782-123">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="bb782-124">Jakie pola należy najpierw skonfigurować w środowisku CRM?</span><span class="sxs-lookup"><span data-stu-id="bb782-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="bb782-125">• Upewnij się, że Waluta jest odpowiednia dla Twojej lokalizacji i dokładnie znajduje się w środowisku CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="bb782-126">• Twój zespół sprzedaży powinien być wymieniony w Twoim środowisku CRM jako użytkownicy CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="bb782-127">Jakie wymagania wstępne są wymagane do Power Automate tworzenia środowiska?</span><span class="sxs-lookup"><span data-stu-id="bb782-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="bb782-128">Aby korzystać ze Power Automate, potrzebne są:</span><span class="sxs-lookup"><span data-stu-id="bb782-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="bb782-129">Wymagana Power Automate licencji użytkownika.</span><span class="sxs-lookup"><span data-stu-id="bb782-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="bb782-130">Wymagany jest magazyn o rozmiarze co najmniej 1 GB.</span><span class="sxs-lookup"><span data-stu-id="bb782-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="bb782-131">Czy do korzystania z rozwiązania Łączniki usługi Salesforce potrzebujesz subskrypcji usługi Dynamics 365?</span><span class="sxs-lookup"><span data-stu-id="bb782-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="bb782-132">Rozwiązanie łącznika usługi Salesforce jest typu "Dynamics Flow", które obsługuje synchronizację z innymi systemami CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="bb782-133">Rozwiązanie nie wymaga wystąpienia usługi Dynamics 365 ani subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="bb782-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="bb782-134">Podczas instalowania rozwiązania Salesforce może pojawić się lista rozwijana z istniejącym środowiskiem usługi CDS w firmie.</span><span class="sxs-lookup"><span data-stu-id="bb782-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="bb782-135">Musisz wybrać to środowisko.</span><span class="sxs-lookup"><span data-stu-id="bb782-135">You need to select that environment.</span></span> <span data-ttu-id="bb782-136">Ponadto jeśli wystąpi błąd "Nie można odnaleźć organizacji usługi Dynamics 365 połączonej z zalogowanym użytkownikiem", konieczne będzie utworzenie nowego środowiska dla łącznika.</span><span class="sxs-lookup"><span data-stu-id="bb782-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="bb782-137">Pytania i odpowiedzi dotyczące konfiguracji</span><span class="sxs-lookup"><span data-stu-id="bb782-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="bb782-138">Co należy zrobić, jeśli podczas aktywowania przepływów na platformie Power Automate Platform wystąpi następujący błąd?</span><span class="sxs-lookup"><span data-stu-id="bb782-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="bb782-139">Błąd: Żądanie Azure Resource Manager nie powiodło się z błędem: "{"error":{"code":"WorkflowTriggerNotFound","message":"Nie można odnaleźć wyzwalacza "manual" przepływu pracy "e14d00f1-1fdf-4b1b-aaac-54a5064093d3".</span><span class="sxs-lookup"><span data-stu-id="bb782-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="bb782-140">Wykonaj następujące kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="bb782-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="bb782-141">Usuń połączenie usługi CDS, a następnie utwórz ponownie połączenia usługi CDS.</span><span class="sxs-lookup"><span data-stu-id="bb782-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="bb782-142">Wyłączanie i włączanie przepływu podrzędnego</span><span class="sxs-lookup"><span data-stu-id="bb782-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="bb782-143">Usuń rozwiązanie, a następnie zainstaluj je ponownie.</span><span class="sxs-lookup"><span data-stu-id="bb782-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="bb782-144">Co należy zrobić, jeśli wystąpi błąd "Zaloguj się" podczas dodawania łącznika Partner Center platformie Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="bb782-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Komunikat o błędzie wymagający logowania":::

<span data-ttu-id="bb782-146">Wykonaj ten krok rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="bb782-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="bb782-147">Użyj swoich Partner Center, aby zalogować się do środowiska przepływu raz (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="bb782-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="bb782-148">Co należy zrobić w przypadku wystąpienia następującego błędu podczas aktywowania przepływu Partner Center CRM na Power Automate Platformie?</span><span class="sxs-lookup"><span data-stu-id="bb782-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Komunikat o błędzie wymagający aktualizacji":::

<span data-ttu-id="bb782-150">Wykonaj następujące kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="bb782-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="bb782-151">Aktywuj następujące dwa przepływy podrzędne przed aktywowaniem przepływu Partner Center do przepływu CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="bb782-152">Partner Center crm — pomocnik (niejawny program testów w wersji zapoznawczej)</span><span class="sxs-lookup"><span data-stu-id="bb782-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="bb782-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="bb782-154">Co należy zrobić, gdy nie możesz dodać połączeń do przepływu podczas próby edytowania przepływu?</span><span class="sxs-lookup"><span data-stu-id="bb782-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="bb782-155">Możesz dodawać połączenia do przepływu, gdy przepływ jest uruchomiony, i dodawać je do każdego przepływu oddzielnie.</span><span class="sxs-lookup"><span data-stu-id="bb782-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="bb782-156">Jeśli okno dialogowe dodawania połączeń nie zostanie automatycznie otwarte podczas edytowania przepływu, możesz edytować poszczególne kroki i pode kroki przepływów osobno.</span><span class="sxs-lookup"><span data-stu-id="bb782-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="bb782-157">Wybierz każdy przepływ i edytuj je indywidualnie.</span><span class="sxs-lookup"><span data-stu-id="bb782-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="bb782-158">Rozwiń wszystkie kroki w przepływie</span><span class="sxs-lookup"><span data-stu-id="bb782-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Kroki, które wymagają połączeń":::

- <span data-ttu-id="bb782-160">Wybierz kroki, w których zobaczysz ikonę ostrzeżenia z prośbą o skojarzenie połączeń i dodanie połączeń.</span><span class="sxs-lookup"><span data-stu-id="bb782-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Edytowanie przepływu krok po kroku":::


5. <span data-ttu-id="bb782-162">Co należy zrobić, jeśli przepływy rozwiązania łączników poleceń do współpracy sprzedaży nie są włączane?</span><span class="sxs-lookup"><span data-stu-id="bb782-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="bb782-163">A.</span><span class="sxs-lookup"><span data-stu-id="bb782-163">A.</span></span> <span data-ttu-id="bb782-164">W Power Automate należy edytować przepływy w następującej kolejności i zaktualizować je, aby używać poprawnych połączeń:</span><span class="sxs-lookup"><span data-stu-id="bb782-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="bb782-165">Partner Center rejestracji webhook (niejawny program testów w wersji zapoznawczej)</span><span class="sxs-lookup"><span data-stu-id="bb782-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="bb782-166">Tworzenie poleceń do współpracy sprzedaży — salesforce do Partner Center (insider preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="bb782-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="bb782-168">Partner Center do usługi Salesforce (niejawny program testów w wersji zapoznawczej)</span><span class="sxs-lookup"><span data-stu-id="bb782-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="bb782-169">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="bb782-170">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="bb782-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="bb782-172">B.</span><span class="sxs-lookup"><span data-stu-id="bb782-172">B.</span></span> <span data-ttu-id="bb782-173">Dla każdego przepływu wybierz **opcję Uruchom tylko** użytkowników.</span><span class="sxs-lookup"><span data-stu-id="bb782-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="bb782-174">Wybierz **pozycję Użyj połączenia** zamiast Dostarczone przez użytkownika tylko do **uruchamiania.**</span><span class="sxs-lookup"><span data-stu-id="bb782-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Aby aktywować przepływ":::


<span data-ttu-id="bb782-176">C.</span><span class="sxs-lookup"><span data-stu-id="bb782-176">C.</span></span> <span data-ttu-id="bb782-177">Aktywuj wymienione poniżej przepływy:</span><span class="sxs-lookup"><span data-stu-id="bb782-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="bb782-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="bb782-179">Salesforce to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="bb782-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="bb782-180">D.</span><span class="sxs-lookup"><span data-stu-id="bb782-180">D.</span></span> <span data-ttu-id="bb782-181">Aktywuj wszystkie pozostałe przepływy.</span><span class="sxs-lookup"><span data-stu-id="bb782-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="bb782-182">E.</span><span class="sxs-lookup"><span data-stu-id="bb782-182">E.</span></span> <span data-ttu-id="bb782-183">W witrynie flow Partner Center webhook Registration (Rejestracja) wybierz pozycję **Run (Uruchom).**</span><span class="sxs-lookup"><span data-stu-id="bb782-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="bb782-184">Podaj adres **URL HTTP** z pierwszej akcji w Partner Center **do przepływu usługi Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="bb782-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="bb782-185">Wybierz wszystkie cztery opcje w obszarze **Zdarzenia do zarejestrowania,** a następnie wybierz **pozycję Tak dla** opcji Zastąp.</span><span class="sxs-lookup"><span data-stu-id="bb782-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="bb782-186">Pytania i odpowiedzi dotyczące uruchamiania/konserwacji</span><span class="sxs-lookup"><span data-stu-id="bb782-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="bb782-187">Jak rozwiązywać problemy z błędami podczas wykonywania Power Automate przepływu?</span><span class="sxs-lookup"><span data-stu-id="bb782-187">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="bb782-188">Aby upewnić się, że przepływy Power Automate działają zgodnie z oczekiwaniami i rozwiązywać problemy z błędami podczas wykonywania, zobacz [Naprawianie błędów przepływu.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="bb782-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="bb782-189">Co należy zrobić, jeśli widzisz polecenia, które nie są prawidłowo synchronizowane Partner Center środowisku CRM?</span><span class="sxs-lookup"><span data-stu-id="bb782-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="bb782-190">Aby określić stan synchronizacji od skierowań, wybierz pozycję **Przejmij inspekcję.**</span><span class="sxs-lookup"><span data-stu-id="bb782-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Jak synchronizować polecenia":::

<span data-ttu-id="bb782-192">Upewnij się, że są spełnione następujące warunki:</span><span class="sxs-lookup"><span data-stu-id="bb782-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="bb782-193">Identyfikator rozwiązania jest dostarczany w ramach szansy sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="bb782-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="bb782-194">Wymagany jest dwulitowy kod kraju.</span><span class="sxs-lookup"><span data-stu-id="bb782-194">Two letter country code is required.</span></span>

- <span data-ttu-id="bb782-195">W przypadku wyboru pomocy firmy Microsoft na potrzeby szansy sprzedaży wymagane są informacje kontaktowe klienta.</span><span class="sxs-lookup"><span data-stu-id="bb782-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="bb782-196">Jak upewnić się, że polecenie będzie synchronizowane dwukierunkowo?</span><span class="sxs-lookup"><span data-stu-id="bb782-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="bb782-197">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="bb782-197">Do the following steps:</span></span>

- <span data-ttu-id="bb782-198">Sprzedawcy partnerscy muszą upewnić się, że włączyli opcję Synchronizuj **z Partner Center** w sekcji CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Upewnij się, że włączono usługę Synch":::

- <span data-ttu-id="bb782-200">Sprzedawcy muszą podać przychód i datę zamknięcia podczas kwalifikowania potencjalnego klienta.</span><span class="sxs-lookup"><span data-stu-id="bb782-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="bb782-201">Jeśli identyfikator CRM zostanie  podany  na etapie tworzenia lub aktualizowania szansy sprzedaży, ale szansa sprzedaży potencjalnego klienta z tym identyfikatorem nie zostanie znaleziona w programie CRM, aktualizacja lub tworzenie zostanie zignorowana.</span><span class="sxs-lookup"><span data-stu-id="bb782-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="bb782-202">Upewnij się, że pole waluty polecenia jest skonfigurowane w środowisku usługi Salesforce.</span><span class="sxs-lookup"><span data-stu-id="bb782-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="bb782-203">Co należy zrobić, jeśli łącznik zostanie odłączony i pominiesz synchronizację poleceń?</span><span class="sxs-lookup"><span data-stu-id="bb782-203">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="bb782-204">Poniżej przedstawiono kilka opcji, które można wypróbować:</span><span class="sxs-lookup"><span data-stu-id="bb782-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="bb782-205">Sprawdź, czy nazwa użytkownika lub hasło wygasły dla Partner Center z rolami administratora poleceń.</span><span class="sxs-lookup"><span data-stu-id="bb782-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="bb782-206">Możesz przejść do niezsynchronizowanych szans sprzedaży, wprowadzić aktualizację pomocniczą i sprawdzić, czy polecenie zostało zsynchronizowane.</span><span class="sxs-lookup"><span data-stu-id="bb782-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="bb782-207">Jeśli przepływy zostały uruchomione i zakończyły się niepowodzeniem, wybierz przepływ i prześlij ponownie przebieg, który zakończył się niepowodzeniem.</span><span class="sxs-lookup"><span data-stu-id="bb782-207">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="bb782-208">Co należy zrobić, gdy występują błędy odmowy dostępu?</span><span class="sxs-lookup"><span data-stu-id="bb782-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="bb782-209">Upewnij się, że istnieją odpowiednie role</span><span class="sxs-lookup"><span data-stu-id="bb782-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="bb782-210">Rola administratora poleceń dla Partner Center sprzedawcy</span><span class="sxs-lookup"><span data-stu-id="bb782-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="bb782-211">Rola administratora systemu lub customizera systemu w wystąpieniu systemu CRM</span><span class="sxs-lookup"><span data-stu-id="bb782-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="bb782-212">Upewnij się, Power Automate konto przepływu danych loguje się wcześniej https://flow.microsoft.com co najmniej raz</span><span class="sxs-lookup"><span data-stu-id="bb782-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="bb782-213">Jeśli zobaczysz, że **brakuje kodu** kraju konta klienta podczas tworzenia możliwości współpracy sprzedaży, co należy zrobić?</span><span class="sxs-lookup"><span data-stu-id="bb782-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="bb782-214">Musisz dodać dwuliterowy kod kraju ISO do konta klienta w systemie CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="bb782-215">Co należy zrobić, jeśli zobaczysz błąd, że **identyfikator rozwiązania jest** wymagany podczas tworzenia możliwości współpracy sprzedaży?</span><span class="sxs-lookup"><span data-stu-id="bb782-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="bb782-216">Aby utworzyć polecenie do współpracy sprzedaży, potrzebujesz gotowego rozwiązania firmy Microsoft do współpracy sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="bb782-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="bb782-217">Co należy zrobić, gdy zobaczysz możliwości współpracy sprzedaży utworzone w Partner Center, które nie są synchronizowane z programem CRM, mimo że nie ma żadnych błędów przepływu?</span><span class="sxs-lookup"><span data-stu-id="bb782-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="bb782-218">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="bb782-218">Do the following:</span></span>

- <span data-ttu-id="bb782-219">Po utworzeniu nowej transakcji sprzedaży typu "co-sell" w programie Partner Center sprawdź, czy zostanie wywołany przepływ Partner Center do usługi Dynamics 365 (może zostać wywołany wiele razy).</span><span class="sxs-lookup"><span data-stu-id="bb782-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="bb782-220">Jeśli przepływ zostanie wywołany, sprawdź wszystkie wywołane przepływy i zidentyfikuj przebieg przepływu, który zaktualizuje system CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-220">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="bb782-221">Możesz wykonać te akcje i sprawdzić, czy program zaktualizował system CRM, czy napotkał problem.</span><span class="sxs-lookup"><span data-stu-id="bb782-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="bb782-222">Sprawdź **nową Partner Center,** aby sprawdzić, czy zostanie ona wypełniona identyfikatorem CRM.</span><span class="sxs-lookup"><span data-stu-id="bb782-222">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="bb782-223">Upewnij się, że transakcja nie została przypadkowo zamknięta jako **Wygrana** lub **Utracona w** Partner Center.</span><span class="sxs-lookup"><span data-stu-id="bb782-223">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bb782-224">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="bb782-224">Next steps</span></span>

- [<span data-ttu-id="bb782-225">Zarządzanie potencjalnymi klientami</span><span class="sxs-lookup"><span data-stu-id="bb782-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="bb782-226">Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)</span><span class="sxs-lookup"><span data-stu-id="bb782-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
