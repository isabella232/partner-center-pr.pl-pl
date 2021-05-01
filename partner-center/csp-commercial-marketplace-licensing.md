---
title: Zarządzanie licencjonowaniem w ofertach platformy handlowej
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak skonfigurować licencjonowanie dla ofert platformy handlowej dla isV i zarządzać nimi.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284891"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="77fb4-103">Zarządzanie licencjonowaniem w ofertach platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="77fb4-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="77fb4-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="77fb4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="77fb4-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="77fb4-105">Global admin</span></span>
- <span data-ttu-id="77fb4-106">Administrator konta</span><span class="sxs-lookup"><span data-stu-id="77fb4-106">Account admin</span></span>

<span data-ttu-id="77fb4-107">W tym artykule o mowa o procesie konfigurowania oferty w u Partner Center, jej Microsoft AppSource, a następnie zarządzania licencjami dla tej oferty.</span><span class="sxs-lookup"><span data-stu-id="77fb4-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="77fb4-108">Możliwości w tym artykule są obecnie dostępne w publicznej wersji zapoznawczej.</span><span class="sxs-lookup"><span data-stu-id="77fb4-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="77fb4-109">Zanim rozpoczniesz</span><span class="sxs-lookup"><span data-stu-id="77fb4-109">Before you begin</span></span>

<span data-ttu-id="77fb4-110">Przed rozpoczęciem tego procesu należy zapoznać się z poniższymi informacjami.</span><span class="sxs-lookup"><span data-stu-id="77fb4-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="77fb4-111">Zapoznaj się z Azure Marketplace dokumentacją</span><span class="sxs-lookup"><span data-stu-id="77fb4-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="77fb4-112">Poniższe artykuły zawierają informacje, które należy znać przed kontynuowaniem.</span><span class="sxs-lookup"><span data-stu-id="77fb4-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="77fb4-113">Tworzenie oferty Dynamics 365 for Customer Engagement & PowerApps</span><span class="sxs-lookup"><span data-stu-id="77fb4-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="77fb4-114">Tworzenie konta komercyjnej platformy handlowej w Partner Center</span><span class="sxs-lookup"><span data-stu-id="77fb4-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="77fb4-115">Tworzenie identyfikatora oferty</span><span class="sxs-lookup"><span data-stu-id="77fb4-115">Create your Offer ID</span></span>

<span data-ttu-id="77fb4-116">W poniższych procedurach zostanie wyświetlony monit o wprowadzenie identyfikatora oferty.</span><span class="sxs-lookup"><span data-stu-id="77fb4-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="77fb4-117">Poślij teraz trochę czasu, aby wymyślić odpowiedni identyfikator oferty, pamiętając o następujących kwestiach:</span><span class="sxs-lookup"><span data-stu-id="77fb4-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="77fb4-118">Ten identyfikator jest widoczny dla klientów w adresie internetowym oferty marketplace i Azure Resource Manager, jeśli ma to zastosowanie.</span><span class="sxs-lookup"><span data-stu-id="77fb4-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="77fb4-119">Identyfikator oferty w połączeniu z identyfikatorem wydawcy musi mieć długość poniżej 40 znaków.</span><span class="sxs-lookup"><span data-stu-id="77fb4-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="77fb4-120">Użyj tylko małych liter i cyfr.</span><span class="sxs-lookup"><span data-stu-id="77fb4-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="77fb4-121">Identyfikator oferty może zawierać łączniki i podkreślenia, ale nie może zawierać spacji.</span><span class="sxs-lookup"><span data-stu-id="77fb4-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="77fb4-122">Jeśli na przykład identyfikator wydawcy to testpublisherid i po wprowadzeniu ciągu test-offer-1, adres internetowy oferty będzie miał wartość https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="77fb4-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="77fb4-123">Tego identyfikatora nie można zmienić po wybraniu opcji **Utwórz**.</span><span class="sxs-lookup"><span data-stu-id="77fb4-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="77fb4-124">Tworzenie aliasu oferty</span><span class="sxs-lookup"><span data-stu-id="77fb4-124">Create your Offer alias</span></span>

