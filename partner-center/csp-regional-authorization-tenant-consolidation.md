---
title: Konsolidacja dzierżawy regionalnej autoryzacji dostawcy usług kryptograficznych
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Te instrukcje służą do konsolidacji dzierżawców dla różnych krajów/regionów. Obejmuje to procedurę migrowania kont klientów i subskrypcji klientów.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502574"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="4083e-104">Instrukcje dotyczące konsolidacji dzierżawy regionalnej autoryzacji dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="4083e-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="4083e-105">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="4083e-105">**Applies to**</span></span>

- <span data-ttu-id="4083e-106">Centrum partnerskie Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="4083e-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="4083e-107">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="4083e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="4083e-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="4083e-108">Global admin</span></span>
- <span data-ttu-id="4083e-109">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="4083e-109">Admin agent</span></span>

<span data-ttu-id="4083e-110">\[Niektóre informacje odnoszą się do wstępnie wydanego produktu, który można w znacznym stopniu modyfikować przed udostępnieniem handlowym.</span><span class="sxs-lookup"><span data-stu-id="4083e-110">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="4083e-111">Firma Microsoft nie udziela żadnych gwarancji, jawnych lub domniemanych, w odniesieniu do informacji podanych w tym miejscu.\]</span><span class="sxs-lookup"><span data-stu-id="4083e-111">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="4083e-112">Można skonsolidować dzierżawców dla swojej firmy.</span><span class="sxs-lookup"><span data-stu-id="4083e-112">You can consolidate tenants for your business.</span></span> <span data-ttu-id="4083e-113">Te instrukcje służą do konsolidacji dzierżawców dla różnych krajów/regionów.</span><span class="sxs-lookup"><span data-stu-id="4083e-113">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="4083e-114">Użytkownik musi mieć świadomość wszystkich zainicjowanych subskrypcji i liczby licencji dla każdego z klientów na koncie, z którego się przechodzi.</span><span class="sxs-lookup"><span data-stu-id="4083e-114">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="4083e-115">Będziesz ponownie obsługiwać te same dokładne subskrypcje z tymi samymi liczbami licencji w ramach nowego centralnego konta CSP w ramach procesu migracji.</span><span class="sxs-lookup"><span data-stu-id="4083e-115">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="4083e-116">Korzystając z funkcji Eksportuj listę, można utworzyć listę klientów, którzy mają przechodzenie do scentralizowanej dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="4083e-116">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="4083e-117">Po zakończeniu konsolidacji nie można przywrócić poprzedniego stanu dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="4083e-117">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="4083e-118">Może być również wymagana akcja klienta.</span><span class="sxs-lookup"><span data-stu-id="4083e-118">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="4083e-119">Przygotowanie do migracji</span><span class="sxs-lookup"><span data-stu-id="4083e-119">Prepare for migration</span></span>

- <span data-ttu-id="4083e-120">Zaloguj się do **Centrum partnerskiego**  przy użyciu konta **przechodzenia** (zostanie ono przenoszone na nowe konto) i przejrzyj wszystkich klientów oraz wszystkie usługi zainicjowane dla tych klientów.</span><span class="sxs-lookup"><span data-stu-id="4083e-120">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="4083e-121">Wyloguj się z tego konta.</span><span class="sxs-lookup"><span data-stu-id="4083e-121">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="4083e-122">Migrowanie kont klientów</span><span class="sxs-lookup"><span data-stu-id="4083e-122">Migrate customer accounts</span></span>

1. <span data-ttu-id="4083e-123">Zaloguj się do **Centrum partnerskiego**  przy użyciu konta **przechodzenia** (nowe) (do którego są przenoszone klienci).</span><span class="sxs-lookup"><span data-stu-id="4083e-123">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="4083e-124">Wybierz pozycję **Klienci**.</span><span class="sxs-lookup"><span data-stu-id="4083e-124">Select **Customers**.</span></span>

