---
title: Kupowanie ofert komercyjnej platformy handlowej
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób partnerzy programu CSP mogą używać platformy handlowej Partner Center do kupowania przez klientów ofert SaaS od niezależnych dostawców oprogramowania.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147857"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a><span data-ttu-id="2365b-103">Kupowanie produktów na platformie handlowej dla klientów w Partner Center</span><span class="sxs-lookup"><span data-stu-id="2365b-103">Purchase commercial marketplace products for your customers in Partner Center</span></span>


<span data-ttu-id="2365b-104">**Odpowiednie role:** Administrator globalny | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="2365b-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="2365b-105">Jako partner w programie Dostawca rozwiązań w chmurze (CSP) możesz użyć platformy handlowej, aby zakupić dla klientów subskrypcje niektórych produktów Oprogramowania jako usługi (SaaS) oferowanych przez niezależnych dostawców oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="2365b-105">As a partner in the Cloud Solution Provider (CSP) program, you can use the commercial marketplace to purchase subscriptions for your customers to certain Software as a Service (SaaS) products offered by Independent Software Vendors (ISVs).</span></span>

<span data-ttu-id="2365b-106">Oferowanie klientom subskrypcji SaaS od isvów może pomóc w odróżnieniu twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="2365b-106">By offering ISV SaaS subscriptions to your customers, you can help differentiate your business.</span></span> <span data-ttu-id="2365b-107">Możesz również udzielić klientom dostępu do pakietów oprogramowania, które są powiązane z ich konkretnymi potrzebami biznesowymi.</span><span class="sxs-lookup"><span data-stu-id="2365b-107">You can also give customers access to software bundles that address their specific business needs.</span></span> <span data-ttu-id="2365b-108">Licencjami i subskrypcjami tych produktów SaaS na platformie handlowej zarządza się od wydawców ISV tak samo jak licencjami i subskrypcjami produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2365b-108">You manage licenses and subscriptions for these marketplace SaaS products from ISV publishers just as you manage licenses and subscriptions for Microsoft products.</span></span>

<span data-ttu-id="2365b-109">Możesz kupić **subskrypcje** SaaS oparte na licencjach lub **subskrypcje oparte na** użyciu.</span><span class="sxs-lookup"><span data-stu-id="2365b-109">You can purchase either **license-based** SaaS subscriptions or **usage-based** subscriptions.</span></span> <span data-ttu-id="2365b-110">Aby dowiedzieć się więcej o różnicach między rozliczeniami opartymi na licencjach i na użyciu, zobacz [Podstawowe informacje o rozliczeniach.](billing-basics.md)</span><span class="sxs-lookup"><span data-stu-id="2365b-110">To learn more about the difference between license-based and usage-based billing, see [Billing basics](billing-basics.md).</span></span>

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a><span data-ttu-id="2365b-111">Kupowanie opartych na licencjach i mierzonych subskrypcji SaaS w Partner Center</span><span class="sxs-lookup"><span data-stu-id="2365b-111">Purchase license-based and metered SaaS subscriptions in Partner Center</span></span>

<span data-ttu-id="2365b-112">Subskrypcje opartych na licencjach lub mierzonych produktach SaaS oferowanych przez wydawców ISV są kupowane przy użyciu tego samego procesu, który jest procesem zakupu subskrypcji produktów firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2365b-112">You purchase subscriptions for license-based or metered SaaS products offered by ISV publishers using the same process you use to purchase subscriptions for Microsoft products.</span></span>