<span data-ttu-id="77fb4-125">Alias oferty to nazwa używana dla oferty w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="77fb4-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="77fb4-126">Będziesz również potrzebować odpowiedniego aliasu oferty, który jest zgodny z poniższymi wytycznymi:</span><span class="sxs-lookup"><span data-stu-id="77fb4-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="77fb4-127">Ta nazwa nie jest używana na platformie handlowej i różni się od nazwy oferty i innych wartości wyświetlanych klientom.</span><span class="sxs-lookup"><span data-stu-id="77fb4-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="77fb4-128">Tej nazwy nie można zmienić po wybraniu opcji Utwórz.</span><span class="sxs-lookup"><span data-stu-id="77fb4-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="77fb4-129">Tworzenie oferty</span><span class="sxs-lookup"><span data-stu-id="77fb4-129">Create your offer</span></span>

<span data-ttu-id="77fb4-130">Pierwszym krokiem procesu licencjonowania jest utworzenie oferty platformy handlowej.</span><span class="sxs-lookup"><span data-stu-id="77fb4-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="77fb4-131">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="77fb4-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="77fb4-132">W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/Przegląd.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="77fb4-133">W górnej części strony Przegląd wybierz pozycję Nowa **oferta,** a następnie wybierz pozycję **Dynamics 365 for Customer Engagement & PowerApps.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="77fb4-134">Wprowadź utworzone **wcześniej identyfikator oferty** i **alias** oferty.</span><span class="sxs-lookup"><span data-stu-id="77fb4-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="77fb4-135">Wybierz **pozycję Utwórz,** aby wygenerować ofertę i kontynuować.</span><span class="sxs-lookup"><span data-stu-id="77fb4-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="77fb4-136">Wybierz opcje licencjonowania.</span><span class="sxs-lookup"><span data-stu-id="77fb4-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="77fb4-137">Aby włączyć zarządzanie licencjami dla oferty, wybierz pozycję **Włącz zarządzanie licencjami aplikacji za pośrednictwem firmy Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="77fb4-138">Jest to ustawienie raz i nie można go zmienić po opublikowaniu oferty.</span><span class="sxs-lookup"><span data-stu-id="77fb4-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="77fb4-139">Możesz również umożliwić klientom uruchamianie podstawowych funkcji aplikacji bez licencji oraz uruchamianie funkcji Premium po zakupie licencji.</span><span class="sxs-lookup"><span data-stu-id="77fb4-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="77fb4-140">W tym celu wybierz pozycję **Zezwalaj klientom na instalowanie mojej aplikacji,** nawet jeśli licencje nie są przypisane.</span><span class="sxs-lookup"><span data-stu-id="77fb4-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="77fb4-141">Jeśli nie chcesz, aby Twoja oferta zawierała włączone zarządzanie licencjami, wybierz pozycję Pobierz teraz **(wersja bezpłatna),** Bezpłatna wersja **próbna** lub **Skontaktuj się ze mną.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="77fb4-142">Tworzenie planu</span><span class="sxs-lookup"><span data-stu-id="77fb4-142">Create your plan</span></span>

