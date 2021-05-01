---
title: Zarządzanie licencjonowaniem w ofertach platformy handlowej
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak skonfigurować licencjonowanie ofert platformy handlowej dla isv i zarządzać nimi.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328019"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="9b838-103">Zarządzanie licencjonowaniem w ofertach platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="9b838-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="9b838-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="9b838-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9b838-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="9b838-105">Global admin</span></span>
- <span data-ttu-id="9b838-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="9b838-106">Account admin</span></span>

<span data-ttu-id="9b838-107">Ten artykuł zawiera informacje na temat procesu konfigurowania oferty w Partner Center, jej Microsoft AppSource, a następnie zarządzania licencjami dla tej oferty.</span><span class="sxs-lookup"><span data-stu-id="9b838-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="9b838-108">Możliwości w tym artykule są obecnie dostępne w publicznej wersji zapoznawczej.</span><span class="sxs-lookup"><span data-stu-id="9b838-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="9b838-109">Zanim rozpoczniesz</span><span class="sxs-lookup"><span data-stu-id="9b838-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="9b838-110">Podstawy komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="9b838-110">Commercial marketplace basics</span></span>

<span data-ttu-id="9b838-111">Przed rozpoczęciem tego procesu należy zapoznać się z podstawami platformy handlowej.</span><span class="sxs-lookup"><span data-stu-id="9b838-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="9b838-112">Artykuły w poniższej tabeli pomogą Ci rozpocząć pracę.</span><span class="sxs-lookup"><span data-stu-id="9b838-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="9b838-113">Temat</span><span class="sxs-lookup"><span data-stu-id="9b838-113">Topic</span></span>  | <span data-ttu-id="9b838-114">Artykuł</span><span class="sxs-lookup"><span data-stu-id="9b838-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="9b838-115">Plany komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="9b838-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="9b838-116">Plany i ceny ofert komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="9b838-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="9b838-117">Oferty komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="9b838-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="9b838-118">Typy ofert</span><span class="sxs-lookup"><span data-stu-id="9b838-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="9b838-119">Konta komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="9b838-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="9b838-120">Tworzenie konta komercyjnej platformy handlowej w Partner Center</span><span class="sxs-lookup"><span data-stu-id="9b838-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="9b838-121">Określanie identyfikatora oferty</span><span class="sxs-lookup"><span data-stu-id="9b838-121">Determine your Offer ID</span></span>