3. <span data-ttu-id="4083e-125">Wybierz pozycję **Żądaj relacji odsprzedawcy**.</span><span class="sxs-lookup"><span data-stu-id="4083e-125">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="4083e-126">Zostanie wyświetlona domyślna wiadomość e-mail do wysłania do klientów.</span><span class="sxs-lookup"><span data-stu-id="4083e-126">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="4083e-127">Ten komunikat zawiera adres URL z unikatowym IDENTYFIKATORem organizacji dla nowego konta Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="4083e-127">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="4083e-128">**Akcja klienta:** Upewnij się, że każdy aktywny klient, który ma zostać zmigrowany, odwiedzi ten adres URL.</span><span class="sxs-lookup"><span data-stu-id="4083e-128">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="4083e-129">Podczas otwierania adresu URL klient zostanie poproszony o zalogowanie się w portalu pakietu Office 365.</span><span class="sxs-lookup"><span data-stu-id="4083e-129">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="4083e-130">Klient loguje się przy użyciu tego samego identyfikatora organizacji, który służy do uzyskiwania dostępu do portali administratorów platformy Azure i pakietu Office 365.</span><span class="sxs-lookup"><span data-stu-id="4083e-130">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="4083e-131">Po zalogowaniu Administrator globalny **konta klienta** zostanie poproszony o przesłanie umowy zapewniającej uprawnienia administratora delegowanego do nowego konta dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="4083e-131">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="4083e-132">Jeśli zgadzają się, klient wybierze pole wyboru i zgadza się na autoryzację relacji.</span><span class="sxs-lookup"><span data-stu-id="4083e-132">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="4083e-133">Po przesłaniu umowy klient zostanie wyświetlony na liście klientów partnera.</span><span class="sxs-lookup"><span data-stu-id="4083e-133">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="4083e-134">Migrowanie subskrypcji pakietu Office 365 i nie korzystających z platformy Azure</span><span class="sxs-lookup"><span data-stu-id="4083e-134">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="4083e-135">Po podpisaniu umowy przez klienta możesz ponownie utworzyć swoje subskrypcje w ramach dzierżawy scentralizowanego partnera.</span><span class="sxs-lookup"><span data-stu-id="4083e-135">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="4083e-136">W **centrum partnerskim** wybierz pozycję **klienci**.</span><span class="sxs-lookup"><span data-stu-id="4083e-136">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="4083e-137">Otwórz nazwę firmy dla klienta, który ma zostać zmigrowany.</span><span class="sxs-lookup"><span data-stu-id="4083e-137">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="4083e-138">Wybierz pozycję **Dodaj subskrypcję**.</span><span class="sxs-lookup"><span data-stu-id="4083e-138">Select **Add subscription**.</span></span>

5. <span data-ttu-id="4083e-139">Dodaj prawidłowe subskrypcje i liczby licencji z wykazu.</span><span class="sxs-lookup"><span data-stu-id="4083e-139">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="4083e-140">Sprawdź informacje zawarte w **przejściu z** kont partnerów.</span><span class="sxs-lookup"><span data-stu-id="4083e-140">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Lista klientów":::

