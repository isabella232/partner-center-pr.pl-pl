---
title: Konsolidacja dzierżawy autoryzacji regionalnej programu CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Użyj tych instrukcji, aby skonsolidować dzierżawy dla różnych krajów/regionów. Obejmuje to kroki migracji kont klientów i subskrypcji klientów.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276879"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="8966a-104">Instrukcje dotyczące konsolidacji dzierżawy regionalnej autoryzacji dostawcy CSP</span><span class="sxs-lookup"><span data-stu-id="8966a-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="8966a-105">**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="8966a-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8966a-106">**Odpowiednie role:** Administrator globalny | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="8966a-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="8966a-107">\[Niektóre informacje odnoszą się do wstępnie wydanego produktu, który może zostać znacząco zmodyfikowany, zanim zostanie wydany komercyjnie.</span><span class="sxs-lookup"><span data-stu-id="8966a-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="8966a-108">Firma Microsoft nie udziela żadnych gwarancji, jawnych lub domniemanych, w odniesieniu do informacji podanych w tym miejscu.\]</span><span class="sxs-lookup"><span data-stu-id="8966a-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="8966a-109">Możesz konsolidować dzierżawy dla swojej firmy.</span><span class="sxs-lookup"><span data-stu-id="8966a-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="8966a-110">Użyj tych instrukcji, aby skonsolidować dzierżawy dla różnych krajów/regionów.</span><span class="sxs-lookup"><span data-stu-id="8966a-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="8966a-111">Musisz mieć świadomość wszystkich aprowowanych subskrypcji i liczby licencji dla każdego z klientów na koncie, z których przechodzisz.</span><span class="sxs-lookup"><span data-stu-id="8966a-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="8966a-112">W ramach procesu migracji ponownie aprowizuje się te same dokładnie subskrypcje z tymi samymi liczbami licencji w ramach nowego konta centralnego CSP.</span><span class="sxs-lookup"><span data-stu-id="8966a-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="8966a-113">Użyj funkcji listy eksportu, aby utworzyć listę klientów, którzy przejdą do scentralizowanej dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="8966a-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="8966a-114">Po zakończeniu konsolidacji nie można przywrócić poprzedniego stanu dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="8966a-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="8966a-115">Może być również wymagana akcja klienta.</span><span class="sxs-lookup"><span data-stu-id="8966a-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="8966a-116">Przygotowanie do migracji</span><span class="sxs-lookup"><span data-stu-id="8966a-116">Prepare for migration</span></span>

- <span data-ttu-id="8966a-117">Zaloguj się do Partner Center przy użyciu konta **Transitioning** (to, które zostanie przejść na nowe konto) i przejrzyj wszystkich klientów **i** wszystkie usługi aprowowane dla tych klientów.</span><span class="sxs-lookup"><span data-stu-id="8966a-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="8966a-118">Wyloguj się z tego konta.</span><span class="sxs-lookup"><span data-stu-id="8966a-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="8966a-119">Migrowanie kont klientów</span><span class="sxs-lookup"><span data-stu-id="8966a-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="8966a-120">Zaloguj się do **Partner Center**  przy użyciu **konta Transitioning** (nowe) (to, do których przekierowywujesz klientów).</span><span class="sxs-lookup"><span data-stu-id="8966a-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="8966a-121">Wybierz pozycję **Klienci**.</span><span class="sxs-lookup"><span data-stu-id="8966a-121">Select **Customers**.</span></span>

