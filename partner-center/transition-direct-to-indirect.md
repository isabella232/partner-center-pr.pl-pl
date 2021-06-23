---
title: Przełączanie partnera z rozliczeniami bezpośrednimi na odsprzedawcę pośredniego
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak Dostawca rozwiązań w chmurze programu (CSP) może Partner Center, aby przejść z partnera z rozliczeniami bezpośrednimi do odsprzedawcy pośredniego.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 205451a1c42c6538936df49ba8a4314372a94082
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112490057"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="05ffc-103">Zmiana z partnera z rozliczaniem bezpośrednim w programie Cloud Solution Provider (CSP) na odsprzedawcę pośredniego w programie CSP</span><span class="sxs-lookup"><span data-stu-id="05ffc-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="05ffc-104">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="05ffc-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="05ffc-105">Ten artykuł jest przeznaczony dla partnerów rozliczanych bezpośrednio, którzy zdecydowali się przejść na odsprzedawców pośrednich.</span><span class="sxs-lookup"><span data-stu-id="05ffc-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="05ffc-106">Jednak nawet jeśli użytkownik nie podjął jeszcze jawnej decyzji o zarejestrowaniu się jako [](direct-partner-new-requirements.md) odsprzedawca pośredni, partnerzy rozliczani bezpośredni, którzy nie spełniają nowych wymagań programu dla partnera rozliczanego bezpośrednio przez program CSP, zostaną poinformowani przez firmę Microsoft o tym, że ich możliwości dotyczące rachunku bezpośredniego będą [ograniczone.](restricted-direct-bill-capabilities.md)</span><span class="sxs-lookup"><span data-stu-id="05ffc-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="05ffc-107">Od stycznia 2021 r. zostanie dodane nowe wymaganie dotyczące przychodów.</span><span class="sxs-lookup"><span data-stu-id="05ffc-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="05ffc-108">Partnerzy zarejestrowani jako partnerzy z rozliczeniami bezpośrednimi muszą mieć co najmniej 300 000 USD przychodu z programu CSP na poziomie globalnego konta partnera w ciągu poprzednich 12 miesięcy.</span><span class="sxs-lookup"><span data-stu-id="05ffc-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in CSP program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="05ffc-109">Będzie można zarejestrować się w programie odsprzedawcy pośredniego przy użyciu istniejącej dzierżawy z rozliczeniami bezpośrednimi.</span><span class="sxs-lookup"><span data-stu-id="05ffc-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="05ffc-110">Rozpoczęcie pracy</span><span class="sxs-lookup"><span data-stu-id="05ffc-110">Get started</span></span>

1. <span data-ttu-id="05ffc-111">Upewnij się, że Twój profil partnera w Partner Center i Microsoft Partner Network (MPN) są aktualne.</span><span class="sxs-lookup"><span data-stu-id="05ffc-111">Make sure your partner profile in Partner Center and Microsoft Partner Network (MPN) ID are current.</span></span>

2. <span data-ttu-id="05ffc-112">Zaloguj się do Partner Center jako administrator globalny dzierżawy z rozliczeniami bezpośrednimi, z których przechodzisz do odsprzedawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Przegląd.":::

3. <span data-ttu-id="05ffc-114">Przejrzyj szczegóły partnera w formularzu rejestracji.</span><span class="sxs-lookup"><span data-stu-id="05ffc-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Zarejestruj się teraz.":::

4. <span data-ttu-id="05ffc-116">Wybierz pozycję Zarejestruj teraz.</span><span class="sxs-lookup"><span data-stu-id="05ffc-116">Select Enroll now.</span></span> <span data-ttu-id="05ffc-117">Twoja firma odsprzedawcy pośredniego będzie używać tej samej Microsoft Azure Active Directory dzierżawy usługi (Azure AD), która jest w twojej bezpośredniej firmie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-117">Your indirect reseller business will use the same Microsoft Azure Active Directory (Azure AD) tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="05ffc-118">Początkowo ta nowa funkcja przejścia będzie dostępna dla partnerów od daty rocznicy września do grudnia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="05ffc-119">Jeśli nie masz daty rocznicy między wrześniem a grudniem, w tej chwili nie zobaczysz tej możliwości.</span><span class="sxs-lookup"><span data-stu-id="05ffc-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="05ffc-120">Partnerzy z datami rocznic po grudniu 2018 r. zostaną powiadomieni później, gdy funkcja zostanie włączona dla partnerów.</span><span class="sxs-lookup"><span data-stu-id="05ffc-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="05ffc-121">Po zatwierdzeniu rejestracji zaloguj się ponownie do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="05ffc-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="05ffc-122">Zatwierdzenie jest zwykle natychmiastowe, ale może potrwać do pięciu dni roboczych.</span><span class="sxs-lookup"><span data-stu-id="05ffc-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="05ffc-123">Po zatwierdzeniu otrzymasz powiadomienie na adres e-mail określony w obszarze kontaktu podstawowego w formularzu rejestracji.</span><span class="sxs-lookup"><span data-stu-id="05ffc-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="05ffc-124">Możesz również sprawdzić stan rejestracji w obszarze Ustawienia Ustawienia Konta Profil partnera >  >    >   informacje o programie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="05ffc-125">Na stronie **Przegląd** zobaczysz umowę odsprzedawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="05ffc-126">Wybierz **pozycję Zaakceptuj i kontynuuj.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-126">Select **Accept and continue**.</span></span> <span data-ttu-id="05ffc-127">Ta akcja włącza możliwości odsprzedawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="05ffc-128">Po zaakceptowaniu umowy odsprzedawcy pośredniego twój profil  partnera identyfikuje Cię zarówno jako odsprzedawcę bezpośredniego, jak i odsprzedawcę pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Umowa odsprzedawcy pośredniego.":::