<span data-ttu-id="9b838-122">W poniższych procedurach zostanie wyświetlony monit o wprowadzenie identyfikatora oferty.</span><span class="sxs-lookup"><span data-stu-id="9b838-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="9b838-123">Poślij trochę czasu, aby znaleźć odpowiedni identyfikator oferty, pamiętając o następujących kwestiach:</span><span class="sxs-lookup"><span data-stu-id="9b838-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="9b838-124">Ten identyfikator jest widoczny dla klientów w adresie internetowym oferty marketplace i Azure Resource Manager szablonów, jeśli ma to zastosowanie.</span><span class="sxs-lookup"><span data-stu-id="9b838-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="9b838-125">Identyfikator oferty w połączeniu z identyfikatorem wydawcy musi mieć długość poniżej 40 znaków.</span><span class="sxs-lookup"><span data-stu-id="9b838-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="9b838-126">Użyj tylko małych liter i cyfr.</span><span class="sxs-lookup"><span data-stu-id="9b838-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="9b838-127">Identyfikator oferty może zawierać łączniki i podkreślenia, ale nie może zawierać spacji.</span><span class="sxs-lookup"><span data-stu-id="9b838-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="9b838-128">Na przykład jeśli identyfikatorem wydawcy jest , a po wprowadzeniu adresu `testpublisherid` internetowego oferty będzie to `test-offer-1` `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="9b838-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="9b838-129">Tego identyfikatora nie można zmienić po wybraniu opcji **Utwórz**.</span><span class="sxs-lookup"><span data-stu-id="9b838-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="9b838-130">Określanie aliasu oferty</span><span class="sxs-lookup"><span data-stu-id="9b838-130">Determine your Offer alias</span></span>

<span data-ttu-id="9b838-131">Alias oferty to nazwa używana dla oferty w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9b838-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="9b838-132">Będziesz również potrzebować odpowiedniego aliasu oferty, który jest zgodny z poniższymi wytycznymi:</span><span class="sxs-lookup"><span data-stu-id="9b838-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="9b838-133">Ta nazwa nie jest używana na platformie handlowej i różni się od nazwy oferty i innych wartości widocznych dla klientów.</span><span class="sxs-lookup"><span data-stu-id="9b838-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="9b838-134">Tej nazwy nie można zmienić po wybraniu opcji Utwórz.</span><span class="sxs-lookup"><span data-stu-id="9b838-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="9b838-135">Tworzenie oferty</span><span class="sxs-lookup"><span data-stu-id="9b838-135">Create your offer</span></span>

<span data-ttu-id="9b838-136">Pierwszym krokiem procesu licencjonowania jest utworzenie oferty platformy handlowej.</span><span class="sxs-lookup"><span data-stu-id="9b838-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="9b838-137">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9b838-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="9b838-138">W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/Przegląd.**</span><span class="sxs-lookup"><span data-stu-id="9b838-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="9b838-139">W górnej części strony Przegląd wybierz pozycję Nowa **oferta,** a następnie wybierz pozycję **Dynamics 365 for Customer Engagement & PowerApps.**</span><span class="sxs-lookup"><span data-stu-id="9b838-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="9b838-140">Wprowadź utworzone **wcześniej identyfikator oferty** i **alias** oferty.</span><span class="sxs-lookup"><span data-stu-id="9b838-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="9b838-141">Wybierz **pozycję Utwórz,** aby wygenerować ofertę i kontynuować.</span><span class="sxs-lookup"><span data-stu-id="9b838-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="9b838-142">Wybierz opcje licencjonowania.</span><span class="sxs-lookup"><span data-stu-id="9b838-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="9b838-143">Aby włączyć zarządzanie licencjami dla oferty, wybierz pozycję **Włącz zarządzanie licencjami aplikacji za pośrednictwem usługi Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="9b838-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="9b838-144">Jest to ustawienie raz i nie można go zmienić po opublikowaniu oferty.</span><span class="sxs-lookup"><span data-stu-id="9b838-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="9b838-145">Możesz również umożliwić klientom uruchamianie podstawowych funkcji aplikacji bez licencji i uruchamianie funkcji Premium po zakupie licencji.</span><span class="sxs-lookup"><span data-stu-id="9b838-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="9b838-146">W tym celu wybierz pozycję **Zezwalaj klientom na instalowanie mojej aplikacji,** nawet jeśli licencje nie są przypisane.</span><span class="sxs-lookup"><span data-stu-id="9b838-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="9b838-147">Jeśli nie chcesz, aby Twoja oferta zawierała włączone zarządzanie licencjami, wybierz pozycję Pobierz teraz **(wersja bezpłatna),** Bezpłatna wersja **próbna** lub **Skontaktuj się ze mną.**</span><span class="sxs-lookup"><span data-stu-id="9b838-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="9b838-148">Tworzenie planu</span><span class="sxs-lookup"><span data-stu-id="9b838-148">Create your plan</span></span>

<span data-ttu-id="9b838-149">W tych krokach zdefiniujesz plan lub plany, które chcesz włączyć dla swojej oferty.</span><span class="sxs-lookup"><span data-stu-id="9b838-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="9b838-150">W menu nawigacji po lewej stronie wybierz **pozycję Przegląd planu,** a następnie wybierz **pozycję Utwórz nowy plan.**</span><span class="sxs-lookup"><span data-stu-id="9b838-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="9b838-151">Wprowadź identyfikator **planu i** **nazwę planu,** a następnie wybierz pozycję **Utwórz.**</span><span class="sxs-lookup"><span data-stu-id="9b838-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="9b838-152">Na stronie **Lista planów** wprowadź **opis planu**.</span><span class="sxs-lookup"><span data-stu-id="9b838-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="9b838-153">Aby zapisać opis i zakończyć go później, wybierz **pozycję Zapisz roboczą.**</span><span class="sxs-lookup"><span data-stu-id="9b838-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="9b838-154">Po zakończeniu wybierz pozycję **Przejrzyj i opublikuj**.</span><span class="sxs-lookup"><span data-stu-id="9b838-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="9b838-155">Informacje o planie będą teraz wyświetlane na stronie appsource.microsoft.com w obszarze oferty (sekcja planów).</span><span class="sxs-lookup"><span data-stu-id="9b838-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="9b838-156">Po utworzeniu wszystkich planów dla tej oferty należy skopiować identyfikator usługi każdego planu.</span><span class="sxs-lookup"><span data-stu-id="9b838-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="9b838-157">Wybierz **pozycję Przegląd planu** w górnej części strony Lista planów.</span><span class="sxs-lookup"><span data-stu-id="9b838-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="9b838-158">Skopiuj identyfikator usługi dla każdego planu do bezpiecznej lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="9b838-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="9b838-159">Dodawanie identyfikatorów usług do rozwiązania</span><span class="sxs-lookup"><span data-stu-id="9b838-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="9b838-160">Następnym krokiem jest zaktualizowanie rozwiązania przez dodanie identyfikatorów usług dla każdego skopiowanego planu.</span><span class="sxs-lookup"><span data-stu-id="9b838-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="9b838-161">Aby uzyskać wskazówki dotyczące tego problemu, [zobacz Create an AppSource Package for your solution (Tworzenie pakietu usługi AppSource dla rozwiązania).](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="9b838-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="9b838-162">Przekazywanie pakietu i publikowanie oferty</span><span class="sxs-lookup"><span data-stu-id="9b838-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="9b838-163">W okienku nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa,** a następnie wybierz **pozycję Konfiguracja techniczna.**</span><span class="sxs-lookup"><span data-stu-id="9b838-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="9b838-164">W **obszarze Podstawowy model licencji** wybierz pozycję **Użytkownik.**</span><span class="sxs-lookup"><span data-stu-id="9b838-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="9b838-165">W **obszarze Pakiet CRM** wprowadź adres URL lokalizacji pakietu.</span><span class="sxs-lookup"><span data-stu-id="9b838-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="9b838-166">Użyj innych kart w okienku nawigacji po lewej stronie, aby wprowadzić inne wymagane informacje.</span><span class="sxs-lookup"><span data-stu-id="9b838-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="9b838-167">Gdy wszystko będzie gotowe, wybierz pozycję **Przejrzyj i opublikuj**.</span><span class="sxs-lookup"><span data-stu-id="9b838-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="9b838-168">Po opublikowaniu oferty przejmiemy i zweryfikujemy Twoje informacje.</span><span class="sxs-lookup"><span data-stu-id="9b838-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="9b838-169">W przypadku jakichkolwiek problemów z tym procesem powiadomimy Cię.</span><span class="sxs-lookup"><span data-stu-id="9b838-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="9b838-170">Gdy wszystkie problemy zostaną rozwiązane, otrzymasz powiadomienie o tym, że oferta jest dostępna w usłudze AppSource.</span><span class="sxs-lookup"><span data-stu-id="9b838-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="9b838-171">W tym momencie można ją udostępnić.</span><span class="sxs-lookup"><span data-stu-id="9b838-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="9b838-172">Udostępnij ofertę w Partner Center</span><span class="sxs-lookup"><span data-stu-id="9b838-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="9b838-173">W poniższej procedurze przedstawiono proces tworzenia oferty na żywo w usłudze AppSource.</span><span class="sxs-lookup"><span data-stu-id="9b838-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="9b838-174">Aby dowiedzieć się więcej na temat tego procesu, zobacz [Wprowadzenie do opcji listy](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="9b838-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="9b838-175">Po opublikowaniu oferty jej opublikowanie potrwa 4–6 godzin.</span><span class="sxs-lookup"><span data-stu-id="9b838-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="9b838-176">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9b838-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="9b838-177">W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/Przegląd.**</span><span class="sxs-lookup"><span data-stu-id="9b838-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="9b838-178">Na **stronie** Przegląd znajdź ofertę, która Cię szuka.</span><span class="sxs-lookup"><span data-stu-id="9b838-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="9b838-179">Oferty gotowe do opublikowania będą mieć stan Wersja **zapoznawcza.**</span><span class="sxs-lookup"><span data-stu-id="9b838-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="9b838-180">Wybierz ofertę.</span><span class="sxs-lookup"><span data-stu-id="9b838-180">Select the offer.</span></span>
4. <span data-ttu-id="9b838-181">Na stronie **Omówienie oferty** wybierz pozycję Przejdź **na żywo.**</span><span class="sxs-lookup"><span data-stu-id="9b838-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="9b838-182">Oferta będzie żywa w ciągu 4–6 godzin.</span><span class="sxs-lookup"><span data-stu-id="9b838-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="9b838-183">Aby wyświetlić ofertę w usłudze AppSource, wybierz link **AppSource** w dolnej części **strony Omówienie** oferty.</span><span class="sxs-lookup"><span data-stu-id="9b838-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="9b838-184">**W przypadku ofert z obsługą** licencji: jeśli oferta wymaga sprawdzenia licencji, użytkownicy będą mogli wprowadzić potencjalnego klienta tylko przez kliknięcie pozycji Skontaktuj się ze **mną,** aby móc się z nimi komunikować.</span><span class="sxs-lookup"><span data-stu-id="9b838-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="9b838-185">**W przypadku ofert z włączoną** licencją z opcją instalacji bezpłatnej:  jeśli oferta nie wymaga sprawdzenia licencji, administratorzy zobaczą oprócz opcji Skontaktuj się ze mną przycisk Pobierz **teraz.**</span><span class="sxs-lookup"><span data-stu-id="9b838-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="9b838-186">Użytkownicy, którzy chcą wypróbować bezpłatną opcję instalacji, powinni kliknąć pozycję Pobierz **teraz,** aby zainstalować ofertę w Power Platform administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="9b838-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="9b838-187">Użytkownicy mogą nadal korzystać z funkcji Skontaktuj się ze **mną,** jeśli mają pytania lub chcą podwyżsić plan do planu płatnego.</span><span class="sxs-lookup"><span data-stu-id="9b838-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="9b838-188">Rejestrowanie transakcji w rejestracji transakcji w programie ISV Connect</span><span class="sxs-lookup"><span data-stu-id="9b838-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="9b838-189">Aby można było przypisać licencje do klienta, każda sprzedaż musi być zarejestrowana w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9b838-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="9b838-190">Aby to zrobić, zobacz [Rejestrowanie transakcji.](register-deals.md)</span><span class="sxs-lookup"><span data-stu-id="9b838-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="9b838-191">Zapraszanie klienta</span><span class="sxs-lookup"><span data-stu-id="9b838-191">Invite the customer</span></span>

<span data-ttu-id="9b838-192">Użyj poniższej procedury, aby zaprosić klienta do wzięcia udziału w tej transakcji.</span><span class="sxs-lookup"><span data-stu-id="9b838-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="9b838-193">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9b838-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="9b838-194">W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/Przegląd.**</span><span class="sxs-lookup"><span data-stu-id="9b838-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="9b838-195">W menu nawigacji po lewej stronie wybierz pozycję **Polecenia**, a następnie wybierz pozycję **Rejestracja transakcji.**</span><span class="sxs-lookup"><span data-stu-id="9b838-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="9b838-196">**Odfiltruj przesłane** transakcje, wybierz **kartę W** toku, a następnie wybierz transakcję, której potrzebujesz.</span><span class="sxs-lookup"><span data-stu-id="9b838-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="9b838-197">Na stronie przeglądu tej transakcji wybierz pozycję **Zarządzaj licencjami.**</span><span class="sxs-lookup"><span data-stu-id="9b838-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="9b838-198">W **oknie Zarządzanie licencjami** wybierz klienta z listy **rozwijanej Szczegóły** klienta.</span><span class="sxs-lookup"><span data-stu-id="9b838-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="9b838-199">Jeśli relacja z klientem jeszcze nie istnieje, wybierz **pozycję +Zaproś nowego klienta do wyrażenia zgody.**</span><span class="sxs-lookup"><span data-stu-id="9b838-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="9b838-200">Skopiuj wyświetlony link.</span><span class="sxs-lookup"><span data-stu-id="9b838-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="9b838-201">Wyślij ten link pocztą e-mail do administratora rozliczeń lub administratora globalnego klienta i pomiń go za pomocą tego linku, aby uzyskać dostęp do usługi admin.microsoft.com oraz zaakceptować i autoryzować nawiązywaną relację.</span><span class="sxs-lookup"><span data-stu-id="9b838-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="9b838-202">Relacja nie zostanie ustanowiona, dopóki klient nie wykona tego kroku.</span><span class="sxs-lookup"><span data-stu-id="9b838-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="9b838-203">Aktywowanie i usuwanie licencji oraz zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="9b838-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="9b838-204">Gdy klient autoryzował relację z Toem, możesz rozpocząć dodawanie planów z oferty i przypisywanie licencji do każdego planu.</span><span class="sxs-lookup"><span data-stu-id="9b838-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="9b838-205">W oknie Zarządzanie licencjami dla tej transakcji wybierz **pozycję +Dodaj plan**.</span><span class="sxs-lookup"><span data-stu-id="9b838-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="9b838-206">Wypełnij pola **Plany dla tego rozwiązania** i Liczba **licencji,** a następnie wybierz **pozycję Aktualizuj licencje.**</span><span class="sxs-lookup"><span data-stu-id="9b838-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="9b838-207">Licencje będą dostępne na stronie admin.microsoft.com, aby klienci mogą zarządzać pracownikami i przypisywać je do pracowników.</span><span class="sxs-lookup"><span data-stu-id="9b838-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="9b838-208">Aby zmienić liczbę licencji dla istniejącego planu, wprowadź nową liczbę w polu Liczba licencji, a następnie wybierz pozycję **Aktualizuj licencje.** </span><span class="sxs-lookup"><span data-stu-id="9b838-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="9b838-209">Aby dezaktywować lub usunąć licencje dla transakcji,  wybierz ikonę kosza w polu Akcje, a następnie wybierz pozycję **Aktualizuj licencje**.</span><span class="sxs-lookup"><span data-stu-id="9b838-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9b838-210">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="9b838-210">Next steps</span></span>

[<span data-ttu-id="9b838-211">Zasoby licencjonowania</span><span class="sxs-lookup"><span data-stu-id="9b838-211">Licensing resources</span></span>](support-resources-licensing.md)
