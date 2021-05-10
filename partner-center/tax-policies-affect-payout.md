---
title: Jak zasady podatkowe wpływają na wypłaty dla Azure Marketplace
description: Dowiedz się, jak zasady podatkowe wpływają na wypłaty dla Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686317"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="a9f7d-103">Jak zasady podatkowe wpływają na wypłaty dla Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="a9f7d-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="a9f7d-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="a9f7d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a9f7d-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="a9f7d-105">Global admin</span></span>
- <span data-ttu-id="a9f7d-106">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="a9f7d-106">User management admin</span></span>
- <span data-ttu-id="a9f7d-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="a9f7d-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="a9f7d-108">Wprowadzenie</span><span class="sxs-lookup"><span data-stu-id="a9f7d-108">Introduction</span></span>

<span data-ttu-id="a9f7d-109">Platforma handlowa firmy Microsoft ma globalny zasięg.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="a9f7d-110">Transakcje występują w różnych granicach i w zależności od tego, gdzie znajduje się isv isv i klient, implikacje podatkowe mogą się różnić.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="a9f7d-111">Microsoft AppSource i Azure Marketplace informacji o profilu Partner Center, aby określić kraj isv.isv.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="a9f7d-112">Aby określić kraj klienta, użyj informacji rozliczeniowych klienta lub, jeśli klient znajduje się w Unii Europejskiej, użyjemy dwóch różnych informacji.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="a9f7d-113">Aby lepiej zrozumieć poniższe scenariusze, zapoznaj się z tabelą Szczegóły podatku, w której pokazano, czy firma Microsoft zbiera i płaci podatki w imieniu wydawcy, czy też ta odpowiedzialność należy do wydawcy. [](tax-details-marketplace.md)</span><span class="sxs-lookup"><span data-stu-id="a9f7d-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="a9f7d-114">Wszystkie przykłady wartości sprzedaży i wartości procentowe podatku w tym temacie mają charakter wyłącznie ilustrujący, a nie dokładne wartości.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="a9f7d-115">Transakcje wydawcy w zarządzanym przez firmę Microsoft kraju podatkowym</span><span class="sxs-lookup"><span data-stu-id="a9f7d-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="a9f7d-116">**Scenariusz A** — transakcje, które odbywają się między wydawcą a klientem w kraju podatkowym zarządzanym przez [firmę Microsoft.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="a9f7d-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="a9f7d-117">Te transakcje będą mieć zastosowanie do podatku dodanego w momencie sprzedaży, a firma Microsoft wyśle ten podatek do odpowiedniego kraju.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="a9f7d-118">Żadne podatki nie są potrącone z wypłaty, a obliczenia wypłat są bez podatku.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="a9f7d-119">Zobacz [scenariusz D,](#foreign-publisher-transacts-with-us-customer) aby uzyskać informacje o transakcjach między wydawcą z innego niż USA a klientem w USA.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Przedstawia przepływ pracy dla scenariusza A procesu wypłaty.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="a9f7d-121">Transakcje wydawcy w zarządzanym przez firmę Microsoft kraju podatkowym, w którym opłata za korzystanie z witryny Marketplace to usługa serwisowa</span><span class="sxs-lookup"><span data-stu-id="a9f7d-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="a9f7d-122">Scenariusz **B** — transakcje, które odbywają się między wydawcą w USA (zgodnie z definicją w informacjach o profilu podatkowym w usłudze Partner Center) na klienta w kraju podatkowym zarządzanym przez firmę Microsoft, w którym kraj nakłada podatek na opłatę za korzystanie z witryny Marketplace (usługę w witrynie Marketplace).</span><span class="sxs-lookup"><span data-stu-id="a9f7d-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="a9f7d-123">W tym scenariuszu podatek od opłaty za usługę sklepu jest odejmowany od wypłaty wydawcy.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="a9f7d-125">Transakcje wydawcy w kraju podatkowym zarządzanym przez wydawcę</span><span class="sxs-lookup"><span data-stu-id="a9f7d-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="a9f7d-126">**Scenariusz C** — transakcje, które odbywają się między wydawcą a klientem w zarządzanym przez wydawcę kraju podatkowym, który nie nakłada podatku potrącanego na klientów.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="a9f7d-127">Klienci nie płacą podatku w punkcie sprzedaży i wydawca jest zobowiązani do zapłacenia wszystkich mających zastosowanie podatków.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="a9f7d-128">Aby uzyskać więcej informacji na temat cen specyficznych dla kraju (na przykład w celu przesunięcia przyszłego podatku), zobacz Plany i ceny ofert [platformy handlowej](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="a9f7d-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="a9f7d-130">Transakcje obcego wydawcy z klientem w USA</span><span class="sxs-lookup"><span data-stu-id="a9f7d-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="a9f7d-131">**Scenariusz D** — wszyscy obci wydawcy (zgodnie z definicją w informacjach o profilu podatkowym w systemie Partner Center) w krajach bez usa (zobacz scenariusz [E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)dokonujący sprzedaży klientowi z USA (zgodnie z definicją w adresie konta klienta).</span><span class="sxs-lookup"><span data-stu-id="a9f7d-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="a9f7d-132">Rząd STANÓW Zjednoczonych wymaga, aby firma Microsoft wstrzymała podatek w imieniu wydawcy.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="a9f7d-133">Podatek od wypłaty do wydawcy jest obliczany na podstawie ceny oferty.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Przedstawia przepływ pracy dla scenariusza D procesu wypłaty.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="a9f7d-135">Obcy wydawca z transakcją transakcyjną z klientem w USA</span><span class="sxs-lookup"><span data-stu-id="a9f7d-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="a9f7d-136">**Scenariusz E** — wszyscy obci wydawcy (zgodnie z definicją w informacjach o profilu podatkowym firmy Partner Center) w krajach, w których usa dokonano sprzedaży u klienta z USA (zgodnie z definicją w adresie konta klienta).</span><span class="sxs-lookup"><span data-stu-id="a9f7d-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="a9f7d-137">Rząd STANÓW Zjednoczonych nie wymaga od firmy Microsoft wstrzymywania podatku w imieniu wydawcy.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="a9f7d-139">Obcy wydawca sprzedaje klientowi zarejestrowanego w UE w ramach podatku VAT w kraju zarządzanym przez firmę Microsoft (poza Irlandią)</span><span class="sxs-lookup"><span data-stu-id="a9f7d-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="a9f7d-140">**Scenariusz F** — wszystkie transakcje między wydawcami zewnętrznymi i klientami zarejestrowanymi w podatku VAT w UE (poza Irlandią) w Microsoft-Managed kraju.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="a9f7d-141">Klient nie płaci podatku od sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłaty F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="a9f7d-143">Obcy wydawca sprzedaje klientowi zarejestrowanego w UNII podatku VAT w kraju zarządzanym przez firmę Microsoft (w Niemczech)</span><span class="sxs-lookup"><span data-stu-id="a9f7d-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="a9f7d-144">**Scenariusz G** — wszystkie transakcje między obcymi wydawcami a klientami zarejestrowanymi w ue pod rygorami VAT (w Niemczech) w Microsoft-Managed kraju.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="a9f7d-145">Klient płaci podatku VAT w witrynie Microsoft, a firma Microsoft płaci ten podatek rządowi w Witrynie.</span><span class="sxs-lookup"><span data-stu-id="a9f7d-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Przedstawia przepływ pracy dla scenariusza procesu wypłatY G.":::

## <a name="next-steps"></a><span data-ttu-id="a9f7d-147">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="a9f7d-147">Next steps</span></span>

- [<span data-ttu-id="a9f7d-148">Wydawca — często zadawane pytania</span><span class="sxs-lookup"><span data-stu-id="a9f7d-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="a9f7d-149">Instrukcje dotyczące tworzenia profilów płatności i profilów podatkowych</span><span class="sxs-lookup"><span data-stu-id="a9f7d-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)