3. <span data-ttu-id="8966a-122">Wybierz **pozycję Request a reseller relationship (Zażądaj relacji odsprzedawcy).**</span><span class="sxs-lookup"><span data-stu-id="8966a-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="8966a-123">Zostanie wyświetlony domyślny komunikat e-mail do wysłania do klientów.</span><span class="sxs-lookup"><span data-stu-id="8966a-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="8966a-124">Ten komunikat zawiera adres URL z identyfikatorem organizacji unikatowym dla nowego Partner Center konta.</span><span class="sxs-lookup"><span data-stu-id="8966a-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="8966a-125">**Akcja klienta:** Upewnij się, że każdy z aktywnych klientów, których chcesz migrować, odwiedzi ten adres URL.</span><span class="sxs-lookup"><span data-stu-id="8966a-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="8966a-126">Podczas otwierania adresu URL klient jest monitowany o zalogowanie się do portalu usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="8966a-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="8966a-127">Klient korzysta z tego samego identyfikatora organizacji, za pomocą których uzyskuje dostęp do portalu administracyjnego platformy Azure i usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="8966a-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="8966a-128">Po zalogowaniu administrator globalny  dla konta klienta jest monitowany o przesłanie umowy, która daje delegowane uprawnienia administratora do nowego konta CSP.</span><span class="sxs-lookup"><span data-stu-id="8966a-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="8966a-129">Jeśli klient się na to zgadza, zaznacza pole wyboru i wyraża zgodę na autoryzowanie relacji.</span><span class="sxs-lookup"><span data-stu-id="8966a-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="8966a-130">Klienci będą pojawiać się na liście klientów partnera po przesłaniu umowy jeden po drugiej.</span><span class="sxs-lookup"><span data-stu-id="8966a-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="8966a-131">Migrowanie subskrypcji usługi Office 365 i subskrypcji spoza platformy Azure opartych na użyciu</span><span class="sxs-lookup"><span data-stu-id="8966a-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="8966a-132">Po podpisaniu umowy przez klienta możesz ponownie utworzyć jego subskrypcje w ramach dzierżawy scentralizowanego partnera.</span><span class="sxs-lookup"><span data-stu-id="8966a-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="8966a-133">W **Partner Center** wybierz pozycję **Klienci.**</span><span class="sxs-lookup"><span data-stu-id="8966a-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="8966a-134">Otwórz nazwę firmy klienta, którego chcesz zmigrować.</span><span class="sxs-lookup"><span data-stu-id="8966a-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="8966a-135">Wybierz **pozycję Dodaj subskrypcję.**</span><span class="sxs-lookup"><span data-stu-id="8966a-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="8966a-136">Dodaj prawidłowe subskrypcje i liczby licencji z katalogu.</span><span class="sxs-lookup"><span data-stu-id="8966a-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="8966a-137">Zweryfikuj przy użyciu informacji podanych **w tece Przechodzenie z** kont partnerów.</span><span class="sxs-lookup"><span data-stu-id="8966a-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="listy klientów.":::

