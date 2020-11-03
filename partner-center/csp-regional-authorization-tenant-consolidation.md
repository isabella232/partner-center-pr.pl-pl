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
ms.openlocfilehash: 0ae107c005eaf6b8ff8a6d99a91075ebc560cf81
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530250"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="7f1a9-104">Instrukcje dotyczące konsolidacji dzierżawy regionalnej autoryzacji dostawcy usług kryptograficznych</span><span class="sxs-lookup"><span data-stu-id="7f1a9-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="7f1a9-105">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="7f1a9-105">**Applies to**</span></span>

-  <span data-ttu-id="7f1a9-106">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="7f1a9-106">Partner Center</span></span>
-  <span data-ttu-id="7f1a9-107">Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA</span><span class="sxs-lookup"><span data-stu-id="7f1a9-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="7f1a9-108">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="7f1a9-108">**Appropriate roles**</span></span>

- <span data-ttu-id="7f1a9-109">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="7f1a9-109">Global admin</span></span>
- <span data-ttu-id="7f1a9-110">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="7f1a9-110">Admin agent</span></span>

<span data-ttu-id="7f1a9-111">\[Niektóre informacje odnoszą się do wstępnie wydanego produktu, który można w znacznym stopniu modyfikować przed udostępnieniem handlowym.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="7f1a9-112">Firma Microsoft nie udziela żadnych gwarancji, jawnych lub domniemanych, w odniesieniu do informacji podanych w tym miejscu.\]</span><span class="sxs-lookup"><span data-stu-id="7f1a9-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="7f1a9-113">Można skonsolidować dzierżawców dla swojej firmy.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="7f1a9-114">Te instrukcje służą do konsolidacji dzierżawców dla różnych krajów/regionów.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="7f1a9-115">Użytkownik musi mieć świadomość wszystkich zainicjowanych subskrypcji i liczby licencji dla każdego z klientów na koncie, z którego się przechodzi.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="7f1a9-116">Będziesz ponownie obsługiwać te same dokładne subskrypcje z tymi samymi liczbami licencji w ramach nowego centralnego konta CSP w ramach procesu migracji.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="7f1a9-117">Korzystając z funkcji Eksportuj listę, można utworzyć listę klientów, którzy mają przechodzenie do scentralizowanej dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="7f1a9-118">Po zakończeniu konsolidacji nie można przywrócić poprzedniego stanu dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="7f1a9-119">Może być również wymagana akcja klienta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="7f1a9-120">Przygotowanie do migracji</span><span class="sxs-lookup"><span data-stu-id="7f1a9-120">Prepare for migration</span></span>

- <span data-ttu-id="7f1a9-121">Zaloguj się do **Centrum partnerskiego**  przy użyciu konta **przechodzenia** (zostanie ono przenoszone na nowe konto) i przejrzyj wszystkich klientów oraz wszystkie usługi zainicjowane dla tych klientów.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="7f1a9-122">Wyloguj się z tego konta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="7f1a9-123">Migrowanie kont klientów</span><span class="sxs-lookup"><span data-stu-id="7f1a9-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="7f1a9-124">Zaloguj się do **Centrum partnerskiego**  przy użyciu konta **przechodzenia** (nowe) (do którego są przenoszone klienci).</span><span class="sxs-lookup"><span data-stu-id="7f1a9-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="7f1a9-125">Wybierz pozycję **Klienci** .</span><span class="sxs-lookup"><span data-stu-id="7f1a9-125">Select **Customers** .</span></span>

3. <span data-ttu-id="7f1a9-126">Kliknij pozycję **Żądaj relacji odsprzedawcy** .</span><span class="sxs-lookup"><span data-stu-id="7f1a9-126">Click **Request a reseller relationship** .</span></span> <span data-ttu-id="7f1a9-127">Zostanie wyświetlona domyślna wiadomość e-mail do wysłania do klientów.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="7f1a9-128">Ten komunikat zawiera adres URL z unikatowym IDENTYFIKATORem organizacji dla nowego konta Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="7f1a9-129">**Akcja klienta:** Upewnij się, że każdy aktywny klient, który ma zostać zmigrowany, odwiedzi ten adres URL.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="7f1a9-130">Podczas otwierania adresu URL klient zostanie poproszony o zalogowanie się w portalu pakietu Office 365.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="7f1a9-131">Klient loguje się przy użyciu tego samego identyfikatora organizacji, który służy do uzyskiwania dostępu do portali administratorów platformy Azure i pakietu Office 365.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="7f1a9-132">Po zalogowaniu Administrator globalny **konta klienta** zostanie poproszony o przesłanie umowy zapewniającej uprawnienia administratora delegowanego do nowego konta dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="7f1a9-133">Jeśli zgadzają się, klient wybierze pole wyboru i zgadza się na autoryzację relacji.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="7f1a9-134">Po przesłaniu umowy klient zostanie wyświetlony na liście klientów partnera.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="7f1a9-135">Migrowanie subskrypcji pakietu Office 365 i nie korzystających z platformy Azure</span><span class="sxs-lookup"><span data-stu-id="7f1a9-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="7f1a9-136">Po podpisaniu umowy przez klienta możesz ponownie utworzyć swoje subskrypcje w ramach dzierżawy scentralizowanego partnera.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="7f1a9-137">W **centrum partnerskim** wybierz pozycję **klienci** .</span><span class="sxs-lookup"><span data-stu-id="7f1a9-137">From **Partner Center** select **Customers** .</span></span>