6. <span data-ttu-id="4083e-142">Wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="4083e-142">Select **Submit.**</span></span>

   <span data-ttu-id="4083e-143">Usługi są teraz udostępniane klientowi z **przechodzenia do** konta partnera.</span><span class="sxs-lookup"><span data-stu-id="4083e-143">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="4083e-144">Powtórz te kroki, aby przeprowadzić migrację subskrypcji dla wszystkich dodatkowych klientów.</span><span class="sxs-lookup"><span data-stu-id="4083e-144">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="4083e-145">Przed przejściem do następnej sekcji upewnij się, że wszystkie subskrypcje klienta istniejące w ramach **przejścia z** kont partnerów są ponownie inicjowane w ramach **przejścia do** konta partnera.</span><span class="sxs-lookup"><span data-stu-id="4083e-145">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="4083e-146">Partnerzy muszą zawiesić subskrypcje dotyczące **przejścia z** konta dzierżawy partnera w centrum partnerskim tego samego dnia, w którym te subskrypcje są przenoszone i konfigurowane w ramach **przejścia do** konta dzierżawcy partnera w Centrum partnerskiego w celu zapewnienia podwójnego rozliczania.</span><span class="sxs-lookup"><span data-stu-id="4083e-146">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="4083e-147">Żądania pomocy technicznej będą odrzucane w przypadku kredytów z powodu jakiegokolwiek nakładania się opłat, które wystąpiły od nieprawidłowego wyłączenia **przejścia z** subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="4083e-147">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="4083e-148">Wyłączanie subskrypcji pakietu Office 365 w ramach przejścia z konta partnera</span><span class="sxs-lookup"><span data-stu-id="4083e-148">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="4083e-149">Wyłączenie subskrypcji dostawcy usług kryptograficznych w ramach **przejścia z** kont partnerskich powoduje zatrzymanie wszelkich przyszłych rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="4083e-149">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="4083e-150">Nie musisz ręcznie wyłączać subskrypcji platformy Azure, ponieważ subskrypcje platformy Azure są automatycznie wyłączane podczas procesu migracji.</span><span class="sxs-lookup"><span data-stu-id="4083e-150">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="4083e-151">Zaloguj się do **Centrum partnerskiego** przy użyciu **przejścia z** konta CSP i przejdź do listy klient.</span><span class="sxs-lookup"><span data-stu-id="4083e-151">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="4083e-152">Otwórz klienta z subskrypcjami, aby wyłączyć, a następnie wybierz pierwszą ofertę do wyłączenia.</span><span class="sxs-lookup"><span data-stu-id="4083e-152">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="4083e-153">Ustaw subskrypcję na **zawieszone**, a następnie wybierz pozycję **Prześlij**.</span><span class="sxs-lookup"><span data-stu-id="4083e-153">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="4083e-154">Wstrzymanie subskrypcji gwarantuje, że podwójne rozliczenie nie nastąpi.</span><span class="sxs-lookup"><span data-stu-id="4083e-154">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="4083e-155">Subskrypcja zostanie **wyświetlona** na liście subskrypcje.</span><span class="sxs-lookup"><span data-stu-id="4083e-155">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="4083e-156">Powtórz te kroki dla wszystkich subskrypcji w ramach klienta.</span><span class="sxs-lookup"><span data-stu-id="4083e-156">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="4083e-157">Sprawdź, czy wszystkie wyświetlanie zostały **zawieszone.**</span><span class="sxs-lookup"><span data-stu-id="4083e-157">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="4083e-158">Wybierz następnego klienta z listy i powtórz proces wyłączania wszystkich subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="4083e-158">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="4083e-159">Migrowanie subskrypcji opartych na użyciu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="4083e-159">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="4083e-160">W przeciwieństwie do subskrypcji programu CSP pakietu Office 365, Azure, subskrypcje programu CSP oparte na użyciu nie muszą być migrowane ręcznie.</span><span class="sxs-lookup"><span data-stu-id="4083e-160">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="4083e-161">Obsługa Microsoft Azure przeprowadzi migrację subskrypcji platformy Azure i wszystkich wdrożonych usług lub zasobów z **przechodzenia z** kont odsprzedawcy programu CSP do **przejścia do** konta odsprzedawcy programu CSP.</span><span class="sxs-lookup"><span data-stu-id="4083e-161">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="4083e-162">W trakcie tego przejścia nie będzie zakłócać działania usługi dla klienta.</span><span class="sxs-lookup"><span data-stu-id="4083e-162">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="4083e-163">Upewnij się, że konta klientów, dla których zostały zmigrowane subskrypcje platformy Azure, zaakceptowały umowę, która zostanie skojarzona z nowym **przejściem do** konta dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="4083e-163">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="4083e-164">Powiadomimy firmę Microsoft o tym, które konta klientów są gotowe do migracji, i podają nazwy firmowe tego klienta.</span><span class="sxs-lookup"><span data-stu-id="4083e-164">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="4083e-165">Firma Microsoft migruje subskrypcje oparte na użyciu platformy Azure i powiadamia o zakończeniu migracji.</span><span class="sxs-lookup"><span data-stu-id="4083e-165">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="4083e-166">Musisz upewnić się, że subskrypcja platformy Azure w ramach **przejścia z** konta odsprzedawcy dostawcy CSP jest teraz oznaczona jako **zawieszona** w centrum partnerskim w sekcji subskrypcje klienta.</span><span class="sxs-lookup"><span data-stu-id="4083e-166">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="4083e-167">Upewnij się, że w ramach subskrypcji platformy Azure w ramach **przejścia do** konta odsprzedawcy CSP jest teraz wyświetlany stan **aktywny** w centrum partnerskim w sekcji subskrypcje klienta.</span><span class="sxs-lookup"><span data-stu-id="4083e-167">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="4083e-168">Wyłączenie subskrypcji w ramach klienta nie powoduje zmiany wyglądu klienta na liście klientów.</span><span class="sxs-lookup"><span data-stu-id="4083e-168">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="4083e-169">Obecnie nie ma możliwości usunięcia klientów z listy.</span><span class="sxs-lookup"><span data-stu-id="4083e-169">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="4083e-170">Partnerzy powinni unikać dodawania **subskrypcji z powrotem** do klientów w przyszłości.</span><span class="sxs-lookup"><span data-stu-id="4083e-170">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="4083e-171">Powtórz te kroki dla wszystkich subskrypcji w ramach wszystkich klientów, aby zrezygnować z przyszłych opłat za **przejście z** kont.</span><span class="sxs-lookup"><span data-stu-id="4083e-171">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="4083e-172">Partner otrzyma jedną fakturę ostateczną ze środkiem za liczbę nieużywanych dni między dniem anulowania a ostatnim dniem okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="4083e-172">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="4083e-173">Nie będą generowane żadne przyszłe faktury po upływie ostatecznego okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="4083e-173">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="4083e-174">Dodatkowe informacje</span><span class="sxs-lookup"><span data-stu-id="4083e-174">Additional information</span></span>

