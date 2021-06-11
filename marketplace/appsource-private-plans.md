---
title: Plany prywatne w Microsoft AppSource
description: Konfigurowanie planów prywatnych w Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008591"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="ae321-103">Plany prywatne w Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="ae321-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="ae321-104">Plany prywatne to sposób, w jaki wydawcy zapewniają plany niestandardowe określonym klientom.</span><span class="sxs-lookup"><span data-stu-id="ae321-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="ae321-105">Ta opcja jest teraz dostępna w Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="ae321-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="ae321-106">Plany prywatne można sprzedawać w usłudze AppSource dla ofert  oprogramowania jako usługi (SaaS) z wezwaniem do akcji Pobierz teraz.</span><span class="sxs-lookup"><span data-stu-id="ae321-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="ae321-107">Poproś własnego isv o plan prywatny</span><span class="sxs-lookup"><span data-stu-id="ae321-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="ae321-108">Aby prywatny plan był dostępny w usłudze AppSource, musisz skontaktować się bezpośrednio z isv i wynegocjować niestandardową cenę i specyfikację techniczną.</span><span class="sxs-lookup"><span data-stu-id="ae321-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="ae321-109">Gdy warunki planu prywatnego zostaną zaakceptowane, isv isv create a plan for you and assign it to your organization's tenant ID, which you need to provide.</span><span class="sxs-lookup"><span data-stu-id="ae321-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="ae321-110">Znajdowanie identyfikatora dzierżawy</span><span class="sxs-lookup"><span data-stu-id="ae321-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="ae321-111">W usłudze AppSource w prawym górnym rogu wybierz ikonę profilu konta, a następnie pozycję **Wyświetl dzierżawę.**</span><span class="sxs-lookup"><span data-stu-id="ae321-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="ae321-112">Skopiuj identyfikator dzierżawy i podaj go u isV.</span><span class="sxs-lookup"><span data-stu-id="ae321-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Pokazuje, jak znaleźć identyfikator dzierżawy.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="ae321-114">Znajdowanie planu prywatnego w usłudze AppSource</span><span class="sxs-lookup"><span data-stu-id="ae321-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="ae321-115">Zanim nowy plan prywatny zostanie wyświetlony w usłudze AppSource, może upłynieć do 48 godzin od opublikowania przez isv isv nowego planu prywatnego.</span><span class="sxs-lookup"><span data-stu-id="ae321-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="ae321-116">Aby znaleźć plany prywatne skojarzone z identyfikatorem dzierżawy, wybierz pozycję **Plany prywatne** (ikona blokady) w prawym górnym rogu usługi AppSource.</span><span class="sxs-lookup"><span data-stu-id="ae321-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Wyświetla ikonę blokady (kłódkę) na górnym pasku narzędzi.":::

<span data-ttu-id="ae321-118">Jeśli nie zalogowano się, zostanie wyświetlony monit o jej zalogowanie.</span><span class="sxs-lookup"><span data-stu-id="ae321-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="ae321-119">Następnie możesz kupić plany prywatne skojarzone z identyfikatorem dzierżawy na **karcie Plany i cennik.**</span><span class="sxs-lookup"><span data-stu-id="ae321-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Przedstawia oferty prywatne na karcie plan i cennik.":::

<span data-ttu-id="ae321-121">Jeśli plany prywatne nie są dostępne dla dzierżawy, zostanie wyświetlony komunikat informujący o tym, że nie masz żadnych planów ani ofert prywatnych.</span><span class="sxs-lookup"><span data-stu-id="ae321-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="ae321-122">Kupowanie planu prywatnego</span><span class="sxs-lookup"><span data-stu-id="ae321-122">Purchase a private plan</span></span>

<span data-ttu-id="ae321-123">IsV can include one or more private plans within an offer.</span><span class="sxs-lookup"><span data-stu-id="ae321-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="ae321-124">Każda oferta może mieć zarówno plany publiczne, jak i prywatne, ale plany prywatne są wyświetlane na osobnej stronie oferty dostępnej za pośrednictwem ikony ofert prywatnych (kłódki) w prawym górnym rogu strony.</span><span class="sxs-lookup"><span data-stu-id="ae321-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="ae321-125">Dostępne plany prywatne są wyświetlane na **karcie Plany i cennik.** Plany prywatne mają niebieski wskaźnik.</span><span class="sxs-lookup"><span data-stu-id="ae321-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Wyświetla wskaźnik niebieskiej oferty prywatnej obok ofert prywatnych.":::

<span data-ttu-id="ae321-127">Aby kupić wybrany plan, wybierz pozycję **Pobierz teraz** i wykonaj podane kroki.</span><span class="sxs-lookup"><span data-stu-id="ae321-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae321-128">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="ae321-128">Next steps</span></span>

- [<span data-ttu-id="ae321-129">Co to jest usługa Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="ae321-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