3. <span data-ttu-id="7f1a9-138">Otwórz nazwę firmy dla klienta, który ma zostać zmigrowany.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="7f1a9-139">Wybierz pozycję **Dodaj subskrypcję** .</span><span class="sxs-lookup"><span data-stu-id="7f1a9-139">Select **Add subscription** .</span></span>

5. <span data-ttu-id="7f1a9-140">Dodaj prawidłowe subskrypcje i liczby licencji z wykazu.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="7f1a9-141">Sprawdź informacje zawarte w **przejściu z** kont partnerów.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Lista klientów":::

6. <span data-ttu-id="7f1a9-143">Kliknij przycisk **Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="7f1a9-143">Click **Submit.**</span></span>

   <span data-ttu-id="7f1a9-144">Usługi są teraz udostępniane klientowi z **przechodzenia do** konta partnera.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="7f1a9-145">Powtórz te kroki, aby przeprowadzić migrację subskrypcji dla wszystkich dodatkowych klientów.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="7f1a9-146">Przed przejściem do następnej sekcji upewnij się, że wszystkie subskrypcje klienta istniejące w ramach **przejścia z** kont partnerów są ponownie inicjowane w ramach **przejścia do** konta partnera.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="7f1a9-147">Partnerzy muszą zawiesić subskrypcje dotyczące **przejścia z** konta dzierżawy partnera w centrum partnerskim tego samego dnia, w którym te subskrypcje są przenoszone i konfigurowane w ramach **przejścia do** konta dzierżawcy partnera w Centrum partnerskiego w celu zapewnienia podwójnego rozliczania.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="7f1a9-148">Żądania pomocy technicznej będą odrzucane w przypadku kredytów z powodu jakiegokolwiek nakładania się opłat, które wystąpiły od nieprawidłowego wyłączenia **przejścia z** subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="7f1a9-149">Wyłączanie subskrypcji pakietu Office 365 w ramach przejścia z konta partnera</span><span class="sxs-lookup"><span data-stu-id="7f1a9-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="7f1a9-150">Wyłączenie subskrypcji dostawcy usług kryptograficznych w ramach **przejścia z** kont partnerskich powoduje zatrzymanie wszelkich przyszłych rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="7f1a9-151">Nie musisz ręcznie wyłączać subskrypcji platformy Azure, ponieważ subskrypcje platformy Azure są automatycznie wyłączane podczas procesu migracji.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="7f1a9-152">Zaloguj się do **Centrum partnerskiego** przy użyciu **przejścia z** konta CSP i przejdź do listy klient.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="7f1a9-153">Otwórz klienta z subskrypcjami, aby wyłączyć, a następnie wybierz pierwszą ofertę do wyłączenia.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="7f1a9-154">Ustaw subskrypcję na **zawieszone** , a następnie kliknij pozycję **Prześlij** .</span><span class="sxs-lookup"><span data-stu-id="7f1a9-154">Set the subscription to **suspended** , and then click **submit** .</span></span>

   >[!Note]
   ><span data-ttu-id="7f1a9-155">Wstrzymanie subskrypcji gwarantuje, że podwójne rozliczenie nie nastąpi.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="7f1a9-156">Subskrypcja zostanie **wyświetlona** na liście subskrypcje.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="7f1a9-157">Powtórz te kroki dla wszystkich subskrypcji w ramach klienta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="7f1a9-158">Sprawdź, czy wszystkie wyświetlanie zostały **zawieszone.**</span><span class="sxs-lookup"><span data-stu-id="7f1a9-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="7f1a9-159">Wybierz następnego klienta z listy i powtórz proces wyłączania wszystkich subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="7f1a9-160">Migrowanie subskrypcji opartych na użyciu platformy Azure</span><span class="sxs-lookup"><span data-stu-id="7f1a9-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="7f1a9-161">W przeciwieństwie do subskrypcji programu CSP pakietu Office 365, Azure, subskrypcje programu CSP oparte na użyciu nie muszą być migrowane ręcznie.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="7f1a9-162">Obsługa Microsoft Azure przeprowadzi migrację subskrypcji platformy Azure, a także wszystkich wdrożonych usług lub zasobów z **przechodzenia z** kont odsprzedawców programu CSP do **przejścia do** konta odsprzedawcy programu CSP.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="7f1a9-163">W trakcie tego przejścia nie będzie zakłócać działania usługi dla klienta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="7f1a9-164">Upewnij się, że konta klientów, dla których zostały zmigrowane subskrypcje platformy Azure, zaakceptowały umowę, która zostanie skojarzona z nowym **przejściem do** konta dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="7f1a9-165">Powiadomimy firmę Microsoft o tym, które konta klientów są gotowe do migracji, i podają nazwy firmowe tego klienta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="7f1a9-166">Firma Microsoft migruje subskrypcje oparte na użyciu platformy Azure i powiadamia o zakończeniu migracji.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="7f1a9-167">Musisz upewnić się, że subskrypcja platformy Azure w ramach **przejścia z** konta odsprzedawcy dostawcy CSP jest teraz oznaczona jako **zawieszona** w centrum partnerskim w sekcji subskrypcje klienta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="7f1a9-168">Upewnij się, że w ramach subskrypcji platformy Azure w ramach **przejścia do** konta odsprzedawcy CSP jest teraz wyświetlany stan **aktywny** w centrum partnerskim w sekcji subskrypcje klienta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="7f1a9-169">Wyłączenie subskrypcji w ramach klienta nie powoduje zmiany wyglądu klienta na liście klientów.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="7f1a9-170">Obecnie nie ma możliwości usunięcia klientów z listy.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="7f1a9-171">Partnerzy powinni unikać dodawania **subskrypcji z powrotem** do klientów w przyszłości.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="7f1a9-172">Powtórz te kroki dla wszystkich subskrypcji w ramach wszystkich klientów, aby zrezygnować z przyszłych opłat za **przejście z** kont.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="7f1a9-173">Partner otrzyma jedną fakturę ostateczną ze środkiem za liczbę nieużywanych dni między dniem anulowania a ostatnim dniem okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="7f1a9-174">Nie będą generowane żadne przyszłe faktury po upływie ostatecznego okresu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="7f1a9-175">Dodatkowe informacje</span><span class="sxs-lookup"><span data-stu-id="7f1a9-175">Additional information</span></span>