- <span data-ttu-id="4083e-175">Wyłączenie **subskrypcji z konta CSP nie** ma wpływu na usługę klienta końcowego, o ile usługa została zainicjowana przy użyciu **przejścia do** konta CSP przed wyłączeniem subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="4083e-175">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="4083e-176">Nie można używać subskrypcji przez klienta i nie generują opłat po wstrzymaniu lub anulowaniu.</span><span class="sxs-lookup"><span data-stu-id="4083e-176">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="4083e-177">Obecnie nie istnieje sposób na całkowite usunięcie klienta z listy **klientów** .</span><span class="sxs-lookup"><span data-stu-id="4083e-177">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="4083e-178">Partnerzy muszą zawiesić subskrypcje dotyczące **przejścia z** konta dzierżawcy partnera w centrum partnerskim tego samego dnia, w którym subskrypcje są przenoszone i konfigurowane w ramach **przejścia do** konta w celu zapewnienia podwójnego rozliczania.</span><span class="sxs-lookup"><span data-stu-id="4083e-178">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="4083e-179">Firma Microsoft nie będzie obsługiwać próśb o kredyty ze względu na to, że wystąpiły zmiany w rozliczeniach, które wynikają z nieprawidłowego ustawienia **przejścia z** subskrypcji na zawieszone.</span><span class="sxs-lookup"><span data-stu-id="4083e-179">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="4083e-180">Uproszczenie migracji przy użyciu eksportu</span><span class="sxs-lookup"><span data-stu-id="4083e-180">Simplify migration using Export</span></span>

<span data-ttu-id="4083e-181">Za pomocą **funkcji eksportu** można przechwytywać subskrypcje, których należy użyć w nowej strukturze skonsolidowanej:</span><span class="sxs-lookup"><span data-stu-id="4083e-181">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="4083e-182">Wybierz pozycję **klienci** w centrum partnerskim, aby wyświetlić listę klientów.</span><span class="sxs-lookup"><span data-stu-id="4083e-182">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="4083e-183">Otwórz żądaną nazwę klienta.</span><span class="sxs-lookup"><span data-stu-id="4083e-183">Open the desired customer name.</span></span>

3. <span data-ttu-id="4083e-184">Na stronie **subskrypcje** wybierz pozycję **Eksportuj subskrypcje** , aby wyeksportować szczegóły subskrypcji do pliku programu Excel.</span><span class="sxs-lookup"><span data-stu-id="4083e-184">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="4083e-185">Użyj tej listy, aby ponownie utworzyć subskrypcje w nowej konsolidowanej dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="4083e-185">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="4083e-186">Rejestracja interfejsu API</span><span class="sxs-lookup"><span data-stu-id="4083e-186">API registration</span></span>

<span data-ttu-id="4083e-187">Aby uzyskać więcej informacji na temat rejestracji interfejsu API, zobacz [Konfigurowanie dostępu do interfejsu API w centrum partnerskim](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="4083e-187">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="4083e-188">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="4083e-188">Next steps</span></span>

- [<span data-ttu-id="4083e-189">Program dostawcy rozwiązań w chmurze — rynki regionalne i waluty, w których można sprzedawać oferty CSP</span><span class="sxs-lookup"><span data-stu-id="4083e-189">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
