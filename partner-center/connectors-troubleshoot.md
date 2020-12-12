---
title: Rozwiązywanie problemów dotyczących współsprzedawanych łączników
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Poznaj odpowiedzi na często zadawane pytania dotyczące korzystania z łączników współsprzedawanych. Przeczytaj ten temat często zadawanych pytań dotyczących rozwiązywania problemów z łącznikami współsprzedawanymi.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354546"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="61b34-104">Rozwiązywanie problemów dotyczących współsprzedawanych łączników</span><span class="sxs-lookup"><span data-stu-id="61b34-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="61b34-105">**Dotyczy:**</span><span class="sxs-lookup"><span data-stu-id="61b34-105">**Applies to:**</span></span>

- <span data-ttu-id="61b34-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="61b34-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="61b34-107">Aplikacja Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="61b34-107">Salesforce CRM</span></span>

<span data-ttu-id="61b34-108">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="61b34-108">**Appropriate roles**</span></span>

- <span data-ttu-id="61b34-109">Administrator odwołań</span><span class="sxs-lookup"><span data-stu-id="61b34-109">Referrals admin</span></span>
- <span data-ttu-id="61b34-110">Administrator systemu lub Konfigurator systemu w programie CRM</span><span class="sxs-lookup"><span data-stu-id="61b34-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="61b34-111">Pytania i odpowiedzi dotyczące wymagań wstępnych</span><span class="sxs-lookup"><span data-stu-id="61b34-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="61b34-112">Czy można korzystać z wersji próbnej do współtworzenia łączników odwołań dla danego środowiska?</span><span class="sxs-lookup"><span data-stu-id="61b34-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="61b34-113">Jeśli pracujesz w środowisku testowym/przejściowym, możesz wybrać rozwiązanie próbne.</span><span class="sxs-lookup"><span data-stu-id="61b34-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="61b34-114">Płatna wersja łączników jest dostępna w AppSource w Stanach Zjednoczonych $15 miesięcznie.</span><span class="sxs-lookup"><span data-stu-id="61b34-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="61b34-115">Dzięki połączeniu płatnym będzie można uzyskać 10 tys. wywołań interfejsu API dziennie.</span><span class="sxs-lookup"><span data-stu-id="61b34-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="61b34-116">Łączniki są otokami na podstawie interfejsów API odwołań Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="61b34-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="61b34-117">Za każdym razem, gdy zostaną uruchomione rozwiązania łącznika w celu **utworzenia** lub **zaktualizowania** zdarzenia dotyczącego możliwości w centrum partnerskim lub po stronie programu CRM, wykonywane jest wywołanie interfejsu API.</span><span class="sxs-lookup"><span data-stu-id="61b34-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="61b34-118">Jaką rolę należy utworzyć w środowisku programu CRM?</span><span class="sxs-lookup"><span data-stu-id="61b34-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="61b34-119">Użytkownicy będący administratorami systemu lub konfiguratorami systemu mogą stosować zmiany dla wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="61b34-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="61b34-120">Wszyscy użytkownicy aplikacji mogą jednak personalizować system i nawet udostępniać niektóre dostosowania innym osobom.</span><span class="sxs-lookup"><span data-stu-id="61b34-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="61b34-121">Czy sprzedawcy w ramach partnerów potrzebują specjalnych ról do pracy w centrum partnerskim?</span><span class="sxs-lookup"><span data-stu-id="61b34-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="61b34-122">Sprzedawcy z partnerami muszą mieć przypisaną rolę "Administrator odwołań".</span><span class="sxs-lookup"><span data-stu-id="61b34-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="61b34-123">Aby uzyskać więcej informacji, zobacz następujące [omówienie uprawnień) (Create-User-Account-and-Set-Permissions).</span><span class="sxs-lookup"><span data-stu-id="61b34-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="61b34-124">Jakie pola należy najpierw skonfigurować w środowisku programu CRM?</span><span class="sxs-lookup"><span data-stu-id="61b34-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="61b34-125">• Upewnij się, że Twoja waluta jest odpowiednia dla Twojej lokalizacji i że znajduje się w środowisku programu CRM.</span><span class="sxs-lookup"><span data-stu-id="61b34-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="61b34-126">• Zespół ds. sprzedaży powinien być wymieniony w środowisku programu CRM jako użytkownicy programu CRM.</span><span class="sxs-lookup"><span data-stu-id="61b34-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="61b34-127">Jakie wymagania wstępne są wymagane do utworzenia środowiska w celu zautomatyzowania pracy?</span><span class="sxs-lookup"><span data-stu-id="61b34-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="61b34-128">Aby móc korzystać ze środowiska automatyzacji, potrzebne są:</span><span class="sxs-lookup"><span data-stu-id="61b34-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="61b34-129">Wymagana jest licencja na automatyzację.</span><span class="sxs-lookup"><span data-stu-id="61b34-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="61b34-130">Wymagany jest co najmniej 1 GB pamięci masowej.</span><span class="sxs-lookup"><span data-stu-id="61b34-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="61b34-131">Potrzebujesz subskrypcji usługi Dynamics 365 do korzystania z rozwiązania usługi Salesforce?</span><span class="sxs-lookup"><span data-stu-id="61b34-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="61b34-132">Rozwiązanie łącznika usługi Salesforce jest typu "Dynamics Flow", które obsługuje synchronizację z innymi systemami CRM.</span><span class="sxs-lookup"><span data-stu-id="61b34-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="61b34-133">Rozwiązanie nie wymaga posiadania wystąpienia usługi Dynamics 365 lub subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="61b34-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="61b34-134">Podczas instalowania rozwiązania Salesforce może pojawić się lista rozwijana z istniejącym środowiskiem dysków CD w firmie.</span><span class="sxs-lookup"><span data-stu-id="61b34-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="61b34-135">Musisz wybrać to środowisko.</span><span class="sxs-lookup"><span data-stu-id="61b34-135">You need to select that environment.</span></span> <span data-ttu-id="61b34-136">Ponadto jeśli zostanie wyświetlony komunikat o błędzie "nie można odnaleźć organizacji usługi Dynamics 365 podłączonej do zalogowanego użytkownika", należy utworzyć nowe środowisko dla łącznika.</span><span class="sxs-lookup"><span data-stu-id="61b34-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="61b34-137">Pytania i odpowiedzi dotyczące konfiguracji</span><span class="sxs-lookup"><span data-stu-id="61b34-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="61b34-138">Co należy zrobić, jeśli podczas aktywowania przepływów na platformie automatyzacji w programie zawarto następujące błędy?</span><span class="sxs-lookup"><span data-stu-id="61b34-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="61b34-139">Błąd: żądanie do Azure Resource Manager nie powiodło się z powodu błędu: "{" błąd ": {" Code ":" WorkflowTriggerNotFound "," Message ":" nie można odnaleźć wyzwalacza "Manual" przepływu pracy "e14d00f1-1fdf-4b1b-aaac-54a5064093d3". "}}".</span><span class="sxs-lookup"><span data-stu-id="61b34-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="61b34-140">Wykonaj następujące kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="61b34-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="61b34-141">Usuń połączenie z DYSKami CD, a następnie ponownie utwórz połączenia z DYSKami CD.</span><span class="sxs-lookup"><span data-stu-id="61b34-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="61b34-142">Włączanie i wyłączanie przepływu podrzędnego</span><span class="sxs-lookup"><span data-stu-id="61b34-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="61b34-143">Usuń rozwiązanie, a następnie ponownie zainstaluj rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="61b34-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="61b34-144">Co należy zrobić, jeśli podczas dodawania łącznika Centrum partnerskiego na platformie automatyzacji jest zależeć błąd "Logowanie"?</span><span class="sxs-lookup"><span data-stu-id="61b34-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Komunikat o błędzie wymagający zalogowania":::