> [!IMPORTANT]
> <span data-ttu-id="05ffc-130">Po zarejestrowaniu się jako odsprzedawca pośredni przy użyciu nowej funkcji nie ma możliwości powrotu do dzierżawy z rozliczeniami bezpośrednimi.</span><span class="sxs-lookup"><span data-stu-id="05ffc-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="05ffc-131">Przed zarejestrowaniem się jako odsprzedawca pośredni upewnij się, że w pełni oceniasz potrzeby biznesowe.</span><span class="sxs-lookup"><span data-stu-id="05ffc-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="05ffc-132">Podczas przechodzenia z odsprzedawcy bezpośredniego do odsprzedawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="05ffc-133">W tej fazie będziesz nadal zarządzać potrzebami subskrypcji klientów bezpośrednich, w tym procesem rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="05ffc-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="05ffc-134">Możesz również rozpocząć akceptowanie klientów od dostawcy pośredniego i działanie jako odsprzedawca pośredni.</span><span class="sxs-lookup"><span data-stu-id="05ffc-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Jesteś zarówno bezpośrednim odsprzedawcą, jak i odsprzedawcą pośrednim.":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="05ffc-136">Wyszukiwanie dostawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-136">Find an indirect provider</span></span>

<span data-ttu-id="05ffc-137">Po zarejestrowaniu w lewym okienku sieci zostanie wyświetlony link do dostawców pośrednich.</span><span class="sxs-lookup"><span data-stu-id="05ffc-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="05ffc-138">Jako odsprzedawca pośredni nawiązesz relację z dostawcą pośrednim, który następnie będzie w stanie obsługiwać rozliczenia, kupować produkty dla klientów i infrastrukturę pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="05ffc-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="05ffc-139">Różni dostawcy pośredni oferują różne usługi i pomoc techniczną, dlatego należy ocenić dostawców w swoim obszarze, aby określić, które z nich najlepiej spełniają Twoje potrzeby.</span><span class="sxs-lookup"><span data-stu-id="05ffc-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="05ffc-140">Ogólnie rzecz biorąc, większość dostawców:</span><span class="sxs-lookup"><span data-stu-id="05ffc-140">Generally, most providers will:</span></span>