6. <span data-ttu-id="8966a-139">Wybierz **pozycję Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="8966a-139">Select **Submit.**</span></span>

   <span data-ttu-id="8966a-140">Usługi są teraz udostępniane klientowi z konta **przejścia do** partnera.</span><span class="sxs-lookup"><span data-stu-id="8966a-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="8966a-141">Powtórz te kroki, aby przeprowadzić migrację subskrypcji dla wszystkich dodatkowych klientów.</span><span class="sxs-lookup"><span data-stu-id="8966a-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="8966a-142">Przed przejściem do następnej sekcji upewnij się, że wszystkie subskrypcje klientów istniejące w obszarze Przechodzenie z kont partnerów są ponownie aprowowane w ramach konta Przejścia **do** partnera. </span><span class="sxs-lookup"><span data-stu-id="8966a-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="8966a-143">Partnerzy muszą wstrzymać  subskrypcje na koncie Przechodzenie z dzierżawy partnera w programie Partner Center tego  samego dnia, w który te subskrypcje zostały przenoszone i ustawione w ramach konta Przechodzenie do dzierżawy partnera w Partner Center, aby zagwarantować, że nie wystąpią podwójne rozliczenia.</span><span class="sxs-lookup"><span data-stu-id="8966a-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="8966a-144">Żądania pomocy technicznej zostaną odrzucone w przypadku środków ze względu na nakładanie się rozliczeń, które nie wyłączają prawidłowo **przejścia z** subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="8966a-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="8966a-145">Wyłączanie subskrypcji usługi Office 365 w obszarze Przechodzenie z konta partnera</span><span class="sxs-lookup"><span data-stu-id="8966a-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="8966a-146">Wyłączenie subskrypcji CSP w obszarze **Przechodzenie z** kont partnerów zatrzymuje wszelkie przyszłe rozliczenia.</span><span class="sxs-lookup"><span data-stu-id="8966a-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="8966a-147">Nie trzeba ręcznie wyłączać subskrypcji platformy Azure, ponieważ subskrypcje platformy Azure są automatycznie wyłączane podczas procesu migracji.</span><span class="sxs-lookup"><span data-stu-id="8966a-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="8966a-148">Zaloguj się do konta **Partner Center** **z** konta CSP i przejdź do listy klientów.</span><span class="sxs-lookup"><span data-stu-id="8966a-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="8966a-149">Otwórz klienta z subskrypcjami do wyłączenia, a następnie wybierz pierwszą ofertę do wyłączenia.</span><span class="sxs-lookup"><span data-stu-id="8966a-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="8966a-150">Ustaw wstrzymaną **subskrypcję** na , a następnie wybierz pozycję **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="8966a-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="8966a-151">Wstrzymanie subskrypcji gwarantuje, że podwójne rozliczenia nie będą występować.</span><span class="sxs-lookup"><span data-stu-id="8966a-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="8966a-152">Subskrypcja jest **wyświetlona jako wstrzymana** na liście subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="8966a-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="8966a-153">Powtórz te kroki dla wszystkich subskrypcji w ramach klienta.</span><span class="sxs-lookup"><span data-stu-id="8966a-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="8966a-154">Sprawdź, czy wszystkie są wyświetlane **jako zawieszone.**</span><span class="sxs-lookup"><span data-stu-id="8966a-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="8966a-155">Wybierz następnego klienta z listy i powtórz proces wyłączania wszystkich subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="8966a-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="8966a-156">Migrowanie subskrypcji platformy Azure opartych na użyciu</span><span class="sxs-lookup"><span data-stu-id="8966a-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="8966a-157">W przeciwieństwie do subskrypcji programu CSP usługi Office 365 na platformie Azure nie trzeba migrować ręcznie subskrypcji CSP opartych na użyciu.</span><span class="sxs-lookup"><span data-stu-id="8966a-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="8966a-158">Microsoft Azure pomoc techniczna zmigruje subskrypcje platformy Azure i  wszystkie wdrożone usługi lub zasoby z konta przechodzenia z kont odsprzedawców CSP do konta odsprzedawcy programu **CSP.**</span><span class="sxs-lookup"><span data-stu-id="8966a-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="8966a-159">Podczas tego przejścia nie będzie żadnych zakłóceń w działaniu usługi dla klienta.</span><span class="sxs-lookup"><span data-stu-id="8966a-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="8966a-160">Upewnij się, że konta klientów, które będą mieć zmigrowane subskrypcje platformy Azure, zaakceptowały umowę skojarzoną z nowym kontem **przechodzenia do** programu CSP.</span><span class="sxs-lookup"><span data-stu-id="8966a-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="8966a-161">Użytkownik powiadomi firmę Microsoft o tym, które konta klientów są gotowe do migracji, i poda nazwy firm tych klientów.</span><span class="sxs-lookup"><span data-stu-id="8966a-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="8966a-162">Firma Microsoft migruje subskrypcje platformy Azure oparte na użyciu i powiadamia o zakończeniu migracji.</span><span class="sxs-lookup"><span data-stu-id="8966a-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="8966a-163">Musisz potwierdzić, że subskrypcja platformy Azure w ramach konta  odsprzedawcy przejścia z programu **CSP** jest teraz oznaczona jako Partner Center w sekcji subskrypcje klienta.</span><span class="sxs-lookup"><span data-stu-id="8966a-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="8966a-164">Upewnij się, że subskrypcja platformy Azure w ramach konta  odsprzedawcy przejścia do programu **CSP** ma teraz stan aktywny Partner Center w sekcji subskrypcje klientów.</span><span class="sxs-lookup"><span data-stu-id="8966a-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="8966a-165">Wyłączenie subskrypcji w ramach klienta nie zmienia wyglądu klienta na liście Klienci.</span><span class="sxs-lookup"><span data-stu-id="8966a-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="8966a-166">Obecnie nie ma możliwości usunięcia klientów z listy.</span><span class="sxs-lookup"><span data-stu-id="8966a-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="8966a-167">Partnerzy powinni unikać dodawania subskrypcji z powrotem do tych klientów ze swojego konta **przechodzenia** z konta w przyszłości.</span><span class="sxs-lookup"><span data-stu-id="8966a-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="8966a-168">Powtórz te kroki dla wszystkich subskrypcji w ramach wszystkich  klientów, aby zatrzymać przyszłe opłaty na kontach przejścia z.</span><span class="sxs-lookup"><span data-stu-id="8966a-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="8966a-169">Partner otrzyma jedną końcową fakturę ze środków za liczbę nieużywanych dni między dniem anulowania a ostatnim dniem okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="8966a-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="8966a-170">Po upływie tego ostatecznego okresu rozliczeniowego nie będą generowane żadne przyszłe faktury.</span><span class="sxs-lookup"><span data-stu-id="8966a-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="8966a-171">Dodatkowe informacje</span><span class="sxs-lookup"><span data-stu-id="8966a-171">Additional information</span></span>