<span data-ttu-id="61b34-146">Wykonaj ten krok rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="61b34-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="61b34-147">Użyj poświadczeń Centrum partnerskiego, aby zalogować się do środowiska przepływu raz (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="61b34-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="61b34-148">Co należy zrobić, jeśli wystąpi następujący błąd podczas aktywowania Centrum partnerskiego do przepływu CRM w ramach platformy w automatyzowaniu?</span><span class="sxs-lookup"><span data-stu-id="61b34-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Komunikat o błędzie wymagający aktualizacji":::

<span data-ttu-id="61b34-150">Wykonaj następujące kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="61b34-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="61b34-151">Przed aktywowaniem Centrum partnerskiego do przepływu CRM należy najpierw aktywować dwa następujące przepływy podrzędne.</span><span class="sxs-lookup"><span data-stu-id="61b34-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="61b34-152">Partner Center do CRM — pomocnik (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="61b34-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="61b34-153">Centrum partnerskie — aktualizacje odwołań towarzyszące firmie Microsoft do programu CRM (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="61b34-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="61b34-154">Co należy zrobić, jeśli nie będziesz w stanie dodać połączeń do przepływu podczas próby edytowania przepływu?</span><span class="sxs-lookup"><span data-stu-id="61b34-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="61b34-155">Można dodać połączenia do przepływu, gdy przepływ jest uruchomiony, i oddzielnie dodać do każdego przepływu.</span><span class="sxs-lookup"><span data-stu-id="61b34-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="61b34-156">Jeśli okno dialogowe dodawania połączeń nie jest automatycznie otwierane podczas edytowania przepływu, można edytować poszczególne kroki i podrzędne etapy przepływów osobno.</span><span class="sxs-lookup"><span data-stu-id="61b34-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="61b34-157">Zaznacz każdy przepływ i edytuj je pojedynczo.</span><span class="sxs-lookup"><span data-stu-id="61b34-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="61b34-158">Rozwiń wszystkie kroki w przepływie</span><span class="sxs-lookup"><span data-stu-id="61b34-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Kroki, które wymagają połączeń":::

- <span data-ttu-id="61b34-160">Wybierz kroki, w których zostanie wyświetlona ikona ostrzeżenia z prośbą o skojarzenie połączeń i Dodawanie połączeń.</span><span class="sxs-lookup"><span data-stu-id="61b34-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Edytuj przepływ krok po kroku":::


5. <span data-ttu-id="61b34-162">Co należy zrobić, jeśli nie można włączyć rozwiązania łączników odwołań współsprzedawanych?</span><span class="sxs-lookup"><span data-stu-id="61b34-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="61b34-163">A.</span><span class="sxs-lookup"><span data-stu-id="61b34-163">A.</span></span> <span data-ttu-id="61b34-164">W programie w celu zautomatyzowania należy edytować przepływy w następującej kolejności i zaktualizować je, aby korzystały z prawidłowych połączeń:</span><span class="sxs-lookup"><span data-stu-id="61b34-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="61b34-165">Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="61b34-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="61b34-166">Utwórz odwołanie do towarzyszącej usługi Salesforce do Centrum partnerskiego (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="61b34-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="61b34-167">Centrum partnerskie — aktualizacje referencyjne firmy Microsoft do usługi Salesforce (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="61b34-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="61b34-168">Centrum partnerskie do usługi Salesforce (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="61b34-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="61b34-169">Centrum usług Salesforce dla partnerów partnerskich (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="61b34-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="61b34-170">Okazja do Centrum partnerskiego w usłudze Salesforce (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="61b34-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="61b34-171">Rozwiązania firmy Microsoft do Centrum partnerskiego (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="61b34-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="61b34-172">B.</span><span class="sxs-lookup"><span data-stu-id="61b34-172">B.</span></span> <span data-ttu-id="61b34-173">Dla każdego przepływu wybierz opcję **Uruchom tylko użytkownicy** .</span><span class="sxs-lookup"><span data-stu-id="61b34-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="61b34-174">Wybierz pozycję **Użyj połączenia** zamiast **podanej przez użytkownika tylko do uruchomienia**.</span><span class="sxs-lookup"><span data-stu-id="61b34-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Aby uaktywnić przepływ":::


<span data-ttu-id="61b34-176">C.</span><span class="sxs-lookup"><span data-stu-id="61b34-176">C.</span></span> <span data-ttu-id="61b34-177">Aktywuj poniższe przepływy:</span><span class="sxs-lookup"><span data-stu-id="61b34-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="61b34-178">Centrum partnerskie — aktualizacje referencyjne firmy Microsoft do usługi Salesforce (wersja zapoznawcza programu testowego)</span><span class="sxs-lookup"><span data-stu-id="61b34-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="61b34-179">Centrum usług Salesforce dla partnerów partnerskich (wersja zapoznawcza)</span><span class="sxs-lookup"><span data-stu-id="61b34-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="61b34-180">D.</span><span class="sxs-lookup"><span data-stu-id="61b34-180">D.</span></span> <span data-ttu-id="61b34-181">Aktywuj wszystkie pozostałe przepływy.</span><span class="sxs-lookup"><span data-stu-id="61b34-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="61b34-182">E.</span><span class="sxs-lookup"><span data-stu-id="61b34-182">E.</span></span> <span data-ttu-id="61b34-183">W obszarze Rejestracja elementu webhook Centrum partnerskiego w usłudze Flow wybierz pozycję **Uruchom**.</span><span class="sxs-lookup"><span data-stu-id="61b34-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="61b34-184">Podaj **adres URL protokołu HTTP** od pierwszej akcji w **centrum partnerskim do** przepływu usługi Salesforce.</span><span class="sxs-lookup"><span data-stu-id="61b34-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="61b34-185">Zaznacz wszystkie cztery opcje w obszarze **zdarzenia do zarejestrowania** i wybierz pozycję **tak** dla opcji Zastąp.</span><span class="sxs-lookup"><span data-stu-id="61b34-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="61b34-186">Pytania i odpowiedzi dotyczące uruchamiania/konserwacji</span><span class="sxs-lookup"><span data-stu-id="61b34-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="61b34-187">Jak rozwiązywać problemy w przypadku awarii podczas wykonywania przepływu w ramach automatyzacji</span><span class="sxs-lookup"><span data-stu-id="61b34-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="61b34-188">Aby upewnić się, że przepływy Automatyzuj działają zgodnie z oczekiwaniami i rozwiązywanie problemów podczas wykonywania, zapoznaj się z tematem [usuwanie błędów przepływu](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="61b34-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="61b34-189">Co należy zrobić, Jeśli zobaczysz odwołania, które nie są prawidłowo zsynchronizowane w centrum partnerskim lub w środowisku programu CRM?</span><span class="sxs-lookup"><span data-stu-id="61b34-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="61b34-190">Aby określić stan synchronizacji odwołań, wybierz pozycję **Inspekcja**.</span><span class="sxs-lookup"><span data-stu-id="61b34-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Jak synchronizować odwołania":::

<span data-ttu-id="61b34-192">Upewnij się, że zostały spełnione następujące warunki:</span><span class="sxs-lookup"><span data-stu-id="61b34-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="61b34-193">Identyfikator rozwiązania jest dostarczany jako część szansy sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="61b34-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="61b34-194">Wymagany jest dwuliterowy kod kraju.</span><span class="sxs-lookup"><span data-stu-id="61b34-194">Two letter country code is required.</span></span>

- <span data-ttu-id="61b34-195">Jeśli dla szansy sprzedaży została wybrana Pomoc firmy Microsoft, wymagane są informacje kontaktowe klienta.</span><span class="sxs-lookup"><span data-stu-id="61b34-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="61b34-196">Jak upewnić się, że odwołanie zostanie zsynchronizowane dwukierunkowo?</span><span class="sxs-lookup"><span data-stu-id="61b34-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="61b34-197">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="61b34-197">Do the following steps:</span></span>

- <span data-ttu-id="61b34-198">Sprzedawcy partnerów muszą mieć pewność, że włączyli opcję **Synchronizuj z Centrum partnerskiego** w sekcji CRM.</span><span class="sxs-lookup"><span data-stu-id="61b34-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Upewnij się, że włączono synchronizację":::

- <span data-ttu-id="61b34-200">Sprzedawcy muszą podawać przychody i daty zamknięcia przy zakwalifikowaniu potencjalnego klienta.</span><span class="sxs-lookup"><span data-stu-id="61b34-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="61b34-201">Jeśli na etapie **tworzenia** lub **aktualizowania** możliwości WSPÓŁsprzedaży została podana nazwa programu CRM, ale w programie CRM nie znaleziono szansy sprzedaży z tym identyfikatorem, aktualizacje lub tworzenie zostaną zignorowane.</span><span class="sxs-lookup"><span data-stu-id="61b34-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="61b34-202">Upewnij się, że pole Waluta odwołania jest skonfigurowane w środowisku usługi Salesforce.</span><span class="sxs-lookup"><span data-stu-id="61b34-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="61b34-203">Co należy zrobić, jeśli łącznik zostanie odłączony i zostanie pominięta synchronizacja odwołań.</span><span class="sxs-lookup"><span data-stu-id="61b34-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="61b34-204">Poniżej przedstawiono kilka opcji, które można wypróbować:</span><span class="sxs-lookup"><span data-stu-id="61b34-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="61b34-205">Sprawdź, czy nazwa użytkownika lub hasło wygasły w przypadku użytkowników Centrum partnerskiego z odwołaniami do ról administratora.</span><span class="sxs-lookup"><span data-stu-id="61b34-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="61b34-206">Możesz przejść do niezsynchronizowanej możliwości, wprowadzić drobną aktualizację i sprawdzić, czy odwołanie zostało zsynchronizowane.</span><span class="sxs-lookup"><span data-stu-id="61b34-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="61b34-207">Jeśli przepływy zostały uruchomione i zakończyły się niepowodzeniem, wybierz przepływ i ponownie prześlij przebieg, który zakończył się niepowodzeniem.</span><span class="sxs-lookup"><span data-stu-id="61b34-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="61b34-208">Co należy zrobić, gdy zostanie wyświetlony błąd odmowy dostępu?</span><span class="sxs-lookup"><span data-stu-id="61b34-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="61b34-209">Upewnij się, że istnieją odpowiednie role</span><span class="sxs-lookup"><span data-stu-id="61b34-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="61b34-210">Rola administratora odwołań dla sprzedawcy Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="61b34-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="61b34-211">Rola Administrator systemu lub Konfigurator systemu w wystąpieniu programu CRM</span><span class="sxs-lookup"><span data-stu-id="61b34-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="61b34-212">Upewnij się, że użytkownik konta przepływu automatyzacji https://flow.microsoft.com</span><span class="sxs-lookup"><span data-stu-id="61b34-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="61b34-213">Co należy zrobić, jeśli podczas tworzenia szansy sprzedaży nie ma **kodu kraju konta klienta** ?</span><span class="sxs-lookup"><span data-stu-id="61b34-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="61b34-214">Konieczne będzie dodanie dwuliterowego kodu ISO do konta klienta w programie CRM.</span><span class="sxs-lookup"><span data-stu-id="61b34-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="61b34-215">Co należy zrobić, Jeśli zobaczysz błąd, którego **Identyfikator rozwiązania jest wymagany** podczas tworzenia możliwości współsprzedaży?</span><span class="sxs-lookup"><span data-stu-id="61b34-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="61b34-216">Aby można było utworzyć odwołanie do współsprzedawcy, potrzebne jest rozwiązanie do współpracy z firmą Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61b34-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="61b34-217">Co należy zrobić, gdy zobaczysz możliwości wspólnej sprzedaży utworzone w centrum partnerskim, które nie są zsynchronizowane z aplikacją CRM, mimo że nie występują błędy przepływu:</span><span class="sxs-lookup"><span data-stu-id="61b34-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="61b34-218">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="61b34-218">Do the following:</span></span>

- <span data-ttu-id="61b34-219">Po utworzeniu nowej transakcji towarzyszącej w centrum partnerskim Sprawdź, czy jest wywoływany przepływ Centrum partnerskiego do systemu Dynamics 365 (może zostać wywołany wiele razy).</span><span class="sxs-lookup"><span data-stu-id="61b34-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="61b34-220">Jeśli przepływ jest wywoływany, zaznacz wszystkie wywołane przepływy i zidentyfikuj przebieg przepływu, który zaktualizuje program CRM.</span><span class="sxs-lookup"><span data-stu-id="61b34-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="61b34-221">Można wykonać akcje i sprawdzić, czy aktualizacja programu CRM została zaktualizowana lub napotkała problem.</span><span class="sxs-lookup"><span data-stu-id="61b34-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="61b34-222">Sprawdź *nowe rozpatrzenie* w centrum partnerskim, aby sprawdzić, czy jest ono wypełnione identyfikatorem programu CRM.</span><span class="sxs-lookup"><span data-stu-id="61b34-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="61b34-223">Upewnij się, że transakcja nie została przypadkowo ZAMKNIĘTA jako "kupione" lub "zgubione" w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="61b34-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="61b34-224">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="61b34-224">Next steps</span></span>

- [<span data-ttu-id="61b34-225">Zarządzanie potencjalnymi klientami</span><span class="sxs-lookup"><span data-stu-id="61b34-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="61b34-226">Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)</span><span class="sxs-lookup"><span data-stu-id="61b34-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