<span data-ttu-id="2365b-113">Aby kupić subskrypcję SaaS opartą na licencji lub mierzoną w u Partner Center, zobacz Tworzenie, zawieszanie lub [anulowanie subskrypcji klientów.](create-a-new-subscription.md#create-a-new-subscription)</span><span class="sxs-lookup"><span data-stu-id="2365b-113">To purchase a license-based or metered SaaS subscription in Partner Center, see [Create, suspend, or cancel customer subscriptions](create-a-new-subscription.md#create-a-new-subscription).</span></span>

<span data-ttu-id="2365b-114">Możesz również użyć [interfejsów API Partner Center do](/partner-center/develop/) tworzenia subskrypcji platformy handlowej dla klientów.</span><span class="sxs-lookup"><span data-stu-id="2365b-114">You can also use [Partner Center APIs](/partner-center/develop/) to create commercial marketplace subscriptions for your customers.</span></span> <span data-ttu-id="2365b-115">(Aby uzyskać więcej informacji na temat korzystania z Partner Center API, zobacz Tworzenie subskrypcji dla produktów platformy [handlowej).](/partner-center/develop/create-subscription-azure-marketplace-products)</span><span class="sxs-lookup"><span data-stu-id="2365b-115">(For more info on using Partner Center APIs, see [Create a subscription for commercial marketplace products](/partner-center/develop/create-subscription-azure-marketplace-products).)</span></span>

>[!IMPORTANT]
> <span data-ttu-id="2365b-116">Jako partner w programie CSP  możesz kupować oparte na licencjach lub mierzone subskrypcje **SaaS** od wydawców ISV w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2365b-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="2365b-117">Oznacza to, że  możesz kupić dowolną ofertę **SaaS** opartą na licencjach lub taryfowej, która została ci udostępnione przez wydawcę ISV, w tym oferty wyłączne, do których masz dostęp. [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)</span><span class="sxs-lookup"><span data-stu-id="2365b-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="2365b-118">Aby kupić lub zarządzać innymi, komercyjnymi ofertami platformy handlowej od isvs (takimi jak oferty oparte na użyciu obejmujące aplikacje platformy Azure, kontenery lub maszyny wirtualne), musisz przejść do witryny [Azure Portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="2365b-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a><span data-ttu-id="2365b-119">Kupowanie subskrypcji opartych na użyciu w Azure Portal</span><span class="sxs-lookup"><span data-stu-id="2365b-119">Purchase usage-based subscriptions in the Azure portal</span></span>

<span data-ttu-id="2365b-120">W przeciwieństwie do opartych na licencjach subskrypcji SaaS od innych wydawców isv, subskrypcje oparte na użyciu najpierw wymagają od klienta subskrypcji platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="2365b-120">In contrast to license-based SaaS subscriptions from third-party ISV publishers, usage-based subscriptions first require a customer to have an Azure subscription.</span></span> <span data-ttu-id="2365b-121">Rozliczenia dla komercyjnej platformy handlowej zasoby oparte na użyciu są dostępne w ramach subskrypcji platformy Azure klienta.</span><span class="sxs-lookup"><span data-stu-id="2365b-121">Billing for commercial marketplace, usage-based resources falls under the customer's Azure subscription.</span></span> <span data-ttu-id="2365b-122">Gdy klient ma subskrypcję platformy Azure, partner w programie CSP może wykonać następujące kroki, aby kupić dla nich subskrypcję platformy handlowej:</span><span class="sxs-lookup"><span data-stu-id="2365b-122">Once your customer has an Azure subscription, a partner in the CSP program can follow these steps to purchase a commercial marketplace subscription for them:</span></span>

1. <span data-ttu-id="2365b-123">Zaloguj się na Partner Center [nawigacyjnym,](https://partner.microsoft.com/dashboard)a następnie wybierz pozycję **Klienci** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="2365b-123">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left-hand menu.</span></span>

2. <span data-ttu-id="2365b-124">Wybierz określonego klienta, a następnie wybierz **pozycję Subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="2365b-124">Select the specific customer, then select **Subscriptions**.</span></span>  

3. <span data-ttu-id="2365b-125">W obszarze **Subskrypcje oparte na użyciu** wybierz pozycję **Wszystkie zasoby.**</span><span class="sxs-lookup"><span data-stu-id="2365b-125">Under the **Usage-based subscriptions**, select **All resources**.</span></span> <span data-ttu-id="2365b-126">Zostanie on przekierowyny do portalu zarządzania platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="2365b-126">This takes you to the Azure Management portal.</span></span>

4. <span data-ttu-id="2365b-127">W portalu zarządzania platformy Azure wybierz **pozycję Utwórz zasób** z menu po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="2365b-127">In the Azure Management portal, select **Create a resource** from the left-hand menu.</span></span>

5. <span data-ttu-id="2365b-128">Wybierz **pozycję Zobacz** wszystko w górnej części Azure Marketplace listy.</span><span class="sxs-lookup"><span data-stu-id="2365b-128">Select **See all** at the top of the Azure Marketplace list.</span></span>

6. <span data-ttu-id="2365b-129">Aby zawęzić listę, użyj filtrów w górnej części listy Marketplace.</span><span class="sxs-lookup"><span data-stu-id="2365b-129">To narrow your list, use filters at the top of the Marketplace list.</span></span> <span data-ttu-id="2365b-130">Na przykład możesz wybrać pozycję **Microsoft** lub **Partner** z listy rozwijanej Wydawca, aby wyświetlić tylko oferty firmy Microsoft lub te od wydawcy ISV. </span><span class="sxs-lookup"><span data-stu-id="2365b-130">For example, you can select **Microsoft** or **Partner** from the **Publisher** dropdown list to view only offers from Microsoft or those from an ISV publisher.</span></span>

7. <span data-ttu-id="2365b-131">Wybierz określoną ofertę, a następnie wybierz **pozycję Utwórz.**</span><span class="sxs-lookup"><span data-stu-id="2365b-131">Choose a specific offer, then select **Create**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2365b-132">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="2365b-132">Next steps</span></span>

- [<span data-ttu-id="2365b-133">Zarządzanie ofertami komercyjnej platformy handlowej</span><span class="sxs-lookup"><span data-stu-id="2365b-133">Manage commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)