- <span data-ttu-id="8966a-172">Wyłączenie subskrypcji z konta przechodzenia z programu **CSP** nie ma wpływu na usługę klienta końcowego, o ile usługa została aprowizowana z konta Przechodzenie do programu **CSP** przed wyłączeniem subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="8966a-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="8966a-173">Klient nie może korzystać z subskrypcji i nie generuje opłat po wstrzymaniu lub anulowaniu.</span><span class="sxs-lookup"><span data-stu-id="8966a-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="8966a-174">Obecnie nie ma możliwości całkowitego usunięcia klienta z **listy** Klienci.</span><span class="sxs-lookup"><span data-stu-id="8966a-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="8966a-175">Partnerzy muszą wstrzymać  subskrypcje na koncie dzierżawy przechodzenia z partnera w programie Partner Center tego  samego dnia, w który te subskrypcje są przenoszone i ustawione w ramach konta Przechodzenie do, aby zagwarantować, że nie wystąpią podwójne rozliczenia.</span><span class="sxs-lookup"><span data-stu-id="8966a-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="8966a-176">Firma Microsoft nie będzie obsługiwać żądań środków ze względu na  nakładanie się rozliczeń, które występują z powodu nieprawidłowo ustawionego przejścia z subskrypcji na wstrzymane.</span><span class="sxs-lookup"><span data-stu-id="8966a-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="8966a-177">Upraszczanie migracji przy użyciu funkcji eksportowania</span><span class="sxs-lookup"><span data-stu-id="8966a-177">Simplify migration using Export</span></span>

<span data-ttu-id="8966a-178">Za pomocą **funkcji Eksportuj** możesz przechwycić subskrypcje, których chcesz użyć w nowej skonsolidowanej strukturze:</span><span class="sxs-lookup"><span data-stu-id="8966a-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="8966a-179">Wybierz **pozycję** Klienci Partner Center, aby wyświetlić listę klientów.</span><span class="sxs-lookup"><span data-stu-id="8966a-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="8966a-180">Otwórz nazwę żądanego klienta.</span><span class="sxs-lookup"><span data-stu-id="8966a-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="8966a-181">Na stronie **Subskrypcje** wybierz pozycję Eksportuj **subskrypcje,** aby wyeksportować szczegóły subskrypcji do pliku programu Excel.</span><span class="sxs-lookup"><span data-stu-id="8966a-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="8966a-182">Użyj tej listy, aby ponownie utworzyć subskrypcje w nowej skonsolidowanej dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="8966a-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="8966a-183">Rejestracja interfejsu API</span><span class="sxs-lookup"><span data-stu-id="8966a-183">API registration</span></span>

<span data-ttu-id="8966a-184">Aby uzyskać więcej informacji na temat rejestracji interfejsu API, zobacz [Konfigurowanie dostępu do interfejsu API w Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="8966a-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8966a-185">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="8966a-185">Next steps</span></span>

- [<span data-ttu-id="8966a-186">Dostawca rozwiązań w chmurze programem regionalne rynki i waluty, w których można sprzedawać oferty CSP</span><span class="sxs-lookup"><span data-stu-id="8966a-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