<span data-ttu-id="77fb4-143">W tych krokach zdefiniujesz plan lub plany, które chcesz włączyć dla oferty.</span><span class="sxs-lookup"><span data-stu-id="77fb4-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="77fb4-144">W menu nawigacji po lewej stronie wybierz **pozycję Przegląd planu,** a następnie wybierz **pozycję Utwórz nowy plan.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="77fb4-145">Wprowadź **identyfikator planu i** **nazwę planu,** a następnie wybierz pozycję **Utwórz.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="77fb4-146">Na stronie **Lista planów** wprowadź **opis planu**.</span><span class="sxs-lookup"><span data-stu-id="77fb4-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="77fb4-147">Aby zapisać opis i zakończyć go później, wybierz pozycję **Zapisz roboczą.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="77fb4-148">Po zakończeniu wybierz pozycję **Przejrzyj i opublikuj**.</span><span class="sxs-lookup"><span data-stu-id="77fb4-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="77fb4-149">Informacje o planie będą teraz wyświetlane na stronie appsource.microsoft.com w obszarze oferty (sekcja planów).</span><span class="sxs-lookup"><span data-stu-id="77fb4-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="77fb4-150">Po utworzeniu wszystkich planów dla tej oferty należy skopiować identyfikator usługi każdego planu.</span><span class="sxs-lookup"><span data-stu-id="77fb4-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="77fb4-151">Wybierz **pozycję Plan overview** (Omówienie planu) w górnej części strony z listą planów.</span><span class="sxs-lookup"><span data-stu-id="77fb4-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="77fb4-152">Skopiuj identyfikator usługi dla każdego planu do bezpiecznej lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="77fb4-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="77fb4-153">Dodawanie identyfikatorów usług do rozwiązania</span><span class="sxs-lookup"><span data-stu-id="77fb4-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="77fb4-154">Następnym krokiem jest zaktualizowanie rozwiązania przez dodanie identyfikatorów usług dla każdego skopiowanego planu.</span><span class="sxs-lookup"><span data-stu-id="77fb4-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="77fb4-155">Aby uzyskać wskazówki dotyczące tego problemu, zobacz Create an AppSource Package for your solution (Tworzenie [pakietu usługi AppSource dla rozwiązania).](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="77fb4-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="77fb4-156">Przekazywanie pakietu i publikowanie oferty</span><span class="sxs-lookup"><span data-stu-id="77fb4-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="77fb4-157">W okienku nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa,** a następnie wybierz **pozycję Konfiguracja techniczna.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="77fb4-158">W **obszarze Podstawowy model licencji** wybierz pozycję **Użytkownik.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="77fb4-159">W **obszarze Pakiet CRM** wprowadź adres URL lokalizacji pakietu.</span><span class="sxs-lookup"><span data-stu-id="77fb4-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="77fb4-160">Użyj innych kart w okienku nawigacji po lewej stronie, aby wprowadzić inne wymagane informacje.</span><span class="sxs-lookup"><span data-stu-id="77fb4-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="77fb4-161">Gdy wszystko będzie gotowe, wybierz pozycję **Przejrzyj i opublikuj.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="77fb4-162">Po opublikowaniu oferty przejmiemy i zweryfikujemy Twoje informacje.</span><span class="sxs-lookup"><span data-stu-id="77fb4-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="77fb4-163">W przypadku jakichkolwiek problemów z tym procesem powiadomimy Cię.</span><span class="sxs-lookup"><span data-stu-id="77fb4-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="77fb4-164">Gdy wszystkie problemy zostaną rozwiązane, otrzymasz powiadomienie o tym, że oferta jest dostępna w usłudze AppSource.</span><span class="sxs-lookup"><span data-stu-id="77fb4-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="77fb4-165">W tym momencie można ją udostępnić.</span><span class="sxs-lookup"><span data-stu-id="77fb4-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="77fb4-166">Udostępnij ofertę w Partner Center</span><span class="sxs-lookup"><span data-stu-id="77fb4-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="77fb4-167">W poniższej procedurze przedstawiono proces tworzenia oferty na żywo w usłudze AppSource.</span><span class="sxs-lookup"><span data-stu-id="77fb4-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="77fb4-168">Aby dowiedzieć się więcej na temat tego procesu, zobacz [Wprowadzenie do opcji listy](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span><span class="sxs-lookup"><span data-stu-id="77fb4-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="77fb4-169">Po opublikowaniu oferty jej opublikowanie potrwa 4–6 godzin.</span><span class="sxs-lookup"><span data-stu-id="77fb4-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="77fb4-170">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="77fb4-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="77fb4-171">W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/Przegląd.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="77fb4-172">Na **stronie Przegląd** znajdź szukaną ofertę.</span><span class="sxs-lookup"><span data-stu-id="77fb4-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="77fb4-173">Oferty gotowe do opublikowania będą mieć stan Wersja **zapoznawcza.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="77fb4-174">Wybierz ofertę.</span><span class="sxs-lookup"><span data-stu-id="77fb4-174">Select the offer.</span></span>
4. <span data-ttu-id="77fb4-175">Na stronie **Omówienie oferty** wybierz pozycję Przejdź **na żywo.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="77fb4-176">Oferta będzie żywa w ciągu 4–6 godzin.</span><span class="sxs-lookup"><span data-stu-id="77fb4-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="77fb4-177">Aby wyświetlić ofertę oferty w usłudze AppSource, wybierz link **AppSource** w dolnej części **strony Omówienie** oferty.</span><span class="sxs-lookup"><span data-stu-id="77fb4-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="77fb4-178">**W przypadku ofert z włączoną** licencją: jeśli Oferta wymaga sprawdzenia licencji, użytkownicy będą mogli wprowadzić potencjalnego klienta tylko przez kliknięcie pozycji Skontaktuj się ze **mną,** aby móc się z nimi komunikować.</span><span class="sxs-lookup"><span data-stu-id="77fb4-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="77fb4-179">**W przypadku ofert** z włączoną licencją z opcją instalacji bezpłatnej: jeśli oferta nie wymaga sprawdzenia licencji, administratorzy zobaczą przycisk Pobierz **teraz** oprócz opcji Skontaktuj się **ze mną.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="77fb4-180">Użytkownicy, którzy chcą wypróbować bezpłatną opcję instalacji, powinni kliknąć pozycję Pobierz **teraz,** aby zainstalować ofertę w Power Platform administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="77fb4-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="77fb4-181">Użytkownicy mogą nadal używać funkcji Skontaktuj się **ze mną,** jeśli mają pytania lub chcą podwyżsić plan do planu płatnego.</span><span class="sxs-lookup"><span data-stu-id="77fb4-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="77fb4-182">Rejestrowanie transakcji isv connect w DealReg</span><span class="sxs-lookup"><span data-stu-id="77fb4-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="77fb4-183">Następnym krokiem jest zarejestrowanie transakcji.</span><span class="sxs-lookup"><span data-stu-id="77fb4-183">The next step is to register your deal.</span></span> <span data-ttu-id="77fb4-184">Aby to zrobić, zobacz [Rejestrowanie transakcji](https://docs.microsoft.com/partner-center/register-deals).</span><span class="sxs-lookup"><span data-stu-id="77fb4-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="77fb4-185">Zapraszanie klienta</span><span class="sxs-lookup"><span data-stu-id="77fb4-185">Invite the customer</span></span>

<span data-ttu-id="77fb4-186">Użyj poniższej procedury, aby zaprosić klienta do wzięcia udziału w tej transakcji.</span><span class="sxs-lookup"><span data-stu-id="77fb4-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="77fb4-187">Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="77fb4-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="77fb4-188">W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/Przegląd.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="77fb4-189">**Odfiltruj przesłane** transakcje, wybierz **kartę W** toku, a następnie wybierz transakcję, której potrzebujesz.</span><span class="sxs-lookup"><span data-stu-id="77fb4-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="77fb4-190">Na stronie przeglądu tej transakcji wybierz pozycję **Zarządzaj licencjami.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="77fb4-191">W **oknie Zarządzanie licencjami** wybierz klienta z **listy rozwijanej Szczegóły** klienta.</span><span class="sxs-lookup"><span data-stu-id="77fb4-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="77fb4-192">Jeśli relacja z klientem jeszcze nie istnieje, wybierz **pozycję +Zaproś nowego klienta do wyrażenia zgody.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="77fb4-193">Skopiuj wyświetlony link.</span><span class="sxs-lookup"><span data-stu-id="77fb4-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="77fb4-194">Wyślij ten link pocztą e-mail do administratora rozliczeń lub administratora globalnego klienta i użyj go do uzyskania dostępu do usługi admin.microsoft.com oraz zaakceptowania i autoryzowania nawiązywanych relacji.</span><span class="sxs-lookup"><span data-stu-id="77fb4-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="77fb4-195">Relacja nie zostanie ustanowiona, dopóki klient nie wykona tego kroku.</span><span class="sxs-lookup"><span data-stu-id="77fb4-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="77fb4-196">Aktywowanie i usuwanie licencji oraz zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="77fb4-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="77fb4-197">Po nawiązywaniu relacji z klientem możesz rozpocząć dodawanie planów z oferty i przypisywanie licencji do każdego planu.</span><span class="sxs-lookup"><span data-stu-id="77fb4-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="77fb4-198">W oknie Zarządzanie licencjami dla tej transakcji wybierz **pozycję +Dodaj plan**.</span><span class="sxs-lookup"><span data-stu-id="77fb4-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="77fb4-199">Wypełnij pola **Plany dla tego rozwiązania i** Liczba **licencji,** a następnie wybierz **pozycję Aktualizuj licencje.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="77fb4-200">Licencje będą dostępne na stronie admin.microsoft.com, aby klienci mogą zarządzać pracownikami i przypisywać je do pracowników.</span><span class="sxs-lookup"><span data-stu-id="77fb4-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="77fb4-201">Aby zmienić liczbę licencji dla istniejącego planu, wprowadź nową liczbę w polu Liczba licencji, a następnie wybierz **pozycję Aktualizuj licencje.** </span><span class="sxs-lookup"><span data-stu-id="77fb4-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="77fb4-202">Aby dezaktywować lub usunąć licencje dla transakcji,  wybierz ikonę kosza w polu Akcje, a następnie wybierz **pozycję Aktualizuj licencje.**</span><span class="sxs-lookup"><span data-stu-id="77fb4-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>