- <span data-ttu-id="7f1a9-176">Wyłączenie **subskrypcji z konta CSP nie** ma wpływu na usługę klienta końcowego, o ile usługa została zainicjowana przy użyciu **przejścia do** konta CSP przed wyłączeniem subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="7f1a9-177">Nie można używać subskrypcji przez klienta i nie generują opłat po wstrzymaniu lub anulowaniu.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="7f1a9-178">Obecnie nie istnieje sposób na całkowite usunięcie klienta z listy **klientów** .</span><span class="sxs-lookup"><span data-stu-id="7f1a9-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="7f1a9-179">Partnerzy muszą zawiesić subskrypcje dotyczące **przejścia z** konta dzierżawcy partnera w centrum partnerskim tego samego dnia, w którym subskrypcje są przenoszone i konfigurowane w ramach **przejścia do** konta w celu zapewnienia podwójnego rozliczania.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="7f1a9-180">Firma Microsoft nie będzie obsługiwać próśb o kredyty ze względu na to, że wystąpiły zmiany w rozliczeniach, które wynikają z nieprawidłowego ustawienia **przejścia z** subskrypcji na zawieszone.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="7f1a9-181">Uproszczenie migracji przy użyciu eksportu</span><span class="sxs-lookup"><span data-stu-id="7f1a9-181">Simplify migration using Export</span></span>

<span data-ttu-id="7f1a9-182">Za pomocą **funkcji eksportu** można przechwytywać subskrypcje, których należy użyć w nowej strukturze skonsolidowanej:</span><span class="sxs-lookup"><span data-stu-id="7f1a9-182">Using the **Export Function** , you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="7f1a9-183">Kliknij pozycję **klienci** w centrum partnerskim, aby wyświetlić listę klientów.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="7f1a9-184">Otwórz żądaną nazwę klienta.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="7f1a9-185">Na stronie **subskrypcje** kliknij pozycję **Eksportuj subskrypcje** , aby wyeksportować szczegóły subskrypcji do pliku programu Excel.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="7f1a9-186">Użyj tej listy, aby ponownie utworzyć subskrypcje w nowej konsolidowanej dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="7f1a9-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="7f1a9-187">Rejestracja interfejsu API</span><span class="sxs-lookup"><span data-stu-id="7f1a9-187">API registration</span></span>

<span data-ttu-id="7f1a9-188">Aby uzyskać więcej informacji na temat rejestracji interfejsu API, zobacz [Konfigurowanie dostępu do interfejsu API w centrum partnerskim](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="7f1a9-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="7f1a9-189">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="7f1a9-189">Next steps</span></span>

- [<span data-ttu-id="7f1a9-190">Program dostawcy rozwiązań w chmurze — rynki regionalne i waluty, w których można sprzedawać oferty CSP</span><span class="sxs-lookup"><span data-stu-id="7f1a9-190">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