- <span data-ttu-id="05ffc-141">Zapewnianie szkoleń technicznych i pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="05ffc-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="05ffc-142">Pomoc w reklamie produktów i usług</span><span class="sxs-lookup"><span data-stu-id="05ffc-142">Help you market your products and services</span></span>
- <span data-ttu-id="05ffc-143">Zarządzanie terminami i postanowieniami kredytowymi</span><span class="sxs-lookup"><span data-stu-id="05ffc-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="05ffc-144">Przeszukaj listę oficjalnych dostawców [pośrednich firmy Microsoft.](https://partnercenter.microsoft.com/partner/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="05ffc-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="05ffc-145">Aby dowiedzieć się więcej, przeczytaj  [partnerów z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="05ffc-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="05ffc-146">Akceptowanie zaproszenia do partnerstwa od dostawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="05ffc-147">Po odnalezieniu dostawcy pośredniego dla partnera należy ustanowić partnerstwo z dostawcą pośrednim w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="05ffc-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="05ffc-148">Wybranie dostawcy pośredniego spowoduje wysłanie w wiadomości e-mail linku zaproszenia do partnerstwa, który spowoduje wysłanie do Ciebie zaproszenia w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="05ffc-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="05ffc-149">Upewnij się, że administrator globalny jest Partner Center i obserwuje link zaproszenia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="05ffc-150">Po zaakceptowaniu zaproszenia nazwa dostawcy będzie wyświetlana na liście dostawców pośrednich.</span><span class="sxs-lookup"><span data-stu-id="05ffc-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="05ffc-151">Pozyskiwanie nowych klientów jako odsprzedawca pośredni</span><span class="sxs-lookup"><span data-stu-id="05ffc-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="05ffc-152">Zarówno Ty, jak i Twój dostawca pośredni muszą mieć relacje odsprzedawcy z klientami.</span><span class="sxs-lookup"><span data-stu-id="05ffc-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="05ffc-153">Te relacje odsprzedawcy umożliwiają zarządzanie subskrypcjami i usługami klienta w jego imieniu.</span><span class="sxs-lookup"><span data-stu-id="05ffc-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="05ffc-154">Aby pozyskać nowego klienta, który ma istniejącą dzierżawę usługi Azure AD, możesz zaprosić klienta do ustanowienia relacji odsprzedawcy z Tobem i dostawcą w tym samym czasie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="05ffc-155">Aby utworzyć zaproszenie odsprzedawcy pośredniego:</span><span class="sxs-lookup"><span data-stu-id="05ffc-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="05ffc-156">Wybierz **pozycję Dostawcy pośredni** z Partner Center nav po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="05ffc-157">Wybierz **pozycję Zaproś** nowych klientów, aby zaprosić klienta do nawiązania relacji odsprzedawcy z Tobem i dostawcą pośrednim w tym samym czasie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="05ffc-158">Dostawca musi mieć relację odsprzedawcy z klientem, aby można było przesyłać zamówienia w imieniu klienta, gdy klient chce kupić nowe subskrypcje lub dodać nowe licencje do istniejących subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="05ffc-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="05ffc-159">Na następnej stronie przejrzyj wersję roboczą wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="05ffc-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="05ffc-160">Możesz otworzyć wiadomość roboczą w wiadomości e-mail lub skopiować wiadomość do schowka i wkleić ją do wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="05ffc-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="05ffc-161">Edytuj tekst w wiadomości e-mail, aby powiedzieć, czego potrzebujesz, ale pamiętaj, aby dołączyć link spersonalizowany, aby połączyć klienta bezpośrednio z kontem i kontem dostawcy.</span><span class="sxs-lookup"><span data-stu-id="05ffc-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="05ffc-162">Następnie wybierz pozycję **Done** (Gotowe).</span><span class="sxs-lookup"><span data-stu-id="05ffc-162">Then select **Done**.</span></span>

5. <span data-ttu-id="05ffc-163">Gdy klient autoryzuje Ciebie i Twojego dostawcę jako swoich odsprzedawców rekordów, będziesz mieć uprawnienia administratora do zarządzania ich subskrypcjami, licencjami i użytkownikami w ich imieniu, a twój dostawca pośredni będzie mógł przesyłać zamówienia w ich imieniu.</span><span class="sxs-lookup"><span data-stu-id="05ffc-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="05ffc-164">Aby zarządzać kontem, usługami, użytkownikami i licencjami klienta, rozwiń rekord klienta, wybierając strzałkę w dół obok jego nazwy.</span><span class="sxs-lookup"><span data-stu-id="05ffc-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="05ffc-165">W przeciwieństwie do partnerów rozliczanych bezpośrednio odsprzedawcy pośredni nie mogą tworzyć dzierżaw usługi Azure AD dla nowych klientów w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="05ffc-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="05ffc-166">Dostawca utworzy dzierżawę i określi Cię jako odsprzedawcę pośredniego dla tego klienta.</span><span class="sxs-lookup"><span data-stu-id="05ffc-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="05ffc-167">Dzięki temu klient pojawi się na liście klientów w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="05ffc-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="05ffc-168">Nie będzie można używać funkcji rachunku bezpośredniego do tworzenia zakupów dla klientów, których pozyskasz jako odsprzedawca pośredni.</span><span class="sxs-lookup"><span data-stu-id="05ffc-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="05ffc-169">Zarządzanie klientami z rozliczeniami bezpośrednimi i klientami odsprzedawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="05ffc-170">Inaczej zarządzasz klientami z rozliczeniami bezpośrednimi i klientami odsprzedawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="05ffc-171">Klienci z rozliczeniami bezpośrednimi (rzeczy, których nie będziesz robić jako odsprzedawca pośredni)</span><span class="sxs-lookup"><span data-stu-id="05ffc-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="05ffc-172">Tworzenie zamówień produktów</span><span class="sxs-lookup"><span data-stu-id="05ffc-172">Create orders for products</span></span>
- <span data-ttu-id="05ffc-173">Zarządzanie rezerwacjami platformy Azure</span><span class="sxs-lookup"><span data-stu-id="05ffc-173">Manage Azure reservations</span></span>
- <span data-ttu-id="05ffc-174">Zarządzanie historią zamówień</span><span class="sxs-lookup"><span data-stu-id="05ffc-174">Manage their order history</span></span>
- <span data-ttu-id="05ffc-175">Kupowanie oprogramowania</span><span class="sxs-lookup"><span data-stu-id="05ffc-175">Purchase software</span></span>
- <span data-ttu-id="05ffc-176">Bezpośrednio rozliczaj klientów</span><span class="sxs-lookup"><span data-stu-id="05ffc-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="05ffc-177">Klienci odsprzedawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-177">Indirect reseller customers</span></span>

- <span data-ttu-id="05ffc-178">Twój dostawca pośredni składa zamówienia produktów dla klientów</span><span class="sxs-lookup"><span data-stu-id="05ffc-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="05ffc-179">Zarządzanie licencjami i użytkownikami klientów</span><span class="sxs-lookup"><span data-stu-id="05ffc-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="05ffc-180">Obsługa odnawiania subskrypcji</span><span class="sxs-lookup"><span data-stu-id="05ffc-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="05ffc-181">Aby zidentyfikować klientów nabytych jako partner z rozliczeniami bezpośrednimi</span><span class="sxs-lookup"><span data-stu-id="05ffc-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="05ffc-182">Wybierz pozycję **Klienci**.</span><span class="sxs-lookup"><span data-stu-id="05ffc-182">Select **Customers**.</span></span>

2. <span data-ttu-id="05ffc-183">Wybierz klienta, aby wyświetlić jego szczegóły.</span><span class="sxs-lookup"><span data-stu-id="05ffc-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="05ffc-184">Jeśli ten klient został pozyskany jako partner z  rozliczeniami bezpośrednimi, zobaczysz opcje dodawania lub wyświetlania produktów, a zobaczysz ich subskrypcje. </span><span class="sxs-lookup"><span data-stu-id="05ffc-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="05ffc-185">Jeśli klient ma z Toem relację odsprzedawcy pośredniego, te opcje nie będą dostępne.</span><span class="sxs-lookup"><span data-stu-id="05ffc-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="05ffc-186">Przenoszenie klientów z rozliczeniami bezpośrednimi do dostawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="05ffc-187">Twój dostawca pośredni nie może przesyłać zamówień ani istniejących transferów subskrypcji dla istniejących klientów z rozliczeniami bezpośrednimi, dopóki nie mają z nimi relacji odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="05ffc-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="05ffc-188">Aby ustanowić relację odsprzedawcy między dostawcą pośrednim i istniejącym klientem z rozliczeniami bezpośrednimi, możesz użyć jednej z następujących metod:</span><span class="sxs-lookup"><span data-stu-id="05ffc-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="05ffc-189">Rozszerzenie relacji odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="05ffc-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="05ffc-190">Wysyłanie zaproszenia odsprzedawcy pośredniego do klienta</span><span class="sxs-lookup"><span data-stu-id="05ffc-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="05ffc-191">Szczegółowe omówienie procesu krok po kroku można znaleźć w dokumencie Przejście bezpośrednie [do pośredniego](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="05ffc-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="05ffc-192">Rozszerzenie relacji odsprzedawcy</span><span class="sxs-lookup"><span data-stu-id="05ffc-192">Reseller relationship extension</span></span>

<span data-ttu-id="05ffc-193">Funkcja rozszerzenia relacji odsprzedawcy umożliwia ustanowienie relacji odsprzedawcy między istniejącymi klientami z rozliczeniami bezpośrednimi i dostawcą pośrednim przy użyciu pulpitu Partner Center nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="05ffc-194">Przed rozpoczęciem korzystania z tej funkcji należy pamiętać o następujących elementach:</span><span class="sxs-lookup"><span data-stu-id="05ffc-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="05ffc-195">Ta funkcja jest dostępna tylko dla bezpośrednich partnerów rozliczających się, którzy przeszli na odsprzedawcę pośredniego, ukończyli rejestrację [odsprzedawcy pośredniego.](#get-started)</span><span class="sxs-lookup"><span data-stu-id="05ffc-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="05ffc-196">Tę funkcję można zastosować tylko do istniejących klientów z rozliczeniami bezpośrednimi.</span><span class="sxs-lookup"><span data-stu-id="05ffc-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="05ffc-197">Nie ma zastosowania do klientów [odsprzedawcy pośredniego.](#acquire-new-customers-as-indirect-reseller)</span><span class="sxs-lookup"><span data-stu-id="05ffc-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="05ffc-198">Możesz wybrać tylko dostawcę pośredniego, dla którego [zaakceptowaliśmy zaproszenie partnera od dostawcy pośredniego.](#accept-a-partnership-invitation-from-your-indirect-provider)</span><span class="sxs-lookup"><span data-stu-id="05ffc-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="05ffc-199">Kopia informacji odbiorcy faktury dla tego klienta zostanie udostępnione dostawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="05ffc-200">Dostęp do informacji dla odbiorcy faktury można uzyskać, korzystając ze strony konta dla tego klienta na Partner Center nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="05ffc-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="05ffc-201">Korzystając z funkcji rozszerzenia relacji odsprzedawcy, wyrażasz zgodę na udostępnianie informacji o rachunku dla tego klienta u dostawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="05ffc-202">Dostawca pośredni nie będzie miał delegowanych uprawnień [administracyjnych do](customers-revoke-admin-privileges.md) dzierżawy klienta.</span><span class="sxs-lookup"><span data-stu-id="05ffc-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="05ffc-203">Jeśli dostawca pośredni wymaga delegowanych uprawnień administracyjnych, zamiast tego należy wysłać zaproszenie odsprzedawcy pośredniego do klienta.</span><span class="sxs-lookup"><span data-stu-id="05ffc-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="05ffc-204">Po nawiązce relacji odsprzedawcy dostawca pośredni będzie wyświetlany jako partner CSP dla klienta na stronie Relacje partnerów w centrum [administracyjnym](https://admin.microsoft.com/AdminPortal/Home#/partners) Microsoft 365 i Microsoft Store dla Firm [.](/microsoft-store/work-with-partner-microsoft-store-business)</span><span class="sxs-lookup"><span data-stu-id="05ffc-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="05ffc-205">Aby uniknąć nieporozumień i nieporozumień, umowa partnerska musi poinformować klienta rozliczanego bezpośrednio i uzyskać zgodę, zanim użyjemy funkcji rozszerzenia relacji w celu ustanowienia relacji odsprzedawcy między istniejącym klientem z rozliczeniami bezpośrednimi i dostawcą pośrednim.</span><span class="sxs-lookup"><span data-stu-id="05ffc-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="05ffc-206">Aby użyć tej funkcji w istniejącej dzierżawie klienta:</span><span class="sxs-lookup"><span data-stu-id="05ffc-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="05ffc-207">Zaloguj się do Partner Center jako **agent administracyjny.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-207">Sign in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="05ffc-208">Na stronie **Klienci wybierz** istniejącego klienta i wybierz jego ikonę Szybkie **linki,** aby rozwinąć widok podsumowania klienta.</span><span class="sxs-lookup"><span data-stu-id="05ffc-208">In the **Customers page**, select an existing customer and select its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="05ffc-209">W **obszarze Dostawcy pośredni wybierz** pozycję Przenieś klienta u dostawcy **pośredniego.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-209">Under **Indirect provider(s)**, select **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Przeniesienie klienta do dostawcy pośredniego.":::

4. <span data-ttu-id="05ffc-211">W podręcznym oknie dialogowym wybierz **dostawcę** pośredniego, który ma mieć relację odsprzedawcy z klientem.</span><span class="sxs-lookup"><span data-stu-id="05ffc-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="05ffc-212">Wybierz przycisk **Zapisz i kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="05ffc-212">Select **Save and continue**.</span></span>

6. <span data-ttu-id="05ffc-213">Sprawdź, czy wybrany dostawca pośredni jest pojawiany w **obszarze Dostawcy pośredni.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Dostawca pośredni wymieniony na liście.":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="05ffc-215">Wysyłanie zaproszenia odsprzedawcy pośredniego do klienta</span><span class="sxs-lookup"><span data-stu-id="05ffc-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="05ffc-216">Dostawca pośredni nie może przesyłać zamówień dla istniejących klientów z rozliczeniami bezpośrednimi, dopóki nie mają z nimi relacji odsprzedawcy.</span><span class="sxs-lookup"><span data-stu-id="05ffc-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="05ffc-217">Aby ustanowić relację odsprzedawcy między istniejącymi klientami i dostawcą pośrednim, zaproś klienta przy użyciu zaproszenia odsprzedawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="05ffc-218">Wybierz **pozycję Dostawcy pośredni** z Partner Center nav po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="05ffc-219">Wybierz **pozycję Zaproś** nowych klientów, aby zaprosić klienta do nawiązania relacji odsprzedawcy z Tobem i dostawcą pośrednim w tym samym czasie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="05ffc-220">Dostawca musi mieć relację odsprzedawcy z klientem, aby można było przesyłać zamówienia w imieniu klienta, gdy klient chce kupić nowe subskrypcje lub dodać nowe licencje do istniejących subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="05ffc-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Zaproś nowych klientów.":::

3. <span data-ttu-id="05ffc-222">Na następnej stronie przejrzyj wersję roboczą wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="05ffc-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="05ffc-223">Możesz otworzyć wiadomość roboczą w wiadomości e-mail lub skopiować wiadomość do schowka i wkleić ją do wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="05ffc-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="05ffc-224">Edytuj tekst w wiadomości e-mail, aby powiedzieć, czego potrzebujesz, ale pamiętaj, aby dołączyć link spersonalizowany, aby połączyć klienta bezpośrednio z kontem i kontem dostawcy.</span><span class="sxs-lookup"><span data-stu-id="05ffc-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="05ffc-225">Następnie wybierz pozycję **Done** (Gotowe).</span><span class="sxs-lookup"><span data-stu-id="05ffc-225">Then select **Done**.</span></span>

5. <span data-ttu-id="05ffc-226">Gdy klient autoryzuje Ciebie i Twojego dostawcę jako swoich odsprzedawców rekordów, będziesz mieć uprawnienia administratora do zarządzania ich subskrypcjami, licencjami i użytkownikami w ich imieniu, a twój dostawca pośredni będzie mógł przesyłać zamówienia w ich imieniu.</span><span class="sxs-lookup"><span data-stu-id="05ffc-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="05ffc-227">Aby zarządzać kontem, usługami, użytkownikami i licencjami klienta, rozwiń rekord klienta, wybierając strzałkę w dół obok jego nazwy.</span><span class="sxs-lookup"><span data-stu-id="05ffc-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="05ffc-228">Umowa z Klientem Microsoft akceptacji</span><span class="sxs-lookup"><span data-stu-id="05ffc-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="05ffc-229">Umowa dotycząca platformy Microsoft Cloud obowiązuje do 31 stycznia 2020 r.</span><span class="sxs-lookup"><span data-stu-id="05ffc-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="05ffc-230">Po tej dacie wszyscy klienci, istniejący i nowi, muszą podpisać nową Umowa z Klientem Microsoft [.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="05ffc-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="05ffc-231">W przypadku przechodzenia klientów, jeśli:</span><span class="sxs-lookup"><span data-stu-id="05ffc-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="05ffc-232">**Klient nie zaakceptował jeszcze Umowa z Klientem Microsoft**</span><span class="sxs-lookup"><span data-stu-id="05ffc-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="05ffc-233">Skontaktuj się z dostawcą pośrednim, aby klient [zaakceptował Umowa z Klientem Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="05ffc-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="05ffc-234">**Klient zaakceptował Umowa z Klientem Microsoft z Toem za pośrednictwem Microsoft 365 Administracyjnego firmy**</span><span class="sxs-lookup"><span data-stu-id="05ffc-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="05ffc-235">Akceptacja zostanie zachowana po nawiązce relacji odsprzedawcy z dostawcą pośrednim.</span><span class="sxs-lookup"><span data-stu-id="05ffc-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="05ffc-236">Nie musisz nic robić.</span><span class="sxs-lookup"><span data-stu-id="05ffc-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="05ffc-237">**Klient zaakceptował Umowa z Klientem Microsoft z Tobem za pośrednictwem zaświadczenia partnera**</span><span class="sxs-lookup"><span data-stu-id="05ffc-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="05ffc-238">Akceptacja nie zostanie zachowana.</span><span class="sxs-lookup"><span data-stu-id="05ffc-238">The acceptance will not be retained.</span></span> <span data-ttu-id="05ffc-239">Skontaktuj się z dostawcą [pośrednim, aby zaktualizować akceptację klienta](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="05ffc-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="05ffc-240">Przenoszenie istniejących subskrypcji z rachunku bezpośredniego do dostawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="05ffc-241">W modelu pośrednim programu CSP odsprzedawcy pośredni nie mają relacji rozliczeń z firmą Microsoft.</span><span class="sxs-lookup"><span data-stu-id="05ffc-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="05ffc-242">Zamiast tego odsprzedawcy pośredni uzyskają subskrypcje dla swoich klientów za pośrednictwem swoich dostawców pośrednich.</span><span class="sxs-lookup"><span data-stu-id="05ffc-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="05ffc-243">Podczas przechodzenia z partnera z rozliczeniami bezpośrednimi do odsprzedawcy pośredniego musisz przenieść istniejące subskrypcje, które masz jako partnera z rozliczeniami bezpośrednimi, do dostawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="05ffc-244">W tym celu możesz użyć funkcji samoobsługowego przenoszenia subskrypcji na Partner Center nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="05ffc-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="05ffc-245">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="05ffc-245">Prerequisites</span></span>

- <span data-ttu-id="05ffc-246">Ta funkcja jest dostępna tylko dla partnerów przejściowych, którzy ukończyli rejestrację odsprzedawcy pośredniego przy użyciu istniejących dzierżaw partnerów z rozliczeniami bezpośrednimi.</span><span class="sxs-lookup"><span data-stu-id="05ffc-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="05ffc-247">Przed przeniesieniem subskrypcji skojarzonych z danym klientem partner przejściowy musi przenieść klienta do dostawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="05ffc-248">Klient musi [zaakceptować usługę Umowa z Klientem Microsoft pośrednictwem dostawcy pośredniego.](#microsoft-customer-agreement-acceptance)</span><span class="sxs-lookup"><span data-stu-id="05ffc-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="05ffc-249">Jak przejść do stanu odsprzedawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="05ffc-250">Ta funkcja jest procesem czteroetapowym, w którym:</span><span class="sxs-lookup"><span data-stu-id="05ffc-250">The feature is a four-step process, where:</span></span>

- <span data-ttu-id="05ffc-251">Partner przejściowy tworzy żądanie przeniesienia subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="05ffc-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="05ffc-252">Żądanie zawiera co najmniej jedną istniejącą subskrypcję skojarzoną z tym samym klientem i jest adresowane do dostawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="05ffc-253">Dostawca pośredni przegląda i akceptuje (lub odrzuca) żądanie przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="05ffc-254">Dostawca pośredni sprawdza, czy żądanie przeniesienia zostało ukończone.</span><span class="sxs-lookup"><span data-stu-id="05ffc-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="05ffc-255">Partner przejściowy sprawdza, czy żądanie przeniesienia zostało ukończone.</span><span class="sxs-lookup"><span data-stu-id="05ffc-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="05ffc-256">Transitioning partner (Partner przejściowy)</span><span class="sxs-lookup"><span data-stu-id="05ffc-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="05ffc-257">Możesz również użyć [interfejsu API Partner Center SDK,](/partner-center/develop/manage-customers) aby przenieść istniejące subskrypcje do dostawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="05ffc-258">Pobieranie uprawnień klienta do przeniesienia subskrypcji</span><span class="sxs-lookup"><span data-stu-id="05ffc-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="05ffc-259">Tworzenie transferu klienta</span><span class="sxs-lookup"><span data-stu-id="05ffc-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="05ffc-260">Wycofywanie transferu klienta</span><span class="sxs-lookup"><span data-stu-id="05ffc-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="05ffc-261">Akceptowanie transferu klienta</span><span class="sxs-lookup"><span data-stu-id="05ffc-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="05ffc-262">Odrzucanie przeniesienia klienta</span><span class="sxs-lookup"><span data-stu-id="05ffc-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="05ffc-263">Pobieranie transferów klienta</span><span class="sxs-lookup"><span data-stu-id="05ffc-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="05ffc-264">Uzyskiwanie szczegółów przeniesienia według identyfikatora</span><span class="sxs-lookup"><span data-stu-id="05ffc-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="05ffc-265">Przenoszenie partnera — tworzenie żądania przeniesienia</span><span class="sxs-lookup"><span data-stu-id="05ffc-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="05ffc-266">Aby utworzyć żądanie przeniesienia jako partner przejściowy:</span><span class="sxs-lookup"><span data-stu-id="05ffc-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="05ffc-267">Zaloguj się do Partner Center jako **agent administracyjny.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-267">Sign in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="05ffc-268">Na stronie **Klienci** wybierz odpowiedniego klienta i wybierz ikonę Szybkie linki, aby rozwinąć widok podsumowania klienta.</span><span class="sxs-lookup"><span data-stu-id="05ffc-268">In the **Customers** page, select the intended customer and select the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="05ffc-269">W **obszarze Dostawcy pośredni potwierdź,** że na liście znajduje się zamierzony dostawca pośredni.</span><span class="sxs-lookup"><span data-stu-id="05ffc-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="05ffc-270">Wybierz **pozycję Wyświetl subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-270">Select **View Subscriptions**.</span></span>

5. <span data-ttu-id="05ffc-271">Na **stronie Subskrypcje** poszukaj przeniesienia **subskrypcji**.</span><span class="sxs-lookup"><span data-stu-id="05ffc-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="05ffc-272">W **obszarze Przenoszenie subskrypcji** wybierz pozycję **Zażądaj przeniesienia subskrypcji.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-272">Under **Subscription Transfer**, select **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Zażądaj przeniesienia subskrypcji.":::

7. <span data-ttu-id="05ffc-274">W oknie dialogowym żądania przeniesienia wybierz co najmniej jedną subskrypcję do przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Utwórz żądanie przeniesienia.":::

8. <span data-ttu-id="05ffc-276">Wybierz przycisk **Utwórz**.</span><span class="sxs-lookup"><span data-stu-id="05ffc-276">Select **Create**.</span></span>

9. <span data-ttu-id="05ffc-277">Aktywne żądanie przeniesienia subskrypcji zostanie wyświetlone w obszarze **Przenoszenie subskrypcji.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Lista żądań przeniesienia.":::

10. <span data-ttu-id="05ffc-279">Poinformuj dostawcę pośredniego, że utworzono dla nich żądanie przeniesienia subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="05ffc-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="05ffc-280">Dostawca pośredni — akceptowanie żądania przeniesienia</span><span class="sxs-lookup"><span data-stu-id="05ffc-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="05ffc-281">Aby przejrzeć i zaakceptować żądanie przeniesienia jako dostawca pośredni:</span><span class="sxs-lookup"><span data-stu-id="05ffc-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="05ffc-282">Zaloguj się do Partner Center jako **agent administracyjny** lub agent **sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-282">Sign in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="05ffc-283">Na stronie **Klienci** wybierz odpowiedniego klienta i wybierz jego ikonę Szybkie linki, aby rozwinąć widok podsumowania klienta.</span><span class="sxs-lookup"><span data-stu-id="05ffc-283">In the **Customers** page, select the intended customer and select its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="05ffc-284">W **obszarze Odsprzedawcy pośredni** potwierdź, że partner przejściowy znajduje się na liście.</span><span class="sxs-lookup"><span data-stu-id="05ffc-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="05ffc-285">Wybierz **pozycję Wyświetl subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-285">Select **View Subscriptions**.</span></span>

5. <span data-ttu-id="05ffc-286">Na **stronie Subskrypcje** poszukaj przeniesienia **subskrypcji**.</span><span class="sxs-lookup"><span data-stu-id="05ffc-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Wyświetl żądanie przeniesienia.":::

6. <span data-ttu-id="05ffc-288">W **obszarze Przenoszenie subskrypcji** wybierz żądanie przeniesienia do przejrzenia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-288">Under **Subscription Transfer**, select the transfer request to review.</span></span>

7. <span data-ttu-id="05ffc-289">Wybierz **pozycję Zaakceptuj** (lub **Odrzuć)** zgodnie z potrzebami.</span><span class="sxs-lookup"><span data-stu-id="05ffc-289">Select **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Zaakceptuj żądanie przeniesienia.":::

8. <span data-ttu-id="05ffc-291">Poczekaj na ukończenie żądania przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="05ffc-292">Dostawca pośredni — sprawdzanie, czy żądanie przeniesienia zostało zakończone</span><span class="sxs-lookup"><span data-stu-id="05ffc-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="05ffc-293">Po pomyślnym zakończeniu żądania przeniesienia sprawdź, czy subskrypcje są widoczne w obszarze **Subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="05ffc-294">Poinformuj partnera przejściowego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="05ffc-295">Przenoszenie partnera — sprawdzanie, czy żądanie przeniesienia zostało zakończone</span><span class="sxs-lookup"><span data-stu-id="05ffc-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="05ffc-296">Partner przejściowy powinien wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="05ffc-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="05ffc-297">Zaloguj się do Partner Center jako **agent administracyjny** lub **agent sprzedaży.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-297">Sign in to Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="05ffc-298">Na stronie **Klienci** wybierz odpowiedniego klienta i wybierz ikonę Szybkie **linki,** aby rozwinąć widok podsumowania klienta.</span><span class="sxs-lookup"><span data-stu-id="05ffc-298">In the **Customers** page, select the intended customer and select the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="05ffc-299">Wybierz **pozycję Wyświetl subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-299">Select **View Subscriptions**.</span></span>

4. <span data-ttu-id="05ffc-300">Na **stronie Subskrypcje** poszukaj przeniesienia **subskrypcji**.</span><span class="sxs-lookup"><span data-stu-id="05ffc-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="05ffc-301">Sprawdź, czy żądanie przeniesienia jest oznaczone jako **Ukończono.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="05ffc-302">Sprawdź, czy subskrypcje nie są już wyświetlane jako aktywne na **stronie** Subskrypcje:</span><span class="sxs-lookup"><span data-stu-id="05ffc-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="05ffc-303">Jeśli jest to subskrypcja platformy Azure (MS-AZR-0145P), nie będzie ona już na liście.</span><span class="sxs-lookup"><span data-stu-id="05ffc-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="05ffc-304">Jeśli jest to subskrypcja oparta na licencjach (Office 365, Dynamics, Intune), zostanie ona wymieniona jako **Wstrzymana.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Wstrzymano subskrypcję.":::

### <a name="considerations"></a><span data-ttu-id="05ffc-306">Zagadnienia do rozważenia</span><span class="sxs-lookup"><span data-stu-id="05ffc-306">Considerations</span></span>

- <span data-ttu-id="05ffc-307">**Identyfikator subskrypcji będzie inny po przeniesieniu.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="05ffc-308">Jeśli jest to subskrypcja platformy Azure (MS-AZR-0145P), ponadto będzie ona mieć identyfikator subskrypcji platformy Azure, który jest zachowywany od poprzedniego właściciela i będzie wyświetlany w portalu zarządzania platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="05ffc-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="05ffc-309">**Wiele żądań przeniesienia nie może odwoływać się do tej samej subskrypcji.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="05ffc-310">Po utworzeniu żądania przeniesienia, które obejmuje istniejącą subskrypcję, nie można utworzyć dodatkowych żądań przeniesienia, w tym tej samej subskrypcji, dopóki pierwsze żądanie przeniesienia nie zostanie anulowane.</span><span class="sxs-lookup"><span data-stu-id="05ffc-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="05ffc-311">**Dodatki dla subskrypcji opartych na licencjach muszą być przenoszone wraz z ich subskrypcją podstawową.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="05ffc-312">Jeśli podczas tworzenia żądania przeniesienia wybierzemy istniejącą subskrypcję z co najmniej jednym dodatkim, dodatki zostaną automatycznie uwzględnione w żądaniu przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="05ffc-313">**Zmiany liczby licencji w subskrypcji nie zostaną odzwierciedlone w istniejącym żądaniu przeniesienia.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="05ffc-314">Po utworzeniu żądania przeniesienia, które obejmuje istniejącą subskrypcję, należy unikać aktualizowania liczby licencji subskrypcji (lub skojarzonych dodatków).</span><span class="sxs-lookup"><span data-stu-id="05ffc-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="05ffc-315">Jeśli to zrobisz, nowa ilość nie zostanie odzwierciedlona w żądaniu przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="05ffc-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="05ffc-316">Gdy dostawca pośredni zaakceptuje żądanie przeniesienia, wynikowa subskrypcja będzie mieć starą ilość.</span><span class="sxs-lookup"><span data-stu-id="05ffc-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="05ffc-317">Jeśli chcesz, aby nowa ilość została przeniesiona do dostawcy pośredniego, musisz anulować istniejące żądanie przeniesienia i ponownie utworzyć nowe.</span><span class="sxs-lookup"><span data-stu-id="05ffc-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="05ffc-318">**Nie wszystkie zakupy można przenieść za pomocą samoobsługowego przenoszenia subskrypcji.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="05ffc-319">Obecnie przy użyciu tej funkcji można przenieść tylko subskrypcje usługi O365 i subskrypcje usługi Azure PAYG (MS-AZR-0145P).</span><span class="sxs-lookup"><span data-stu-id="05ffc-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="05ffc-320">Inne zakupy, w tym plany platformy Azure, wystąpienia zarezerwowane platformy Azure, subskrypcje oparte na terminach i subskrypcje SaaS Azure Marketplace nie są obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="05ffc-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="05ffc-321">Na stronie przesyłania żądania przeniesienia zostanie wyświetlony powód, dla którego nie można przenieść subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="05ffc-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="05ffc-322">Aby przenieść te subskrypcje, [](create-a-new-subscription.md#suspend-or-cancel-a-subscription) musisz anulować istniejącą subskrypcję i zakupić nową ofertę dla klienta za pośrednictwem dostawcy pośredniego.</span><span class="sxs-lookup"><span data-stu-id="05ffc-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="05ffc-323">**Nie można przetestować przy użyciu środowiska piaskownicy.**</span><span class="sxs-lookup"><span data-stu-id="05ffc-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="05ffc-324">Rejestrowanie w ramach zachęt odsprzedawcy pośredniego</span><span class="sxs-lookup"><span data-stu-id="05ffc-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="05ffc-325">Po pomyślnym zarejestrowaniu się jako odsprzedawca pośredni w istniejącej dzierżawie partnera z rozliczeniami bezpośrednimi otrzymasz zaproszenie do rejestracji w ramach zachęty odsprzedawcy pośredniego w ciągu 30 dni.</span><span class="sxs-lookup"><span data-stu-id="05ffc-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="05ffc-326">Zaproszenie jest oparte na koncie MPN partnera, które jest obecnie skojarzone z dzierżawą partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="05ffc-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="05ffc-327">Zaproszenie zostanie wysłane na adres e-mail skojarzony z kontem MPN partnera.</span><span class="sxs-lookup"><span data-stu-id="05ffc-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="05ffc-328">Możesz również zarejestrować się w programach zachęt dla rachunku bezpośredniego w tej samej dzierżawie partnera.</span><span class="sxs-lookup"><span data-stu-id="05ffc-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="05ffc-329">Należy zarządzać programami oddzielnie.</span><span class="sxs-lookup"><span data-stu-id="05ffc-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="05ffc-330">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="05ffc-330">Next steps</span></span>

- [<span data-ttu-id="05ffc-331">Dodatkowe informacje na temat zostania odsprzedawcą pośrednim</span><span class="sxs-lookup"><span data-stu-id="05ffc-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="05ffc-332">Nowe wymagania dotyczące partnerów bezpośrednich w programie CSP</span><span class="sxs-lookup"><span data-stu-id="05ffc-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="05ffc-333">Ograniczone możliwości na rachunku bezpośrednim</span><span class="sxs-lookup"><span data-stu-id="05ffc-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
